# Comparing `tmp/CToolKit-1.13.tar.gz` & `tmp/CToolKit-1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CToolKit-1.13.tar", last modified: Mon Jun 19 17:49:49 2023, max compression
+gzip compressed data, was "CToolKit-1.20.tar", last modified: Tue Jul  4 19:08:52 2023, max compression
```

## Comparing `CToolKit-1.13.tar` & `CToolKit-1.20.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-19 17:49:49.153201 CToolKit-1.13/
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-19 17:49:49.125201 CToolKit-1.13/CToolKit/
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      504 2023-06-18 19:59:56.000000 CToolKit-1.13/CToolKit/ComandLineExecution.py
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-19 17:49:49.149201 CToolKit-1.13/CToolKit/Errors/
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      306 2023-06-17 06:47:02.000000 CToolKit-1.13/CToolKit/Errors/ComandLineError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      226 2023-06-17 06:58:51.000000 CToolKit-1.13/CToolKit/Errors/ComandLineWarning.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      110 2023-06-17 06:48:41.000000 CToolKit-1.13/CToolKit/Errors/CopilationError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      118 2023-06-17 06:49:33.000000 CToolKit-1.13/CToolKit/Errors/CopilationWarning.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      108 2023-06-17 06:47:14.000000 CToolKit-1.13/CToolKit/Errors/ExecutionError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      116 2023-06-17 06:57:42.000000 CToolKit-1.13/CToolKit/Errors/ValgrindError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      115 2023-06-17 07:04:59.000000 CToolKit-1.13/CToolKit/Errors/ValgrindLeak.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        0 2023-06-17 04:59:48.000000 CToolKit-1.13/CToolKit/Errors/__init__.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      813 2023-06-19 15:08:57.000000 CToolKit-1.13/CToolKit/__init__.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1472 2023-06-19 17:37:40.000000 CToolKit-1.13/CToolKit/amalgamation.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     4653 2023-06-19 15:20:15.000000 CToolKit-1.13/CToolKit/comand_line_functions.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     2967 2023-06-18 20:01:08.000000 CToolKit-1.13/CToolKit/readme_converter.py
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-19 17:49:49.129201 CToolKit-1.13/CToolKit.egg-info/
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3330 2023-06-19 17:49:48.000000 CToolKit-1.13/CToolKit.egg-info/PKG-INFO
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      566 2023-06-19 17:49:48.000000 CToolKit-1.13/CToolKit.egg-info/SOURCES.txt
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        1 2023-06-19 17:49:48.000000 CToolKit-1.13/CToolKit.egg-info/dependency_links.txt
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        9 2023-06-19 17:49:48.000000 CToolKit-1.13/CToolKit.egg-info/top_level.txt
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1060 2023-06-17 02:11:11.000000 CToolKit-1.13/LICENSE
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3330 2023-06-19 17:49:49.153201 CToolKit-1.13/PKG-INFO
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     2921 2023-06-19 15:21:21.000000 CToolKit-1.13/README.md
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)       38 2023-06-19 17:49:49.153201 CToolKit-1.13/setup.cfg
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      664 2023-06-19 17:49:38.000000 CToolKit-1.13/setup.py
+drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-07-04 19:08:52.580567 CToolKit-1.20/
+drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-07-04 19:08:52.576567 CToolKit-1.20/CToolKit/
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      504 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/ComandLineExecution.py
+drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-07-04 19:08:52.580567 CToolKit-1.20/CToolKit/Errors/
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      306 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/Errors/ComandLineError.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      226 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/Errors/ComandLineWarning.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      110 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/Errors/CopilationError.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      118 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/Errors/CopilationWarning.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      108 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/Errors/ExecutionError.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      205 2023-07-03 20:51:23.000000 CToolKit-1.20/CToolKit/Errors/NotExpectedResult.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      265 2023-07-03 09:56:48.000000 CToolKit-1.20/CToolKit/Errors/ValgrindError.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      264 2023-07-03 09:57:03.000000 CToolKit-1.20/CToolKit/Errors/ValgrindLeak.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        0 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/Errors/__init__.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      874 2023-07-03 18:38:00.000000 CToolKit-1.20/CToolKit/__init__.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1470 2023-07-03 18:39:36.000000 CToolKit-1.20/CToolKit/amalgamation.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     7282 2023-07-04 18:42:05.000000 CToolKit-1.20/CToolKit/comand_line_functions.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      445 2023-07-03 20:58:17.000000 CToolKit-1.20/CToolKit/output_formatation.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3168 2023-07-04 18:47:02.000000 CToolKit-1.20/CToolKit/readme_converter.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1427 2023-07-03 20:37:39.000000 CToolKit-1.20/CToolKit/valgrind_parser.py
+drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-07-04 19:08:52.576567 CToolKit-1.20/CToolKit.egg-info/
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3330 2023-07-04 19:08:52.000000 CToolKit-1.20/CToolKit.egg-info/PKG-INFO
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      662 2023-07-04 19:08:52.000000 CToolKit-1.20/CToolKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        1 2023-07-04 19:08:52.000000 CToolKit-1.20/CToolKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        9 2023-07-04 19:08:52.000000 CToolKit-1.20/CToolKit.egg-info/top_level.txt
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1060 2023-06-17 02:11:11.000000 CToolKit-1.20/LICENSE
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3330 2023-07-04 19:08:52.580567 CToolKit-1.20/PKG-INFO
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     2921 2023-07-03 14:26:26.000000 CToolKit-1.20/README.md
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)       38 2023-07-04 19:08:52.580567 CToolKit-1.20/setup.cfg
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      664 2023-07-04 19:07:51.000000 CToolKit-1.20/setup.py
```

### Comparing `CToolKit-1.13/CToolKit/__init__.py` & `CToolKit-1.20/CToolKit/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,12 +6,13 @@
 from CToolKit.comand_line_functions import test_binary_with_valgrind
 from CToolKit.comand_line_functions import execute_test_for_file
 from CToolKit.comand_line_functions import execute_test_for_folder
 
 
 from CToolKit.Errors.CopilationError import CopilationError
 from CToolKit.Errors.CopilationWarning import CopilationWarning
