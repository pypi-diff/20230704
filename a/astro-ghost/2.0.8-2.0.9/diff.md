# Comparing `tmp/astro_ghost-2.0.8.tar.gz` & `tmp/astro_ghost-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-2.0.8.tar", last modified: Sun Jun 18 20:32:44 2023, max compression
+gzip compressed data, was "astro_ghost-2.0.9.tar", last modified: Mon Jul  3 22:27:54 2023, max compression
```

## Comparing `astro_ghost-2.0.8.tar` & `astro_ghost-2.0.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.823954 astro_ghost-2.0.8/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.748112 astro_ghost-2.0.8/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.753527 astro_ghost-2.0.8/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      601 2023-06-17 21:52:31.000000 astro_ghost-2.0.8/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-18 20:32:44.824143 astro_ghost-2.0.8/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.8/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.806973 astro_ghost-2.0.8/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    23495 2023-06-18 19:28:46.000000 astro_ghost-2.0.8/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.8/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    38694 2023-06-06 15:46:00.000000 astro_ghost-2.0.8/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.8/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.8/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.8/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.8/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-06-18 20:32:27.000000 astro_ghost-2.0.8/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.8/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    42652 2023-06-18 20:31:32.000000 astro_ghost-2.0.8/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.8/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.8/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    17703 2023-06-18 19:28:46.000000 astro_ghost-2.0.8/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-06-06 16:38:06.000000 astro_ghost-2.0.8/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.8/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.8/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.8/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.809674 astro_ghost-2.0.8/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-18 20:32:44.000000 astro_ghost-2.0.8/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-06-18 20:32:44.000000 astro_ghost-2.0.8/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-18 20:32:44.000000 astro_ghost-2.0.8/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-18 20:32:44.000000 astro_ghost-2.0.8/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-06-18 20:32:44.000000 astro_ghost-2.0.8/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-06-18 20:32:44.000000 astro_ghost-2.0.8/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.812856 astro_ghost-2.0.8/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.8/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.8/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.819597 astro_ghost-2.0.8/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.8/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.8/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.8/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.8/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.8/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.8/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.8/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.8/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.821409 astro_ghost-2.0.8/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-06-18 20:32:44.824883 astro_ghost-2.0.8/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-06-18 20:32:18.000000 astro_ghost-2.0.8/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.823607 astro_ghost-2.0.8/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.8/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.8/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.8/tests/pytest.ini
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4492 2023-06-18 19:28:46.000000 astro_ghost-2.0.8/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.8/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-07-03 22:27:54.057581 astro_ghost-2.0.9/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-07-03 22:27:53.976185 astro_ghost-2.0.9/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-07-03 22:27:53.982288 astro_ghost-2.0.9/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.9/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      601 2023-06-17 21:52:31.000000 astro_ghost-2.0.9/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.9/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.9/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.9/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-07-03 22:27:54.057923 astro_ghost-2.0.9/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.9/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-07-03 22:27:54.028395 astro_ghost-2.0.9/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    23504 2023-07-03 22:24:42.000000 astro_ghost-2.0.9/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-06-18 20:57:46.000000 astro_ghost-2.0.9/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    38694 2023-06-06 15:46:00.000000 astro_ghost-2.0.9/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.9/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.9/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.9/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.9/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-07-03 22:26:23.000000 astro_ghost-2.0.9/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.9/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    43692 2023-07-03 22:24:36.000000 astro_ghost-2.0.9/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.9/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.9/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    17703 2023-06-18 19:28:46.000000 astro_ghost-2.0.9/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     9808 2023-07-03 22:17:51.000000 astro_ghost-2.0.9/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.9/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.9/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.9/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-07-03 22:27:54.032101 astro_ghost-2.0.9/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-07-03 22:27:53.000000 astro_ghost-2.0.9/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-07-03 22:27:53.000000 astro_ghost-2.0.9/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-07-03 22:27:53.000000 astro_ghost-2.0.9/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-07-03 22:27:53.000000 astro_ghost-2.0.9/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-07-03 22:27:53.000000 astro_ghost-2.0.9/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-07-03 22:27:53.000000 astro_ghost-2.0.9/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-07-03 22:27:54.035642 astro_ghost-2.0.9/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.9/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.9/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.9/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.9/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-07-03 22:27:54.049698 astro_ghost-2.0.9/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.9/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.9/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.9/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.9/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.9/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.9/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.9/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.9/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-07-03 22:27:54.052699 astro_ghost-2.0.9/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.9/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.9/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.9/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-07-03 22:27:54.059701 astro_ghost-2.0.9/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-07-03 22:26:35.000000 astro_ghost-2.0.9/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-07-03 22:27:54.056781 astro_ghost-2.0.9/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.9/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.9/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.9/tests/pytest.ini
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4492 2023-06-18 19:28:46.000000 astro_ghost-2.0.9/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.9/tox.ini
```

### Comparing `astro_ghost-2.0.8/.github/workflows/tests.yml` & `astro_ghost-2.0.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/.gitignore` & `astro_ghost-2.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/PKG-INFO` & `astro_ghost-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 2.0.8
+Version: 2.0.9
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.0.8/README.rst` & `astro_ghost-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/astro_ghost/DLR.py` & `astro_ghost-2.0.9/astro_ghost/DLR.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,15 +411,15 @@
         ra_SN = float(row['RA'])
         dec_SN = float(row['DEC'])
         class_SN = str(row['Obj. Type'])
 
         #query the glade catalog
         Vizier.ROW_LIMIT = -1
         Vizier.TIMEOUT = 500
