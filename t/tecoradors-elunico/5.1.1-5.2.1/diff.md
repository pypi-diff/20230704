# Comparing `tmp/tecoradors-elunico-5.1.1.tar.gz` & `tmp/tecoradors-elunico-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tecoradors-elunico-5.1.1.tar", last modified: Thu Apr  6 17:23:48 2023, max compression
+gzip compressed data, was "tecoradors-elunico-5.2.1.tar", last modified: Tue Jul  4 17:56:52 2023, max compression
```

## Comparing `tecoradors-elunico-5.1.1.tar` & `tecoradors-elunico-5.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-04-06 17:23:48.955489 tecoradors-elunico-5.1.1/
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1073 2023-02-25 18:38:36.000000 tecoradors-elunico-5.1.1/LICENSE
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      100 2023-02-25 18:38:36.000000 tecoradors-elunico-5.1.1/MANIFEST.in
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1136 2023-04-06 17:23:48.955114 tecoradors-elunico-5.1.1/PKG-INFO
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      672 2023-04-06 17:15:06.000000 tecoradors-elunico-5.1.1/README.md
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      103 2023-02-25 18:38:36.000000 tecoradors-elunico-5.1.1/pyproject.toml
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)       38 2023-04-06 17:23:48.955620 tecoradors-elunico-5.1.1/setup.cfg
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      729 2023-04-06 17:23:26.000000 tecoradors-elunico-5.1.1/setup.py
-drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-04-06 17:23:48.952436 tecoradors-elunico-5.1.1/tecoradors/
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      701 2023-04-06 17:23:18.000000 tecoradors-elunico-5.1.1/tecoradors/__init__.py
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)    35403 2023-04-05 15:30:25.000000 tecoradors-elunico-5.1.1/tecoradors/tecoradors.py
-drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-04-06 17:23:48.954262 tecoradors-elunico-5.1.1/tecoradors_elunico.egg-info/
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1136 2023-04-06 17:23:48.000000 tecoradors-elunico-5.1.1/tecoradors_elunico.egg-info/PKG-INFO
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      282 2023-04-06 17:23:48.000000 tecoradors-elunico-5.1.1/tecoradors_elunico.egg-info/SOURCES.txt
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)        1 2023-04-06 17:23:48.000000 tecoradors-elunico-5.1.1/tecoradors_elunico.egg-info/dependency_links.txt
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)       11 2023-04-06 17:23:48.000000 tecoradors-elunico-5.1.1/tecoradors_elunico.egg-info/top_level.txt
-drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-04-06 17:23:48.954620 tecoradors-elunico-5.1.1/test/
--rw-r--r--   0 thomaspovinelli   (501) staff       (20)      340 2023-04-06 17:22:28.000000 tecoradors-elunico-5.1.1/test/test.py
+drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-07-04 17:56:52.750229 tecoradors-elunico-5.2.1/
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1073 2023-02-25 18:38:36.000000 tecoradors-elunico-5.2.1/LICENSE
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      100 2023-02-25 18:38:36.000000 tecoradors-elunico-5.2.1/MANIFEST.in
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1180 2023-07-04 17:56:52.749932 tecoradors-elunico-5.2.1/PKG-INFO
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      716 2023-07-04 17:51:52.000000 tecoradors-elunico-5.2.1/README.md
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      103 2023-02-25 18:38:36.000000 tecoradors-elunico-5.2.1/pyproject.toml
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)       38 2023-07-04 17:56:52.750330 tecoradors-elunico-5.2.1/setup.cfg
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      729 2023-07-04 17:56:44.000000 tecoradors-elunico-5.2.1/setup.py
+drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-07-04 17:56:52.747086 tecoradors-elunico-5.2.1/tecoradors/
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      701 2023-04-06 17:23:18.000000 tecoradors-elunico-5.2.1/tecoradors/__init__.py
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)    40619 2023-07-04 17:53:31.000000 tecoradors-elunico-5.2.1/tecoradors/tecoradors.py
+drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-07-04 17:56:52.748963 tecoradors-elunico-5.2.1/tecoradors_elunico.egg-info/
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)     1180 2023-07-04 17:56:52.000000 tecoradors-elunico-5.2.1/tecoradors_elunico.egg-info/PKG-INFO
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      282 2023-07-04 17:56:52.000000 tecoradors-elunico-5.2.1/tecoradors_elunico.egg-info/SOURCES.txt
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)        1 2023-07-04 17:56:52.000000 tecoradors-elunico-5.2.1/tecoradors_elunico.egg-info/dependency_links.txt
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)       11 2023-07-04 17:56:52.000000 tecoradors-elunico-5.2.1/tecoradors_elunico.egg-info/top_level.txt
+drwxr-xr-x   0 thomaspovinelli   (501) staff       (20)        0 2023-07-04 17:56:52.749278 tecoradors-elunico-5.2.1/test/
+-rw-r--r--   0 thomaspovinelli   (501) staff       (20)      341 2023-04-06 17:24:39.000000 tecoradors-elunico-5.2.1/test/test.py
```

### Comparing `tecoradors-elunico-5.1.1/LICENSE` & `tecoradors-elunico-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tecoradors-elunico-5.1.1/PKG-INFO` & `tecoradors-elunico-5.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecoradors-elunico
-Version: 5.1.1
+Version: 5.2.1
 Summary: A small collection of decorators I like to use often
 Home-page: https://github.com/elunico/tecoradors
 Author: Thomas Povinelli
 Author-email: tompov227@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,16 @@
 [Find the pypi package here](https://pypi.org/project/tecoradors-elunico/)
 
 Named based on my name which starts with a T. You can find more information reading the docstrings of the functions
 
 ### Decorators are
   *  accepts
   *  json_serializable
+  *  builder
+  *  tattle
   *  spread
   *  timed
   *  squash
   *  stringable
   *  equatable
   *  hashable
   *  dataclass
@@ -42,7 +44,8 @@
   *  lazy
   *  precompute
 
 ### Support from types
   *  Self
   *  PrecomputeStorage
   *  NoSuchValue
+  *  TattleOptions
```

### Comparing `tecoradors-elunico-5.1.1/README.md` & `tecoradors-elunico-5.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 [Find the pypi package here](https://pypi.org/project/tecoradors-elunico/)
 
 Named based on my name which starts with a T. You can find more information reading the docstrings of the functions
 
 ### Decorators are
   *  accepts
   *  json_serializable
+  *  builder
+  *  tattle
   *  spread
   *  timed
   *  squash
   *  stringable
   *  equatable
   *  hashable
   *  dataclass
@@ -28,7 +30,8 @@
   *  lazy
   *  precompute
 
 ### Support from types
   *  Self
   *  PrecomputeStorage
   *  NoSuchValue
+  *  TattleOptions
```

### Comparing `tecoradors-elunico-5.1.1/setup.py` & `tecoradors-elunico-5.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tecoradors-elunico",
-    version="5.1.1",
+    version="5.2.1",
     author="Thomas Povinelli",
     author_email="tompov227@gmail.com",
     description="A small collection of decorators I like to use often",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/elunico/tecoradors",
```

### Comparing `tecoradors-elunico-5.1.1/tecoradors/__init__.py` & `tecoradors-elunico-5.2.1/tecoradors/__init__.py`

 * *Files identical despite different names*

### Comparing `tecoradors-elunico-5.1.1/tecoradors/tecoradors.py` & `tecoradors-elunico-5.2.1/tecoradors/tecoradors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import enum
 import functools
 import inspect
-import typing
 import sys
+import typing
 
 
 # taken from https://stackoverflow.com/questions/3589311/get-defining-class-of-unbound-method-object-in-python-3
 def _get_class_that_defined_method(meth):
     if isinstance(meth, functools.partial):
         return _get_class_that_defined_method(meth.func)
     if inspect.ismethod(meth) or (
@@ -334,14 +334,140 @@
             return results
 
         return wrapper
 
     return inner
 
 
+def builder(typechecking=True):
+    """
+    The builder decorator allows you to create builder classes based on the desired attributes and optionally types.
+
+    You can define a class with attributes and types and decorate with the builder decorator and you will get
+        -  An __init__ that takes no arguments and initializes all fields to None
+        -  A setX method for every attribute defined in the class which sets the corresponding field and returns self
+
+    If you decorate a class @builder you get type checking by default. This is equivalent to @builder(True) and if you
+    want to turn off type checking you can use @builder(False) or @builder(typechecking=False)
+
+    An example of how to use it
+
+    >>> @builder
+    >>> class HTTPServerOptions:
+    >>>     ip: str
+    >>>     port: int
+    >>>     username: str
+
+    This would generate the equivalent of
+
+    >>> class HTTPServerOptions:
+    >>>     def __init__(self):
+    >>>         self.ip = None
+    >>>         self.port = None
+    >>>         self.username = None
+    >>>
+    >>>     def setip(self, value):
+    >>>         if not isinstance(value, str):
+    >>>             raise TypeError("Excepted attribute ip of type {} but got type {}".format(str, type(value)))
+    >>>         self.ip = value
+    >>>         return self
+    >>>
+    >>>     def setport(self, value):
+    >>>         if not isinstance(value, int):
+    >>>             raise TypeError("Excepted attribute port of type {} but got type {}".format(int, type(value)))
+    >>>         self.port = value
+    >>>         return self
+    >>>
+    >>>     def setusername(self, value):
+    >>>         if not isinstance(value, str):
+    >>>             raise TypeError("Excepted attribute username of type {} but got type {}".format(str, type(value)))
+    >>>         self.username = value
+    >>>         return self
+    """
+    def builder_interior(cls):
+        attributes = cls.__annotations__
+
+        def cls_init(self):
+            for (attr, typename) in attributes.items():
+                setattr(self, attr, None)
+
+        def setter_maker(attr):
+            def setter(self, value):
+                if typechecking and not isinstance(value, typename):
+                    raise TypeError(
+                        "Excepted attribute {} of type {} but got type {}".format(attr, typename, type(value)))
+                setattr(self, attr, value)
+                return self
+
+            return setter
+
+        for (attr, typename) in attributes.items():
+            setattr(cls, 'set{}'.format(attr), setter_maker(attr))
+
+        setattr(cls, '__init__', cls_init)
+        return cls
+
+    if callable(typechecking):
+        return builder_interior(typechecking)
+    else:
+        return builder_interior
+
+
+@builder
+class TattleOptions:
+    """
+    Determines what happens when a function is decorated with @tattle. See there for more. See also @builder for
+    how to construct a TattleOptions
+
+    Each option can either be None or a Callable.
+
+    The onenter property is called before calling the function and it is passed a *args **kwargs splat equivalent
+    to what will be passed into the function when it is called. This is never used if onexit is None
+
+    The onexit property is called after the function returns and it is passed (result, *args, **kwargs) that is the
+    result of the function call and the same args, kwargs splat that went into the function. This is never used if
+    onexit is None *or* if an exception occurs before the function returns
+
+    The onexception property is only called if an exception is raised. The callable is passed (exception, *args, **kwargs)
+    where exception is the instance of the caught exception and *args, and **kwargs are the splat arguments passed to
+    the function when it was called. This is never used if onexception is None or if the function returns normally
+    without raising an Exception.
+    """
+    onenter: typing.Callable
+    onexit: typing.Callable
+    onexception: typing.Callable
+
+
+def tattle(options: typing.Union[TattleOptions, typing.Callable]):
+    """
+    Function decorator that allows the reporting of events. A function decorated with @tattle
+    can have the entrance, exit, and exceptions of the function reported. The `options` parameter is a TattleOptions
+    instance that can is given callables for `onenter`, `onexit`, and `onexception`. These callables are called
+    with arguments at the appropriate time. These options can also be None and no action on that event will be taken
+    """
+    def interior(fn):
+        def wrapper(*args, **kwargs):
+            if options.onenter is not None:
+                options.onenter(*args, **kwargs)
+            try:
+                result = fn(*args, **kwargs)
+            except Exception as exception:
+                if options.onexception is not None:
+                    options.onexception(exception, *args, **kwargs)
+                else:
+                    raise
+            else:
+                if options.onexit is not None:
+                    options.onexit(result, *args, **kwargs)
+                return result
+        return wrapper
+    return interior
+
+
+
 def timed(fn):
     """
     Wraps a function using time.time() in order to time the execution of the function
 
     Returns the a tuple of original function result and the time elapsed in
     seconds
     """
@@ -449,15 +575,16 @@
     out of the object's __dict__ attribute and includes the class name at the beginning
 
     Note that this decorator will return the original cls value passed into it. You will get the same object out that
     gets put in, though, obviously, it will be mutated.
     """
 
     def __str__(self):
-        items = ['{}={}'.format(k, repr(v)) for (k, v) in self.__dict__.items() if not k.startswith('__') and not k.endswith('__')]
+        items = ['{}={}'.format(k, repr(v)) for (k, v) in self.__dict__.items() if
+                 not k.startswith('__') and not k.endswith('__')]
         items_string = ', '.join(items)
         return '{}[{}]'.format(self.__class__.__name__, items_string)
 
     setattr(cls, '__str__', __str__)
     setattr(cls, '__repr__', __str__)
 
     return cls
@@ -843,15 +970,16 @@
 
 
 T = typing.TypeVar('T')
 R = typing.TypeVar('R')
 
 
 class Descriptor(typing.Protocol):
-    def __get__(this, self: typing.Optional[R], owner: typing.Optional[typing.Any] = None, *args, **kwargs) -> typing.Union[T, typing.Self]:
+    def __get__(this, self: typing.Optional[R], owner: typing.Optional[typing.Any] = None, *args, **kwargs) -> \
+    typing.Union[T, typing.Self]:
         ...
 
 
 def lazy(method: typing.Callable[[typing.Any], T]) -> Descriptor:
     '''
     Similar to the `@property` decorator, lazy allows you to access the value computed by a method
     call as if it were a simple attribute on an instance. The main difference between `@property`
@@ -863,15 +991,16 @@
     In this way, it creates a lazy attribute, storing the code to initialize the attribute
     in a function, and only evaluating the function when accessed. It also elimited the overhead of
     other similar solutions like `@functools.cache` by re-writing the attribute after first access,
     removing the descriptor and obviating the need for an `if arg in cache` check
     '''
 
     class descriptor(Descriptor):
-        def __get__(self, receiver: typing.Optional[R], owner: typing.Optional[typing.Any] = None, *args, **kwargs) -> typing.Union[T, typing.Self]:
+        def __get__(self, receiver: typing.Optional[R], owner: typing.Optional[typing.Any] = None, *args, **kwargs) -> \
+        typing.Union[T, typing.Self]:
             if receiver is None:
                 return self
             value = method(receiver, *args, **kwargs)
             setattr(receiver, method.__name__, value)
             return value
 
     return descriptor()
@@ -883,15 +1012,16 @@
     PRESERVING = 3
 
 
 class NoSuchValue(ValueError):
     pass
 
 
-def precompute(argument_tuples: typing.Iterable[tuple], storage: PrecomputeStorage = PrecomputeStorage.PRESERVING, max: typing.Optional[int] = None):
+def precompute(argument_tuples: typing.Iterable[tuple], storage: PrecomputeStorage = PrecomputeStorage.PRESERVING,
+               max: typing.Optional[int] = None):
     """
     Function decorator used to declaratively state precomputed values for a function
 
     On defintion of a function decorated with precompute, the decorated function will be called once for each item
     in argument_tuples. On each call, that item of argument_tuples is splatted into the function.
 
     The decorator can also storage method as the storage parameter. This indicates how the decorated function
@@ -905,36 +1035,42 @@
     if storage != PrecomputeStorage.PRESERVING and max is not None:
         raise ValueError("storage must be PRESERVING or max must be None")
     if storage == PrecomputeStorage.PRESERVING:
         def wrapper(fn):
             @functools.lru_cache(maxsize=max)
             def decorator(*args):
                 return fn(*args)
+
             for args in argument_tuples:
                 decorator(*args)  # cached by functools
             return decorator
+
         return wrapper
     elif storage == PrecomputeStorage.LIMITED:
         def wrapper(fn):
             cache = {}
             for args in argument_tuples:
                 cache[args] = fn(*args)
 
             def decorator(*args):
                 if args in cache:
                     return cache[args]
                 else:
                     return fn(*args)
+
             return decorator
+
         return wrapper
     else:
         def wrapper(fn):
             cache = {}
             for args in argument_tuples:
                 cache[args] = fn(*args)
 
             def decorator(*args):
                 if args not in cache:
                     raise NoSuchValue('{} was not precomputed for the given function'.format(args))
                 return cache[args]
+
             return decorator
+
         return wrapper
```

### Comparing `tecoradors-elunico-5.1.1/tecoradors_elunico.egg-info/PKG-INFO` & `tecoradors-elunico-5.2.1/tecoradors_elunico.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecoradors-elunico
-Version: 5.1.1
+Version: 5.2.1
 Summary: A small collection of decorators I like to use often
 Home-page: https://github.com/elunico/tecoradors
 Author: Thomas Povinelli
 Author-email: tompov227@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,16 @@
 [Find the pypi package here](https://pypi.org/project/tecoradors-elunico/)
 
 Named based on my name which starts with a T. You can find more information reading the docstrings of the functions
 
 ### Decorators are
   *  accepts
   *  json_serializable
+  *  builder
+  *  tattle
   *  spread
   *  timed
   *  squash
   *  stringable
   *  equatable
   *  hashable
   *  dataclass
@@ -42,7 +44,8 @@
   *  lazy
   *  precompute
 
 ### Support from types
   *  Self
   *  PrecomputeStorage
   *  NoSuchValue
+  *  TattleOptions
```

