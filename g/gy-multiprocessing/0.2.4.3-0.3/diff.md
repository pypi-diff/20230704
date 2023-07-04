# Comparing `tmp/gy_multiprocessing-0.2.4.3.tar.gz` & `tmp/gy_multiprocessing-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gy_multiprocessing-0.2.4.3.tar", last modified: Wed May 17 15:26:05 2023, max compression
+gzip compressed data, was "gy_multiprocessing-0.3.tar", last modified: Tue Jul  4 10:21:22 2023, max compression
```

## Comparing `gy_multiprocessing-0.2.4.3.tar` & `gy_multiprocessing-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:26:05.047311 gy_multiprocessing-0.2.4.3/
--rw-r--r--   0 guangyuhe   (501) staff       (20)     6428 2023-05-17 15:26:05.047198 gy_multiprocessing-0.2.4.3/PKG-INFO
--rw-r--r--   0 guangyuhe   (501) staff       (20)     6008 2023-05-17 15:25:02.000000 gy_multiprocessing-0.2.4.3/README.md
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:26:05.046207 gy_multiprocessing-0.2.4.3/gy_multiprocessing/
--rw-r--r--   0 guangyuhe   (501) staff       (20)      184 2023-05-17 15:16:59.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing/__init__.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:26:05.046850 gy_multiprocessing-0.2.4.3/gy_multiprocessing/multiprocessing/
--rw-r--r--   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:16:20.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing/multiprocessing/__init__.py
--rw-r--r--   0 guangyuhe   (501) staff       (20)     7217 2023-05-17 15:21:24.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing/multiprocessing/multi_process.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:26:05.047037 gy_multiprocessing-0.2.4.3/gy_multiprocessing/multithreading/
--rw-r--r--   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:16:59.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing/multithreading/__init__.py
--rw-r--r--   0 guangyuhe   (501) staff       (20)     2289 2023-02-22 11:22:12.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing/multithreading/multi_thread.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:26:05.046646 gy_multiprocessing-0.2.4.3/gy_multiprocessing.egg-info/
--rw-r--r--   0 guangyuhe   (501) staff       (20)     6428 2023-05-17 15:26:05.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing.egg-info/PKG-INFO
--rw-r--r--   0 guangyuhe   (501) staff       (20)      412 2023-05-17 15:26:05.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)        1 2023-05-17 15:26:05.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)       19 2023-05-17 15:26:05.000000 gy_multiprocessing-0.2.4.3/gy_multiprocessing.egg-info/top_level.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)       38 2023-05-17 15:26:05.047344 gy_multiprocessing-0.2.4.3/setup.cfg
--rw-r--r--   0 guangyuhe   (501) staff       (20)      826 2023-05-17 15:21:51.000000 gy_multiprocessing-0.2.4.3/setup.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-07-04 10:21:22.426794 gy_multiprocessing-0.3/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     7349 2023-07-04 10:21:22.426676 gy_multiprocessing-0.3/PKG-INFO
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     6933 2023-07-04 10:15:23.000000 gy_multiprocessing-0.3/README.md
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-07-04 10:21:22.424948 gy_multiprocessing-0.3/gy_multiprocessing/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      184 2023-05-17 15:16:59.000000 gy_multiprocessing-0.3/gy_multiprocessing/__init__.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-07-04 10:21:22.426046 gy_multiprocessing-0.3/gy_multiprocessing/multiprocessing/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:16:20.000000 gy_multiprocessing-0.3/gy_multiprocessing/multiprocessing/__init__.py
+-rw-r--r--   0 guangyuhe   (501) staff       (20)    11347 2023-07-04 10:15:23.000000 gy_multiprocessing-0.3/gy_multiprocessing/multiprocessing/multi_process.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-07-04 10:21:22.426277 gy_multiprocessing-0.3/gy_multiprocessing/multithreading/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)        0 2023-05-17 15:16:59.000000 gy_multiprocessing-0.3/gy_multiprocessing/multithreading/__init__.py
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     2289 2023-02-22 11:22:12.000000 gy_multiprocessing-0.3/gy_multiprocessing/multithreading/multi_thread.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-07-04 10:21:22.425828 gy_multiprocessing-0.3/gy_multiprocessing.egg-info/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     7349 2023-07-04 10:21:22.000000 gy_multiprocessing-0.3/gy_multiprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      412 2023-07-04 10:21:22.000000 gy_multiprocessing-0.3/gy_multiprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)        1 2023-07-04 10:21:22.000000 gy_multiprocessing-0.3/gy_multiprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       19 2023-07-04 10:21:22.000000 gy_multiprocessing-0.3/gy_multiprocessing.egg-info/top_level.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       38 2023-07-04 10:21:22.426839 gy_multiprocessing-0.3/setup.cfg
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      822 2023-07-04 10:15:23.000000 gy_multiprocessing-0.3/setup.py
```

### Comparing `gy_multiprocessing-0.2.4.3/PKG-INFO` & `gy_multiprocessing-0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: gy_multiprocessing
-Version: 0.2.4.3
-Summary: Run function in multiple processes
-Home-page: https://github.com/guangyu-he/gy-multiprocessing
-Author: Guangyu He
-Author-email: me@heguangyu.net
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # gy-multiprocessing
 
 ## Installation
 
 ### via Github
 
 ```bash
@@ -46,37 +33,47 @@
 
 ```python
 import time
 import gy_multiprocessing as gymp
 
 
 def your_func(a_string: int, queue):
