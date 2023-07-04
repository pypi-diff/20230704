# Comparing `tmp/igbpyutils-0.0.6.tar.gz` & `tmp/igbpyutils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igbpyutils-0.0.6.tar", last modified: Wed May  3 20:49:21 2023, max compression
+gzip compressed data, was "igbpyutils-0.0.7.tar", last modified: Tue Jul  4 16:52:11 2023, max compression
```

## Comparing `igbpyutils-0.0.6.tar` & `igbpyutils-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 20:49:21.239650 igbpyutils-0.0.6/
--rw-------   0 haukex    (1000) haukex    (1000)    35149 2023-04-14 17:49:50.000000 igbpyutils-0.0.6/LICENSE.txt
--rw-------   0 haukex    (1000) haukex    (1000)     2439 2023-05-03 20:49:21.239650 igbpyutils-0.0.6/PKG-INFO
--rw-------   0 haukex    (1000) haukex    (1000)     1491 2023-05-03 20:27:15.000000 igbpyutils-0.0.6/README.rst
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 20:49:21.239650 igbpyutils-0.0.6/igbpyutils/
--rw-------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:16:14.000000 igbpyutils-0.0.6/igbpyutils/__init__.py
--rw-------   0 haukex    (1000) haukex    (1000)     1537 2023-05-03 20:27:15.000000 igbpyutils-0.0.6/igbpyutils/dt.py
--rw-------   0 haukex    (1000) haukex    (1000)     5737 2023-05-03 20:27:15.000000 igbpyutils-0.0.6/igbpyutils/error.py
--rw-------   0 haukex    (1000) haukex    (1000)     9756 2023-05-03 20:27:15.000000 igbpyutils-0.0.6/igbpyutils/file.py
--rw-------   0 haukex    (1000) haukex    (1000)     5494 2023-05-03 20:27:15.000000 igbpyutils-0.0.6/igbpyutils/iter.py
--rw-------   0 haukex    (1000) haukex    (1000)     1457 2023-05-03 20:27:15.000000 igbpyutils-0.0.6/igbpyutils/test.py
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 20:49:21.239650 igbpyutils-0.0.6/igbpyutils.egg-info/
--rw-------   0 haukex    (1000) haukex    (1000)     2439 2023-05-03 20:49:21.000000 igbpyutils-0.0.6/igbpyutils.egg-info/PKG-INFO
--rw-------   0 haukex    (1000) haukex    (1000)      384 2023-05-03 20:49:21.000000 igbpyutils-0.0.6/igbpyutils.egg-info/SOURCES.txt
--rw-------   0 haukex    (1000) haukex    (1000)        1 2023-05-03 20:49:21.000000 igbpyutils-0.0.6/igbpyutils.egg-info/dependency_links.txt
--rw-------   0 haukex    (1000) haukex    (1000)       11 2023-05-03 20:49:21.000000 igbpyutils-0.0.6/igbpyutils.egg-info/top_level.txt
--rw-------   0 haukex    (1000) haukex    (1000)      970 2023-05-03 20:38:16.000000 igbpyutils-0.0.6/pyproject.toml
--rw-------   0 haukex    (1000) haukex    (1000)       38 2023-05-03 20:49:21.239650 igbpyutils-0.0.6/setup.cfg
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 20:49:21.239650 igbpyutils-0.0.6/tests/
--rwxr-xr-x   0 haukex    (1000) haukex    (1000)     2023 2023-04-16 11:23:30.000000 igbpyutils-0.0.6/tests/test_dt.py
--rwx------   0 haukex    (1000) haukex    (1000)     6923 2023-05-03 16:39:39.000000 igbpyutils-0.0.6/tests/test_error.py
--rwx------   0 haukex    (1000) haukex    (1000)    11434 2023-05-03 16:24:28.000000 igbpyutils-0.0.6/tests/test_file.py
--rwx------   0 haukex    (1000) haukex    (1000)     9018 2023-04-16 11:21:31.000000 igbpyutils-0.0.6/tests/test_iter.py
--rwx------   0 haukex    (1000) haukex    (1000)     1606 2023-04-14 19:26:01.000000 igbpyutils-0.0.6/tests/test_test.py
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-07-04 16:52:11.866783 igbpyutils-0.0.7/
+-rw-------   0 haukex    (1000) haukex    (1000)    35149 2023-04-14 17:49:50.000000 igbpyutils-0.0.7/LICENSE.txt
+-rw-------   0 haukex    (1000) haukex    (1000)     2490 2023-07-04 16:52:11.866783 igbpyutils-0.0.7/PKG-INFO
+-rw-------   0 haukex    (1000) haukex    (1000)     1491 2023-07-04 16:49:37.000000 igbpyutils-0.0.7/README.rst
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-07-04 16:52:11.866783 igbpyutils-0.0.7/igbpyutils/
+-rw-------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:16:14.000000 igbpyutils-0.0.7/igbpyutils/__init__.py
+-rw-------   0 haukex    (1000) haukex    (1000)     1537 2023-05-03 20:27:15.000000 igbpyutils-0.0.7/igbpyutils/dt.py
+-rw-------   0 haukex    (1000) haukex    (1000)     6141 2023-07-04 14:45:24.000000 igbpyutils-0.0.7/igbpyutils/error.py
+-rw-------   0 haukex    (1000) haukex    (1000)    11133 2023-07-04 15:10:41.000000 igbpyutils-0.0.7/igbpyutils/file.py
+-rw-------   0 haukex    (1000) haukex    (1000)     5708 2023-07-04 15:15:04.000000 igbpyutils-0.0.7/igbpyutils/iter.py
+-rw-------   0 haukex    (1000) haukex    (1000)     1457 2023-05-03 20:27:15.000000 igbpyutils-0.0.7/igbpyutils/test.py
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-07-04 16:52:11.866783 igbpyutils-0.0.7/igbpyutils.egg-info/
+-rw-------   0 haukex    (1000) haukex    (1000)     2490 2023-07-04 16:52:11.000000 igbpyutils-0.0.7/igbpyutils.egg-info/PKG-INFO
+-rw-------   0 haukex    (1000) haukex    (1000)      384 2023-07-04 16:52:11.000000 igbpyutils-0.0.7/igbpyutils.egg-info/SOURCES.txt
+-rw-------   0 haukex    (1000) haukex    (1000)        1 2023-07-04 16:52:11.000000 igbpyutils-0.0.7/igbpyutils.egg-info/dependency_links.txt
+-rw-------   0 haukex    (1000) haukex    (1000)       11 2023-07-04 16:52:11.000000 igbpyutils-0.0.7/igbpyutils.egg-info/top_level.txt
+-rw-------   0 haukex    (1000) haukex    (1000)     1016 2023-07-04 16:46:41.000000 igbpyutils-0.0.7/pyproject.toml
+-rw-------   0 haukex    (1000) haukex    (1000)       38 2023-07-04 16:52:11.866783 igbpyutils-0.0.7/setup.cfg
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-07-04 16:52:11.866783 igbpyutils-0.0.7/tests/
+-rwxr-xr-x   0 haukex    (1000) haukex    (1000)     2023 2023-04-16 11:23:30.000000 igbpyutils-0.0.7/tests/test_dt.py
+-rwx------   0 haukex    (1000) haukex    (1000)     7007 2023-06-15 11:35:47.000000 igbpyutils-0.0.7/tests/test_error.py
+-rwx------   0 haukex    (1000) haukex    (1000)    11435 2023-06-15 11:35:47.000000 igbpyutils-0.0.7/tests/test_file.py
+-rwx------   0 haukex    (1000) haukex    (1000)     9610 2023-05-19 07:02:12.000000 igbpyutils-0.0.7/tests/test_iter.py
+-rwx------   0 haukex    (1000) haukex    (1000)     1606 2023-04-14 19:26:01.000000 igbpyutils-0.0.7/tests/test_test.py
```

### Comparing `igbpyutils-0.0.6/LICENSE.txt` & `igbpyutils-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.6/PKG-INFO` & `igbpyutils-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: igbpyutils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Various Python Utilities
 Author-email: Hauke D <haukex@zero-g.net>
 Project-URL: Homepage, https://github.com/haukex/igbpyutils
 Project-URL: Bug Tracker, https://github.com/haukex/igbpyutils/issues
 Project-URL: Documentation, https://igbpyutils.readthedocs.io/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
