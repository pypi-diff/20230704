# Comparing `tmp/decoratory-0.9.1.18.tar.gz` & `tmp/decoratory-0.9.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.9.1.18.tar", last modified: Tue Jun 27 12:14:32 2023, max compression
+gzip compressed data, was "decoratory-0.9.2.5.tar", last modified: Tue Jul  4 07:01:40 2023, max compression
```

## Comparing `decoratory-0.9.1.18.tar` & `decoratory-0.9.2.5.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:14:32.190822 decoratory-0.9.1.18/
--rw-rw-rw-   0        0        0     1252 2023-06-27 11:25:14.000000 decoratory-0.9.1.18/License.txt
--rw-rw-rw-   0        0        0    49014 2023-06-27 12:14:32.190822 decoratory-0.9.1.18/PKG-INFO
--rw-rw-rw-   0        0        0    47411 2023-06-27 12:10:25.000000 decoratory-0.9.1.18/Readme.rst
--rw-rw-rw-   0        0        0     1823 2023-06-27 11:36:48.000000 decoratory-0.9.1.18/ReleaseNotes.txt
--rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.1.18/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 12:14:32.120852 decoratory-0.9.1.18/Sources/
-drwxrwxrwx   0        0        0        0 2023-06-27 12:14:32.159662 decoratory-0.9.1.18/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.9.1.18/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     7614 2023-06-27 12:13:55.000000 decoratory-0.9.1.18/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     5880 2023-06-27 11:42:36.000000 decoratory-0.9.1.18/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    14152 2023-06-27 11:42:36.000000 decoratory-0.9.1.18/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    12414 2023-06-27 11:42:36.000000 decoratory-0.9.1.18/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    36902 2023-06-27 11:42:36.000000 decoratory-0.9.1.18/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     7995 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0    10855 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-27 12:14:32.172235 decoratory-0.9.1.18/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    49014 2023-06-27 12:14:32.000000 decoratory-0.9.1.18/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-06-27 12:14:32.000000 decoratory-0.9.1.18/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:14:32.000000 decoratory-0.9.1.18/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-27 12:14:32.000000 decoratory-0.9.1.18/Sources/decoratory.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 12:14:32.188622 decoratory-0.9.1.18/Unittest/
--rw-rw-rw-   0        0        0    24037 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Unittest/test_basic.py
--rw-rw-rw-   0        0        0    23858 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Unittest/test_multiton.py
--rw-rw-rw-   0        0        0    40107 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Unittest/test_observer.py
--rw-rw-rw-   0        0        0    10729 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Unittest/test_singleton.py
--rw-rw-rw-   0        0        0    10193 2023-06-27 11:42:37.000000 decoratory-0.9.1.18/Unittest/test_wrapper.py
--rw-rw-rw-   0        0        0       42 2023-06-27 12:14:32.190822 decoratory-0.9.1.18/setup.cfg
--rw-rw-rw-   0        0        0     4537 2023-06-27 12:13:55.000000 decoratory-0.9.1.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:01:40.100032 decoratory-0.9.2.5/
+-rw-rw-rw-   0        0        0     1252 2023-06-27 11:25:14.000000 decoratory-0.9.2.5/License.txt
+-rw-rw-rw-   0        0        0    47333 2023-07-04 07:01:40.100032 decoratory-0.9.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    45661 2023-07-04 07:01:04.000000 decoratory-0.9.2.5/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.2.5/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 07:01:39.467330 decoratory-0.9.2.5/Sources/
+drwxrwxrwx   0        0        0        0 2023-07-04 07:01:39.781650 decoratory-0.9.2.5/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-07-04 05:40:20.000000 decoratory-0.9.2.5/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     7612 2023-07-04 07:01:04.000000 decoratory-0.9.2.5/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     5878 2023-07-04 07:01:04.000000 decoratory-0.9.2.5/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    14151 2023-07-04 07:01:04.000000 decoratory-0.9.2.5/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    12415 2023-07-04 07:01:04.000000 decoratory-0.9.2.5/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    36905 2023-07-04 07:01:04.000000 decoratory-0.9.2.5/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     7996 2023-07-04 07:01:04.000000 decoratory-0.9.2.5/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    10856 2023-07-04 07:01:04.000000 decoratory-0.9.2.5/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-04 07:01:39.850297 decoratory-0.9.2.5/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    47333 2023-07-04 07:01:39.000000 decoratory-0.9.2.5/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-07-04 07:01:39.000000 decoratory-0.9.2.5/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 07:01:39.000000 decoratory-0.9.2.5/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-04 07:01:39.000000 decoratory-0.9.2.5/Sources/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 07:01:40.051655 decoratory-0.9.2.5/Unittest/
+-rw-rw-rw-   0        0        0    24036 2023-07-04 07:01:04.000000 decoratory-0.9.2.5/Unittest/test_basic.py
+-rw-rw-rw-   0        0        0    23857 2023-07-04 07:01:05.000000 decoratory-0.9.2.5/Unittest/test_multiton.py
+-rw-rw-rw-   0        0        0    40106 2023-07-04 07:01:05.000000 decoratory-0.9.2.5/Unittest/test_observer.py
+-rw-rw-rw-   0        0        0    10728 2023-07-04 07:01:05.000000 decoratory-0.9.2.5/Unittest/test_singleton.py
+-rw-rw-rw-   0        0        0    10192 2023-07-04 07:01:05.000000 decoratory-0.9.2.5/Unittest/test_wrapper.py
+-rw-rw-rw-   0        0        0       42 2023-07-04 07:01:40.100032 decoratory-0.9.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     4597 2023-07-04 07:01:05.000000 decoratory-0.9.2.5/setup.py
```

### Comparing `decoratory-0.9.1.18/License.txt` & `decoratory-0.9.2.5/License.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.9.1.18/PKG-INFO` & `decoratory-0.9.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.1.18
+Version: 0.9.2.5
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
-Download-URL: http://evation.eu
+Download-URL: http://evation.eu\section\download.html
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
 License: MIT
 Project-URL: Projekt, http://evation.eu
-Project-URL: Release Notes, http://evation.eu
-Project-URL: Download, http://evation.eu
+Project-URL: Release Notes, http://evation.eu\section\download.html
+Project-URL: Download, http://evation.eu\section\releasenotes.html
 Keywords: decorator singleton multiton observer observable wrapper
 Platform: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
@@ -47,19 +47,19 @@
     __module__ = "Readme.rst"
     __author__ = "Martin Abel"
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu"
-    __copyright__ = f"(c) copyright 2020-2023, {__company__}"
+    __copyright__ = f"(c) copyright 2020-2023, {__author__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.1.13"
-    __date__ = "2023-06-27"
-    __time__ = "14:10:25"
+    __version__ = "0.9.2.3"
+    __date__ = "2023-07-04"
+    __time__ = "09:01:04"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
@@ -107,16 +107,16 @@
 
 
 **Description**
 
 To illustrate the functionality of each module, simple as well as
 more complex examples are presented. Even if only one particular module
 is needed, it is recommended to view the preceding examples as well. For even
