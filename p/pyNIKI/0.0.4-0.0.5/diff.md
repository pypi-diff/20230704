# Comparing `tmp/pyniki-0.0.4.tar.gz` & `tmp/pyniki-0.0.5.tar.gz`

## Comparing `pyniki-0.0.4.tar` & `pyniki-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyniki-0.0.4/src/pyniki/__init__.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 pyniki-0.0.4/src/pyniki/curses.py
--rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 pyniki-0.0.4/src/pyniki/field.py
--rw-r--r--   0        0        0    15402 2020-02-02 00:00:00.000000 pyniki-0.0.4/src/pyniki/main.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pyniki-0.0.4/src/pyniki/sim.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pyniki-0.0.4/src/pyniki/ui.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyniki-0.0.4/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 pyniki-0.0.4/LICENSE
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyniki-0.0.4/README.md
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 pyniki-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    21613 2020-02-02 00:00:00.000000 pyniki-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyniki-0.0.5/src/pyniki/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pyniki-0.0.5/src/pyniki/curses.py
+-rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 pyniki-0.0.5/src/pyniki/field.py
+-rw-r--r--   0        0        0    15459 2020-02-02 00:00:00.000000 pyniki-0.0.5/src/pyniki/main.py
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 pyniki-0.0.5/src/pyniki/sim.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pyniki-0.0.5/src/pyniki/ui.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyniki-0.0.5/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 pyniki-0.0.5/LICENSE
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyniki-0.0.5/README.md
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 pyniki-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    21613 2020-02-02 00:00:00.000000 pyniki-0.0.5/PKG-INFO
```

### Comparing `pyniki-0.0.4/src/pyniki/curses.py` & `pyniki-0.0.5/src/pyniki/curses.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 import curses
+import sys
 from contextlib import contextmanager
 
 _curs_state = None
 _scr = None
 
+
+class SizeError(Exception):
+    pass
+
+
 def setup():
     global _scr
     global _curs_state
     _scr = curses.initscr()
-
     _curs_state = curses.curs_set(0)
+
+    y, x = _scr.getmaxyx()
+    if y < 25 or x < 80:
+        raise SizeError
+
     curses.noecho()
     curses.cbreak()
-    curses.set_escdelay(1)
+    try:
+        curses.set_escdelay(1)
+    except AttributeError:
+        pass
     _scr.keypad(True)
     _scr.clear()
 
 
 def teardown():
     curses.nocbreak()
     _scr.keypad(False)
@@ -30,15 +43,21 @@
         return getattr(_scr, name)
 
 scr = ScrWrapper()
 
 
 @contextmanager
 def curses_setup():
-    setup()
+    try:
+        setup()
+    except SizeError:
+        teardown()
+        print('Terminalfenster zu klein!')
+        sys.exit(1)
+
     try:
         yield
     finally:
         teardown()
 
 
 @contextmanager
```

### Comparing `pyniki-0.0.4/src/pyniki/field.py` & `pyniki-0.0.5/src/pyniki/field.py`

 * *Files identical despite different names*

### Comparing `pyniki-0.0.4/src/pyniki/main.py` & `pyniki-0.0.5/src/pyniki/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,14 +168,17 @@
     def draw(self):
         draw_frame(9, 80, self.y, 0)
         for row in self.word_array:
             for w in row:
                 w.draw()
 
     def run(self):
+        if not self.word_array:
+            return None
+
         self.set_selected(0, 0)
 
         while True:
             key = scr.getch()
             if key == curses.KEY_RIGHT:
                 if self.sx + 1 < len(self.path_array[self.sy]):
                     self.set_selected(self.sy, self.sx+1)
```

### Comparing `pyniki-0.0.4/src/pyniki/sim.py` & `pyniki-0.0.5/src/pyniki/sim.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,23 +42,22 @@
     scr.nodelay(False)
     if speed > 0:
         time.sleep(0.1 + (9-speed)*0.2)
 
 
 def is_free(direction):
     y, x = _field.pos
-    match direction:
-        case 0:
-            return not _field.v_walls[y][x+1]
-        case 1:
-            return not _field.h_walls[y+1][x]
-        case 2:
-            return not _field.v_walls[y][x]
-        case 3:
-            return not _field.h_walls[y][x]
+    if direction == 0:
+        return not _field.v_walls[y][x+1]
+    elif direction == 1:
+        return not _field.h_walls[y+1][x]
+    elif direction == 2:
+        return not _field.v_walls[y][x]
+    else:
+        return not _field.h_walls[y][x]
 
 
 def vorne_frei():
     return is_free(_field.direction)
 
 
 def links_frei():
@@ -101,23 +100,22 @@
     wait()
 
 
 def vor():
     if not vorne_frei():
         raise NikiError()
     y, x = _field.pos
-    match _field.direction:
-        case 0:
-            _field.pos = [y, x+1]
-        case 1:
-            _field.pos = [y+1, x]
-        case 2:
-            _field.pos = [y, x-1]
-        case 3:
-            _field.pos = [y-1, x]
+    if _field.direction == 0:
+        _field.pos = [y, x+1]
+    elif _field.direction == 1:
+        _field.pos = [y+1, x]
+    elif _field.direction == 2:
+        _field.pos = [y, x-1]
+    else:
+        _field.pos = [y-1, x]
     wait()
 
 
 def drehe_links():
     _field.direction = (_field.direction + 1) % 4
     wait()
 
@@ -171,15 +169,21 @@
                                 'links_frei', 'rechts_frei', 'hat_vorrat', 'platz_belegt']})
     except KeyboardInterrupt:
         pass
     except NikiError:
         error = True
     except NameError as e:
         line = traceback.extract_tb(sys.exc_info()[2])[-1].lineno
-        print_first_line(f'@FEHLER!@ Unbekannter Name "{e.name}" in Zeile {line}')
+        try:
+            name = e.name
+        except AttributeError:  # Python < 3.10
+            # from https://stackoverflow.com/a/44731654
+            import re
+            name = re.search("'(?P<name>.+?)'", e.args[0]).group('name')
+        print_first_line(f'@FEHLER!@ Unbekannter Name "{name}" in Zeile {line}')
         error = True
     if error:
         _field.zustand = False
         _field.draw()
         print_last_line(
             'Niki hat sich abgeschaltet                                  <Leertaste drücken>'
         )
```

### Comparing `pyniki-0.0.4/src/pyniki/ui.py` & `pyniki-0.0.5/src/pyniki/ui.py`

 * *Files identical despite different names*

### Comparing `pyniki-0.0.4/LICENSE` & `pyniki-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyniki-0.0.4/pyproject.toml` & `pyniki-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyNIKI"
-version = "0.0.4"
+version = "0.0.5"
 description = "Classic Niki the robot in Python"
 readme = "README.md"
 license.file = "LICENSE"
 requires-python = ">=3.8"
 authors = [
     { name = "Stephan Rave", email = "stephan.rave@uni-muenster.de" },
 ]
```

### Comparing `pyniki-0.0.4/PKG-INFO` & `pyniki-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNIKI
-Version: 0.0.4
+Version: 0.0.5
 Summary: Classic Niki the robot in Python
 Project-URL: Homepage, https://github.com/sdrave/pyniki
 Author-email: Stephan Rave <stephan.rave@uni-muenster.de>
 Maintainer-email: Stephan Rave <stephan.rave@uni-muenster.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
```

