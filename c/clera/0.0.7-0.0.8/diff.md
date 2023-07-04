# Comparing `tmp/clera-0.0.7.tar.gz` & `tmp/clera-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clera-0.0.7.tar", last modified: Tue Apr 25 05:45:24 2023, max compression
+gzip compressed data, was "clera-0.0.8.tar", last modified: Tue Jul  4 00:45:44 2023, max compression
```

## Comparing `clera-0.0.7.tar` & `clera-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 05:45:24.204774 clera-0.0.7/
--rw-rw-rw-   0        0        0      654 2023-04-25 04:51:01.000000 clera-0.0.7/CHANGELOG.md
--rw-rw-rw-   0        0        0     7651 2023-04-23 00:22:43.000000 clera-0.0.7/LICENCE.txt
--rw-rw-rw-   0        0        0       42 2023-04-01 11:31:56.000000 clera-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2503 2023-04-25 05:45:24.198527 clera-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1135 2023-04-25 05:28:48.000000 clera-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 05:45:24.009375 clera-0.0.7/clera/
--rw-rw-rw-   0        0        0      140 2023-04-24 21:56:58.000000 clera-0.0.7/clera/__init__.py
--rw-rw-rw-   0        0        0    51545 2023-04-24 20:28:34.000000 clera-0.0.7/clera/core.py
-drwxrwxrwx   0        0        0        0 2023-04-25 05:45:24.090233 clera-0.0.7/clera/icons/
--rw-rw-rw-   0        0        0   290225 2023-02-13 13:07:36.000000 clera-0.0.7/clera/icons/hand-drawn-icon.png
--rw-rw-rw-   0        0        0    41561 2023-04-25 04:20:56.000000 clera-0.0.7/clera/icons/toon-icon.ico
-drwxrwxrwx   0        0        0        0 2023-04-25 05:45:24.173017 clera-0.0.7/clera/utils/
--rw-rw-rw-   0        0        0      121 2023-03-19 13:16:12.000000 clera-0.0.7/clera/utils/__init__.py
--rw-rw-rw-   0        0        0      129 2023-03-24 12:03:54.000000 clera-0.0.7/clera/utils/exceptions.py
--rw-rw-rw-   0        0        0    16214 2023-04-24 20:53:36.000000 clera-0.0.7/clera/utils/handlers.py
--rw-rw-rw-   0        0        0     1071 2023-03-19 13:17:06.000000 clera-0.0.7/clera/utils/keys.py
--rw-rw-rw-   0        0        0     6196 2023-03-24 12:02:34.000000 clera-0.0.7/clera/utils/procr.py
--rw-rw-rw-   0        0        0     4238 2023-04-25 04:56:14.000000 clera-0.0.7/clera/utils/style.py
--rw-rw-rw-   0        0        0    27118 2023-04-24 20:54:33.000000 clera-0.0.7/clera/widgets.py
-drwxrwxrwx   0        0        0        0 2023-04-25 05:45:24.074920 clera-0.0.7/clera.egg-info/
--rw-rw-rw-   0        0        0     2503 2023-04-25 05:45:23.000000 clera-0.0.7/clera.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      476 2023-04-25 05:45:23.000000 clera-0.0.7/clera.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 05:45:23.000000 clera-0.0.7/clera.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 05:45:23.000000 clera-0.0.7/clera.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-25 05:45:23.000000 clera-0.0.7/clera.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 05:45:24.189582 clera-0.0.7/images/
--rw-rw-rw-   0        0        0   290225 2023-02-13 13:07:36.000000 clera-0.0.7/images/icon.png
--rw-rw-rw-   0        0        0     7524 2023-04-04 11:32:50.000000 clera-0.0.7/images/window.png
--rw-rw-rw-   0        0        0       42 2023-04-25 05:45:24.207492 clera-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1238 2023-04-25 05:45:20.000000 clera-0.0.7/setup.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-04 00:45:44.778245 clera-0.0.8/
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1127 2023-07-03 21:26:01.000000 clera-0.0.8/CHANGELOG.md
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     7651 2023-04-23 00:22:42.000000 clera-0.0.8/LICENCE.txt
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)       42 2023-04-01 11:31:56.000000 clera-0.0.8/MANIFEST.in
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3024 2023-07-04 00:45:44.778245 clera-0.0.8/PKG-INFO
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1259 2023-07-04 00:37:32.000000 clera-0.0.8/README.md
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-04 00:45:44.770248 clera-0.0.8/clera/
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      160 2023-07-03 21:11:09.000000 clera-0.0.8/clera/__init__.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    60519 2023-07-03 20:55:43.000000 clera-0.0.8/clera/core.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-04 00:45:44.774246 clera-0.0.8/clera/icons/
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)   290225 2023-02-13 13:07:36.000000 clera-0.0.8/clera/icons/hand-drawn-icon.png
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)    41561 2023-04-25 04:20:56.000000 clera-0.0.8/clera/icons/toon-icon.ico
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-04 00:45:44.774246 clera-0.0.8/clera/utils/
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      121 2023-03-19 13:16:12.000000 clera-0.0.8/clera/utils/__init__.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      129 2023-03-24 12:03:54.000000 clera-0.0.8/clera/utils/exceptions.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    18834 2023-07-02 22:56:52.000000 clera-0.0.8/clera/utils/handlers.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     1071 2023-03-19 13:17:06.000000 clera-0.0.8/clera/utils/keys.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     6431 2023-07-02 16:17:50.000000 clera-0.0.8/clera/utils/procr.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     4295 2023-07-03 00:25:19.000000 clera-0.0.8/clera/utils/style.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    27761 2023-07-03 00:12:08.000000 clera-0.0.8/clera/widgets.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-04 00:45:44.774246 clera-0.0.8/clera.egg-info/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3024 2023-07-04 00:45:44.000000 clera-0.0.8/clera.egg-info/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      442 2023-07-04 00:45:44.000000 clera-0.0.8/clera.egg-info/SOURCES.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-04 00:45:44.000000 clera-0.0.8/clera.egg-info/dependency_links.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        8 2023-07-04 00:45:44.000000 clera-0.0.8/clera.egg-info/requires.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        6 2023-07-04 00:45:44.000000 clera-0.0.8/clera.egg-info/top_level.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-04 00:45:44.778245 clera-0.0.8/setup.cfg
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1267 2023-07-03 21:16:42.000000 clera-0.0.8/setup.py
```

### Comparing `clera-0.0.7/LICENCE.txt` & `clera-0.0.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `clera-0.0.7/clera/core.py` & `clera-0.0.8/clera/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-
 from PySide6.QtCore import QSize, QPoint, QEvent
-from PySide6.QtGui import QIcon, Qt, QMouseEvent, QScreen
+from PySide6.QtGui import QIcon, Qt, QMouseEvent, QScreen, QSyntaxHighlighter
 from PySide6.QtWidgets import QMainWindow, QToolBar, QStatusBar, QGroupBox, QButtonGroup
 from PySide6.QtWidgets import QWidget,  QHBoxLayout, QVBoxLayout,  QGridLayout, QTabWidget, QMenu
-from PySide6.QtWidgets import QDialog, QFileDialog, QStyleFactory
-
+from PySide6.QtWidgets import QDialog, QFileDialog, QStyleFactory, QStackedWidget
+################################
+################################
 from .utils import *
 from .widgets import *
 
 __all__ = [
     'Window', 'Box', 'Grid', 'fieldset', 'Column', 'column', 'Group', 'group', 'Toolbar', 'toolbar',
     'Menubar', 'menubar', 'Statusbar', 'statusbar', 'GET', 'get', 'Button', 'button', 'Input',
     'input', 'Text', 'text', 'Image', 'image', 'CheckBox', 'checkbox', 'RadioButton', 'radiobutton',
     'Textarea', 'textarea', 'item', 'empty', 'separator', 'Exit', 'exit', 'Copy', 'copy', 'Cut', 'cut',
     'Paste', 'paste', 'Undo', 'undo', 'Redo', 'redo', 'link', 'ListWidget', 'listwidget', 'ListItem',
     'tab', 'TabWidget', 'tabwidget', 'Select', 'select', 'option', 'ProgressBar', 'progressbar',
     'Slider', 'slider', 'Dial', 'dial', 'Popup', 'popup', 'call', 'Titlebar', 'titlebar', 'File', 'file',
-    'Folder', 'folder', 'ScrollArea', 'scrollarea', 'minimize', 'maximize', 'close', 'title'
+    'Folder', 'folder', 'ScrollArea', 'scrollarea', 'minimize', 'maximize', 'close', 'title', 'Highlight',
+    'r', 'Stack'
 ]
 
 
 app = start()
 
 DEFAULT_WINDOW_LAYOUT = QWidget()
 
@@ -43,15 +44,15 @@
             property = property.replace(TYPE_MARKER, _type)
             widget.setStyleSheet(property)
 
     app.setStyleSheet(builtins)
 
 
 def link(href: None = None):
-    if href != None:
+    if href != None and href.strip().endswith('.cx'):
         LINK_ITEMS_INCLUDED.append(href)
 
 
 def init_linked_files():
     for LINK_ITEM in LINK_ITEMS_INCLUDED:
         file_path = path.abspath(LINK_ITEM)
 
@@ -248,34 +249,42 @@
     def REMOVE_STATUSBAR_WIDGET(self, ID):
         if ID in WIDGET_ID_SAFE:
             self.statusBar().removeWidget(WIDGET_ID_SAFE[ID])
         else:
             raise IdError(f'id "{ID}" does not exist')
 
     def mousePressEvent(self, event):
+        if self._movable == True:
+            window.setCursor(Qt.SizeAllCursor)
+
         self.old_position = event.globalPos()
         return self.old_position
 
     def mouseMoveEvent(self, event):
         omega = QPoint(event.globalPos() - self.old_position)
 
         if self._custom_title_bar == False and self._movable == True and self._frame == False:
             self.move(self.x() + omega.x(), self.y() + omega.y())
             self.old_position = event.globalPos()
         else:
             return omega
+    
+    def mouseReleaseEvent(self, event: QMouseEvent):
+        window.setCursor(Qt.ArrowCursor)
 
     def WindowTitlebar(self, icon, title, widgets, alignment, backgound_color,  text_color, height,
                        button_style):
         current_window_style = window.style().name().lower()
 
         if current_window_style == SYSTEM_PLATFORM_FUSION:
             CONTROL_MINIMIZED, CONTROL_RESTORE, CONTROL_MAXIMIZED = FUSION_CONTROLS()
-        elif current_window_style == SYSTEM_PLATFORM_WINDOWS:
+        elif current_window_style == SYSTEM_PLATFORM_WINDOWS or 'windows' in current_window_style:
             CONTROL_MINIMIZED, CONTROL_RESTORE, CONTROL_MAXIMIZED = WINDOWS_CONTROLS()
+            if SYSTEM_OS_PLATFORM == 'windows':
+                CONTROL_MAXIMIZED = '🗖'
         else:
             CONTROL_MINIMIZED, CONTROL_RESTORE, CONTROL_MAXIMIZED = CLERA_CONTROLS()
 
         if self._custom_title_bar == False and self._frame == False:
             if alignment != None:
                 if alignment.lower() == 'center':
                     align = 'center'
@@ -356,14 +365,15 @@
             container.setStyleSheet('margin: 0; padding: 0; border: 0px;')
 
             container.setMovable(False)
             titlebar.setMovable(False)
 
             self.addToolBar(Qt.TopToolBarArea, container)
 
+            container.toggleViewAction().setVisible(False)
             titlebar.toggleViewAction().setVisible(False)
 
             titlebar.setIconSize(QSize(20, 20))
 
             # self.addToolBar(Qt.TopToolBarArea, titlebar)
 
             self.addToolBarBreak()
@@ -436,25 +446,29 @@
 
 # ------------------------------------------------------------------------#
 
 
 class Window:
     def __init__(self, title: str = DEFAULT_WINDOW_TITLE, icon: str = DEFAULT_WINDOW_ICON, size: tuple = DEFAULT_WINDOW_SIZE,
                  geometry: tuple = DEFAULT_WINDOW_GEOMETRY, style: str = DEFAULT_WINDOW_STYLE, fixed_size: tuple = DEFAULT_WINDOW_FIXED_SIZE, frame: bool = True,
-                 movable: bool = False, top: bool = False, spacing: int = 2, content_margin: tuple = (2, 2, 2, 2),
+                 movable: bool = False, top: bool = False, spacing: int = 5, content_margin: tuple = (5, 5, 5, 5),
                  move: tuple = (None, None)):
         '''
         :param title:
         :param icon:
         :param size:
         :param geometry:
         :param style:
         :param fixed_size:
         :param frame:
         :param movable:
+        :param top:
+        :param spacing:
+        :param content_margin:
+        :param move:
         '''
         global window
 
         self.window_title = title
         self.window_icon = icon
         self.window_size = size
         self.window_fixed_size = fixed_size
@@ -554,14 +568,25 @@
 
     def _move(self, position: tuple = (None, None), top: bool = None):
         positionx, positiony = position
 
         if positionx != None and positiony != None:
             window.move(positionx, positiony)
 
+    # def frames(self, value):
+    #     # if value != window.frame:
+
+    #     if value == False:
+    #         window.setWindowFlag(Qt.FramelessWindowHint)
+    #     elif value == True:
+    #         window.setWindowFlag(~Qt.FramelessWindowHint)
+
+    #     print(window.windowFlags())
+    #     window.show()
+
 
 # ------------------------------------------------------------------------#
 
 ###########################################################################
 ############################## CORE HANDLERS ##############################
 ###########################################################################
 
@@ -626,15 +651,15 @@
 
 def Box(widgets):
     containers = [ELEM_TYPE_COLUMN, ELEM_TYPE_FIELDSET,
                   ELEM_TYPE_GROUP]
     box_layout = QVBoxLayout()
     box_widget = QWidget()
 
-    if ELEM_TYPE_TAB not in get_parent() and BOX_IDENTIFIER not in get_parent() and ELEM_TYPE_SCROLL_AREA not in get_parent():
+    if get_parent(BOX_IDENTIFIER):
         box_widget = DEFAULT_WINDOW_LAYOUT
         box_layout = layout
         window.setCentralWidget(box_widget)
 
     box_widget.setLayout(box_layout)
 
     for items in widgets:
@@ -695,23 +720,23 @@
                         group_element_layout = QVBoxLayout()
                     elif group_layout.lower() in DEFAULT_HORIZONTAL_TYPES:
                         group_element_layout = QHBoxLayout()
                     else:
                         raise ValueError(group_layout)
                     layout.addLayout(group_element_layout)
                     handle_group(widgets, group_element_layout)
-
+    # returns a QWidget and layout like QVBoxLayout
     return [box_widget, box_layout]
 
 
 def Grid(widgets):
     grid_widget = QWidget()
     grid = QGridLayout()
 
-    if ELEM_TYPE_TAB not in get_parent() and GRID_IDENTIFIER not in get_parent():
+    if get_parent(GRID_IDENTIFIER):
         grid_widget = DEFAULT_WINDOW_LAYOUT
         grid_layout = layout
 
         window.setCentralWidget(grid_widget)
         grid_layout.addLayout(grid)
 
     grid_widget.setLayout(grid)
@@ -723,55 +748,104 @@
         for item in items:
             widget_type, widget_items = check_func(item)
             LayItOut(grid, widget_type, widget_items, grid_pos_x, grid_pos_y)
             grid_pos_y += 1
         grid_pos_y = 0
         grid_pos_x += 1
 
-    return grid_widget
+    return [grid_widget, grid_layout]
 
 
 class ScrollArea:
     def __init__(self, widgets: None = None, id: None = None, contain: bool = True):
         '''
         ScrollArea
 
         :param widgets:
         :param id:
         :param contain:
         '''
+
         elem_type = ELEM_TYPE_SCROLL_AREA
         widgets = widgets[0]
-
         self.scroll_widget = QWidget()
+
+        if ELEM_TYPE_TAB not in get_parent() and SCROLL_AREA_IDENTIFIER not in get_parent():
+            # layout.addWidget(scroll_area)
+            window.setCentralWidget(self.scroll_widget)
+
         scroll_layout = QVBoxLayout()
 
         scroll_area = INIT_WIDGET(id, QScrollArea())
         scroll_layout.addWidget(scroll_area)
         self.scroll_widget.setLayout(scroll_layout)
-
         scroll_area.setWidget(widgets)
         scroll_area.setAlignment(Qt.AlignBottom)
         scroll_area.setWidgetResizable(contain)
 
-        if ELEM_TYPE_TAB not in get_parent() and SCROLL_AREA_IDENTIFIER not in get_parent():
-            layout.addWidget(scroll_area)
+        
 
     def __repr__(self):
         return [self.scroll_widget]
 
     def __call__(self):
         return [self.scroll_widget]
 
 
 class scrollarea(ScrollArea):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
+class Stack:
+    def __init__(self, widgets: None = None, id: None = None, current_changed: None = None, widget_removed: None = None):
+        '''
+        Stack Widget
+
+        :param widgets:
+        :param id:
+        :param current_changed:
+        :param widget_removed:
+        '''
+        self.stacked_widget = INIT_WIDGET(id, QStackedWidget())
+        
+        def init_stack(widget):
+            widget = widget[0]
+            self.stacked_widget.addWidget(widget)
+
+        if widgets != None:
+            if process_request(ELEM_TYPE_SCROLL_AREA, str(type(widgets)).lower()):
+                widgets = widgets()
+            
+            if type(widgets[0]) == sample_list:
+                for widget in widgets:
+                    init_stack(widget)    
+            else:
+                init_stack(widgets)    
+        
+        layout.addWidget(self.stacked_widget)
+        DEFAULT_WINDOW_LAYOUT.setLayout(layout)
+
+        self.stacked_widget.currentChanged.connect(current_changed)
+        self.stacked_widget.widgetRemoved.connect(widget_removed)
+        
+        window.setCentralWidget(DEFAULT_WINDOW_LAYOUT)
+    def set(self, index):
+        self.stacked_widget.setCurrentIndex(index)
+
+    def show(self, widget):
+        widget, layout = widget
+        self.stacked_widget.setCurrentWidget(widget)
+
+
+class stack(Stack):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
 # ------------------------------------------------------------------------#
 
 ###########################################################################
 ############################## CORE ELEMENTS ##############################
 ###########################################################################
 
 # ------------------------------------------------------------------------#
@@ -889,14 +963,15 @@
         Open File Dialog
 
         :param caption:
         :param filter:
         :param directory:
         :param type:
         '''
+
         open_type = type.lower()
 
         if type == OPEN_FILE_TYPE_SINGLE:
             file = self.getOpenFileName(
                 caption=caption,
                 dir=directory,
                 filter=get_filter(filter))
@@ -933,42 +1008,50 @@
     def __init__(self, caption: str = None, directory: str = None):
         '''
         Folder Dialog
 
         :param caption:
         :param directory:
         '''
+        
         self.folder = self.getExistingDirectory(caption=caption,
                                                 dir=directory)
 
     def __repr__(self):
         return self.folder
 
 
 class folder(Folder):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class Popup:
     def __init__(self, title: None = None, widgets: None = None, size: tuple = (None, None), id: None = None,
-                 modal: bool = False, frame: bool = True):
+                 modal: bool = False, frame: bool = True, lock: bool = False):
         '''
         Popup Window
 
         :param title:
         :param widgets:
         :param size:
         :param id:
         :param modal:
         :param frame:
+        :param lock:
         '''
 
+        if lock == True:
+            parent = DEFAULT_WINDOW_LAYOUT
+        else:
+            parent = None
+
         elem_type = ELEM_TYPE_POPUP
-        popup = INIT_WIDGET(id, QDialog())
+        popup = INIT_WIDGET(id, QDialog(parent))
+
         self.popup = popup
 
         popup.setWindowTitle(title)
 
         if widgets != None:
             popup_layout = Box(widgets)
 
@@ -981,24 +1064,27 @@
             popup.resize(int(width), int(height))
 
         # popup.resize(200, 120)
 
         if frame == False:
             popup.setWindowFlag(Qt.FramelessWindowHint)
 
-        popup.exec()
+        if popup.isModal:
+            popup.show()
+        else:
+            popup.exec()
 
         self.rtn = [elem_type, id, popup]
 
     def __call__(self):
         return self.rtn
 
     def result(self):
         return self.popup.result()
-
+    
 
 class popup(Popup):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class TabWidget:
@@ -1038,16 +1124,100 @@
 
 
 class tabwidget(TabWidget):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
+class Highlighter(QSyntaxHighlighter):
+    def __init__(self, mapping, parent=None):
+        super().__init__(parent)
+        self.mapping = mapping
+
+    def highlightBlock(self, text):
+        for pattern, format in self.mapping.items():
+            for match in re.finditer(pattern, text):
+                start, end = match.span()
+                self.setFormat(start, end-start, format)
+
+
+class Highlight:
+    def __init__(self, id, synthax):
+
+        mapping = {}
+
+        for item in synthax.items():
+            pattern, format = item
+        
+            pattern = rf'{pattern}'
+            _format = INIT_FORMAT(format)
+
+            mapping[pattern] = _format
+        
+        widget = WIDGET_ID_SAFE[id]
+        synthax = Highlighter(mapping)
+        synthax.setDocument(widget.document())
+        
+        synthax.document()
+        
+
 class GET:
     def __init__(self, id):
+
+        '''
+        GET ELEMENT
+
+        :param id:
+
+        :method value:
+        :method update:
+        :method delete:
+        :method append:
+        :method html:
+        :method insert_html:
+        :method plain_text:
+        :method alignment:
+        :method is_default:
+        :method is_readonly:
+        :method style:
+        :method is_checked:
+        :method hidden:
+        :method hide:
+        :method diabled:
+        :method disable:
+        :method enable:
+        :method is_hidden:
+        :method is_disabled:
+        :method select_all:
+        :method copy:
+        :method cut:
+        :method undo:
+        :method redo:
+        :method paste:
+        :method clear:
+        :method add:
+        :method remove:
+        :method current:
+        :method count:
+        :method selected_items:
+        :method set:
+        :method index:
+        :method reset:
+        :method minimum:
+        :method maximum:
+        :method is_text_visible:
+        :method reject:
+        :method accept:
+        :method focus:
+        :method cursor:
+        :method setcursor:
+        :method icon:
+        :method show:
+        :method scrollbar:
+        '''
         self.id = id
         self.widget = WIDGET_ID_SAFE[self.id]
         self.widget_type = str(type(self.widget))
 
     def __repr__(self):
         allowed = [
             [
@@ -1055,29 +1225,29 @@
                 GET_ELEM_TYPE_SLIDER,
                 GET_ELEM_TYPE_DIAL
             ],
 
             GET_ELEM_TYPE_TEXTAREA
         ]
 
-        if process_request(allowed[0], self.widget_type) == True:
+        if process_request(allowed[0], self.widget_type):
             return str(self.widget.value())
         elif process_request(allowed[1], self.widget_type):
             return self.widget.toPlainText()
         else:
             return self.widget.text()
 
     def value(self, value: str | None = None):
         allowed = [
             GET_ELEM_TYPE_PROGRESS_BAR,
             GET_ELEM_TYPE_SLIDER,
             GET_ELEM_TYPE_DIAL
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.setValue(int(value))
         else:
             self.widget.setText(str(value))
 
     def update(self, widget):
         widget_type, widget_items = check_func(widget)
 
@@ -1099,45 +1269,45 @@
         self.widget = None
 
     def append(self, value: str = ''):
         allowed = [
             GET_ELEM_TYPE_TEXTAREA
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.append(value)
 
     def html(self, value):
         allowed = [
             GET_ELEM_TYPE_TEXTAREA
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.setHtml(value)
 
     def insert_html(self, value):
         allowed = [
             GET_ELEM_TYPE_TEXTAREA
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.insertHtml(value)
 
     def plain_text(self, value: None = None):
         allowed = [
             GET_ELEM_TYPE_TEXTAREA
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             if value != None:
                 self.widget.setPlainText(value)
             else:
                 return self.widget.toPlainText()
 
-    def alignmnet(self, value: None = None):
+    def alignment(self, value: None = None):
         if value != None:
             make_alignment(self.widget, value)
         else:
             return self.widget.alignment()
 
     def is_default(self):
         return self.widget.isDefault()
@@ -1225,210 +1395,324 @@
 
     def hidden(self, value: bool | None = None):
         if value != None:
             self.widget.setHidden(value)
 
     def hide(self):
         self.widget.setHidden(True)
+    
+    def disabled(self, value: bool | None = None):
+        if value != None:
+            self.widget.setDisabled(value)
+
+    def disable(self):
+        self.widget.setDisabled(True)
+
+    def enable(self):
+        self.widget.setEnabled(True)
 
     def is_hidden(self):
         return self.widget.isHidden()
 
+    def is_disabled(self):
+            return self.widget.isDisabled()
+
     def select_all(self):
         allowed = [
             GET_ELEM_TYPE_TEXTAREA
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.selectAll()
 
     def copy(self):
         allowed = [
             GET_ELEM_TYPE_TEXTAREA
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.copy()
 
     def cut(self):
         allowed = [
             GET_ELEM_TYPE_TEXTAREA
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.cut()
 
     def undo(self):
         allowed = [
             GET_ELEM_TYPE_TEXTAREA
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.undo()
 
     def redo(self):
         allowed = [
             GET_ELEM_TYPE_TEXTAREA
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.redo()
 
     def paste(self):
         allowed = [
             GET_ELEM_TYPE_TEXTAREA
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.paste()
 
     def clear(self):
         allowed = [
             GET_ELEM_TYPE_TEXTAREA,
             GET_ELEM_TYPE_LISTWIDGET,
             GET_ELEM_TYPE_SELECT,
             GET_ELEM_TYPE_TAB_WIDGET
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.clear()
 
     def add(self, items):
         allowed = [
             GET_ELEM_TYPE_LISTWIDGET,
             GET_ELEM_TYPE_SELECT,
-            GET_ELEM_TYPE_TAB_WIDGET
+            GET_ELEM_TYPE_TAB_WIDGET,
+            GET_ELEM_TYPE_STACKED
         ]
 
-        if process_request(allowed[0], self.widget_type) == True:
+        if process_request(allowed[0], self.widget_type):
             add_list_items(self.widget, items)
-        elif process_request(allowed[1], self.widget_type) == True:
+        elif process_request(allowed[1], self.widget_type):
             if type(items[0]) == sample_list:
                 pass
             elif type(items[0]) == sample_string:
                 items = [items]
-        elif process_request(allowed[2], self.widget_type) == True:
+        elif process_request(allowed[2], self.widget_type):
             add_tabs(self.widget, items)
+        elif process_request(allowed[3], self.widget_type):
+            add_stacks(self.widget, items)
 
     def remove(self, items):
         allowed = [
             GET_ELEM_TYPE_LISTWIDGET,
             GET_ELEM_TYPE_SELECT,
-            GET_ELEM_TYPE_TAB_WIDGET
+            GET_ELEM_TYPE_TAB_WIDGET,
+            GET_ELEM_TYPE_STACKED
         ]
 
-        if process_request(allowed[0], self.widget_type) == True:
+        if process_request(allowed[0], self.widget_type):
             self.widget.takeItem(items)
-        elif process_request(allowed[1], self.widget_type) == True:
+        elif process_request(allowed[1], self.widget_type):
             self.widget.removeItem(items)
-        elif process_request(allowed[2], self.widget_type) == True:
+        elif process_request(allowed[2], self.widget_type):
             self.widget.removeTab(items)
+        elif process_request(allowed[3], self.widget_type):
+            def init_remove(widget):
+                widget, layout = widget
+                if widget != None:
+                    self.widget.removeWidget(widget)
+            
+            
+            if type(items) == sample_integer:
+                # Handle later
+                items = [self.widget.widget(items), None]
+                init_remove(items)
+            elif type(items[0]) == sample_list:
+                for item in items:
+                    init_remove(item)
+            else:
+                init_remove(items)
+
 
     def current(self):
         allowed = [
             GET_ELEM_TYPE_LISTWIDGET,
             GET_ELEM_TYPE_SELECT,
-            GET_ELEM_TYPE_TAB_WIDGET
+            [
+                GET_ELEM_TYPE_TAB_WIDGET,
+                GET_ELEM_TYPE_STACKED
+            ]
         ]
 
-        if process_request(allowed[0], self.widget_type) == True:
+        if process_request(allowed[0], self.widget_type):
             return self.widget.currentRow()
-        elif process_request(allowed[1], self.widget_type) == True:
+        elif process_request(allowed[1], self.widget_type):
             return self.widget.currentText()
-        elif process_request(allowed[2], self.widget_type) == True:
+        elif process_request(allowed[2], self.widget_type):
             return self.widget.currentIndex()
 
     def count(self):
         allowed = [
             GET_ELEM_TYPE_LISTWIDGET,
             GET_ELEM_TYPE_SELECT,
-            GET_ELEM_TYPE_TAB_WIDGET
+            GET_ELEM_TYPE_TAB_WIDGET,
+            GET_ELEM_TYPE_STACKED
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             return self.widget.count()
 
     def selected_items(self):
         allowed = [
             GET_ELEM_TYPE_LISTWIDGET,
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             selected_items = [items.text()
                               for items in self.widget.selectedItems()]
             return selected_items
 
     def set(self, value):
         allowed = [
             GET_ELEM_TYPE_SELECT,
+            GET_ELEM_TYPE_STACKED
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.setCurrentIndex(value)
 
+
     def index(self):
         allowed = [
             GET_ELEM_TYPE_SELECT,
+            GET_ELEM_TYPE_STACKED
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             return self.widget.currentIndex()
 
     def reset(self):
         allowed = [
             GET_ELEM_TYPE_PROGRESS_BAR,
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.reset()
 
     def minimum(self):
         allowed = [
             GET_ELEM_TYPE_PROGRESS_BAR,
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             return self.widget.minimum()
 
     def maximum(self):
         allowed = [
             GET_ELEM_TYPE_PROGRESS_BAR,
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             return self.widget.maximum()
 
     def is_text_visible(self):
         allowed = [
             GET_ELEM_TYPE_PROGRESS_BAR,
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             return self.widget.isTextVisible()
 
     def reject(self, result: int = None):
         allowed = [
             GET_ELEM_TYPE_POPUP,
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.reject()
             if result != None:
                 self.widget.setResult(result)
 
     def accept(self, result: int = None):
         allowed = [
             GET_ELEM_TYPE_POPUP,
         ]
 
-        if process_request(allowed, self.widget_type) == True:
+        if process_request(allowed, self.widget_type):
             self.widget.accept()
             if result != None:
                 self.widget.setResult(result)
+    
+    def focus(self, value: bool = True):
+        allowed = [
+            GET_ELEM_TYPE_INPUT,
+            GET_ELEM_TYPE_TEXTAREA
+        ]
+
+        if process_request(allowed, self.widget_type):
+            self.widget.setFocus()
+    
+
+    def has_focus(self, value: bool = True):
+        allowed = [
+            GET_ELEM_TYPE_INPUT,
+            GET_ELEM_TYPE_TEXTAREA
+        ]
+
+        if process_request(allowed, self.widget_type):
+            return self.widget.hasFocus()
+
+    def cursor(self):
+        allowed = [
+            GET_ELEM_TYPE_INPUT,
+            GET_ELEM_TYPE_TEXTAREA
+        ]
+
+        if process_request(allowed, self.widget_type):
+            cursor = self.widget.textCursor()
+            position = cursor.position()
+
+            return cursor, position
 
+    
+    def setcursor(self, cursor):
+        cursor, position = cursor
+
+        cursor.setPosition(position)
+        self.widget.setTextCursor(cursor)
+
+    def icon(self, path):
+        self.widget.setIcon(QIcon(path))
+
+    def show(self, widget):
+        allowed = [
+            GET_ELEM_TYPE_STACKED
+        ]
+
+        if process_request(allowed, self.widget_type):
+            widget, layout = widget
+            self.widget.setCurrentWidget(widget)
+
+    def scrollbar(self, scrollbar: None = None, bar_type: str = 'v', id: None = None):
+        allowed = [
+            GET_ELEM_TYPE_TEXTAREA
+        ]
+
+        if process_request(allowed, self.widget_type):
+            if scrollbar != None:
+                if bar_type == 'v':
+                    self.widget.setVerticalScrollBar(scrollbar)
+                elif bar_type == 'h':
+                    self.widget.setHorizontalScrollBar(scrollbar)
+            else:
+                if bar_type == 'v':
+                    bar =  self.widget.verticalScrollBar()
+                elif bar_type == 'h':
+                    bar = self.widget.horizontalScrollBar()
+                else:
+                    bar = None
+
+                if bar != None:
+                    return INIT_WIDGET(id, bar)
+                else:
+                    return bar
 
 class get(GET):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 # ------------------------------------------------------------------------#
@@ -1439,120 +1723,126 @@
 
 # ------------------------------------------------------------------------#
 
 
 class Exit(Button):
     def __init__(self, label: str = 'Exit', icon: None = None, id: None = None,
                  disabled: bool = False, default: bool = False, grid: tuple = (None, None),
-                 sizepolicy: tuple = (None, None), checkable: bool = False, checked: bool = False, hidden: bool = False, focus: bool = True):
+                 sizepolicy: tuple = (None, None), checkable: bool = False, checked: bool = False, hidden: bool = False, focus: bool = True, 
+                 icon_size: int = 20, statustip: str = None, tooltip: str = None, shortcut: str = None):
 
         elem_type = ELEM_TYPE_BUTTON
 
         self.rtn = [elem_type, label, Window.quit, icon, id,
-                    disabled, default, grid, sizepolicy, checkable, checked, hidden, focus]
+                    disabled, default, grid, sizepolicy, checkable, checked, hidden, focus, icon_size, statustip, tooltip, shortcut]
 
     def __call__(self):
         return self.rtn
 
 
 class exit(Exit):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class Copy(Button):
     def __init__(self, Target_ID, button_text: str = 'Copy', icon: None = None,
                  id: None = None, disabled: bool = False, default: bool = False,
-                 grid: tuple = (None, None), sizePolicy: tuple = (None, None), checked: bool = False, hidden: bool = False, focus: bool = True):
+                 grid: tuple = (None, None), sizePolicy: tuple = (None, None), checked: bool = False, hidden: bool = False, focus: bool = True, 
+                 icon_size: int = 20, statustip: str = None, tooltip: str = None, shortcut: str = None):
 
         elem_type = elem_type, id = pre_widget_process('copy')
         METHOD_COPY.append(f'{id}:{Target_ID}')
 
         self.rtn = [elem_type, button_text, action_copy, icon, id,
-                    disabled, default, grid, sizePolicy, True, checked, hidden, focus]
+                    disabled, default, grid, sizePolicy, True, checked, hidden, focus, icon_size, statustip, tooltip, shortcut]
 
     def __call__(self):
         return self.rtn
 
 
 class copy(Copy):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class Cut(Button):
     def __init__(self, Target_ID, button_text: str = 'Cut', icon: None = None,
                  id: None = None, disabled: bool = False, default: bool = False,
-                 grid: tuple = (None, None), sizePolicy: tuple = (None, None), checked: bool = False, hidden: bool = False, focus: bool = True):
+                 grid: tuple = (None, None), sizePolicy: tuple = (None, None), checked: bool = False, hidden: bool = False, focus: bool = True, 
+                 icon_size: int = 20, statustip: str = None, tooltip: str = None, shortcut: str = None):
 
         elem_type, id = pre_widget_process('cut')
         METHOD_CUT.append(f'{id}:{Target_ID}')
 
         self.rtn = [elem_type, button_text, action_cut, icon, id,
-                    disabled, default, grid, sizePolicy, True, checked, hidden, focus]
+                    disabled, default, grid, sizePolicy, True, checked, hidden, focus, icon_size, statustip, tooltip, shortcut]
 
     def __call__(self):
         return self.rtn
 
 
 class cut(Cut):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class Paste(Button):
     def __init__(self, Target_ID, button_text: str = 'Paste', icon: None = None,
                  id: None = None, disabled: bool = False, default: bool = False,
-                 grid: tuple = (None, None), sizePolicy: tuple = (None, None), checked: bool = False, hidden: bool = False, focus: bool = True):
+                 grid: tuple = (None, None), sizePolicy: tuple = (None, None), checked: bool = False, hidden: bool = False, focus: bool = True, 
+                 icon_size: int = 20, statustip: str = None, tooltip: str = None, shortcut: str = None):
 
         elem_type, id = pre_widget_process('paste')
         METHOD_PASTE.append(f'{id}:{Target_ID}')
 
         self.rtn = [elem_type, button_text, action_paste, icon, id,
-                    disabled, default, grid, sizePolicy, True, checked, hidden, focus]
+                    disabled, default, grid, sizePolicy, True, checked, hidden, focus, icon_size, statustip, tooltip, shortcut]
 
     def __call__(self):
         return self.rtn
 
 
 class paste(Paste):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class Undo(Button):
     def __init__(self, Target_ID, button_text: str = 'Undo', icon: None = None,
                  id: None = None, disabled: bool = False, default: bool = False,
-                 grid: tuple = (None, None), sizePolicy: tuple = (None, None), checked: bool = False, hidden: bool = False, focus: bool = True):
+                 grid: tuple = (None, None), sizePolicy: tuple = (None, None), checked: bool = False, hidden: bool = False, focus: bool = True, 
+                 icon_size: int = 20, statustip: str = None, tooltip: str = None, shortcut: str = None):
 
         elem_type = elem_type, id = pre_widget_process('undo')
         METHOD_UNDO.append(f'{id}:{Target_ID}')
 
         self.rtn = [elem_type, button_text, action_undo, icon, id,
-                    disabled, default, grid, sizePolicy, True, checked, hidden, focus]
+                    disabled, default, grid, sizePolicy, True, checked, hidden, focus, icon_size, statustip, tooltip, shortcut]
 
     def __call__(self):
         return self.rtn
 
 
 class undo(Undo):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
 class Redo(Button):
     def __init__(self, Target_ID, button_text: str = 'Redo', icon: None = None,
                  id: None = None, disabled: bool = False, default: bool = False,
-                 grid: tuple = (None, None), sizePolicy: tuple = (None, None), checked: bool = False, hidden: bool = False, focus: bool = True):
+                 grid: tuple = (None, None), sizePolicy: tuple = (None, None), checked: bool = False, hidden: bool = False, focus: bool = True, 
+                 icon_size: int = 20, statustip: str = None, tooltip: str = None, shortcut: str = None):
 
         elem_type = elem_type, id = pre_widget_process('redo')
         METHOD_REDO.append(f'{id}:{Target_ID}')
 
         self.rtn = [elem_type, button_text, action_redo, icon, id,
-                    disabled, default, grid, sizePolicy, True, checked, hidden, focus]
+                    disabled, default, grid, sizePolicy, True, checked, hidden, focus, icon_size, statustip, tooltip, shortcut]
 
     def __call__(self):
         return self.rtn
 
 
 class redo(Redo):
     def __init__(self, *args, **kwargs):
@@ -1593,7 +1883,17 @@
 # ------------------------------------------------------------------------#
 
 
 # def main():
 #     window = Window()
 #     Box([[Button('UNAVAILABLE')]])
 #     window.run()
+
+
+# ------------------------------------------------------------------------#
+
+###########################################################################
+########################### CLERA STYLING EDITOR ##########################
+###########################################################################
+
+# ------------------------------------------------------------------------#
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clera-0.0.7/clera/icons/hand-drawn-icon.png` & `clera-0.0.8/clera/icons/hand-drawn-icon.png`

 * *Files identical despite different names*