-more examples of the full range of possibilities, please refer to the
-`project homepage`_.
+more examples of the full range of possibilities, please refer to
+`Decorator Implementations`_ on the `project homepage`_.
 
 
 ******************************************************************************
 Singleton
 ******************************************************************************
 
 A `singleton pattern`_ is a design pattern that limits the instantiation of
@@ -162,15 +162,15 @@
     print(f"a == b: {a == b}")      # a == b: True
 
 .. _dynamic-decoration:
 
 If instead of the above *static decoration* using pie-notation, i.e. with
 @-notation at the class declaration, the *dynamic decoration* within Python
 code is used, additional parameters can be passed to the decorator for
-passing to or through the class constructor.
+passing to or through the class initializer.
 
 .. code-block:: python
 
     # *** example_singleton.py - dynamic decoration with extra parameters
 
     # Case 2: Dynamic decoration providing extra initial default values
     Animal = Singleton(Animal, 'Teddy')
@@ -180,15 +180,15 @@
 
 Quite generally, for all the following decorators based on this
 `Decorator Arguments Template`_, these two properties are always fulfilled:
 
 #. Decoration as a class (without parentheses) and Decoration as an instance
    (with empty parentheses) are equivalent
 #. For dynamic decoration, extra parameters can be passed, e.g. for the
-   class constructor
+   class initializer
 
 So far, this singleton implementation follows the concept of *once
 forever*, i.e. whenever a new instance of a class is created, one always
 gets the *primary instance* back - without any possibility of ever changing
 it again.
 
 Although this behavior is consistent with the fundamental concept of a
@@ -214,15 +214,15 @@
     print(Animal(name='Roxie'))     # Animal('Teddy')   (=primary instance)
     Animal.reset()                  # Reset the singleton
     print(Animal(name='Roxie'))     # Animal('Roxie')
     print(Animal(name='Teddy'))     # Animal('Roxie')   (=primary instance)
 
 Without this striking ``resettable=True`` decoration ``Animal`` has no
 ``reset`` method and the call ``Animal.reset()`` will fail raising an
-``AttributeError``. For situations where this concept really needs
+``AttributeError``. For situations where this concept needs
 to be used more often, a subclass shortcut ``SemiSingleton`` is provided.
 
 .. code-block:: python
 
     # *** example_singleton.py - decoration as a 'semi singleton'
 
     from decoratory.singleton import SemiSingleton
@@ -259,15 +259,15 @@
 one key value the multiton simply collapses to a singleton, therefore the
 decoration ``@Multiton`` resp. ``@Multiton()`` or even ``@Multiton(key=17)``
 or  ``@Multiton(key='some constant value')`` and so on always creates a
 singleton.
 
 Normally, the key is part of or is composed from the initial values of the
 classified object, as in the following example, where the key function matches
-the signature of the constructor and uses the initial value of the ``name``
+the signature of the initializer and uses the initial value of the ``name``
 parameter to construct a key value for the instances of ``Animal``.
 
 .. code-block:: python
 
     # *** example_multitonton.py - class Animal with Multiton decoration
 
     from decoratory.multiton import Multiton
@@ -311,15 +311,15 @@
     # *** example_multitonton.py - One unique instance per equivalence class
 
     # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
     print(a)                        # Animal('dog', 'Teddy')
     print(b)                        # Animal('cat', 'Molly')
     print(c)                        # Animal('cat', 'Molly')
 
-The initial parameter values of the constructor can also be accessed by their
+The initial parameter values of the initializer can also be accessed by their
 ``args``-index or ``kwargs``-name. So the following decorations are also
 possible:
 
 .. code-block:: python
 
     # *** example_multitonton.py - Alternative decoration examples
 
@@ -359,27 +359,27 @@
 code that instances are often retrieved but rarely modified, setting the
 decorator parameter ``resettable=True`` will expose the ``reset()`` method,
 by means of which the internal directory of instances can be completely cleared.
 
 Last but not least, ``Multiton`` provides a ``instances`` property and
 associated getter and setter methods to directly retrieve the internal
 dictionary of primary instances. It is obvious that manipulations on this
-directory can corrupt the functionality of the multiton, so this is a method
-for experts, but sometimes they want and/or need to have exactly this freedom.
+directory can corrupt the functionality of the multiton, but sometimes it
+is useful to have the freedom of access.
 
     **Hint** --- Changes affecting key values of classified objects
 
     *Classifications into the multiton directory are done only once on
     initial key data. Subsequent changes affecting a key value are not
     reflected in the multiton directory key, i.e. the directory may then be
     corrupted by such modifications.*
 
     *Therefore,* **never change key related values of classified objects!**
 
-This results in the following exemplary picture:
+All these things taken together could give the following exemplary picture:
 
 .. code-block:: python
 
     # *** example_multitonton.py - seal, unseal, reset, get_instance
 
     # Case 7: with decoration @Multiton(key=lambda spec, name: name,
     #                                   resettable=True)
@@ -479,19 +479,19 @@
 Accordingly, the keyword parameter ``after=F(print_message, message="LEAVE")``
 would also be possible.
 
 The idea behind the ``replace`` option is not so much to replace the complete
 original functionality, because you could simply create your own functionality
 for that but to wrap the original functionality, e.g. according to the principle:
 
-#. Edit the call parameters for the original functionality
+#. Edit and/or prepare the call parameters for the original functionality
 #. Execute the original functionality with these modified call parameters
-#. Edit the result and return this modified result
+#. Edit and/or revise the result and return this modified result
 
-This could then look like this:
+All this together could then look like this:
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose and replacing original function
 
     # Case 3: Decoration with replace functionality
     def replace_wrapper(value: str="replace"):
@@ -507,19 +507,19 @@
         print(f"value = '{value}'")
         return value
 
     result = some_function()        # value = 'REPLACE'
     print(result)                   # result: 'REPLACE'
 
 The first output ``value = 'REPLACE'`` comes from the original function
-``some_function()`` but using parameters modified by the
-``replace_wrapper()``. The second line ``result: 'REPLACE'`` is the result
-of the ``return`` modified by the ``replace_wrapper()``. Please note the line
-marked with ``(1)`` in the ``replace_wrapper()``: It is very important
-to avoid self-recursions:
+``some_function()`` but using parameters  modified to uppercase letters
+by the``replace_wrapper()``. The second line ``result: 'REPLACE'`` is the
+result of the ``return`` modified by the ``replace_wrapper()``. Please note
+the line marked with ``(1)`` in the ``replace_wrapper()``: It is very
+important to avoid self-recursions:
 
     **Hint** --- Avoidance of self-recursion in the replace wrapper
 
     *In the replace wrapper, the undecorated version of the original
     functionality must always be called. It is accessible via the*
     ``substitute.callee`` *method of the wrapper!*
 