-    # NOTE! you MUST add an argument for queue and use put() method to fetch the returning value
+    # NEW from v0.3! if multiprocessing is not used, queue is not a necessary parameter
+    # NOTE! you MUST add an argument for queue and use put() method to fetch the returning value if multiprocessing is used
 
     print(a_string)
     if a_string % 5 == 0:
         time.sleep(2)
 
-    # NOTE! if you are missing this method, there will be None result returned for current process
+    # NEW from v0.3! if multiprocessing is not used, all queue relevant codes can still be kept
+    # NEW from v0.3! and the if queue is not None: is not necessary anymore
+    # NOTE! if you are missing this method, there will be None result returned for current process if multiprocessing is used
     queue.put(a_string)
+    return a_string
 
 
 if __name__ == '__main__':
     # the multiprocessing must work in a function or entrance
     # do not use it barely
 
     """
     # initializing the multiprocessing instance
     # the default max_process are your cpu max cores
     # max_process could be infinite, but performance will get suffered when the hardware is overloaded
     """
+
+    # NEW from v0.3! set max_process to 0 will disable multiprocessing
     mp = gymp.MultiProcess(max_process=8)
 
     # example for multiprocessing in the loop
     outer_loop_times = 5
+
+    # NEW from v0.3! it is possible to test beforehand if the function and args is suitable for multiprocessing
+    test_your_func: bool = mp.test(your_func, (1,))
+
     for current_loop_index in range(outer_loop_times):
         # your running arguments, must be tuple
         args = (current_loop_index,)
 
         """
         # adding tasks in multiprocessing pool
         """
@@ -244,14 +241,23 @@
 ### v0.2.4.3
 
 #### updates
 
 - package import improvement. **PLEASE UPDATE IMPORT AS EXAMPLES ABOVE**
 - check a boolean type input argument
 
+### v0.3
+
+#### feature
+
+- added a test method to check if the function and args is suitable for multiprocessing
+- added a max_process=0 possibility to disable multiprocessing
+- queue parameter in user function has a more flexibility to be used among multiprocessing mode on and off
+- a new multiprocessing pool logic to check if the subprocess is done
+
 ## Support
 
 feel free to check source code in <a href="https://github.com/guangyu-he/gy-multiprocessing">GitHub</a>, you are welcome
 to leave any comments.
 
 2022&copy;Guangyu He, for further support please contact author. <br>
 Email: <a href="mailto:me@heguangyu.net">me@heguangyu.net</a>
```

### Comparing `gy_multiprocessing-0.2.4.3/README.md` & `gy_multiprocessing-0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: gy_multiprocessing
+Version: 0.3
+Summary: Run function in multiple processes
+Home-page: https://github.com/guangyu-he/gy-multiprocessing
+Author: Guangyu He
+Author-email: me@heguangyu.net
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # gy-multiprocessing
 
 ## Installation
 
 ### via Github
 
 ```bash
@@ -33,37 +46,47 @@
 
 ```python
 import time
 import gy_multiprocessing as gymp
 
 
 def your_func(a_string: int, queue):
-    # NOTE! you MUST add an argument for queue and use put() method to fetch the returning value
+    # NEW from v0.3! if multiprocessing is not used, queue is not a necessary parameter
+    # NOTE! you MUST add an argument for queue and use put() method to fetch the returning value if multiprocessing is used
 
     print(a_string)
     if a_string % 5 == 0:
         time.sleep(2)
 
