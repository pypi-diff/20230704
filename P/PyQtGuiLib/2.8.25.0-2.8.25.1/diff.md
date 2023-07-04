# Comparing `tmp/PyQtGuiLib-2.8.25.0.tar.gz` & `tmp/PyQtGuiLib-2.8.25.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtGuiLib-2.8.25.0.tar", last modified: Thu Jun 29 02:26:40 2023, max compression
+gzip compressed data, was "PyQtGuiLib-2.8.25.1.tar", last modified: Tue Jul  4 03:20:45 2023, max compression
```

## Comparing `PyQtGuiLib-2.8.25.0.tar` & `PyQtGuiLib-2.8.25.1.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.625626 PyQtGuiLib-2.8.25.0/
--rw-rw-rw-   0        0        0    11556 2023-04-28 01:43:54.000000 PyQtGuiLib-2.8.25.0/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.363983 PyQtGuiLib-2.8.25.0/Log/
--rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/Log/__init__.py
--rw-rw-rw-   0        0        0    10842 2023-05-02 01:07:20.000000 PyQtGuiLib-2.8.25.0/Log/developmentLog.py
--rw-rw-rw-   0        0        0    17970 2023-06-29 02:26:40.625626 PyQtGuiLib-2.8.25.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.364983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/
--rw-rw-rw-   0        0        0      108 2023-04-15 02:34:22.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.373984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/animation/
--rw-rw-rw-   0        0        0     6797 2023-05-08 00:28:14.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/animation/PropertyAnimation.py
--rw-rw-rw-   0        0        0      232 2023-04-25 06:49:49.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/animation/__init__.py
--rw-rw-rw-   0        0        0     7128 2023-06-29 02:04:28.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/animation/animation.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.384983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/
--rw-rw-rw-   0        0        0      840 2023-05-31 09:45:20.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/__init__.py
--rw-rw-rw-   0        0        0     5953 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/bubbleWidget.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.393983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/
--rw-rw-rw-   0        0        0      104 2023-06-09 02:31:14.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/__init__.py
--rw-rw-rw-   0        0        0     2675 2023-06-08 10:21:26.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/chatRoom.py
--rw-rw-rw-   0        0        0      553 2023-06-08 10:18:08.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/headImage.py
--rw-rw-rw-   0        0        0     8808 2023-06-12 01:20:37.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/message.py
--rw-rw-rw-   0        0        0     1560 2023-06-08 10:31:07.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/test.py
--rw-rw-rw-   0        0        0     4759 2023-06-12 02:18:02.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/transmitter.py
--rw-rw-rw-   0        0        0      530 2023-06-12 01:21:18.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/utility.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.396984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/comboBox/
--rw-rw-rw-   0        0        0      218 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/comboBox/__init__.py
--rw-rw-rw-   0        0        0     8171 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/comboBox/comboBox.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.400983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/comboBox/comboCheckBox/
--rw-rw-rw-   0        0        0      107 2023-04-25 08:09:32.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/comboBox/comboCheckBox/__init__.py
--rw-rw-rw-   0        0        0    21095 2023-04-25 08:15:03.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/comboBox/comboCheckBox/comboCheckBox.py
--rw-rw-rw-   0        0        0     2327 2023-04-25 08:09:33.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_message_box.py
--rw-rw-rw-   0        0        0    28106 2023-04-25 03:37:41.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_style.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.404986 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/drawers/
--rw-rw-rw-   0        0        0      107 2023-04-20 09:35:26.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/drawers/__init__.py
--rw-rw-rw-   0        0        0     3239 2023-05-02 01:02:42.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/drawers/drawer.py
--rw-rw-rw-   0        0        0     3886 2023-02-08 01:08:13.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/flowLayout.py
--rw-rw-rw-   0        0        0     5090 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/listWidget.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.409983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/logBrowser/
--rw-rw-rw-   0        0        0      107 2023-03-27 09:33:07.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/logBrowser/__init__.py
--rw-rw-rw-   0        0        0     1823 2023-03-31 09:04:34.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/logBrowser/loadLogTh.py
--rw-rw-rw-   0        0        0     5112 2023-04-03 02:45:06.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/logBrowser/logBrowser.py
--rw-rw-rw-   0        0        0      554 2023-03-31 09:29:33.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/logBrowser/logSizeTh.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.411984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/notice/
--rw-rw-rw-   0        0        0        0 2023-02-08 01:08:13.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/notice/__init__.py
--rw-rw-rw-   0        0        0     4822 2023-02-10 11:02:17.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/notice/notice.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.413983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/pager/
--rw-rw-rw-   0        0        0      106 2023-04-26 01:41:17.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/pager/__init__.py
--rw-rw-rw-   0        0        0     7939 2023-04-26 01:48:10.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/pager/pageCuttingButtonGroup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.418984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/
--rw-rw-rw-   0        0        0        0 2023-05-27 07:16:04.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/__init__.py
--rw-rw-rw-   0        0        0    10022 2023-05-11 04:23:31.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/colorHsv.py
--rw-rw-rw-   0        0        0     6492 2023-05-09 09:37:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/paletteFrame.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.424983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/paletteTools/
--rw-rw-rw-   0        0        0      107 2023-05-27 07:33:06.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/paletteTools/__init__.py
--rw-rw-rw-   0        0        0    40064 2023-05-31 08:49:44.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/paletteTools/area.py
--rw-rw-rw-   0        0        0    16131 2023-05-31 09:28:26.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/paletteTools/paletteToolUI.py
--rw-rw-rw-   0        0        0     4959 2023-05-31 09:45:57.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/paletteTools/palettetools.py
--rw-rw-rw-   0        0        0    63735 2023-05-31 08:49:44.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/palettetools.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.431983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/progressBar/
--rw-rw-rw-   0        0        0      325 2023-04-13 08:34:31.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/progressBar/__init__.py
--rw-rw-rw-   0        0        0     5602 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/progressBar/circularBar.py
--rw-rw-rw-   0        0        0     6158 2023-04-28 09:40:27.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/progressBar/circularProgressBar.py
--rw-rw-rw-   0        0        0     3943 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/progressBar/gradientBar.py
--rw-rw-rw-   0        0        0     4365 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/progressBar/loadBar.py
--rw-rw-rw-   0        0        0     6734 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/progressBar/waterBar.py
--rw-rw-rw-   0        0        0     5092 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/pullOver.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.434984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/resolver/
--rw-rw-rw-   0        0        0       59 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/resolver/__init__.py
--rw-rw-rw-   0        0        0      674 2023-05-05 03:11:46.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/resolver/controls.py
--rw-rw-rw-   0        0        0     7628 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/rollWidget.py
--rw-rw-rw-   0        0        0    10547 2023-04-15 10:18:10.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/slideShow.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.436983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/slider/
--rw-rw-rw-   0        0        0        0 2023-02-14 00:37:29.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/slider/__init__.py
--rw-rw-rw-   0        0        0     8596 2023-04-13 07:56:58.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/slider/slider.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.439984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/switchButtons/
--rw-rw-rw-   0        0        0       63 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/switchButtons/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-02-23 01:29:46.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/switchButtons/swButton.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.442984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/table/
--rw-rw-rw-   0        0        0      107 2023-04-28 09:24:43.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/table/__init__.py
--rw-rw-rw-   0        0        0     1442 2023-05-02 00:56:46.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/table/table.py
--rw-rw-rw-   0        0        0     2743 2023-03-06 05:54:08.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/toolBox.py
--rw-rw-rw-   0        0        0     5588 2023-03-14 01:24:55.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/toolList.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.449984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/
--rw-rw-rw-   0        0        0    11338 2023-04-13 05:09:14.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/WidgetABC.py
--rw-rw-rw-   0        0        0      260 2023-02-09 10:20:35.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/__init__.py
--rw-rw-rw-   0        0        0     3995 2023-02-10 07:29:38.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/borderlessMainWindow.py
--rw-rw-rw-   0        0        0      303 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/borderlessWidget.py
--rw-rw-rw-   0        0        0     4935 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/statusBar.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.453983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/tets/
--rw-rw-rw-   0        0        0      375 2023-02-27 10:18:30.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/tets/1.py
--rw-rw-rw-   0        0        0     3504 2023-02-27 00:36:50.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/tets/2.py
--rw-rw-rw-   0        0        0        0 2023-02-24 00:57:42.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/tets/__init__.py
--rw-rw-rw-   0        0        0    17840 2023-02-10 03:56:26.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/titleBar.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.459983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.468984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/Qt/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/Qt/__init__.py
--rw-rw-rw-   0        0        0     6038 2023-04-26 01:43:34.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/Qt/qt.py
--rw-rw-rw-   0        0        0      534 2023-04-25 05:53:49.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/Qt/qtCore.py
--rw-rw-rw-   0        0        0      564 2023-05-13 06:17:36.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/Qt/qtGui.py
--rw-rw-rw-   0        0        0      509 2023-02-09 08:33:46.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/Qt/qtSip.py
--rw-rw-rw-   0        0        0      505 2023-02-13 08:07:57.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/Qt/qtUic.py
--rw-rw-rw-   0        0        0      460 2023-04-25 04:13:46.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/Qt/qtWidgets.py
--rw-rw-rw-   0        0        0      803 2023-05-13 06:37:57.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/__init__.py
--rw-rw-rw-   0        0        0     6406 2023-04-25 05:54:19.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/customStyle.py
--rw-rw-rw-   0        0        0      262 2023-02-10 01:34:45.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/error.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.470984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/py/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/py/__init__.py
--rw-rw-rw-   0        0        0      103 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/py/common.py
--rw-rw-rw-   0        0        0     3602 2023-06-02 06:14:32.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/utility.py
--rw-rw-rw-   0        0        0      403 2023-05-12 02:40:17.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/versions.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.473984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/layoutDeformation/
--rw-rw-rw-   0        0        0      106 2023-03-04 03:38:59.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/layoutDeformation/__init__.py
--rw-rw-rw-   0        0        0     4425 2023-03-07 08:03:39.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/layoutDeformation/test.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.475983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/particle/
--rw-rw-rw-   0        0        0        0 2023-06-16 08:38:55.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/particle/__init__.py
--rw-rw-rw-   0        0        0     3907 2023-06-16 10:35:31.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/particle/particle.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.479002 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/
--rw-rw-rw-   0        0        0      364 2023-04-25 07:58:50.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.484984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/builtStyleDesigner/
--rw-rw-rw-   0        0        0      105 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/builtStyleDesigner/__init__.py
--rw-rw-rw-   0        0        0     7168 2023-02-24 00:57:42.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py
--rw-rw-rw-   0        0        0     5062 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py
--rw-rw-rw-   0        0        0     1237 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.486983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/buttons/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/buttons/__init__.py
--rw-rw-rw-   0        0        0      620 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/buttons/buttonStyle.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.489985 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/guiLibStyle/
--rw-rw-rw-   0        0        0     1456 2023-05-12 10:28:01.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/guiLibStyle/__init__.py
--rw-rw-rw-   0        0        0     1527 2023-05-12 10:34:14.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/guiLibStyle/libStyle.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.493983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/
--rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.497984 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/drak/
--rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/drak/__init__.py
--rw-rw-rw-   0        0        0      187 2023-03-29 08:26:42.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/drak/config.py
--rw-rw-rw-   0        0        0    11537 2023-03-30 09:13:08.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/drak/qssDrak.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.500983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/image/
--rw-rw-rw-   0        0        0      107 2023-03-29 03:26:49.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/image/__init__.py
--rw-rw-rw-   0        0        0    29060 2023-03-30 10:20:11.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/image/image_rc.py
--rw-rw-rw-   0        0        0      300 2023-03-30 10:19:06.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/image/qssFile.py
--rw-rw-rw-   0        0        0    20518 2023-03-30 10:20:35.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/qssFile.py
--rw-rw-rw-   0        0        0     6221 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/test.py
--rw-rw-rw-   0        0        0    10615 2023-02-09 08:32:36.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/skinABC.py
--rw-rw-rw-   0        0        0     8593 2023-04-26 10:22:16.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/styleAnalysis.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.503983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/superPainter/
--rw-rw-rw-   0        0        0      107 2023-03-18 07:49:47.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/superPainter/__init__.py
--rw-rw-rw-   0        0        0    15520 2023-06-25 10:29:13.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/superPainter/superPainter.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.504987 PyQtGuiLib-2.8.25.0/PyQtGuiLib/templateWindow/
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.507983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/templateWindow/UI/
--rw-rw-rw-   0        0        0      193 2023-04-11 03:59:36.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/templateWindow/UI/__init__.py
--rw-rw-rw-   0        0        0     5539 2023-04-13 05:40:13.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.509983 PyQtGuiLib-2.8.25.0/PyQtGuiLib/templateWindow/Window/
--rw-rw-rw-   0        0        0      107 2023-04-10 09:41:12.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/templateWindow/Window/__init__.py
--rw-rw-rw-   0        0        0     9497 2023-04-15 10:09:10.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py
--rw-rw-rw-   0        0        0      189 2023-04-11 04:44:35.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib/templateWindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.369984 PyQtGuiLib-2.8.25.0/PyQtGuiLib.egg-info/
--rw-rw-rw-   0        0        0    17970 2023-06-29 02:26:40.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7340 2023-06-29 02:26:40.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 02:26:40.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-29 02:26:40.000000 PyQtGuiLib-2.8.25.0/PyQtGuiLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17541 2023-05-15 00:32:06.000000 PyQtGuiLib-2.8.25.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.519985 PyQtGuiLib-2.8.25.0/abandonCase/
--rw-rw-rw-   0        0        0      108 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.524983 PyQtGuiLib-2.8.25.0/abandonCase/acrylic/
--rw-rw-rw-   0        0        0       37 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/acrylic/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/acrylic/acrylicWidget.py
--rw-rw-rw-   0        0        0     1550 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/acrylic/cstruct.py
--rw-rw-rw-   0        0        0     2183 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/acrylic/windowEffect.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.533014 PyQtGuiLib-2.8.25.0/abandonCase/animation/
--rw-rw-rw-   0        0        0      107 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.25.0/abandonCase/animation/__init__.py
--rw-rw-rw-   0        0        0    21249 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.25.0/abandonCase/animation/animation.py
--rw-rw-rw-   0        0        0     2792 2023-03-28 09:06:54.000000 PyQtGuiLib-2.8.25.0/abandonCase/animation/animationDrawType.py
--rw-rw-rw-   0        0        0    11526 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.25.0/abandonCase/animation/animationFactory.py
--rw-rw-rw-   0        0        0     1636 2023-03-20 04:02:29.000000 PyQtGuiLib-2.8.25.0/abandonCase/animation/animationLayout.py
--rw-rw-rw-   0        0        0     2292 2023-03-15 01:17:54.000000 PyQtGuiLib-2.8.25.0/abandonCase/animation/customAniTest.py
--rw-rw-rw-   0        0        0     9981 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/bubbleWidget.py
--rw-rw-rw-   0        0        0     3620 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/bubbleWidget_case.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.539017 PyQtGuiLib-2.8.25.0/abandonCase/linker/
--rw-rw-rw-   0        0        0      106 2023-02-20 02:36:19.000000 PyQtGuiLib-2.8.25.0/abandonCase/linker/__init__.py
--rw-rw-rw-   0        0        0    26952 2023-02-23 01:15:37.000000 PyQtGuiLib-2.8.25.0/abandonCase/linker/component.py
--rw-rw-rw-   0        0        0     8822 2023-03-13 01:50:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/linker/controlType.py
--rw-rw-rw-   0        0        0    11488 2023-04-25 08:02:33.000000 PyQtGuiLib-2.8.25.0/abandonCase/linker/styleLinker.py
--rw-rw-rw-   0        0        0     1444 2023-02-22 03:17:40.000000 PyQtGuiLib-2.8.25.0/abandonCase/linker/styleLinkerUi.py
--rw-rw-rw-   0        0        0     1411 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/nodeBar.py
--rw-rw-rw-   0        0        0     9873 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/slideShow.py
--rw-rw-rw-   0        0        0     7801 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/slideShow2.py
--rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/spaceWidget.py
--rw-rw-rw-   0        0        0    17813 2023-04-25 08:21:59.000000 PyQtGuiLib-2.8.25.0/abandonCase/superPainter.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.549984 PyQtGuiLib-2.8.25.0/abandonCase/widgets/
--rw-rw-rw-   0        0        0      110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/widgets/__init__.py
--rw-rw-rw-   0        0        0     1389 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/widgets/borderlessFrame.py
--rw-rw-rw-   0        0        0     1962 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/widgets/borderlessMainWindow.py
--rw-rw-rw-   0        0        0     1441 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/widgets/borderlessStackedWidget.py
--rw-rw-rw-   0        0        0     1402 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/widgets/borderlessWidget.py
--rw-rw-rw-   0        0        0    10095 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/widgets/borderlessWidgetABC.py
--rw-rw-rw-   0        0        0     5034 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/widgets/statusBar.py
--rw-rw-rw-   0        0        0    17577 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/abandonCase/widgets/titleBar.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.551983 PyQtGuiLib-2.8.25.0/auxiliaryMeans/
--rw-rw-rw-   0        0        0        0 2023-04-17 01:54:33.000000 PyQtGuiLib-2.8.25.0/auxiliaryMeans/__init__.py
--rw-rw-rw-   0        0        0     5067 2023-04-17 02:06:33.000000 PyQtGuiLib-2.8.25.0/auxiliaryMeans/toolNewProject.py
--rw-rw-rw-   0        0        0       42 2023-06-29 02:26:40.626596 PyQtGuiLib-2.8.25.0/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-06-29 02:23:19.000000 PyQtGuiLib-2.8.25.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.587984 PyQtGuiLib-2.8.25.0/tests/
--rw-rw-rw-   0        0        0      107 2023-06-26 10:28:21.000000 PyQtGuiLib-2.8.25.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.593595 PyQtGuiLib-2.8.25.0/tests/test_Animation/
--rw-rw-rw-   0        0        0     1990 2023-06-14 07:54:17.000000 PyQtGuiLib-2.8.25.0/tests/test_Animation/1.py
--rw-rw-rw-   0        0        0      606 2023-03-15 09:52:36.000000 PyQtGuiLib-2.8.25.0/tests/test_Animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.596595 PyQtGuiLib-2.8.25.0/tests/test_Animation/test_ani/
--rw-rw-rw-   0        0        0     1589 2023-04-20 01:28:51.000000 PyQtGuiLib-2.8.25.0/tests/test_Animation/test_ani/1.py
--rw-rw-rw-   0        0        0      107 2023-03-27 05:53:58.000000 PyQtGuiLib-2.8.25.0/tests/test_Animation/test_ani/__init__.py
--rw-rw-rw-   0        0        0     1351 2023-06-29 02:03:17.000000 PyQtGuiLib-2.8.25.0/tests/test_Animation/test_animation.py
--rw-rw-rw-   0        0        0     1728 2023-06-25 10:32:05.000000 PyQtGuiLib-2.8.25.0/tests/test_Animation/test_p_ani.py
--rw-rw-rw-   0        0        0     1541 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_BubbleWidget.py
--rw-rw-rw-   0        0        0     2738 2023-04-13 08:35:22.000000 PyQtGuiLib-2.8.25.0/tests/test_CircularProgressBar.py
--rw-rw-rw-   0        0        0     1288 2023-04-25 08:18:48.000000 PyQtGuiLib-2.8.25.0/tests/test_ComboCheckBox.py
--rw-rw-rw-   0        0        0     1596 2023-04-19 07:50:47.000000 PyQtGuiLib-2.8.25.0/tests/test_Notice.py
--rw-rw-rw-   0        0        0     1829 2023-04-26 01:49:56.000000 PyQtGuiLib-2.8.25.0/tests/test_PageCuttingButtonGroup.py
--rw-rw-rw-   0        0        0     1898 2023-05-31 09:45:31.000000 PyQtGuiLib-2.8.25.0/tests/test_PaletteTools.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.607627 PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/
--rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-04-06 02:24:28.000000 PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg1.py
--rw-rw-rw-   0        0        0     2306 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg2.py
--rw-rw-rw-   0        0        0     1891 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg3.py
--rw-rw-rw-   0        0        0     2110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg4.py
--rw-rw-rw-   0        0        0     2519 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg5.py
--rw-rw-rw-   0        0        0     1881 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg6.py
--rw-rw-rw-   0        0        0     2617 2023-03-22 05:45:33.000000 PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg7.py
--rw-rw-rw-   0        0        0     2042 2023-04-06 03:41:23.000000 PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/test.py
--rw-rw-rw-   0        0        0     2275 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis.py
--rw-rw-rw-   0        0        0     2605 2023-04-13 09:27:46.000000 PyQtGuiLib-2.8.25.0/tests/test_SlideShow.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.616596 PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/
--rw-rw-rw-   0        0        0      871 2023-04-20 09:50:12.000000 PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/1.py
--rw-rw-rw-   0        0        0      106 2023-04-07 09:06:55.000000 PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/__init__.py
--rw-rw-rw-   0        0        0     1568 2023-04-07 09:19:44.000000 PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/eg1.py
--rw-rw-rw-   0        0        0     2143 2023-04-10 00:27:52.000000 PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/eg2.py
--rw-rw-rw-   0        0        0     1648 2023-04-07 09:39:03.000000 PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/eg3.py
--rw-rw-rw-   0        0        0     3527 2023-04-19 03:20:23.000000 PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/eg4.py
--rw-rw-rw-   0        0        0     1531 2023-05-11 09:36:30.000000 PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/test.py
--rw-rw-rw-   0        0        0     2465 2023-04-13 01:50:22.000000 PyQtGuiLib-2.8.25.0/tests/test_barset.py
--rw-rw-rw-   0        0        0     1648 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_circularBar.py
--rw-rw-rw-   0        0        0     1723 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_colorPalette.py
--rw-rw-rw-   0        0        0     1979 2023-05-02 10:29:36.000000 PyQtGuiLib-2.8.25.0/tests/test_drawer.py
--rw-rw-rw-   0        0        0      289 2023-05-05 10:31:26.000000 PyQtGuiLib-2.8.25.0/tests/test_dumpStructure.py
--rw-rw-rw-   0        0        0     1315 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_flowLayot.py
--rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_gradientBar.py
--rw-rw-rw-   0        0        0     1865 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_listWidget.py
--rw-rw-rw-   0        0        0     1386 2023-05-08 00:28:14.000000 PyQtGuiLib-2.8.25.0/tests/test_loadbar.py
--rw-rw-rw-   0        0        0     2498 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_no_border.py
--rw-rw-rw-   0        0        0     1365 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_no_border_pullOver.py
--rw-rw-rw-   0        0        0     1022 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_pullOverWidget.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.618595 PyQtGuiLib-2.8.25.0/tests/test_qssFile/
--rw-rw-rw-   0        0        0      107 2023-03-29 06:12:59.000000 PyQtGuiLib-2.8.25.0/tests/test_qssFile/__init__.py
--rw-rw-rw-   0        0        0      584 2023-04-04 06:18:57.000000 PyQtGuiLib-2.8.25.0/tests/test_qssFile/test.py
--rw-rw-rw-   0        0        0     1444 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_rollWidget.py
--rw-rw-rw-   0        0        0     1666 2023-05-29 10:31:16.000000 PyQtGuiLib-2.8.25.0/tests/test_slider.py
--rw-rw-rw-   0        0        0     1778 2023-04-13 01:45:35.000000 PyQtGuiLib-2.8.25.0/tests/test_statusBar.py
--rw-rw-rw-   0        0        0     1014 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_styles.py
--rw-rw-rw-   0        0        0     1122 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_switchButton.py
--rw-rw-rw-   0        0        0      543 2023-04-17 01:43:36.000000 PyQtGuiLib-2.8.25.0/tests/test_template.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.620595 PyQtGuiLib-2.8.25.0/tests/test_templateWindow/
--rw-rw-rw-   0        0        0      107 2023-04-11 04:44:35.000000 PyQtGuiLib-2.8.25.0/tests/test_templateWindow/__init__.py
--rw-rw-rw-   0        0        0     2718 2023-04-13 10:00:15.000000 PyQtGuiLib-2.8.25.0/tests/test_templateWindow/test_listTemplateWindow.py
--rw-rw-rw-   0        0        0     1356 2023-03-13 08:03:45.000000 PyQtGuiLib-2.8.25.0/tests/test_toolList.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:26:40.623597 PyQtGuiLib-2.8.25.0/tests/test_uic/
--rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_uic/__init__.py
--rw-rw-rw-   0        0        0      377 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_uic/test_uic.py
--rw-rw-rw-   0        0        0     1547 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.0/tests/test_waterBar.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.568538 PyQtGuiLib-2.8.25.1/
+-rw-rw-rw-   0        0        0    11556 2023-04-28 01:43:54.000000 PyQtGuiLib-2.8.25.1/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.316892 PyQtGuiLib-2.8.25.1/Log/
+-rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/Log/__init__.py
+-rw-rw-rw-   0        0        0    10842 2023-05-02 01:07:20.000000 PyQtGuiLib-2.8.25.1/Log/developmentLog.py
+-rw-rw-rw-   0        0        0    17970 2023-07-04 03:20:45.568538 PyQtGuiLib-2.8.25.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.318891 PyQtGuiLib-2.8.25.1/PyQtGuiLib/
+-rw-rw-rw-   0        0        0      108 2023-04-15 02:34:22.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.328538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/animation/
+-rw-rw-rw-   0        0        0     6797 2023-05-08 00:28:14.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/animation/PropertyAnimation.py
+-rw-rw-rw-   0        0        0      232 2023-04-25 06:49:49.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/animation/__init__.py
+-rw-rw-rw-   0        0        0     7128 2023-06-29 02:04:28.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/animation/animation.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.340538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/
+-rw-rw-rw-   0        0        0      840 2023-05-31 09:45:20.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/__init__.py
+-rw-rw-rw-   0        0        0     6097 2023-07-04 03:18:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/bubbleWidget.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.348538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/
+-rw-rw-rw-   0        0        0      104 2023-06-09 02:31:14.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/__init__.py
+-rw-rw-rw-   0        0        0     2675 2023-06-08 10:21:26.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/chatRoom.py
+-rw-rw-rw-   0        0        0      553 2023-06-08 10:18:08.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/headImage.py
+-rw-rw-rw-   0        0        0     8808 2023-06-12 01:20:37.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/message.py
+-rw-rw-rw-   0        0        0     1560 2023-06-08 10:31:07.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/test.py
+-rw-rw-rw-   0        0        0     4759 2023-06-12 02:18:02.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/transmitter.py
+-rw-rw-rw-   0        0        0      530 2023-06-12 01:21:18.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/utility.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.351539 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/comboBox/
+-rw-rw-rw-   0        0        0      218 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/comboBox/__init__.py
+-rw-rw-rw-   0        0        0     8171 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/comboBox/comboBox.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.356538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/comboBox/comboCheckBox/
+-rw-rw-rw-   0        0        0      107 2023-04-25 08:09:32.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/comboBox/comboCheckBox/__init__.py
+-rw-rw-rw-   0        0        0    21095 2023-04-25 08:15:03.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/comboBox/comboCheckBox/comboCheckBox.py
+-rw-rw-rw-   0        0        0     2327 2023-04-25 08:09:33.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/comboBox/comboCheckBox/py_message_box.py
+-rw-rw-rw-   0        0        0    28106 2023-04-25 03:37:41.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/comboBox/comboCheckBox/py_style.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.358538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/drawers/
+-rw-rw-rw-   0        0        0      107 2023-04-20 09:35:26.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/drawers/__init__.py
+-rw-rw-rw-   0        0        0     3239 2023-05-02 01:02:42.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/drawers/drawer.py
+-rw-rw-rw-   0        0        0     3886 2023-02-08 01:08:13.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/flowLayout.py
+-rw-rw-rw-   0        0        0     5090 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/listWidget.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.363538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/logBrowser/
+-rw-rw-rw-   0        0        0      107 2023-03-27 09:33:07.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/logBrowser/__init__.py
+-rw-rw-rw-   0        0        0     1823 2023-03-31 09:04:34.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/logBrowser/loadLogTh.py
+-rw-rw-rw-   0        0        0     5112 2023-04-03 02:45:06.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/logBrowser/logBrowser.py
+-rw-rw-rw-   0        0        0      554 2023-03-31 09:29:33.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/logBrowser/logSizeTh.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.365538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/notice/
+-rw-rw-rw-   0        0        0        0 2023-02-08 01:08:13.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/notice/__init__.py
+-rw-rw-rw-   0        0        0     4822 2023-02-10 11:02:17.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/notice/notice.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.367538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/pager/
+-rw-rw-rw-   0        0        0      106 2023-04-26 01:41:17.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/pager/__init__.py
+-rw-rw-rw-   0        0        0     7939 2023-04-26 01:48:10.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/pager/pageCuttingButtonGroup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.373541 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/
+-rw-rw-rw-   0        0        0        0 2023-05-27 07:16:04.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/__init__.py
+-rw-rw-rw-   0        0        0    10022 2023-05-11 04:23:31.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/colorHsv.py
+-rw-rw-rw-   0        0        0     6492 2023-05-09 09:37:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/paletteFrame.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.378538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/paletteTools/
+-rw-rw-rw-   0        0        0      107 2023-05-27 07:33:06.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/paletteTools/__init__.py
+-rw-rw-rw-   0        0        0    40064 2023-05-31 08:49:44.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/paletteTools/area.py
+-rw-rw-rw-   0        0        0    16131 2023-05-31 09:28:26.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/paletteTools/paletteToolUI.py
+-rw-rw-rw-   0        0        0     4959 2023-05-31 09:45:57.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/paletteTools/palettetools.py
+-rw-rw-rw-   0        0        0    63735 2023-07-04 02:05:16.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/palettetools.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.385538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/progressBar/
+-rw-rw-rw-   0        0        0      325 2023-04-13 08:34:31.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/progressBar/__init__.py
+-rw-rw-rw-   0        0        0     5669 2023-07-04 03:12:03.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/progressBar/circularBar.py
+-rw-rw-rw-   0        0        0     6158 2023-04-28 09:40:27.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/progressBar/circularProgressBar.py
+-rw-rw-rw-   0        0        0     3943 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/progressBar/gradientBar.py
+-rw-rw-rw-   0        0        0     4433 2023-07-04 03:12:03.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/progressBar/loadBar.py
+-rw-rw-rw-   0        0        0     6734 2023-02-10 01:10:59.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/progressBar/waterBar.py
+-rw-rw-rw-   0        0        0     5092 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/pullOver.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.387538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/resolver/
+-rw-rw-rw-   0        0        0       59 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/resolver/__init__.py
+-rw-rw-rw-   0        0        0      674 2023-05-05 03:11:46.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/resolver/controls.py
+-rw-rw-rw-   0        0        0     7628 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/rollWidget.py
+-rw-rw-rw-   0        0        0    10547 2023-04-15 10:18:10.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/slideShow.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.390539 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/slider/
+-rw-rw-rw-   0        0        0        0 2023-02-14 00:37:29.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/slider/__init__.py
+-rw-rw-rw-   0        0        0     8596 2023-04-13 07:56:58.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/slider/slider.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.392538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/switchButtons/
+-rw-rw-rw-   0        0        0       63 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/switchButtons/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-02-23 01:29:46.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/switchButtons/swButton.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.394538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/table/
+-rw-rw-rw-   0        0        0      107 2023-04-28 09:24:43.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/table/__init__.py
+-rw-rw-rw-   0        0        0     1442 2023-05-02 00:56:46.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/table/table.py
+-rw-rw-rw-   0        0        0     2743 2023-03-06 05:54:08.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/toolBox.py
+-rw-rw-rw-   0        0        0     5588 2023-03-14 01:24:55.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/toolList.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.402538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/
+-rw-rw-rw-   0        0        0    11338 2023-04-13 05:09:14.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/WidgetABC.py
+-rw-rw-rw-   0        0        0      260 2023-02-09 10:20:35.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3995 2023-02-10 07:29:38.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/borderlessMainWindow.py
+-rw-rw-rw-   0        0        0      303 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/borderlessWidget.py
+-rw-rw-rw-   0        0        0     4935 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/statusBar.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.406538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/tets/
+-rw-rw-rw-   0        0        0      375 2023-02-27 10:18:30.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/tets/1.py
+-rw-rw-rw-   0        0        0     3504 2023-02-27 00:36:50.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/tets/2.py
+-rw-rw-rw-   0        0        0        0 2023-02-24 00:57:42.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/tets/__init__.py
+-rw-rw-rw-   0        0        0    17840 2023-02-10 03:56:26.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/titleBar.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.411538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.420540 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/Qt/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/Qt/__init__.py
+-rw-rw-rw-   0        0        0     6038 2023-04-26 01:43:34.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/Qt/qt.py
+-rw-rw-rw-   0        0        0      534 2023-04-25 05:53:49.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/Qt/qtCore.py
+-rw-rw-rw-   0        0        0      564 2023-05-13 06:17:36.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/Qt/qtGui.py
+-rw-rw-rw-   0        0        0      509 2023-02-09 08:33:46.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/Qt/qtSip.py
+-rw-rw-rw-   0        0        0      505 2023-02-13 08:07:57.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/Qt/qtUic.py
+-rw-rw-rw-   0        0        0      460 2023-04-25 04:13:46.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/Qt/qtWidgets.py
+-rw-rw-rw-   0        0        0      803 2023-05-13 06:37:57.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/__init__.py
+-rw-rw-rw-   0        0        0     6406 2023-04-25 05:54:19.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/customStyle.py
+-rw-rw-rw-   0        0        0      262 2023-02-10 01:34:45.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/error.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.422538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/py/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/py/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/py/common.py
+-rw-rw-rw-   0        0        0     3602 2023-06-02 06:14:32.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/utility.py
+-rw-rw-rw-   0        0        0      403 2023-05-12 02:40:17.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/versions.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.424552 PyQtGuiLib-2.8.25.1/PyQtGuiLib/layoutDeformation/
+-rw-rw-rw-   0        0        0      106 2023-03-04 03:38:59.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/layoutDeformation/__init__.py
+-rw-rw-rw-   0        0        0     4425 2023-03-07 08:03:39.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/layoutDeformation/test.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.427539 PyQtGuiLib-2.8.25.1/PyQtGuiLib/particle/
+-rw-rw-rw-   0        0        0        0 2023-06-16 08:38:55.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/particle/__init__.py
+-rw-rw-rw-   0        0        0     3907 2023-06-16 10:35:31.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/particle/particle.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.430538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/
+-rw-rw-rw-   0        0        0      364 2023-04-25 07:58:50.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.435538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/builtStyleDesigner/
+-rw-rw-rw-   0        0        0      105 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/builtStyleDesigner/__init__.py
+-rw-rw-rw-   0        0        0     7168 2023-02-24 00:57:42.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py
+-rw-rw-rw-   0        0        0     5062 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py
+-rw-rw-rw-   0        0        0     1237 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.437538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/buttons/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/buttons/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-02-01 01:34:23.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/buttons/buttonStyle.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.440538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/guiLibStyle/
+-rw-rw-rw-   0        0        0     1456 2023-05-12 10:28:01.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/guiLibStyle/__init__.py
+-rw-rw-rw-   0        0        0     1527 2023-05-12 10:34:14.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/guiLibStyle/libStyle.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.443538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/
+-rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.446538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/drak/
+-rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/drak/__init__.py
+-rw-rw-rw-   0        0        0      187 2023-03-29 08:26:42.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/drak/config.py
+-rw-rw-rw-   0        0        0    11537 2023-03-30 09:13:08.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/drak/qssDrak.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.450539 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/image/
+-rw-rw-rw-   0        0        0      107 2023-03-29 03:26:49.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/image/__init__.py
+-rw-rw-rw-   0        0        0    29060 2023-03-30 10:20:11.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/image/image_rc.py
+-rw-rw-rw-   0        0        0      300 2023-03-30 10:19:06.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/image/qssFile.py
+-rw-rw-rw-   0        0        0    20518 2023-03-30 10:20:35.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/qssFile.py
+-rw-rw-rw-   0        0        0     6221 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/test.py
+-rw-rw-rw-   0        0        0    10615 2023-02-09 08:32:36.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/skinABC.py
+-rw-rw-rw-   0        0        0     8593 2023-04-26 10:22:16.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/styleAnalysis.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.453539 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/superPainter/
+-rw-rw-rw-   0        0        0      107 2023-03-18 07:49:47.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/superPainter/__init__.py
+-rw-rw-rw-   0        0        0    15520 2023-06-25 10:29:13.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/superPainter/superPainter.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.454538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/templateWindow/
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.456538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/templateWindow/UI/
+-rw-rw-rw-   0        0        0      193 2023-04-11 03:59:36.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/templateWindow/UI/__init__.py
+-rw-rw-rw-   0        0        0     5539 2023-04-13 05:40:13.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.459538 PyQtGuiLib-2.8.25.1/PyQtGuiLib/templateWindow/Window/
+-rw-rw-rw-   0        0        0      107 2023-04-10 09:41:12.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/templateWindow/Window/__init__.py
+-rw-rw-rw-   0        0        0     9497 2023-04-15 10:09:10.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py
+-rw-rw-rw-   0        0        0      189 2023-04-11 04:44:35.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib/templateWindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.324531 PyQtGuiLib-2.8.25.1/PyQtGuiLib.egg-info/
+-rw-rw-rw-   0        0        0    17970 2023-07-04 03:20:45.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7340 2023-07-04 03:20:45.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 03:20:45.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-04 03:20:45.000000 PyQtGuiLib-2.8.25.1/PyQtGuiLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17541 2023-05-15 00:32:06.000000 PyQtGuiLib-2.8.25.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.469539 PyQtGuiLib-2.8.25.1/abandonCase/
+-rw-rw-rw-   0        0        0      108 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.473538 PyQtGuiLib-2.8.25.1/abandonCase/acrylic/
+-rw-rw-rw-   0        0        0       37 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/acrylic/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/acrylic/acrylicWidget.py
+-rw-rw-rw-   0        0        0     1550 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/acrylic/cstruct.py
+-rw-rw-rw-   0        0        0     2183 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/acrylic/windowEffect.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.480538 PyQtGuiLib-2.8.25.1/abandonCase/animation/
+-rw-rw-rw-   0        0        0      107 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.25.1/abandonCase/animation/__init__.py
+-rw-rw-rw-   0        0        0    21249 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.25.1/abandonCase/animation/animation.py
+-rw-rw-rw-   0        0        0     2792 2023-03-28 09:06:54.000000 PyQtGuiLib-2.8.25.1/abandonCase/animation/animationDrawType.py
+-rw-rw-rw-   0        0        0    11526 2023-04-20 09:24:50.000000 PyQtGuiLib-2.8.25.1/abandonCase/animation/animationFactory.py
+-rw-rw-rw-   0        0        0     1636 2023-03-20 04:02:29.000000 PyQtGuiLib-2.8.25.1/abandonCase/animation/animationLayout.py
+-rw-rw-rw-   0        0        0     2292 2023-03-15 01:17:54.000000 PyQtGuiLib-2.8.25.1/abandonCase/animation/customAniTest.py
+-rw-rw-rw-   0        0        0     9981 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/bubbleWidget.py
+-rw-rw-rw-   0        0        0     3620 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/bubbleWidget_case.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.486538 PyQtGuiLib-2.8.25.1/abandonCase/linker/
+-rw-rw-rw-   0        0        0      106 2023-02-20 02:36:19.000000 PyQtGuiLib-2.8.25.1/abandonCase/linker/__init__.py
+-rw-rw-rw-   0        0        0    26952 2023-02-23 01:15:37.000000 PyQtGuiLib-2.8.25.1/abandonCase/linker/component.py
+-rw-rw-rw-   0        0        0     8822 2023-03-13 01:50:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/linker/controlType.py
+-rw-rw-rw-   0        0        0    11488 2023-04-25 08:02:33.000000 PyQtGuiLib-2.8.25.1/abandonCase/linker/styleLinker.py
+-rw-rw-rw-   0        0        0     1444 2023-02-22 03:17:40.000000 PyQtGuiLib-2.8.25.1/abandonCase/linker/styleLinkerUi.py
+-rw-rw-rw-   0        0        0     1411 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/nodeBar.py
+-rw-rw-rw-   0        0        0     9873 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/slideShow.py
+-rw-rw-rw-   0        0        0     7801 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/slideShow2.py
+-rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/spaceWidget.py
+-rw-rw-rw-   0        0        0    17813 2023-04-25 08:21:59.000000 PyQtGuiLib-2.8.25.1/abandonCase/superPainter.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.496538 PyQtGuiLib-2.8.25.1/abandonCase/widgets/
+-rw-rw-rw-   0        0        0      110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1389 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/widgets/borderlessFrame.py
+-rw-rw-rw-   0        0        0     1962 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/widgets/borderlessMainWindow.py
+-rw-rw-rw-   0        0        0     1441 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/widgets/borderlessStackedWidget.py
+-rw-rw-rw-   0        0        0     1402 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/widgets/borderlessWidget.py
+-rw-rw-rw-   0        0        0    10095 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/widgets/borderlessWidgetABC.py
+-rw-rw-rw-   0        0        0     5034 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/widgets/statusBar.py
+-rw-rw-rw-   0        0        0    17577 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/abandonCase/widgets/titleBar.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.498538 PyQtGuiLib-2.8.25.1/auxiliaryMeans/
+-rw-rw-rw-   0        0        0        0 2023-04-17 01:54:33.000000 PyQtGuiLib-2.8.25.1/auxiliaryMeans/__init__.py
+-rw-rw-rw-   0        0        0     5067 2023-04-17 02:06:33.000000 PyQtGuiLib-2.8.25.1/auxiliaryMeans/toolNewProject.py
+-rw-rw-rw-   0        0        0       42 2023-07-04 03:20:45.569538 PyQtGuiLib-2.8.25.1/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-07-04 03:17:22.000000 PyQtGuiLib-2.8.25.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.533540 PyQtGuiLib-2.8.25.1/tests/
+-rw-rw-rw-   0        0        0      107 2023-06-26 10:28:21.000000 PyQtGuiLib-2.8.25.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.538538 PyQtGuiLib-2.8.25.1/tests/test_Animation/
+-rw-rw-rw-   0        0        0     1990 2023-06-14 07:54:17.000000 PyQtGuiLib-2.8.25.1/tests/test_Animation/1.py
+-rw-rw-rw-   0        0        0      606 2023-03-15 09:52:36.000000 PyQtGuiLib-2.8.25.1/tests/test_Animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.540538 PyQtGuiLib-2.8.25.1/tests/test_Animation/test_ani/
+-rw-rw-rw-   0        0        0     1589 2023-04-20 01:28:51.000000 PyQtGuiLib-2.8.25.1/tests/test_Animation/test_ani/1.py
+-rw-rw-rw-   0        0        0      107 2023-03-27 05:53:58.000000 PyQtGuiLib-2.8.25.1/tests/test_Animation/test_ani/__init__.py
+-rw-rw-rw-   0        0        0     1364 2023-06-29 03:04:29.000000 PyQtGuiLib-2.8.25.1/tests/test_Animation/test_animation.py
+-rw-rw-rw-   0        0        0     1728 2023-06-25 10:32:05.000000 PyQtGuiLib-2.8.25.1/tests/test_Animation/test_p_ani.py
+-rw-rw-rw-   0        0        0     1541 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_BubbleWidget.py
+-rw-rw-rw-   0        0        0     2738 2023-04-13 08:35:22.000000 PyQtGuiLib-2.8.25.1/tests/test_CircularProgressBar.py
+-rw-rw-rw-   0        0        0     1288 2023-04-25 08:18:48.000000 PyQtGuiLib-2.8.25.1/tests/test_ComboCheckBox.py
+-rw-rw-rw-   0        0        0     1596 2023-04-19 07:50:47.000000 PyQtGuiLib-2.8.25.1/tests/test_Notice.py
+-rw-rw-rw-   0        0        0     1829 2023-04-26 01:49:56.000000 PyQtGuiLib-2.8.25.1/tests/test_PageCuttingButtonGroup.py
+-rw-rw-rw-   0        0        0     1898 2023-05-31 09:45:31.000000 PyQtGuiLib-2.8.25.1/tests/test_PaletteTools.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.551538 PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/
+-rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-04-06 02:24:28.000000 PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg1.py
+-rw-rw-rw-   0        0        0     2306 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg2.py
+-rw-rw-rw-   0        0        0     1891 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg3.py
+-rw-rw-rw-   0        0        0     2110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg4.py
+-rw-rw-rw-   0        0        0     2519 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg5.py
+-rw-rw-rw-   0        0        0     1881 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg6.py
+-rw-rw-rw-   0        0        0     2617 2023-03-22 05:45:33.000000 PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg7.py
+-rw-rw-rw-   0        0        0     2042 2023-04-06 03:41:23.000000 PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/test.py
+-rw-rw-rw-   0        0        0     2275 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis.py
+-rw-rw-rw-   0        0        0     2605 2023-04-13 09:27:46.000000 PyQtGuiLib-2.8.25.1/tests/test_SlideShow.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.559538 PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/
+-rw-rw-rw-   0        0        0      871 2023-04-20 09:50:12.000000 PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/1.py
+-rw-rw-rw-   0        0        0      106 2023-04-07 09:06:55.000000 PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/__init__.py
+-rw-rw-rw-   0        0        0     1568 2023-04-07 09:19:44.000000 PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/eg1.py
+-rw-rw-rw-   0        0        0     2143 2023-04-10 00:27:52.000000 PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/eg2.py
+-rw-rw-rw-   0        0        0     1648 2023-04-07 09:39:03.000000 PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/eg3.py
+-rw-rw-rw-   0        0        0     3527 2023-04-19 03:20:23.000000 PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/eg4.py
+-rw-rw-rw-   0        0        0     1531 2023-05-11 09:36:30.000000 PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/test.py
+-rw-rw-rw-   0        0        0     2465 2023-04-13 01:50:22.000000 PyQtGuiLib-2.8.25.1/tests/test_barset.py
+-rw-rw-rw-   0        0        0     1648 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_circularBar.py
+-rw-rw-rw-   0        0        0     1723 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_colorPalette.py
+-rw-rw-rw-   0        0        0     1979 2023-05-02 10:29:36.000000 PyQtGuiLib-2.8.25.1/tests/test_drawer.py
+-rw-rw-rw-   0        0        0      289 2023-05-05 10:31:26.000000 PyQtGuiLib-2.8.25.1/tests/test_dumpStructure.py
+-rw-rw-rw-   0        0        0     1315 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_flowLayot.py
+-rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_gradientBar.py
+-rw-rw-rw-   0        0        0     1865 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_listWidget.py
+-rw-rw-rw-   0        0        0     1386 2023-05-08 00:28:14.000000 PyQtGuiLib-2.8.25.1/tests/test_loadbar.py
+-rw-rw-rw-   0        0        0     2498 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_no_border.py
+-rw-rw-rw-   0        0        0     1365 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_no_border_pullOver.py
+-rw-rw-rw-   0        0        0     1022 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_pullOverWidget.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.562538 PyQtGuiLib-2.8.25.1/tests/test_qssFile/
+-rw-rw-rw-   0        0        0      107 2023-03-29 06:12:59.000000 PyQtGuiLib-2.8.25.1/tests/test_qssFile/__init__.py
+-rw-rw-rw-   0        0        0      584 2023-04-04 06:18:57.000000 PyQtGuiLib-2.8.25.1/tests/test_qssFile/test.py
+-rw-rw-rw-   0        0        0     1444 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_rollWidget.py
+-rw-rw-rw-   0        0        0     1666 2023-05-29 10:31:16.000000 PyQtGuiLib-2.8.25.1/tests/test_slider.py
+-rw-rw-rw-   0        0        0     1778 2023-04-13 01:45:35.000000 PyQtGuiLib-2.8.25.1/tests/test_statusBar.py
+-rw-rw-rw-   0        0        0     1014 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_styles.py
+-rw-rw-rw-   0        0        0     1122 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_switchButton.py
+-rw-rw-rw-   0        0        0      543 2023-04-17 01:43:36.000000 PyQtGuiLib-2.8.25.1/tests/test_template.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.564538 PyQtGuiLib-2.8.25.1/tests/test_templateWindow/
+-rw-rw-rw-   0        0        0      107 2023-04-11 04:44:35.000000 PyQtGuiLib-2.8.25.1/tests/test_templateWindow/__init__.py
+-rw-rw-rw-   0        0        0     2718 2023-04-13 10:00:15.000000 PyQtGuiLib-2.8.25.1/tests/test_templateWindow/test_listTemplateWindow.py
+-rw-rw-rw-   0        0        0     1356 2023-03-13 08:03:45.000000 PyQtGuiLib-2.8.25.1/tests/test_toolList.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:20:45.566550 PyQtGuiLib-2.8.25.1/tests/test_uic/
+-rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_uic/__init__.py
+-rw-rw-rw-   0        0        0      377 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_uic/test_uic.py
+-rw-rw-rw-   0        0        0     1547 2023-03-06 00:27:58.000000 PyQtGuiLib-2.8.25.1/tests/test_waterBar.py
```

### Comparing `PyQtGuiLib-2.8.25.0/LICENSE.txt` & `PyQtGuiLib-2.8.25.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/Log/developmentLog.py` & `PyQtGuiLib-2.8.25.1/Log/developmentLog.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PKG-INFO` & `PyQtGuiLib-2.8.25.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtGuiLib
-Version: 2.8.25.0
+Version: 2.8.25.1
 Summary: Python version of the qt component library.
 Home-page: https://github.com/LX-sys/PyQtGuiLib
 Author: LX
 Author-email: lx984608061@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/animation/PropertyAnimation.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/animation/PropertyAnimation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/animation/animation.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/animation/animation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/__init__.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/bubbleWidget.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/bubbleWidget.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,76 +28,82 @@
         super().__init__(*args,**kwargs)
         self.resize(100,60)
 
         # 箭头高度(三角形)
         self._arrows_h = 16
 
         # 文字
