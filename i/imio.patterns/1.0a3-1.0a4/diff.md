# Comparing `tmp/imio.patterns-1.0a3.tar.gz` & `tmp/imio.patterns-1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.patterns-1.0a3.tar", last modified: Mon Jan  4 15:34:04 2021, max compression
+gzip compressed data, was "imio.patterns-1.0a4.tar", last modified: Tue Jul  4 13:23:54 2023, max compression
```

## Comparing `imio.patterns-1.0a3.tar` & `imio.patterns-1.0a4.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      650 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/LICENSE.rst
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     2108 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/setup.py
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/docs/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     7881 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/docs/conf.py
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)       62 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/docs/index.rst
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio.patterns.egg-info/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)        5 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio.patterns.egg-info/top_level.txt
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)        5 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio.patterns.egg-info/namespace_packages.txt
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      173 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio.patterns.egg-info/requires.txt
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     3340 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio.patterns.egg-info/PKG-INFO
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)        1 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio.patterns.egg-info/dependency_links.txt
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      138 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio.patterns.egg-info/entry_points.txt
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     2469 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio.patterns.egg-info/SOURCES.txt
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)        1 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio.patterns.egg-info/not-zip-safe
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)       80 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/__init__.py
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     1489 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/testing.py
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      570 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/configure.zcml
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/overrides/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/overrides/.gitkeep
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/fonts/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     2152 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/fonts/slick.svg
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     1892 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/fonts/slick.ttf
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     2048 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/fonts/slick.eot
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     1380 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/fonts/slick.woff
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/pattern/
--rwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)    80335 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/pattern/slick.js
--rwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)    42863 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/pattern/slick.min.js
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)       66 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/pattern/imio-patterns-bundle-compiled.js
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     3057 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/pattern/pattern.slick.js
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      710 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/pattern/i18n.js
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      108 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/pattern/imio.pattern.js
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/.gitkeep
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/css/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      477 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/css/imio-patterns-bundle-compiled.css
--rwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)    10333 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/css/slick.css
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/less/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)       36 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/less/imio-patterns-bundle.less
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      178 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/less/theme-compiled.less.map
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      193 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/static/less/imio-patterns-bundle-compiled.less.map
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/browser/__init__.py
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/locales/
--rwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)      476 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/locales/update.sh
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/locales/en/
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/locales/en/LC_MESSAGES/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/locales/en/LC_MESSAGES/imio.patterns.po
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      611 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/locales/README.rst
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/locales/__init__.py
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     1571 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/locales/update.py
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/locales/imio.patterns.pot
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      205 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/upgrades.py
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      260 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/permissions.zcml
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      614 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/setuphandlers.py
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      382 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/upgrades.zcml
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     1372 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/configure.zcml
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      262 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/interfaces.py
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/profiles/
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/profiles/default/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     2906 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/profiles/default/registry.xml
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      118 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/profiles/default/rolemap.xml
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      105 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/profiles/default/catalog.xml
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      195 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/profiles/default/metadata.xml
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      165 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/profiles/default/browserlayer.xml
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/profiles/uninstall/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      123 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/tests/
-drwxrwxr-x   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/tests/robot/
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     1983 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/tests/robot/test_example.robot
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     2395 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/tests/test_setup.py
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      875 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/tests/test_robot.py
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)        0 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/tests/__init__.py
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      130 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/src/imio/patterns/__init__.py
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     3340 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/PKG-INFO
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)       61 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/MANIFEST.in
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)     1406 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/README.rst
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)       57 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/CONTRIBUTORS.rst
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      321 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/setup.cfg
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      586 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/DEVELOP.rst
--rw-rw-r--   0 bsuttor   (1000) bsuttor   (1000)      262 2021-01-04 15:34:04.000000 imio.patterns-1.0a3/CHANGES.rst
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.817825 imio.patterns-1.0a4/
+-rw-r--r--   0 thom       (501) staff       (20)      345 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/CHANGES.rst
+-rw-r--r--   0 thom       (501) staff       (20)       57 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/CONTRIBUTORS.rst
+-rw-r--r--   0 thom       (501) staff       (20)      586 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/DEVELOP.rst
+-rw-r--r--   0 thom       (501) staff       (20)    18092 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/LICENSE.GPL
+-rw-r--r--   0 thom       (501) staff       (20)      650 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/LICENSE.rst
+-rw-r--r--   0 thom       (501) staff       (20)       61 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/MANIFEST.in
+-rw-r--r--   0 thom       (501) staff       (20)     2590 2023-07-04 13:23:54.818004 imio.patterns-1.0a4/PKG-INFO
+-rw-r--r--   0 thom       (501) staff       (20)     1406 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/README.rst
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.791931 imio.patterns-1.0a4/docs/
+-rw-r--r--   0 thom       (501) staff       (20)     7881 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/docs/conf.py
+-rw-r--r--   0 thom       (501) staff       (20)       62 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/docs/index.rst
+-rw-r--r--   0 thom       (501) staff       (20)      321 2023-07-04 13:23:54.818741 imio.patterns-1.0a4/setup.cfg
+-rw-r--r--   0 thom       (501) staff       (20)     2072 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/setup.py
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.781164 imio.patterns-1.0a4/src/
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.792404 imio.patterns-1.0a4/src/imio/
+-rw-r--r--   0 thom       (501) staff       (20)       80 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/__init__.py
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.799975 imio.patterns-1.0a4/src/imio/patterns/
+-rw-r--r--   0 thom       (501) staff       (20)      130 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/__init__.py
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.800858 imio.patterns-1.0a4/src/imio/patterns/browser/
+-rw-r--r--   0 thom       (501) staff       (20)        0 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/__init__.py
+-rw-r--r--   0 thom       (501) staff       (20)      570 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/configure.zcml
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.801331 imio.patterns-1.0a4/src/imio/patterns/browser/overrides/
+-rw-r--r--   0 thom       (501) staff       (20)        0 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/overrides/.gitkeep
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.801718 imio.patterns-1.0a4/src/imio/patterns/browser/static/
+-rw-r--r--   0 thom       (501) staff       (20)        0 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/.gitkeep
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.802609 imio.patterns-1.0a4/src/imio/patterns/browser/static/css/
+-rw-r--r--   0 thom       (501) staff       (20)      477 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/css/imio-patterns-bundle-compiled.css
+-rwxr-xr-x   0 thom       (501) staff       (20)    10333 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/css/slick.css
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.804581 imio.patterns-1.0a4/src/imio/patterns/browser/static/fonts/
+-rw-r--r--   0 thom       (501) staff       (20)     2048 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/fonts/slick.eot
+-rw-r--r--   0 thom       (501) staff       (20)     2152 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/fonts/slick.svg
+-rw-r--r--   0 thom       (501) staff       (20)     1892 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/fonts/slick.ttf
+-rw-r--r--   0 thom       (501) staff       (20)     1380 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/fonts/slick.woff
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.806137 imio.patterns-1.0a4/src/imio/patterns/browser/static/less/
+-rw-r--r--   0 thom       (501) staff       (20)      193 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/less/imio-patterns-bundle-compiled.less.map
+-rw-r--r--   0 thom       (501) staff       (20)       36 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/less/imio-patterns-bundle.less
+-rw-r--r--   0 thom       (501) staff       (20)      178 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/less/theme-compiled.less.map
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.809452 imio.patterns-1.0a4/src/imio/patterns/browser/static/pattern/
+-rw-r--r--   0 thom       (501) staff       (20)      710 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/pattern/i18n.js
+-rw-r--r--   0 thom       (501) staff       (20)       66 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/pattern/imio-patterns-bundle-compiled.js
+-rw-r--r--   0 thom       (501) staff       (20)      108 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/pattern/imio.pattern.js
+-rw-r--r--   0 thom       (501) staff       (20)     3057 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/pattern/pattern.slick.js
+-rwxr-xr-x   0 thom       (501) staff       (20)    80335 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/pattern/slick.js
+-rwxr-xr-x   0 thom       (501) staff       (20)    42863 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/browser/static/pattern/slick.min.js
+-rw-r--r--   0 thom       (501) staff       (20)     1372 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/configure.zcml
+-rw-r--r--   0 thom       (501) staff       (20)      262 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/interfaces.py
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.811789 imio.patterns-1.0a4/src/imio/patterns/locales/
+-rw-r--r--   0 thom       (501) staff       (20)      611 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/locales/README.rst
+-rw-r--r--   0 thom       (501) staff       (20)        0 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/locales/__init__.py
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.784875 imio.patterns-1.0a4/src/imio/patterns/locales/en/
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.812407 imio.patterns-1.0a4/src/imio/patterns/locales/en/LC_MESSAGES/
+-rw-r--r--   0 thom       (501) staff       (20)        0 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/locales/en/LC_MESSAGES/imio.patterns.po
+-rw-r--r--   0 thom       (501) staff       (20)        0 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/locales/imio.patterns.pot
+-rw-r--r--   0 thom       (501) staff       (20)     1571 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/locales/update.py
+-rwxr-xr-x   0 thom       (501) staff       (20)      476 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/locales/update.sh
+-rw-r--r--   0 thom       (501) staff       (20)      260 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/permissions.zcml
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.785668 imio.patterns-1.0a4/src/imio/patterns/profiles/
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.815099 imio.patterns-1.0a4/src/imio/patterns/profiles/default/
+-rw-r--r--   0 thom       (501) staff       (20)      165 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/profiles/default/browserlayer.xml
+-rw-r--r--   0 thom       (501) staff       (20)      105 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/profiles/default/catalog.xml
+-rw-r--r--   0 thom       (501) staff       (20)      195 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/profiles/default/metadata.xml
+-rw-r--r--   0 thom       (501) staff       (20)     2906 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/profiles/default/registry.xml
+-rw-r--r--   0 thom       (501) staff       (20)      118 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/profiles/default/rolemap.xml
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.815580 imio.patterns-1.0a4/src/imio/patterns/profiles/uninstall/
+-rw-r--r--   0 thom       (501) staff       (20)      123 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 thom       (501) staff       (20)      614 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/setuphandlers.py
+-rw-r--r--   0 thom       (501) staff       (20)     1489 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/testing.py
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.816925 imio.patterns-1.0a4/src/imio/patterns/tests/
+-rw-r--r--   0 thom       (501) staff       (20)        0 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/tests/__init__.py
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.817408 imio.patterns-1.0a4/src/imio/patterns/tests/robot/
+-rw-r--r--   0 thom       (501) staff       (20)     1983 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/tests/robot/test_example.robot
+-rw-r--r--   0 thom       (501) staff       (20)      875 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/tests/test_robot.py
+-rw-r--r--   0 thom       (501) staff       (20)     2395 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/tests/test_setup.py
+-rw-r--r--   0 thom       (501) staff       (20)      205 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/upgrades.py
+-rw-r--r--   0 thom       (501) staff       (20)      382 2023-07-04 13:23:53.000000 imio.patterns-1.0a4/src/imio/patterns/upgrades.zcml
+drwxr-xr-x   0 thom       (501) staff       (20)        0 2023-07-04 13:23:54.796184 imio.patterns-1.0a4/src/imio.patterns.egg-info/
+-rw-r--r--   0 thom       (501) staff       (20)     2590 2023-07-04 13:23:54.000000 imio.patterns-1.0a4/src/imio.patterns.egg-info/PKG-INFO
+-rw-r--r--   0 thom       (501) staff       (20)     2481 2023-07-04 13:23:54.000000 imio.patterns-1.0a4/src/imio.patterns.egg-info/SOURCES.txt
+-rw-r--r--   0 thom       (501) staff       (20)        1 2023-07-04 13:23:54.000000 imio.patterns-1.0a4/src/imio.patterns.egg-info/dependency_links.txt
+-rw-r--r--   0 thom       (501) staff       (20)      118 2023-07-04 13:23:54.000000 imio.patterns-1.0a4/src/imio.patterns.egg-info/entry_points.txt
+-rw-r--r--   0 thom       (501) staff       (20)        5 2023-07-04 13:23:54.000000 imio.patterns-1.0a4/src/imio.patterns.egg-info/namespace_packages.txt
+-rw-r--r--   0 thom       (501) staff       (20)        1 2023-07-04 13:23:54.000000 imio.patterns-1.0a4/src/imio.patterns.egg-info/not-zip-safe
+-rw-r--r--   0 thom       (501) staff       (20)      173 2023-07-04 13:23:54.000000 imio.patterns-1.0a4/src/imio.patterns.egg-info/requires.txt
+-rw-r--r--   0 thom       (501) staff       (20)        5 2023-07-04 13:23:54.000000 imio.patterns-1.0a4/src/imio.patterns.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `imio.patterns-1.0a3/LICENSE.rst` & `imio.patterns-1.0a4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/setup.py` & `imio.patterns-1.0a4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='imio.patterns',
-    version='1.0a3',
+    version='1.0a4',
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
@@ -36,15 +36,14 @@
     url='https://pypi.python.org/pypi/imio.patterns',
     license='GPL version 2',
     packages=find_packages('src', exclude=['ez_setup']),
     namespace_packages=['imio'],
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
-    python_requires="==2.7, >=3.6",
     install_requires=[
         'setuptools',
         # -*- Extra requirements: -*-
         'z3c.jbot',
         'plone.api>=1.8.4',
         'plone.restapi',
         'plone.app.dexterity',
```