-    # NOTE! if you are missing this method, there will be None result returned for current process
+    # NEW from v0.3! if multiprocessing is not used, all queue relevant codes can still be kept
+    # NEW from v0.3! and the if queue is not None: is not necessary anymore
+    # NOTE! if you are missing this method, there will be None result returned for current process if multiprocessing is used
     queue.put(a_string)
+    return a_string
 
 
 if __name__ == '__main__':
     # the multiprocessing must work in a function or entrance
     # do not use it barely
 
     """
     # initializing the multiprocessing instance
     # the default max_process are your cpu max cores
     # max_process could be infinite, but performance will get suffered when the hardware is overloaded
     """
+
+    # NEW from v0.3! set max_process to 0 will disable multiprocessing
     mp = gymp.MultiProcess(max_process=8)
 
     # example for multiprocessing in the loop
     outer_loop_times = 5
+
+    # NEW from v0.3! it is possible to test beforehand if the function and args is suitable for multiprocessing
+    test_your_func: bool = mp.test(your_func, (1,))
+
     for current_loop_index in range(outer_loop_times):
         # your running arguments, must be tuple
         args = (current_loop_index,)
 
         """
         # adding tasks in multiprocessing pool
         """
@@ -231,14 +254,23 @@
 ### v0.2.4.3
 
 #### updates
 
 - package import improvement. **PLEASE UPDATE IMPORT AS EXAMPLES ABOVE**
 - check a boolean type input argument
 
+### v0.3
+
+#### feature
+
+- added a test method to check if the function and args is suitable for multiprocessing
+- added a max_process=0 possibility to disable multiprocessing
+- queue parameter in user function has a more flexibility to be used among multiprocessing mode on and off
+- a new multiprocessing pool logic to check if the subprocess is done
+
 ## Support
 
 feel free to check source code in <a href="https://github.com/guangyu-he/gy-multiprocessing">GitHub</a>, you are welcome
 to leave any comments.
 
 2022&copy;Guangyu He, for further support please contact author. <br>
 Email: <a href="mailto:me@heguangyu.net">me@heguangyu.net</a>
```

### Comparing `gy_multiprocessing-0.2.4.3/gy_multiprocessing/multiprocessing/multi_process.py` & `gy_multiprocessing-0.3/gy_multiprocessing/multiprocessing/multi_process.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # importing relevant types
 from multiprocessing.context import Process as ProcessType
 from types import FunctionType, MethodType
 
 # importing necessary modules
 import time
+import inspect
 import warnings
 
 
 class MultiProcess:
 
     def __init__(self, max_process: int = cpu_count(), silent: bool = False):
         """
@@ -20,32 +21,73 @@
 
         Using Process method from multiprocessing to process the multiprocessing tasks
         """
 
         # error handling
         if type(max_process) is not int:
             raise TypeError(f"Wrong type of max process '{max_process}', must be an integer!")
-        if max_process == 0:
-            raise IndexError("max process can not be 0!")
         if max_process > cpu_count():
             warnings.warn("too much sub processes, performance may get influenced!")
         if isinstance(silent, bool) is False:
             raise TypeError(f"Wrong type of silent '{silent}', must be a boolean!")
 
         # set max processing pool equals to the cpu core number
         self.max_process: int = max_process
 
         # show log in console
         self.silent: bool = silent
 
+        if max_process == 0 and not self.silent:
+            print(f"max process is set to 0: multiprocessing will not be used.")
+
+        # see if there is a queue object in user function parameters
+        self.has_queue_param: bool = True
+
         # see if there is a valid queue.put() method
         self.has_queue_put: bool = True
 
+        # use to store the multiprocessing processes
         self.mp_pool_list: list[dict] = []
 