### Comparing `clera-0.0.7/clera/icons/toon-icon.ico` & `clera-0.0.8/clera/icons/toon-icon.ico`

 * *Files identical despite different names*

### Comparing `clera-0.0.7/clera/utils/handlers.py` & `clera-0.0.8/clera/utils/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import os.path as path
 import sys
 import inspect
+import re
 
-
-from PySide6.QtGui import QAction, QIcon, Qt
+from PySide6.QtGui import QAction, QIcon, Qt, QTextCharFormat, QColor,QKeyEvent
 from PySide6.QtWidgets import QSizePolicy, QApplication
 from PySide6.QtWidgets import QListWidgetItem, QAbstractItemView, QComboBox
 
 
 def start():
     app = QApplication(sys.argv)
     return app
@@ -60,14 +60,15 @@
 ELEM_TYPE_PROGRESS_BAR = 'progress_bar'
 ELEM_TYPE_SLIDER = 'slider'
 ELEM_TYPE_DIAL = 'dial'
 ELEM_TYPE_POPUP = 'popup'
 ELEM_TYPE_TAB = 'tab'
 ELEM_TYPE_TAB_WIDGET = 'tab_widget'
 ELEM_TYPE_SCROLL_AREA = 'scrollarea'
+ELEM_TYPE_STACKED = 'stack'
 
 
 DEFAULT_VERTICAL_TYPES = ['vertical', 'v']
 DEFAULT_HORIZONTAL_TYPES = ['horizontal', 'h']
 
 SET_HORIZONTAL = 'HORIZONTAL'
 SET_VERTICAL = 'VERTICAL'
