# Comparing `tmp/look_like_scanned-0.2.4.tar.gz` & `tmp/look_like_scanned-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "look_like_scanned-0.2.4.tar", max compression
+gzip compressed data, was "look_like_scanned-0.2.5.tar", max compression
```

## Comparing `look_like_scanned-0.2.4.tar` & `look_like_scanned-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-06-19 06:11:55.870797 look_like_scanned-0.2.4/LICENSE
--rw-r--r--   0        0        0    10326 2023-06-19 06:11:55.870797 look_like_scanned-0.2.4/README.md
--rw-r--r--   0        0        0     1778 2023-06-19 06:11:55.870797 look_like_scanned-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      168 2023-06-19 06:11:55.870797 look_like_scanned-0.2.4/scanner/__init__.py
--rw-r--r--   0        0        0    13653 2023-06-19 06:11:55.870797 look_like_scanned-0.2.4/scanner/scanner.py
--rw-r--r--   0        0        0    11844 1970-01-01 00:00:00.000000 look_like_scanned-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-04 11:39:08.128256 look_like_scanned-0.2.5/LICENSE
+-rw-r--r--   0        0        0    10814 2023-07-04 11:39:08.128256 look_like_scanned-0.2.5/README.md
+-rw-r--r--   0        0        0     1778 2023-07-04 11:39:08.128256 look_like_scanned-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-04 11:39:08.128256 look_like_scanned-0.2.5/scanner/__init__.py
+-rw-r--r--   0        0        0    15319 2023-07-04 11:39:08.128256 look_like_scanned-0.2.5/scanner/scanner.py
+-rw-r--r--   0        0        0    12332 1970-01-01 00:00:00.000000 look_like_scanned-0.2.5/PKG-INFO
```

### Comparing `look_like_scanned-0.2.4/LICENSE` & `look_like_scanned-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `look_like_scanned-0.2.4/README.md` & `look_like_scanned-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 ```shell
 pip install look-like-scanned
 ```
 
 Or to install latest version from GitHub
 ```shell
 git clone https://github.com/navchandar/look-like-scanned.git
+cd look-like-scanned
 pip install poetry
 poetry install
 pip install .
 ```
 
 ### Verify Installation:
 ```shell
@@ -69,14 +70,17 @@
 
 # Convert all PDF files including sub folders
 scanner -i .\tests -f "pdf" -r yes
 
 # Convert all Images including sub folders into one PDF
 scanner -i .\tests -f "image" -r yes
 
+# Convert all PDF files including sub folders and save in black & white format
+scanner -i .\tests -f "pdf" -r yes -b yes
+
 ```
 
 ## Arguments
 
 These are the command-line arguments accepted:
 
 - `-i, --input_folder` : Specifies the input folder to read files from and convert. The default value is the current directory. 
@@ -87,14 +91,17 @@
 
 - `-q, --file_quality` : Specifies the quality of the converted output files. The value must be between 50 and 100. The default value is 95. 
     - Example: `-q 90`
 
 - `-a, --askew` : Controls whether to make the output documents slightly askew or slightly tilted. Accepted values are "yes" or "no". The default value is "yes". 
     - Example: `-a yes` or `--askew no`
 
+- `-b, --black_and_white` : Controls whether to save output documents in black and white format (to make it look like a photocopy) . Accepted values are "yes" or "no". The default value is "no". 
+    - Example: `-b yes` or `--black_and_white no`
+
 - `-r, --recurse` : Allows scripts to find all matching files including subdirectories. Accepted values are "yes" or "no". The default value is "yes". 
     - Example: `-r yes` or `--recurse no`
 
 
 ❗❗ **Note:** ❗❗
 
 - The supported file types are: ".jpg", ".png", ".jpeg", ".webp", ".pdf".
@@ -103,14 +110,16 @@
 
 - Bookmarks / Links / Metadata will be removed when saving the output file.
 
 - Transparency will be removed from png files when converting to pdf.
 
 - Password protected PDF files are not yet supported.
 
+- [Youtube: How to Insert a Signature on a PDF File](http://www.youtube.com/watch?v=FKlAwFcMutY)
+
 
 ## License
  
  [MIT license](LICENSE)
 
 
 ## Support This Project
```