-        result = Vizier.query_region(SkyCoord(ra=ra_SN, dec=dec_SN,unit=(u.deg, u.deg),frame='icrs'),radius=Angle(1.0, "deg"), catalog=["VII/275/glade1"])
+        result = Vizier.query_region(SkyCoord(ra=ra_SN, dec=dec_SN,unit=(u.deg, u.deg),frame='icrs'),radius=Angle(0.2, "deg"), catalog=["VII/275/glade1"])
         if result:
             hosts = result[0].to_pandas()
         else:
             hosts = pd.DataFrame({'a_b':[np.nan], 'maj':[np.nan], 'min':[np.nan]})
         
         # query NED for GLADE sources and get their radius
         GLADE_rad = hosts.dropna(subset=['a_b', 'maj', 'min'])
@@ -440,15 +440,16 @@
                 GLADE_norad.loc[GLADE_norad.index == idx, 'min'] = tempMin_arcsec*2./60
                 GLADE_norad.loc[GLADE_norad.index == idx, 'a_b'] = 1/AxisRatio  
             except:
                 badRadCount +=1
 
         #recombine
         if verbose:
-            print("No NED radius found for %i GLADE galaxies."%badRadCount)
+            print("No NED radius found for %i GLADE galaxies."%badRadCount, file=f)
+
         hosts = pd.concat([GLADE_rad, GLADE_norad], ignore_index=True)
 
         hosts.dropna(subset=['a_b', 'maj', 'min'], inplace=True)
         if len(hosts)<1:
             noGladeHosts.append(name)
             continue
         hosts['MajorRad'] = hosts['maj']*60./2 #in arcsec, to radius
```

### Comparing `astro_ghost-2.0.8/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-2.0.9/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-2.0.9/astro_ghost/PS1QueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-2.0.9/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-2.0.9/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-2.0.9/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/astro_ghost/conftest.py` & `astro_ghost-2.0.9/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-2.0.9/astro_ghost/ghostHelperFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,15 @@
         h_link.membership, cluster.id AS cluster
         FROM (SELECT oid, id FROM basic JOIN ident ON oidref = oid WHERE
         CONTAINS(POINT('ICRS',ra,dec),CIRCLE('ICRS',{0},{1},0.000556))=1 ) AS cluster, basic
         JOIN h_link ON basic.oid = h_link.parent WHERE h_link.child = cluster.oid ORDER BY dist ASC;
         """.format(row.raMean, row.decMean)
         result = tap_simbad.search(query)
         tap_pandas = result.to_table().to_pandas().reset_index(drop=True)
+        tap_pandas.dropna(subset=['membership'], inplace=True)
         if ((not tap_pandas.empty) and (tap_pandas.loc[0, 'membership'] > 50)):
             tap_pandas.drop_duplicates(subset=['main_id'], inplace=True)
             tap_pandas.reset_index(drop=True, inplace=True)
  
             if tap_pandas['main_id'].values[0].startswith("VIRTUAL PARENT"):
                 continue
 
@@ -606,15 +607,15 @@
                 GHOSTpath = GHOSTpath.split("/")[:-1]
                 GHOSTpath = "/".join(GHOSTpath)
             except:
                 print("Error! I don't know where you installed GHOST -- set GHOST_PATH as an environmental variable or pass in the GHOSTpath parameter.")
     fullTable = pd.read_csv(GHOSTpath+"/database/GHOST.csv")
     return fullTable
 
-def getTransientHosts(transientName=[''], snCoord=[''], snClass=[''], verbose=False, starcut='normal', ascentMatch=False, px=800, savepath='./', GHOSTpath='', redo_search=True):
+def getTransientHosts(transientName=[''], snCoord=[''], snClass=[''], verbose=False, starcut='normal', ascentMatch=False, GLADE=True, px=800, savepath='./', GHOSTpath='', redo_search=True):
     """The wrapper function for the main host association pipeline. The function first
        searches the pre-existing GHOST database by transient name, then by transient coordinates, and finally
        associates the remaining transients not found.
 
     :param transientName: List of transients to associate.
     :type transientName: array-like
     :param snCoord: List of astropy SkyCoord transient positions.
