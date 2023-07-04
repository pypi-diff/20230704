# Comparing `tmp/djangocms-audio-2.1.0.tar.gz` & `tmp/djangocms-audio-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-audio-2.1.0.tar", last modified: Thu Jun 29 13:09:46 2023, max compression
+gzip compressed data, was "djangocms-audio-2.1.1.tar", last modified: Tue Jul  4 00:13:38 2023, max compression
```

## Comparing `djangocms-audio-2.1.0.tar` & `djangocms-audio-2.1.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.807745 djangocms-audio-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-29 13:09:46.807745 djangocms-audio-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/cms_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.799745 djangocms-audio-2.1.0/djangocms_audio/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.799745 djangocms-audio-2.1.0/djangocms_audio/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.799745 djangocms-audio-2.1.0/djangocms_audio/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.799745 djangocms-audio-2.1.0/djangocms_audio/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.799745 djangocms-audio-2.1.0/djangocms_audio/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.799745 djangocms-audio-2.1.0/djangocms_audio/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.807745 djangocms-audio-2.1.0/djangocms_audio/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/migrations/0002_auto_20160825_1821.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/migrations/0003_alter_audiofile_cmsplugin_ptr_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.807745 djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/audio_player.html
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/folder.html
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/track.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.803745 djangocms-audio-2.1.0/djangocms_audio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-29 13:09:46.000000 djangocms-audio-2.1.0/djangocms_audio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-29 13:09:46.000000 djangocms-audio-2.1.0/djangocms_audio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:09:46.000000 djangocms-audio-2.1.0/djangocms_audio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:09:46.000000 djangocms-audio-2.1.0/djangocms_audio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-29 13:09:46.000000 djangocms-audio-2.1.0/djangocms_audio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 13:09:46.000000 djangocms-audio-2.1.0/djangocms_audio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:09:46.807745 djangocms-audio-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:46.807745 djangocms-audio-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-06-29 13:09:35.000000 djangocms-audio-2.1.0/tests/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.504977 djangocms-audio-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-04 00:13:38.504977 djangocms-audio-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.500977 djangocms-audio-2.1.1/djangocms_audio/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.496977 djangocms-audio-2.1.1/djangocms_audio/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.496977 djangocms-audio-2.1.1/djangocms_audio/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.500977 djangocms-audio-2.1.1/djangocms_audio/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.496977 djangocms-audio-2.1.1/djangocms_audio/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.500977 djangocms-audio-2.1.1/djangocms_audio/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.496977 djangocms-audio-2.1.1/djangocms_audio/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.500977 djangocms-audio-2.1.1/djangocms_audio/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.496977 djangocms-audio-2.1.1/djangocms_audio/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.500977 djangocms-audio-2.1.1/djangocms_audio/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.496977 djangocms-audio-2.1.1/djangocms_audio/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.500977 djangocms-audio-2.1.1/djangocms_audio/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.500977 djangocms-audio-2.1.1/djangocms_audio/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/migrations/0002_auto_20160825_1821.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/migrations/0003_alter_audiofile_cmsplugin_ptr_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.496977 djangocms-audio-2.1.1/djangocms_audio/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.496977 djangocms-audio-2.1.1/djangocms_audio/templates/djangocms_audio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.500977 djangocms-audio-2.1.1/djangocms_audio/templates/djangocms_audio/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/templates/djangocms_audio/default/audio_player.html
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/templates/djangocms_audio/default/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/templates/djangocms_audio/default/folder.html
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/djangocms_audio/templates/djangocms_audio/default/track.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.500977 djangocms-audio-2.1.1/djangocms_audio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-04 00:13:38.000000 djangocms-audio-2.1.1/djangocms_audio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-04 00:13:38.000000 djangocms-audio-2.1.1/djangocms_audio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:13:38.000000 djangocms-audio-2.1.1/djangocms_audio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 00:13:38.000000 djangocms-audio-2.1.1/djangocms_audio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-04 00:13:38.000000 djangocms-audio-2.1.1/djangocms_audio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 00:13:38.000000 djangocms-audio-2.1.1/djangocms_audio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 00:13:38.504977 djangocms-audio-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:38.504977 djangocms-audio-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-04 00:13:24.000000 djangocms-audio-2.1.1/tests/test_plugins.py
```

### Comparing `djangocms-audio-2.1.0/LICENSE` & `djangocms-audio-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/PKG-INFO` & `djangocms-audio-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-audio
-Version: 2.1.0
+Version: 2.1.1
 Summary: Adds audio plugin to django CMS.
 Home-page: https://github.com/django-cms/djangocms-audio
 Author: Divio AG
 Author-email: info@divio.com
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-audio-2.1.0/README.rst` & `djangocms-audio-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/cms_plugins.py` & `djangocms-audio-2.1.1/djangocms_audio/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/locale/de/LC_MESSAGES/django.mo` & `djangocms-audio-2.1.1/djangocms_audio/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/locale/de/LC_MESSAGES/django.po` & `djangocms-audio-2.1.1/djangocms_audio/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/locale/en/LC_MESSAGES/django.mo` & `djangocms-audio-2.1.1/djangocms_audio/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/locale/en/LC_MESSAGES/django.po` & `djangocms-audio-2.1.1/djangocms_audio/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/locale/es/LC_MESSAGES/django.po` & `djangocms-audio-2.1.1/djangocms_audio/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/locale/fr/LC_MESSAGES/django.mo` & `djangocms-audio-2.1.1/djangocms_audio/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/locale/fr/LC_MESSAGES/django.po` & `djangocms-audio-2.1.1/djangocms_audio/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/locale/it/LC_MESSAGES/django.po` & `djangocms-audio-2.1.1/djangocms_audio/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/migrations/0001_initial.py` & `djangocms-audio-2.1.1/djangocms_audio/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/migrations/0002_auto_20160825_1821.py` & `djangocms-audio-2.1.1/djangocms_audio/migrations/0002_auto_20160825_1821.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/migrations/0003_alter_audiofile_cmsplugin_ptr_and_more.py` & `djangocms-audio-2.1.1/djangocms_audio/migrations/0003_alter_audiofile_cmsplugin_ptr_and_more.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/models.py` & `djangocms-audio-2.1.1/djangocms_audio/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/file.html` & `djangocms-audio-2.1.1/djangocms_audio/templates/djangocms_audio/default/file.html`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/folder.html` & `djangocms-audio-2.1.1/djangocms_audio/templates/djangocms_audio/default/folder.html`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio/templates/djangocms_audio/default/track.html` & `djangocms-audio-2.1.1/djangocms_audio/templates/djangocms_audio/default/track.html`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/djangocms_audio.egg-info/PKG-INFO` & `djangocms-audio-2.1.1/djangocms_audio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-audio
-Version: 2.1.0
+Version: 2.1.1
 Summary: Adds audio plugin to django CMS.
 Home-page: https://github.com/django-cms/djangocms-audio
 Author: Divio AG
 Author-email: info@divio.com
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-audio-2.1.0/djangocms_audio.egg-info/SOURCES.txt` & `djangocms-audio-2.1.1/djangocms_audio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/setup.py` & `djangocms-audio-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from setuptools import find_packages, setup
 
 from djangocms_audio import __version__
 
 REQUIREMENTS = [
     'django-cms>=3.7',
     'django-filer>=1.7',
-    'djangocms-attributes-field>=1',
-    'django-treebeard>=4.3,<4.5',
+    'djangocms-attributes-field>=1'
 ]
 
 
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
```

### Comparing `djangocms-audio-2.1.0/tests/helpers.py` & `djangocms-audio-2.1.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/tests/test_migrations.py` & `djangocms-audio-2.1.1/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/tests/test_models.py` & `djangocms-audio-2.1.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-audio-2.1.0/tests/test_plugins.py` & `djangocms-audio-2.1.1/tests/test_plugins.py`

 * *Files identical despite different names*

