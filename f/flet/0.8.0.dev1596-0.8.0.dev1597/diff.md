# Comparing `tmp/flet-0.8.0.dev1596.tar.gz` & `tmp/flet-0.8.0.dev1597.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-0.8.0.dev1596.tar", max compression
+gzip compressed data, was "flet-0.8.0.dev1597.tar", max compression
```

## Comparing `flet-0.8.0.dev1596.tar` & `flet-0.8.0.dev1597.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     2145 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/README.md
--rw-r--r--   0        0        0     1069 2023-06-30 21:09:05.417268 flet-0.8.0.dev1596/pyproject.toml
--rw-r--r--   0        0        0       27 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/__init__.py
--rw-r--r--   0        0        0       72 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/__pyinstaller/__init__.py
--rw-r--r--   0        0        0       20 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/__pyinstaller/config.py
--rw-r--r--   0        0        0      378 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/__pyinstaller/hook-flet.py
--rw-r--r--   0        0        0     2985 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/__pyinstaller/macos_utils.py
--rw-r--r--   0        0        0      187 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
--rw-r--r--   0        0        0       61 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/__pyinstaller/rthooks.dat
--rw-r--r--   0        0        0      562 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/__pyinstaller/utils.py
--rw-r--r--   0        0        0     3620 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/__pyinstaller/win_utils.py
--rw-r--r--   0        0        0     7267 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/async_websocket_connection.py
--rw-r--r--   0        0        0       32 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/auth/__init__.py
--rw-r--r--   0        0        0       42 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/auth/providers/__init__.py
--rw-r--r--   0        0        0       31 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     3053 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/cli/cli.py
--rw-r--r--   0        0        0     1953 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/cli/commands/base.py
--rw-r--r--   0        0        0     1989 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/cli/commands/create.py
--rw-r--r--   0        0        0      673 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/cli/commands/options.py
--rw-r--r--   0        0        0     8473 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/cli/commands/pack.py
--rw-r--r--   0        0        0     9293 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/cli/commands/publish.py
--rw-r--r--   0        0        0     9745 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/cli/commands/run.py
--rw-r--r--   0        0        0       52 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/constants.py
--rw-r--r--   0        0        0       55 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3212 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/reconnecting_websocket.py
--rw-r--r--   0        0        0     1272 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/security.py
--rw-r--r--   0        0        0     5461 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/sync_websocket_connection.py
--rw-r--r--   0        0        0      145 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/utils/__init__.py
--rw-r--r--   0        0        0     1469 2023-06-30 21:08:29.090062 flet-0.8.0.dev1596/src/flet/version.py
--rw-r--r--   0        0        0       32 2023-06-30 20:59:00.000000 flet-0.8.0.dev1596/src/flet/web/.last_build_id
--rw-r--r--   0        0        0      484 2023-06-30 20:58:57.000000 flet-0.8.0.dev1596/src/flet/web/assets/AssetManifest.bin
--rw-r--r--   0        0        0      455 2023-06-30 20:58:57.000000 flet-0.8.0.dev1596/src/flet/web/assets/AssetManifest.json
--rw-r--r--   0        0        0       82 2023-06-30 20:58:57.000000 flet-0.8.0.dev1596/src/flet/web/assets/FontManifest.json
--rw-r--r--   0        0        0  1738123 2023-06-30 20:58:57.000000 flet-0.8.0.dev1596/src/flet/web/assets/NOTICES
--rw-r--r--   0        0        0  1261080 2023-06-30 20:58:59.000000 flet-0.8.0.dev1596/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
--rw-r--r--   0        0        0      298 2023-06-30 20:58:57.000000 flet-0.8.0.dev1596/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
--rw-r--r--   0        0        0      271 2023-06-30 20:58:57.000000 flet-0.8.0.dev1596/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
--rw-r--r--   0        0        0      166 2023-06-30 20:58:57.000000 flet-0.8.0.dev1596/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
--rw-r--r--   0        0        0      366 2023-06-30 20:58:57.000000 flet-0.8.0.dev1596/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
--rw-r--r--   0        0        0     9242 2023-06-30 20:58:57.000000 flet-0.8.0.dev1596/src/flet/web/assets/shaders/ink_sparkle.frag
--rw-r--r--   0        0        0     1028 2023-06-30 20:58:59.000000 flet-0.8.0.dev1596/src/flet/web/favicon.png
--rw-r--r--   0        0        0    14240 2023-06-30 20:57:48.000000 flet-0.8.0.dev1596/src/flet/web/flutter.js
--rw-r--r--   0        0        0     8316 2023-06-30 20:59:00.000000 flet-0.8.0.dev1596/src/flet/web/flutter_service_worker.js
--rw-r--r--   0        0        0     4699 2023-06-30 20:58:59.000000 flet-0.8.0.dev1596/src/flet/web/icons/apple-touch-icon-192.png
--rw-r--r--   0        0        0     6622 2023-06-30 20:58:59.000000 flet-0.8.0.dev1596/src/flet/web/icons/icon-192.png
--rw-r--r--   0        0        0    18666 2023-06-30 20:58:59.000000 flet-0.8.0.dev1596/src/flet/web/icons/icon-512.png
--rw-r--r--   0        0        0     4128 2023-06-30 20:58:59.000000 flet-0.8.0.dev1596/src/flet/web/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    11906 2023-06-30 20:58:59.000000 flet-0.8.0.dev1596/src/flet/web/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    17040 2023-06-30 20:58:59.000000 flet-0.8.0.dev1596/src/flet/web/icons/loading-animation.png
--rw-r--r--   0        0        0     3159 2023-06-30 20:58:59.000000 flet-0.8.0.dev1596/src/flet/web/index.html
--rw-r--r--   0        0        0  5449285 2023-06-30 20:58:56.000000 flet-0.8.0.dev1596/src/flet/web/main.dart.js
--rw-r--r--   0        0        0      789 2023-06-30 20:58:59.000000 flet-0.8.0.dev1596/src/flet/web/manifest.json
--rw-r--r--   0        0        0     1573 2023-06-30 20:58:59.000000 flet-0.8.0.dev1596/src/flet/web/python-worker.js
--rw-r--r--   0        0        0      744 2023-06-30 20:58:59.000000 flet-0.8.0.dev1596/src/flet/web/python.js
--rw-r--r--   0        0        0       92 2023-06-30 20:58:56.000000 flet-0.8.0.dev1596/src/flet/web/version.json
--rw-r--r--   0        0        0     3317 1970-01-01 00:00:00.000000 flet-0.8.0.dev1596/PKG-INFO
+-rw-r--r--   0        0        0     2145 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/README.md
+-rw-r--r--   0        0        0     1085 2023-07-04 18:09:12.441024 flet-0.8.0.dev1597/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/__init__.py
+-rw-r--r--   0        0        0       72 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0       20 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/__pyinstaller/config.py
+-rw-r--r--   0        0        0      378 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/__pyinstaller/hook-flet.py
+-rw-r--r--   0        0        0     2985 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/__pyinstaller/macos_utils.py
+-rw-r--r--   0        0        0      187 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
+-rw-r--r--   0        0        0       61 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/__pyinstaller/rthooks.dat
+-rw-r--r--   0        0        0      562 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/__pyinstaller/utils.py
+-rw-r--r--   0        0        0     3620 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/__pyinstaller/win_utils.py
+-rw-r--r--   0        0        0     7267 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/async_websocket_connection.py
+-rw-r--r--   0        0        0       32 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/auth/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/auth/providers/__init__.py
+-rw-r--r--   0        0        0       31 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     3053 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/cli/cli.py
+-rw-r--r--   0        0        0     1953 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/cli/commands/base.py
+-rw-r--r--   0        0        0     1989 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/cli/commands/create.py
+-rw-r--r--   0        0        0      673 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/cli/commands/options.py
+-rw-r--r--   0        0        0     8473 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/cli/commands/pack.py
+-rw-r--r--   0        0        0     9293 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/cli/commands/publish.py
+-rw-r--r--   0        0        0     9745 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/cli/commands/run.py
+-rw-r--r--   0        0        0       52 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/constants.py
+-rw-r--r--   0        0        0       55 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3212 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/reconnecting_websocket.py
+-rw-r--r--   0        0        0     1272 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/security.py
+-rw-r--r--   0        0        0     5461 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/sync_websocket_connection.py
+-rw-r--r--   0        0        0      145 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/utils/__init__.py
+-rw-r--r--   0        0        0     1469 2023-07-04 18:08:38.440639 flet-0.8.0.dev1597/src/flet/version.py
+-rw-r--r--   0        0        0       32 2023-07-04 17:59:56.000000 flet-0.8.0.dev1597/src/flet/web/.last_build_id
+-rw-r--r--   0        0        0      484 2023-07-04 17:59:52.000000 flet-0.8.0.dev1597/src/flet/web/assets/AssetManifest.bin
+-rw-r--r--   0        0        0      455 2023-07-04 17:59:52.000000 flet-0.8.0.dev1597/src/flet/web/assets/AssetManifest.json
+-rw-r--r--   0        0        0       82 2023-07-04 17:59:52.000000 flet-0.8.0.dev1597/src/flet/web/assets/FontManifest.json
+-rw-r--r--   0        0        0  1738123 2023-07-04 17:59:52.000000 flet-0.8.0.dev1597/src/flet/web/assets/NOTICES
+-rw-r--r--   0        0        0  1261080 2023-07-04 17:59:55.000000 flet-0.8.0.dev1597/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
+-rw-r--r--   0        0        0      298 2023-07-04 17:59:52.000000 flet-0.8.0.dev1597/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
+-rw-r--r--   0        0        0      271 2023-07-04 17:59:52.000000 flet-0.8.0.dev1597/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
+-rw-r--r--   0        0        0      166 2023-07-04 17:59:52.000000 flet-0.8.0.dev1597/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
+-rw-r--r--   0        0        0      366 2023-07-04 17:59:52.000000 flet-0.8.0.dev1597/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
+-rw-r--r--   0        0        0     9242 2023-07-04 17:59:53.000000 flet-0.8.0.dev1597/src/flet/web/assets/shaders/ink_sparkle.frag
+-rw-r--r--   0        0        0     1028 2023-07-04 17:59:55.000000 flet-0.8.0.dev1597/src/flet/web/favicon.png
+-rw-r--r--   0        0        0    14240 2023-07-04 17:58:36.000000 flet-0.8.0.dev1597/src/flet/web/flutter.js
+-rw-r--r--   0        0        0     8316 2023-07-04 17:59:56.000000 flet-0.8.0.dev1597/src/flet/web/flutter_service_worker.js
+-rw-r--r--   0        0        0     4699 2023-07-04 17:59:55.000000 flet-0.8.0.dev1597/src/flet/web/icons/apple-touch-icon-192.png
+-rw-r--r--   0        0        0     6622 2023-07-04 17:59:55.000000 flet-0.8.0.dev1597/src/flet/web/icons/icon-192.png
+-rw-r--r--   0        0        0    18666 2023-07-04 17:59:55.000000 flet-0.8.0.dev1597/src/flet/web/icons/icon-512.png
+-rw-r--r--   0        0        0     4128 2023-07-04 17:59:55.000000 flet-0.8.0.dev1597/src/flet/web/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    11906 2023-07-04 17:59:55.000000 flet-0.8.0.dev1597/src/flet/web/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    17040 2023-07-04 17:59:55.000000 flet-0.8.0.dev1597/src/flet/web/icons/loading-animation.png
+-rw-r--r--   0        0        0     3159 2023-07-04 17:59:55.000000 flet-0.8.0.dev1597/src/flet/web/index.html
+-rw-r--r--   0        0        0  5449285 2023-07-04 17:59:52.000000 flet-0.8.0.dev1597/src/flet/web/main.dart.js
+-rw-r--r--   0        0        0      789 2023-07-04 17:59:55.000000 flet-0.8.0.dev1597/src/flet/web/manifest.json
+-rw-r--r--   0        0        0     1573 2023-07-04 17:59:55.000000 flet-0.8.0.dev1597/src/flet/web/python-worker.js
+-rw-r--r--   0        0        0      744 2023-07-04 17:59:55.000000 flet-0.8.0.dev1597/src/flet/web/python.js
+-rw-r--r--   0        0        0       92 2023-07-04 17:59:52.000000 flet-0.8.0.dev1597/src/flet/web/version.json
+-rw-r--r--   0        0        0     3346 1970-01-01 00:00:00.000000 flet-0.8.0.dev1597/PKG-INFO
```

### Comparing `flet-0.8.0.dev1596/README.md` & `flet-0.8.0.dev1597/README.md`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/pyproject.toml` & `flet-0.8.0.dev1597/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet"
-version = "0.8.0.dev1596"
+version = "0.8.0.dev1597"
 description = "Flet for Python - easily build interactive multi-platform apps in Python"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,23 +12,24 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-runtime = "0.8.0.dev1596"
+flet-runtime = "0.8.0.dev1597"
 python = "^3.7"
 typing-extensions = { version = "^4.6.2", python = "<3.8" }
 websocket-client = "^1.5.2"
 watchdog = "^3.0.0"
 websockets = "^11.0.3"
 packaging = "^23.1"
 copier = "^8.0.0"
 qrcode = "^7.4.2"
+pydantic = "<2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.6"
 pytest = "^7.2.0"
 cryptography = "^39.0.0"
 
 [tool.poetry.scripts]
```