@@ -557,15 +557,15 @@
                                     # 9             (output default_printer)
 
 The absence of the outputs of ``UNDEFINED`` and ``UNKNOWN`` reflects the
 correct replacements by the decoration, and the order of execution is exactly
 as expected: ``before`` then ``replace`` then ``after`` and in each of these
 variables the lists are processed in ascending order.
 
-The *decoration of a class* always refers to the constructor of the class, e.g.
+The *decoration of a class* always refers to the initializer of the class, e.g.
 
 .. code-block:: python
 
     # *** example_wrapper.py - class decoration
 
     @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
     class Animal:
@@ -775,18 +775,19 @@
 
     # Case 1: Observer decoration
     #    ---> Person as an observer to observable dog
     person()                        # person says 'Hello?'
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
-The use of the semantic ``X`` instead of ``F`` indicates that ``dog`` is the
-observable, but the ``X`` arguments apply for the observer ``person``.
+The use of the *semantic cross-function* ``X`` from ``decoratory.basic``
+instead of ``F`` indicates that ``dog`` is the observable, but the ``X``
+arguments apply for the observer ``person``.
 
-For multiple decorations, the *order of decoration* is also relevant here.
+For multiple decorations, the *order of decoration* is also relevant, again.
 Each observable must be decorated before it is used by an observer.
 
     **2. Rule:** Decorating as *@Observable* before using in an *@Observer*
 
 The situation ``Case 2`` from `Observable Decoration`_ with person,
 dog and cat would then look like:
 
@@ -864,15 +865,15 @@
 ----------------
 
 Both techniques, `Observable Decoration`_ and `Observer Decoration`_,
 are static, in the sense, decorations are done e.g. in @-notation evaluated
 at compile time. They are applied to *static functions*.
 
 *Decoration of a class* by default addresses decoration of the
-*class constructor*, this means
+*class initializer*, this means
 
 .. code-block:: python
 
     @Observable
     class Dog:
         def __init__(self):
             pass                    # Some code ...
@@ -906,15 +907,15 @@
     # Case 1: Dog is an observable to Person
     prs = Person()                  # Jane Doe arrived.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe arrived.
 
 The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
-    **Hint** --- Take care when decorating a class constructor
+    **Hint** --- Take care when decorating a class initializer
 
     *Notifying the* ``__init__`` *method of an observer results in a new
     instance! This means calling the observable induces instantiation of
     a new observer object, surely in not any case this is the desired
     behavior ...*
 
 So the decoration should not address a class but one (or more) target
@@ -1075,15 +1076,15 @@
     # *** example_observer.py - instance decoration
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
             print(f"Note.info: val = {thing.a}")
 
     class Thing:                            # Observable without decoration!
-        def __init__(self, a=0):            # Constructor, defining variabe 'a'
+        def __init__(self, a=0):            # Initializer, defining variabe 'a'
             self._a = a
         def inc(self):                      # Instance method, modifying 'a'
             self._a += 1
         def get_a(self):                    # Getter, setter, property,
             return self._a                  # modifying variable 'a'
         def set_a(self, value):
             self._a = value
@@ -1144,75 +1145,18 @@
 (2) decorates the relevant instance methods (2), and then
 (3) registers the observers with the associated observables (3).
 
 This method of instance decoration is certainly the most flexible.
 However, it bears the risk of losing track of all dependencies.
 
 
-******************************************************************************
-Version History
-******************************************************************************
-
-**Version: 0.9.1.*, Build: 2023-06-27**
-
-- Switch from PSF License to MIT License
-
-**Version: 0.9.0.*, Build: 2023-06-23**
-
-- Unit test integration for Windows, Linux (and probably MacOS - feedback?)
-- Pre production state, version 0.9.* for module
-    - observer [ ``python -m decoratory.observer --version`` ]
-- Pre production state, version 0.9.* for package
-    - decoratory [ ``python -m decoratory --version`` ]
-
-**Version: 0.1.5.*, Build: 2023-06-21**
-
-- Pre production state, version 0.9.* for module
-    - wrapper [ ``python -m decoratory.wrapper --version`` ]
-
-**Version: 0.1.4.*, Build: 2023-06-21**
-
-- A new subclass SemiSingleton for a resettable singleton
-- Accessible parameter for singleton and multiton removed
-- Additional test and documentation
-- Pre production state, version 0.9.* for modules
-    - singleton [ ``python -m decoratory.singleton --version`` ]
-    - multiton  [ ``python -m decoratory.multiton  --version`` ]
-
-**Version: 0.1.3.*, Build: 2023-06-19**
-
-- Extensions and improvements for module observer: test and documentation
-
-**Version: 0.1.2.*, Build: 2023-06-18**
-
-- Intergration of unit tests for modules singleton, multiton and wrapper
-- An overall unit test for the package decoratory
-- Documentation enhancements for module observer, t.b.c.
-
-**Version: 0.1.1.*, Build: 2023-06-16**
-
-- Initial version of the observer, incl. documentation
-
-**Version: 0.1.0.3, Build: 2023-06-15**
-
-- Accessible parameter for singleton and multiton, incl. documentation
-- Resettable parameter for singleton and multiton, incl. documentation
-
-**Version: 0.1.0.2, Build: 2023-06-13**
-
-- Documentation enhancements for for singleton, multiton and wrapper
-
-**Version: 0.1.0.1, Build: 2023-06-12**
-
-- Initial version with singleton, multiton and wrapper
-
-
 ~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
 
 
 .. ===========================================================================
-.. _project homepage: http://evation.eu
+.. _project homepage: http://evation.eu/decoratory
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
-.. _Decorator Arguments Template: http://evation.eu
+.. _Decorator Arguments Template: http://evation.eu/decoratory/Section/ArgumentsTemplate.html
+.. _Decorator Implementations: http://evation.eu/decoratory/Section/Decorators.html
```

### Comparing `decoratory-0.9.1.18/Readme.rst` & `decoratory-0.9.2.5/Readme.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     __module__ = "Readme.rst"
     __author__ = "Martin Abel"
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu"
-    __copyright__ = f"(c) copyright 2020-2023, {__company__}"
+    __copyright__ = f"(c) copyright 2020-2023, {__author__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.1.13"
-    __date__ = "2023-06-27"
-    __time__ = "14:10:25"
+    __version__ = "0.9.2.3"
+    __date__ = "2023-07-04"
+    __time__ = "09:01:04"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
@@ -68,16 +68,16 @@
 
 
 **Description**
 
 To illustrate the functionality of each module, simple as well as
 more complex examples are presented. Even if only one particular module
 is needed, it is recommended to view the preceding examples as well. For even
-more examples of the full range of possibilities, please refer to the
-`project homepage`_.
+more examples of the full range of possibilities, please refer to
+`Decorator Implementations`_ on the `project homepage`_.
 
 
 ******************************************************************************
 Singleton
 ******************************************************************************
 
 A `singleton pattern`_ is a design pattern that limits the instantiation of
