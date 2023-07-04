# Comparing `tmp/collective.fullcalendar-1.0b2.tar.gz` & `tmp/collective.fullcalendar-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.fullcalendar-1.0b2.tar", last modified: Sat Dec 11 09:54:08 2021, max compression
+gzip compressed data, was "collective.fullcalendar-1.2.tar", last modified: Tue Jul  4 06:35:14 2023, max compression
```

## Comparing `collective.fullcalendar-1.0b2.tar` & `collective.fullcalendar-1.2.tar`

### file list

```diff
@@ -1,93 +1,96 @@
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.341085 collective.fullcalendar-1.0b2/
--rw-r--r--   0 pbauer     (501) staff       (20)     1926 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/.gitlab-ci.yml
--rw-r--r--   0 pbauer     (501) staff       (20)     1663 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/.travis.yml
--rw-r--r--   0 pbauer     (501) staff       (20)     1113 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/CHANGES.rst
--rw-r--r--   0 pbauer     (501) staff       (20)       95 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/CONTRIBUTORS.rst
--rw-r--r--   0 pbauer     (501) staff       (20)      586 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/DEVELOP.rst
--rw-r--r--   0 pbauer     (501) staff       (20)    18092 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/LICENSE.GPL
--rw-r--r--   0 pbauer     (501) staff       (20)      667 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/LICENSE.rst
--rw-r--r--   0 pbauer     (501) staff       (20)      124 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/MANIFEST.in
--rw-r--r--   0 pbauer     (501) staff       (20)     6211 2021-12-11 09:54:08.341174 collective.fullcalendar-1.0b2/PKG-INFO
--rw-r--r--   0 pbauer     (501) staff       (20)     2584 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/README.rst
--rw-r--r--   0 pbauer     (501) staff       (20)       27 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/constraints.txt
--rw-r--r--   0 pbauer     (501) staff       (20)      105 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/constraints_plone52.txt
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.335440 collective.fullcalendar-1.0b2/docs/
--rw-r--r--   0 pbauer     (501) staff       (20)     7983 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/docs/conf.py
--rw-r--r--   0 pbauer     (501) staff       (20)       92 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/docs/index.rst
--rw-r--r--   0 pbauer     (501) staff       (20)       42 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/requirements.txt
--rw-r--r--   0 pbauer     (501) staff       (20)      495 2021-12-11 09:54:08.341450 collective.fullcalendar-1.0b2/setup.cfg
--rw-r--r--   0 pbauer     (501) staff       (20)     2457 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/setup.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.332495 collective.fullcalendar-1.0b2/src/
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.335549 collective.fullcalendar-1.0b2/src/collective/
--rw-r--r--   0 pbauer     (501) staff       (20)       80 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/__init__.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.337049 collective.fullcalendar-1.0b2/src/collective/fullcalendar/
--rw-r--r--   0 pbauer     (501) staff       (20)      140 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/__init__.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.337345 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/__init__.py
--rw-r--r--   0 pbauer     (501) staff       (20)     1936 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/configure.zcml
--rw-r--r--   0 pbauer     (501) staff       (20)     8942 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/fullcalendar.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.337447 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/overrides/
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/overrides/.gitkeep
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.337530 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/static/
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/static/.gitkeep
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.337613 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/static/css/
--rw-r--r--   0 pbauer     (501) staff       (20)    25473 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/static/css/main.min.css
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.337867 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/static/js/
--rw-r--r--   0 pbauer     (501) staff       (20)    22539 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/static/js/locales-all.min.js
--rw-r--r--   0 pbauer     (501) staff       (20)   268430 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/static/js/main.min.js
--rw-r--r--   0 pbauer     (501) staff       (20)     1429 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/configure.zcml
--rw-r--r--   0 pbauer     (501) staff       (20)      563 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/interfaces.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.338499 collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/
--rw-r--r--   0 pbauer     (501) staff       (20)      611 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/README.rst
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/__init__.py
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/collective.fullcalendar.pot
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.333089 collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/de/
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.338603 collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/de/LC_MESSAGES/
--rw-r--r--   0 pbauer     (501) staff       (20)     2582 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/de/LC_MESSAGES/collective.fullcalendar.po
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.333208 collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/en/
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.338710 collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/en/LC_MESSAGES/
--rw-r--r--   0 pbauer     (501) staff       (20)     2489 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/en/LC_MESSAGES/collective.fullcalendar.po
--rw-r--r--   0 pbauer     (501) staff       (20)     1762 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/update.py
--rwxr-xr-x   0 pbauer     (501) staff       (20)      506 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/update.sh
--rw-r--r--   0 pbauer     (501) staff       (20)      260 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/permissions.zcml
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.333457 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.339346 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/
--rw-r--r--   0 pbauer     (501) staff       (20)     2286 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/actions.xml
--rw-r--r--   0 pbauer     (501) staff       (20)      195 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/browserlayer.xml
--rw-r--r--   0 pbauer     (501) staff       (20)      105 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/catalog.xml
--rw-r--r--   0 pbauer     (501) staff       (20)      195 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/metadata.xml
--rw-r--r--   0 pbauer     (501) staff       (20)     1484 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/registry.xml
--rw-r--r--   0 pbauer     (501) staff       (20)      118 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/rolemap.xml
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.339563 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/types/
--rw-r--r--   0 pbauer     (501) staff       (20)      271 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/types/Collection.xml
--rw-r--r--   0 pbauer     (501) staff       (20)      267 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/types/Folder.xml
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.339670 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/uninstall/
--rw-r--r--   0 pbauer     (501) staff       (20)      133 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 pbauer     (501) staff       (20)      623 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/setuphandlers.py
--rw-r--r--   0 pbauer     (501) staff       (20)     1574 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/testing.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.340170 collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/__init__.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.340270 collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/robot/
--rw-r--r--   0 pbauer     (501) staff       (20)     2023 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/robot/test_example.robot
--rw-r--r--   0 pbauer     (501) staff       (20)      964 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/test_robot.py
--rw-r--r--   0 pbauer     (501) staff       (20)     2453 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/test_setup.py
--rw-r--r--   0 pbauer     (501) staff       (20)     1543 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/test_view_edit_event.py
--rw-r--r--   0 pbauer     (501) staff       (20)     1602 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/test_view_fullcalendar_view.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.340994 collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/__init__.py
--rw-r--r--   0 pbauer     (501) staff       (20)      765 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/add_event_view.py
--rw-r--r--   0 pbauer     (501) staff       (20)     1115 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/configure.zcml
--rw-r--r--   0 pbauer     (501) staff       (20)      445 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/edit_event.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     2932 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/edit_event.py
--rw-r--r--   0 pbauer     (501) staff       (20)     4234 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/fullcalendar_view.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     5869 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/fullcalendar_view.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2021-12-11 09:54:08.336415 collective.fullcalendar-1.0b2/src/collective.fullcalendar.egg-info/
--rw-r--r--   0 pbauer     (501) staff       (20)     6211 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective.fullcalendar.egg-info/PKG-INFO
--rw-r--r--   0 pbauer     (501) staff       (20)     2991 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective.fullcalendar.egg-info/SOURCES.txt
--rw-r--r--   0 pbauer     (501) staff       (20)        1 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective.fullcalendar.egg-info/dependency_links.txt
--rw-r--r--   0 pbauer     (501) staff       (20)      148 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective.fullcalendar.egg-info/entry_points.txt
--rw-r--r--   0 pbauer     (501) staff       (20)       11 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective.fullcalendar.egg-info/namespace_packages.txt
--rw-r--r--   0 pbauer     (501) staff       (20)        1 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective.fullcalendar.egg-info/not-zip-safe
--rw-r--r--   0 pbauer     (501) staff       (20)      173 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective.fullcalendar.egg-info/requires.txt
--rw-r--r--   0 pbauer     (501) staff       (20)       11 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/src/collective.fullcalendar.egg-info/top_level.txt
--rw-r--r--   0 pbauer     (501) staff       (20)     3642 2021-12-11 09:54:08.000000 collective.fullcalendar-1.0b2/tox.ini
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.083519 collective.fullcalendar-1.2/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1926 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/.gitlab-ci.yml
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1663 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/.travis.yml
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1425 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/CHANGES.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)      128 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/CONTRIBUTORS.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)      586 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/DEVELOP.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)    18092 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/LICENSE.GPL
+-rw-r--r--   0 katjasuss   (501) staff       (20)      667 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/LICENSE.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)      124 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/MANIFEST.in
+-rw-r--r--   0 katjasuss   (501) staff       (20)     3563 2023-07-04 06:35:14.083648 collective.fullcalendar-1.2/PKG-INFO
+-rw-r--r--   0 katjasuss   (501) staff       (20)      830 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/README.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)       27 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/constraints.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)      105 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/constraints_plone52.txt
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.071273 collective.fullcalendar-1.2/docs/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     7983 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/docs/conf.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)       92 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/docs/index.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)       42 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/requirements.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)      495 2023-07-04 06:35:14.084270 collective.fullcalendar-1.2/setup.cfg
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2603 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/setup.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.064566 collective.fullcalendar-1.2/src/
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.071494 collective.fullcalendar-1.2/src/collective/
+-rw-r--r--   0 katjasuss   (501) staff       (20)       80 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/__init__.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.074672 collective.fullcalendar-1.2/src/collective/fullcalendar/
+-rw-r--r--   0 katjasuss   (501) staff       (20)      140 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/__init__.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.075302 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/__init__.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1936 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/configure.zcml
+-rw-r--r--   0 katjasuss   (501) staff       (20)     8860 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/fullcalendar.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.075535 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/overrides/
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/overrides/.gitkeep
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.075725 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/static/
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/static/.gitkeep
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.075920 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/static/css/
+-rw-r--r--   0 katjasuss   (501) staff       (20)    25473 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/static/css/main.min.css
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.076446 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/static/js/
+-rw-r--r--   0 katjasuss   (501) staff       (20)    22539 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/static/js/locales-all.min.js
+-rw-r--r--   0 katjasuss   (501) staff       (20)   268430 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/browser/static/js/main.min.js
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1429 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/configure.zcml
+-rw-r--r--   0 katjasuss   (501) staff       (20)      577 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/interfaces.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.077853 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/
+-rw-r--r--   0 katjasuss   (501) staff       (20)      611 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/README.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/__init__.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     4722 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/collective.fullcalendar.pot
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.065882 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/de/
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.078076 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/de/LC_MESSAGES/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     5765 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/de/LC_MESSAGES/collective.fullcalendar.po
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.066141 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/en/
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.078309 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/en/LC_MESSAGES/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     5672 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/en/LC_MESSAGES/collective.fullcalendar.po
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.066399 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/no/
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.078542 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/no/LC_MESSAGES/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     5882 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/no/LC_MESSAGES/collective.fullcalendar.po
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1762 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/update.py
+-rwxr-xr-x   0 katjasuss   (501) staff       (20)      506 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/locales/update.sh
+-rw-r--r--   0 katjasuss   (501) staff       (20)      260 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/permissions.zcml
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.066944 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.079852 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2262 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/actions.xml
+-rw-r--r--   0 katjasuss   (501) staff       (20)      195 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/browserlayer.xml
+-rw-r--r--   0 katjasuss   (501) staff       (20)      105 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/catalog.xml
+-rw-r--r--   0 katjasuss   (501) staff       (20)      195 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/metadata.xml
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1484 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/registry.xml
+-rw-r--r--   0 katjasuss   (501) staff       (20)      118 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/rolemap.xml
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.080299 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/types/
+-rw-r--r--   0 katjasuss   (501) staff       (20)      271 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/types/Collection.xml
+-rw-r--r--   0 katjasuss   (501) staff       (20)      267 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/types/Folder.xml
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.080528 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/uninstall/
+-rw-r--r--   0 katjasuss   (501) staff       (20)      133 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 katjasuss   (501) staff       (20)      623 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/setuphandlers.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1574 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/testing.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.081609 collective.fullcalendar-1.2/src/collective/fullcalendar/tests/
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/tests/__init__.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.081831 collective.fullcalendar-1.2/src/collective/fullcalendar/tests/robot/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2025 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/tests/robot/test_example.robot
+-rw-r--r--   0 katjasuss   (501) staff       (20)      964 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/tests/test_robot.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2453 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/tests/test_setup.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1543 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/tests/test_view_edit_event.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1602 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/tests/test_view_fullcalendar_view.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.083330 collective.fullcalendar-1.2/src/collective/fullcalendar/views/
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/views/__init__.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      766 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/views/add_event_view.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1115 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/views/configure.zcml
+-rw-r--r--   0 katjasuss   (501) staff       (20)      445 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/views/edit_event.pt
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2932 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/views/edit_event.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     3886 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/views/fullcalendar_view.pt
+-rw-r--r--   0 katjasuss   (501) staff       (20)     6181 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/src/collective/fullcalendar/views/fullcalendar_view.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-04 06:35:14.073324 collective.fullcalendar-1.2/src/collective.fullcalendar.egg-info/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     3563 2023-07-04 06:35:13.000000 collective.fullcalendar-1.2/src/collective.fullcalendar.egg-info/PKG-INFO
+-rw-r--r--   0 katjasuss   (501) staff       (20)     3069 2023-07-04 06:35:14.000000 collective.fullcalendar-1.2/src/collective.fullcalendar.egg-info/SOURCES.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)        1 2023-07-04 06:35:13.000000 collective.fullcalendar-1.2/src/collective.fullcalendar.egg-info/dependency_links.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)      128 2023-07-04 06:35:13.000000 collective.fullcalendar-1.2/src/collective.fullcalendar.egg-info/entry_points.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)       11 2023-07-04 06:35:13.000000 collective.fullcalendar-1.2/src/collective.fullcalendar.egg-info/namespace_packages.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)        1 2023-07-04 06:35:13.000000 collective.fullcalendar-1.2/src/collective.fullcalendar.egg-info/not-zip-safe
+-rw-r--r--   0 katjasuss   (501) staff       (20)      173 2023-07-04 06:35:13.000000 collective.fullcalendar-1.2/src/collective.fullcalendar.egg-info/requires.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)       11 2023-07-04 06:35:13.000000 collective.fullcalendar-1.2/src/collective.fullcalendar.egg-info/top_level.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)     3642 2023-07-04 06:35:12.000000 collective.fullcalendar-1.2/tox.ini
```

### Comparing `collective.fullcalendar-1.0b2/.gitlab-ci.yml` & `collective.fullcalendar-1.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/.travis.yml` & `collective.fullcalendar-1.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/DEVELOP.rst` & `collective.fullcalendar-1.2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/LICENSE.GPL` & `collective.fullcalendar-1.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/LICENSE.rst` & `collective.fullcalendar-1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/docs/conf.py` & `collective.fullcalendar-1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/setup.py` & `collective.fullcalendar-1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,30 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.fullcalendar",
-    version="1.0b2",
+    version="1.2",
     description="Fullcalendar for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords="Python Plone CMS",
     author="Werkbank GmbH",
     author_email="mail@werkbank.de",
     url="https://github.com/collective/collective.fullcalendar",