-        self.text = ""
+        self._text = ""
 
         # 追踪的控件
         self.trackWidget = None #type:QWidget
 
-        self.direction = BubbleWidget.Down
+        self.__direction = BubbleWidget.Down
 
         #
         self.setText("气泡窗口")
 
     def set_Arrows(self,size:int):
         self._arrows_h = size
 
     def get_Arrows(self) -> int:
         return self._arrows_h
     # ----------------
 
     # 设置文字
     def setText(self,text:str):
-        self.text = text
+        self._text = text
         self.textExtend()
 
+    def text(self)->str:
+        return self._text
+
     # 文字扩展
     def textExtend(self):
         f = QFont()
         f.setPointSize(self.get_fontSize())
         # 文字大小
-        fs = textSize(f, self.text)
+        fs = textSize(f, self._text)
         fw = fs.width()
         fh = fs.height()
 
-        if self.direction in [BubbleWidget.Top,BubbleWidget.Down]:
+        if self.__direction in [BubbleWidget.Top,BubbleWidget.Down]:
             self.resize(fw + 30, self.height())
         else:
             self.resize(fw + 30+self._arrows_h, self.height())
 
         if fh >= self.height():
             self.resize(self.width(),self.height()+40)
 
         self.setTrack(self.trackWidget)
 
     # 设置气泡箭头方向
     def setDirection(self,d):
