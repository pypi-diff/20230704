# Comparing `tmp/cs.ebooks-20230110.tar.gz` & `tmp/cs.ebooks-20230704.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.ebooks-20230110.tar", last modified: Mon Jan  9 22:22:49 2023, max compression
+gzip compressed data, was "cs.ebooks-20230704.tar", last modified: Tue Jul  4 05:42:16 2023, max compression
```

## Comparing `cs.ebooks-20230110.tar` & `cs.ebooks-20230704.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-01-09 22:22:49.498620 cs.ebooks-20230110/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-01-09 22:22:34.000000 cs.ebooks-20230110/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     2967 2023-01-09 22:22:49.498818 cs.ebooks-20230110/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     2077 2023-01-09 22:22:36.000000 cs.ebooks-20230110/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-01-09 22:22:49.490456 cs.ebooks-20230110/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-01-09 22:22:49.490816 cs.ebooks-20230110/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-01-09 22:22:49.490950 cs.ebooks-20230110/lib/python/cs/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-01-09 22:22:49.498304 cs.ebooks-20230110/lib/python/cs/ebooks/
--rw-r--r--   0 cameron    (501) cameron    (502)     1036 2023-01-09 22:22:22.000000 cs.ebooks-20230110/lib/python/cs/ebooks/__init__.py
--rw-r--r--   0 cameron    (501) cameron    (502)      555 2023-01-09 22:22:22.000000 cs.ebooks-20230110/lib/python/cs/ebooks/__main__.py
--rw-r--r--   0 cameron    (501) cameron    (502)     8216 2023-01-09 22:22:22.000000 cs.ebooks-20230110/lib/python/cs/ebooks/apple.py
--rw-r--r--   0 cameron    (501) cameron    (502)    57144 2023-01-09 22:22:22.000000 cs.ebooks-20230110/lib/python/cs/ebooks/calibre.py
--rw-r--r--   0 cameron    (501) cameron    (502)    19471 2023-01-09 22:22:22.000000 cs.ebooks-20230110/lib/python/cs/ebooks/dedrm.py
--rw-r--r--   0 cameron    (501) cameron    (502)    27727 2023-01-09 22:22:22.000000 cs.ebooks-20230110/lib/python/cs/ebooks/kindle.py
--rw-r--r--   0 cameron    (501) cameron    (502)     5360 2023-01-09 22:22:22.000000 cs.ebooks-20230110/lib/python/cs/ebooks/mobi.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-01-09 22:22:49.494625 cs.ebooks-20230110/lib/python/cs.ebooks.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     2967 2023-01-09 22:22:49.000000 cs.ebooks-20230110/lib/python/cs.ebooks.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      492 2023-01-09 22:22:49.000000 cs.ebooks-20230110/lib/python/cs.ebooks.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-01-09 22:22:49.000000 cs.ebooks-20230110/lib/python/cs.ebooks.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      485 2023-01-09 22:22:49.000000 cs.ebooks-20230110/lib/python/cs.ebooks.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-01-09 22:22:49.000000 cs.ebooks-20230110/lib/python/cs.ebooks.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     3788 2023-01-09 22:22:40.000000 cs.ebooks-20230110/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1384 2023-01-09 22:22:49.500188 cs.ebooks-20230110/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-01-09 22:22:36.000000 cs.ebooks-20230110/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-04 05:42:16.094889 cs.ebooks-20230704/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-07-04 05:41:59.000000 cs.ebooks-20230704/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    11926 2023-07-04 05:42:16.095054 cs.ebooks-20230704/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    10971 2023-07-04 05:42:01.000000 cs.ebooks-20230704/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-04 05:42:16.088204 cs.ebooks-20230704/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-04 05:42:16.088601 cs.ebooks-20230704/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-04 05:42:16.088739 cs.ebooks-20230704/lib/python/cs/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-04 05:42:16.094610 cs.ebooks-20230704/lib/python/cs/ebooks/
+-rw-r--r--   0 cameron    (501) cameron    (502)    10079 2023-07-04 05:41:48.000000 cs.ebooks-20230704/lib/python/cs/ebooks/__init__.py
+-rw-r--r--   0 cameron    (501) cameron    (502)      555 2023-07-04 05:41:48.000000 cs.ebooks-20230704/lib/python/cs/ebooks/__main__.py
+-rw-r--r--   0 cameron    (501) cameron    (502)     8225 2023-07-04 05:41:48.000000 cs.ebooks-20230704/lib/python/cs/ebooks/apple.py
+-rw-r--r--   0 cameron    (501) cameron    (502)    57781 2023-07-04 05:41:48.000000 cs.ebooks-20230704/lib/python/cs/ebooks/calibre.py
+-rw-r--r--   0 cameron    (501) cameron    (502)    19643 2023-07-04 05:41:48.000000 cs.ebooks-20230704/lib/python/cs/ebooks/dedrm.py
+-rw-r--r--   0 cameron    (501) cameron    (502)    28033 2023-07-04 05:41:48.000000 cs.ebooks-20230704/lib/python/cs/ebooks/kindle.py
+-rw-r--r--   0 cameron    (501) cameron    (502)     5360 2023-07-04 05:41:48.000000 cs.ebooks-20230704/lib/python/cs/ebooks/mobi.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-04 05:42:16.092010 cs.ebooks-20230704/lib/python/cs.ebooks.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    11926 2023-07-04 05:42:16.000000 cs.ebooks-20230704/lib/python/cs.ebooks.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      492 2023-07-04 05:42:16.000000 cs.ebooks-20230704/lib/python/cs.ebooks.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-07-04 05:42:16.000000 cs.ebooks-20230704/lib/python/cs.ebooks.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      495 2023-07-04 05:42:16.000000 cs.ebooks-20230704/lib/python/cs.ebooks.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-07-04 05:42:16.000000 cs.ebooks-20230704/lib/python/cs.ebooks.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    12755 2023-07-04 05:42:07.000000 cs.ebooks-20230704/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1459 2023-07-04 05:42:16.095741 cs.ebooks-20230704/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-07-04 05:42:01.000000 cs.ebooks-20230704/setup.py
```

### Comparing `cs.ebooks-20230110/lib/python/cs/ebooks/__main__.py` & `cs.ebooks-20230704/lib/python/cs/ebooks/__main__.py`

 * *Files identical despite different names*

### Comparing `cs.ebooks-20230110/lib/python/cs/ebooks/apple.py` & `cs.ebooks-20230704/lib/python/cs/ebooks/apple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python3
 
 ''' Apple Books access.
 '''
 
 from contextlib import contextmanager