### Comparing `imio.patterns-1.0a3/docs/conf.py` & `imio.patterns-1.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio.patterns.egg-info/SOURCES.txt` & `imio.patterns-1.0a4/src/imio.patterns.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGES.rst
 CONTRIBUTORS.rst
 DEVELOP.rst
+LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/conf.py
 docs/index.rst
```

### Comparing `imio.patterns-1.0a3/src/imio/patterns/testing.py` & `imio.patterns-1.0a4/src/imio/patterns/testing.py`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/browser/configure.zcml` & `imio.patterns-1.0a4/src/imio/patterns/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/browser/static/fonts/slick.svg` & `imio.patterns-1.0a4/src/imio/patterns/browser/static/fonts/slick.svg`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/browser/static/fonts/slick.ttf` & `imio.patterns-1.0a4/src/imio/patterns/browser/static/fonts/slick.ttf`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/browser/static/fonts/slick.eot` & `imio.patterns-1.0a4/src/imio/patterns/browser/static/fonts/slick.eot`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/browser/static/fonts/slick.woff` & `imio.patterns-1.0a4/src/imio/patterns/browser/static/fonts/slick.woff`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/browser/static/pattern/slick.js` & `imio.patterns-1.0a4/src/imio/patterns/browser/static/pattern/slick.js`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/browser/static/pattern/slick.min.js` & `imio.patterns-1.0a4/src/imio/patterns/browser/static/pattern/slick.min.js`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/browser/static/pattern/pattern.slick.js` & `imio.patterns-1.0a4/src/imio/patterns/browser/static/pattern/pattern.slick.js`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/browser/static/pattern/i18n.js` & `imio.patterns-1.0a4/src/imio/patterns/browser/static/pattern/i18n.js`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/browser/static/css/slick.css` & `imio.patterns-1.0a4/src/imio/patterns/browser/static/css/slick.css`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/locales/README.rst` & `imio.patterns-1.0a4/src/imio/patterns/locales/README.rst`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/locales/update.py` & `imio.patterns-1.0a4/src/imio/patterns/locales/update.py`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/setuphandlers.py` & `imio.patterns-1.0a4/src/imio/patterns/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/configure.zcml` & `imio.patterns-1.0a4/src/imio/patterns/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/profiles/default/registry.xml` & `imio.patterns-1.0a4/src/imio/patterns/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/tests/robot/test_example.robot` & `imio.patterns-1.0a4/src/imio/patterns/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/tests/test_setup.py` & `imio.patterns-1.0a4/src/imio/patterns/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/src/imio/patterns/tests/test_robot.py` & `imio.patterns-1.0a4/src/imio/patterns/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/README.rst` & `imio.patterns-1.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `imio.patterns-1.0a3/DEVELOP.rst` & `imio.patterns-1.0a4/DEVELOP.rst`

 * *Files identical despite different names*

