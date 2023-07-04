# Comparing `tmp/medit-0.0.5.tar.gz` & `tmp/medit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medit-0.0.5.tar", max compression
+gzip compressed data, was "medit-0.0.6.tar", max compression
```

## Comparing `medit-0.0.5.tar` & `medit-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2328 2023-07-03 06:21:56.302488 medit-0.0.5/Readme.md
--rw-r--r--   0        0        0        0 2023-06-16 07:35:55.912297 medit-0.0.5/medit/__init__.py
--rwxr-xr-x   0        0        0     2192 2023-07-03 06:21:56.302488 medit-0.0.5/medit/cli.py
--rw-r--r--   0        0        0     2362 2023-07-03 06:51:24.784057 medit-0.0.5/medit/medit.ui
--rw-r--r--   0        0        0     5064 2023-07-03 07:10:06.510948 medit-0.0.5/medit/meditor.py
--rw-r--r--   0        0        0     7517 2023-07-03 06:21:56.302488 medit-0.0.5/medit/mview.py
--rw-r--r--   0        0        0        0 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/__init__.py
--rw-r--r--   0        0        0    18966 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/github-markdown-dark.css
--rw-r--r--   0        0        0    18979 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/github-markdown-light.css
--rw-r--r--   0        0        0     5061 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/pygments-solarized-style/solarized-dark.css
--rw-r--r--   0        0        0     5061 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/pygments-solarized-style/solarized-light.css
--rw-r--r--   0        0        0    36899 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/solarized-dark-all-sites.css
--rw-r--r--   0        0        0    36890 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/solarized-light-all-sites.css
--rw-r--r--   0        0        0     4282 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/thomasf-solarized-css/solarized-dark.css
--rw-r--r--   0        0        0     4282 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/thomasf-solarized-css/solarized-light.css
--rwxr-xr-x   0        0        0     8338 2023-07-03 06:21:56.302488 medit-0.0.5/medit/ui.py
--rw-r--r--   0        0        0     5023 2023-07-03 06:21:56.302488 medit-0.0.5/medit/utils.py
--rwxr-xr-x   0        0        0     6266 2023-06-29 19:10:09.897127 medit-0.0.5/medit/yatl.py
--rw-r--r--   0        0        0     2315 2023-07-03 07:18:17.940235 medit-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3269 1970-01-01 00:00:00.000000 medit-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3100 2023-07-03 07:44:20.904244 medit-0.0.6/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-16 07:35:55.912297 medit-0.0.6/medit/__init__.py
+-rwxr-xr-x   0        0        0     2192 2023-07-03 06:21:56.302488 medit-0.0.6/medit/cli.py
+-rw-r--r--   0        0        0     2362 2023-07-03 06:51:24.784057 medit-0.0.6/medit/medit.ui
+-rw-r--r--   0        0        0     5067 2023-07-04 06:15:16.074437 medit-0.0.6/medit/meditor.py
+-rw-r--r--   0        0        0     7517 2023-07-03 06:21:56.302488 medit-0.0.6/medit/mview.py
+-rw-r--r--   0        0        0        0 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/__init__.py
+-rw-r--r--   0        0        0    18966 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/github-markdown-dark.css
+-rw-r--r--   0        0        0    18979 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/github-markdown-light.css
+-rw-r--r--   0        0        0     5061 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/pygments-solarized-style/solarized-dark.css
+-rw-r--r--   0        0        0     5061 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/pygments-solarized-style/solarized-light.css
+-rw-r--r--   0        0        0    36899 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/solarized-dark-all-sites.css
+-rw-r--r--   0        0        0    36890 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/solarized-light-all-sites.css
+-rw-r--r--   0        0        0     4282 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/thomasf-solarized-css/solarized-dark.css
+-rw-r--r--   0        0        0     4282 2023-07-03 06:21:56.302488 medit-0.0.6/medit/styles/external/thomasf-solarized-css/solarized-light.css
+-rwxr-xr-x   0        0        0     8700 2023-07-04 06:36:24.786456 medit-0.0.6/medit/ui.py
+-rw-r--r--   0        0        0     5361 2023-07-04 06:15:16.098475 medit-0.0.6/medit/utils.py
+-rwxr-xr-x   0        0        0     6266 2023-06-29 19:10:09.897127 medit-0.0.6/medit/yatl.py
+-rw-r--r--   0        0        0     2315 2023-07-04 06:37:03.356763 medit-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4041 1970-01-01 00:00:00.000000 medit-0.0.6/PKG-INFO
```

### Comparing `medit-0.0.5/Readme.md` & `medit-0.0.6/Readme.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,34 @@
-# MEdit - Markup Editor
+# MEdit - Previewing [M]arkup [Editor]
+
+A simple text editor based on PyQt6/QScintilla with the following goals in mind:
+
+- Auto-saves and tracks filesystem in order to make loading/saving obsolete
+- Syntax highlighting for typical file formats
+- Previewing markdown or representations in other file formats
+- Support for local and remote images in Markdown/reST
+- Decent nice looking interface for easily distractable people like me
+
+As almost all of my projects, `medit` is in dangerous alpha state - use it with
+care and don't believe anything written here.
 
 
 ## Installation
 
 ```sh
 [<PYTHON> -m] pip[3] install [--upgrade] medit
 ```
 
 
 ## Usage
 