@@ -680,29 +681,29 @@
 
             df_transients_remaining = df_transients_remaining[df_transients_remaining['snCoord'].isin(notFoundCoords)]
 
             transientName_remaining =  df_transients_remaining['Name'].values
             snCoord_remaining = df_transients_remaining['snCoord'].values
             snClass_remaining = df_transients_remaining['snClass'].values
 
-            tempHost3 = findNewHosts(transientName_remaining, snCoord_remaining, snClass_remaining, verbose, starcut, ascentMatch, px, savepath)
+            tempHost3 = findNewHosts(transientName_remaining, snCoord_remaining, snClass_remaining, verbose, starcut, ascentMatch, px, savepath, GLADE=GLADE)
 
             if (len(transientName_remaining) > 0) and (len(tempHost3)==0) and (redo_search):
                  #bump up the search radius to 150 arcsec for extremely low-redshift hosts...
                  if verbose:
                      print("Couldn't find any hosts! Trying again with a search radius of 150''.")
                  tempHost3 = findNewHosts(transientName_remaining, snCoord_remaining, snClass_remaining, verbose, starcut, ascentMatch, px, savepath, 150)
             found_by_manual = len(tempHost3)
     hostDB = pd.concat([tempHost1, tempHost2, tempHost3], ignore_index=True)
     hostDB.replace(-999.0, np.nan, inplace=True)
     if verbose:
         print("%i transients found by name, %i transients found by coordinates, %i transients manually associated."% (found_by_name, found_by_coord, found_by_manual))
     return hostDB
 