-        self.direction = d
+        self.__direction = d
+
+    def direction(self)->str:
+        return self.__direction
 
     # 控件追踪
     def setTrack(self, widget: QWidget):
         if widget is None:
             return
 
         self.trackWidget = widget
 
         x,y = widget.x(),widget.y()
         w,h = widget.width(),widget.height()
         cx = widget.x()+w//2-self.width()//2  # x轴中心
         cy = widget.y()+h//2-self.height()//2
 
-        if self.direction == BubbleWidget.Top:
+        if self.__direction == BubbleWidget.Top:
             self.move(cx,y+h)
-        elif self.direction == BubbleWidget.Left:
+        elif self.__direction == BubbleWidget.Left:
             self.move(x+w,cy)
-        elif self.direction == BubbleWidget.Right:
+        elif self.__direction == BubbleWidget.Right:
             self.move(x-self.width(),cy)
         else:
             self.move(cx,y-self.height())
 
     # 绘制气泡
     def drawBubble(self,painter:QPainter,ppath:QPainterPath):
         # 矩形高度
@@ -109,47 +115,47 @@
         line_y = self.height()//2  # 线的位置-垂直
 
         # 绘制文字
         f = QFont()
         f.setPointSize(self.get_fontSize())
         painter.setFont(f)
         # 文字大小