+```sh
+medit [<PATH>]  # will open medit in given directory or on given file
+```
+
 
 ## Development & Contribution
 
 ```sh
 pip3 install -U poetry pre-commit
 git clone --recurse-submodules https://projects.om-office.de/frans/pocketrockit.git
 cd pocketrockit
@@ -23,55 +38,59 @@
 poetry install
 ```
 
 After modifications, this way a newly built wheel can be checked and installed:
 
 ```sh
 poetry build
-poetry run twine check dist/pocketrockit-0.0.25-py3-none-any.whl
-python3 -m pip install --user --upgrade dist/pocketrockit-0.0.25-py3-none-any.whl
+poetry run twine check dist/medit-0.0.5-py3-none-any.whl
+python3 -m pip install --user --upgrade dist/medit-0.0.5-py3-none-any.whl
 ```
 
-## 1.0 TODO
+## My personal MLP (v1.0) goals
 
 * [x] File to title
 * [x] File viewer for Plain, Python, YAML, JSON, ..
 * [x] Autosave
+* [x] Manage word wrap in editor
 * [ ] Autoload
+* [ ] Multi-File Undo/Redo
 * [ ] Change into / step up current directory
 * [ ] Zen mode
 * [ ] Recent files
 * [ ] Search/open files
 * [ ] Search in files
-* [ ] Preview for Markdown/.. only
-* [ ] Manage word wrap in editor
+* [ ] Preview for previewable only
 * [ ] Hightlight todo.txt
 * [ ] Notify external file changes
 * [ ] (Re-)store zoom and fullscreen
 * [ ] File ignore filter
-* [ ] Icon
+* [ ] Icon / .desktop file
 * [ ] Proper Qt style
 * [ ] Show local images
 * [ ] Show remote images
 * [ ] Slim file / folder create / rename
 * [ ] Proper View CSS selector
 * [ ] View follows editor
 * [ ] Links clickable
 * [ ] Fix Links to support `(text)[url]` syntax
 
 
 ## Feature ideas
 
-* [ ] Export to Pdf / Html / docx ..
+* [ ] Export to Pdf / Html / Docx ..
 * [ ] Copy / paste images
 * [ ] Drag & drop images
 * [ ] Spell checker
+* [ ] Script console with preview
+* [ ] Preview rules (markdown->HTML, xml/json/yaml -> xml/json/yaml ..)
 
 
 ## Read
+
 * https://web.archive.org/web/20190604145031/https://qscintilla.com/prepare-image-hack/
 
 * https://github.com/sindresorhus/github-markdown-css
 * https://python-markdown.github.io/extensions/code_hilite/#step-1-download-and-install-pygments
 * https://github.com/richleland/pygments-css
 * https://github.com/OzakIOne/markdown-github-dark
 * https://github.com/jamiemcg/remarkable
```

### Comparing `medit-0.0.5/medit/cli.py` & `medit-0.0.6/medit/cli.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.5/medit/medit.ui` & `medit-0.0.6/medit/medit.ui`

 * *Files identical despite different names*

### Comparing `medit-0.0.5/medit/meditor.py` & `medit-0.0.6/medit/meditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         self.setMarginsFont(font)
         # self.zoomIn()
         # self.zoomOut()
 
         # Margin 0 is used for line numbers
         fontmetrics = QtGui.QFontMetrics(font)
         self.setMarginsFont(font)