### Comparing `look_like_scanned-0.2.4/pyproject.toml` & `look_like_scanned-0.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "look-like-scanned"
-version = "0.2.4"
+version = "0.2.5"
 description = "Python script to make documents look like they were scanned."
 authors = ["navchandar <12165092+navchandar@users.noreply.github.com>"]
 repository    = "https://github.com/navchandar/look-like-scanned"
 homepage = "https://github.com/navchandar/look-like-scanned"
 readme = "README.md"
 keywords = ["pdf", "scan", "scanner", "image-to-pdf", "pdf-to-scan"]
 packages = [
```

### Comparing `look_like_scanned-0.2.4/scanner/scanner.py` & `look_like_scanned-0.2.5/scanner/scanner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python
 """Module to convert PDF/Images to look like they were scanned"""
 
 import os
 import io
 import random
 import argparse
-import colorama
-from colorama import Fore, Style
+from pathlib import Path
+from importlib import metadata
 import pypdfium2 as pdfium
 from PIL import Image, ImageEnhance
-from pathlib import Path
 from pprint import pprint as pretty_print
+import colorama
+from colorama import Fore, Style
 
 SUPPORTED_IMAGES = ["jpg", "png", "jpeg", "webp"]
 SUPPORTED_DOCS = ["pdf", "PDF"]
 CHOICES = ["y", "yes", "n", "no", "true", "false"]
 
 
 def print_color(text, color):
@@ -78,14 +79,23 @@
         "--recurse",
         type=str.lower,
         choices=CHOICES,
         default="no",
         help="Recurse in all sub folders to find matching files and convert them (default: no)",
     )
 