-        fs = textSize(f, self.text)
+        fs = textSize(f, self._text)
         fw = fs.width()
         fh = fs.height()
 
         self.textExtend()
 
         # 画刷
         bru = QBrush(self.get_backgroundColor())
         painter.setBrush(bru)
 
         # 画笔
         painter.setPen(qt.NoPen)
 
-        if self.direction == BubbleWidget.Top:
+        if self.__direction == BubbleWidget.Top:
             # 画三角
             ploys = [QPointF(lien_x,self._arrows_h,),QPointF(lien_x+line_w//2,1),
                      QPointF(lien_x+line_w,self._arrows_h)
                      ]
             # 画矩形
             rect = QRect(self.get_margin(),self._arrows_h+self.get_margin(),self.width()-self.get_margin()*2,rect_h-self.get_margin()*2)
             # 文字位置
             x = self.width() // 2 - fw // 2
             y = rect_h//2 + fh//2+self._arrows_h
-        elif self.direction == BubbleWidget.Left:
+        elif self.__direction == BubbleWidget.Left:
             # 画三角
             ploys = [QPointF(1,line_y),QPointF(self._arrows_h,line_y-line_w//2),
                      QPointF(self._arrows_h,line_y+line_w//2)
             ]
             rect = QRect(self._arrows_h+self.get_margin(),self.get_margin(),rect_w-self.get_margin()*2,self.height()-self.get_margin()*2)
             # 文字位置
             x = self.width()//2-fw//2 + self._arrows_h//2
             y = self.height()//2 + fh//2
-        elif self.direction == BubbleWidget.Right:
+        elif self.__direction == BubbleWidget.Right:
             # 画三角
             ploys =[QPointF(rect_w,line_y-line_w//2),QPointF(rect_w+self._arrows_h,line_y),
                     QPointF(rect_w,line_y+line_w//2)
             ]
             rect = QRect(self.get_margin(),self.get_margin(),rect_w-self.get_margin()*2,self.height()-self.get_margin()*2)
             # 文字位置
             x = (self.width()-self._arrows_h)//2 - fw//2
@@ -168,15 +174,15 @@
         # 绘制三角形
         ppath.addPolygon(QPolygonF(ploys))
         painter.fillPath(ppath, self.get_backgroundColor())
         # 绘制文字
         op = QPen()
         op.setColor(QColor(255, 255, 255))
         painter.setPen(op)
-        painter.drawText(x,y, self.text)
+        painter.drawText(x,y, self._text)
 
     def paintEvent(self, e:QPaintEvent) -> None:
         painter = QPainter(self)
         painter.setRenderHints(qt.Antialiasing | qt.SmoothPixmapTransform | qt.TextAntialiasing)
 
         ppath = QPainterPath()
```

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/chatRoom.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/chatRoom.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/headImage.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/headImage.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/message.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/message.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/test.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/transmitter.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/transmitter.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/charRooms/utility.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/charRooms/utility.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/comboBox/comboBox.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/comboBox/comboBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/comboBox/comboCheckBox/comboCheckBox.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/comboBox/comboCheckBox/comboCheckBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_message_box.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/comboBox/comboCheckBox/py_message_box.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/comboBox/comboCheckBox/py_style.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/comboBox/comboCheckBox/py_style.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/drawers/drawer.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/drawers/drawer.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/flowLayout.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/flowLayout.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/listWidget.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/listWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/logBrowser/loadLogTh.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/logBrowser/loadLogTh.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/logBrowser/logBrowser.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/logBrowser/logBrowser.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/logBrowser/logSizeTh.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/logBrowser/logSizeTh.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/notice/notice.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/notice/notice.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/pager/pageCuttingButtonGroup.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/pager/pageCuttingButtonGroup.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/colorHsv.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/colorHsv.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/paletteFrame.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/paletteFrame.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/paletteTools/area.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/paletteTools/area.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/paletteTools/paletteToolUI.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/paletteTools/paletteToolUI.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/paletteTools/palettetools.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/paletteTools/palettetools.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/palettes/palettetools.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/palettes/palettetools.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/progressBar/circularBar.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/progressBar/circularBar.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     qt
 )
 
 
 
 '''
     圆环进度条
+    2023.7.4 该组件需要重写,无法适配在设计器上面
 '''
 class CircularBar(QWidget):
     # 进度改变时,发出信号
     valueChange = Signal(int)
 
     # 外圈/内圈
     OuterRing = "OuterRing"
```

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/progressBar/circularProgressBar.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/progressBar/circularProgressBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/progressBar/gradientBar.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/progressBar/gradientBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/progressBar/loadBar.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/progressBar/loadBar.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     QResizeEvent,
     qt,
     textSize
 )
 
 
 '''
-    加载进度条
+    加载进度条 
+    2023.7.4 该组件需要重写,无法适配在设计器上面
 '''
 class LoadBar(QWidget):
     # 进度改变时,发出信号
     valueChange = Signal(int)
 
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
```

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/progressBar/waterBar.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/progressBar/waterBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/pullOver.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/pullOver.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/resolver/controls.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/resolver/controls.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/rollWidget.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/rollWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/slideShow.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/slideShow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/slider/slider.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/slider/slider.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/switchButtons/swButton.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/switchButtons/swButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/table/table.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/table/table.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/toolBox.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/toolBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/toolList.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/toolList.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/WidgetABC.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/WidgetABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/borderlessMainWindow.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/borderlessMainWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/statusBar.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/statusBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/tets/2.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/tets/2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/core/widgets/titleBar.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/core/widgets/titleBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/Qt/qt.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/Qt/qt.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/Qt/qtCore.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/Qt/qtCore.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/Qt/qtGui.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/Qt/qtGui.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/__init__.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/customStyle.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/customStyle.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/header/utility.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/header/utility.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/layoutDeformation/test.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/layoutDeformation/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/particle/particle.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/particle/particle.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/buttons/buttonStyle.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/buttons/buttonStyle.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/guiLibStyle/__init__.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/guiLibStyle/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/guiLibStyle/libStyle.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/guiLibStyle/libStyle.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/drak/qssDrak.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/drak/qssDrak.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/image/image_rc.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/image/image_rc.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/qssFile.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/qssFile.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/qssFile/test.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/qssFile/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/skinABC.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/skinABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/styleAnalysis.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/styleAnalysis.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/styles/superPainter/superPainter.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/styles/superPainter/superPainter.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib.egg-info/PKG-INFO` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtGuiLib
-Version: 2.8.25.0
+Version: 2.8.25.1
 Summary: Python version of the qt component library.
 Home-page: https://github.com/LX-sys/PyQtGuiLib
 Author: LX
 Author-email: lx984608061@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyQtGuiLib-2.8.25.0/PyQtGuiLib.egg-info/SOURCES.txt` & `PyQtGuiLib-2.8.25.1/PyQtGuiLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/README.md` & `PyQtGuiLib-2.8.25.1/README.md`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/acrylic/acrylicWidget.py` & `PyQtGuiLib-2.8.25.1/abandonCase/acrylic/acrylicWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/acrylic/cstruct.py` & `PyQtGuiLib-2.8.25.1/abandonCase/acrylic/cstruct.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/acrylic/windowEffect.py` & `PyQtGuiLib-2.8.25.1/abandonCase/acrylic/windowEffect.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/animation/animation.py` & `PyQtGuiLib-2.8.25.1/abandonCase/animation/animation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/animation/animationDrawType.py` & `PyQtGuiLib-2.8.25.1/abandonCase/animation/animationDrawType.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/animation/animationFactory.py` & `PyQtGuiLib-2.8.25.1/abandonCase/animation/animationFactory.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/animation/animationLayout.py` & `PyQtGuiLib-2.8.25.1/abandonCase/animation/animationLayout.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/animation/customAniTest.py` & `PyQtGuiLib-2.8.25.1/abandonCase/animation/customAniTest.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/bubbleWidget.py` & `PyQtGuiLib-2.8.25.1/abandonCase/bubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/bubbleWidget_case.py` & `PyQtGuiLib-2.8.25.1/abandonCase/bubbleWidget_case.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/linker/component.py` & `PyQtGuiLib-2.8.25.1/abandonCase/linker/component.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/linker/controlType.py` & `PyQtGuiLib-2.8.25.1/abandonCase/linker/controlType.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/linker/styleLinker.py` & `PyQtGuiLib-2.8.25.1/abandonCase/linker/styleLinker.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/linker/styleLinkerUi.py` & `PyQtGuiLib-2.8.25.1/abandonCase/linker/styleLinkerUi.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/nodeBar.py` & `PyQtGuiLib-2.8.25.1/abandonCase/nodeBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/slideShow.py` & `PyQtGuiLib-2.8.25.1/abandonCase/slideShow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/slideShow2.py` & `PyQtGuiLib-2.8.25.1/abandonCase/slideShow2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/superPainter.py` & `PyQtGuiLib-2.8.25.1/abandonCase/superPainter.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/widgets/borderlessFrame.py` & `PyQtGuiLib-2.8.25.1/abandonCase/widgets/borderlessFrame.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/widgets/borderlessMainWindow.py` & `PyQtGuiLib-2.8.25.1/abandonCase/widgets/borderlessMainWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/widgets/borderlessStackedWidget.py` & `PyQtGuiLib-2.8.25.1/abandonCase/widgets/borderlessStackedWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/widgets/borderlessWidget.py` & `PyQtGuiLib-2.8.25.1/abandonCase/widgets/borderlessWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/widgets/borderlessWidgetABC.py` & `PyQtGuiLib-2.8.25.1/abandonCase/widgets/borderlessWidgetABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/widgets/statusBar.py` & `PyQtGuiLib-2.8.25.1/abandonCase/widgets/statusBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/abandonCase/widgets/titleBar.py` & `PyQtGuiLib-2.8.25.1/abandonCase/widgets/titleBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/auxiliaryMeans/toolNewProject.py` & `PyQtGuiLib-2.8.25.1/auxiliaryMeans/toolNewProject.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/setup.py` & `PyQtGuiLib-2.8.25.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 
 setup(
     name="PyQtGuiLib",
     packages =find_packages(),
-    version="2.8.25.0",
+    version="2.8.25.1",
     author="LX",
     author_email = "lx984608061@163.com",
     description = "Python version of the qt component library.",
     long_description=open('README.md', 'r',encoding="utf8").read(),
     long_description_content_type="text/markdown",
     url = "https://github.com/LX-sys/PyQtGuiLib",
     classifiers = [
```

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_Animation/1.py` & `PyQtGuiLib-2.8.25.1/tests/test_Animation/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_Animation/__init__.py` & `PyQtGuiLib-2.8.25.1/tests/test_Animation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_Animation/test_ani/1.py` & `PyQtGuiLib-2.8.25.1/tests/test_Animation/test_ani/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_Animation/test_animation.py` & `PyQtGuiLib-2.8.25.1/tests/test_Animation/test_animation.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 }
         ''')
 
         self.stopbtn = QPushButton("暂停",self)
 
 
         self.ani = Animation()
-        self.ani.addAni(self.btn.pos(),QPoint(300,300),courseFunc=self.btn.move,duration=5000)
+        self.ani.addAni(self.btn.pos(),QPoint(300,300),courseFunc=self.btn.move,duration=5000,loopCount=-1)
 
         self.ani.start()
 
         self.stopbtn.clicked.connect(self.test)
 
     def test(self):
         if self.ani.state() == Animation.START:
```

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_Animation/test_p_ani.py` & `PyQtGuiLib-2.8.25.1/tests/test_Animation/test_p_ani.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_BubbleWidget.py` & `PyQtGuiLib-2.8.25.1/tests/test_BubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_CircularProgressBar.py` & `PyQtGuiLib-2.8.25.1/tests/test_CircularProgressBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_ComboCheckBox.py` & `PyQtGuiLib-2.8.25.1/tests/test_ComboCheckBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_Notice.py` & `PyQtGuiLib-2.8.25.1/tests/test_Notice.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_PageCuttingButtonGroup.py` & `PyQtGuiLib-2.8.25.1/tests/test_PageCuttingButtonGroup.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_PaletteTools.py` & `PyQtGuiLib-2.8.25.1/tests/test_PaletteTools.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/__init__.py` & `PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg1.py` & `PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg2.py` & `PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg3.py` & `PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg3.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg4.py` & `PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg4.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg5.py` & `PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg5.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg6.py` & `PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg6.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/eg7.py` & `PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/eg7.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis/test.py` & `PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_QssStyleAnalysis.py` & `PyQtGuiLib-2.8.25.1/tests/test_QssStyleAnalysis.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_SlideShow.py` & `PyQtGuiLib-2.8.25.1/tests/test_SlideShow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/1.py` & `PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/eg1.py` & `PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/eg1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/eg2.py` & `PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/eg2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/eg3.py` & `PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/eg3.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/eg4.py` & `PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/eg4.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_SuperPainter/test.py` & `PyQtGuiLib-2.8.25.1/tests/test_SuperPainter/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_barset.py` & `PyQtGuiLib-2.8.25.1/tests/test_barset.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_circularBar.py` & `PyQtGuiLib-2.8.25.1/tests/test_circularBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_colorPalette.py` & `PyQtGuiLib-2.8.25.1/tests/test_colorPalette.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_drawer.py` & `PyQtGuiLib-2.8.25.1/tests/test_drawer.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_flowLayot.py` & `PyQtGuiLib-2.8.25.1/tests/test_flowLayot.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_gradientBar.py` & `PyQtGuiLib-2.8.25.1/tests/test_gradientBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_listWidget.py` & `PyQtGuiLib-2.8.25.1/tests/test_listWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_loadbar.py` & `PyQtGuiLib-2.8.25.1/tests/test_loadbar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_no_border.py` & `PyQtGuiLib-2.8.25.1/tests/test_no_border.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_no_border_pullOver.py` & `PyQtGuiLib-2.8.25.1/tests/test_no_border_pullOver.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_pullOverWidget.py` & `PyQtGuiLib-2.8.25.1/tests/test_pullOverWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_qssFile/test.py` & `PyQtGuiLib-2.8.25.1/tests/test_qssFile/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_rollWidget.py` & `PyQtGuiLib-2.8.25.1/tests/test_rollWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_slider.py` & `PyQtGuiLib-2.8.25.1/tests/test_slider.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_statusBar.py` & `PyQtGuiLib-2.8.25.1/tests/test_statusBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_styles.py` & `PyQtGuiLib-2.8.25.1/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_switchButton.py` & `PyQtGuiLib-2.8.25.1/tests/test_switchButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_template.py` & `PyQtGuiLib-2.8.25.1/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_templateWindow/test_listTemplateWindow.py` & `PyQtGuiLib-2.8.25.1/tests/test_templateWindow/test_listTemplateWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_toolList.py` & `PyQtGuiLib-2.8.25.1/tests/test_toolList.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.8.25.0/tests/test_waterBar.py` & `PyQtGuiLib-2.8.25.1/tests/test_waterBar.py`

 * *Files identical despite different names*