@@ -84,14 +85,17 @@
 GET_ELEM_TYPE_LISTWIDGET = 'QListWidget'
 GET_ELEM_TYPE_SELECT = 'QComboBox'
 GET_ELEM_TYPE_PROGRESS_BAR = 'QProgressBar'
 GET_ELEM_TYPE_SLIDER = 'QSlider'
 GET_ELEM_TYPE_DIAL = 'QDial'
 GET_ELEM_TYPE_TAB_WIDGET = 'QTabWidget'
 GET_ELEM_TYPE_POPUP = 'QDialog'
+GET_ELEM_TYPE_INPUT = 'QLineEdit'
+GET_ELEM_TYPE_STACKED = 'QStackedWidget'
+# GET_ELEM_TYPE_SCROLLAREA = 'QScrollArea'
 
 ITEM_SELECTION_MODE_EXTENDED = 'extended'
 ITEM_SELECTION_MODE_NO_SELECTION = 'no_selection'
 ITEM_SELECTION_MODE_MULTI = 'multi'
 ITEM_SELECTION_MODE_SINGLE = 'single'
 
 
@@ -125,15 +129,19 @@
 TITLE_TEXT_ID = '-clera_title-'
 MINIMIZE_BUTTON_ID = '-clera_minimize_button-'
 MAXIMIZE_BUTTON_ID = '-clera_maximize_button-'
 CLOSE_BUTTON_ID = '-clera_close_button-'
 
 GRID_IDENTIFIER = '=grid'
 BOX_IDENTIFIER = '=box'
