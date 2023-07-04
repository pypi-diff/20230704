# Comparing `tmp/ytdld-0.0.1.tar.gz` & `tmp/ytdld-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdld-0.0.1.tar", max compression
+gzip compressed data, was "ytdld-0.0.2.tar", max compression
```

## Comparing `ytdld-0.0.1.tar` & `ytdld-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-07-04 03:34:15.085856 ytdld-0.0.1/LICENSE
--rw-r--r--   0        0        0     2443 2023-07-04 03:52:16.950829 ytdld-0.0.1/README.md
--rw-r--r--   0        0        0      614 2023-07-04 03:35:17.822277 ytdld-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    10347 2023-07-04 05:51:39.924100 ytdld-0.0.1/ytdld.py
--rw-r--r--   0        0        0     3115 1970-01-01 00:00:00.000000 ytdld-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-04 03:34:15.085856 ytdld-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2649 2023-07-04 11:01:18.880854 ytdld-0.0.2/README.md
+-rw-r--r--   0        0        0      614 2023-07-04 10:57:26.364162 ytdld-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10831 2023-07-04 11:00:09.116074 ytdld-0.0.2/ytdld.py
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 ytdld-0.0.2/PKG-INFO
```

### Comparing `ytdld-0.0.1/LICENSE` & `ytdld-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdld-0.0.1/README.md` & `ytdld-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -34,18 +34,22 @@
 ### Pip
  - `pip3 install ytdld` [For Termux]
  - `sudo pip3 install ytdld --break-system-packages` [For Linux]
  - `ytdld`
 
 ### [~] Options
 ```
-usage: ytdld.py [-h] [-t TYPE] [-f FORMAT] [-q QUALITY] [-b]
+usage: ytdld.py [-h] [-u URL] [-d DIRECTORY] [-t TYPE] [-f FORMAT]
+                [-q QUALITY] [-b]
 
 options:
   -h, --help            show this help message and exit
+  -u URL, --url URL     Youtube url of the media
+  -d DIRECTORY, --directory DIRECTORY
+                        Download path, the folder in which media will be saved
   -t TYPE, --type TYPE  Type of the media
   -f FORMAT, --format FORMAT
                         File Format or Extension of the media
   -q QUALITY, --quality QUALITY
                         Resolution or Bitrate the media
   -b, --best            Automatically download the media of best resolution or
                         bitrate
```

### Comparing `ytdld-0.0.1/pyproject.toml` & `ytdld-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=58.0.4",
     "wheel>=0.37.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "ytdld"
-version = "0.0.1"
+version = "0.0.2"
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/KasRoudra/ytdld/"
 include = ["README.md", "LICENSE", "ytdld.py"]
 description = "Just another youtube downloader"
 authors = ["KasRoudra <kasroudrakrd@gmail.com>"]
```

### Comparing `ytdld-0.0.1/ytdld.py` & `ytdld-0.0.2/ytdld.py`

 * *Files 7% similar despite different names*

```diff
@@ -143,14 +143,24 @@
 
 home = getenv("HOME")
 config_file = f"{home}/.config/ytdld/config.json"
 
 argparser = ArgumentParser()
 
 argparser.add_argument(
+    "-u",
+    "--url",
+    help="Youtube url of the media"
+)
+argparser.add_argument(
+    "-d",
+    "--directory",
+    help="Download path, the folder in which media will be saved"
+)
+argparser.add_argument(
     "-t",
     "--type",
     help="Type of the media"
 )
 argparser.add_argument(
     "-f",
     "--format",
@@ -166,19 +176,46 @@
     "--best",
     help="Automatically download the media of best resolution or bitrate",
     action="store_true"
 )
 
 args = argparser.parse_args()
 
+arg_url = args.url
+arg_dir = args.directory
 arg_type = args.type
 arg_format = args.format
 arg_quality = args.quality
 best = args.best
 
