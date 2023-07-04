# Comparing `tmp/hay_say_common-0.1.2.tar.gz` & `tmp/hay_say_common-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hay_say_common-0.1.2.tar", last modified: Sat Jul  1 04:46:00 2023, max compression
+gzip compressed data, was "hay_say_common-0.1.3.tar", last modified: Tue Jul  4 15:41:07 2023, max compression
```

## Comparing `hay_say_common-0.1.2.tar` & `hay_say_common-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-07-01 04:46:00.811364 hay_say_common-0.1.2/
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)    11358 2023-04-13 03:14:23.000000 hay_say_common-0.1.2/LICENSE
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      856 2023-07-01 04:46:00.811364 hay_say_common-0.1.2/PKG-INFO
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      192 2023-04-08 03:11:32.000000 hay_say_common-0.1.2/README.md
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      805 2023-07-01 04:45:32.000000 hay_say_common-0.1.2/pyproject.toml
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       38 2023-07-01 04:46:00.811364 hay_say_common-0.1.2/setup.cfg
-drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-07-01 04:46:00.811364 hay_say_common-0.1.2/src/
-drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-07-01 04:46:00.811364 hay_say_common-0.1.2/src/hay_say_common/
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      965 2023-07-01 04:32:16.000000 hay_say_common-0.1.2/src/hay_say_common/__init__.py
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     7291 2023-06-26 03:44:42.000000 hay_say_common-0.1.2/src/hay_say_common/file_integration.py
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     2444 2023-07-01 04:39:54.000000 hay_say_common-0.1.2/src/hay_say_common/server_utility.py
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     2202 2023-07-01 04:31:55.000000 hay_say_common-0.1.2/src/hay_say_common/utility.py
-drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-07-01 04:46:00.811364 hay_say_common-0.1.2/src/hay_say_common.egg-info/
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      856 2023-07-01 04:46:00.000000 hay_say_common-0.1.2/src/hay_say_common.egg-info/PKG-INFO
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      378 2023-07-01 04:46:00.000000 hay_say_common-0.1.2/src/hay_say_common.egg-info/SOURCES.txt
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)        1 2023-07-01 04:46:00.000000 hay_say_common-0.1.2/src/hay_say_common.egg-info/dependency_links.txt
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       52 2023-07-01 04:46:00.000000 hay_say_common-0.1.2/src/hay_say_common.egg-info/requires.txt
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       15 2023-07-01 04:46:00.000000 hay_say_common-0.1.2/src/hay_say_common.egg-info/top_level.txt
+drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-07-04 15:41:07.520235 hay_say_common-0.1.3/
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)    11358 2023-04-13 03:14:23.000000 hay_say_common-0.1.3/LICENSE
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      856 2023-07-04 15:41:07.520235 hay_say_common-0.1.3/PKG-INFO
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      192 2023-04-08 03:11:32.000000 hay_say_common-0.1.3/README.md
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      805 2023-07-04 15:38:59.000000 hay_say_common-0.1.3/pyproject.toml
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       38 2023-07-04 15:41:07.520235 hay_say_common-0.1.3/setup.cfg
+drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-07-04 15:41:07.520235 hay_say_common-0.1.3/src/
+drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-07-04 15:41:07.520235 hay_say_common-0.1.3/src/hay_say_common/
+-rw-r--r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      984 2023-07-03 12:37:37.000000 hay_say_common-0.1.3/src/hay_say_common/__init__.py
+-rw-r--r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     7972 2023-07-03 02:32:43.000000 hay_say_common-0.1.3/src/hay_say_common/file_integration.py
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     2432 2023-07-01 04:57:44.000000 hay_say_common-0.1.3/src/hay_say_common/server_utility.py
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     2186 2023-07-01 04:57:44.000000 hay_say_common-0.1.3/src/hay_say_common/utility.py
+drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-07-04 15:41:07.520235 hay_say_common-0.1.3/src/hay_say_common.egg-info/
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      856 2023-07-04 15:41:07.000000 hay_say_common-0.1.3/src/hay_say_common.egg-info/PKG-INFO
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      378 2023-07-04 15:41:07.000000 hay_say_common-0.1.3/src/hay_say_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)        1 2023-07-04 15:41:07.000000 hay_say_common-0.1.3/src/hay_say_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       52 2023-07-04 15:41:07.000000 hay_say_common-0.1.3/src/hay_say_common.egg-info/requires.txt
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       15 2023-07-04 15:41:07.000000 hay_say_common-0.1.3/src/hay_say_common.egg-info/top_level.txt
```

### Comparing `hay_say_common-0.1.2/LICENSE` & `hay_say_common-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hay_say_common-0.1.2/PKG-INFO` & `hay_say_common-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hay_say_common
-Version: 0.1.2
+Version: 0.1.3
 Summary: Constants and methods that are shared between the Hay Say UI and various Docker containers it communicates with.
 Author-email: HydrusBeta <hydrusgamma@gmail.com>
 Project-URL: Homepage, https://github.com/hydrusbeta/hay_say_common
 Project-URL: Bug Tracker, https://github.com/hydrusbeta/hay_say_common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hay_say_common-0.1.2/pyproject.toml` & `hay_say_common-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hay_say_common"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
 	{name = "HydrusBeta", email="hydrusgamma@gmail.com"},
 ]
 description = "Constants and methods that are shared between the Hay Say UI and various Docker containers it communicates with."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `hay_say_common-0.1.2/src/hay_say_common/__init__.py` & `hay_say_common-0.1.3/src/hay_say_common/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     METADATA_FILENAME,
     TIMESTAMP_FORMAT,
     MAX_FILES_PER_CACHE_FOLDER,
     CACHE_FORMAT,
     CACHE_EXTENSION,
     CACHE_MIMETYPE,
     model_dirs,
+    character_dir,
     read_metadata,
     write_metadata,
     read_audio_from_cache,
     save_audio_to_cache,
     write_audio_file,
     count_audio_cache_files,
     delete_oldest_cache_file,
```