@@ -123,15 +123,15 @@
     print(f"a == b: {a == b}")      # a == b: True
 
 .. _dynamic-decoration:
 
 If instead of the above *static decoration* using pie-notation, i.e. with
 @-notation at the class declaration, the *dynamic decoration* within Python
 code is used, additional parameters can be passed to the decorator for
-passing to or through the class constructor.
+passing to or through the class initializer.
 
 .. code-block:: python
 
     # *** example_singleton.py - dynamic decoration with extra parameters
 
     # Case 2: Dynamic decoration providing extra initial default values
     Animal = Singleton(Animal, 'Teddy')
@@ -141,15 +141,15 @@
 
 Quite generally, for all the following decorators based on this
 `Decorator Arguments Template`_, these two properties are always fulfilled:
 
 #. Decoration as a class (without parentheses) and Decoration as an instance
    (with empty parentheses) are equivalent
 #. For dynamic decoration, extra parameters can be passed, e.g. for the
-   class constructor
+   class initializer
 
 So far, this singleton implementation follows the concept of *once
 forever*, i.e. whenever a new instance of a class is created, one always
 gets the *primary instance* back - without any possibility of ever changing
 it again.
 
 Although this behavior is consistent with the fundamental concept of a
@@ -175,15 +175,15 @@
     print(Animal(name='Roxie'))     # Animal('Teddy')   (=primary instance)
     Animal.reset()                  # Reset the singleton
     print(Animal(name='Roxie'))     # Animal('Roxie')
     print(Animal(name='Teddy'))     # Animal('Roxie')   (=primary instance)
 
 Without this striking ``resettable=True`` decoration ``Animal`` has no
 ``reset`` method and the call ``Animal.reset()`` will fail raising an
-``AttributeError``. For situations where this concept really needs
+``AttributeError``. For situations where this concept needs
 to be used more often, a subclass shortcut ``SemiSingleton`` is provided.
 
 .. code-block:: python
 
     # *** example_singleton.py - decoration as a 'semi singleton'
 
     from decoratory.singleton import SemiSingleton
@@ -220,15 +220,15 @@
 one key value the multiton simply collapses to a singleton, therefore the
 decoration ``@Multiton`` resp. ``@Multiton()`` or even ``@Multiton(key=17)``
 or  ``@Multiton(key='some constant value')`` and so on always creates a
 singleton.
 
 Normally, the key is part of or is composed from the initial values of the
 classified object, as in the following example, where the key function matches
-the signature of the constructor and uses the initial value of the ``name``
+the signature of the initializer and uses the initial value of the ``name``
 parameter to construct a key value for the instances of ``Animal``.
 
 .. code-block:: python
 
     # *** example_multitonton.py - class Animal with Multiton decoration
 
     from decoratory.multiton import Multiton
@@ -272,15 +272,15 @@
     # *** example_multitonton.py - One unique instance per equivalence class
 
     # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
     print(a)                        # Animal('dog', 'Teddy')
     print(b)                        # Animal('cat', 'Molly')
     print(c)                        # Animal('cat', 'Molly')
 
-The initial parameter values of the constructor can also be accessed by their
+The initial parameter values of the initializer can also be accessed by their
 ``args``-index or ``kwargs``-name. So the following decorations are also
 possible:
 
 .. code-block:: python
 
     # *** example_multitonton.py - Alternative decoration examples
 
@@ -320,27 +320,27 @@
 code that instances are often retrieved but rarely modified, setting the
 decorator parameter ``resettable=True`` will expose the ``reset()`` method,
 by means of which the internal directory of instances can be completely cleared.
 
 Last but not least, ``Multiton`` provides a ``instances`` property and
 associated getter and setter methods to directly retrieve the internal
 dictionary of primary instances. It is obvious that manipulations on this
-directory can corrupt the functionality of the multiton, so this is a method
-for experts, but sometimes they want and/or need to have exactly this freedom.
+directory can corrupt the functionality of the multiton, but sometimes it
+is useful to have the freedom of access.
 
     **Hint** --- Changes affecting key values of classified objects
 
     *Classifications into the multiton directory are done only once on
     initial key data. Subsequent changes affecting a key value are not
     reflected in the multiton directory key, i.e. the directory may then be
     corrupted by such modifications.*
 
     *Therefore,* **never change key related values of classified objects!**
 
-This results in the following exemplary picture:
+All these things taken together could give the following exemplary picture:
 
 .. code-block:: python
 
     # *** example_multitonton.py - seal, unseal, reset, get_instance
 
     # Case 7: with decoration @Multiton(key=lambda spec, name: name,
     #                                   resettable=True)
@@ -440,19 +440,19 @@
 Accordingly, the keyword parameter ``after=F(print_message, message="LEAVE")``
 would also be possible.
 
 The idea behind the ``replace`` option is not so much to replace the complete
 original functionality, because you could simply create your own functionality
 for that but to wrap the original functionality, e.g. according to the principle:
 
-#. Edit the call parameters for the original functionality
+#. Edit and/or prepare the call parameters for the original functionality
 #. Execute the original functionality with these modified call parameters
-#. Edit the result and return this modified result
+#. Edit and/or revise the result and return this modified result
 
-This could then look like this:
+All this together could then look like this:
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose and replacing original function
 
     # Case 3: Decoration with replace functionality
     def replace_wrapper(value: str="replace"):
@@ -468,19 +468,19 @@
         print(f"value = '{value}'")
         return value
 
     result = some_function()        # value = 'REPLACE'
     print(result)                   # result: 'REPLACE'
 
 The first output ``value = 'REPLACE'`` comes from the original function
-``some_function()`` but using parameters modified by the
-``replace_wrapper()``. The second line ``result: 'REPLACE'`` is the result
-of the ``return`` modified by the ``replace_wrapper()``. Please note the line
-marked with ``(1)`` in the ``replace_wrapper()``: It is very important
-to avoid self-recursions:
+``some_function()`` but using parameters  modified to uppercase letters
+by the``replace_wrapper()``. The second line ``result: 'REPLACE'`` is the
+result of the ``return`` modified by the ``replace_wrapper()``. Please note
+the line marked with ``(1)`` in the ``replace_wrapper()``: It is very
+important to avoid self-recursions:
 
     **Hint** --- Avoidance of self-recursion in the replace wrapper
 
     *In the replace wrapper, the undecorated version of the original
     functionality must always be called. It is accessible via the*
     ``substitute.callee`` *method of the wrapper!*
 
@@ -518,15 +518,15 @@
                                     # 9             (output default_printer)
 
 The absence of the outputs of ``UNDEFINED`` and ``UNKNOWN`` reflects the
 correct replacements by the decoration, and the order of execution is exactly
 as expected: ``before`` then ``replace`` then ``after`` and in each of these
 variables the lists are processed in ascending order.
 