-        self.setMarginWidth(0, fontmetrics.boundingRect("000").width()+ 6)
-        #self.setMarginLineNumbers(0, True)
+        self.setMarginWidth(0, fontmetrics.boundingRect("000").width() + 6)
+        # self.setMarginLineNumbers(0, True)
         self.setMarginsBackgroundColor(QtGui.QColor("#eee8d5"))
         self.setMarginsForegroundColor(QtGui.QColor("#93a1a1"))
         # self.setMarginBackgroundColor(1, QtGui.QColor("lightgray"))
 
         # self._marker = None
         # Clickable margin 1 for showing markers
         # self.setMarginSensitivity(1, True)
@@ -53,15 +53,15 @@
         self.SendScintilla(Qsci.QsciScintilla.SCI_STYLESETFONT, 1, "Courier".encode())
 
         # Don't want to see the horizontal scrollbar at all
         # Use raw message to Scintilla here (all messages are documented
         # here: http://www.scintilla.org/ScintillaDoc.html)
         self.SendScintilla(Qsci.QsciScintilla.SCI_SETHSCROLLBAR, 0)
 
-        #self.setWrapMode(self.WrapMode.WrapWord)
+        # self.setWrapMode(self.WrapMode.WrapWord)
         self.setWrapMode(self.WrapMode.WrapNone)
         self.setEolMode(self.EolMode.EolUnix)
         self.setEolVisibility(False)
         self.setWhitespaceVisibility(self.WhitespaceVisibility.WsVisible)
 
         # self.image = QImage("logo_mk.png")
         # painter = QPainter()
```

### Comparing `medit-0.0.5/medit/mview.py` & `medit-0.0.6/medit/mview.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.5/medit/styles/external/github-markdown-dark.css` & `medit-0.0.6/medit/styles/external/github-markdown-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.5/medit/styles/external/github-markdown-light.css` & `medit-0.0.6/medit/styles/external/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.5/medit/styles/external/pygments-solarized-style/solarized-dark.css` & `medit-0.0.6/medit/styles/external/pygments-solarized-style/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.5/medit/styles/external/pygments-solarized-style/solarized-light.css` & `medit-0.0.6/medit/styles/external/pygments-solarized-style/solarized-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.5/medit/styles/external/solarized-dark-all-sites.css` & `medit-0.0.6/medit/styles/external/solarized-dark-all-sites.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.5/medit/styles/external/solarized-light-all-sites.css` & `medit-0.0.6/medit/styles/external/solarized-light-all-sites.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.5/medit/styles/external/thomasf-solarized-css/solarized-dark.css` & `medit-0.0.6/medit/styles/external/thomasf-solarized-css/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.5/medit/styles/external/thomasf-solarized-css/solarized-light.css` & `medit-0.0.6/medit/styles/external/thomasf-solarized-css/solarized-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.5/medit/ui.py` & `medit-0.0.6/medit/ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #!/usr/bin/env python3
 
 """QrM - Connect to reMarkable and modify contents
 """
 
 # pylint: disable=invalid-name
 
+import asyncio
 import json
 import logging
 import os
 import signal
 import sys
 from contextlib import suppress
 from pathlib import Path
-import asyncio
+
+import qdarktheme
 from PyQt6 import QtCore, QtGui, QtWidgets, uic
 from PyQt6.QtWebEngineWidgets import QWebEngineView
-from medit.utils import fs_changes, watchdog, setup_logging
-import qdarktheme
+
+from medit.utils import fs_changes, impatient, setup_logging, watchdog
 
 CFG_FILE = "~/.medit.cfg"
 
 
 def log() -> logging.Logger:
     """Returns the local logger"""
     return logging.getLogger("medit.ui")
@@ -31,14 +33,15 @@
         return json.load(open(os.path.expanduser(filename)))
     return default
 
 
 class MEditWindow(QtWidgets.QMainWindow):
     """The one and only application window"""
 
+    @impatient
     def __init__(self, path: Path | None) -> None:
         super().__init__()
         uic.loadUi(Path(__file__).parent / "medit.ui", self)
         # self.setStyleSheet(styleSheet)
         # self.setStyleSheet("background-color: yellow;")
 
         # css =  open(Path(__file__).parent / "github-markdown-light.css").read()
