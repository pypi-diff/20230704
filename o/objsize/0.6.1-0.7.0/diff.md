# Comparing `tmp/objsize-0.6.1.tar.gz` & `tmp/objsize-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objsize-0.6.1.tar", last modified: Wed Sep 28 07:35:01 2022, max compression
+gzip compressed data, was "objsize-0.7.0.tar", last modified: Mon Jul  3 22:47:03 2023, max compression
```

## Comparing `objsize-0.6.1.tar` & `objsize-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2022-09-28 07:35:01.335003 objsize-0.6.1/
--rw-rw-r--   0 liran     (1000) liran     (1000)     1501 2022-09-28 07:31:12.000000 objsize-0.6.1/LICENSE
--rw-rw-r--   0 liran     (1000) liran     (1000)       78 2022-07-11 10:31:23.000000 objsize-0.6.1/MANIFEST.in
--rw-rw-r--   0 liran     (1000) liran     (1000)    10100 2022-09-28 07:35:01.331003 objsize-0.6.1/PKG-INFO
--rwxrwxr-x   0 liran     (1000) liran     (1000)     9347 2022-09-28 07:31:12.000000 objsize-0.6.1/README.md
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2022-09-28 07:35:01.331003 objsize-0.6.1/objsize.egg-info/
--rw-rw-r--   0 liran     (1000) liran     (1000)    10100 2022-09-28 07:35:01.000000 objsize-0.6.1/objsize.egg-info/PKG-INFO
--rw-rw-r--   0 liran     (1000) liran     (1000)      218 2022-09-28 07:35:01.000000 objsize-0.6.1/objsize.egg-info/SOURCES.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)        1 2022-09-28 07:35:01.000000 objsize-0.6.1/objsize.egg-info/dependency_links.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)       65 2022-09-28 07:35:01.000000 objsize-0.6.1/objsize.egg-info/requires.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)        8 2022-09-28 07:35:01.000000 objsize-0.6.1/objsize.egg-info/top_level.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)    12456 2022-09-28 07:31:12.000000 objsize-0.6.1/objsize.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     3258 2022-09-28 07:31:12.000000 objsize-0.6.1/pyproject.toml
--rw-rw-r--   0 liran     (1000) liran     (1000)       38 2022-09-28 07:35:01.335003 objsize-0.6.1/setup.cfg
--rw-rw-r--   0 liran     (1000) liran     (1000)     1697 2022-09-28 07:31:12.000000 objsize-0.6.1/setup.py
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 22:47:03.698055 objsize-0.7.0/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-06-17 00:23:49.000000 objsize-0.7.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1501 2023-07-03 22:38:52.000000 objsize-0.7.0/LICENSE
+-rw-rw-r--   0 liran     (1000) liran     (1000)       78 2022-07-11 10:31:23.000000 objsize-0.7.0/MANIFEST.in
+-rw-rw-r--   0 liran     (1000) liran     (1000)    11886 2023-07-03 22:47:03.698055 objsize-0.7.0/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)    11112 2023-07-03 22:41:31.000000 objsize-0.7.0/README.md
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 22:47:03.694055 objsize-0.7.0/objsize/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     7898 2023-07-03 22:38:52.000000 objsize-0.7.0/objsize/__init__.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)    13967 2023-06-13 07:18:17.000000 objsize-0.7.0/objsize/traverse.py
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 22:47:03.698055 objsize-0.7.0/objsize.egg-info/
+-rw-rw-r--   0 liran     (1000) liran     (1000)    11886 2023-07-03 22:47:03.000000 objsize-0.7.0/objsize.egg-info/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)      257 2023-07-03 22:47:03.000000 objsize-0.7.0/objsize.egg-info/SOURCES.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-07-03 22:47:03.000000 objsize-0.7.0/objsize.egg-info/dependency_links.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)      187 2023-07-03 22:47:03.000000 objsize-0.7.0/objsize.egg-info/requires.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)        8 2023-07-03 22:47:03.000000 objsize-0.7.0/objsize.egg-info/top_level.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1927 2023-07-03 22:38:52.000000 objsize-0.7.0/pyproject.toml
+-rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-07-03 22:47:03.698055 objsize-0.7.0/setup.cfg
```

### Comparing `objsize-0.6.1/LICENSE` & `objsize-0.7.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2006-2022, Liran Funaro.
+Copyright (c) 2006-2023, Liran Funaro.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 1. Redistributions of source code must retain the above copyright
    notice, this list of conditions and the following disclaimer.
 2. Redistributions in binary form must reproduce the above copyright
```

### Comparing `objsize-0.6.1/PKG-INFO` & `objsize-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,144 +1,113 @@
 Metadata-Version: 2.1
 Name: objsize
-Version: 0.6.1
+Version: 0.7.0
 Summary: Traversal over Python's objects subtree and calculate the total size of the subtree in bytes (deep size).
 Author-email: Liran Funaro <liran.funaro@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/liran-funaro/objsize
 Keywords: object-size,recursive,deep,traversal,object,size,debug,deep-object-size
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
-<!---
-Copyright (c) 2006-2022, Liran Funaro.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-1. Redistributions of source code must retain the above copyright
-   notice, this list of conditions and the following disclaimer.
-2. Redistributions in binary form must reproduce the above copyright
-   notice, this list of conditions and the following disclaimer in the
-   documentation and/or other materials provided with the distribution.
-3. Neither the name of the copyright holder nor the
-   names of its contributors may be used to endorse or promote products
-   derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
-LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
---->
-
 # objsize
 