-The *decoration of a class* always refers to the constructor of the class, e.g.
+The *decoration of a class* always refers to the initializer of the class, e.g.
 
 .. code-block:: python
 
     # *** example_wrapper.py - class decoration
 
     @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
     class Animal:
@@ -736,18 +736,19 @@
 
     # Case 1: Observer decoration
     #    ---> Person as an observer to observable dog
     person()                        # person says 'Hello?'
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
-The use of the semantic ``X`` instead of ``F`` indicates that ``dog`` is the
-observable, but the ``X`` arguments apply for the observer ``person``.
+The use of the *semantic cross-function* ``X`` from ``decoratory.basic``
+instead of ``F`` indicates that ``dog`` is the observable, but the ``X``
+arguments apply for the observer ``person``.
 
-For multiple decorations, the *order of decoration* is also relevant here.
+For multiple decorations, the *order of decoration* is also relevant, again.
 Each observable must be decorated before it is used by an observer.
 
     **2. Rule:** Decorating as *@Observable* before using in an *@Observer*
 
 The situation ``Case 2`` from `Observable Decoration`_ with person,
 dog and cat would then look like:
 
@@ -825,15 +826,15 @@
 ----------------
 
 Both techniques, `Observable Decoration`_ and `Observer Decoration`_,
 are static, in the sense, decorations are done e.g. in @-notation evaluated
 at compile time. They are applied to *static functions*.
 
 *Decoration of a class* by default addresses decoration of the
-*class constructor*, this means
+*class initializer*, this means
 
 .. code-block:: python
 
     @Observable
     class Dog:
         def __init__(self):
             pass                    # Some code ...
@@ -867,15 +868,15 @@
     # Case 1: Dog is an observable to Person
     prs = Person()                  # Jane Doe arrived.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe arrived.
 
 The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
-    **Hint** --- Take care when decorating a class constructor
+    **Hint** --- Take care when decorating a class initializer
 
     *Notifying the* ``__init__`` *method of an observer results in a new
     instance! This means calling the observable induces instantiation of
     a new observer object, surely in not any case this is the desired
     behavior ...*
 
 So the decoration should not address a class but one (or more) target
@@ -1036,15 +1037,15 @@
     # *** example_observer.py - instance decoration
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
             print(f"Note.info: val = {thing.a}")
 
     class Thing:                            # Observable without decoration!
-        def __init__(self, a=0):            # Constructor, defining variabe 'a'
+        def __init__(self, a=0):            # Initializer, defining variabe 'a'
             self._a = a
         def inc(self):                      # Instance method, modifying 'a'
             self._a += 1
         def get_a(self):                    # Getter, setter, property,
             return self._a                  # modifying variable 'a'
         def set_a(self, value):
             self._a = value
@@ -1105,75 +1106,18 @@
 (2) decorates the relevant instance methods (2), and then
 (3) registers the observers with the associated observables (3).
 
 This method of instance decoration is certainly the most flexible.
 However, it bears the risk of losing track of all dependencies.
 
 
-******************************************************************************
-Version History
-******************************************************************************
-
-**Version: 0.9.1.*, Build: 2023-06-27**
-
-- Switch from PSF License to MIT License
-
-**Version: 0.9.0.*, Build: 2023-06-23**
-
-- Unit test integration for Windows, Linux (and probably MacOS - feedback?)
-- Pre production state, version 0.9.* for module
-    - observer [ ``python -m decoratory.observer --version`` ]
-- Pre production state, version 0.9.* for package
-    - decoratory [ ``python -m decoratory --version`` ]
-
-**Version: 0.1.5.*, Build: 2023-06-21**
-
-- Pre production state, version 0.9.* for module
-    - wrapper [ ``python -m decoratory.wrapper --version`` ]
-
-**Version: 0.1.4.*, Build: 2023-06-21**
-
-- A new subclass SemiSingleton for a resettable singleton
-- Accessible parameter for singleton and multiton removed
-- Additional test and documentation
-- Pre production state, version 0.9.* for modules
-    - singleton [ ``python -m decoratory.singleton --version`` ]
-    - multiton  [ ``python -m decoratory.multiton  --version`` ]
-
-**Version: 0.1.3.*, Build: 2023-06-19**
-
-- Extensions and improvements for module observer: test and documentation
-
-**Version: 0.1.2.*, Build: 2023-06-18**
-
-- Intergration of unit tests for modules singleton, multiton and wrapper
-- An overall unit test for the package decoratory
-- Documentation enhancements for module observer, t.b.c.
-
-**Version: 0.1.1.*, Build: 2023-06-16**
-
-- Initial version of the observer, incl. documentation
-
-**Version: 0.1.0.3, Build: 2023-06-15**
-
-- Accessible parameter for singleton and multiton, incl. documentation
-- Resettable parameter for singleton and multiton, incl. documentation
-
-**Version: 0.1.0.2, Build: 2023-06-13**
-
-- Documentation enhancements for for singleton, multiton and wrapper
-
-**Version: 0.1.0.1, Build: 2023-06-12**
-
-- Initial version with singleton, multiton and wrapper
-
-
 ~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
 
 
 .. ===========================================================================