@@ -60,19 +63,19 @@
             and (path if path.is_dir else path.parent)
             or Path(config.get("base_dir") or ".").absolute()
         )
         self.autoload_thread = QtCore.QThread(self)
         self.autoload_thread.run = lambda: self.async_stuff()
         self.autoload_thread.start()
 
-        #self.fs_watcher = QtCore.QFileSystemWatcher([self.base_dir.as_posix()])
-        #self.fs_watcher.fileChanged.connect(self.on_file_changed_externally)
-        #self.fs_watcher.directoryChanged.connect(self.on_file_changed_externally)
-        #self.fs_watcher.addPaths([self.base_dir.as_posix()])
-        #print(self.fs_watcher.files())
+        # self.fs_watcher = QtCore.QFileSystemWatcher([self.base_dir.as_posix()])
+        # self.fs_watcher.fileChanged.connect(self.on_file_changed_externally)
+        # self.fs_watcher.directoryChanged.connect(self.on_file_changed_externally)
+        # self.fs_watcher.addPaths([self.base_dir.as_posix()])
+        # print(self.fs_watcher.files())
 
         self.fs_model = QtGui.QFileSystemModel()
         self.fs_model.setRootPath(Path.home().as_posix())
 
         self.open_file = None
 
         self.set_open_file(path if path and path.is_file() else config.get("open_file"))
@@ -82,105 +85,114 @@
         self.tv_files.setModel(self.fs_model)
 
         self.tv_files.selectionModel().selectionChanged.connect(self.on_tv_files_selectionChanged)
 
         self.tv_files.hideColumn(1)
         self.tv_files.hideColumn(2)
         self.tv_files.hideColumn(3)
+        self.tv_files.setHeaderHidden(True)
+
         self.tv_files.setRootIndex(self.fs_model.index(self.base_dir.as_posix()))
         self.tv_files.expand(self.fs_model.index(self.base_dir.as_posix()))
         if self.open_file:
             self.tv_files.setCurrentIndex(self.fs_model.index(self.open_file.absolute().as_posix()))
         else:
             self.tv_files.setCurrentIndex(self.fs_model.index(self.base_dir.absolute().as_posix()))
 
         self.show()
 
     def async_stuff(self):
         print("Async")
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
-        #terminator = threading.Event()
+        # terminator = threading.Event()
 
         # https://stackoverflow.com/a/71956673
-        _tasks = {
-            asyncio.ensure_future(self.watch_fs_changes())
-        }
+        _tasks = {asyncio.ensure_future(self.watch_fs_changes())}
         loop.run_forever()
 
     @watchdog
     async def watch_fs_changes(self) -> None:
         """Observe changes to filesystem and mark walls dirty"""
         async for changed_path in fs_changes(self.base_dir, timeout=1, postpone=True):
             log().info("file %s changed", changed_path)
             QtCore.QMetaObject.invokeMethod(
-                self, "on_file_changed_externally", QtCore.Qt.QueuedConnection,
-                #QtCore.Q_ARG(list, [])
+                self,
+                "on_file_changed_externally",
+                QtCore.Qt.ConnectionType.QueuedConnection,
+                QtCore.Q_ARG(str, changed_path.as_posix()),
             )
 
-
     def reset_timer(self):
         logging.debug("reset modification timer")
         self.autosave_timer.start(300)
 
+    @impatient
     def render_content(self):
         self.wv_rendered.show(
             self.txt_editor.text(), self.open_file and self.open_file.suffix.strip("~")
         )
 
+    @impatient
     def on_autosave_timer_timeout(self):
         """"""
         self.autosave_timer.stop()
         self.render_content()
         self.save()
 
+    @impatient
     def save(self):
         # if not self.dirty:
         # return
         log().info("save to %s", self.open_file)
         # self.dirty = True
         text_to_save = self.txt_editor.text()
         if not text_to_save:
             log().warning("I don't dare to overwrite with empty content..")
             return
         open(self.open_file, "w").write(text_to_save)
 