@@ -27,15 +28,15 @@
 developed at the Leibniz Institute of Freshwater Ecology and Inland Fisheries
 (IGB) in the Forschungsverbund Berlin e.V. (https://www.igb-berlin.de/en).
 
 This is a companion library to the ``igbdatatools`` library
 (https://github.com/haukex/igbdatatools) which normally targets the latest
 Python version.
 This library is intended to contain more general-purpose tools and
-cover a slightly broader range of Python versions, currently Python 3.9 to 3.11.
+cover a slightly broader range of Python versions, currently Python 3.9 to 3.12.
 
 The documentation is available at https://igbpyutils.readthedocs.io/
 
 
 Author, Copyright, and License
 ------------------------------
```

### Comparing `igbpyutils-0.0.6/README.rst` & `igbpyutils-0.0.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 developed at the Leibniz Institute of Freshwater Ecology and Inland Fisheries
 (IGB) in the Forschungsverbund Berlin e.V. (https://www.igb-berlin.de/en).
 
 This is a companion library to the ``igbdatatools`` library
 (https://github.com/haukex/igbdatatools) which normally targets the latest
 Python version.
 This library is intended to contain more general-purpose tools and
-cover a slightly broader range of Python versions, currently Python 3.9 to 3.11.
+cover a slightly broader range of Python versions, currently Python 3.9 to 3.12.
 
 The documentation is available at https://igbpyutils.readthedocs.io/
 
 
 Author, Copyright, and License
 ------------------------------
```

### Comparing `igbpyutils-0.0.6/igbpyutils/dt.py` & `igbpyutils-0.0.7/igbpyutils/dt.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.6/igbpyutils/error.py` & `igbpyutils-0.0.7/igbpyutils/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 #!python3
 """Error Handling and Formatting Utilities
 
+This module primarily provides :func:`~igbpyutils.error.javaishstacktrace` and a custom version of
+:func:`warnings.showwarning`, both of which produce somewhat shorter messages than the default Python messages.
+They can be set up via the context manager :class:`~igbpyutils.error.CustomHandlers` or, more typically, via a
+call to :func:`~igbpyutils.error.init_handlers` at the beginning of the script.
+
 Author, Copyright, and License
 ------------------------------
 Copyright (c) 2022-2023 Hauke Daempfling (haukex@zero-g.net)
 at the Leibniz Institute of Freshwater Ecology and Inland Fisheries (IGB),
 Berlin, Germany, https://www.igb-berlin.de/
 
 This program is free software: you can redistribute it and/or modify
@@ -108,20 +113,20 @@
         ex = ex.__cause__
         causes.append(ex)
     first = True
     for e in reversed(causes):
         r = ex_repr(e)
         if isinstance(e, AssertionError):  # for "assert"s we'd like to see the source that caused it
             assert e.__traceback__  # for some reason, the coverage tool is reporting the following `if` is false on 3.9?
-            if e.__traceback__:  # cover-not-le3.9
+            if e.__traceback__:  # cover-req-ge3.10
                 lines = inspect.getinnerframes(e.__traceback__)[-1].code_context
                 if lines:
                     r += f" [{ lines[0].strip() if len(lines)==1 else ''.join(lines) !r}]"
                 else: pass  # pragma: no cover
-            else: pass  # cover-not-ge3.10
+            else: pass  # cover-req-lt3.10
         yield r if first else "which caused: " + r
         for item in reversed( extract_tb(e.__traceback__) ):
             try:
                 fn = Path(item.filename).resolve(strict=True)
             except OSError:  # pragma: no cover
                 fn = Path(item.filename)
             if fn.is_relative_to(_basepath): fn = fn.relative_to(_basepath)
```

### Comparing `igbpyutils-0.0.6/igbpyutils/file.py` & `igbpyutils-0.0.7/igbpyutils/file.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,24 +20,34 @@
 You should have received a copy of the GNU General Public License
 along with this program. If not, see https://www.gnu.org/licenses/
 """
 import os
 import stat
 import sys
 import uuid
+import typing
+import io
+from gzip import GzipFile
 from pathlib import Path
 from contextlib import contextmanager
 from functools import singledispatch
 from tempfile import NamedTemporaryFile
 from typing import Union
 from collections.abc import Generator, Iterable
 
 Filename = Union[str, os.PathLike]
+"""A type to represent filenames."""
+
+BinaryStream = Union[typing.IO[bytes], io.RawIOBase, io.BufferedIOBase, GzipFile]
+"""A type to represent binary file handles."""
 
 AnyPaths = Union[ Filename, bytes, Iterable[ Union[Filename, bytes] ] ]
+"""A type to represent any path or iterable of paths.
+
+Can be converted to :class:`~pathlib.Path` objects with :func:`to_Paths`."""
 @singledispatch
 def _topath(item :Union[Filename,bytes]):
     raise TypeError(f"I don't know how to covert this to a Path: {item!r}")
 @_topath.register
 def _(item :bytes): return Path(os.fsdecode(item))
 @_topath.register
 def _(item :str): return Path(item)
@@ -60,43 +70,61 @@
 def _(paths :str) -> Generator[Path, None, None]:
     yield _topath(paths)
 @to_Paths.register
 def _(paths :os.PathLike) -> Generator[Path, None, None]:
     yield _topath(paths)
 
 def autoglob(files :Iterable[str], *, force :bool=False) -> Generator[str, None, None]:
-    """In Windows, automatically apply :func:`~glob.glob` and :func:`~os.path.expanduser`, otherwise don't change the input."""
+    """In Windows, automatically apply :func:`~glob.glob` and :func:`~os.path.expanduser`, otherwise don't change the input.
+
+    For example, take the following script:
+
+    >>> import argparse
+    ... from igbpyutils.file import autoglob
+    ... parser = argparse.ArgumentParser(description='Example')
+    ... parser.add_argument('files', metavar="FILE", help="Files", nargs="+")
+    ... args = parser.parse_args()
+    ... paths = autoglob(args.files)
+
+    On a normal \\*NIX shell, calling this script as ``python3 script.py ~/*.py`` would result in
+    ``args.files`` being a list of ``"/home/username/filename.py"`` strings if such files exist, or
+    otherwise a single element of ``"/home/username/*.py"``. However, in a Windows ``cmd.exe`` shell,
+    the aforementioned command always results in ``args.files`` being ``['~/*.py']``. This function
+    fixes that, such that the behavior on Windows is the same as on Linux.
+    """
     from glob import glob
     from os.path import expanduser
     if sys.platform.startswith('win32') or force:
         for f in files:
             f = expanduser(f)
             g = glob(f)  # note glob always returns a list
             # If a *NIX glob doesn't match anything, it isn't expanded,
             # while glob() returns an empty list, so we emulate *NIX.
             if g: yield from g
             else: yield f
     else:
         yield from files
 
-class Pushd:  # cover-not-ge3.11
-    """A context manager that temporarily changes the current working directory."""
+class Pushd:  # cover-req-lt3.11
+    """A context manager that temporarily changes the current working directory.
+
+    On Python >=3.11, this is simply an alias for :func:`contextlib.chdir`."""
     def __init__(self, newdir :Filename):
         self.newdir = newdir
     def __enter__(self):
         self.prevdir = os.getcwd()
         os.chdir(self.newdir)
         return
     def __exit__(self, exc_type, exc_val, exc_tb):
         os.chdir(self.prevdir)
         return False  # raise exception if any
-if sys.hexversion>=0x030B00F0:  # cover-not-le3.10
+if sys.hexversion>=0x030B00F0:  # cover-req-ge3.11
     import contextlib
     Pushd = contextlib.chdir  # type: ignore
-else: pass  # cover-not-ge3.11
+else: pass  # cover-req-lt3.11
 
 def filetypestr(st :os.stat_result) -> str:
     """Return a string naming the file type reported by :func:`os.stat`."""
     if stat.S_ISDIR(st.st_mode): return "directory"
     elif stat.S_ISCHR(st.st_mode): return "character special device file"  # pragma: no cover
     elif stat.S_ISBLK(st.st_mode): return "block special device file"  # pragma: no cover
     elif stat.S_ISREG(st.st_mode): return "regular file"
@@ -133,15 +161,15 @@
 @contextmanager
 def replacer(file :Filename, *, binary :bool=False, encoding=None, errors=None, newline=None):
     """Replace a file by renaming a temporary file over the original.
 
     With this context manager, a temporary file is created in the same directory as the original file.
     The context manager gives you two file handles: the input file, and the output file, the latter
     being the temporary file. You can then read from the input file and write to the output file.
-    When the context manager is exited, it will replace the input file over the temporary file.
+    When the context manager is exited, it will replace the input file with the temporary file.
     If an error occurs in the context manager, the temporary file is unlinked and the original file left unchanged.
 
     Depending on the OS and file system, the :func:`os.replace` used here *may* be an atomic operation.
     However, this function doesn't provide protection against multiple writers and is therefore
     intended for files with a single writer and multiple readers.
     Multiple writers will need to be coordinated with external locking mechanisms.
     """
@@ -190,17 +218,20 @@
         os.replace(tf, dst)
     except BaseException:
         os.unlink(tf)
         raise
 
 # noinspection PyPep8Naming
 @contextmanager
-def NamedTempFileDeleteLater(*args, **kwargs) -> Generator:  # cover-not-ge3.12
-    """A :func:`~tempfile.NamedTemporaryFile` that is unlinked on context manager exit, not on close."""
+def NamedTempFileDeleteLater(*args, **kwargs) -> Generator:  # cover-req-lt3.12
+    """A :func:`~tempfile.NamedTemporaryFile` that is unlinked on context manager exit, not on close.
+
+    On Python >=3.12, this simply calls :func:`tempfile.NamedTemporaryFile` with ``delete=True``
+    and the new ``delete_on_close=False``."""
     tf = NamedTemporaryFile(*args, **kwargs, delete=False)  # type: ignore
     try: yield tf
     finally: os.unlink(tf.name)
 #TODO Later: Once 3.12 is released, change the following to 0x030C00F0
-if sys.hexversion>=0x030C0000:  # cover-not-le3.11
+if sys.hexversion>=0x030C0000:  # cover-req-ge3.12
     from functools import partial
     NamedTempFileDeleteLater = partial(NamedTemporaryFile, delete=True, delete_on_close=False)  # type: ignore
-else: pass  # cover-not-ge3.12
+else: pass  # cover-req-lt3.12
```

### Comparing `igbpyutils-0.0.6/igbpyutils/iter.py` & `igbpyutils-0.0.7/igbpyutils/iter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!python3
 """A Few Useful Iterators
 
 Note the iterator "``gray_product``" that used to be in this module
-has been merged into :mod:`more_itertools` as of its version 9.1.0.
+has been merged into :mod:`more_itertools` as of its version 9.1.0
+as :func:`~more_itertools.gray_product`.
 
 Author, Copyright, and License
 ------------------------------
 Copyright (c) 2022-2023 Hauke Daempfling (haukex@zero-g.net)
 at the Leibniz Institute of Freshwater Ecology and Inland Fisheries (IGB),
 Berlin, Germany, https://www.igb-berlin.de/
 
@@ -22,15 +23,15 @@
 
 You should have received a copy of the GNU General Public License
 along with this program. If not, see https://www.gnu.org/licenses/
 """
 import sys
 from collections.abc import Sized, Iterator, Iterable, Callable, Generator
 from typing import TypeVar, Generic, Optional, Any, overload
-from itertools import tee, zip_longest
+from itertools import zip_longest
 
 _marker = object()
 _T0 = TypeVar('_T0')
 _T1 = TypeVar('_T1')
 _T2 = TypeVar('_T2')
 @overload
 def zip_strict(__iter1: Iterable[_T1]) -> Iterator[tuple[_T1]]: ...  # pragma: no cover
@@ -41,28 +42,30 @@
 @overload
 def zip_strict(
     __iter1: Iterable[_T0],
     __iter2: Iterable[_T0],
     __iter3: Iterable[_T0],
     *iterables: Iterable[_T0],
 ) -> Iterator[tuple[_T0, ...]]: ...  # pragma: no cover
-def zip_strict(*iterables):  # cover-not-ge3.10
-    """Like Python's ``zip``, but requires all iterables to return the same number of items."""
+def zip_strict(*iterables):  # cover-req-lt3.10
+    """Like Python's ``zip``, but requires all iterables to return the same number of items.
+
+    On Python >=3.10, this simply calls :func:`zip` with ``strict=True``."""
     for combo in zip_longest(*iterables, fillvalue=_marker):
         if any( v is _marker for v in combo ):
             raise ValueError("Iterables have different lengths")
         yield combo
-if sys.hexversion>=0x030A00F0:  # cover-not-le3.9
+if sys.hexversion>=0x030A00F0:  # cover-req-ge3.10
     from functools import partial
     zip_strict = partial(zip, strict=True)  # type: ignore
-else: pass  # cover-not-ge3.10
+else: pass  # cover-req-lt3.10
 
 _T = TypeVar('_T', covariant=True)
 class SizedCallbackIterator(Generic[_T], Sized, Iterator[_T]):
-    """Wrapper to add :func:`len` support to an iterator.
+    """Wrapper to add :func:`len` support and a callback to an iterator.
 
     For example, this can be used to wrap a generator which has a known output length
     (e.g. if it returns exactly one item per input item), so that it can then
     be used in libraries like `tqdm <https://tqdm.github.io/>`_."""
     def __init__(self, it :Iterable[_T], length :int, *, strict :bool=False, callback :Optional[Callable[[int, _T], None]]=None):
         if length<0: raise ValueError("length must be >= 0")
         self.it = iter(it)
@@ -106,14 +109,16 @@
         except TypeError:
             if k not in seen_list:
                 seen_list.append(k)
                 yield True
             else:
                 yield False
 
+# this is for "element", probably because PyCharm doesn't detect element:=x
+# noinspection PyUnboundLocalVariable
 def no_duplicates(iterable :Iterable[_V], *, key :Optional[Callable[[_V], Any]] = None, name :str="item") -> Generator[_V, None, None]:
     """Raise a :exc:`ValueError` if there are any duplicate elements in the
     input iterable.
 
     Remember that if you don't want to use this iterator's return values,
     but only use it for checking a list, you need to force it to execute
     by wrapping the call e.g. in a :class:`set` or :class:`list`.
@@ -123,11 +128,10 @@
 
     :func:`more_itertools.duplicates_everseen` could also be used for this purpose,
     but this function returns the values of the input iterable.
 
     The implementation is very similar :func:`more_itertools.unique_everseen`
     and is subject to the same performance considerations.
     """
-    it1, it2 = tee(iterable)
-    for element, unique in zip_strict(it1, is_unique_everseen(it2, key=key)):
+    for unique in is_unique_everseen( (element:=x for x in iterable), key=key ):
         if not unique: raise ValueError(f"duplicate {name}: {element!r}")
         else: yield element
```

### Comparing `igbpyutils-0.0.6/igbpyutils/test.py` & `igbpyutils-0.0.7/igbpyutils/test.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.6/igbpyutils.egg-info/PKG-INFO` & `igbpyutils-0.0.7/igbpyutils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: igbpyutils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Various Python Utilities
 Author-email: Hauke D <haukex@zero-g.net>
 Project-URL: Homepage, https://github.com/haukex/igbpyutils
 Project-URL: Bug Tracker, https://github.com/haukex/igbpyutils/issues
 Project-URL: Documentation, https://igbpyutils.readthedocs.io/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
@@ -27,15 +28,15 @@
 developed at the Leibniz Institute of Freshwater Ecology and Inland Fisheries
 (IGB) in the Forschungsverbund Berlin e.V. (https://www.igb-berlin.de/en).
 
 This is a companion library to the ``igbdatatools`` library
 (https://github.com/haukex/igbdatatools) which normally targets the latest
 Python version.
 This library is intended to contain more general-purpose tools and
-cover a slightly broader range of Python versions, currently Python 3.9 to 3.11.
+cover a slightly broader range of Python versions, currently Python 3.9 to 3.12.
 
 The documentation is available at https://igbpyutils.readthedocs.io/
 
 
 Author, Copyright, and License
 ------------------------------
```

### Comparing `igbpyutils-0.0.6/pyproject.toml` & `igbpyutils-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "igbpyutils"
 description = "Various Python Utilities"
-version = "0.0.6"
+version = "0.0.7"
 authors = [ { name="Hauke D", email="haukex@zero-g.net" } ]
 readme = "README.rst"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS :: MacOS X",
     "Development Status :: 5 - Production/Stable",
     "Topic :: Software Development :: Libraries",
 ]
```

### Comparing `igbpyutils-0.0.6/tests/test_dt.py` & `igbpyutils-0.0.7/tests/test_dt.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.6/tests/test_error.py` & `igbpyutils-0.0.7/tests/test_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import io
 import sys
 import os
 import subprocess
 import inspect
 from contextlib import redirect_stderr
 from pathlib import Path
-from warnings import warn
+from warnings import warn, simplefilter, catch_warnings
 from igbpyutils.error import running_in_unittest, javaishstacktrace, CustomHandlers, init_handlers, extype_fullname, ex_repr
 # noinspection PyProtectedMember
 from igbpyutils.error import _basepath
 import tests.error_test_funcs
 import tests.error_test_unraisable
 
 class TestErrorUtils(unittest.TestCase):
@@ -117,15 +117,16 @@
         except AssertionError as ex:
             self.assertEqual(
                 ("AssertionError() ['assert 1+1==3']",
                  f"\tat {self.mybasepath/'test_error.py'}:{exline} in test_javaishstacktrace"),
                 tuple(javaishstacktrace(ex)) )
 
     def test_customwarn(self):
-        with redirect_stderr(io.StringIO()) as s:
+        with redirect_stderr(io.StringIO()) as s, catch_warnings():
+            simplefilter('default')
             warnline = inspect.stack()[0].lineno
             warn("Test 1")
             with CustomHandlers(): warn("Test 2"); \
                 warn("Test 3", RuntimeWarning)
             warn("Test 4")
             init_handlers(); warn("Test 5")
         self.assertEqual(
```

### Comparing `igbpyutils-0.0.6/tests/test_file.py` & `igbpyutils-0.0.7/tests/test_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,17 @@
         self.assertTrue(len(files)>3)
         # this doesn't really test expanduser but that's ok
         self.assertEqual( files+[noglob], sorted(autoglob([testglob, noglob], force=True)) )
         self.assertEqual( files if sys.platform.startswith('win32') else [testglob], list(autoglob([testglob])) )
 
     def test_pushd(self):
         def realpath(pth):
-            if sys.hexversion>=0x030A00F0:  # cover-not-le3.9
+            if sys.hexversion>=0x030A00F0:  # cover-req-ge3.10
                 return os.path.realpath(pth, strict=True)
-            else:  # cover-not-ge3.10
+            else:  # cover-req-lt3.10
                 return os.path.realpath(pth)
         prevwd = realpath(os.getcwd())
         with (TemporaryDirectory() as td1, TemporaryDirectory() as td2):
             # basic pushd
             with Pushd(td1):
                 self.assertEqual(realpath(os.getcwd()), realpath(td1))
                 with Pushd(td2):
@@ -238,18 +238,18 @@
             self.assertFalse( Path(tf1.name).exists() )
         with NamedTempFileDeleteLater() as tf2:
             tf2.write(b'Bar')
             tf2.close()
             self.assertTrue( Path(tf2.name).exists() )
         self.assertFalse( Path(tf2.name).exists() )
         #TODO Later: Once 3.12 is released, change the following to 0x030C00F0
-        if sys.hexversion>=0x030C0000:  # cover-not-le3.11
+        if sys.hexversion>=0x030C0000:  # cover-req-ge3.12
             # noinspection PyArgumentList
             with NamedTemporaryFile(delete=True, delete_on_close=False) as tf3:
                 tf3.write(b'Quz')
                 tf3.close()
                 self.assertTrue( Path(tf3.name).exists() )
             self.assertFalse( Path(tf3.name).exists() )
-        else: pass  # cover-not-ge3.12
+        else: pass  # cover-req-lt3.12
 
 if __name__ == '__main__':  # pragma: no cover
     unittest.main()
```

### Comparing `igbpyutils-0.0.6/tests/test_iter.py` & `igbpyutils-0.0.7/tests/test_iter.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,16 @@
         # check that an unequal number of columns throws an error
         tbl2 = ((0, "x", "y"), (1, "a"))
         with self.assertRaises(ValueError):
             tuple( zip_strict( *( tuple(x) for x in unzip(tbl2) ) ) )
 
     def test_tee_zip(self):
         """Make sure that the ``tee``-then-``zip`` pattern works as expected,
-        that is, that it really does consume the input one-at-a-time."""
+        that is, that it really does consume the input one-at-a-time.
+        **However**, see the "better variant" in the code below!!"""
         from itertools import tee
         totest = []
         def gen():
             for x in range(1,4):
                 totest.append(f"gen {x}")
                 yield x
         def trans(seq):
@@ -88,14 +89,24 @@
         g1, g2 = tee(gen())
         for i, o in zip_strict(g1, trans(g2)):
             totest.append(f"got {i}-{o}")
         self.assertEqual( totest, [
             'gen 1', 'trans 1-A', 'got 1-A',
             'gen 2', 'trans 2-B', 'got 2-B',
             'gen 3', 'trans 3-C', 'got 3-C'] )
+        totest.clear()
+        # The better variant by Stefan Pochmann at https://stackoverflow.com/a/76271631
+        # (the only minor downside being that PyChram detects "i" as "referenced before assignment")
+        for o in trans( i := x for x in gen() ):
+            # noinspection PyUnboundLocalVariable
+            totest.append(f"got {i}-{o}")
+        self.assertEqual( totest, [
+            'gen 1', 'trans 1-A', 'got 1-A',
+            'gen 2', 'trans 2-B', 'got 2-B',
+            'gen 3', 'trans 3-C', 'got 3-C'] )
 
     def test_gray_product(self):
         # gray_product has been merged into more_itertools, but we'll keep this test here for now anyway
         self.assertEqual( tuple( gray_product( ('a','b','c'), range(1,3) ) ),
             ( ("a",1), ("b",1), ("c",1), ("c",2), ("b",2), ("a",2) ) )
 
         out = gray_product(('foo', 'bar'), (3, 4, 5, 6), ['quz', 'baz'])
```

### Comparing `igbpyutils-0.0.6/tests/test_test.py` & `igbpyutils-0.0.7/tests/test_test.py`

 * *Files identical despite different names*