-from CToolKit.Errors.ExecutionError import  ExecutionError
-from CToolKit.Errors.ValgrindError import  ValgrindError
-from CToolKit.Errors.ValgrindLeak import  ValgrindLeak
+from CToolKit.Errors.ExecutionError import ExecutionError
+from CToolKit.Errors.ValgrindError import ValgrindError
+from CToolKit.Errors.ValgrindLeak import ValgrindLeak
+from CToolKit.Errors.NotExpectedResult import NotExpectedResult
 
 from CToolKit.readme_converter import include_code_in_markdown
```

### Comparing `CToolKit-1.13/CToolKit/amalgamation.py` & `CToolKit-1.20/CToolKit/amalgamation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from os.path import join
 
 
 
-
-
 def get_action(referencer_dir: str, line: str) -> str or None:
     line = line.strip()
     if not line.startswith('#include'):
         return None
 
     if '"' in line:
         relative_file = line.split('"')[1]
```

### Comparing `CToolKit-1.13/CToolKit/comand_line_functions.py` & `CToolKit-1.20/CToolKit/comand_line_functions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from typing import List
 
 from CToolKit.Errors.CopilationError import CopilationError
 from CToolKit.Errors.CopilationWarning import CopilationWarning
 
 from CToolKit.Errors.ValgrindError import  ValgrindError
 from CToolKit.Errors.ValgrindLeak import  ValgrindLeak
-from CToolKit.ComandLineExecution import ComandLineExecution
+from CToolKit.Errors.NotExpectedResult import NotExpectedResult
 
+from CToolKit.ComandLineExecution import ComandLineExecution
+from .valgrind_parser import parse_valgrind_result
 from platform import system as current_os
-
+from os.path import isdir
 from os import listdir,remove