+# TAB_IDENTIFIER = 'tab('
 SCROLL_AREA_IDENTIFIER = '=scrollarea'
+# STACK_IDENTIFIER = '=stack'
+
+SYSTEM_OS_PLATFORM = sys.platform.lower()
 
 
 def FUSION_CONTROLS():
     global CONTROL_MINIMIZED, CONTROL_RESTORE, CONTROL_MAXIMIZED
 
     CONTROL_MINIMIZED = '-'
     CONTROL_RESTORE = '+'
@@ -262,36 +270,51 @@
 
         return align
 
     align = alignCheck(alignments)
     widget.setAlignment(align)
 
 
-def get_parent():
+def get_parent(identifier):
     inspector = inspect.stack()[2][4]
-    return str(inspector).lower().replace(' ', '')
+    result = str(inspector).lower().replace(' ', '')
 
+    if (identifier not in result and f"{ELEM_TYPE_TAB}({identifier.removeprefix('=')}" not in result and 
+        ELEM_TYPE_SCROLL_AREA not in result and ELEM_TYPE_STACKED not in result):
+        return True
+    else:
+        return False
 
 def get_filter(value):
-    split_markers = ['), (', ') ,(', ') , (', '),(']
-    for split_marker in split_markers:
-        if split_marker in value:
-            value = value.replace(split_marker, FILTER_SPLIT_MARKER)
-
-    value = value.replace('(', '').replace(')', '')
-
+    # split_markers = ['), (', ') ,(', ') , (', '),(']
+    # for split_marker in split_markers:
+    #     if split_marker in value:
+    #         value = value.replace(split_marker, FILTER_SPLIT_MARKER)
+    # "(Python: *.py) , (Bash: *.sh, *.cmd)"
+    # value = value.replace('(', '').replace(')', '')
+    
+    value = value.split(')')
+    value = [item.split('(') for item in value]
+
+    result = [
+        item 
+            for items in range(len(value)) 
+                for item in value[items] 
+                    if len(item) != 0 and item.strip() != ','
+            ]
+    value = FILTER_SPLIT_MARKER.join(result)
+    
     def init_filter(filter):
         filter = filter.split(':')
         filter_type = filter[0].strip()
         extensions = filter[1]
         extensions = extensions.split(',')