+    parser.add_argument(
+        "-b",
+        "--black_and_white",
+        type=str.lower,
+        choices=CHOICES,
+        default="no",
+        help="Make output documents black and white. Make it look like a photocopy (default: no)",
+    )
+
     return parser.parse_args()
 
 
 def get_input_folder(args):
     """
     Gets the input folder from the command-line argument.
     If argument not provided, returns current working directory as input folder
@@ -101,41 +111,49 @@
 
 
 def get_quality(args):
     """Return the output file quality from command-line argument"""
     return args.file_quality
 
 
+def _is_true(arg):
+    """Return True in boolean type if given argument string is true or yes"""
+    return arg.lower().startswith(("y", "t"))
+
+
 def get_askew(args):
     """Return if output file should have skewed pages"""
-    return args.askew.lower().startswith(("y", "t"))
+    return _is_true(args.askew)
 
 
 def get_recurse(args):
     """Return if input files should be searched within sub folders"""
-    return args.recurse.lower().startswith(("y", "t"))
+    return _is_true(args.recurse)
+
+
+def get_blackandwhite(args):
+    """Return if output files should look like a photocopy"""
+    return _is_true(args.black_and_white)
 
 
 def get_file_type(args):
     """Get file type and supported documents based on input arguments"""
     if args.file_type_or_name:
         file_type = args.file_type_or_name.lower()
         if file_type == "image":
             return "image", SUPPORTED_IMAGES
-        elif any(
+        if any(
             f.endswith(file_type) or file_type.endswith(f) for f in SUPPORTED_IMAGES
         ):
             return "image", [args.file_type_or_name]
-        elif any(
-            f.endswith(file_type) or file_type.endswith(f) for f in SUPPORTED_DOCS
-        ):
+        if any(f.endswith(file_type) or file_type.endswith(f) for f in SUPPORTED_DOCS):
             return "pdf", [args.file_type_or_name]
-    else:
-        print("Defaulting to find pdf files")
-        return "pdf", SUPPORTED_DOCS
+    # if none of the above scenarios match, default to PDFs
+    print("Defaulting to find pdf files")
+    return "pdf", SUPPORTED_DOCS
 
 
 def human_size(num, suffix="B"):
     """Return file size in a human readable format"""
     for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
         if abs(num) < 1024.0:
             return f"{num:3.1f}{unit}{suffix}"
@@ -184,15 +202,29 @@
     """Rotate PIL Image object with given angle value"""
     rotated_image = image.rotate(
         angle, resample=Image.BICUBIC, expand=True, fillcolor=(255, 255, 255)
     )
     return rotated_image
 
 
-def _convert_pdf_pages_to_jpg_list(pdf_path, image_quality=100, askew=True):
+def black_and_white_image(image):
+    """Make image black and white like a photocopy"""
+    bw_image = image.convert("L")
+    # Adjust the contrast level
+    enhancer = ImageEnhance.Contrast(bw_image)
+    bw_image = enhancer.enhance(random.uniform(1.2, 1.5))
+    return bw_image
+
+
+def _convert_pdf_pages_to_jpg_list(
+    pdf_path,
+    image_quality=100,
+    askew=True,
+    blackandwhite=False,
+):
     """
     Reads given pdf file and reads all pages and converts them to image objects
     """
     images_list = []
     doc = pdfium.PdfDocument(pdf_path)
     for page in doc:
         # increase render resolution for better scanned image quality
@@ -207,14 +239,18 @@
         enhancer = ImageEnhance.Brightness(image)
         image = enhancer.enhance(random.uniform(1.01, 1.02))
 
         # Rotate every image by a small random angle
         if askew:
             image = rotate_image(image, random.uniform(-0.55, 0.55))
 
+        # Make image black and white like a photocopy
+        if blackandwhite:
+            image = black_and_white_image(image)
+
         image = _change_image_to_byte_buffer(image)
         images_list.append(image)
         page.close()
     doc.close()
     return images_list
 
 
@@ -290,15 +326,15 @@
         energy_saved = f"{energy_saved:.2f} Mega Watt hours"
 
     if pages_scanned > 0:
         savings = f"\nYou just saved {energy_saved} energy by avoiding printing {pages_scanned} pages of paper!\n"
         print_color(savings, "Green")
 
 
-def convert_images_to_pdf(input_image_list, image_quality, askew):
+def convert_images_to_pdf(input_image_list, image_quality, askew, blackandwhite):
     """Converts all image files in a folder to PDF"""
     images_list = []
     output_pdf_path = None
     if input_image_list:
         # Output pdf name will be the fetched from first Image's name
         output_pdf_path = os.path.splitext(input_image_list[0])[0] + "_output.pdf"
         for image_path in input_image_list:
@@ -310,55 +346,69 @@
                     # reduce image quality a little bit
                     image = reduce_image_quality(image, image_quality)
 
                     # Rotate every image by a small random angle
                     if askew:
                         image = rotate_image(image, random.uniform(-0.75, 0.75))
 
+                    # Make image black and white like a photocopy
+                    if blackandwhite:
+                        image = black_and_white_image(image)
+
                     image = _change_image_to_byte_buffer(image)
                     images_list.append(image)
                 except Exception as err:
                     print_color(f"Error converting file {image_path} :- {err}", "Red")
 
         pages_scanned = _save_image_obj_to_pdf(images_list, output_pdf_path)
         _calc_energy_savings(pages_scanned)
     return output_pdf_path
 
 
-def convert_pdf_to_scanned(pdf_list, image_quality, askew):
+def convert_pdf_to_scanned(pdf_list, image_quality, askew, blackandwhite):
     """
     Converts PDF files into scanned PDF files
     """
     output_file_list = []
     pages_scanned = 0
     for pdf_path in pdf_list:
         if files_exists(pdf_path):
             try:
                 output_path = _add_suffix(pdf_path)
-                images = _convert_pdf_pages_to_jpg_list(pdf_path, image_quality, askew)
+                images = _convert_pdf_pages_to_jpg_list(
+                    pdf_path, image_quality, askew, blackandwhite
+                )
                 pages_scanned += _save_image_obj_to_pdf(images, output_path)
                 output_file_list.append(output_path)
             except Exception as err:
                 print_color(f"Error converting file {pdf_path} :- {err}", "Red")
 
     _calc_energy_savings(pages_scanned)
     return output_file_list
 
 
+def print_version():
+    """prints the version number of the module"""
+    version = metadata.version("look-like-scanned")
+    print_color(f"Scanner version: {version}", "Green")
+
+
 def find_matching_files(input_folder, file_type_list, recurse=False):
     """
     Find files in the given input folder and filter only matching file types.
     If recurse is True, this method will identify all matching files in all subdirectories.
     """
     files_list = []
     try:
         path = Path(input_folder)
         for file in path.iterdir():
             if file.is_file() and file.suffix.lower().lstrip(".") in file_type_list:
                 files_list.append(str(file.absolute()))
+            elif file.is_file() and file.name in file_type_list:
+                files_list.append(str(file.absolute()))
             elif recurse and file.is_dir():
                 files_list.extend(find_matching_files(file, file_type_list, recurse))
     except FileNotFoundError as err:
         print_color(f"Input folder not found: {input_folder}", "red")
     except PermissionError as err:
         print_color(f"Permission denied: {input_folder}", "red")
     except Exception as err:
@@ -370,39 +420,44 @@
     """Method to help sort file paths based on level"""
     directories = path.split(os.path.sep)
     return len(directories)
 
 
 def main():
     """Get input arguments and run the script"""
+    print_version()
     args = parse_args()
 
     # Gather input arguments from command-line
     input_folder = get_input_folder(args)
     quality = get_quality(args)
     askew = get_askew(args)
     recurse = get_recurse(args)
+    blackandwhite = get_blackandwhite(args)
     doc_type, file_type_list = get_file_type(args)
 
-    print_color(f"{quality=} {recurse=} {askew=} {doc_type=} {file_type_list=}", "Cyan")
+    print_color(
+        f"{quality=} {recurse=} {askew=} {blackandwhite=} {doc_type=} {file_type_list=}",
+        "Cyan",
+    )
 
     # Gather the input files based on the arguments
     files_list = find_matching_files(input_folder, file_type_list, recurse)
     # Sort file paths so output gets saved in top level directory
     files_list = sorted(files_list, key=sort_by_top_level_directory)
 
     print_color(f"\nMatching Files Found: {len(files_list)}", "Blue")
     pretty_print(files_list)
 
     # Convert the files found into output files
     pdf_path = None
     if doc_type == "image":
-        pdf_path = convert_images_to_pdf(files_list, quality, askew)
+        pdf_path = convert_images_to_pdf(files_list, quality, askew, blackandwhite)
     elif doc_type == "pdf":
-        pdf_path = convert_pdf_to_scanned(files_list, quality, askew)
+        pdf_path = convert_pdf_to_scanned(files_list, quality, askew, blackandwhite)
     else:
         print_color("Error: Unsupported file format!", "Red")
 
     if pdf_path:
         print("The Output PDF files saved at:")
         pretty_print(pdf_path)
     else:
```

### Comparing `look_like_scanned-0.2.4/PKG-INFO` & `look_like_scanned-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: look-like-scanned
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python script to make documents look like they were scanned.
 Home-page: https://github.com/navchandar/look-like-scanned
 Keywords: pdf,scan,scanner,image-to-pdf,pdf-to-scan
 Author: navchandar
 Author-email: 12165092+navchandar@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -57,14 +57,15 @@
 ```shell
 pip install look-like-scanned
 ```
 
 Or to install latest version from GitHub
 ```shell
 git clone https://github.com/navchandar/look-like-scanned.git
+cd look-like-scanned
 pip install poetry
 poetry install
 pip install .
 ```
 
 ### Verify Installation:
 ```shell
@@ -102,14 +103,17 @@
 
 # Convert all PDF files including sub folders
 scanner -i .\tests -f "pdf" -r yes
 
 # Convert all Images including sub folders into one PDF
 scanner -i .\tests -f "image" -r yes
 
+# Convert all PDF files including sub folders and save in black & white format
+scanner -i .\tests -f "pdf" -r yes -b yes
+
 ```
 
 ## Arguments
 
 These are the command-line arguments accepted:
 
 - `-i, --input_folder` : Specifies the input folder to read files from and convert. The default value is the current directory. 
@@ -120,14 +124,17 @@
 
 - `-q, --file_quality` : Specifies the quality of the converted output files. The value must be between 50 and 100. The default value is 95. 
     - Example: `-q 90`
 
 - `-a, --askew` : Controls whether to make the output documents slightly askew or slightly tilted. Accepted values are "yes" or "no". The default value is "yes". 
     - Example: `-a yes` or `--askew no`
 
+- `-b, --black_and_white` : Controls whether to save output documents in black and white format (to make it look like a photocopy) . Accepted values are "yes" or "no". The default value is "no". 
+    - Example: `-b yes` or `--black_and_white no`
+
 - `-r, --recurse` : Allows scripts to find all matching files including subdirectories. Accepted values are "yes" or "no". The default value is "yes". 
     - Example: `-r yes` or `--recurse no`
 
 
 ❗❗ **Note:** ❗❗
 
 - The supported file types are: ".jpg", ".png", ".jpeg", ".webp", ".pdf".
@@ -136,14 +143,16 @@
 
 - Bookmarks / Links / Metadata will be removed when saving the output file.
 
 - Transparency will be removed from png files when converting to pdf.
 
 - Password protected PDF files are not yet supported.
 
+- [Youtube: How to Insert a Signature on a PDF File](http://www.youtube.com/watch?v=FKlAwFcMutY)
+
 
 ## License
  
  [MIT license](LICENSE)
 
 
 ## Support This Project
```