@@ -43,15 +47,14 @@
     },
     license="GPL version 2",
     packages=find_packages("src", exclude=["ez_setup"]),
     namespace_packages=["collective"],
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
-    python_requires="==2.7, >=3.6",
     install_requires=[
         "setuptools",
         # -*- Extra requirements: -*-
         "z3c.jbot",
         "plone.api>=1.8.4",
         "plone.restapi",
         "plone.app.dexterity",
```

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/configure.zcml` & `collective.fullcalendar-1.2/src/collective/fullcalendar/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/fullcalendar.py` & `collective.fullcalendar-1.2/src/collective/fullcalendar/browser/fullcalendar.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,40 +44,40 @@
         vocabulary=SimpleVocabulary.fromValues(
             ["dayGridMonth", "timeGridWeek", "listWeek", "dayGridWeek"]
         ),
         default="dayGridMonth",
     )
     # Possible for headerLeft/headerRight: title, prev, next, prevYear, nextYear, today, dayGridMonth, timeGridWeek, listWeek, dayGridWeek
     headerLeft = schema.TextLine(
-        title=_(u"label_headerLeft", default=u"Kopfbereich links"),
+        title=_(u"label_headerLeft", default=u"Head area left"),
         description=_(
             u"help_headerLeft",
-            default=u"Mögliche Werte: title, prev, next, prevYear, nextYear, today, dayGridMonth, timeGridWeek, listWeek, dayGridWeek",
+            default=u"Possible values: title, prev, next, prevYear, nextYear, today, dayGridMonth, timeGridWeek, listWeek, dayGridWeek",
         ),
         required=False,
         default="prev,next today",
     )
     headerRight = schema.TextLine(
-        title=_(u"label_headerRight", default=u"Kopfbereich rechts"),
+        title=_(u"label_headerRight", default=u"Head area right"),
         description=_(
             u"help_headerRight",
-            default=u"Mögliche Werte: title, prev, next, prevYear, nextYear, today, dayGridMonth, timeGridWeek, listWeek, dayGridWeek",
+            default=u"Possible values: title, prev, next, prevYear, nextYear, today, dayGridMonth, timeGridWeek, listWeek, dayGridWeek",
         ),
         required=False,
         default="dayGridMonth timeGridWeek listWeek",
     )
     weekends = schema.Bool(
-        title=_(u"label_weekends", default=u"Wochenenden anzeigen"),
-        description=_(u"help_weekends", default=u"Wochenenden anzeigen"),
+        title=_(u"label_weekends", default=u"Show weekends"),
+        description=_(u"help_weekends", default=u"Show weekends"),
         required=False,
         default=True,
     )
     firstDay = schema.Choice(
-        title=_(u"label_firstDay", default=u"Erster Wochentag"),
-        description=_(u"help_firstDay", default=u"Erster Wochentag"),
+        title=_(u"label_firstDay", default=u"First day of the week"),
+        description=_(u"help_firstDay", default=u"Choose the first day of the week."),
         required=True,
         vocabulary=SimpleVocabulary(
             [
                 SimpleTerm(value=pair[0], token=pair[0], title=pair[1])
                 for pair in [
                     (0, u"sunday"),
                     (1, u"monday"),
@@ -88,44 +88,44 @@
                     (6, u"saturday"),
                 ]
             ]
         ),
         default=1,
     )
     firstHour = schema.TextLine(
-        title=_(u"label_firstHour", default=u"Erste angezeigte Stunde"),
+        title=_(u"label_firstHour", default=u"First visible hour"),
         description=_(
             u"help_firstHour",
-            default=u'Legen Sie die anfängliche Scrollposition der Kalender-Tagesansicht fest (eine Zahl zwischen 0 und 23). Wenn vor dieser Zahl ein "+" oder "-" steht, wird die Zahl mit der aktuellen Zeit addiert bzw. substrahiert.',
+            default=u'Set the starting calendar day view scroll position (a number between 0 and 23). If there is a "+" or "-" in front of this number, the number is added or subtracted with the current time.',
         ),
         required=True,
         default="6",
     )
     minTime = schema.TextLine(
-        title=_(u"label_minTime", default=u"Erste sichtbare Stunde"),
+        title=_(u"label_minTime", default=u"First visible hour"),
         description=_(
             u"help_minTime",
-            default=u"Wählen Sie die erste sichtbare Stunde des Kalenders (z.B. '5' oder '5:30').",
+            default=u"Select the first visible hour of the calendar (e.g. '5' or '5:30').",
         ),
         required=True,
         default="00:00:00",
     )
     maxTime = schema.TextLine(
-        title=_(u"label_maxTime", default=u"Letzte sichtbare Stunde"),
+        title=_(u"label_maxTime", default=u"Last visible hour"),
         description=_(
             u"help_maxTime",
-            default=u"Wählen Sie die letzte sichtbare Stunde des Kalenders (z.B. '5' oder '5:30').",
+            default=u"Select the last visible hour of the calendar (e.g. '5' oder '5:30').",
         ),
         required=True,
         default="24:00:00",
     )
     # Target for new events
     target_folder = RelationChoice(
-        title=_(u"label_target_folder", default=u"Zielordner für neue Termine"),
-        description=_(u"help_target_folder", default=u"Zielordner für neue Termine"),
+        title=_(u"label_target_folder", default=u"Destination folder for new appointments"),
+        description=_(u"help_target_folder", default=u"Destination folder for new appointments"),
         vocabulary="plone.app.vocabularies.Catalog",
         required=False,
     )
     directives.widget(
         "target_folder",
         RelatedItemsFieldWidget,
         pattern_options={
@@ -139,21 +139,21 @@
             u"help_event_type",
             default=u"Or leave blank for default event type 'Event'.",
         ),
         vocabulary="plone.app.vocabularies.PortalTypes",
         required=False,
         default="Event",
     )
-    # Höhe des Kalenders
+    # Height of Calendar
     calendarHeight = schema.Int(
         title=_(u"label_calendarHeight", default=u"Calendar height"),
         description=_(u"help_calendarHeight", default=u"Calendar height in pixels"),
         required=False,
     )
-    # Bearbeitung von Terminen erlauben
+    # Enable editing on events
     caleditable = schema.Bool(
         title=_(u"label_caleditable", default=u"Calendar editable"),
         description=_(
             u"help_caleditable",
             default=u"Check this box if you want the events in the calendar to be editable.",
         ),
         required=False,
@@ -190,23 +190,21 @@
         IStatusMessage(self.request).addStatusMessage(_(u"Changes canceled."), "info")
         self.request.response.redirect(
             "%s/%s" % (self.context.absolute_url(), "@@fullcalendar_settings")
         )
 
 
 class IFullcalendarTool(BrowserView):
-    @property
+
     def available(self):
         return IDexterityContainer.providedBy(self.context) or ISyndicatableCollection.providedBy(self.context)
 
-    @property
     def available_disabled(self):
-        return self.available and not self.enabled
+        return self.available() and not self.enabled()
 
-    @property
     def enabled(self):
         return IFullcalendarEnabled.providedBy(self.context)
 
 
 class FullcalendarSettingsFormView(FormWrapper):
     form = FullcalendarSettingsForm
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/static/css/main.min.css` & `collective.fullcalendar-1.2/src/collective/fullcalendar/browser/static/css/main.min.css`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/static/js/locales-all.min.js` & `collective.fullcalendar-1.2/src/collective/fullcalendar/browser/static/js/locales-all.min.js`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/browser/static/js/main.min.js` & `collective.fullcalendar-1.2/src/collective/fullcalendar/browser/static/js/main.min.js`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/configure.zcml` & `collective.fullcalendar-1.2/src/collective/fullcalendar/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/interfaces.py` & `collective.fullcalendar-1.2/src/collective/fullcalendar/interfaces.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 """Module where all interfaces, events and exceptions live."""
-
+from zope.interface import Interface
 from zope.publisher.interfaces.browser import IDefaultBrowserLayer
 
 
 class ICollectiveFullcalendarLayer(IDefaultBrowserLayer):
     """Marker interface that defines a browser layer."""
 
 
-class IFullcalendarEnabled(IDefaultBrowserLayer):
+class IFullcalendarEnabled(Interface):
     """Marker interface for Fullcalendar possibilities."""
 
 
-class IFullcalenderEnabled(IDefaultBrowserLayer):
+class IFullcalenderEnabled(Interface):
     """Marker interface for Fullcalendar possibilities.
 
     Backward compatibility
     - renaming calender to calendar
     """
```

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/README.rst` & `collective.fullcalendar-1.2/src/collective/fullcalendar/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/locales/update.py` & `collective.fullcalendar-1.2/src/collective/fullcalendar/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/actions.xml` & `collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/actions.xml`

 * *Files 8% similar despite different names*

#### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/actions.xml` & `collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/actions.xml`

```diff
@@ -2,37 +2,37 @@
 <object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="portal_actions" meta_type="Plone Actions Tool">
   <object name="object" meta_type="CMF Action Category">
     <object name="fullcalendar_settings" meta_type="CMF Action" i18n:domain="plone">
       <property name="title" i18n:translate="title_fullcalendar">Fullcalendar Settings</property>
       <property name="description" i18n:translate="help_fullcalendar">Set setting for Fullcalendar.</property>
       <property name="url_expr">string:${object_url}/@@fullcalendar_settings</property>
       <property name="icon_expr"/>
-      <property name="available_expr">object/@@fullcalendar_tool/enabled|nothing</property>
+      <property name="available_expr">object/@@fullcalendar_tool/enabled</property>
       <property name="permissions">
         <element value="plone.app.event: Import Ical"/>
       </property>
       <property name="visible">True</property>
     </object>
   </object>
   <object name="object_buttons" meta_type="CMF Action Category">
     <object name="fullcalendar_enable" meta_type="CMF Action" i18n:domain="plone">
       <property name="title" i18n:translate="title_fullcalendar_enable">Enable fullcalendar</property>
       <property name="description" i18n:translate="help_fullcalendar_enable">Click to enable the fullcalendar feature on this context.</property>
       <property name="url_expr">string:$object_url/@@fullcalendar_settings/enable</property>
-      <property name="available_expr">object/@@fullcalendar_tool/available_disabled|nothing</property>
+      <property name="available_expr">object/@@fullcalendar_tool/available_disabled</property>
       <property name="permissions">
         <element value="plone.app.event: Import Ical"/>
       </property>
       <property name="visible">True</property>
     </object>
     <object name="fullcalendar_disable" meta_type="CMF Action" i18n:domain="plone">
       <property name="title" i18n:translate="title_fullcalendar_disable">Disable fullcalendar</property>
       <property name="description" i18n:translate="help_fullcalendar_disable">Click to disable the fullcalendar feature on this context.</property>
       <property name="url_expr">string:$object_url/@@fullcalendar_settings/disable</property>
-      <property name="available_expr">object/@@fullcalendar_tool/enabled|nothing</property>
+      <property name="available_expr">object/@@fullcalendar_tool/enabled</property>
       <property name="permissions">
         <element value="plone.app.event: Import Ical"/>
       </property>
       <property name="visible">True</property>
     </object>
   </object>
 </object>
```

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/profiles/default/registry.xml` & `collective.fullcalendar-1.2/src/collective/fullcalendar/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/setuphandlers.py` & `collective.fullcalendar-1.2/src/collective/fullcalendar/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/testing.py` & `collective.fullcalendar-1.2/src/collective/fullcalendar/testing.py`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/robot/test_example.robot` & `collective.fullcalendar-1.2/src/collective/fullcalendar/tests/robot/test_example.robot`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # $ bin/robot-server --reload-path src collective.fullcalendar.testing.COLLECTIVE_FULLCALENDAR_ACCEPTANCE_TESTING
 #
 # 2) Run robot tests:
 #
 # $ bin/robot src/collective/fullcalendar/tests/robot/test_example.robot
 #
-# See the http://docs.plone.org for further details (search for robot
+# See the https://docs.plone.org/ for further details (search for robot
 # framework).
 #
 # ============================================================================
 
 *** Settings *****************************************************************
 
 Resource  plone/app/robotframework/selenium.robot
```

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/test_robot.py` & `collective.fullcalendar-1.2/src/collective/fullcalendar/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/test_setup.py` & `collective.fullcalendar-1.2/src/collective/fullcalendar/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/test_view_edit_event.py` & `collective.fullcalendar-1.2/src/collective/fullcalendar/tests/test_view_edit_event.py`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/tests/test_view_fullcalendar_view.py` & `collective.fullcalendar-1.2/src/collective/fullcalendar/tests/test_view_fullcalendar_view.py`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/add_event_view.py` & `collective.fullcalendar-1.2/src/collective/fullcalendar/views/add_event_view.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
             self.widgets['IEventBasic.end'].value = infos['end']
 
         if 'allDay' in infos and infos['allDay'] == 'true':
             self.widgets['IEventBasic.whole_day'].value = ('selected',)
 
 
 class AddView(add.DefaultAddView):
-    form = AddForm
+    form = AddForm
```

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/configure.zcml` & `collective.fullcalendar-1.2/src/collective/fullcalendar/views/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/edit_event.py` & `collective.fullcalendar-1.2/src/collective/fullcalendar/views/edit_event.py`

 * *Files identical despite different names*

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/fullcalendar_view.pt` & `collective.fullcalendar-1.2/src/collective/fullcalendar/views/fullcalendar_view.pt`

 * *Files 22% similar despite different names*

```diff
@@ -41,54 +41,49 @@
             var calendarEditArea = $('#calendarEditArea');
             var parentURL = '<tal:block tal:content="structure python:context.aq_parent.absolute_url()" />';
 
             var calendar = new FullCalendar.Calendar(calendarElement, <tal:block tal:content="structure python:view.calendar_config()" />);
 
             calendar.render();
 
-
-            // Klick auf einen Slot. Bei Monatsansicht wird ganztägiger Termin erstellt, ansonsten Termin in Slotgröße
             calendar.on('dateClick', function(info) {
                 date = info.dateStr;
                 allDay = info.allDay;
                 var href = calendarAddLink.getAttribute('href');
                 var url = new URL(href);
                 url.searchParams.delete('start')
                 url.searchParams.delete('end')
                 url.searchParams.set('date', date);
                 url.searchParams.set('allDay', allDay);
                 calendarAddLink.setAttribute('href', url);
                 calendarAddLink.click();
             });
 
-            // Auswahl eines Bereichs: Bei Monatsansicht werden mehrtägige Termine erstellt, ansonsten Termin in Bereichsgröße
             calendar.on('select', function(info) {
                 start = info.startStr;
                 end = info.endStr;
                 allDay = info.allDay;
                 var href = calendarAddLink.getAttribute('href');
                 var url = new URL(href);
                 url.searchParams.set('start', start);
                 url.searchParams.set('end', end);
                 url.searchParams.delete('date')
                 url.searchParams.set('allDay', allDay);
                 calendarAddLink.setAttribute('href', url);
                 calendarAddLink.click();
             });
 
-            // Vergrößern/Verkleinern eines Termins
             calendar.on('eventResize', function(info) {
                 if (confirm("Do you want to change the event?")) {
                     window.location.href = "@@edit-event?method=resize&uid="+info.event.id+"&new_end="+info.event.end.toISOString();
                 } else {
                     info.revert();
                 }
             });
 
-            // Verschieben eines Termins
             calendar.on('eventDrop', function(info) {
                 if (confirm("Do you want to change the event?")) {
                     window.location.href = "@@edit-event?method=move&uid="+info.event.id+"&new_start="+info.event.start.toISOString()+"&new_end="+info.event.end.toISOString();
                 } else {
                     info.revert();
                 }
             });
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `collective.fullcalendar-1.0b2/src/collective/fullcalendar/views/fullcalendar_view.py` & `collective.fullcalendar-1.2/src/collective/fullcalendar/views/fullcalendar_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 from collective.fullcalendar.browser.fullcalendar import IIFullcalendarSettings
 from DateTime import DateTime
 from datetime import timedelta
 from plone import api
 from plone.app.contenttypes.behaviors.collection import ISyndicatableCollection
 from plone.app.event.base import get_events
-from plone.app.event.base import RET_MODE_BRAINS
+from plone.app.event.base import RET_MODE_OBJECTS
 from plone.dexterity.interfaces import IDexterityContainer
-from plone.event.interfaces import IEvent
+from plone.event.interfaces import IEvent, IOccurrence
 from Products.Five.browser import BrowserView
 
 
 class FullcalendarView(BrowserView):
     def __call__(self):
         return self.index()
 
@@ -40,24 +40,29 @@
 
     def _get_events(self):
         if ISyndicatableCollection.providedBy(self.context):
             # Filter out non-events. Assume all event-types provde IEvent
             # Do not limit and batch results...
             custom_query = {'object_provides': IEvent.__identifier__}
             brains = self.context.results(batch=False, custom_query=custom_query, limit=10000)
+            objects = [brain.getObject() for brain in brains]
         elif IDexterityContainer.providedBy(self.context):
             path = "/".join(self.context.getPhysicalPath())
-            brains = get_events(self.context, expand=True, path=path)
+            objects = get_events(self.context, ret_mode=RET_MODE_OBJECTS, expand=True, path=path)
         results = []
-        for brain in brains:
+        for obj in objects:
             result = {}
-            obj = brain.getObject()
             result["id"] = obj.UID()
             result["title"] = obj.Title()
             result["url"] = obj.absolute_url()
+            if IOccurrence.providedBy(obj):
+                state = api.content.get_state(obj.aq_parent)
+            else:
+                state = api.content.get_state(obj)
+            result["className"] = "state-{}".format(state)
             if obj.whole_day:
                 result["start"] = obj.start.strftime("%Y-%m-%d")
                 # Fullcalendar counts to end date 00:00
                 end = obj.end + timedelta(days=1)
                 result["end"] = end.strftime("%Y-%m-%d")
             else:
                 result["start"] = obj.start.strftime("%Y-%m-%d %H:%M:%S")
@@ -109,21 +114,21 @@
             else:
                 if firstHourInt > 23:
                     firstHourInt = 23
                 result = str(firstHourInt) + ":00:00"
         return result
 
     def get_time(self, time):
-        if time.isdigit():  # Volle Stunde
+        if time.isdigit():  # full hour
             timeInt = int(time)
             if timeInt < 10:
                 result = "0" + time + ":00"
             else:
                 result = time + ":00"
-        else:  # Krumme Angabe, z.B. '5:30'
+        else:  # half hour or other datetimes, e.g. '5:30'
             if len(time) == 4:
                 result = "0" + time
             else:
                 result = time
         return result
 
     def get_editable(self):
```

### Comparing `collective.fullcalendar-1.0b2/src/collective.fullcalendar.egg-info/SOURCES.txt` & `collective.fullcalendar-1.2/src/collective.fullcalendar.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 src/collective/fullcalendar/locales/README.rst
 src/collective/fullcalendar/locales/__init__.py
 src/collective/fullcalendar/locales/collective.fullcalendar.pot
 src/collective/fullcalendar/locales/update.py
 src/collective/fullcalendar/locales/update.sh
 src/collective/fullcalendar/locales/de/LC_MESSAGES/collective.fullcalendar.po
 src/collective/fullcalendar/locales/en/LC_MESSAGES/collective.fullcalendar.po
+src/collective/fullcalendar/locales/no/LC_MESSAGES/collective.fullcalendar.po
 src/collective/fullcalendar/profiles/default/actions.xml
 src/collective/fullcalendar/profiles/default/browserlayer.xml
 src/collective/fullcalendar/profiles/default/catalog.xml
 src/collective/fullcalendar/profiles/default/metadata.xml
 src/collective/fullcalendar/profiles/default/registry.xml
 src/collective/fullcalendar/profiles/default/rolemap.xml
 src/collective/fullcalendar/profiles/default/types/Collection.xml
```

### Comparing `collective.fullcalendar-1.0b2/tox.ini` & `collective.fullcalendar-1.2/tox.ini`

 * *Files identical despite different names*