-
         filter_extensions = ''
         for extension in extensions:
-            filter_extensions += '*' + extension.strip() + ' '
+            filter_extensions += extension.strip() + ' '
         else:
             filter_extensions = filter_extensions[:-1]
 
         return f'{filter_type} ({filter_extensions})'
 
     if FILTER_SPLIT_MARKER in value:
         filters = value.split(FILTER_SPLIT_MARKER)
@@ -317,29 +340,26 @@
         widget_type = property()[0]
         property = property()
 
     return widget_type, property
 
 
 def process_request(allowed: list = None, widget_type: None = None):
-
     if type(allowed) == sample_list:
         for values in allowed:
             if values in widget_type:
                 return True
         else:
             return False
 
     elif type(allowed) == sample_string:
         if allowed in widget_type:
             return True
         else:
             return False
-    else:
-        ...
 
 
 def add_list_items(widget, list_items):
 
     for items in list_items:
         NotRequired, label, icon = items
 
@@ -386,14 +406,26 @@
     if type(tabs[0]) == sample_list:
         for tab in tabs:
             init_tab(tab)
     elif type(tabs[0]) == sample_string:
         init_tab(tabs)
 
 
+def add_stacks(stack_widget, stacks):
+    def init_stack(stack):
+        widget, layout = stack
+        stack_widget.addWidget(widget)
+        
+    if type(stacks[0]) == sample_list:
+        for stack in stacks:
+            init_stack(stack)
+    else:
+        init_stack(stacks)
+
+
 def get_path(href):
     return path.abspath(href)
 
 
 # PRE-DEFINED WIDGETS
 PRE_DEFINED_WIDGETS = []
 PRE_WIDGETS_COUNT = [0]