+    @impatient
     def set_open_file(self, path):
         self.open_file = None
         block_state = self.txt_editor.blockSignals(True)
         selected_file = Path(path) if path else None
         if not path:
             return
         try:
             self.txt_editor.openFile(selected_file)
             self.open_file = selected_file
         except UnicodeDecodeError:
             self.txt_editor.setText("")
         finally:
             self.txt_editor.blockSignals(block_state)
             self.setWindowTitle(str(self.open_file))
+            QtWidgets.QApplication.instance().setApplicationName(f"medit - {self.open_file.name}")
+
         self.render_content()
 
-    def on_tv_files_selectionChanged(self, selection) -> None:
+    @impatient
+    def on_tv_files_selectionChanged(self, selection1, selection2) -> None:
         # print(Path(self.fs_model.filePath(selection.indexes()[0])))
         try:
-
-            selected_path = Path(self.fs_model.filePath(selection.indexes()[0]))
+            selected_path = Path(self.fs_model.filePath(selection1.indexes()[0]))
             if selected_path.is_file():
                 self.set_open_file(selected_path)
         except IndexError:
             print("FILE REMOVED?")
 
     def on_txt_editor_textChanged(self) -> None:
         self.reset_timer()
 
+    @impatient
     @QtCore.pyqtSlot(str)
-    def on_file_changed_externally(file) -> None:
+    def on_file_changed_externally(self, file) -> None:
         print(file)
 
+    @impatient
     def event(self, event: QtCore.QEvent) -> bool:
         # if event.type() == QtCore.QEvent.DragEnter:
         # if any(
         # Path(u.url()).suffix.lower() in {".pdf", ".epub"} for u in event.mimeData().urls()
         # ):
         # event.accept()
         # elif event.type() == QtCore.QEvent.Drop:
@@ -203,14 +215,15 @@
         # QtCore.QEvent.DragMove,
         # QtCore.QEvent.DragLeave,
         # }:
         ## log().warn("unknown event: %r %r", event.type(), event)
         # pass
         return super().event(event)
 
+    @impatient
     def closeEvent(self, _event: QtGui.QCloseEvent) -> None:
         """save state before shutting down"""
         logging.info("got some closish signal, bye")
         # self.autoload_thread.terminate()
         # self.autoload_thread.wait()
         # self.save()
         g = self.geometry()
```

### Comparing `medit-0.0.5/medit/utils.py` & `medit-0.0.6/medit/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """Stuff that doesn't go anywhere else
 """
 
 import asyncio
 import logging
 import os
+import time
 from collections.abc import AsyncIterator, Callable, Coroutine, Iterator
 from functools import wraps
 from pathlib import Path
 from typing import NoReturn, cast
 
 from asyncinotify import Event, Inotify, Mask
 
@@ -26,25 +27,38 @@
 
     @wraps(afunc)
     async def run(*args: object, **kwargs: object) -> object:
         """Run wrapped function and handle exceptions"""
         try:
             return await afunc(*args, **kwargs)
         except asyncio.CancelledError:
-            logger().info("Task cancelled: `%s`", afunc.__name__)
+            log().info("Task cancelled: `%s`", afunc.__name__)
         except KeyboardInterrupt:
-            logger().info("KeyboardInterrupt in `%s`", afunc.__name__)
+            log().info("KeyboardInterrupt in `%s`", afunc.__name__)
         except Exception:  # pylint: disable=broad-except
-            logger().exception("Exception in `%s`:", afunc.__name__)
+            log().exception("Exception in `%s`:", afunc.__name__)
             asyncio.get_event_loop().stop()
         return None
 
     return run
 
 