+def parse_url():
+    """
+    Check for argument url 
+    If not available ask for url input
+    """
+    url = text("Enter youtube url:").ask() if arg_url is None else arg_url
+    # url = "https://youtube.com/watch?v=dCxSsr5xuL8&feature=share9"
+    if url is None:
+        return
+    elif "https://youtube.com/" in url:
+        ytid = url.split("=")[1].split("&")[0]
+        if not len(ytid)==11:
+            print(f"{error}NotYouTubeURLError: This is not a valid youtube url!")
+            return
+    # https://youtu.be/rdC1_jZtWKE
+    elif "https://youtu.be/" in url:
+        ytid = url.split("/")[-1]
+        if not len(ytid)==11:
+            print(f"{error}NotYouTubeURLError: This is not a valid youtube url!")
+            return
+    else:
+        pass
+    return url
+
+
 def parse_config() -> dict:
     """
     Read config or create one if doesn't exists
     """
     if isfile(config_file):
         with open(config_file, encoding=ENCODING) as conf:
             config = loads(conf.read())
@@ -289,15 +326,15 @@
     return filtered_streams
 
 def download_stream(stream):
     """
     Download video from stream
     """
     config = parse_config()
-    directory = config["directory"]
+    directory = config["directory"] if arg_dir is None else arg_dir
     if not isdir(directory):
         mkdir(directory)
     quality = stream.resolution or stream.abr
     extension = stream.mime_type.split("/")[1]
     filename = f"{stream.title}-{quality}.{extension}"
     print(f"{info}Staring download of {filename}")
     stream.download(output_path=directory)
@@ -307,27 +344,14 @@
 
 def download(url):
     """
     Validate url and show download options
     """
     if url is None:
         return
-    elif "https://youtube.com/" in url:
-        ytid = url.split("=")[1].split("&")[0]
-        if not len(ytid)==11:
-            print(f"{error}NotYouTubeURLError: This is not a valid youtube url!")
-            return
-    # https://youtu.be/rdC1_jZtWKE
-    elif "https://youtu.be/" in url:
-        ytid = url.split("/")[-1]
-        if not len(ytid)==11:
-            print(f"{error}NotYouTubeURLError: This is not a valid youtube url!")
-            return
-    else:
-        pass
     youtube = YouTube(url, on_progress_callback=on_progress)
     streams = youtube.streams
     filtered_streams = filter_streams(streams)
     choices = get_choice(filtered_streams)
     if len(filtered_streams) == 0:
         print(f"{error}NotFoundError: No media matched for config/argument")
         exit()
@@ -347,16 +371,15 @@
 
 def main():
     """
     Entrypoint of script
     """
     try:
         clear(logo=logo)
-        url = text("Enter youtube url:").ask()
-        # url = "https://youtube.com/watch?v=dCxSsr5xuL8&feature=share9"
+        url = parse_url()
         download(url)
     except KeyboardInterrupt:
         print(f"\n{info2}KeyboardInterrupt: Shutting down due to user interrption")
         exit(0)
     except Exception as err:
         print(err)
```

### Comparing `ytdld-0.0.1/PKG-INFO` & `ytdld-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdld
-Version: 0.0.1
+Version: 0.0.2
 Summary: Just another youtube downloader
 Home-page: https://github.com/KasRoudra/ytdld/
 License: MIT
 Author: KasRoudra
 Author-email: kasroudrakrd@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -53,18 +53,22 @@
 ### Pip
  - `pip3 install ytdld` [For Termux]
  - `sudo pip3 install ytdld --break-system-packages` [For Linux]
  - `ytdld`
 
 ### [~] Options
 ```
-usage: ytdld.py [-h] [-t TYPE] [-f FORMAT] [-q QUALITY] [-b]
+usage: ytdld.py [-h] [-u URL] [-d DIRECTORY] [-t TYPE] [-f FORMAT]
+                [-q QUALITY] [-b]
 
 options:
   -h, --help            show this help message and exit
+  -u URL, --url URL     Youtube url of the media
+  -d DIRECTORY, --directory DIRECTORY
+                        Download path, the folder in which media will be saved
   -t TYPE, --type TYPE  Type of the media
   -f FORMAT, --format FORMAT
                         File Format or Extension of the media
   -q QUALITY, --quality QUALITY
                         Resolution or Bitrate the media
   -b, --best            Automatically download the media of best resolution or
                         bitrate
```