@@ -475,18 +507,18 @@
 
 sample_function = type(sample_func())
 
 sample_integer = type(int())
 
 sample_tuple = type(tuple())
 
-if sys.platform.lower() == 'linux':
-    minimize_padding = ' padding: 0 7px 2px 7px'
-    maximize_padding = 'padding: 0px 6px 2px 6px'
-    close_padding = 'padding: 0 4px 1px 4px'
+if SYSTEM_OS_PLATFORM == 'linux':
+    minimize_padding = ' padding: 1px 7px 2px 7px'
+    maximize_padding = 'padding: 1px 6px 2px 6px'
+    close_padding = 'padding: 1px 4px 2px 4px'
 else:
     minimize_padding = 'padding: 1px 8px 3px 8px'
     maximize_padding = 'padding: 1px 6px 3px 6px'
     close_padding = 'padding: 1px 6px 3px 6px'
 
 
 def fusion_style(minimize, maximize, close, control_button_style):
@@ -495,15 +527,15 @@
             color: rgb(18, 18, 18);
             font-weight: bold;
             {minimize_padding};
             margin: 0 4px 0 5px;
             background: rgb(18, 18, 18);
             border-radius: {control_button_style};
             min-width: 0px;
-            height: 20px;
+            height: 17px;
         ]
 
         button:hover [
             color: white;
         ]
     ''')
 
@@ -512,15 +544,15 @@
             color: rgb(18, 18, 18);
             font-weight: bold;
             {maximize_padding};
             margin-right: 4px;
             background: rgb(18, 18, 18);
             border-radius: {control_button_style};
             min-width: 0px;
-            height: 20px;
+            height: 17px;
         ]
 
         button:hover [
             color: white;
         ]
     ''')
 