+from dataclasses import dataclass
 from getopt import GetoptError
 from glob import glob
 from os.path import join as joinpath
 from pprint import pprint
 import sys
+from typing import Optional
 
 from sqlalchemy import (
     Column,
     Float,
     Integer,
     LargeBinary,
     String,
@@ -206,19 +208,17 @@
     self.collections = Collection
     self.collection_members = CollectionMember
 
 class AppleBooksCommand(BaseCommand):
   ''' Command line access to Apple Books.
   '''
 
-  def apply_defaults(self):
-    ''' Set up the default values in `options`.
-    '''
-    options = self.options
-    options.apple_path = None
+  @dataclass
+  class Options(BaseCommand.Options):
+    apple_path: Optional[str] = None
 
   @contextmanager
   def run_context(self):
     ''' Prepare the `SQLTags` around each command invocation.
     '''
     with super().run_context():
       options = self.options
```

### Comparing `cs.ebooks-20230110/lib/python/cs/ebooks/calibre.py` & `cs.ebooks-20230704/lib/python/cs/ebooks/calibre.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 # pylint: disable=too-many-lines
 
 ''' Support for Calibre libraries.
 '''
 
 from code import interact
 from contextlib import contextmanager
+from dataclasses import dataclass, field
 from datetime import datetime, timezone
 import filecmp
 from functools import total_ordering
 from getopt import GetoptError
 from itertools import chain
 import json
 import os
 from os.path import (
     basename,
+    dirname,
     exists as existspath,
     expanduser,
     isabs as isabspath,
     isdir as isdirpath,
     isfile as isfilepath,
     join as joinpath,
     splitext,
@@ -48,31 +50,32 @@
 from cs.cmdutils import BaseCommand
 from cs.context import contextif
 from cs.deco import cachedmethod
 from cs.fs import FSPathBasedSingleton, HasFSPath, shortpath
 from cs.lex import (
     cutprefix,
     get_dotted_identifier,
+    lc_,
     FormatableMixin,
     FormatAsError,
 )
 from cs.logutils import warning, error
 from cs.numeric import intif
 from cs.obj import SingletonMixin
 from cs.pfx import Pfx, pfx_call, pfx_method
 from cs.progress import progressbar
 from cs.psutils import run
-from cs.resources import MultiOpenMixin
+from cs.resources import MultiOpenMixin, RunState, uses_runstate
 from cs.sqlalchemy_utils import (
     ORM, BasicTableMixin, HasIdMixin, RelationProxy, proxy_on_demand_field
 )
 from cs.tagset import TagSet
 from cs.threads import locked
 from cs.units import transcribe_bytes_geek
-from cs.upd import UpdProxy, run_task, uses_upd, print  # pylint: disable=redefined-builtin
+from cs.upd import UpdProxy, uses_upd, print  # pylint: disable=redefined-builtin
 
 from .dedrm import DeDRMWrapper, DEDRM_PACKAGE_PATH_ENVVAR
 
 class CalibreTree(FSPathBasedSingleton, MultiOpenMixin):
   ''' Work with a Calibre ebook tree.
   '''
 
@@ -377,45 +380,45 @@
               pfx_call(MB.make_cbz, cbzpath)
               self.add_format(cbzpath, force=replace_format)
           else:
             raise ValueError(
                 "no AZW3, AZW or MOBI format from which to construct a CBZ"
             )
 
+      @uses_runstate
       def pull(
           self,
           obook,
           *,
           doit=True,
           formats=None,
-          runstate=None,
           force=False,
           quiet=False,
           verbose=False,
+          runstate: RunState,
       ):
         ''' Pull formats from another `CalibreBook`.
 
             Parameters:
             * `obook`: the other book
             * `doit`: optional flag, default `True`;
               import formats if true, report actions otherwise
             * `formats`: optional list of Calibre format keys to pull if present
-            * `runstate`: optional `RunState` for early termination
             * `force`: optional flag, default `False`;
               if true import formats even if already present
             * `quiet`: optional flag, default `False`;
               if true only print warnings
             * `verbose`: optional flag, default `False`;
               if true print all actions and inactions
         '''
         if formats is None:
           formats = sorted(obook.formats.keys())
         with Pfx("%s <= %s", self, obook):
           for fmtk in formats:
-            if runstate and runstate.cancelled:
+            if runstate.cancelled:
               break
             ofmtpath = obook.formatpath(fmtk)
             if ofmtpath is None:
               continue
             with Pfx(fmtk):
               self.pull_format(
                   ofmtpath,
@@ -505,14 +508,24 @@
   @cachedmethod
   def db(self):
     ''' The associated `CalibreMetadataDB` ORM,
         instantiated on demand.
     '''
     return CalibreMetadataDB(self)
 
+  @contextmanager
+  def db_session(self):
+    ''' Context manager for a database session.
+        This is not fired by `startup_shutdown` because any callout
+        to the Calibre command executables also want exclusive
+        access to the database.
+    '''
+    with self.db.session() as session:
+      yield session
+
   def dbshell(self):
     ''' Interactive db shell.
     '''
     return self.db.shell()
 
   @uses_upd
   def preload(self, upd):
@@ -595,15 +608,15 @@
     subp_options.setdefault('capture_output', True)
     subp_options.setdefault('check', False)
     subp_options.setdefault('text', True)
     if not isabspath(calcmd):
       calcmd = joinpath(self.CALIBRE_BINDIR_DEFAULT, calcmd)
     calargv = [calcmd, *calargv]
     cp = run(calargv, doit=doit, quiet=quiet, **subp_options)
-    if cp.stdout and not quiet:
+    if cp is not None and cp.stdout and not quiet:
       print(" ", cp.stdout.rstrip().replace("\n", "\n  "))
     return cp
 
   def calibredb(self, dbcmd, *argv, doit=True, quiet=False, **subp_options):
     ''' Run `dbcmd` via the `calibredb` command.
         Return a `CompletedProcess` or `None` if `doit` is false.
     '''
@@ -1032,50 +1045,48 @@
   }
 
   # mapping of target format key to source format and extra options
   CONVERT_MAP = {
       'EPUB': (['MOBI', 'AZW', 'AZW3'], ()),
   }
 
-  class OPTIONS_CLASS(BaseCommand.OPTIONS_CLASS):
+  @dataclass
+  class Options(BaseCommand.Options):
     ''' Special class for `self.options` with various properties.
     '''
 
-    def __init__(
-        self,
-        kindle_path=None,
-        calibre_path=None,
-        calibre_path_other=None,
-        linkto_dirpath=None,
-        **kw,
-    ):
-      super().__init__(**kw)
-      from .kindle import KindleTree  # pylint: disable=import-outside-toplevel
-      try:
-        # pylint: disable=protected-access
-        kindle_path = KindleTree._resolve_fspath(kindle_path)
-      except ValueError:
-        kindle_path = None
-      try:
-        # pylint: disable=protected-access
-        calibre_path_other = CalibreTree._resolve_fspath(
-            calibre_path_other,
-            envvar=CalibreCommand.OTHER_LIBRARY_PATH_ENVVAR
+    calibre_path: str = field(
+        default_factory=lambda: CalibreTree.
+        _resolve_fspath(None, CalibreTree.FSPATH_ENVVAR)
+    )
+    calibre_path_other: Optional[str] = field(
+        default_factory=lambda: (
+            CalibreTree.
+            _resolve_fspath(None, CalibreCommand.OTHER_LIBRARY_PATH_ENVVAR)
+            if CalibreCommand.OTHER_LIBRARY_PATH_ENVVAR in os.environ else None
         )
-      except ValueError:
-        calibre_path_other = None
-      self.kindle_path = kindle_path
-      self.calibre_path = calibre_path
-      self.calibre_path_other = calibre_path_other
-      self.linkto_dirpath = (
-          linkto_dirpath
-          or os.environ.get(CalibreCommand.DEFAULT_LINKTO_DIRPATH_ENVVAR)
-          or expanduser(CalibreCommand.DEFAULT_LINKTO_DIRPATH)
+    )
+    dedrm_package_path: Optional[str] = field(
+        default_factory=lambda: os.environ.get(DEDRM_PACKAGE_PATH_ENVVAR)
+    )
+
+    def _default_kindle_path():
+      from .kindle import KindleTree  # pylint: disable=import-outside-toplevel
+      return (
+          KindleTree._resolve_fspath(None)
+          if KindleTree.FSPATH_ENVVAR in os.environ else None
       )
 
+    kindle_path: Optional[str] = field(default_factory=_default_kindle_path)
+    linkto_dirpath: str = field(
+        default_factory=lambda: os.environ.get(
+            CalibreCommand.DEFAULT_LINKTO_DIRPATH_ENVVAR
+        ) or expanduser(CalibreCommand.DEFAULT_LINKTO_DIRPATH)
+    )
+
     @property
     def calibre(self):
       ''' The `CalibreTree` from `self.calibre_path`.
       '''
       return CalibreTree(self.calibre_path)
 
     @property
@@ -1091,20 +1102,14 @@
       ''' The `KindleTree` from `self.kindle_path`.
       '''
       if self.kindle_path is None:
         raise AttributeError(".kindle: no .kindle_path")
       from .kindle import KindleTree  # pylint: disable=import-outside-toplevel
       return KindleTree(self.kindle_path)
 
-  def apply_defaults(self):
-    ''' Set up the default values in `options`.
-    '''
-    options = self.options
-    options.dedrm_package_path = os.environ.get(DEDRM_PACKAGE_PATH_ENVVAR)
-
   def apply_opt(self, opt, val):
     ''' Apply a command line option.
     '''
     options = self.options
     if opt == '-C':
       options.calibre_path = val
     elif opt == '-K':
@@ -1115,16 +1120,18 @@
       super().apply_opt(opt, val)
 
   @contextmanager
   def run_context(self):
     ''' Prepare the `SQLTags` around each command invocation.
     '''
     with super().run_context():
-      with self.options.calibre:
-        yield
+      calibre = self.options.calibre
+      with calibre:
+        with calibre.db_session():
+          yield
 
   @staticmethod
   def books_from_spec(calibre, book_spec):
     ''' Generator yielding `CalibreBook` instances from `book_spec`.
     '''
     # raw dbid
     try:
@@ -1362,38 +1369,49 @@
       with upd.run_task('linkto: ') as proxy:
         if runstate.cancelled:
           break
         proxy.text = str(cbook)
         with Pfx(cbook):
           fmttags = cbook.format_tagset()
           series_name = fmttags.get('series.name')
+          if series_name:
+            series_name = series_name.strip()
           name_format = link_format or (
               '{series.name:lc}--{series.index}--{title:lc}'
               if series_name else '{title:lc}'
           )
           name = (
               cbook.format_as(name_format).replace('_', '-').replace('/', ':')
           )
+          name_subdir = (
+              lc_(series_name).replace('/', ':')
+              if series_name and not link_format else ''
+          )
           for fmt in formats:
             if runstate.cancelled:
               break
             proxy.text = f'{cbook}: {fmt}'
             srcpath = cbook.formatpath(fmt)
             if srcpath is None:
               continue
-            dstpath = joinpath(linkto_dirpath, name + '.' + fmt.lower())
+            dstpath = joinpath(
+                linkto_dirpath, name_subdir, name + '.' + fmt.lower()
+            )
             if existspath(dstpath):
               if force:
                 warning("dst already exists, will be replaced: %s", dstpath)
+                (verbose or not doit) and print("unlink", shortpath(dstpath))
+                doit and pfx_call(os.unlink, dstpath)
               else:
                 ##warning("dst already exists, skipped: %s", dstpath)
                 continue
-            if existspath(dstpath):
-              (verbose or not doit) and print("unlink", shortpath(dstpath))
-              doit and pfx_call(os.unlink, dstpath)
+            dstdir = dirname(dstpath)
+            if not isdirpath(dstdir) and doit:
+              verbose and print("mkdir", shortpath(dstdir))
+              pfx_call(os.mkdir, dstdir)
             (quiet and doit
              ) or print("link", shortpath(srcpath), '=>', shortpath(dstpath))
             doit and pfx_call(os.link, srcpath, dstpath)
             if first_format:
               break
           proxy.text = f'{cbook}'
     if runstate.cancelled:
@@ -1695,27 +1713,26 @@
                       )
                   )
                   continue
                 else:
                   cbook, = cbooks
                 cbook.pull(
                     obook,
-                    runstate=runstate,
                     doit=doit,
                     force=force,
                     quiet=quiet,
                     verbose=verbose
                 )
         if runstate.cancelled:
           xit = 1
         return xit
 
   def cmd_shell(self, argv):
     ''' Usage: {cmd}
-          Run an interactive Python prompt with some predefined named:
+          Run an interactive Python prompt with some predefined names:
           calibre: the CalibreTree
           options: self.options
     '''
     if argv:
       raise GetoptError("extra arguments: %r" % (argv,))
     options = self.options
     interact(
```

### Comparing `cs.ebooks-20230110/lib/python/cs/ebooks/dedrm.py` & `cs.ebooks-20230704/lib/python/cs/ebooks/dedrm.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
     This is an experimental module aimed at making the DeDRM/noDRM
     packages run outside Calibre's plugin environment.
     It does not yet work.
 '''
 
 from contextlib import contextmanager, redirect_stdout
+from dataclasses import dataclass, field
 from datetime import datetime
 from getopt import GetoptError
 import importlib
 import json
 import os
 from os.path import (
     basename,
@@ -25,15 +26,15 @@
 import sys
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 import time
 from typing import Iterable, List, Optional
 
 from cs.cmdutils import BaseCommand
 from cs.context import stackattrs
-from cs.deco import fmtdoc
+from cs.deco import fmtdoc, Promotable
 from cs.fileutils import atomic_filename
 from cs.lex import r, stripped_dedent
 from cs.logutils import warning
 from cs.pfx import Pfx, pfx_call, pfx_method
 from cs.sqltags import SQLTags
 from cs.upd import print  # pylint: disable=redefined-builtin
 
@@ -51,18 +52,19 @@
     -D  Specify the filesystem path to the DeDRM/noDRM plugin top level.
         For example, if you had a checkout of git@github.com:noDRM/DeDRM_tools.git
         at /path/to/DeDRM_tools--noDRM you could supply:
         -D /path/to/DeDRM_tools--noDRM/DeDRM_plugin
         or place that value in the $DEDRM_PACKAGE_PATH environment variable.
   '''
 
-  def apply_defaults(self):
-    super().apply_defaults()
-    options = self.options
-    options.dedrm_package_path = None
+  @dataclass
+  class Options(BaseCommand.Options):
+    dedrm_package_path: Optional[str] = field(
+        default_factory=lambda: os.environ.get(DEDRM_PACKAGE_PATH_ENVVAR)
+    )
 
   def apply_opt(self, opt, val):
     badopt = False
     if opt == '-D':
       self.options.dedrm_package_path = val
     else:
       raise RuntimeError("unhandled option")
@@ -156,15 +158,15 @@
         output_filename = normpath(
             joinpath(
                 realpath(output_dirpath), 'decrypted-' + basename(filename)
             )
         )
         pfx_call(dedrm.remove, filename, output_filename, exists_ok=exists_ok)
 
-class DeDRMWrapper:
+class DeDRMWrapper(Promotable):
   ''' Class embodying the DeDRM/noDRM package actions.
   '''
 
   # The package name to use for the DeDRM/noDRM package.
   # We also use these symbols to convince the DRM package to run
   # without being installed as a calibre plugin inside calibre.
   DEDRM_PACKAGE_NAME = 'dedrm'
@@ -310,15 +312,15 @@
       with stackattrs(
           sys,
           path=[tmpdirpath, joinpath(tmpdirpath, self.DEDRM_PACKAGE_NAME)] +
           sys.path):
         import builtins
         with stackattrs(builtins, print=print):
           with redirect_stdout(sys.stderr):
-            import prefs
+            import prefs  # imported for its side effect
             yield
 
   def import_name(self, module_name, name=None, *, package=None):
     ''' Shim for `importlib.import_module` to import from the DeDRM/noDRM package.
 
         Parameters:
         * `module_name`: the module name to import
@@ -425,20 +427,19 @@
 
   @classmethod
   def promote(cls, obj) -> "DeDRMWrapper":
     ''' Promote an object to a `DeDRMWrapper`.
 
         If `obj` is `None` or a `str` return `DeDRMWrapper(dedrm_package_path=obj)`.
     '''
-    if not isinstance(obj, cls):
-      if obj is None or isinstance(obj, str):
-        obj = cls(dedrm_package_path=obj)
-      else:
-        raise TypeError("cannot promote %s", r(obj))
-    return obj
+    if isinstance(obj, cls):
+      return obj
+    if obj is None or isinstance(obj, str):
+      return cls(dedrm_package_path=obj)
+    raise TypeError("%s.promote: cannot promote %s", cls.__name__, r(obj))
 
 class DeDRMOverride:
   ''' A collection of override methods from the DeDRM/noDRM `DeDRM` class
       which we use to make it work outside the calibre plugin stuff.
   '''
 
 class DeDRM_PrefsOverride:
@@ -455,16 +456,18 @@
         there are distinct classes all over the code, a disaster.
         This class is bug-for-bug compatible.
     '''
     pass
 
   # interface to needed routines in openssl's libcrypto
   def _load_crypto_libcrypto():
-    from ctypes import CDLL, byref, POINTER, c_void_p, c_char_p, c_int, c_long, \
-        Structure, c_ulong, create_string_buffer, addressof, string_at, cast
+    from ctypes import (
+        CDLL, byref, POINTER, c_void_p, c_char_p, c_int, c_long, Structure,
+        c_ulong, create_string_buffer, addressof, string_at, cast
+    )
     from ctypes.util import find_library
 
     libcrypto = find_library('crypto')
     if libcrypto is None:
       raise DrmException(u"libcrypto not found")
     libcrypto = CDLL(libcrypto)
```

### Comparing `cs.ebooks-20230110/lib/python/cs/ebooks/kindle.py` & `cs.ebooks-20230704/lib/python/cs/ebooks/kindle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/usr/bin/env python3
 
 ''' Support for Kindle libraries.
 '''
 
 from contextlib import contextmanager
+from dataclasses import dataclass, field
 import filecmp
 from getopt import GetoptError
 import os
 from os.path import (
     dirname,
     expanduser,
     exists as existspath,
     isdir as isdirpath,
     isfile as isfilepath,
     join as joinpath,
 )
 import sys
+from typing import Optional
 
 from icontract import require
 from sqlalchemy import (
     Column,
     ForeignKey,
     Integer,
     String,
@@ -627,32 +629,42 @@
   -C calibre_library
     Specify calibre library location.
   -K kindle_library
     Specify kindle library location.'''
 
   SUBCOMMAND_ARGV_DEFAULT = 'info'
 
-  def apply_defaults(self):
+  @dataclass
+  class Options(BaseCommand.Options):
     ''' Set up the default values in `options`.
     '''
-    options = self.options
-    try:
-      # pylint: disable=protected-access
-      kindle_path = KindleTree._resolve_fspath(None)
-    except ValueError:
-      kindle_path = None
-    from .calibre import CalibreTree  # pylint: disable=import-outside-toplevel
-    try:
-      # pylint: disable=protected-access
-      calibre_path = CalibreTree._resolve_fspath(None)
-    except ValueError:
-      calibre_path = None
-    options.kindle_path = kindle_path
-    options.calibre_path = calibre_path
-    options.dedrm_package_path = os.environ.get(DEDRM_PACKAGE_PATH_ENVVAR)
+
+    def _kindle_path():
+      try:
+        # pylint: disable=protected-access
+        kindle_path = KindleTree._resolve_fspath(None)
+      except ValueError:
+        kindle_path = None
+      return kindle_path
+
+    kindle_path: Optional[str] = field(default_factory=_kindle_path)
+
+    def _calibre_path():
+      from .calibre import CalibreTree  # pylint: disable=import-outside-toplevel
+      try:
+        # pylint: disable=protected-access
+        calibre_path = CalibreTree._resolve_fspath(None)
+      except ValueError:
+        calibre_path = None
+      return calibre_path
+
+    calibre_path: Optional[str] = field(default_factory=_calibre_path)
+    dedrm_package_path: Optional[str] = field(
+        default_factory=lambda: os.environ.get(DEDRM_PACKAGE_PATH_ENVVAR)
+    )
 
   def apply_opt(self, opt, val):
     ''' Apply a command line option.
     '''
     options = self.options
     if opt == '-C':
       options.calibre_path = val
@@ -663,15 +675,15 @@
       )
       for db_subpath in db_subpaths:
         db_fspath = joinpath(val, db_subpath)
         if existspath(db_fspath):
           break
       else:
         raise GetoptError(
-            "cannot find db at %s" % (" or ".join(map(repr, dbsubpaths)),)
+            "cannot find db at %s" % (" or ".join(map(repr, db_subpaths)),)
         )
       options.kindle_path = dirname(db_fspath)
     else:
       super().apply_opt(opt, val)
 
   @contextmanager
   def run_context(self):
```

### Comparing `cs.ebooks-20230110/lib/python/cs/ebooks/mobi.py` & `cs.ebooks-20230704/lib/python/cs/ebooks/mobi.py`

 * *Files identical despite different names*

### Comparing `cs.ebooks-20230110/setup.cfg` & `cs.ebooks-20230704/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = cs.ebooks
-version = 20230110
+version = 20230704
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
-description = Utilities and command line for working with EBooks. Basic support for talking to Apple Books, Calibre, Kindle, Mobi.
+description = Utilities and command line for working with EBooks. Basic support for talking to Apple Books, Calibre, Kindle, Mobi. These form the basis of my personal Kindle and Calibre workflow.
 keywords = python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
@@ -20,34 +20,34 @@
 
 [options]
 package_dir = 
 	= lib/python
 install_requires = 
 	cs.app.osx.defaults
 	cs.app.osx.plist>=20221228
-	cs.cmdutils>=20221228
-	cs.context>=20230109
-	cs.deco>=20221214
-	cs.fileutils>=20221118
-	cs.fs>=20221221
-	cs.fstags>=20221228
-	cs.lex>=20220918
-	cs.logutils>=20220531
+	cs.cmdutils>=20230703
+	cs.context>=20230331
+	cs.deco>=20230331
+	cs.fileutils>=20230421
+	cs.fs>=20230401
+	cs.fstags>=20230407
+	cs.lex>=20230401
+	cs.logutils>=20230212
 	cs.numeric>=20220606
 	cs.obj>=20220918
-	cs.pfx>=20221118
-	cs.progress>=20221207
-	cs.psutils>=20221228
-	cs.resources>=20221228
-	cs.sqlalchemy_utils
-	cs.sqltags>=20221228
-	cs.tagset>=20221228
-	cs.threads>=20221228
+	cs.pfx>=20230604
+	cs.progress>=20230401
+	cs.psutils>=20230612
+	cs.resources>=20230503
+	cs.sqlalchemy_utils>=20230612
+	cs.sqltags>=20230612
+	cs.tagset>=20230612
+	cs.threads>=20230331
 	cs.units
-	cs.upd>=20221228
+	cs.upd>=20230401
 	icontract
 	mobi
 	pycryptodomex
 	sqlalchemy
 	typeguard
 
 [egg_info]
```