### Comparing `hay_say_common-0.1.2/src/hay_say_common/file_integration.py` & `hay_say_common-0.1.3/src/hay_say_common/file_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 ROOT_DIR = os.path.join(os.path.expanduser('~'), 'hay_say')
 AUDIO_FOLDER = os.path.join(ROOT_DIR, 'audio_cache')
 RAW_DIR = os.path.join(AUDIO_FOLDER, 'raw')
 PREPROCESSED_DIR = os.path.join(AUDIO_FOLDER, 'preprocessed')
 OUTPUT_DIR = os.path.join(AUDIO_FOLDER, 'output')
 POSTPROCESSED_DIR = os.path.join(AUDIO_FOLDER, 'postprocessed')
+MODELS_DIR = os.path.join(ROOT_DIR, 'models')
 METADATA_FILENAME = 'metadata.json'
 TIMESTAMP_FORMAT = '%Y/%m/%d %H:%M:%S.%f'
 MAX_FILES_PER_CACHE_FOLDER = 25
 
 if os.path.exists(AUDIO_FOLDER):
     if not os.path.exists(RAW_DIR):
         os.mkdir(RAW_DIR)
@@ -51,17 +52,26 @@
         dirs.append(custom_model_path)
     characters_dir = os.path.join(ROOT_DIR, 'models', architecture_name, 'characters')
     if os.path.exists(characters_dir):
         dirs.append(characters_dir)
     return dirs
 
 
+def character_dir(architecture_name, character_name):
+    """Returns the directory where the files for a given character model should be stored when that character is
+    downloaded using the individual character download mechanism in the UI.
+    Important! Do not use this method to find an existing character directory. It is possible for users to download
+    characters using model packs, and those character directories are stored elsewhere. Instead, you should
+    search for the character directory within the directories returned by model_dirs."""
+    return os.path.join(MODELS_DIR, architecture_name, 'characters', character_name)
+
+
 def multispeaker_model_dir(architecture_name):
     """Returns the directory where multi-speaker models are stored for the given architecture."""
-    return os.path.join(ROOT_DIR, 'models', architecture_name, 'multispeaker_models')
+    return os.path.join(MODELS_DIR, architecture_name, 'multispeaker_models')
 
 
 def read_metadata(folder):
     """Return the metadata dictionary of a given audio_cache subfolder.
     'folder' should be one of: RAW_DIR, PREPROCESSED_DIR, OUTPUT_DIR, or POSTPROCESSED_DIR."""
     path_to_file = os.path.join(folder, METADATA_FILENAME)
     metadata = dict()
```

### Comparing `hay_say_common-0.1.2/src/hay_say_common/server_utility.py` & `hay_say_common-0.1.3/src/hay_say_common/server_utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,12 +52,12 @@
     output_files = get_file_list(OUTPUT_DIR)
     return 'An error occurred while generating the output: \n' + traceback.format_exc() + \
            '\n\nPayload:\n' + json.dumps(request.json) + \
            '\n\nInput Audio Dir Listing: \n' + input_files + \
            '\n\nOutput Audio Dir Listing: \n' + output_files
 
 
-def get_file_list(directory):
-    if os.path.exists(directory):
-        return ', '.join(os.listdir(directory))
+def get_file_list(folder):
+    if os.path.exists(folder):
+        return ', '.join(os.listdir(folder))
     else:
-        return directory + ' does not exist'
+        return folder + ' does not exist'
```

### Comparing `hay_say_common-0.1.2/src/hay_say_common/utility.py` & `hay_say_common-0.1.3/src/hay_say_common/utility.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     return librosa.load(buffer, sr=None)
 
 
 def read_audio(path):
     return librosa.load(path, sr=None)
 
 
-def get_singleton_file(directory):
-    """Given a directory, return the path of the single file within that directory. If there is no file in that
-    directory, or if there is more than one file in that directory, raise an Exception."""
-    potential_filenames = [file for file in os.listdir(directory)]
+def get_singleton_file(folder):
+    """Given a folder, return the full path of the single file within that folder. If there is no file in that folder,
+    or if there is more than one file in that folder, raise an Exception."""
+    potential_filenames = [file for file in os.listdir(folder)]
     if len(potential_filenames) > 1:
         raise Exception('more than one file was found in the indicated folder. Only one was expected.')
     elif len(potential_filenames) == 0:
         raise Exception('No file was found in the indicated folder.')
-    return os.path.join(directory, potential_filenames[0])
+    return os.path.join(folder, potential_filenames[0])
 
 
 def get_single_file_with_extension(directory, extension):
     """Finds the single file with the given extension in the specified directory. If there is no such file or if there
     is more than one file with the extension, throw an Exception. Otherwise, return the path to the file."""
     all_files = get_files_with_extension(directory, extension)
     if len(all_files) > 1:
```

### Comparing `hay_say_common-0.1.2/src/hay_say_common.egg-info/PKG-INFO` & `hay_say_common-0.1.3/src/hay_say_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hay-say-common
-Version: 0.1.2
+Version: 0.1.3
 Summary: Constants and methods that are shared between the Hay Say UI and various Docker containers it communicates with.
 Author-email: HydrusBeta <hydrusgamma@gmail.com>
 Project-URL: Homepage, https://github.com/hydrusbeta/hay_say_common
 Project-URL: Bug Tracker, https://github.com/hydrusbeta/hay_say_common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