-.. _project homepage: http://evation.eu
+.. _project homepage: http://evation.eu/decoratory
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
-.. _Decorator Arguments Template: http://evation.eu
+.. _Decorator Arguments Template: http://evation.eu/decoratory/Section/ArgumentsTemplate.html
+.. _Decorator Implementations: http://evation.eu/decoratory/Section/Decorators.html
```

### Comparing `decoratory-0.9.1.18/Sources/decoratory/__main__.py` & `decoratory-0.9.2.5/Sources/decoratory/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 __module__ = "__main__.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.18"
-__date__ = "2023-06-27"
-__time__ = "14:13:55"
+__version__ = "0.9.2.5"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["get_file_location"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.1.18/Sources/decoratory/banner.py` & `decoratory-0.9.2.5/Sources/decoratory/banner.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 __module__ = "banner.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.15"
-__date__ = "2023-06-27"
-__time__ = "13:42:36"
+__version__ = "0.9.2.2"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["__banner"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.1.18/Sources/decoratory/basic.py` & `decoratory-0.9.2.5/Sources/decoratory/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 __module__ = "basic.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.6"
-__date__ = "2023-06-27"
-__time__ = "13:42:36"
+__version__ = "0.9.2.2"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Activation", "Parser", "F", "X"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.1.18/Sources/decoratory/multiton.py` & `decoratory-0.9.2.5/Sources/decoratory/multiton.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,19 +123,19 @@
 __module__ = "multiton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.5"
-__date__ = "2023-06-27"
-__time__ = "13:42:36"
+__version__ = "0.9.2.2"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Multiton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -228,15 +228,15 @@
         """Apply the decorator"""
         # --- Decorator Arguments Template (2/2)
         if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
             return self
-        else:  # *** Wrapper ***
+        else:  # *** Decorator ***
             # If no current values, take defaults
             if args or kwargs:
                 subst = F(self.__get__substitute().callee, *args, **kwargs)
             else:
                 subst = self.__get__substitute()
 
             # Calculate key from callable or read key from arguments
```

### Comparing `decoratory-0.9.1.18/Sources/decoratory/observer.py` & `decoratory-0.9.2.5/Sources/decoratory/observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,19 +405,19 @@
 __module__ = "observer.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.5"
-__date__ = "2023-06-27"
-__time__ = "13:42:36"
+__version__ = "0.9.2.2"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Observer", "BaseObserver", "Observable", "BaseObservable"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -677,15 +677,15 @@
                     for observer in self.__get__observers():
                         self.__get__observable().register(observer)
 
                 # Complete wrapper and return observable
                 update_wrapper(self, self.__get__substitute().callee,
                                updated=())
                 return self
-        else:  # *** Wrapper ***
+        else:  # *** Decorator ***
             # Dispatch BEFORE
             if self.__get__activate() & Activation.BEFORE:
                 self.__get__observable().dispatch()
 
             # Delegation: apply the substitute, current before default values
             if args or kwargs:
                 result = F(self.__get__substitute().callee, *args,
@@ -865,15 +865,15 @@
                             raise TypeError(
                                 f"{observable.callee} is not an observable.")
 
                 # Complete wrapper and return observer
                 update_wrapper(self, self.__get__substitute().callee,
                                updated=())
                 return self
-        else:  # *** Wrapper ***
+        else:  # *** Decorator ***
             # Delegation: apply the substitute, current before default values
             if args or kwargs:
                 return F(self.__get__substitute().callee, *args,
                          **kwargs).eval()
             else:
                 return self.__get__substitute().eval()
```

### Comparing `decoratory-0.9.1.18/Sources/decoratory/singleton.py` & `decoratory-0.9.2.5/Sources/decoratory/singleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,19 +82,19 @@
 __module__ = "singleton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.5"
-__date__ = "2023-06-27"
-__time__ = "13:42:36"
+__version__ = "0.9.2.2"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Singleton", "SemiSingleton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -167,15 +167,15 @@
 
         # --- Decorator Arguments Template (2/2)
         if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
             return self
-        else:  # *** Wrapper ***
+        else:  # *** Decorator ***
             # Create and store new or return existing instance
             if self.__instance is None:
                 if args or kwargs:
                     self.__instance = F(self.__get__substitute().callee,
                                         *args, **kwargs).eval()
                 else:
                     self.__instance = self.__get__substitute().eval()
```

### Comparing `decoratory-0.9.1.18/Sources/decoratory/wrapper.py` & `decoratory-0.9.2.5/Sources/decoratory/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,19 +134,19 @@
 __module__ = "wrapper.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.5"
-__date__ = "2023-06-27"
-__time__ = "13:42:36"
+__version__ = "0.9.2.2"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -214,15 +214,15 @@
     def __call__(self, *args, **kwargs):
         # --- Decorator Arguments Template (2/2)
         if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
             return self
-        else:  # *** Wrapper ***
+        else:  # *** Decorator ***
             # Action BEFORE
             if self.__get__before():
                 for before in self.__get__before():
                     before.eval()
 
             # Delegation vs. REPLACE
             result = None
```

### Comparing `decoratory-0.9.1.18/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.9.2.5/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.1.18
+Version: 0.9.2.5
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
-Download-URL: http://evation.eu
+Download-URL: http://evation.eu\section\download.html
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
 License: MIT
 Project-URL: Projekt, http://evation.eu
-Project-URL: Release Notes, http://evation.eu
-Project-URL: Download, http://evation.eu
+Project-URL: Release Notes, http://evation.eu\section\download.html
+Project-URL: Download, http://evation.eu\section\releasenotes.html
 Keywords: decorator singleton multiton observer observable wrapper
 Platform: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
@@ -47,19 +47,19 @@
     __module__ = "Readme.rst"
     __author__ = "Martin Abel"
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu"
-    __copyright__ = f"(c) copyright 2020-2023, {__company__}"
+    __copyright__ = f"(c) copyright 2020-2023, {__author__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.1.13"
-    __date__ = "2023-06-27"
-    __time__ = "14:10:25"
+    __version__ = "0.9.2.3"
+    __date__ = "2023-07-04"
+    __time__ = "09:01:04"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
@@ -107,16 +107,16 @@
 
 
 **Description**
 
 To illustrate the functionality of each module, simple as well as
 more complex examples are presented. Even if only one particular module
 is needed, it is recommended to view the preceding examples as well. For even
-more examples of the full range of possibilities, please refer to the
-`project homepage`_.
+more examples of the full range of possibilities, please refer to
+`Decorator Implementations`_ on the `project homepage`_.
 
 
 ******************************************************************************
 Singleton
 ******************************************************************************
 
 A `singleton pattern`_ is a design pattern that limits the instantiation of
@@ -162,15 +162,15 @@
     print(f"a == b: {a == b}")      # a == b: True
 
 .. _dynamic-decoration:
 
 If instead of the above *static decoration* using pie-notation, i.e. with
 @-notation at the class declaration, the *dynamic decoration* within Python
 code is used, additional parameters can be passed to the decorator for
-passing to or through the class constructor.
+passing to or through the class initializer.
 
 .. code-block:: python
 
     # *** example_singleton.py - dynamic decoration with extra parameters
 
     # Case 2: Dynamic decoration providing extra initial default values
     Animal = Singleton(Animal, 'Teddy')
@@ -180,15 +180,15 @@
 
 Quite generally, for all the following decorators based on this
 `Decorator Arguments Template`_, these two properties are always fulfilled:
 
 #. Decoration as a class (without parentheses) and Decoration as an instance
    (with empty parentheses) are equivalent
 #. For dynamic decoration, extra parameters can be passed, e.g. for the
-   class constructor
+   class initializer
 
 So far, this singleton implementation follows the concept of *once
 forever*, i.e. whenever a new instance of a class is created, one always
 gets the *primary instance* back - without any possibility of ever changing
 it again.
 
 Although this behavior is consistent with the fundamental concept of a
@@ -214,15 +214,15 @@
     print(Animal(name='Roxie'))     # Animal('Teddy')   (=primary instance)
     Animal.reset()                  # Reset the singleton
     print(Animal(name='Roxie'))     # Animal('Roxie')
     print(Animal(name='Teddy'))     # Animal('Roxie')   (=primary instance)
 
 Without this striking ``resettable=True`` decoration ``Animal`` has no
 ``reset`` method and the call ``Animal.reset()`` will fail raising an
-``AttributeError``. For situations where this concept really needs
+``AttributeError``. For situations where this concept needs
 to be used more often, a subclass shortcut ``SemiSingleton`` is provided.
 
 .. code-block:: python
 
     # *** example_singleton.py - decoration as a 'semi singleton'
 
     from decoratory.singleton import SemiSingleton
@@ -259,15 +259,15 @@
 one key value the multiton simply collapses to a singleton, therefore the
 decoration ``@Multiton`` resp. ``@Multiton()`` or even ``@Multiton(key=17)``
 or  ``@Multiton(key='some constant value')`` and so on always creates a
 singleton.
 
 Normally, the key is part of or is composed from the initial values of the
 classified object, as in the following example, where the key function matches
-the signature of the constructor and uses the initial value of the ``name``
+the signature of the initializer and uses the initial value of the ``name``
 parameter to construct a key value for the instances of ``Animal``.
 
 .. code-block:: python
 
     # *** example_multitonton.py - class Animal with Multiton decoration
 
     from decoratory.multiton import Multiton
@@ -311,15 +311,15 @@
     # *** example_multitonton.py - One unique instance per equivalence class
 
     # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
     print(a)                        # Animal('dog', 'Teddy')
     print(b)                        # Animal('cat', 'Molly')
     print(c)                        # Animal('cat', 'Molly')
 
-The initial parameter values of the constructor can also be accessed by their
+The initial parameter values of the initializer can also be accessed by their
 ``args``-index or ``kwargs``-name. So the following decorations are also
 possible:
 
 .. code-block:: python
 
     # *** example_multitonton.py - Alternative decoration examples
 
@@ -359,27 +359,27 @@
 code that instances are often retrieved but rarely modified, setting the
 decorator parameter ``resettable=True`` will expose the ``reset()`` method,
 by means of which the internal directory of instances can be completely cleared.
 
 Last but not least, ``Multiton`` provides a ``instances`` property and
 associated getter and setter methods to directly retrieve the internal
 dictionary of primary instances. It is obvious that manipulations on this
-directory can corrupt the functionality of the multiton, so this is a method
-for experts, but sometimes they want and/or need to have exactly this freedom.
+directory can corrupt the functionality of the multiton, but sometimes it
+is useful to have the freedom of access.
 
     **Hint** --- Changes affecting key values of classified objects
 
     *Classifications into the multiton directory are done only once on
     initial key data. Subsequent changes affecting a key value are not
     reflected in the multiton directory key, i.e. the directory may then be
     corrupted by such modifications.*
 
     *Therefore,* **never change key related values of classified objects!**
 
-This results in the following exemplary picture:
+All these things taken together could give the following exemplary picture:
 
 .. code-block:: python
 
     # *** example_multitonton.py - seal, unseal, reset, get_instance
 
     # Case 7: with decoration @Multiton(key=lambda spec, name: name,
     #                                   resettable=True)
@@ -479,19 +479,19 @@
 Accordingly, the keyword parameter ``after=F(print_message, message="LEAVE")``
 would also be possible.
 
 The idea behind the ``replace`` option is not so much to replace the complete
 original functionality, because you could simply create your own functionality
 for that but to wrap the original functionality, e.g. according to the principle:
 
-#. Edit the call parameters for the original functionality
+#. Edit and/or prepare the call parameters for the original functionality
 #. Execute the original functionality with these modified call parameters
-#. Edit the result and return this modified result
+#. Edit and/or revise the result and return this modified result
 
-This could then look like this:
+All this together could then look like this:
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose and replacing original function
 
     # Case 3: Decoration with replace functionality
     def replace_wrapper(value: str="replace"):
@@ -507,19 +507,19 @@
         print(f"value = '{value}'")
         return value
 
     result = some_function()        # value = 'REPLACE'
     print(result)                   # result: 'REPLACE'
 
 The first output ``value = 'REPLACE'`` comes from the original function
-``some_function()`` but using parameters modified by the
-``replace_wrapper()``. The second line ``result: 'REPLACE'`` is the result
-of the ``return`` modified by the ``replace_wrapper()``. Please note the line
-marked with ``(1)`` in the ``replace_wrapper()``: It is very important
-to avoid self-recursions:
+``some_function()`` but using parameters  modified to uppercase letters
+by the``replace_wrapper()``. The second line ``result: 'REPLACE'`` is the
+result of the ``return`` modified by the ``replace_wrapper()``. Please note
+the line marked with ``(1)`` in the ``replace_wrapper()``: It is very
+important to avoid self-recursions:
 
     **Hint** --- Avoidance of self-recursion in the replace wrapper
 
     *In the replace wrapper, the undecorated version of the original
     functionality must always be called. It is accessible via the*
     ``substitute.callee`` *method of the wrapper!*
 
@@ -557,15 +557,15 @@
                                     # 9             (output default_printer)
 
 The absence of the outputs of ``UNDEFINED`` and ``UNKNOWN`` reflects the
 correct replacements by the decoration, and the order of execution is exactly
 as expected: ``before`` then ``replace`` then ``after`` and in each of these
 variables the lists are processed in ascending order.
 
-The *decoration of a class* always refers to the constructor of the class, e.g.
+The *decoration of a class* always refers to the initializer of the class, e.g.
 
 .. code-block:: python
 
     # *** example_wrapper.py - class decoration
 
     @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
     class Animal:
@@ -775,18 +775,19 @@
 
     # Case 1: Observer decoration
     #    ---> Person as an observer to observable dog
     person()                        # person says 'Hello?'
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
-The use of the semantic ``X`` instead of ``F`` indicates that ``dog`` is the
-observable, but the ``X`` arguments apply for the observer ``person``.
+The use of the *semantic cross-function* ``X`` from ``decoratory.basic``
+instead of ``F`` indicates that ``dog`` is the observable, but the ``X``
+arguments apply for the observer ``person``.
 
-For multiple decorations, the *order of decoration* is also relevant here.
+For multiple decorations, the *order of decoration* is also relevant, again.
 Each observable must be decorated before it is used by an observer.
 
     **2. Rule:** Decorating as *@Observable* before using in an *@Observer*
 
 The situation ``Case 2`` from `Observable Decoration`_ with person,
 dog and cat would then look like:
 
@@ -864,15 +865,15 @@
 ----------------
 
 Both techniques, `Observable Decoration`_ and `Observer Decoration`_,
 are static, in the sense, decorations are done e.g. in @-notation evaluated
 at compile time. They are applied to *static functions*.
 
 *Decoration of a class* by default addresses decoration of the
-*class constructor*, this means
+*class initializer*, this means
 
 .. code-block:: python
 
     @Observable
     class Dog:
         def __init__(self):
             pass                    # Some code ...
@@ -906,15 +907,15 @@
     # Case 1: Dog is an observable to Person
     prs = Person()                  # Jane Doe arrived.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe arrived.
 
 The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
-    **Hint** --- Take care when decorating a class constructor
+    **Hint** --- Take care when decorating a class initializer
 
     *Notifying the* ``__init__`` *method of an observer results in a new
     instance! This means calling the observable induces instantiation of
     a new observer object, surely in not any case this is the desired
     behavior ...*
 
 So the decoration should not address a class but one (or more) target
@@ -1075,15 +1076,15 @@
     # *** example_observer.py - instance decoration
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
             print(f"Note.info: val = {thing.a}")
 
     class Thing:                            # Observable without decoration!
-        def __init__(self, a=0):            # Constructor, defining variabe 'a'
+        def __init__(self, a=0):            # Initializer, defining variabe 'a'
             self._a = a
         def inc(self):                      # Instance method, modifying 'a'
             self._a += 1
         def get_a(self):                    # Getter, setter, property,
             return self._a                  # modifying variable 'a'
         def set_a(self, value):
             self._a = value
@@ -1144,75 +1145,18 @@
 (2) decorates the relevant instance methods (2), and then
 (3) registers the observers with the associated observables (3).
 
 This method of instance decoration is certainly the most flexible.
 However, it bears the risk of losing track of all dependencies.
 
 
-******************************************************************************
-Version History
-******************************************************************************
-
-**Version: 0.9.1.*, Build: 2023-06-27**
-
-- Switch from PSF License to MIT License
-
-**Version: 0.9.0.*, Build: 2023-06-23**
-
-- Unit test integration for Windows, Linux (and probably MacOS - feedback?)
-- Pre production state, version 0.9.* for module
-    - observer [ ``python -m decoratory.observer --version`` ]
-- Pre production state, version 0.9.* for package
-    - decoratory [ ``python -m decoratory --version`` ]
-
-**Version: 0.1.5.*, Build: 2023-06-21**
-
-- Pre production state, version 0.9.* for module
-    - wrapper [ ``python -m decoratory.wrapper --version`` ]
-
-**Version: 0.1.4.*, Build: 2023-06-21**
-
-- A new subclass SemiSingleton for a resettable singleton
-- Accessible parameter for singleton and multiton removed
-- Additional test and documentation
-- Pre production state, version 0.9.* for modules
-    - singleton [ ``python -m decoratory.singleton --version`` ]
-    - multiton  [ ``python -m decoratory.multiton  --version`` ]
-
-**Version: 0.1.3.*, Build: 2023-06-19**
-
-- Extensions and improvements for module observer: test and documentation
-
-**Version: 0.1.2.*, Build: 2023-06-18**
-
-- Intergration of unit tests for modules singleton, multiton and wrapper
-- An overall unit test for the package decoratory
-- Documentation enhancements for module observer, t.b.c.
-
-**Version: 0.1.1.*, Build: 2023-06-16**
-
-- Initial version of the observer, incl. documentation
-
-**Version: 0.1.0.3, Build: 2023-06-15**
-
-- Accessible parameter for singleton and multiton, incl. documentation
-- Resettable parameter for singleton and multiton, incl. documentation
-
-**Version: 0.1.0.2, Build: 2023-06-13**
-
-- Documentation enhancements for for singleton, multiton and wrapper
-
-**Version: 0.1.0.1, Build: 2023-06-12**
-
-- Initial version with singleton, multiton and wrapper
-
-
 ~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
 
 
 .. ===========================================================================
-.. _project homepage: http://evation.eu
+.. _project homepage: http://evation.eu/decoratory
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
-.. _Decorator Arguments Template: http://evation.eu
+.. _Decorator Arguments Template: http://evation.eu/decoratory/Section/ArgumentsTemplate.html
+.. _Decorator Implementations: http://evation.eu/decoratory/Section/Decorators.html
```

### Comparing `decoratory-0.9.1.18/Sources/decoratory.egg-info/SOURCES.txt` & `decoratory-0.9.2.5/Sources/decoratory.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 License.txt
 Readme.rst
-ReleaseNotes.txt
 Requirements.txt
 setup.py
 Sources/decoratory/__init__.py
 Sources/decoratory/__main__.py
 Sources/decoratory/banner.py
 Sources/decoratory/basic.py
 Sources/decoratory/multiton.py
```

### Comparing `decoratory-0.9.1.18/Unittest/test_basic.py` & `decoratory-0.9.2.5/Unittest/test_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 __module__ = "test_basic.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.3"
-__date__ = "2023-06-27"
-__time__ = "13:42:36"
+__version__ = "0.9.2.2"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.1.18/Unittest/test_multiton.py` & `decoratory-0.9.2.5/Unittest/test_multiton.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 __module__ = "test_multiton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.3"
-__date__ = "2023-06-27"
-__time__ = "13:42:36"
+__version__ = "0.9.2.2"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.1.18/Unittest/test_observer.py` & `decoratory-0.9.2.5/Unittest/test_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 __module__ = "test_observer.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.4"
-__date__ = "2023-06-27"
-__time__ = "13:42:36"
+__version__ = "0.9.2.2"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.1.18/Unittest/test_singleton.py` & `decoratory-0.9.2.5/Unittest/test_singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 __module__ = "test_singleton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.3"
-__date__ = "2023-06-27"
-__time__ = "13:42:36"
+__version__ = "0.9.2.2"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.1.18/Unittest/test_wrapper.py` & `decoratory-0.9.2.5/Unittest/test_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 __module__ = "test_wrapper.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.3"
-__date__ = "2023-06-27"
-__time__ = "13:42:36"
+__version__ = "0.9.2.2"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.1.18/setup.py` & `decoratory-0.9.2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 __module__ = "setup.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
-__copyright__ = f"(c) copyright 2020-2023, {__company__}"
+__copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.1.18"
-__date__ = "2023-06-27"
-__time__ = "14:13:55"
+__version__ = "0.9.2.5"
+__date__ = "2023-07-04"
+__time__ = "09:01:04"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
@@ -61,23 +61,23 @@
     name=__title__,
     version=__version__,
     author=__author__,
     author_email=f'{__author__} <{__email__}>',
     maintainer=f'{__author__}',
     maintainer_email=f'{__author__} <{__email__}>',
     url=__url__,
-    download_url=__url__,
+    download_url=join(__url__, "section", "download.html"),
     description=('Decorators: Singleton, Multiton, Observer, Observable, '
                  'generic Wrapper.'),
     long_description=description,
     long_description_content_type='text/x-rst',
     project_urls={
         'Projekt': __url__,
-        'Release Notes': __url__,
-        'Download': __url__},
+        'Release Notes': join(__url__, "section", "download.html"),
+        'Download': join(__url__, "section", "releasenotes.html")},
     keywords='decorator singleton multiton observer observable wrapper',
     # Technical
     license=__license__,
     platforms=['Operating System :: OS Independent'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
@@ -102,15 +102,14 @@
     # https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#finding-simple-packages
     packages=find_packages(where=src),
     package_dir={"": src},
     package_data={},
     py_modules=[],
     data_files=[(dta, ["License.txt",
                        "Readme.rst",
-                       "ReleaseNotes.txt",
                        "Requirements.txt"]),
                 (tst, ["Unittest/test_basic.py",
                        "Unittest/test_singleton.py",
                        "Unittest/test_multiton.py",
                        "Unittest/test_wrapper.py",
                        "Unittest/test_observer.py"])],
     entry_points={},
```