@@ -529,15 +561,15 @@
             color: rgb(18, 18, 18);
             margin-right: 8px;
             font-weight: bold;
             {close_padding};
             background: rgb(56, 109, 209);
             border-radius: {control_button_style};
             min-width: 0px;
-            height: 20px;
+            height: 17px;
         ]
 
         button:hover [
             color: white;
         ]
     ''')
 
@@ -638,7 +670,63 @@
 #             color: rgb(61, 0, 0);
 #         ]
 #     ''')
 
 
 def append_items(append_list, item):
     append_list.append(item)
+
+COLORS = {
+    'red'       : Qt.red,
+    'black'     : Qt.black,
+    'white'     : Qt.white,
+    'gray'      : Qt.gray,
+    'green'     : Qt.green,
+    'blue'      : Qt.blue,
+    'cyan'      : Qt.cyan,
+    'magenta'   : Qt.magenta,
+    'yellow'    : Qt.yellow,
+}
+
+def get_color(value):
+    if 'rgb' in value:
+        rgb = [0, 0, 0]
+        new_color = value.lower()
+        new_color = value.replace('(', '').replace(')', '')
+        new_color = new_color.replace('rgba', 'rgb')
+        color = new_color.removeprefix('rgb') 
+        color = color.split(',')
+
+        for _index in range(len(color)):
+            if _index <= 2:
+                rgb[_index] = int(color[_index])
+        else:
+            rgb = rgb[0:3]
+            red, green, blue = rgb
+            color = QColor(red, green, blue)
+    else:
+        try:
+            color = COLORS[value]
+        except:
+            color = None
+
+    return color
+
+
+def INIT_FORMAT(elements):
+    format = QTextCharFormat()
+    KEYS = elements.keys()
+    if 'color' in KEYS:
+        color = get_color(elements['color'])
+        if color != None:
+            format.setForeground(color)
+
+    if 'background' in KEYS:
+        background = get_color(elements['background'])
+        if background != None:
+            format.setBackground(background)
+            
+    return format
+
+def r(list: list = None):
+    if list != None:
+        return '|'.join([fr'\b{list[i]}\b' for i in range(len(list))])
```

### Comparing `clera-0.0.7/clera/utils/keys.py` & `clera-0.0.8/clera/utils/keys.py`

 * *Files identical despite different names*

### Comparing `clera-0.0.7/clera/utils/procr.py` & `clera-0.0.8/clera/utils/procr.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,33 @@
 
 
 def LayItOut(lyt, elem_type, property, grid_pos_x: None = None, grid_pos_y: None = None):
     if elem_type == ELEM_TYPE_BUTTON:
         [
             NotRequired,
             button_text,
-            func, icon,
-            id, disabled,
+            func, 
+            icon,
+            id, 
+            disabled,
             default,
             grid,
             sizepolicy,
             checkable,
             checked,
             hidden,
-            focus
+            focus,
+            icon_size, 
+            statustip,
+            tooltip,
+            shortcut
         ] = property
-
         widget = window_button(
-            lyt, button_text, func, icon, id, disabled, default, sizepolicy, grid, grid_pos_x, grid_pos_y, checkable, checked, hidden, focus)
+            lyt, button_text, func, icon, id, disabled, default, sizepolicy, grid, grid_pos_x, grid_pos_y, checkable, checked, hidden, focus, 
+            icon_size, statustip, tooltip, shortcut)
 
     elif elem_type == ELEM_TYPE_INPUT:
         [
             NotRequired,
             placeholder,
             id,
             value,
@@ -128,20 +134,22 @@
             undo_available,
             redo_available,
             maxlength,
             font,
             fontsize,
             sizepolicy,
             grid,
-            tabWidth
+            tabwidth,
+            wordwrap
         ] = property
 
         widget = window_textarea(lyt, id, placeholder, hidden, alignment, value, disabled, readonly,
                                  text_changed, selection_changed, undo_available, redo_available,
-                                 maxlength, font, fontsize, sizepolicy, grid, grid_pos_x, grid_pos_y, tabWidth)
+                                 maxlength, font, fontsize, sizepolicy, grid, grid_pos_x, grid_pos_y, 
+                                 tabwidth, wordwrap)
 
     elif elem_type == ELEM_TYPE_LIST_WIDGET:
         [
             NotRequired,
             list_items,
             id,
             mode,
```

### Comparing `clera-0.0.7/clera/utils/style.py` & `clera-0.0.8/clera/utils/style.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     'select::QComboBox',
     'progressbar::QProgressBar',
     'slider::QSlider',
     'dial::QDial',
     'tabwidget::QTabWidget',
     'popup::QDialog',
     'group::QGroupBox',
+    'scrollbar::QScrollBar',
+    'stack::QStackedWidget'
 ]
 
 
 def error_check(property):
     if property.count(':') != property.count(';'):
         property = property.split(';')
         for items in property:
```

### Comparing `clera-0.0.7/clera/widgets.py` & `clera-0.0.8/clera/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 
 from PySide6.QtGui import QIcon, QFont, QPixmap, QTextCursor
 from PySide6.QtWidgets import QPushButton, QLabel, QLineEdit, QRadioButton, QCheckBox, QTextEdit, QListWidget
 from PySide6.QtWidgets import QComboBox, QProgressBar, QSlider, QDial, QWidget, QScrollArea
 from PySide6.QtCore import QSize
 
-
 def Column(widgets):
     type = ELEM_TYPE_COLUMN
     return [type, widgets]
 
 
 def column(*args, **kwargs):
     return Column(*args, **kwargs)
@@ -20,15 +19,15 @@
          tooltip: None = None, statustip: None = None, shortcut: None = None):
     type = ELEM_TYPE_ITEM
     return [type, label, func, icon, tooltip, statustip, shortcut]
 
 
 def tab(layout: None = None, name: None = None, icon: None = None):
     type = ELEM_TYPE_TAB
-    x, layout = check_func(layout)
+    NotRequired, layout = check_func(layout)
     return [type, layout[0], name, icon]
 
 
 def option(value: any = '', icon: None = None):
     type = ELEM_TYPE_OPTION
     return [type, value, icon]
 
@@ -69,23 +68,29 @@
 ###########################################################################
 
 # ---------------ToolBarArea---------------------------------------------------------#
 
 
 def window_button(lyt, button_text, func, icon,
                   ID, disabled, default, sizepolicy, grid, grid_pos_x, grid_pos_y, checkable,
-                  checked, hidden, focus):
+                  checked, hidden, focus, icon_size, statustip, tooltip, shortcut):
 
     button = INIT_WIDGET(ID, QPushButton(button_text))
 
     set_widget(lyt, grid, button, grid_pos_x, grid_pos_y)
     set_size_policy(button, sizepolicy)
 
+    button.setStatusTip(statustip)
+    button.setToolTip(tooltip)
+    if shortcut != None:
+        button.setShortcut(shortcut)
+
     button.setIcon(QIcon(icon))
-    button.setEnabled(not disabled)
+    button.setIconSize(QSize(icon_size, icon_size))
+    button.setDisabled(disabled)
     button.setDefault(default)
     button.setCheckable(checkable)
     button.setChecked(checked)
     button.clicked.connect(func)
     button.setHidden(hidden)
 
     # button.setFocus(Qt.NoFocusReason)
@@ -95,15 +100,16 @@
     return button
 
 
 class Button:
     def __init__(self, value: any = '', func: None = None, icon: str = None, id: any = None,
                  disabled: bool = False, default: bool = False, grid: tuple = (None, None),
                  sizepolicy: tuple = (None, None), checkable: bool = False,
-                 checked: bool = False, hidden: bool = False, focus: bool = True):
+                 checked: bool = False, hidden: bool = False, focus: bool = True, 
+                 icon_size: int = 20, statustip: str = None, tooltip: str = None, shortcut: str = None):
         '''
         Button Widget
 
         :param value:
         :param func:
         :param icon:
         :param id:
@@ -111,19 +117,23 @@
         :param default:
         :param grid:
         :param sizepolicy:
         :param checkable:
         :param checked:
         :param hidden:
         :param focus:
+        :param icon_size:
+        :param statustip:
+        :param tooltip:
+        :param shortcut:
         '''
 
         elem_type = ELEM_TYPE_BUTTON
         self.rtn = [elem_type, str(value), func, icon, id,
-                    disabled, default, grid, sizepolicy, checkable, checked, hidden, focus]
+                    disabled, default, grid, sizepolicy, checkable, checked, hidden, focus, icon_size, statustip, tooltip, shortcut]
 
     def __call__(self):
         return self.rtn
 
 
 class button(Button):
     def __init__(self, *args, **kwargs):
@@ -469,34 +479,36 @@
 ###########################################################################
 
 # ------------------------------------------------------------------------#
 
 
 def window_textarea(lyt, ID, placeholder, hidden, alignment, value, disabled, readonly, text_changed,
                     selection_changed, undo_available, redo_available, maxlength, font, fontsize,
-                    sizepolicy, grid, grid_pos_x, grid_pos_y, tabWidth):
+                    sizepolicy, grid, grid_pos_x, grid_pos_y, tabwidth, wordwrap):
 
     textarea = INIT_WIDGET(ID, QTextEdit())
 
     set_widget(lyt, grid, textarea, grid_pos_x, grid_pos_y)
     set_size_policy(textarea, sizepolicy)
-
-    textarea.setHidden(hidden)
+    
+    #  set word wrap for textedit
+    if wordwrap:
+        textarea.setLineWrapMode(textarea.LineWrapMode.NoWrap)
 
     textarea.setDisabled(disabled)
     textarea.setReadOnly(readonly)
     textarea.setText(value)
     textarea.setPlaceholderText(placeholder)
 
     textarea.textChanged.connect(text_changed)
     textarea.selectionChanged.connect(selection_changed)
     textarea.undoAvailable.connect(undo_available)
     textarea.redoAvailable.connect(redo_available)
 
-    textarea.setTabStopDistance(tabWidth)
+    textarea.setTabStopDistance(tabwidth)
 
     if fontsize != None:
         textarea.setFont(QFont(font, fontsize))
     else:
         textarea.setFont(QFont(font))
 
     if maxlength != None:
@@ -511,15 +523,16 @@
 class Textarea:
     def __init__(self, id: any = None, placeholder: any = None,
                  hidden: bool = False, alignment: str = None, value: any = None,
                  disabled: bool = False, readonly: bool = False, text_changed: None = None,
                  selection_changed: None = None, undo_available: None = None,
                  redo_available: None = None, maxlength: int | None = None, font: str | None = None,
                  fontsize: int | None = None, sizepolicy: tuple = (None, None),
-                 grid: tuple = (None, None), tabWidth: int = DEFAULT_TAB_DISTANCE):
+                 grid: tuple = (None, None), tabwidth: int = DEFAULT_TAB_DISTANCE,
+                 wordwrap: bool = False):
         '''
         Textarea Widget
 
         :param id:
         :param placeholder
         :param hidden:
         :param alignment:
@@ -535,15 +548,16 @@
         :param fontsize:
         :param sizepolicy:
         :param grid:
         :param tabWidth:
         '''
         elem_type = ELEM_TYPE_TEXTAREA
         self.rtn = [elem_type, id, placeholder, hidden, alignment, value, disabled, readonly, text_changed,
-                    selection_changed, undo_available, redo_available, maxlength, font, fontsize, sizepolicy, grid, tabWidth]
+                    selection_changed, undo_available, redo_available, maxlength, font, fontsize, sizepolicy, grid,
+                    tabwidth, wordwrap]
 
     def __call__(self):
         return self.rtn
 
 
 class textarea(Textarea):
     def __init__(self, *args, **kwargs):
```

### Comparing `clera-0.0.7/setup.py` & `clera-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as readme:
     with codecs.open(os.path.join(here, "CHANGELOG.md"), encoding="utf-8") as changelog:
         LONG_DESCRIPTION = readme.read() + '\n\n\n' + changelog.read()
 
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Write Simple and Quick Python GUI Application'
 KEYWORDS = ['gui', 'clera', 'simple', 'simplegui', 'pyside', 'pyside6', 'python', 'easy']
 
 
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
@@ -30,12 +30,13 @@
     author="Erasmus A. Junior",
     author_email="eirasmx@pm.me",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     licence='GNU LGPLv3',
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
+    python_requires='>=3.7',
     install_requires=['PySide6'],
     keywords=KEYWORDS,
     classifiers=CLASSIFIERS,
     py_modules=['clera']
 )
```