### Comparing `flet-0.8.0.dev1596/src/flet/__pyinstaller/macos_utils.py` & `flet-0.8.0.dev1597/src/flet/__pyinstaller/macos_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/__pyinstaller/utils.py` & `flet-0.8.0.dev1597/src/flet/__pyinstaller/utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/__pyinstaller/win_utils.py` & `flet-0.8.0.dev1597/src/flet/__pyinstaller/win_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/async_websocket_connection.py` & `flet-0.8.0.dev1597/src/flet/async_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/cli/cli.py` & `flet-0.8.0.dev1597/src/flet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/cli/commands/base.py` & `flet-0.8.0.dev1597/src/flet/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/cli/commands/create.py` & `flet-0.8.0.dev1597/src/flet/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/cli/commands/options.py` & `flet-0.8.0.dev1597/src/flet/cli/commands/options.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/cli/commands/pack.py` & `flet-0.8.0.dev1597/src/flet/cli/commands/pack.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/cli/commands/publish.py` & `flet-0.8.0.dev1597/src/flet/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/cli/commands/run.py` & `flet-0.8.0.dev1597/src/flet/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/reconnecting_websocket.py` & `flet-0.8.0.dev1597/src/flet/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/security.py` & `flet-0.8.0.dev1597/src/flet/security.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/sync_websocket_connection.py` & `flet-0.8.0.dev1597/src/flet/sync_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/version.py` & `flet-0.8.0.dev1597/src/flet/version.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/assets/NOTICES` & `flet-0.8.0.dev1597/src/flet/web/assets/NOTICES`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/assets/fonts/MaterialIcons-Regular.otf` & `flet-0.8.0.dev1597/src/flet/web/assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/assets/shaders/ink_sparkle.frag` & `flet-0.8.0.dev1597/src/flet/web/assets/shaders/ink_sparkle.frag`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/favicon.png` & `flet-0.8.0.dev1597/src/flet/web/favicon.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/flutter.js` & `flet-0.8.0.dev1597/src/flet/web/flutter.js`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/flutter_service_worker.js` & `flet-0.8.0.dev1597/src/flet/web/flutter_service_worker.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -30,16 +30,16 @@
     "canvaskit/skwasm.js": "1df4d741f441fa1a4d10530ced463ef8",
     "canvaskit/canvaskit.js": "76f7d822f42397160c5dfc69cbc9b2de",
     "canvaskit/skwasm.worker.js": "19659053a277272607529ef87acf9d8a",
     "canvaskit/skwasm.wasm": "6711032e17bf49924b2b001cef0d3ea3",
     "canvaskit/chromium/canvaskit.wasm": "fc18c3010856029414b70cae1afc5cd9",
     "canvaskit/chromium/canvaskit.js": "8c8392ce4a4364cbb240aa09b5652e05",
     "python-worker.js": "b961f261b9ad85e06369e83fd2e33bb7",