+def impatient(func):
+    @wraps(func)
+    def run(*args: object, **kwargs: object) -> object:
+        try:
+            t1 = time.time()
+            return func(*args, **kwargs)
+        finally:
+            if (duration := time.time() - t1) > 0.1:
+                log().warn("%s took %.2fs!", func.__name__, duration)
+
+    return run
+
+
 async def fs_changes(
     *paths: Path,
     queue: asyncio.Queue[str] = asyncio.Queue(),
     mask: Mask = Mask.CLOSE_WRITE
     | Mask.MOVED_TO
     | Mask.CREATE
     | Mask.MODIFY
```

### Comparing `medit-0.0.5/medit/yatl.py` & `medit-0.0.6/medit/yatl.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.5/pyproject.toml` & `medit-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "medit"
-version = "0.0.5"
+version = "0.0.6"
 description = "Markup Editor"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/medit.git"
 readme = "Readme.md"
 packages = [
   {include = "medit/**/*.py"},
   {include = "medit/**/*.ui"},
```

### Comparing `medit-0.0.5/PKG-INFO` & `medit-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medit
-Version: 0.0.5
+Version: 0.0.6
 Summary: Markup Editor
 Home-page: https://projects.om-office.de/frans/medit.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -18,26 +18,41 @@
 Requires-Dist: pyqt6-qscintilla (>=2.14.0,<3.0.0)
 Requires-Dist: pyqt6-webengine (>=6.5.0,<7.0.0)
 Requires-Dist: pyqtdarktheme (>=2.1.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://projects.om-office.de/frans/medit.git
 Description-Content-Type: text/markdown
 
-# MEdit - Markup Editor
+# MEdit - Previewing [M]arkup [Editor]
+
+A simple text editor based on PyQt6/QScintilla with the following goals in mind:
+
+- Auto-saves and tracks filesystem in order to make loading/saving obsolete
+- Syntax highlighting for typical file formats
+- Previewing markdown or representations in other file formats
+- Support for local and remote images in Markdown/reST
+- Decent nice looking interface for easily distractable people like me
+
+As almost all of my projects, `medit` is in dangerous alpha state - use it with
+care and don't believe anything written here.
 
 
 ## Installation
 
 ```sh
 [<PYTHON> -m] pip[3] install [--upgrade] medit
 ```
 
 
 ## Usage
 
+```sh
+medit [<PATH>]  # will open medit in given directory or on given file
+```
+
 
 ## Development & Contribution
 
 ```sh
 pip3 install -U poetry pre-commit
 git clone --recurse-submodules https://projects.om-office.de/frans/pocketrockit.git
 cd pocketrockit
@@ -47,55 +62,59 @@
 poetry install
 ```
 
 After modifications, this way a newly built wheel can be checked and installed:
 
 ```sh
 poetry build
-poetry run twine check dist/pocketrockit-0.0.25-py3-none-any.whl
-python3 -m pip install --user --upgrade dist/pocketrockit-0.0.25-py3-none-any.whl
+poetry run twine check dist/medit-0.0.5-py3-none-any.whl
+python3 -m pip install --user --upgrade dist/medit-0.0.5-py3-none-any.whl
 ```
 
-## 1.0 TODO
+## My personal MLP (v1.0) goals
 
 * [x] File to title
 * [x] File viewer for Plain, Python, YAML, JSON, ..
 * [x] Autosave
+* [x] Manage word wrap in editor
 * [ ] Autoload
+* [ ] Multi-File Undo/Redo
 * [ ] Change into / step up current directory
 * [ ] Zen mode
 * [ ] Recent files
 * [ ] Search/open files
 * [ ] Search in files
-* [ ] Preview for Markdown/.. only
-* [ ] Manage word wrap in editor
+* [ ] Preview for previewable only
 * [ ] Hightlight todo.txt
 * [ ] Notify external file changes
 * [ ] (Re-)store zoom and fullscreen
 * [ ] File ignore filter
-* [ ] Icon
+* [ ] Icon / .desktop file
 * [ ] Proper Qt style
 * [ ] Show local images
 * [ ] Show remote images
 * [ ] Slim file / folder create / rename
 * [ ] Proper View CSS selector
 * [ ] View follows editor
 * [ ] Links clickable
 * [ ] Fix Links to support `(text)[url]` syntax
 
 
 ## Feature ideas
 
-* [ ] Export to Pdf / Html / docx ..
+* [ ] Export to Pdf / Html / Docx ..
 * [ ] Copy / paste images
 * [ ] Drag & drop images
 * [ ] Spell checker
+* [ ] Script console with preview
+* [ ] Preview rules (markdown->HTML, xml/json/yaml -> xml/json/yaml ..)
 
 
 ## Read
+
 * https://web.archive.org/web/20190604145031/https://qscintilla.com/prepare-image-hack/
 
 * https://github.com/sindresorhus/github-markdown-css
 * https://python-markdown.github.io/extensions/code_hilite/#step-1-download-and-install-pygments
 * https://github.com/richleland/pygments-css
 * https://github.com/OzakIOne/markdown-github-dark
 * https://github.com/jamiemcg/remarkable
```

