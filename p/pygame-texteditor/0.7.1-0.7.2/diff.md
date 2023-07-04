# Comparing `tmp/pygame_texteditor-0.7.1.tar.gz` & `tmp/pygame_texteditor-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_texteditor-0.7.1.tar", max compression
+gzip compressed data, was "pygame_texteditor-0.7.2.tar", max compression
```

## Comparing `pygame_texteditor-0.7.1.tar` & `pygame_texteditor-0.7.2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1092 2023-04-20 09:30:36.501202 pygame_texteditor-0.7.1/LICENSE
--rw-r--r--   0        0        0     1539 2023-04-20 09:58:02.905719 pygame_texteditor-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6933 2023-04-20 09:55:36.909461 pygame_texteditor-0.7.1/README.md
--rw-r--r--   0        0        0       36 2023-04-20 09:30:36.506702 pygame_texteditor-0.7.1/src/pygame_texteditor/__init__.py
--rw-r--r--   0        0        0     3924 2023-04-20 09:30:36.507705 pygame_texteditor-0.7.1/src/pygame_texteditor/_caret.py
--rw-r--r--   0        0        0     5444 2023-04-20 09:57:05.199680 pygame_texteditor-0.7.1/src/pygame_texteditor/_customization.py
--rw-r--r--   0        0        0     1783 2023-04-20 09:30:36.509810 pygame_texteditor-0.7.1/src/pygame_texteditor/_editor_getters.py
--rw-r--r--   0        0        0    17455 2023-04-20 09:30:36.511139 pygame_texteditor-0.7.1/src/pygame_texteditor/_input_handling_keyboard.py
--rw-r--r--   0        0        0     9639 2023-04-20 09:30:36.512448 pygame_texteditor-0.7.1/src/pygame_texteditor/_input_handling_keyboard_highlight.py
--rw-r--r--   0        0        0     8518 2023-04-20 09:30:36.513236 pygame_texteditor-0.7.1/src/pygame_texteditor/_input_handling_mouse.py
--rw-r--r--   0        0        0     1428 2023-04-20 09:30:36.513738 pygame_texteditor-0.7.1/src/pygame_texteditor/_letter_operations.py
--rw-r--r--   0        0        0     1503 2023-04-20 09:30:36.514737 pygame_texteditor-0.7.1/src/pygame_texteditor/_other.py
--rw-r--r--   0        0        0     8041 2023-04-20 09:30:36.515239 pygame_texteditor-0.7.1/src/pygame_texteditor/_rendering.py
--rw-r--r--   0        0        0     5117 2023-04-20 09:30:36.516239 pygame_texteditor-0.7.1/src/pygame_texteditor/_rendering_highlighting.py
--rw-r--r--   0        0        0     1072 2023-04-20 09:30:36.517237 pygame_texteditor-0.7.1/src/pygame_texteditor/_rendering_syntax_coloring.py
--rw-r--r--   0        0        0     1852 2023-04-20 09:30:36.518237 pygame_texteditor-0.7.1/src/pygame_texteditor/_scrollbar_vertical.py
--rw-r--r--   0        0        0     2094 2023-04-20 09:30:36.518741 pygame_texteditor-0.7.1/src/pygame_texteditor/_usage.py
--rw-r--r--   0        0        0     3428 2023-04-20 09:30:36.505702 pygame_texteditor-0.7.1/src/pygame_texteditor/ColorFormatter.py
--rw-r--r--   0        0        0      468 2023-04-20 09:30:36.519971 pygame_texteditor-0.7.1/src/pygame_texteditor/elements/colorstyles/bright.yml
--rw-r--r--   0        0        0      469 2023-04-20 09:30:36.519971 pygame_texteditor-0.7.1/src/pygame_texteditor/elements/colorstyles/dark.yml
--rw-r--r--   0        0        0    59516 2023-04-20 09:30:36.520986 pygame_texteditor-0.7.1/src/pygame_texteditor/elements/fonts/Courier.ttf
--rw-r--r--   0        0        0      211 2023-04-20 09:30:36.521992 pygame_texteditor-0.7.1/src/pygame_texteditor/elements/graphics/Scroll_Bar.png
--rw-r--r--   0        0        0    10313 2023-04-20 09:49:10.509400 pygame_texteditor-0.7.1/src/pygame_texteditor/TextEditor.py
--rw-r--r--   0        0        0     7843 1970-01-01 00:00:00.000000 pygame_texteditor-0.7.1/setup.py
--rw-r--r--   0        0        0     7875 1970-01-01 00:00:00.000000 pygame_texteditor-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-21 05:19:33.913074 pygame_texteditor-0.7.2/LICENSE
+-rw-r--r--   0        0        0     1541 2023-07-04 06:29:34.882202 pygame_texteditor-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6933 2023-04-21 05:19:33.919070 pygame_texteditor-0.7.2/README.md
+-rw-r--r--   0        0        0       36 2023-04-21 05:19:33.950069 pygame_texteditor-0.7.2/src/pygame_texteditor/__init__.py
+-rw-r--r--   0        0        0     3924 2023-04-21 05:19:33.955070 pygame_texteditor-0.7.2/src/pygame_texteditor/_caret.py
+-rw-r--r--   0        0        0     5444 2023-04-21 05:19:33.961071 pygame_texteditor-0.7.2/src/pygame_texteditor/_customization.py
+-rw-r--r--   0        0        0     1783 2023-04-21 05:19:33.966070 pygame_texteditor-0.7.2/src/pygame_texteditor/_editor_getters.py
+-rw-r--r--   0        0        0    17455 2023-04-21 05:19:33.970069 pygame_texteditor-0.7.2/src/pygame_texteditor/_input_handling_keyboard.py
+-rw-r--r--   0        0        0     9639 2023-04-21 05:19:33.976071 pygame_texteditor-0.7.2/src/pygame_texteditor/_input_handling_keyboard_highlight.py
+-rw-r--r--   0        0        0     8518 2023-04-21 05:19:33.981071 pygame_texteditor-0.7.2/src/pygame_texteditor/_input_handling_mouse.py
+-rw-r--r--   0        0        0     1428 2023-04-21 05:19:33.985071 pygame_texteditor-0.7.2/src/pygame_texteditor/_letter_operations.py
+-rw-r--r--   0        0        0     1503 2023-04-21 05:19:33.989069 pygame_texteditor-0.7.2/src/pygame_texteditor/_other.py
+-rw-r--r--   0        0        0     8041 2023-04-21 05:19:33.995071 pygame_texteditor-0.7.2/src/pygame_texteditor/_rendering.py
+-rw-r--r--   0        0        0     5117 2023-04-21 05:19:34.000069 pygame_texteditor-0.7.2/src/pygame_texteditor/_rendering_highlighting.py
+-rw-r--r--   0        0        0     1072 2023-04-21 05:19:34.005071 pygame_texteditor-0.7.2/src/pygame_texteditor/_rendering_syntax_coloring.py
+-rw-r--r--   0        0        0     1852 2023-04-21 05:19:34.011074 pygame_texteditor-0.7.2/src/pygame_texteditor/_scrollbar_vertical.py
+-rw-r--r--   0        0        0     2094 2023-04-21 05:19:34.016074 pygame_texteditor-0.7.2/src/pygame_texteditor/_usage.py
+-rw-r--r--   0        0        0     3428 2023-04-21 05:19:33.945073 pygame_texteditor-0.7.2/src/pygame_texteditor/ColorFormatter.py
+-rw-r--r--   0        0        0      468 2023-04-21 05:19:34.017073 pygame_texteditor-0.7.2/src/pygame_texteditor/elements/colorstyles/bright.yml
+-rw-r--r--   0        0        0      469 2023-04-21 05:19:34.017073 pygame_texteditor-0.7.2/src/pygame_texteditor/elements/colorstyles/dark.yml
+-rw-r--r--   0        0        0    59516 2023-04-21 05:19:34.018073 pygame_texteditor-0.7.2/src/pygame_texteditor/elements/fonts/Courier.ttf
+-rw-r--r--   0        0        0      211 2023-04-21 05:19:34.019070 pygame_texteditor-0.7.2/src/pygame_texteditor/elements/graphics/Scroll_Bar.png
+-rw-r--r--   0        0        0    10327 2023-07-04 06:29:01.697222 pygame_texteditor-0.7.2/src/pygame_texteditor/TextEditor.py
+-rw-r--r--   0        0        0     7875 1970-01-01 00:00:00.000000 pygame_texteditor-0.7.2/PKG-INFO
```

### Comparing `pygame_texteditor-0.7.1/LICENSE` & `pygame_texteditor-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/pyproject.toml` & `pygame_texteditor-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygame-texteditor"
-version = "0.7.1"
+version = "0.7.2"
 description = "A WYSIWYG-texteditor based on pygame."
 authors = ["Victor Seifert <seifert.victor@web.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pygame_texteditor", from="src"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -17,20 +17,20 @@
     "Natural Language :: English",
     "Topic :: Software Development",
 ]
 keywords=[
     "pygame",
     "texteditor",
     "text",
-    "editor"
+    "editor",
 ]
 include = [
     "src/pygame_texteditor/elements/graphics/*.png",
     "src/pygame_texteditor/elements/fonts/.ttf",
-    "src/pygame_texteditor/elements/colorstyles/*.yml"
+    "src/pygame_texteditor/elements/colorstyles/*.yml",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pygame = ">=1.9.6"
 PyYAML = ">=5.3.1"
```

### Comparing `pygame_texteditor-0.7.1/README.md` & `pygame_texteditor-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_caret.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_caret.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_customization.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_customization.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_editor_getters.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_editor_getters.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_input_handling_keyboard.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_input_handling_keyboard.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_input_handling_keyboard_highlight.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_input_handling_keyboard_highlight.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_input_handling_mouse.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_input_handling_mouse.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_letter_operations.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_letter_operations.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_other.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_other.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_rendering.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_rendering.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_rendering_highlighting.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_rendering_highlighting.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_rendering_syntax_coloring.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_rendering_syntax_coloring.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_scrollbar_vertical.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_scrollbar_vertical.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/_usage.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/_usage.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/ColorFormatter.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/ColorFormatter.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/elements/fonts/Courier.ttf` & `pygame_texteditor-0.7.2/src/pygame_texteditor/elements/fonts/Courier.ttf`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.1/src/pygame_texteditor/TextEditor.py` & `pygame_texteditor-0.7.2/src/pygame_texteditor/TextEditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         self.color_scrollbar = (60, 61, 61)
         self.color_scrollbar_background = (49, 50, 50)
         self.color_line_number_font = (255, 255, 255)
         self.color_line_number_background = (60, 61, 61)
         self.color_text = (255, 255, 255)
         self.color_caret = (255, 255, 255)
 
-        self.lexer = PythonLexer()
+        self.lexer = PythonLexer(ensurenl=False)
         self.color_formatter = ColorFormatter()
         self.set_colorscheme(style)
 
         # Key input variables+
         self.key_initial_delay = 300
         self.key_continued_interval = 30
         pygame.key.set_repeat(self.key_initial_delay, self.key_continued_interval)
```

### Comparing `pygame_texteditor-0.7.1/setup.py` & `pygame_texteditor-0.7.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,215 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pygame-texteditor
+Version: 0.7.2
+Summary: A WYSIWYG-texteditor based on pygame.
+License: MIT
+Keywords: pygame,texteditor,text,editor
+Author: Victor Seifert
+Author-email: seifert.victor@web.de
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: PyYAML (>=5.3.1)
+Requires-Dist: Pygments (>=2.6.1)
+Requires-Dist: pygame (>=1.9.6)
+Requires-Dist: pyperclip (>=1.8.1)
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# A WYSIWYG-texteditor based on pygame for pygame
 
-packages = \
-['pygame_texteditor']
+![PyPI](https://img.shields.io/pypi/v/pygame-texteditor?color=%233775A9&label=pypi%20package&style=plastic)
+![GitHub](https://img.shields.io/github/license/CribberSix/pygame-texteditor?style=plastic)
 
-package_data = \
-{'': ['*'],
- 'pygame_texteditor': ['elements/colorstyles/*',
-                       'elements/fonts/*',
-                       'elements/graphics/*']}
-
-install_requires = \
-['PyYAML>=5.3.1', 'Pygments>=2.6.1', 'pygame>=1.9.6', 'pyperclip>=1.8.1']
-
-setup_kwargs = {
-    'name': 'pygame-texteditor',
-    'version': '0.7.1',
-    'description': 'A WYSIWYG-texteditor based on pygame.',
-    'long_description': '# A WYSIWYG-texteditor based on pygame for pygame\n\n![PyPI](https://img.shields.io/pypi/v/pygame-texteditor?color=%233775A9&label=pypi%20package&style=plastic)\n![GitHub](https://img.shields.io/github/license/CribberSix/pygame-texteditor?style=plastic)\n\n## Introduction & examples\n\nThe text editor can be inserted into any existing pygame window.\nA minimal code example of it being activated within an existing pygame window can be found below.\n\nThe code editor comes with line numbers and syntax highlighting for python if enabled:\n\n![](./resources/example_one.png)\n\nExample with default configuration:\n\n![](./resources/example_two.png)\n\n## Usage\n\nThe texteditor takes 5 obligatory parameters and 4 optional parameters.\n\n##### Obligatory parameters\n- ```offset_X``` : integer - the offset from the left border of the pygame screen\n- ```offset_y``` : integer - the offset from the top border of the pygame screen\n- ```editor_width``` : integer - the width of texteditor\n- ```editor_height``` : integer - the height of texteditor\n- ```screen``` : pygame display surface - on which the texteditor is to be displayed\n\n##### Optional Parameters with default values\n\n- ```display_line_numbers``` - a boolean enabling showing line numbers\n    > Default: ```False```\n- ```style``` - a String setting the color scheme of editor and syntax highlighting\n    > Default: ```\'dark\'```\n- ```syntax_highlighting_python``` - a boolean enabling syntax highlighting for Python code\n    > Default: ```False```\n- ```font_size``` - an integer to set for the font size.\n    > Default: ```16```\n\n## Setup and configuration\n\n##### Minimal texteditor setup example\n\n```python\nimport pygame\nfrom pygame_texteditor import TextEditor\n\n# minimal pygame setup\npygame.init()\nscreen = pygame.display.set_mode((500, 600))\npygame.display.set_caption("Pygame")\npygame.display.get_surface().fill((200, 200, 200))  # background coloring\n\n# Instantiation & customization of the text editor\nTX = TextEditor(\n    offset_x=50, offset_y=50, editor_width=500, editor_height=400, screen=pygame.display.get_surface()\n)\nTX.set_line_numbers(True)\nTX.set_syntax_highlighting(True)\nTX.set_font_size(18)\n\n# TextEditor in the pygame-loop\nwhile True:\n    # INPUT - Mouse + Keyboard\n    pygame_events = pygame.event.get()\n    pressed_keys = pygame.key.get_pressed()\n    mouse_x, mouse_y = pygame.mouse.get_pos()\n    mouse_pressed = pygame.mouse.get_pressed()\n\n    # displays editor functionality once per loop\n    TX.display_editor(pygame_events, pressed_keys, mouse_x, mouse_y, mouse_pressed)\n    pygame.display.flip()  # updates pygame window\n\n```\n\n##### Retrieving text from the editor\n\nThe editor offers the function `get_text_as_string()` to retrieve the entire text\nas a String from the editor. Lines are separated by the new line character ```\\n```.\n\nThe editor offers the function `get_text_as_list()` to retrieve the entire text as a list from the editor.\nEach String-item in the list represents one line from the editor.\n\n##### Removing text from the editor\n\nThe editor offers the function `clear_text()` to clear the editor of any text.\n\n##### Inserting text into the editor\n\nInserting text can be done by using one of the two available functions:\n1. With a list of strings in which each string represents one line, or\n2. With a string which includes linebreak characters which get parsed.\n\n```\nset_text_from_list(["First line", "Second Line.", "Third Line."]\nset_text_from_string("First line.\\nSecond line.\\nThird Line")\n```\n\n## Customization\n\n#### Cursor mode\n\nCursor mode can either be `static` or `blinking` (=default).\n\n```python\nTX = TextEditor(...)\nTX.set_cursor_mode("static")\nTX.set_cursor_mode("blinking")\n```\n\n#### Key repetition speeds\n\nWhile a key is being held, multiple key events are being triggered.\nThe delay of the first repetition as well as the interval between all sequential key triggers can be\ncustomized by using the function `set_key_repetition(delay=300, intervall=30)`.\n\nFrom the [official documentation](http://www.pygame.org/docs/ref/key.html#pygame.key.set_repeat):\n> The delay parameter is the number of milliseconds before the first repeated pygame.KEYDOWN event will be sent.\n> After that, another pygame.KEYDOWN event will be sent every interval milliseconds.\n\n\n#### Font Customization\n\nThe editor uses a ttf file to set the font for the editor. By default, the Courier monospace font is used.\n\nA custom font can be loaded with the following method, passing an *absolute* path:\n- `set_font_from_ttf("X:\\path\\to\\custom\\font.ttf")`\n\nDISCLAIMER: As the width of a letter (space) is only calculated once after setting the font_size, any fonts that are not monospace will lead to the editor not working correctly anymore, as it cannot be determined correctly between which letters the user clicked.\n\n#### Font size\n\nFont size can be customized with the command `set_font_size(size)` - the parameter is an integer\nwith the default value `16` to be able to reset it.\n\n#### Line Numbers\nLine numbers can be shown on the left side of the editor. Line numbers begin with 0 as is the Pythonian way.\n\nLine numbers can be enabled and disabled with ```set_line_numbers(Boolean)```.\n\n\n#### Syntax Highlighting\n\nThe editor comes with syntax highlighting for Python code. Tokenization is based on the ```pygment``` package.\n\nSyntax highlighting can be enabled/disabled with ```set_syntax_coloring(boolean_value)```.\n\nThe syntax colors being used are also specified in the yml style file.\n\n\n#### Color-scheme customization\n\nThe editor uses a yml file to set the color-scheme for the editor itself and for the syntax coloring.\n\nTwo styles are delivered with the editor, they can be activated respectively by:\n- `set_colorscheme("dark")`\n- `set_colorscheme("bright")`\n\nA custom style can be loaded with the following method from a created yml file:\n- `set_colorscheme_from_yaml("X:\\path\\to\\custom\\filename.yml")`\n\nAll keys must be present with values. Acceptable values are\nRGB colors in the following format: ```(255, 255, 255)``` or ```255, 255, 255```.\n\nThe following keys are required in the ```stylename.yml``` file, syntax colors are only used if syntax\nhighlighting is enabled, but are still required to be included.\n\n**Editor colors** (source: bright.yml)\n\n- `codingBackgroundColor: (255, 255, 255)`\n- `codingScrollBarBackgroundColor: (49, 50, 50)`\n- `lineNumberColor: (255, 255, 255)`\n- `lineNumberBackgroundColor: (60, 61, 61)`\n- `textColor: (255, 255, 255)`\n\n** Syntax colors** (source: bright.yml)\n\n- `textColor_normal: (0, 255, 255)`\n- `textColor_comments: (119, 115, 115)`\n- `textColor_quotes: (227, 215, 115)`\n- `textColor_operators: (237, 36, 36)`\n- `textColor_keywords: (237, 36, 36)`\n- `textColor_function: (50, 150, 36)`\n- `textColor_builtin: (50, 50, 136)`\n',
-    'author': 'Victor Seifert',
-    'author_email': 'seifert.victor@web.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+## Introduction & examples
 
+The text editor can be inserted into any existing pygame window.
+A minimal code example of it being activated within an existing pygame window can be found below.
+
+The code editor comes with line numbers and syntax highlighting for python if enabled:
+
+![](./resources/example_one.png)
+
+Example with default configuration:
+
+![](./resources/example_two.png)
+
+## Usage
+
+The texteditor takes 5 obligatory parameters and 4 optional parameters.
+
+##### Obligatory parameters
+- ```offset_X``` : integer - the offset from the left border of the pygame screen
+- ```offset_y``` : integer - the offset from the top border of the pygame screen
+- ```editor_width``` : integer - the width of texteditor
+- ```editor_height``` : integer - the height of texteditor
+- ```screen``` : pygame display surface - on which the texteditor is to be displayed
+
+##### Optional Parameters with default values
+
+- ```display_line_numbers``` - a boolean enabling showing line numbers
+    > Default: ```False```
+- ```style``` - a String setting the color scheme of editor and syntax highlighting
+    > Default: ```'dark'```
+- ```syntax_highlighting_python``` - a boolean enabling syntax highlighting for Python code
+    > Default: ```False```
+- ```font_size``` - an integer to set for the font size.
+    > Default: ```16```
+
+## Setup and configuration
+
+##### Minimal texteditor setup example
+
+```python
+import pygame
+from pygame_texteditor import TextEditor
+
+# minimal pygame setup
+pygame.init()
+screen = pygame.display.set_mode((500, 600))
+pygame.display.set_caption("Pygame")
+pygame.display.get_surface().fill((200, 200, 200))  # background coloring
+
+# Instantiation & customization of the text editor
+TX = TextEditor(
+    offset_x=50, offset_y=50, editor_width=500, editor_height=400, screen=pygame.display.get_surface()
+)
+TX.set_line_numbers(True)
+TX.set_syntax_highlighting(True)
+TX.set_font_size(18)
+
+# TextEditor in the pygame-loop
+while True:
+    # INPUT - Mouse + Keyboard
+    pygame_events = pygame.event.get()
+    pressed_keys = pygame.key.get_pressed()
+    mouse_x, mouse_y = pygame.mouse.get_pos()
+    mouse_pressed = pygame.mouse.get_pressed()
+
+    # displays editor functionality once per loop
+    TX.display_editor(pygame_events, pressed_keys, mouse_x, mouse_y, mouse_pressed)
+    pygame.display.flip()  # updates pygame window
+
+```
+
+##### Retrieving text from the editor
+
+The editor offers the function `get_text_as_string()` to retrieve the entire text
+as a String from the editor. Lines are separated by the new line character ```\n```.
+
+The editor offers the function `get_text_as_list()` to retrieve the entire text as a list from the editor.
+Each String-item in the list represents one line from the editor.
+
+##### Removing text from the editor
+
+The editor offers the function `clear_text()` to clear the editor of any text.
+
+##### Inserting text into the editor
+
+Inserting text can be done by using one of the two available functions:
+1. With a list of strings in which each string represents one line, or
+2. With a string which includes linebreak characters which get parsed.
+
+```
+set_text_from_list(["First line", "Second Line.", "Third Line."]
+set_text_from_string("First line.\nSecond line.\nThird Line")
+```
+
+## Customization
+
+#### Cursor mode
+
+Cursor mode can either be `static` or `blinking` (=default).
+
+```python
+TX = TextEditor(...)
+TX.set_cursor_mode("static")
+TX.set_cursor_mode("blinking")
+```
+
+#### Key repetition speeds
+
+While a key is being held, multiple key events are being triggered.
+The delay of the first repetition as well as the interval between all sequential key triggers can be
+customized by using the function `set_key_repetition(delay=300, intervall=30)`.
+
+From the [official documentation](http://www.pygame.org/docs/ref/key.html#pygame.key.set_repeat):
+> The delay parameter is the number of milliseconds before the first repeated pygame.KEYDOWN event will be sent.
+> After that, another pygame.KEYDOWN event will be sent every interval milliseconds.
+
+
+#### Font Customization
+
+The editor uses a ttf file to set the font for the editor. By default, the Courier monospace font is used.
+
+A custom font can be loaded with the following method, passing an *absolute* path:
+- `set_font_from_ttf("X:\path\to\custom\font.ttf")`
+
+DISCLAIMER: As the width of a letter (space) is only calculated once after setting the font_size, any fonts that are not monospace will lead to the editor not working correctly anymore, as it cannot be determined correctly between which letters the user clicked.
+
+#### Font size
+
+Font size can be customized with the command `set_font_size(size)` - the parameter is an integer
+with the default value `16` to be able to reset it.
+
+#### Line Numbers
+Line numbers can be shown on the left side of the editor. Line numbers begin with 0 as is the Pythonian way.
+
+Line numbers can be enabled and disabled with ```set_line_numbers(Boolean)```.
+
+
+#### Syntax Highlighting
+
+The editor comes with syntax highlighting for Python code. Tokenization is based on the ```pygment``` package.
+
+Syntax highlighting can be enabled/disabled with ```set_syntax_coloring(boolean_value)```.
+
+The syntax colors being used are also specified in the yml style file.
+
+
+#### Color-scheme customization
+
+The editor uses a yml file to set the color-scheme for the editor itself and for the syntax coloring.
+
+Two styles are delivered with the editor, they can be activated respectively by:
+- `set_colorscheme("dark")`
+- `set_colorscheme("bright")`
+
+A custom style can be loaded with the following method from a created yml file:
+- `set_colorscheme_from_yaml("X:\path\to\custom\filename.yml")`
+
+All keys must be present with values. Acceptable values are
+RGB colors in the following format: ```(255, 255, 255)``` or ```255, 255, 255```.
+
+The following keys are required in the ```stylename.yml``` file, syntax colors are only used if syntax
+highlighting is enabled, but are still required to be included.
+
+**Editor colors** (source: bright.yml)
+
+- `codingBackgroundColor: (255, 255, 255)`
+- `codingScrollBarBackgroundColor: (49, 50, 50)`
+- `lineNumberColor: (255, 255, 255)`
+- `lineNumberBackgroundColor: (60, 61, 61)`
+- `textColor: (255, 255, 255)`
+
+** Syntax colors** (source: bright.yml)
+
+- `textColor_normal: (0, 255, 255)`
+- `textColor_comments: (119, 115, 115)`
+- `textColor_quotes: (227, 215, 115)`
+- `textColor_operators: (237, 36, 36)`
+- `textColor_keywords: (237, 36, 36)`
+- `textColor_function: (50, 150, 36)`
+- `textColor_builtin: (50, 50, 136)`
 
-setup(**setup_kwargs)
```