-    "index.html": "1fd6aa1c6fe4538354dabc7f27a08391",
-    "/": "1fd6aa1c6fe4538354dabc7f27a08391"
+    "index.html": "a56bbcd186b5ba0c31657e556a0a3542",
+    "/": "a56bbcd186b5ba0c31657e556a0a3542"
 };
 // The application shell files that are downloaded before a service worker can
 // start.
 const CORE = ["main.dart.js",
     "index.html",
     "assets/AssetManifest.json",
     "assets/FontManifest.json"
```

### Comparing `flet-0.8.0.dev1596/src/flet/web/icons/apple-touch-icon-192.png` & `flet-0.8.0.dev1597/src/flet/web/icons/apple-touch-icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/icons/icon-192.png` & `flet-0.8.0.dev1597/src/flet/web/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/icons/icon-512.png` & `flet-0.8.0.dev1597/src/flet/web/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/icons/icon-maskable-192.png` & `flet-0.8.0.dev1597/src/flet/web/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/icons/icon-maskable-512.png` & `flet-0.8.0.dev1597/src/flet/web/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/icons/loading-animation.png` & `flet-0.8.0.dev1597/src/flet/web/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/index.html` & `flet-0.8.0.dev1597/src/flet/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   <!-- webRenderer -->
   <!-- useColorEmoji -->
 
   <!-- pyodideCode -->
 
   <script>
     // The value below is injected by flutter build, do not touch.
-    var serviceWorkerVersion = "2247750865";
+    var serviceWorkerVersion = "3649380178";
   </script>
   <!-- This script adds the flutter initialization JS code -->
   <script src="flutter.js" defer></script>
 </head>
 
 <body>
   <div id="loading">
```

### Comparing `flet-0.8.0.dev1596/src/flet/web/main.dart.js` & `flet-0.8.0.dev1597/src/flet/web/main.dart.js`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/manifest.json` & `flet-0.8.0.dev1597/src/flet/web/manifest.json`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/python-worker.js` & `flet-0.8.0.dev1597/src/flet/web/python-worker.js`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/src/flet/web/python.js` & `flet-0.8.0.dev1597/src/flet/web/python.js`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1596/PKG-INFO` & `flet-0.8.0.dev1597/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: flet
-Version: 0.8.0.dev1596
+Version: 0.8.0.dev1597
 Summary: Flet for Python - easily build interactive multi-platform apps in Python
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: copier (>=8.0.0,<9.0.0)
-Requires-Dist: flet-runtime (==0.8.0.dev1596)
+Requires-Dist: flet-runtime (==0.8.0.dev1597)
 Requires-Dist: packaging (>=23.1,<24.0)
+Requires-Dist: pydantic (<2)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0) ; python_version < "3.8"
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
 Requires-Dist: websocket-client (>=1.5.2,<2.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
```