-[![Coverage Status](https://coveralls.io/repos/github/liran-funaro/objsize/badge.svg?branch=master)](https://coveralls.io/github/liran-funaro/objsize?branch=master)
-
-Traversal over Python's objects subtree and calculate the total size of the subtree in bytes (deep size).
+[![Coverage Status](https://coveralls.io/repos/github/liran-funaro/objsize/badge.svg?branch=master)](https://coveralls.io/github/liran-funaro/objsize?branch=master) [![Downloads](https://static.pepy.tech/badge/objsize)](https://pepy.tech/project/objsize)
 
-This module traverses all child objects using Python's internal GC implementation.
-It attempts to ignore shared objects (i.e., `None`, types, modules, classes, functions, lambdas), as they are common
-among all objects.
-It is implemented without recursive calls for high performance.
-
-# Features
-
-- Traverse objects' subtree
-- Calculate objects' (deep) size in bytes
-- Exclude non-exclusive objects
-- Exclude specified objects subtree
-- Allow the user to specify unique handlers for:
-    - Object's size calculation
-    - Object's referents (i.e., its children)
-    - Object filter (skip specific objects)
+The `objsize` Python package allows for the exploration and
+measurement of an object’s complete memory usage in bytes, including its
+child objects. This process, often referred to as deep size calculation,
+is achieved through Python’s internal Garbage Collection (GC) mechanism.
+
+The `objsize` package is designed to ignore shared objects, such as
+`None`, types, modules, classes, functions, and lambdas, because they
+are shared across many instances. One of the key performance features of
+`objsize` is that it avoids recursive calls, ensuring a faster and
+safer execution.
+
+## Key Features
+
+* Traverse objects’ subtree
+* Calculates the size of objects, including nested objects (deep size), in bytes
+* Exclude non-exclusive objects
+* Exclude specified objects subtree
+* Provides flexibility by allowing users to define custom handlers for:
+  - Object’s size calculation
+  - Object’s referents (i.e., its children)
+  - Object filter (skip specific objects)
 
-[Pympler](https://pythonhosted.org/Pympler/) also supports determining an object deep size via `pympler.asizeof()`.
-There are two main differences between `objsize` and `pympler`.
+## Documentation
 
-1. `objsize` has additional features:
-    * Traversing the object subtree: iterating all the object's descendants one by one.
-    * Excluding non-exclusive objects. That is, objects that are also referenced from somewhere else in the program.
-      This is true for calculating the object's deep size and for traversing its descendants.
-2. `objsize` has a simple and robust implementation with significantly fewer lines of code, compared to `pympler`.
-   The Pympler implementation uses recursion, and thus have to use a maximal depth argument to avoid reaching Python's
-   max depth.
-   `objsize`, however, uses BFS which is more efficient and simple to follow.
-   Moreover, the Pympler implementation carefully takes care of any object type.
-   `objsize` archives the same goal with a simple and generic implementation, which has fewer lines of code.
+| [`objsize`](https://liran-funaro.github.io/objsize/library/objsize.html#module-objsize)   | Traversal over Python's objects subtree and calculating the total size of the subtree (deep size).   |
+|-------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
 
 # Install
 
 ```bash
-pip install objsize==0.6.1
+pip install objsize==0.7.0
 ```
 
 # Basic Usage
 
 Calculate the size of the object including all its members in bytes.
 
 ```pycon
 >>> import objsize
 >>> objsize.get_deep_size(dict(arg1='hello', arg2='world'))
 340
 ```
 
-It is possible to calculate the deep size of multiple objects by passing multiple arguments:
+It is possible to calculate the deep size of multiple objects by passing
+multiple arguments:
 
 ```pycon
 >>> objsize.get_deep_size(['hello', 'world'], dict(arg1='hello', arg2='world'), {'hello', 'world'})
 628
 ```
 
 # Complex Data
 
-`objsize` can calculate the size of an object's entire subtree in bytes regardless of the type of objects in it, and its
-depth.
+`objsize` can calculate the size of an object’s entire subtree in
+bytes regardless of the type of objects in it, and its depth.
 
-Here is a complex data structure, for example, that include a self reference:
+Here is a complex data structure, for example, that include a self
+reference:
 
 ```python
-my_data = (list(range(3)), list(range(3, 6)))
-
+my_data = list(range(3)), list(range(3, 6))
 
 class MyClass:
     def __init__(self, x, y):
         self.x = x
         self.y = y
         self.d = {'x': x, 'y': y, 'self': self}
 
     def __repr__(self):
-        return "MyClass"
-
+        return f"{self.__class__.__name__}()"
 
 my_obj = MyClass(*my_data)
 ```
 
 We can calculate `my_obj` deep size, including its stored data.
 
 ```pycon
 >>> objsize.get_deep_size(my_obj)
-708
+724
 ```
 
-We might want to ignore non-exclusive objects such as the ones stored in `my_data`.
+We might want to ignore non-exclusive objects such as the ones stored in
+`my_data`.
 
 ```pycon
 >>> objsize.get_deep_size(my_obj, exclude=[my_data])
 384
 ```
 
 Or simply let `objsize` detect that automatically:
@@ -146,203 +115,263 @@
 ```pycon
 >>> objsize.get_exclusive_deep_size(my_obj)
 384
 ```
 
 # Non Shared Functions or Classes
 
-`objsize` filters functions, lambdas, and classes by default since they are usually shared among many objects.
-For example:
+`objsize` filters functions, lambdas, and classes by default since
+they are usually shared among many objects. For example:
 
 ```pycon
 >>> method_dict = {"identity": lambda x: x, "double": lambda x: x*2}
 >>> objsize.get_deep_size(method_dict)
 232
 ```
 
-Some objects, however, as illustrated in the above example, have unique functions not shared by other objects.
-Due to this, it may be useful to count their sizes.
-You can achieve this by providing an alternative filter function.
+Some objects, however, as illustrated in the above example, have unique
+functions not shared by other objects. Due to this, it may be useful to
+count their sizes. You can achieve this by providing an alternative
+filter function.
 
 ```pycon
 >>> objsize.get_deep_size(method_dict, filter_func=objsize.shared_object_filter)
 986
 ```
 
 Notes:
 
-* The default filter function is `objsize.shared_object_or_function_filter`.
-* When using `objsize.shared_object_filter`, shared functions and lambdas are also counted, but builtin functions are
-  still excluded.
+* The default filter function is
+  [`objsize.traverse.shared_object_or_function_filter()`](https://liran-funaro.github.io/objsize/library/objsize.traverse.html#objsize.traverse.shared_object_or_function_filter).
+* When using [`objsize.traverse.shared_object_filter()`](https://liran-funaro.github.io/objsize/library/objsize.traverse.html#objsize.traverse.shared_object_filter), shared functions and
+  lambdas are also counted, but builtin functions are still excluded.
 
 # Special Cases
 
-Some objects handle their data in a way that prevents Python's GC from detecting it.
-The user can supply a special way to calculate the actual size of these objects.
+Some objects handle their data in a way that prevents Python’s GC from
+detecting it. The user can supply a special way to calculate the actual
+size of these objects.
 
-## Case 1: `torch`
+## Case 1: [`torch`](https://pytorch.org/docs/stable/torch.html#module-torch)
 
-Using a simple calculation of the object size won't work for `torch.Tensor`.
+Using a simple calculation of the object size won’t work for
+[`torch.Tensor`](https://pytorch.org/docs/stable/tensors.html#torch.Tensor).
 
 ```pycon
 >>> import torch
 >>> objsize.get_deep_size(torch.rand(200))
 72
 ```
 
 So the user can define its own size calculation handler for such cases:
 
 ```python
 import objsize
 import sys
 import torch
 
-
 def get_size_of_torch(o):
     # `objsize.safe_is_instance` catches `ReferenceError` caused by `weakref` objects
     if objsize.safe_is_instance(o, torch.Tensor):
-        return sys.getsizeof(o.storage())
+        return sys.getsizeof(o) + (o.element_size() * o.nelement())
     else:
         return sys.getsizeof(o)
 ```
 
 Then use it as follows:
 
 ```pycon
->>> import torch
 >>> objsize.get_deep_size(
 ...   torch.rand(200),
 ...   get_size_func=get_size_of_torch
 ... )
-848
+872
 ```
 
-However, this neglects the object's internal structure.
-The user can help `objsize` to find the object's hidden storage by supplying it with its own referent and filter
-functions:
+The above approach may neglect the object’s internal structure. The user
+can help `objsize` to find the object’s hidden storage by supplying it
+with its own referent and filter functions:
 
 ```python
 import objsize
 import gc
 import torch
 
-
 def get_referents_torch(*objs):
     # Yield all native referents
     yield from gc.get_referents(*objs)
-
     for o in objs:
         # If the object is a torch tensor, then also yield its storage
         if type(o) == torch.Tensor:
-            yield o.storage()
+            yield o.untyped_storage()
 
+# `torch.dtype` is a common object like Python's types.
+MySharedObjects = (*objsize.SharedObjectOrFunctionType, torch.dtype)
 
 def filter_func(o):
-    # Torch storage points to another meta storage that is
-    # already included in the outer storage calculation, 
-    # so we need to filter it.
-    # Also, `torch.dtype` is a common object like Python's types.
-    return not objsize.safe_is_instance(o, (
-        *objsize.SharedObjectOrFunctionType, torch.storage._UntypedStorage, torch.dtype
-    ))
+    return not objsize.safe_is_instance(o, MySharedObjects)
 ```
 
 Then use these as follows:
 
 ```pycon
->>> import torch
 >>> objsize.get_deep_size(
 ...   torch.rand(200),
-...   get_referents_func=get_referents_torch, 
+...   get_referents_func=get_referents_torch,
 ...   filter_func=filter_func
 ... )
-1024
+928
 ```
 
-## Case 2: `weakref`
+## Case 2: [`weakref`](https://docs.python.org/3/library/weakref.html#module-weakref)
 
-Using a simple calculation of the object size won't work for `weakref.proxy`.
+Using a simple calculation of the object size won’t work for
+`weakref.proxy`.
 
 ```pycon
->>> import weakref
->>> class Foo(list):
-...     pass
-... 
->>> o = Foo([0]*100)
+>>> from collections import UserList
+>>> o = UserList([0]*100)
 >>> objsize.get_deep_size(o)
-896
+1032
+>>> import weakref
 >>> o_ref = weakref.proxy(o)
 >>> objsize.get_deep_size(o_ref)
 72
 ```
 
-To mitigate this, you can provide a method that attempts to fetch the proxy's referents:
+To mitigate this, you can provide a method that attempts to fetch the
+proxy’s referents:
 
 ```python
 import weakref
 import gc
 
-
 def get_weakref_referents(*objs):
     yield from gc.get_referents(*objs)
-
     for o in objs:
         if type(o) in weakref.ProxyTypes:
             try:
                 yield o.__repr__.__self__
             except ReferenceError:
                 pass
 ```
 
 Then use it as follows:
 
 ```pycon
 >>> objsize.get_deep_size(o_ref, get_referents_func=get_weakref_referents)
-968
+1104
 ```
 
-After the referenced object will be collected, then the size of the proxy object will be reduced.
+After the referenced object will be collected, then the size of the
+proxy object will be reduced.
 
 ```pycon
 >>> del o
 >>> gc.collect()
->>> # Wait for the object to be collected 
+>>> # Wait for the object to be collected
 >>> objsize.get_deep_size(o_ref, get_referents_func=get_weakref_referents)
 72
 ```
 
+# Object Size Settings
+
+To avoid repeating the input settings when handling the special cases
+above, you can use the [`ObjSizeSettings`](https://liran-funaro.github.io/objsize/library/objsize.traverse.html#objsize.traverse.ObjSizeSettings) class.
+
+```pycon
+>>> torch_objsize = objsize.ObjSizeSettings(
+...   get_referents_func=get_referents_torch,
+...   filter_func=filter_func,
+... )
+>>> torch_objsize.get_deep_size(torch.rand(200))
+928
+>>> torch_objsize.get_deep_size(torch.rand(300))
+1328
+```
+
+See [`ObjSizeSettings`](https://liran-funaro.github.io/objsize/library/objsize.traverse.html#objsize.traverse.ObjSizeSettings) for the
+list of configurable parameters.
+
 # Traversal
 
-A user can implement its own function over the entire subtree using the traversal method, which traverses all the
-objects in the subtree.
+A user can implement its own function over the entire subtree using the
+traversal method, which traverses all the objects in the subtree.
 
 ```pycon
 >>> for o in objsize.traverse_bfs(my_obj):
 ...     print(o)
-... 
-MyClass
-{'x': [0, 1, 2], 'y': [3, 4, 5], 'd': {'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass}}
+...
+MyClass()
+{'x': [0, 1, 2], 'y': [3, 4, 5], 'd': {'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass()}}
 [0, 1, 2]
 [3, 4, 5]
-{'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass}
+{'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass()}
 2
 1
 0
 5
 4
 3
 ```
 
 Similar to before, non-exclusive objects can be ignored.
 
 ```pycon
 >>> for o in objsize.traverse_exclusive_bfs(my_obj):
 ...     print(o)
-... 
-MyClass
-{'x': [0, 1, 2], 'y': [3, 4, 5], 'd': {'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass}}
-{'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass}
+...
+MyClass()
+{'x': [0, 1, 2], 'y': [3, 4, 5], 'd': {'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass()}}
+{'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass()}
 ```
 
-# License
+# Alternative
+
+[Pympler](https://pythonhosted.org/Pympler/) also supports
+determining an object deep size via `pympler.asizeof()`. There are two
+main differences between `objsize` and `pympler`.
+
+1. `objsize` has additional features:
+   * Traversing the object subtree: iterating all the object’s
+     descendants one by one.
+   * Excluding non-exclusive objects. That is, objects that are also
+     referenced from somewhere else in the program. This is true for
+     calculating the object’s deep size and for traversing its
+     descendants.
+2. `objsize` has a simple and robust implementation with significantly
+   fewer lines of code, compared to `pympler`. The Pympler
+   implementation uses recursion, and thus have to use a maximal depth
+   argument to avoid reaching Python’s max depth. `objsize`, however,
+   uses BFS which is more efficient and simple to follow. Moreover, the
+   Pympler implementation carefully takes care of any object type.
+   `objsize` archives the same goal with a simple and generic
+   implementation, which has fewer lines of code.
+
+# License: BSD-3
+
+Copyright (c) 2006-2023, Liran Funaro.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright
+   notice, this list of conditions and the following disclaimer.
+2. Redistributions in binary form must reproduce the above copyright
+   notice, this list of conditions and the following disclaimer in the
+   documentation and/or other materials provided with the distribution.
+3. Neither the name of the copyright holder nor the
+   names of its contributors may be used to endorse or promote products
+   derived from this software without specific prior written permission.
 
-[BSD-3](LICENSE)
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS”
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGE.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `objsize-0.6.1/README.md` & `objsize-0.7.0/objsize.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,113 @@
-<!---
-Copyright (c) 2006-2022, Liran Funaro.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-1. Redistributions of source code must retain the above copyright
-   notice, this list of conditions and the following disclaimer.
-2. Redistributions in binary form must reproduce the above copyright
-   notice, this list of conditions and the following disclaimer in the
-   documentation and/or other materials provided with the distribution.
-3. Neither the name of the copyright holder nor the
-   names of its contributors may be used to endorse or promote products
-   derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
-LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
---->
+Metadata-Version: 2.1
+Name: objsize
+Version: 0.7.0
+Summary: Traversal over Python's objects subtree and calculate the total size of the subtree in bytes (deep size).
+Author-email: Liran Funaro <liran.funaro@gmail.com>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/liran-funaro/objsize
+Keywords: object-size,recursive,deep,traversal,object,size,debug,deep-object-size
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
 
 # objsize
 
-[![Coverage Status](https://coveralls.io/repos/github/liran-funaro/objsize/badge.svg?branch=master)](https://coveralls.io/github/liran-funaro/objsize?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/liran-funaro/objsize/badge.svg?branch=master)](https://coveralls.io/github/liran-funaro/objsize?branch=master) [![Downloads](https://static.pepy.tech/badge/objsize)](https://pepy.tech/project/objsize)
 
-Traversal over Python's objects subtree and calculate the total size of the subtree in bytes (deep size).
+The `objsize` Python package allows for the exploration and
+measurement of an object’s complete memory usage in bytes, including its
+child objects. This process, often referred to as deep size calculation,
+is achieved through Python’s internal Garbage Collection (GC) mechanism.
+
+The `objsize` package is designed to ignore shared objects, such as
+`None`, types, modules, classes, functions, and lambdas, because they
+are shared across many instances. One of the key performance features of
+`objsize` is that it avoids recursive calls, ensuring a faster and
+safer execution.
+
+## Key Features
+
+* Traverse objects’ subtree
+* Calculates the size of objects, including nested objects (deep size), in bytes
+* Exclude non-exclusive objects
+* Exclude specified objects subtree
+* Provides flexibility by allowing users to define custom handlers for:
+  - Object’s size calculation
+  - Object’s referents (i.e., its children)
+  - Object filter (skip specific objects)
 
-This module traverses all child objects using Python's internal GC implementation.
-It attempts to ignore shared objects (i.e., `None`, types, modules, classes, functions, lambdas), as they are common
-among all objects.
-It is implemented without recursive calls for high performance.
-
-# Features
-
-- Traverse objects' subtree
-- Calculate objects' (deep) size in bytes
-- Exclude non-exclusive objects
-- Exclude specified objects subtree
-- Allow the user to specify unique handlers for:
-    - Object's size calculation
-    - Object's referents (i.e., its children)
-    - Object filter (skip specific objects)
+## Documentation
 
-[Pympler](https://pythonhosted.org/Pympler/) also supports determining an object deep size via `pympler.asizeof()`.
-There are two main differences between `objsize` and `pympler`.
-
-1. `objsize` has additional features:
-    * Traversing the object subtree: iterating all the object's descendants one by one.
-    * Excluding non-exclusive objects. That is, objects that are also referenced from somewhere else in the program.
-      This is true for calculating the object's deep size and for traversing its descendants.
-2. `objsize` has a simple and robust implementation with significantly fewer lines of code, compared to `pympler`.
-   The Pympler implementation uses recursion, and thus have to use a maximal depth argument to avoid reaching Python's
-   max depth.
-   `objsize`, however, uses BFS which is more efficient and simple to follow.
-   Moreover, the Pympler implementation carefully takes care of any object type.
-   `objsize` archives the same goal with a simple and generic implementation, which has fewer lines of code.
+| [`objsize`](https://liran-funaro.github.io/objsize/library/objsize.html#module-objsize)   | Traversal over Python's objects subtree and calculating the total size of the subtree (deep size).   |
+|-------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
 
 # Install
 
 ```bash
-pip install objsize==0.6.1
+pip install objsize==0.7.0
 ```
 
 # Basic Usage
 
 Calculate the size of the object including all its members in bytes.
 
 ```pycon
 >>> import objsize
 >>> objsize.get_deep_size(dict(arg1='hello', arg2='world'))
 340
 ```
 
-It is possible to calculate the deep size of multiple objects by passing multiple arguments:
+It is possible to calculate the deep size of multiple objects by passing
+multiple arguments:
 
 ```pycon
 >>> objsize.get_deep_size(['hello', 'world'], dict(arg1='hello', arg2='world'), {'hello', 'world'})
 628
 ```
 
 # Complex Data
 
-`objsize` can calculate the size of an object's entire subtree in bytes regardless of the type of objects in it, and its
-depth.
+`objsize` can calculate the size of an object’s entire subtree in
+bytes regardless of the type of objects in it, and its depth.
 
-Here is a complex data structure, for example, that include a self reference:
+Here is a complex data structure, for example, that include a self
+reference:
 
 ```python
-my_data = (list(range(3)), list(range(3, 6)))
-
+my_data = list(range(3)), list(range(3, 6))
 
 class MyClass:
     def __init__(self, x, y):
         self.x = x
         self.y = y
         self.d = {'x': x, 'y': y, 'self': self}
 
     def __repr__(self):
-        return "MyClass"
-
+        return f"{self.__class__.__name__}()"
 
 my_obj = MyClass(*my_data)
 ```
 
 We can calculate `my_obj` deep size, including its stored data.
 
 ```pycon
 >>> objsize.get_deep_size(my_obj)
-708
+724
 ```
 
-We might want to ignore non-exclusive objects such as the ones stored in `my_data`.
+We might want to ignore non-exclusive objects such as the ones stored in
+`my_data`.
 
 ```pycon
 >>> objsize.get_deep_size(my_obj, exclude=[my_data])
 384
 ```
 
 Or simply let `objsize` detect that automatically:
@@ -128,203 +115,263 @@
 ```pycon
 >>> objsize.get_exclusive_deep_size(my_obj)
 384
 ```
 
 # Non Shared Functions or Classes
 
-`objsize` filters functions, lambdas, and classes by default since they are usually shared among many objects.
-For example:
+`objsize` filters functions, lambdas, and classes by default since
+they are usually shared among many objects. For example:
 
 ```pycon
 >>> method_dict = {"identity": lambda x: x, "double": lambda x: x*2}
 >>> objsize.get_deep_size(method_dict)
 232
 ```
 
-Some objects, however, as illustrated in the above example, have unique functions not shared by other objects.
-Due to this, it may be useful to count their sizes.
-You can achieve this by providing an alternative filter function.
+Some objects, however, as illustrated in the above example, have unique
+functions not shared by other objects. Due to this, it may be useful to
+count their sizes. You can achieve this by providing an alternative
+filter function.
 
 ```pycon
 >>> objsize.get_deep_size(method_dict, filter_func=objsize.shared_object_filter)
 986
 ```
 
 Notes:
 
-* The default filter function is `objsize.shared_object_or_function_filter`.
-* When using `objsize.shared_object_filter`, shared functions and lambdas are also counted, but builtin functions are
-  still excluded.
+* The default filter function is
+  [`objsize.traverse.shared_object_or_function_filter()`](https://liran-funaro.github.io/objsize/library/objsize.traverse.html#objsize.traverse.shared_object_or_function_filter).
+* When using [`objsize.traverse.shared_object_filter()`](https://liran-funaro.github.io/objsize/library/objsize.traverse.html#objsize.traverse.shared_object_filter), shared functions and
+  lambdas are also counted, but builtin functions are still excluded.
 
 # Special Cases
 
-Some objects handle their data in a way that prevents Python's GC from detecting it.
-The user can supply a special way to calculate the actual size of these objects.
+Some objects handle their data in a way that prevents Python’s GC from
+detecting it. The user can supply a special way to calculate the actual
+size of these objects.
 
-## Case 1: `torch`
+## Case 1: [`torch`](https://pytorch.org/docs/stable/torch.html#module-torch)
 
-Using a simple calculation of the object size won't work for `torch.Tensor`.
+Using a simple calculation of the object size won’t work for
+[`torch.Tensor`](https://pytorch.org/docs/stable/tensors.html#torch.Tensor).
 
 ```pycon
 >>> import torch
 >>> objsize.get_deep_size(torch.rand(200))
 72
 ```
 
 So the user can define its own size calculation handler for such cases:
 
 ```python
 import objsize
 import sys
 import torch
 
-
 def get_size_of_torch(o):
     # `objsize.safe_is_instance` catches `ReferenceError` caused by `weakref` objects
     if objsize.safe_is_instance(o, torch.Tensor):
-        return sys.getsizeof(o.storage())
+        return sys.getsizeof(o) + (o.element_size() * o.nelement())
     else:
         return sys.getsizeof(o)
 ```
 
 Then use it as follows:
 
 ```pycon
->>> import torch
 >>> objsize.get_deep_size(
 ...   torch.rand(200),
 ...   get_size_func=get_size_of_torch
 ... )
-848
+872
 ```
 
-However, this neglects the object's internal structure.
-The user can help `objsize` to find the object's hidden storage by supplying it with its own referent and filter
-functions:
+The above approach may neglect the object’s internal structure. The user
+can help `objsize` to find the object’s hidden storage by supplying it
+with its own referent and filter functions:
 
 ```python
 import objsize
 import gc
 import torch
 
-
 def get_referents_torch(*objs):
     # Yield all native referents
     yield from gc.get_referents(*objs)
-
     for o in objs:
         # If the object is a torch tensor, then also yield its storage
         if type(o) == torch.Tensor:
-            yield o.storage()
+            yield o.untyped_storage()
 
+# `torch.dtype` is a common object like Python's types.
+MySharedObjects = (*objsize.SharedObjectOrFunctionType, torch.dtype)
 
 def filter_func(o):
-    # Torch storage points to another meta storage that is
-    # already included in the outer storage calculation, 
-    # so we need to filter it.
-    # Also, `torch.dtype` is a common object like Python's types.
-    return not objsize.safe_is_instance(o, (
-        *objsize.SharedObjectOrFunctionType, torch.storage._UntypedStorage, torch.dtype
-    ))
+    return not objsize.safe_is_instance(o, MySharedObjects)
 ```
 
 Then use these as follows:
 
 ```pycon
->>> import torch
 >>> objsize.get_deep_size(
 ...   torch.rand(200),
-...   get_referents_func=get_referents_torch, 
+...   get_referents_func=get_referents_torch,
 ...   filter_func=filter_func
 ... )
-1024
+928
 ```
 
-## Case 2: `weakref`
+## Case 2: [`weakref`](https://docs.python.org/3/library/weakref.html#module-weakref)
 
-Using a simple calculation of the object size won't work for `weakref.proxy`.
+Using a simple calculation of the object size won’t work for
+`weakref.proxy`.
 
 ```pycon
->>> import weakref
->>> class Foo(list):
-...     pass
-... 
->>> o = Foo([0]*100)
+>>> from collections import UserList
+>>> o = UserList([0]*100)
 >>> objsize.get_deep_size(o)
-896
+1032
+>>> import weakref
 >>> o_ref = weakref.proxy(o)
 >>> objsize.get_deep_size(o_ref)
 72
 ```
 
-To mitigate this, you can provide a method that attempts to fetch the proxy's referents:
+To mitigate this, you can provide a method that attempts to fetch the
+proxy’s referents:
 
 ```python
 import weakref
 import gc
 
-
 def get_weakref_referents(*objs):
     yield from gc.get_referents(*objs)
-
     for o in objs:
         if type(o) in weakref.ProxyTypes:
             try:
                 yield o.__repr__.__self__
             except ReferenceError:
                 pass
 ```
 
 Then use it as follows:
 
 ```pycon
 >>> objsize.get_deep_size(o_ref, get_referents_func=get_weakref_referents)
-968
+1104
 ```
 
-After the referenced object will be collected, then the size of the proxy object will be reduced.
+After the referenced object will be collected, then the size of the
+proxy object will be reduced.
 
 ```pycon
 >>> del o
 >>> gc.collect()
->>> # Wait for the object to be collected 
+>>> # Wait for the object to be collected
 >>> objsize.get_deep_size(o_ref, get_referents_func=get_weakref_referents)
 72
 ```
 
+# Object Size Settings
+
+To avoid repeating the input settings when handling the special cases
+above, you can use the [`ObjSizeSettings`](https://liran-funaro.github.io/objsize/library/objsize.traverse.html#objsize.traverse.ObjSizeSettings) class.
+
+```pycon
+>>> torch_objsize = objsize.ObjSizeSettings(
+...   get_referents_func=get_referents_torch,
+...   filter_func=filter_func,
+... )
+>>> torch_objsize.get_deep_size(torch.rand(200))
+928
+>>> torch_objsize.get_deep_size(torch.rand(300))
+1328
+```
+
+See [`ObjSizeSettings`](https://liran-funaro.github.io/objsize/library/objsize.traverse.html#objsize.traverse.ObjSizeSettings) for the
+list of configurable parameters.
+
 # Traversal
 
-A user can implement its own function over the entire subtree using the traversal method, which traverses all the
-objects in the subtree.
+A user can implement its own function over the entire subtree using the
+traversal method, which traverses all the objects in the subtree.
 
 ```pycon
 >>> for o in objsize.traverse_bfs(my_obj):
 ...     print(o)
-... 
-MyClass
-{'x': [0, 1, 2], 'y': [3, 4, 5], 'd': {'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass}}
+...
+MyClass()
+{'x': [0, 1, 2], 'y': [3, 4, 5], 'd': {'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass()}}
 [0, 1, 2]
 [3, 4, 5]
-{'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass}
+{'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass()}
 2
 1
 0
 5
 4
 3
 ```
 
 Similar to before, non-exclusive objects can be ignored.
 
 ```pycon
 >>> for o in objsize.traverse_exclusive_bfs(my_obj):
 ...     print(o)
-... 
-MyClass
-{'x': [0, 1, 2], 'y': [3, 4, 5], 'd': {'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass}}
-{'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass}
+...
+MyClass()
+{'x': [0, 1, 2], 'y': [3, 4, 5], 'd': {'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass()}}
+{'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass()}
 ```
 
-# License
+# Alternative
+
+[Pympler](https://pythonhosted.org/Pympler/) also supports
+determining an object deep size via `pympler.asizeof()`. There are two
+main differences between `objsize` and `pympler`.
+
+1. `objsize` has additional features:
+   * Traversing the object subtree: iterating all the object’s
+     descendants one by one.
+   * Excluding non-exclusive objects. That is, objects that are also
+     referenced from somewhere else in the program. This is true for
+     calculating the object’s deep size and for traversing its
+     descendants.
+2. `objsize` has a simple and robust implementation with significantly
+   fewer lines of code, compared to `pympler`. The Pympler
+   implementation uses recursion, and thus have to use a maximal depth
+   argument to avoid reaching Python’s max depth. `objsize`, however,
+   uses BFS which is more efficient and simple to follow. Moreover, the
+   Pympler implementation carefully takes care of any object type.
+   `objsize` archives the same goal with a simple and generic
+   implementation, which has fewer lines of code.
+
+# License: BSD-3
 
-[BSD-3](LICENSE)
+Copyright (c) 2006-2023, Liran Funaro.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright
+   notice, this list of conditions and the following disclaimer.
+2. Redistributions in binary form must reproduce the above copyright
+   notice, this list of conditions and the following disclaimer in the
+   documentation and/or other materials provided with the distribution.
+3. Neither the name of the copyright holder nor the
+   names of its contributors may be used to endorse or promote products
+   derived from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS”
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGE.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `objsize-0.6.1/objsize.egg-info/PKG-INFO` & `objsize-0.7.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,144 +1,94 @@
-Metadata-Version: 2.1
-Name: objsize
-Version: 0.6.1
-Summary: Traversal over Python's objects subtree and calculate the total size of the subtree in bytes (deep size).
-Author-email: Liran Funaro <liran.funaro@gmail.com>
-License: BSD-3-Clause
-Project-URL: Homepage, https://github.com/liran-funaro/objsize
-Keywords: object-size,recursive,deep,traversal,object,size,debug,deep-object-size
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-<!---
-Copyright (c) 2006-2022, Liran Funaro.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-1. Redistributions of source code must retain the above copyright
-   notice, this list of conditions and the following disclaimer.
-2. Redistributions in binary form must reproduce the above copyright
-   notice, this list of conditions and the following disclaimer in the
-   documentation and/or other materials provided with the distribution.
-3. Neither the name of the copyright holder nor the
-   names of its contributors may be used to endorse or promote products
-   derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
-LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
---->
-
 # objsize
 
-[![Coverage Status](https://coveralls.io/repos/github/liran-funaro/objsize/badge.svg?branch=master)](https://coveralls.io/github/liran-funaro/objsize?branch=master)
-
-Traversal over Python's objects subtree and calculate the total size of the subtree in bytes (deep size).
+[![Coverage Status](https://coveralls.io/repos/github/liran-funaro/objsize/badge.svg?branch=master)](https://coveralls.io/github/liran-funaro/objsize?branch=master) [![Downloads](https://static.pepy.tech/badge/objsize)](https://pepy.tech/project/objsize)
 
-This module traverses all child objects using Python's internal GC implementation.
-It attempts to ignore shared objects (i.e., `None`, types, modules, classes, functions, lambdas), as they are common
-among all objects.
-It is implemented without recursive calls for high performance.
-
-# Features
-
-- Traverse objects' subtree
-- Calculate objects' (deep) size in bytes
-- Exclude non-exclusive objects
-- Exclude specified objects subtree
-- Allow the user to specify unique handlers for:
-    - Object's size calculation
-    - Object's referents (i.e., its children)
-    - Object filter (skip specific objects)
+The `objsize` Python package allows for the exploration and
+measurement of an object’s complete memory usage in bytes, including its
+child objects. This process, often referred to as deep size calculation,
+is achieved through Python’s internal Garbage Collection (GC) mechanism.
+
+The `objsize` package is designed to ignore shared objects, such as
+`None`, types, modules, classes, functions, and lambdas, because they
+are shared across many instances. One of the key performance features of
+`objsize` is that it avoids recursive calls, ensuring a faster and
+safer execution.
+
+## Key Features
+
+* Traverse objects’ subtree
+* Calculates the size of objects, including nested objects (deep size), in bytes
+* Exclude non-exclusive objects
+* Exclude specified objects subtree
+* Provides flexibility by allowing users to define custom handlers for:
+  - Object’s size calculation
+  - Object’s referents (i.e., its children)
+  - Object filter (skip specific objects)
 
-[Pympler](https://pythonhosted.org/Pympler/) also supports determining an object deep size via `pympler.asizeof()`.
-There are two main differences between `objsize` and `pympler`.
+## Documentation
 
-1. `objsize` has additional features:
-    * Traversing the object subtree: iterating all the object's descendants one by one.
-    * Excluding non-exclusive objects. That is, objects that are also referenced from somewhere else in the program.
-      This is true for calculating the object's deep size and for traversing its descendants.
-2. `objsize` has a simple and robust implementation with significantly fewer lines of code, compared to `pympler`.
-   The Pympler implementation uses recursion, and thus have to use a maximal depth argument to avoid reaching Python's
-   max depth.
-   `objsize`, however, uses BFS which is more efficient and simple to follow.
-   Moreover, the Pympler implementation carefully takes care of any object type.
-   `objsize` archives the same goal with a simple and generic implementation, which has fewer lines of code.
+| [`objsize`](https://liran-funaro.github.io/objsize/library/objsize.html#module-objsize)   | Traversal over Python's objects subtree and calculating the total size of the subtree (deep size).   |
+|-------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
 
 # Install
 
 ```bash
-pip install objsize==0.6.1
+pip install objsize==0.7.0
 ```
 
 # Basic Usage
 
 Calculate the size of the object including all its members in bytes.
 
 ```pycon
 >>> import objsize
 >>> objsize.get_deep_size(dict(arg1='hello', arg2='world'))
 340
 ```
 
-It is possible to calculate the deep size of multiple objects by passing multiple arguments:
+It is possible to calculate the deep size of multiple objects by passing
+multiple arguments:
 
 ```pycon
 >>> objsize.get_deep_size(['hello', 'world'], dict(arg1='hello', arg2='world'), {'hello', 'world'})
 628
 ```
 
 # Complex Data
 
-`objsize` can calculate the size of an object's entire subtree in bytes regardless of the type of objects in it, and its
-depth.
+`objsize` can calculate the size of an object’s entire subtree in
+bytes regardless of the type of objects in it, and its depth.
 
-Here is a complex data structure, for example, that include a self reference:
+Here is a complex data structure, for example, that include a self
+reference:
 
 ```python
-my_data = (list(range(3)), list(range(3, 6)))
-
+my_data = list(range(3)), list(range(3, 6))
 
 class MyClass:
     def __init__(self, x, y):
         self.x = x
         self.y = y
         self.d = {'x': x, 'y': y, 'self': self}
 
     def __repr__(self):
-        return "MyClass"
-
+        return f"{self.__class__.__name__}()"
 
 my_obj = MyClass(*my_data)
 ```
 
 We can calculate `my_obj` deep size, including its stored data.
 
 ```pycon
 >>> objsize.get_deep_size(my_obj)
-708
+724
 ```
 
-We might want to ignore non-exclusive objects such as the ones stored in `my_data`.
+We might want to ignore non-exclusive objects such as the ones stored in
+`my_data`.
 
 ```pycon
 >>> objsize.get_deep_size(my_obj, exclude=[my_data])
 384
 ```
 
 Or simply let `objsize` detect that automatically:
@@ -146,203 +96,263 @@
 ```pycon
 >>> objsize.get_exclusive_deep_size(my_obj)
 384
 ```
 
 # Non Shared Functions or Classes
 
-`objsize` filters functions, lambdas, and classes by default since they are usually shared among many objects.
-For example:
+`objsize` filters functions, lambdas, and classes by default since
+they are usually shared among many objects. For example:
 
 ```pycon
 >>> method_dict = {"identity": lambda x: x, "double": lambda x: x*2}
 >>> objsize.get_deep_size(method_dict)
 232
 ```
 
-Some objects, however, as illustrated in the above example, have unique functions not shared by other objects.
-Due to this, it may be useful to count their sizes.
-You can achieve this by providing an alternative filter function.
+Some objects, however, as illustrated in the above example, have unique
+functions not shared by other objects. Due to this, it may be useful to
+count their sizes. You can achieve this by providing an alternative
+filter function.
 
 ```pycon
 >>> objsize.get_deep_size(method_dict, filter_func=objsize.shared_object_filter)
 986
 ```
 
 Notes:
 
-* The default filter function is `objsize.shared_object_or_function_filter`.
-* When using `objsize.shared_object_filter`, shared functions and lambdas are also counted, but builtin functions are
-  still excluded.
+* The default filter function is
+  [`objsize.traverse.shared_object_or_function_filter()`](https://liran-funaro.github.io/objsize/library/objsize.traverse.html#objsize.traverse.shared_object_or_function_filter).
+* When using [`objsize.traverse.shared_object_filter()`](https://liran-funaro.github.io/objsize/library/objsize.traverse.html#objsize.traverse.shared_object_filter), shared functions and
+  lambdas are also counted, but builtin functions are still excluded.
 
 # Special Cases
 
-Some objects handle their data in a way that prevents Python's GC from detecting it.
-The user can supply a special way to calculate the actual size of these objects.
+Some objects handle their data in a way that prevents Python’s GC from
+detecting it. The user can supply a special way to calculate the actual
+size of these objects.
 
-## Case 1: `torch`
+## Case 1: [`torch`](https://pytorch.org/docs/stable/torch.html#module-torch)
 
-Using a simple calculation of the object size won't work for `torch.Tensor`.
+Using a simple calculation of the object size won’t work for
+[`torch.Tensor`](https://pytorch.org/docs/stable/tensors.html#torch.Tensor).
 
 ```pycon
 >>> import torch
 >>> objsize.get_deep_size(torch.rand(200))
 72
 ```
 
 So the user can define its own size calculation handler for such cases:
 
 ```python
 import objsize
 import sys
 import torch
 
-
 def get_size_of_torch(o):
     # `objsize.safe_is_instance` catches `ReferenceError` caused by `weakref` objects
     if objsize.safe_is_instance(o, torch.Tensor):
-        return sys.getsizeof(o.storage())
+        return sys.getsizeof(o) + (o.element_size() * o.nelement())
     else:
         return sys.getsizeof(o)
 ```
 
 Then use it as follows:
 
 ```pycon
->>> import torch
 >>> objsize.get_deep_size(
 ...   torch.rand(200),
 ...   get_size_func=get_size_of_torch
 ... )
-848
+872
 ```
 
-However, this neglects the object's internal structure.
-The user can help `objsize` to find the object's hidden storage by supplying it with its own referent and filter
-functions:
+The above approach may neglect the object’s internal structure. The user
+can help `objsize` to find the object’s hidden storage by supplying it
+with its own referent and filter functions:
 
 ```python
 import objsize
 import gc
 import torch
 
-
 def get_referents_torch(*objs):
     # Yield all native referents
     yield from gc.get_referents(*objs)
-
     for o in objs:
         # If the object is a torch tensor, then also yield its storage
         if type(o) == torch.Tensor:
-            yield o.storage()
+            yield o.untyped_storage()
 
+# `torch.dtype` is a common object like Python's types.
+MySharedObjects = (*objsize.SharedObjectOrFunctionType, torch.dtype)
 
 def filter_func(o):
-    # Torch storage points to another meta storage that is
-    # already included in the outer storage calculation, 
-    # so we need to filter it.
-    # Also, `torch.dtype` is a common object like Python's types.
-    return not objsize.safe_is_instance(o, (
-        *objsize.SharedObjectOrFunctionType, torch.storage._UntypedStorage, torch.dtype
-    ))
+    return not objsize.safe_is_instance(o, MySharedObjects)
 ```
 
 Then use these as follows:
 
 ```pycon
->>> import torch
 >>> objsize.get_deep_size(
 ...   torch.rand(200),
-...   get_referents_func=get_referents_torch, 
+...   get_referents_func=get_referents_torch,
 ...   filter_func=filter_func
 ... )
-1024
+928
 ```
 
-## Case 2: `weakref`
+## Case 2: [`weakref`](https://docs.python.org/3/library/weakref.html#module-weakref)
 
-Using a simple calculation of the object size won't work for `weakref.proxy`.
+Using a simple calculation of the object size won’t work for
+`weakref.proxy`.
 
 ```pycon
->>> import weakref
->>> class Foo(list):
-...     pass
-... 
->>> o = Foo([0]*100)
+>>> from collections import UserList
+>>> o = UserList([0]*100)
 >>> objsize.get_deep_size(o)
-896
+1032
+>>> import weakref
 >>> o_ref = weakref.proxy(o)
 >>> objsize.get_deep_size(o_ref)
 72
 ```
 
-To mitigate this, you can provide a method that attempts to fetch the proxy's referents:
+To mitigate this, you can provide a method that attempts to fetch the
+proxy’s referents:
 
 ```python
 import weakref
 import gc
 
-
 def get_weakref_referents(*objs):
     yield from gc.get_referents(*objs)
-
     for o in objs:
         if type(o) in weakref.ProxyTypes:
             try:
                 yield o.__repr__.__self__
             except ReferenceError:
                 pass
 ```
 
 Then use it as follows:
 
 ```pycon
 >>> objsize.get_deep_size(o_ref, get_referents_func=get_weakref_referents)
-968
+1104
 ```
 
-After the referenced object will be collected, then the size of the proxy object will be reduced.
+After the referenced object will be collected, then the size of the
+proxy object will be reduced.
 
 ```pycon
 >>> del o
 >>> gc.collect()
->>> # Wait for the object to be collected 
+>>> # Wait for the object to be collected
 >>> objsize.get_deep_size(o_ref, get_referents_func=get_weakref_referents)
 72
 ```
 
+# Object Size Settings
+
+To avoid repeating the input settings when handling the special cases
+above, you can use the [`ObjSizeSettings`](https://liran-funaro.github.io/objsize/library/objsize.traverse.html#objsize.traverse.ObjSizeSettings) class.
+
+```pycon
+>>> torch_objsize = objsize.ObjSizeSettings(
+...   get_referents_func=get_referents_torch,
+...   filter_func=filter_func,
+... )
+>>> torch_objsize.get_deep_size(torch.rand(200))
+928
+>>> torch_objsize.get_deep_size(torch.rand(300))
+1328
+```
+
+See [`ObjSizeSettings`](https://liran-funaro.github.io/objsize/library/objsize.traverse.html#objsize.traverse.ObjSizeSettings) for the
+list of configurable parameters.
+
 # Traversal
 
-A user can implement its own function over the entire subtree using the traversal method, which traverses all the
-objects in the subtree.
+A user can implement its own function over the entire subtree using the
+traversal method, which traverses all the objects in the subtree.
 
 ```pycon
 >>> for o in objsize.traverse_bfs(my_obj):
 ...     print(o)
-... 
-MyClass
-{'x': [0, 1, 2], 'y': [3, 4, 5], 'd': {'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass}}
+...
+MyClass()
+{'x': [0, 1, 2], 'y': [3, 4, 5], 'd': {'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass()}}
 [0, 1, 2]
 [3, 4, 5]
-{'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass}
+{'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass()}
 2
 1
 0
 5
 4
 3
 ```
 
 Similar to before, non-exclusive objects can be ignored.
 
 ```pycon
 >>> for o in objsize.traverse_exclusive_bfs(my_obj):
 ...     print(o)
-... 
-MyClass
-{'x': [0, 1, 2], 'y': [3, 4, 5], 'd': {'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass}}
-{'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass}
+...
+MyClass()
+{'x': [0, 1, 2], 'y': [3, 4, 5], 'd': {'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass()}}
+{'x': [0, 1, 2], 'y': [3, 4, 5], 'self': MyClass()}
 ```
 
-# License
+# Alternative
+
+[Pympler](https://pythonhosted.org/Pympler/) also supports
+determining an object deep size via `pympler.asizeof()`. There are two
+main differences between `objsize` and `pympler`.
+
+1. `objsize` has additional features:
+   * Traversing the object subtree: iterating all the object’s
+     descendants one by one.
+   * Excluding non-exclusive objects. That is, objects that are also
+     referenced from somewhere else in the program. This is true for
+     calculating the object’s deep size and for traversing its
+     descendants.
+2. `objsize` has a simple and robust implementation with significantly
+   fewer lines of code, compared to `pympler`. The Pympler
+   implementation uses recursion, and thus have to use a maximal depth
+   argument to avoid reaching Python’s max depth. `objsize`, however,
+   uses BFS which is more efficient and simple to follow. Moreover, the
+   Pympler implementation carefully takes care of any object type.
+   `objsize` archives the same goal with a simple and generic
+   implementation, which has fewer lines of code.
+
+# License: BSD-3
+
+Copyright (c) 2006-2023, Liran Funaro.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright
+   notice, this list of conditions and the following disclaimer.
+2. Redistributions in binary form must reproduce the above copyright
+   notice, this list of conditions and the following disclaimer in the
+   documentation and/or other materials provided with the distribution.
+3. Neither the name of the copyright holder nor the
+   names of its contributors may be used to endorse or promote products
+   derived from this software without specific prior written permission.
 
-[BSD-3](LICENSE)
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS”
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGE.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `objsize-0.6.1/objsize.py` & `objsize-0.7.0/objsize/traverse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,23 @@
 """
-Traversal over Python's objects subtree and calculating
-the total size of the subtree (deep size).
-
-Author: Liran Funaro <liran.funaro@gmail.com>
-
-Copyright (c) 2006-2022, Liran Funaro.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-1. Redistributions of source code must retain the above copyright
-   notice, this list of conditions and the following disclaimer.
-2. Redistributions in binary form must reproduce the above copyright
-   notice, this list of conditions and the following disclaimer in the
-   documentation and/or other materials provided with the distribution.
-3. Neither the name of the copyright holder nor the
-   names of its contributors may be used to endorse or promote products
-   derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
-LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
+Handling of traversal.
 """
 import collections
 import gc
 import inspect
 import sys
 import types
-from typing import Any, Iterable, Optional, Set
-
-__version__ = "0.6.1"
+import warnings
+from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Set, Tuple
 
 # Common type: a set of objects' ID
 MarkedSet = Set[int]
+FilterFunc = Callable[[Any], bool]
+GetReferentsFunc = Callable[..., Iterable[Any]]
+SizeFunc = Callable[[Any], int]
 
 SharedObjectType = (
     type,
     types.ModuleType,
     types.FrameType,
     types.BuiltinFunctionType,
 )
@@ -52,340 +25,360 @@
 SharedObjectOrFunctionType = (
     *SharedObjectType,
     types.FunctionType,
     types.LambdaType,
 )
 
 
-def safe_is_instance(o: Any, type_tuple) -> bool:
+def safe_is_instance(obj: Any, type_tuple) -> bool:
     """
     Return whether an object is an instance of a class or of a subclass thereof.
-    See `isinstance()` for more information.
+    See :py:func:`isinstance()` for more information.
 
-    Catches `ReferenceError` because applying `isinstance()` on `weakref.proxy`
+    Catches :class:`ReferenceError` because applying :py:func:`isinstance()` on :py:func:`weakref.proxy`
     objects attempts to dereference the proxy objects, which may yield an exception.
+
+    Parameters
+    ----------
+    obj :
+        Any object
+    type_tuple :
+        A type or a tuple of types
+
+    Returns
+    -------
+    bool
+        True if the objects matches one of the types
     """
     try:
-        return isinstance(o, type_tuple)
+        return isinstance(obj, type_tuple)
     except ReferenceError:
         return False
 
 
-def shared_object_or_function_filter(o: Any) -> bool:
+def shared_object_or_function_filter(obj: Any) -> bool:
     """Filters objects that are likely to be shared among many objects."""
-    return not safe_is_instance(o, SharedObjectOrFunctionType)
+    return not safe_is_instance(obj, SharedObjectOrFunctionType)
 
 
-def shared_object_filter(o: Any) -> bool:
+def shared_object_filter(obj: Any) -> bool:
     """Filters objects that are likely to be shared among many objects, but includes functions and lambdas."""
-    return not safe_is_instance(o, SharedObjectType)
+    return not safe_is_instance(obj, SharedObjectType)
 
 
-# See https://docs.python.org/3/library/gc.html#gc.get_referents
 default_get_referents = gc.get_referents
-# See https://docs.python.org/3/library/sys.html#sys.getsizeof
-default_get_size = sys.getsizeof
-# By default, we filter shared objects, i.e., types, modules, functions, and lambdas
+"""See https://docs.python.org/3/library/gc.html#gc.get_referents"""
 default_object_filter = shared_object_or_function_filter
+"""By default, we filter shared objects, i.e., types, modules, functions, and lambdas"""
+default_get_size = sys.getsizeof
+"""See https://docs.python.org/3/library/sys.html#sys.getsizeof"""
 
 
-def get_exclude_set(
-    exclude: Optional[Iterable] = None,
-    exclude_set: Optional[MarkedSet] = None,
-    get_referents_func=default_get_referents,
-    filter_func=default_object_filter,
-) -> Optional[set]:
-    """
-    Traverse all the arguments' subtree without ingesting the result, just to update the `marked_set`.
-    See `traverse_bfs()` for more information.
-
-    Parameters
-    ----------
-    exclude : iterable, optional
-        One or more object(s).
-    exclude_set : set, optional
-        See `traverse_bfs()`.
-    get_referents_func : callable
-        See `traverse_bfs()`.
-    filter_func : callable
-        See `traverse_bfs()`.
-
-    Returns
-    -------
-    The updated exclude-set.
-    """
-    if exclude_set is None:
-        exclude_set = set()
-    if exclude is None:
-        return exclude_set
-    it = traverse_bfs(
-        *exclude,
-        marked_set=exclude_set,
-        exclude_set=exclude_set,
-        get_referents_func=get_referents_func,
-        filter_func=filter_func,
-    )
-    collections.deque(it, maxlen=0)
-    return exclude_set
-
-
-def __iter_modules_globals():
+def _iter_modules_globals():
     modules = list(sys.modules.values())
-    for m in modules:
+    for mod in modules:
         try:
-            yield vars(m)
+            yield vars(mod)
         except TypeError:
             pass
 
 
-def traverse_bfs(
-    *objs,
-    exclude: Optional[Iterable] = None,
-    marked_set: Optional[MarkedSet] = None,
-    exclude_set: Optional[MarkedSet] = None,
-    get_referents_func=default_get_referents,
-    filter_func=default_object_filter,
-) -> Iterable[Any]:
-    """
-    Traverse all the arguments' subtree.
-    By default, this excludes shared objects, i.e., types, modules, functions, and lambdas.
+def _default(optional_value, default_value):
+    if optional_value is None:
+        return default_value
+    return optional_value
 
-    Parameters
-    ----------
-    objs : object(s)
-        One or more object(s).
-    exclude : iterable, optional
-        Objects that will be excluded from this calculation, as well as their subtrees.
-    marked_set : set, optional
-        An existing set of marked objects' ID, i.e., `id(obj)`.
-        Objects that their ID is in this set will not be traversed.
-        If a set is given, it will be updated with all the traversed objects' ID.
-    exclude_set : set, optional
-        Similar to the marked set, but contains excluded objects' ID.
-    get_referents_func : callable
-        Receives any number of objects and returns iterable over the objects that are referred by these objects.
-        Default: `gc.get_referents()`.
-        See: https://docs.python.org/3/library/gc.html#gc.get_referents
-    filter_func : callable
-        Receives an objects and return `True` if the object---and its subtree---should be traversed.
-        Default: `objsize.shared_object_filter`.
-
-    Yields
-    ------
-    object
-        The traversed objects, one by one.
-    """
-    if marked_set is None:
-        marked_set = set()
-    if exclude_set is None:
-        exclude_set = set()
-
-    # None shouldn't be included in size calculations because it is a singleton
-    exclude_set.add(id(None))
-    # Modules' "globals" should not be included as they are shared
-    exclude_set.update(map(id, __iter_modules_globals()))
-
-    exclude_set = get_exclude_set(
-        exclude,
-        exclude_set=exclude_set,
-        get_referents_func=get_referents_func,
-        filter_func=filter_func,
-    )
-
-    while objs:
-        # Get the object's ids
-        objs = ((id(o), o) for o in objs)
-
-        # Filter:
-        #  - Object that are already marked/excluded (using the marked-set/exclude-set).
-        #  - Objects that are filtered by the given filter function (see above).
-        #  - Repeated objects (using dict notation).
-        objs = {
-            o_id: o
-            for o_id, o in objs
-            if o_id not in marked_set and o_id not in exclude_set and filter_func(o)
-        }
-
-        # We stop when there are no new valid objects to traverse.
-        if not objs:
-            break
-
-        # Update the marked set with the ids, so we will not traverse them again.
-        marked_set.update(objs.keys())
-
-        # Yield traversed objects
-        yield from objs.values()
-
-        # Lookup all the object referred to by the object from the current round.
-        objs = get_referents_func(*objs.values())
-
-
-def traverse_exclusive_bfs(
-    *objs,
-    exclude: Optional[Iterable] = None,
-    marked_set: Optional[MarkedSet] = None,
-    exclude_set: Optional[MarkedSet] = None,
-    get_referents_func=default_get_referents,
-    filter_func=default_object_filter,
-) -> Iterable[Any]:
-    """
-    Traverse all the arguments' subtree, excluding non-exclusive objects.
-    That is, objects that are referenced by objects that are not in this subtree.
 
-    Parameters
-    ----------
-    objs : object(s)
-        One or more object(s).
-    exclude : iterable, optional
-        See `traverse_bfs()`.
-    marked_set : set, optional
-        See `traverse_bfs()`.
-    exclude_set : set, optional
-        See `traverse_bfs()`.
-    get_referents_func : callable
-        See `traverse_bfs()`.
-    filter_func : callable
-        See `traverse_bfs()`.
-
-    Yields
-    ------
-    object
-        The traversed objects, one by one.
-
-    See Also
-    --------
-    traverse_bfs : to understand which objects are traversed.
-    """
-    if marked_set is None:
-        marked_set = set()
-    if exclude_set is None:
-        exclude_set = set()
-
-    # The arguments are considered the root objects, which we include
-    # regardless of their exclusiveness.
-    root_obj_ids = set(map(id, objs))
-
-    # We have to complete the entire traverse, so we will have
-    # a complete marked set.
-    subtree = tuple(
-        traverse_bfs(
-            *objs,
-            exclude=exclude,
-            marked_set=marked_set,
-            exclude_set=exclude_set,
-            get_referents_func=get_referents_func,
-            filter_func=filter_func,
-        )
-    )
+def _default_generator(optional_value, default_value_generator):
+    if optional_value is None:
+        return default_value_generator()
+    return optional_value
 
-    # We keep the current frame and `subtree` objects in addition to the marked-set because they refer to objects
-    # in our subtree which may cause them to appear non-exclusive.
-    # `objs` should not be added as it only refers to the root objects.
-    frame_set = marked_set | {id(inspect.currentframe()), id(subtree)}
-
-    # We first make sure that any "old" objects that may refer to our subtree were collected.
-    gc.collect()
-
-    # Test for each object that all the object that refer to it is in the marked-set, frame-set, or is a root
-    # See: https://docs.python.org/3.7/library/gc.html#gc.get_referrers
-    for o in subtree:
-        if id(o) in root_obj_ids or frame_set.issuperset(map(id, gc.get_referrers(o))):
-            yield o
-
-
-def get_deep_size(
-    *objs,
-    exclude: Optional[Iterable] = None,
-    marked_set: Optional[MarkedSet] = None,
-    exclude_set: Optional[MarkedSet] = None,
-    get_size_func=default_get_size,
-    get_referents_func=default_get_referents,
-    filter_func=default_object_filter,
-) -> int:
+
+class ObjSizeSettings:
     """
-    Calculates the deep size of all the arguments.
+    Object traversal and size settings.
 
     Parameters
     ----------
-    objs : object(s)
-        One or more object(s).
-    exclude : iterable, optional
-        Objects that will be excluded from this calculation, as well as their subtrees.
-    marked_set : set, optional
-        See `traverse_bfs()`.
-    exclude_set : set, optional
-        See `traverse_bfs()`.
-    get_size_func : function, optional
+    filter_func :
+        Receives an objects and return :py:obj:`True` if the object---and its subtree---should be traversed.
+        Default: :py:func:`shared_object_filter`.
+        By default, this excludes shared objects, i.e., types, modules, functions, and lambdas.
+    get_referents_func :
+        Receives any number of objects and returns iterable over the objects that are referred by these objects.
+        Default: :py:func:`gc.get_referents`.
+    get_size_func :
         A function that determines the object size.
-        Default: `sys.getsizeof()`
-    get_referents_func : callable
-        See `traverse_bfs()`.
-    filter_func : callable
-        See `traverse_bfs()`.
+        Default: :py:func:`sys.getsizeof`.
+    exclude :
+        Objects that will be excluded from this calculation, as well as their subtrees.
+    exclude_modules_globals :
+        If True (default), loaded modules globals will be added to the
+        :py:attr:`~TraversalContext.exclude_set`.
+    """
+
+    def __init__(
+        self,
+        get_referents_func: Optional[GetReferentsFunc] = None,
+        filter_func: Optional[FilterFunc] = None,
+        get_size_func: Optional[SizeFunc] = None,
+        exclude: Optional[Iterable] = None,
+        exclude_modules_globals: Optional[bool] = None,
+    ):
+        self.get_referents_func = _default(get_referents_func, default_get_referents)
+        self.filter_func = _default(filter_func, default_object_filter)
+        self.get_size_func = _default(get_size_func, default_get_size)
+        self.exclude = _default(exclude, None)
+        self.exclude_modules_globals = _default(exclude_modules_globals, True)
+
+    def replace(
+        self,
+        get_referents_func: Optional[GetReferentsFunc] = None,
+        filter_func: Optional[FilterFunc] = None,
+        get_size_func: Optional[SizeFunc] = None,
+        exclude: Optional[Iterable] = None,
+        exclude_modules_globals: Optional[bool] = None,
+    ) -> "ObjSizeSettings":
+        """
+        Replaces some of the settings into a new settings object.
+
+        Returns
+        -------
+            A new settings instance
+        """
+        return ObjSizeSettings(
+            get_referents_func=_default(get_referents_func, self.get_referents_func),
+            filter_func=_default(filter_func, self.filter_func),
+            get_size_func=_default(get_size_func, self.get_size_func),
+            exclude=_default(exclude, self.exclude),
+            exclude_modules_globals=_default(exclude_modules_globals, self.exclude_modules_globals),
+        )
 
-    Returns
-    -------
-    int
-        The objects' deep size in bytes.
+    def update(
+        self,
+        get_referents_func: Optional[GetReferentsFunc] = None,
+        filter_func: Optional[FilterFunc] = None,
+        get_size_func: Optional[SizeFunc] = None,
+        exclude: Optional[Iterable] = None,
+        exclude_modules_globals: Optional[bool] = None,
+    ):
+        """
+        Updates some of the settings in place.
+        """
+        self.get_referents_func = _default(get_referents_func, self.get_referents_func)
+        self.filter_func = _default(filter_func, self.filter_func)
+        self.get_size_func = _default(get_size_func, self.get_size_func)
+        self.exclude = _default(exclude, self.exclude)
+        self.exclude_modules_globals = _default(exclude_modules_globals, self.exclude_modules_globals)
+
+    def new_context(self, *, marked_set: Optional[MarkedSet] = None, exclude_set: Optional[MarkedSet] = None):
+        """See :py:class:`TraversalContext`."""
+        return TraversalContext(self, marked_set, exclude_set)
+
+    def traverse_bfs(
+        self, *objs: Any, marked_set: Optional[MarkedSet] = None, exclude_set: Optional[MarkedSet] = None
+    ) -> Iterator[Any]:
+        """See :py:meth:`TraversalContext.traverse_bfs`"""
+        yield from self.new_context(marked_set=marked_set, exclude_set=exclude_set).traverse_bfs(*objs)
+
+    def traverse_exclusive_bfs(
+        self, *objs: Any, marked_set: Optional[MarkedSet] = None, exclude_set: Optional[MarkedSet] = None
+    ) -> Iterator[Any]:
+        """See :py:meth:`TraversalContext.traverse_exclusive_bfs`"""
+        yield from self.new_context(marked_set=marked_set, exclude_set=exclude_set).traverse_exclusive_bfs(*objs)
+
+    def get_deep_size(
+        self, *objs: Any, marked_set: Optional[MarkedSet] = None, exclude_set: Optional[MarkedSet] = None
+    ) -> int:
+        """See :py:meth:`TraversalContext.get_deep_size`"""
+        return self.new_context(marked_set=marked_set, exclude_set=exclude_set).get_deep_size(*objs)
+
+    def get_exclusive_deep_size(
+        self, *objs: Any, marked_set: Optional[MarkedSet] = None, exclude_set: Optional[MarkedSet] = None
+    ) -> int:
+        """See :py:meth:`TraversalContext.get_exclusive_deep_size`"""
+        return self.new_context(marked_set=marked_set, exclude_set=exclude_set).get_exclusive_deep_size(*objs)
 
-    See Also
-    --------
-    traverse_bfs : to understand which objects are traversed.
-    """
-    it = traverse_bfs(
-        *objs,
-        exclude=exclude,
-        marked_set=marked_set,
-        exclude_set=exclude_set,
-        get_referents_func=get_referents_func,
-        filter_func=filter_func,
-    )
-    return sum(map(get_size_func, it))
-
-
-def get_exclusive_deep_size(
-    *objs,
-    exclude: Optional[Iterable] = None,
-    marked_set: Optional[MarkedSet] = None,
-    exclude_set: Optional[MarkedSet] = None,
-    get_size_func=default_get_size,
-    get_referents_func=default_get_referents,
-    filter_func=default_object_filter,
-) -> int:
+
+class TraversalContext:
     """
-    Calculates the deep size of all the arguments, excluding non-exclusive objects.
+    Object traversal context.
 
     Parameters
     ----------
-    objs : object(s)
-        One or more object(s).
-    exclude : iterable, optional
-        See `get_deep_size()`.
-    marked_set : set, optional
-        See `traverse_bfs()`.
-    exclude_set : set, optional
-        See `traverse_bfs()`.
-    get_size_func : function, optional
-        See `get_deep_size()`.
-    get_referents_func : callable
-        See `traverse_bfs()`.
-    filter_func : callable
-        See `traverse_bfs()`.
-
-    Returns
-    -------
-    int
-        The objects' deep size in bytes.
-
-    See Also
-    --------
-    traverse_exclusive_bfs : to understand which objects are traversed.
+    settings :
+        See :py:class:`ObjSizeSettings`
+    marked_set :
+        An existing set of marked objects' ID, i.e., `id(obj)`.
+        Objects that their ID is in this set will not be traversed.
+        If a set is given, it will be updated with all the traversed objects' ID.
+    exclude_set :
+        Similar to the marked set, but contains excluded objects' ID.
     """
-    it = traverse_exclusive_bfs(
-        *objs,
-        exclude=exclude,
-        marked_set=marked_set,
-        exclude_set=exclude_set,
-        get_referents_func=get_referents_func,
-        filter_func=filter_func,
-    )
-    return sum(map(get_size_func, it))
+
+    def __init__(
+        self,
+        settings: Optional[ObjSizeSettings] = None,
+        marked_set: Optional[MarkedSet] = None,
+        exclude_set: Optional[MarkedSet] = None,
+    ):
+        if marked_set is not None or exclude_set is not None:
+            warnings.warn(
+                "marked_set and exclude_set parameters are deprecated. They will be removed on version 1.0.0. "
+                "Please use objsize.traverse.TraversalContext(settings) instead.",
+                DeprecationWarning,
+            )
+        self.settings = _default_generator(settings, ObjSizeSettings)
+        self.marked_set = _default_generator(marked_set, set)
+        self.exclude_set = _default_generator(exclude_set, set)
+        self._update_exclude_set()
+
+    def _update_exclude_set(self):
+        """
+        Traverse all the excluded subtree without ingesting the result, just to update the `exclude_set`.
+        See `traverse_bfs()` for more information.
+        """
+        # None shouldn't be included in size calculations because it is a singleton
+        self.exclude_set.add(id(None))
+
+        if self.settings.exclude_modules_globals:
+            # Modules' "globals" should not be included as they are shared
+            self.exclude_set.update(map(id, _iter_modules_globals()))
+
+        if self.settings.exclude is not None:
+            collections.deque(self.traverse_bfs(*self.settings.exclude, exclude=True), maxlen=0)
+
+    def _obj_filter_iterator(self, obj_it: Iterable[Any]) -> Iterator[Tuple[int, Any]]:
+        """
+        Filters the input. Only yields objects such that:
+         - Object ID was not already marked/excluded (using the marked-set/exclude-set).
+         - Object pass the given filter function (see above).
+        """
+        for obj in obj_it:
+            obj_id = id(obj)
+            if obj_id not in self.marked_set and obj_id not in self.exclude_set and self.settings.filter_func(obj):
+                yield obj_id, obj
+
+    def _filter(self, obj_it: Iterable[Any]) -> Dict[int, Any]:
+        """Apply filter, and screen repeated objects (using dict notation)."""
+        return dict(self._obj_filter_iterator(obj_it))
+
+    def traverse_bfs(self, *objs: Any, exclude=False) -> Iterator[Any]:
+        """
+        Traverse all the arguments' subtree.
+
+        Parameters
+        ----------
+        objs : object(s)
+            One or more object(s).
+        exclude: bool
+            If true, all objects will be added to the exclude set.
+
+        Yields
+        ------
+        object
+            The traversed objects, one by one.
+        """
+        if not exclude:
+            marked_set = self.marked_set
+        else:
+            marked_set = self.exclude_set
+
+        obj_it: Iterable[Any] = iter(objs)
+
+        while obj_it:
+            # Apply filter, and screen repeated objects.
+            objs_map = self._filter(obj_it)
+
+            # We stop when there are no new valid objects to traverse.
+            if not objs_map:
+                break
+
+            # Update the marked set with the ids, so we will not traverse them again.
+            marked_set.update(objs_map.keys())
+
+            # Yield traversed objects
+            yield from objs_map.values()
+
+            # Lookup all the object referred to by the object from the current round.
+            obj_it = self.settings.get_referents_func(*objs_map.values())
+
+    def traverse_exclusive_bfs(self, *objs: Any) -> Iterator[Any]:
+        """
+        Traverse all the arguments' subtree, excluding non-exclusive objects.
+        That is, objects that are referenced by objects that are not in this subtree.
+
+        Parameters
+        ----------
+        objs : object(s)
+            One or more object(s).
+
+        Yields
+        ------
+        object
+            The traversed objects, one by one.
+
+        See Also
+        --------
+        :py:meth:`traverse_bfs` : to understand which objects are traversed.
+        """
+        # The arguments are considered the root objects, which we include regardless of their exclusiveness.
+        root_obj_ids = set(map(id, objs))
+
+        # We have to complete the entire traverse, so we will have a complete marked set.
+        subtree = tuple(self.traverse_bfs(*objs))
+
+        # We keep the current frame and `subtree` objects in addition to the marked-set because they refer to objects
+        # in our subtree which may cause them to appear non-exclusive.
+        # `objs` should not be added as it only refers to the root objects.
+        frame_set = self.marked_set | {id(inspect.currentframe()), id(subtree)}
+
+        # We first make sure that any "old" objects that may refer to our subtree were collected.
+        gc.collect()
+
+        # Test for each object that all the object that refer to it is in the marked-set, frame-set, or is a root
+        # See: https://docs.python.org/3.7/library/gc.html#gc.get_referrers
+        for obj in subtree:
+            if id(obj) in root_obj_ids or frame_set.issuperset(map(id, gc.get_referrers(obj))):
+                yield obj
+
+    def get_deep_size(self, *objs: Any) -> int:
+        """
+        Calculates the deep size of all the arguments.
+
+        Parameters
+        ----------
+        objs : object(s)
+            One or more object(s).
+
+        Returns
+        -------
+        int
+            The objects' deep size in bytes.
+
+        See Also
+        --------
+        :py:func:`~objsize.traverse.TraversalContext.traverse_bfs` : to understand which objects are traversed.
+        """
+        return sum(map(self.settings.get_size_func, self.traverse_bfs(*objs)))
+
+    def get_exclusive_deep_size(self, *objs: Any) -> int:
+        """
+        Calculates the deep size of all the arguments, excluding non-exclusive objects.
+
+        Parameters
+        ----------
+        objs : object(s)
+            One or more object(s).
+
+        Returns
+        -------
+        int
+            The objects' deep size in bytes.
+
+        See Also
+        --------
+        :py:func:`~objsize.traverse.TraversalContext.traverse_exclusive_bfs` :
+            to understand which objects are traversed.
+        """
+        return sum(map(self.settings.get_size_func, self.traverse_exclusive_bfs(*objs)))
```