+from .output_formatation import sanitize_value
 
 
 def compile_project_by_command(command: str, raise_errors: bool = True, raise_warnings: bool = True):
     """execute an copilation with the given comand
     Args:
         command (str): the comand copilation ,ex: 'gcc test.c'
         raise_errors (bool, optional): if its to raise An copilation Error
@@ -64,77 +67,154 @@
     compile_project_by_command(command, raise_errors, raise_warnings)
     return output
 
 
 
 
 
-def test_binary_with_valgrind(binary_file:str,flags: List[str]= None):
+def test_binary_with_valgrind(binary_file:str,flags: List[str]= None)->dict:
     """ will test an binary execution with valgrind
     Args:
         binary_file (str): the binary execution ex: test.out
         flags (List[str], optional): addition flags to the copilation
 
     Raises:
         ValgrindError: And valgrind Error ex: an buffer overflow
         ValgrindLeak: _An valgrind leak, ex: an non free alocation
     """
     if flags is None:
         flags = []
 
-    command = f'valgrind  {binary_file} ' + ' '.join(flags)
+    command = f'valgrind  ./{binary_file} ' + ' '.join(flags)
     result = ComandLineExecution(command)
 
+    #(result.output)
+    parsed_result = parse_valgrind_result(result.output)
+
+
     if 'ERROR SUMMARY: 0 errors from 0 contexts (suppressed: 0 from 0)' not in result.output:
-        raise ValgrindError(result.output)
+        raise ValgrindError(result.output,parsed_result)
 
     if 'All heap blocks were freed -- no leaks are possible' not in result.output:
-        raise ValgrindLeak(result.output)
+        raise ValgrindLeak(result.output,parsed_result)
+    
+    return parsed_result
+
+    
 
 
-def execute_test_for_file(compiler:str, file: str):
+def execute_test_for_file(compiler:str, file: str,use_valgrind=True,raise_warnings=True)->dict or ComandLineExecution:
     """Execute an presset test for the current file
     Args:
         compiler (str): the compiler to use, ex: gcc or clang
         file (str): the file to copile , ex: test.c
-
+        raise_warnings(bool): if its to raise warnings generated
     Raises:
         e: all possible errors
     """
     result = compile_project(
         compiler,
         file,
         raise_errors=True,
-        raise_warnings=False
+        raise_warnings=raise_warnings
     )
+    if not use_valgrind:
+        return  ComandLineExecution(result)
+
     try:
-        test_binary_with_valgrind(result)
+        valgrind_test = test_binary_with_valgrind(result)
         remove(result)
     except Exception as e:
         remove(result)
         raise e
 
+    return valgrind_test
+
+
+
+def execute_folder_presset(compiler:str,use_valgrind:bool, filepath: str,dirname:str,raise_warnings:bool)->dict or ComandLineExecution:
+    files = listdir(filepath)
 
-def execute_test_for_folder(compiler:str, folder: str, print_values:bool = True):
+    target_file_name = f'{dirname.replace("##","")}.c'
+    target = f'{filepath}/{target_file_name}'
+
+    if target_file_name not in files:
+        raise FileNotFoundError(filepath)
+
+
+    expected_file_name = None 
+    
+    for file in files:
+        if file.startswith('expected'):
+            expected_file_name = f'{filepath}/{file}'
+    
+   
+    if expected_file_name is None:
+        raise FileNotFoundError(
+            'expected.txt'
+        )
+
+    with open(expected_file_name,'r') as arq:
+        expected = sanitize_value(expected_file_name,arq.read())
+        
+
+    if use_valgrind:
+        r:dict = execute_test_for_file(compiler, target, True, raise_warnings)
+        saninitzed_result = sanitize_value(expected_file_name,r['output'])
+    else:
+        r:ComandLineExecution = execute_test_for_file(compiler, target, False, raise_warnings)
+        saninitzed_result = sanitize_value(expected_file_name,r.output)
+
+    if expected != saninitzed_result:
+        raise NotExpectedResult(saninitzed_result,expected)
+
+
+    return r
+
+    
+    
+          
+    
+def execute_test_for_folder(compiler:str, folder: str, print_values = True,use_valgrind=True, raise_warnings=True):
     """execute tests for all .c or cpp files in the given folder
     Args:
         compiler (str): the compiler, ex: gcc , or clang
         folder (str): the folder to copile
         print_values (bool, optional): if is to print errors and sucess