-def findNewHosts(transientName, snCoord, snClass, verbose=False, starcut='gentle', ascentMatch=False, px=800, savepath='./', rad=60):
+def findNewHosts(transientName, snCoord, snClass, verbose=False, starcut='gentle', ascentMatch=False, px=800, savepath='./', rad=60, GLADE=True):
     """Associates hosts of transients not in the GHOST database.
 
     :param transientName: List of transients to associate.
     :type transientName: array-like
     :param snCoord: List of astropy SkyCoord transient positions.
     :type snCoord: array-like
     :param snClass: List of transient classifications (if they exist).
@@ -754,27 +755,33 @@
     path = savepath+dir_name+'/'
 
     #create temp dataframe with RA and DEC corresponding to the transient
     snDF = pd.DataFrame({'Name':transientName_arr, 'RA':snRA_arr, 'DEC':snDEC_arr, 'HostName':['']*len(snDEC_arr), 'Obj. Type':snClass_arr})
     snDF.to_csv(path+fn_transients, index=False)
 
     #new low-z method (beta) - before we do anything else, find and associate with GLADE
-    fn_glade = "gladeDLR.txt"
-    foundGladeHosts, noGladeHosts = chooseByGladeDLR(path, fn_glade, snDF, verbose=verbose, todo="r")
-
-    #open transients df and drop the transients already found in GLADE. We'll add these back in at the end
-    snDF = snDF[snDF['Name'].isin(noGladeHosts)]
-    fn_transients_preGLADE = fn_transients
-    fn_transients = 'transients_%s_postGlade.csv' % dateStr
-    snDF.to_csv(path+fn_transients, index=False)
+    if GLADE: 
+        fn_glade = "gladeDLR.txt"
+        foundGladeHosts, noGladeHosts = chooseByGladeDLR(path, fn_glade, snDF, verbose=verbose, todo="r")
+
+        #open transients df and drop the transients already found in GLADE. We'll add these back in at the end
+        snDF = snDF[snDF['Name'].isin(noGladeHosts)]
+        fn_transients_preGLADE = fn_transients
+        fn_transients = 'transients_%s_postGlade.csv' % dateStr
+        snDF.to_csv(path+fn_transients, index=False)
+
+    else: 
+        foundGladeHosts = []
+        noGladeHosts = snDF['Name'].values
+        fn_transients_preGLADE = fn_transients
 
     if len(noGladeHosts) < 1:
         #just return the GLADE df!
         foundGladeHosts['GLADE_source'] = True
-        host_DF = foundGladeHosts
+        host_DF = foundGladeHosts 
     else:
         #begin doing the heavy lifting after GLADE to associate transients with hosts
         host_DF = get_hosts(path, fn_transients, fn_host, rad)
 
         if len(host_DF) < 1:
             print("ERROR: Found no hosts in cone search during manual association!")
             return None
@@ -916,26 +923,42 @@
         if len(foundGladeHosts) > 0:
             if verbose:
                 print("Adding %i sources from GLADE back into the catalog..."%len(foundGladeHosts))
 
             host_DF['GLADE_source'] = False
             foundGladeHosts['GLADE_source'] = True
 
-            #kluge for lookup later
-            foundGladeHosts['objID'] = foundGladeHosts['objName'] = foundGladeHosts['NED_name']
+            #get PS1 photometry for GLADE sources by crossmatching
+            ps1matches = []
+            for idx, row in foundGladeHosts.iterrows():
+                a = ps1cone(row.raMean, row.decMean, 10./3600)
+                if a:
+                    a = ascii.read(a)
+                    a = a.to_pandas()
+                    ps1match = a.iloc[[0]] 
+                    #get rid of coord info - GLADE properties are better!
+                    ps1match.drop(['raMean', 'decMean'], axis=1, inplace=True)
+                    foundGladeHosts.loc[foundGladeHosts.index == idx, 'objID'] = ps1match['objID'].values[0]
+                    ps1matches.append(ps1match)
+            ps1matches = pd.concat(ps1matches)
+            foundGladeHosts = foundGladeHosts.merge(ps1matches, on=['objID'])
+
 
             #combine
             host_DF = pd.concat([host_DF, foundGladeHosts], ignore_index=True)
 
         with open(path+"/dictionaries/" + "Final_Dictionary.p", 'wb') as fp:
                dump(final_dict, fp)
 
     host_DF = checkSimbadHierarchy(host_DF, verbose=verbose)
 
     #a few final cleaning steps
+    #first, add back in some features 
+    host_DF = getColors(host_DF)
+    host_DF = calc_7DCD(host_DF)
     host_DF.drop_duplicates(subset=['TransientName'], inplace=True)
     host_DF = host_DF[host_DF['TransientName'] != ""]
     host_DF.reset_index(inplace=True, drop=True)
     host_DF['TransientName'] = [x.replace(" ", "") for x in host_DF['TransientName']]
 
     allTransients = pd.read_csv(path+fn_transients_preGLADE)
```

### Comparing `astro_ghost-2.0.8/astro_ghost/gradientAscent.py` & `astro_ghost-2.0.9/astro_ghost/gradientAscent.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/astro_ghost/hostMatching.py` & `astro_ghost-2.0.9/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/astro_ghost/photoz_helper.py` & `astro_ghost-2.0.9/astro_ghost/photoz_helper.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/astro_ghost/sourceCleaning.py` & `astro_ghost-2.0.9/astro_ghost/sourceCleaning.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,14 @@
     df.replace(-999, np.nan, inplace=True)
     df.replace(999, np.nan, inplace=True)
 
     # create color attributes for all hosts
     df["g-r"]= df["gApMag"] - df["rApMag"]
     df["r-i"]= df["rApMag"] - df["iApMag"]
     df["i-z"] = df["iApMag"] - df["zApMag"]
-#    df["g-i"] = df["gApMag"] - df["iApMag"]
     df["z-y"] = df["zApMag"] - df["yApMag"]
 
     df['g-rErr'] = np.sqrt(df['gApMagErr']**2 + df['rApMagErr']**2)
     df['r-iErr'] = np.sqrt(df['rApMagErr']**2 + df['iApMagErr']**2)
     df['i-zErr'] = np.sqrt(df['iApMagErr']**2 + df['zApMagErr']**2)
     df['z-yErr'] = np.sqrt(df['zApMagErr']**2 + df['yApMagErr']**2)
```

### Comparing `astro_ghost-2.0.8/astro_ghost/starSeparation.py` & `astro_ghost-2.0.9/astro_ghost/starSeparation.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/astro_ghost/stellarLocus.py` & `astro_ghost-2.0.9/astro_ghost/stellarLocus.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-2.0.9/astro_ghost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-ghost
-Version: 2.0.8
+Version: 2.0.9
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.0.8/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-2.0.9/astro_ghost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/docs/Makefile` & `astro_ghost-2.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/docs/conf.py` & `astro_ghost-2.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/docs/index.rst` & `astro_ghost-2.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/docs/make.bat` & `astro_ghost-2.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/docs/source/associationmodules.rst` & `astro_ghost-2.0.9/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/docs/source/basicusage.rst` & `astro_ghost-2.0.9/docs/source/basicusage.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/docs/source/catalogmodules.rst` & `astro_ghost-2.0.9/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/docs/source/installation.rst` & `astro_ghost-2.0.9/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/docs/source/preprocessingmodules.rst` & `astro_ghost-2.0.9/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/licenses/LICENSE.rst` & `astro_ghost-2.0.9/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/setup.cfg` & `astro_ghost-2.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/setup.py` & `astro_ghost-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "2.0.8"
+version = "2.0.9"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-2.0.8/tests/debug.py` & `astro_ghost-2.0.9/tests/debug.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/tests/test_tutorial.py` & `astro_ghost-2.0.9/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.8/tox.ini` & `astro_ghost-2.0.9/tox.ini`

 * *Files identical despite different names*