+        # use to store the result from each process when multiprocessing is not used
+        self.non_mp_result: list = []
+
+    class _NoneQueue:
+        """
+        A class to replace queue when multiprocessing is not used, and avoid error when calling queue.put()
+        """
+
+        def put(*args):
+            pass
+
+    def test(self, func, args: tuple) -> bool:
+        """
+        Testing the function and arguments to see if they are suitable for multiprocessing
+        Args:
+            func (function): the function to be called
+            args (tuple): the arguments to be passed to the function
+        Returns:
+            bool: whether the function and arguments are suitable for multiprocessing
+        """
+        test_passed: bool = True
+
+        if not isinstance(func, FunctionType) and not isinstance(func, MethodType):
+            print("Wrong type of func, must be a FunctionType!")
+            test_passed = False
+        if not isinstance(args, tuple):
+            print("Wrong type of args, must be a tuple!")
+            test_passed = False
+
+        parameters = inspect.signature(func).parameters
+        if "queue" not in parameters and self.max_process > 0:
+            print(f"queue parameter not found in '{func.__name__}'")
+            test_passed = False
+
+        return test_passed
+
     def add(self, func, args: tuple, process_name: str = ""):
         """
         Args:
             func (function): the function to be called
             args (tuple): the arguments to be passed to the function
             process_name (str, optional): the name of the process. Defaults to "".
 
@@ -59,104 +101,162 @@
         if not isinstance(func, FunctionType) and not isinstance(func, MethodType):
             raise TypeError("Wrong type of func, must be a FunctionType!")
         if not isinstance(args, tuple):
             raise TypeError("Wrong type of args, must be a tuple!")
         if not isinstance(process_name, str):
             raise TypeError("Wrong type of process name, must be a str!")
 
-        # a get context method for get return value
-        # NOTE! a q.put() method must include in the called func and its args
-        queue_instance = get_context('spawn').Queue()
-
-        # initialize multiprocessing for core loop function
-        process: ProcessType = Process(target=func, args=args + (queue_instance,))
-        # set dict inside the process list
-        process_list_dict: dict = {'process': process, 'start_time': int, 'process_result': queue_instance,
-                                   'process_name': process_name}
-        self.mp_pool_list.append(process_list_dict)
+        # check if there is a queue parameter in the user function
+        parameters = inspect.signature(func).parameters
+        if "queue" not in parameters:
+            self.has_queue_param = False
+
+        if self.max_process == 0:
+            # if max process is set to 0, multiprocessing will not be used
+
+            # initialize time and result
+            current_time = time.time()
+
+            if self.has_queue_param:
+                # there is queue parameter in the func, but multiprocessing is not used
+                # then set up a fake queue object to avoid error when calling queue.put()
+                args = args + (self._NoneQueue,)
+
+            # execute the function
+            get_result = func(*args)
+
+            # store the result from the function
+            self.non_mp_result.append(get_result)
+
+            time_cost = time.time() - current_time
+            if not self.silent:
+                if process_name != "":
+                    process_name = f"process: '{process_name}'"
+                else:
+                    process_name = "process"
+                print(
+                    f"{process_name} done in {format(time_cost, '.1f')}s with result {get_result}")
+        else:
+            if not self.test(func, args):
+                raise Exception("Function and arguments are not suitable for multiprocessing!")
+
+            # a get context method for get return value
+            # NOTE! a q.put() method must include in the called func and its args
+            queue_instance = get_context('spawn').Queue()
+
+            # initialize multiprocessing for core loop function
+            process: ProcessType = Process(target=func, args=args + (queue_instance,))
+            # set dict inside the process list
+            process_list_dict: dict = {'process': process, 'start_time': int, 'process_result': queue_instance,
+                                       'process_name': process_name}
+            self.mp_pool_list.append(process_list_dict)
 
     def each_process_func(self, list_of_processes: list) -> list:
         for processing_index, each_processing_process in enumerate(list_of_processes):
-            if not each_processing_process['process'].is_alive():
-
-                # check each process
-                current_time = time.time()
-                time_cost = current_time - each_processing_process['start_time']
-
-                # initialize the result
-                get_result = None
-
-                if each_processing_process['process'].exitcode == 1:
-                    # means there is an error occurred in this process
-                    get_result = f"{each_processing_process['process_name'] + ' '}FAILED"
-                    each_processing_process['process'].kill()
-                else:
-                    try:
-                        # if the process is not alive, use a small timeout to see if there is a valid non-empty queue
-                        get_result = each_processing_process['process_result'].get(timeout=0.05)
-                    except Exception as e:
-                        if repr(e) == "Empty()":
-                            self.has_queue_put = False
-                            get_result = None
-
-                if not self.silent:
-                    print(
-                        f"process: {str(each_processing_process['process'].name)} done in: {format(time_cost, '.1f')}s with {each_processing_process['process_name']} and result {get_result}") \
-                        if each_processing_process['process_name'] != "" \
-                        else print(
-                        f"process: {str(each_processing_process['process'].name)} done in: {format(time_cost, '.1f')}s with result {get_result}")
 
-                # remove the stopped task from processing list
+            # check each process
+            current_time = time.time()
+            time_cost = current_time - each_processing_process['start_time']
+
+            # initialize the result
+            get_result = None
+
+            if each_processing_process['process'].exitcode is None:
+                # the process is still alive
+                continue
+
+            # the following code is for the process is done
+            elif each_processing_process['process'].exitcode == 0:
+                # the process is done successfully
+                try:
+                    # if the process is not alive, use a small timeout to see if there is a valid non-empty queue
+                    get_result = each_processing_process['process_result'].get(timeout=0.05)
+                except Exception as e:
+                    if repr(e) == "Empty()":
+                        # script finds no queue.put() method in the user function
+                        self.has_queue_put = False
+                        get_result = None
+            elif each_processing_process['process'].exitcode == 1:
+                # means there is an error occurred in this process
+                get_result = f"{each_processing_process['process_name'] + ' '}FAILED"
+            else:
+                # the process is done with an unknown error
+                # shutdown the process and raise an error
+                each_processing_process['process'].kill()
                 list_of_processes.pop(processing_index)
-                for process_index, each_process in enumerate(self.mp_pool_list):
-                    if each_processing_process['process'].name == each_process['process'].name:
-                        self.mp_pool_list[process_index]['process_result'] = get_result
+                raise Exception(f"Unknown error occurred in process: {each_processing_process['process'].name}")
+
+            if not self.silent:
+                print(
+                    f"process: {str(each_processing_process['process'].name)} done in {format(time_cost, '.1f')}s with {each_processing_process['process_name']} and result {get_result}") \
+                    if each_processing_process['process_name'] != "" \
+                    else print(
+                    f"process: {str(each_processing_process['process'].name)} done in {format(time_cost, '.1f')}s with result {get_result}")
+
+            # saving the result into the full process list, corresponding to the process name
+            for process_index, each_process in enumerate(self.mp_pool_list):
+                if each_processing_process['process'].name == each_process['process'].name:
+                    self.mp_pool_list[process_index]['process_result'] = get_result
+
+            # as long as the process is done, kill it
+            each_processing_process['process'].kill()
+
+            # remove the stopped task from processing list
+            list_of_processes.pop(processing_index)
+
+            # everytime the loop find a finished process, break the loop and return the list
+            # then let the outer while loop to check if there is any process left
+            # if there is still process alive, the outer while loop will continue give process to
+            # the internal for loop
+            break
 
         return list_of_processes
 
     def run(self) -> list:
         """
         Returns:
             the result list of returned value from each tasks
 
         Run all the processes
         """
 
-        # initializing a processing list with max length of max_process
-        processing_list: list = []
-
-        if len(self.mp_pool_list) <= self.max_process:
-            # if the number of tasks is less than max_process number
-            for process_index, each_process in enumerate(self.mp_pool_list):
-                # put all tasks in the pool
-                processing_list.append(each_process)
-                each_process['start_time'] = time.time()
-                each_process['process'].start()
-
-            while processing_list:
-                time.sleep(0.05)
-                processing_list = self.each_process_func(processing_list)
+        if self.max_process == 0:
+            # not using multiprocessing at all
+            return self.non_mp_result
 
         else:
-            # if the number of tasks is more than max_process number
-            for pool_index, each_process in enumerate(self.mp_pool_list):
-                if len(processing_list) < self.max_process:
-                    # if there is less than max_process number of tasks in the pool
-                    # add a new task in it
+            # initializing a processing list with max length of max_process
+            processing_list: list = []
+
+            if len(self.mp_pool_list) <= self.max_process:
+                # if the number of tasks is less than max_process number
+                for process_index, each_process in enumerate(self.mp_pool_list):
+                    # put all tasks in the pool
                     processing_list.append(each_process)
                     each_process['start_time'] = time.time()
                     each_process['process'].start()
+
                 while processing_list:
+                    processing_list = self.each_process_func(processing_list)
 
-                    if len(processing_list) < self.max_process and pool_index != len(self.mp_pool_list) - 1:
-                        # if all tasks are in the pool then wait until all tasks are finished
-                        # or break the loop to add a new task in the pool
-                        break
-                    else:
-                        time.sleep(0.05)
+            else:
+                # if the number of tasks is more than max_process number
+                for pool_index, each_process in enumerate(self.mp_pool_list):
+                    if len(processing_list) < self.max_process:
+                        # if there is less than max_process number of tasks in the pool
+                        # add a new task in it
+                        processing_list.append(each_process)
+                        each_process['start_time'] = time.time()
+                        each_process['process'].start()
+                    while processing_list:
+
+                        if len(processing_list) < self.max_process and pool_index != len(self.mp_pool_list) - 1:
+                            # if all tasks are in the pool then wait until all tasks are finished
+                            # or break the loop to add a new task in the pool
+                            break
 
-                    processing_list = self.each_process_func(processing_list)
+                        processing_list = self.each_process_func(processing_list)
 
-        if not self.has_queue_put:
-            warnings.warn("You may miss the queue.put() method in your function. The results may not correct!")
+            if not self.has_queue_put:
+                warnings.warn("You may miss the queue.put() method in your function. The results may not correct!")
 
-        return [res['process_result'] for res in self.mp_pool_list]
+            return [res['process_result'] for res in self.mp_pool_list]
```

### Comparing `gy_multiprocessing-0.2.4.3/gy_multiprocessing/multithreading/multi_thread.py` & `gy_multiprocessing-0.3/gy_multiprocessing/multithreading/multi_thread.py`

 * *Files identical despite different names*

### Comparing `gy_multiprocessing-0.2.4.3/gy_multiprocessing.egg-info/PKG-INFO` & `gy_multiprocessing-0.3/gy_multiprocessing.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gy-multiprocessing
-Version: 0.2.4.3
+Version: 0.3
 Summary: Run function in multiple processes
 Home-page: https://github.com/guangyu-he/gy-multiprocessing
 Author: Guangyu He
 Author-email: me@heguangyu.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -46,37 +46,47 @@
 
 ```python
 import time
 import gy_multiprocessing as gymp
 
 
 def your_func(a_string: int, queue):
-    # NOTE! you MUST add an argument for queue and use put() method to fetch the returning value
+    # NEW from v0.3! if multiprocessing is not used, queue is not a necessary parameter
+    # NOTE! you MUST add an argument for queue and use put() method to fetch the returning value if multiprocessing is used
 
     print(a_string)
     if a_string % 5 == 0:
         time.sleep(2)
 
-    # NOTE! if you are missing this method, there will be None result returned for current process
+    # NEW from v0.3! if multiprocessing is not used, all queue relevant codes can still be kept
+    # NEW from v0.3! and the if queue is not None: is not necessary anymore
+    # NOTE! if you are missing this method, there will be None result returned for current process if multiprocessing is used
     queue.put(a_string)
+    return a_string
 
 
 if __name__ == '__main__':
     # the multiprocessing must work in a function or entrance
     # do not use it barely
 
     """
     # initializing the multiprocessing instance
     # the default max_process are your cpu max cores
     # max_process could be infinite, but performance will get suffered when the hardware is overloaded
     """
+
+    # NEW from v0.3! set max_process to 0 will disable multiprocessing
     mp = gymp.MultiProcess(max_process=8)
 
     # example for multiprocessing in the loop
     outer_loop_times = 5
+
+    # NEW from v0.3! it is possible to test beforehand if the function and args is suitable for multiprocessing
+    test_your_func: bool = mp.test(your_func, (1,))
+
     for current_loop_index in range(outer_loop_times):
         # your running arguments, must be tuple
         args = (current_loop_index,)
 
         """
         # adding tasks in multiprocessing pool
         """
@@ -244,14 +254,23 @@
 ### v0.2.4.3
 
 #### updates
 
 - package import improvement. **PLEASE UPDATE IMPORT AS EXAMPLES ABOVE**
 - check a boolean type input argument
 
+### v0.3
+
+#### feature
+
+- added a test method to check if the function and args is suitable for multiprocessing
+- added a max_process=0 possibility to disable multiprocessing
+- queue parameter in user function has a more flexibility to be used among multiprocessing mode on and off
+- a new multiprocessing pool logic to check if the subprocess is done
+
 ## Support
 
 feel free to check source code in <a href="https://github.com/guangyu-he/gy-multiprocessing">GitHub</a>, you are welcome
 to leave any comments.
 
 2022&copy;Guangyu He, for further support please contact author. <br>
 Email: <a href="mailto:me@heguangyu.net">me@heguangyu.net</a>
```

### Comparing `gy_multiprocessing-0.2.4.3/setup.py` & `gy_multiprocessing-0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = Path(__file__).parent
 with open(this_directory / "README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="gy_multiprocessing",
-    version="0.2.4.3",
+    version="0.3",
     author="Guangyu He",
     author_email="me@heguangyu.net",
     description="Run function in multiple processes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/guangyu-he/gy-multiprocessing",
     install_requires=[],
```