+        raise_warnings(bool): if its to raise warnings generated
     Raises:
         e: if happen some error
     """
+    
+    print('\033[92m'+f'folder: {folder}')
+    
     files = listdir(folder)
     for file in files:
-        if not file.endswith('.c') or file.endswith('.cpp'):
+        file_path = f'{folder}/{file}'
+        
+        if isdir(file_path):
+            
+            if file.startswith('##'):
+
+                try:
+                    execute_folder_presset(compiler,use_valgrind, file_path, file, raise_warnings)
+                    print('\033[92m' + f'\tpassed: {file}' + '\33[37m')
+                except Exception as e:
+                    print('\033[91m' + f'fail with folder: {file}' + '\33[37m')
+                    raise e
+
+            else:
+                execute_test_for_folder(compiler,file_path,print_values, use_valgrind,raise_warnings)
             continue
 
+        if not file.endswith('.c') or file.endswith('.cpp'):
+            continue
+            
         try:
-            execute_test_for_file(compiler, f'{folder}/{file}')
+            execute_test_for_file(compiler, file_path,use_valgrind,raise_warnings)
             if print_values:
-                print('\033[92m'+f'passed: {file}' + '\33[37m')
-
+                print('\033[92m'+f'\tpassed: {file_path}' + '\33[37m')
         except Exception as e:
             if print_values:
-                print('\033[91m' + f'fail with file: {file}' + '\33[37m')
+                print('\033[91m' + f'fail with file: {file_path}' + '\33[37m')
                 print('\033[0m')
             raise e
```

### Comparing `CToolKit-1.13/CToolKit/readme_converter.py` & `CToolKit-1.20/CToolKit/readme_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
+from typing import Callable
 import json
 
 
 def get_code_reference(line:str)->str or None:
     test = ''
     TARGET  = '<!--codeof:'
     inclusion = ''
     found_start = False
 
     for letter in line:
 
-
         if found_start == False:
-
             if letter == ' ':
                 continue
 
             if not TARGET.startswith(test):
                 return None
 
             test+=letter
@@ -78,15 +77,15 @@
         if ref is None:
             block+=line+'\n'
 
     constructed.append({'type': 'block', 'text': block})
     return constructed
 
 
-def include_code_in_markdown(markdown_file:str,save_file:bool=True)->str:
+def include_code_in_markdown(markdown_file:str,save_file:bool=True,modifier:Callable=None)->str:
     """include all <!--codeof:teste.c--> in the given markdown file
     Args:
         markdown_file (str):the markdown file, ex: README.md
         save_file (bool, optional): if is to save the file
     Returns:
         str: the generated markdown
     """
@@ -101,15 +100,19 @@
             if l['type'] == 'ref':
 
                 text+=f'<!--codeof:{l["ref"]}-->\n'
 
                 with open(l['ref'] ,'r') as ref_arq:
 
                     text+=f'~~~{l["extension"]}\n'
-                    text+=ref_arq.read()
+                    ref_text = ref_arq.read()
+                    if modifier:
+                        text+=modifier(ref_text)
+                    else:
+                        text+=ref_text
                     text+='\n~~~\n'
 
     if '\n' in text:
         text = text[0:-1]
 
     if save_file:
         with open(markdown_file,'w') as arq:
```

### Comparing `CToolKit-1.13/CToolKit.egg-info/PKG-INFO` & `CToolKit-1.20/CToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CToolKit
-Version: 1.13
+Version: 1.20
 Summary: CToolKit to manipulate CPipeLines and Repos
 Home-page: https://oui.tec.br/
 Author: Mateus Moutinho
 Author-email: mateusmoutinho01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `CToolKit-1.13/LICENSE` & `CToolKit-1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `CToolKit-1.13/PKG-INFO` & `CToolKit-1.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CToolKit
-Version: 1.13
+Version: 1.20
 Summary: CToolKit to manipulate CPipeLines and Repos
 Home-page: https://oui.tec.br/
 Author: Mateus Moutinho
 Author-email: mateusmoutinho01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `CToolKit-1.13/README.md` & `CToolKit-1.20/README.md`

 * *Files identical despite different names*

### Comparing `CToolKit-1.13/setup.py` & `CToolKit-1.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='CToolKit',
-    version='1.13',
+    version='1.20',
     description='CToolKit to manipulate CPipeLines and Repos',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mateus Moutinho',
     author_email='mateusmoutinho01@gmail.com',
     url='https://oui.tec.br/',
     packages=find_packages(),
```

