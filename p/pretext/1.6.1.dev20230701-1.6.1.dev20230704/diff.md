# Comparing `tmp/pretext-1.6.1.dev20230701.tar.gz` & `tmp/pretext-1.6.1.dev20230704.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230701.tar", max compression
+gzip compressed data, was "pretext-1.6.1.dev20230704.tar", max compression
```

## Comparing `pretext-1.6.1.dev20230701.tar` & `pretext-1.6.1.dev20230704.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-07-01 06:13:37.836882 pretext-1.6.1.dev20230701/LICENSE
--rw-r--r--   0        0        0     9757 2023-07-01 06:13:37.836882 pretext-1.6.1.dev20230701/README.md
--rw-r--r--   0        0        0     1962 2023-07-01 06:14:18.353105 pretext-1.6.1.dev20230701/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-07-01 06:13:37.840882 pretext-1.6.1.dev20230701/pretext/__main__.py
--rw-r--r--   0        0        0     8531 2023-07-01 06:13:37.840882 pretext-1.6.1.dev20230701/pretext/build.py
--rw-r--r--   0        0        0    25736 2023-07-01 06:13:37.840882 pretext-1.6.1.dev20230701/pretext/cli.py
--rw-r--r--   0        0        0     5856 2023-07-01 06:13:37.840882 pretext-1.6.1.dev20230701/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-07-01 06:13:37.840882 pretext-1.6.1.dev20230701/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-07-01 06:13:37.840882 pretext-1.6.1.dev20230701/pretext/core/__init__.py
--rw-r--r--   0        0        0   172492 2023-07-01 06:14:23.877102 pretext-1.6.1.dev20230701/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-07-01 06:13:37.840882 pretext-1.6.1.dev20230701/pretext/core/resources.py
--rw-r--r--   0        0        0  1042093 2023-07-01 06:14:23.877102 pretext-1.6.1.dev20230701/pretext/core/resources.zip
--rw-r--r--   0        0        0    16741 2023-07-01 06:13:37.840882 pretext-1.6.1.dev20230701/pretext/generate.py
--rw-r--r--   0        0        0    29108 2023-07-01 06:13:37.840882 pretext-1.6.1.dev20230701/pretext/project.py
--rw-r--r--   0        0        0      739 2023-07-01 06:13:37.840882 pretext-1.6.1.dev20230701/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-07-01 06:14:23.969102 pretext-1.6.1.dev20230701/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-07-01 06:14:23.969102 pretext-1.6.1.dev20230701/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160110 2023-07-01 06:14:23.961102 pretext-1.6.1.dev20230701/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7616 2023-07-01 06:14:23.965102 pretext-1.6.1.dev20230701/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173309 2023-07-01 06:14:23.953102 pretext-1.6.1.dev20230701/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2192 2023-07-01 06:14:23.969102 pretext-1.6.1.dev20230701/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4657 2023-07-01 06:14:23.929102 pretext-1.6.1.dev20230701/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-07-01 06:14:23.969102 pretext-1.6.1.dev20230701/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-07-01 06:14:23.969102 pretext-1.6.1.dev20230701/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8392 2023-07-01 06:14:23.969102 pretext-1.6.1.dev20230701/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    25086 2023-07-01 06:13:37.840882 pretext-1.6.1.dev20230701/pretext/utils.py
--rw-r--r--   0        0        0     3333 2023-07-01 06:14:18.353105 pretext-1.6.1.dev20230701/pyproject.toml
--rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230701/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-04 06:15:06.421399 pretext-1.6.1.dev20230704/LICENSE
+-rw-r--r--   0        0        0     9757 2023-07-04 06:15:06.421399 pretext-1.6.1.dev20230704/README.md
+-rw-r--r--   0        0        0     1962 2023-07-04 06:15:41.003341 pretext-1.6.1.dev20230704/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-04 06:15:06.421399 pretext-1.6.1.dev20230704/pretext/__main__.py
+-rw-r--r--   0        0        0     8531 2023-07-04 06:15:06.421399 pretext-1.6.1.dev20230704/pretext/build.py
+-rw-r--r--   0        0        0    25736 2023-07-04 06:15:06.421399 pretext-1.6.1.dev20230704/pretext/cli.py
+-rw-r--r--   0        0        0     5856 2023-07-04 06:15:06.421399 pretext-1.6.1.dev20230704/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172498 2023-07-04 06:15:46.119619 pretext-1.6.1.dev20230704/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/core/resources.py
+-rw-r--r--   0        0        0  1044427 2023-07-04 06:15:46.119619 pretext-1.6.1.dev20230704/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16741 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/generate.py
+-rw-r--r--   0        0        0    29108 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/project.py
+-rw-r--r--   0        0        0      739 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-07-04 06:15:46.203623 pretext-1.6.1.dev20230704/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-07-04 06:15:46.203623 pretext-1.6.1.dev20230704/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160110 2023-07-04 06:15:46.195623 pretext-1.6.1.dev20230704/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7616 2023-07-04 06:15:46.199623 pretext-1.6.1.dev20230704/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173309 2023-07-04 06:15:46.183622 pretext-1.6.1.dev20230704/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2192 2023-07-04 06:15:46.203623 pretext-1.6.1.dev20230704/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4657 2023-07-04 06:15:46.167621 pretext-1.6.1.dev20230704/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-07-04 06:15:46.203623 pretext-1.6.1.dev20230704/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-07-04 06:15:46.203623 pretext-1.6.1.dev20230704/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8392 2023-07-04 06:15:46.203623 pretext-1.6.1.dev20230704/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    25086 2023-07-04 06:15:06.425400 pretext-1.6.1.dev20230704/pretext/utils.py
+-rw-r--r--   0        0        0     3333 2023-07-04 06:15:41.003341 pretext-1.6.1.dev20230704/pyproject.toml
+-rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230704/PKG-INFO
```

### Comparing `pretext-1.6.1.dev20230701/LICENSE` & `pretext-1.6.1.dev20230704/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/README.md` & `pretext-1.6.1.dev20230704/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pretext/__init__.py` & `pretext-1.6.1.dev20230704/pretext/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 from single_version import get_version
 
 log = logging.getLogger("ptxlogger")
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = '4da2a0f824785143c917c0f16007cbd0d48ba88d'
+CORE_COMMIT = 'd0c0cf9e039e95a0d1cf57dbf1a5a00c2a5e866e'
 
 # List of templates, build formats, and assets that are supported by the CLI.
 NEW_TEMPLATES = ["book", "article", "demo", "hello", "slideshow"]
 BUILD_FORMATS = [
     "html",
     "pdf",
     "latex",
```

### Comparing `pretext-1.6.1.dev20230701/pretext/build.py` & `pretext-1.6.1.dev20230704/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pretext/cli.py` & `pretext-1.6.1.dev20230704/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pretext/codechat.py` & `pretext-1.6.1.dev20230704/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pretext/config/xml_overlay.py` & `pretext-1.6.1.dev20230704/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pretext/core/pretext.py` & `pretext-1.6.1.dev20230704/pretext/core/pretext.py`

 * *Files 0% similar despite different names*

```diff
@@ -2037,15 +2037,15 @@
     numAttempt = 0
     maxAttempts = 10  # In case failure is not due to blocked ports.
     while looking_for_port and numAttempt < maxAttempts:
         try:
             numAttempt = numAttempt + 1
             log.info(f"Opening subprocess http.server with port={port}")
             # -u so that stdout and stderr are not cached
-            server = subprocess.Popen(["python", "-u", "-m", "http.server", f"{port}", "-d", tmp_dir], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+            server = subprocess.Popen([sys.executable, "-u", "-m", "http.server", f"{port}", "-d", tmp_dir], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
             # Check if terminated. Allow 1 second to start-up.
             try:
                 result = server.wait(1)
                 log.debug(f"Server startup failed")
                 port = random.randint(49152, 65535)
                 log.debug(f"Trying port {port} instead")
             # The exception is success because process did not terminate.
```

### Comparing `pretext-1.6.1.dev20230701/pretext/core/resources.py` & `pretext-1.6.1.dev20230704/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pretext/core/resources.zip` & `pretext-1.6.1.dev20230704/pretext/core/resources.zip`

 * *Files 21% similar despite different names*

#### zipinfo {}

```diff
@@ -1,144 +1,144 @@
-Zip file size: 1042093 bytes, number of entries: 142
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 xsl/utilities/
--rw-r--r--  2.0 unx     8125 b- defN 23-Jul-01 06:14 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jul-01 06:14 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jul-01 06:14 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jul-01 06:14 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jul-01 06:14 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jul-01 06:14 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jul-01 06:14 xsl/README.md
--rw-r--r--  2.0 unx     2725 b- defN 23-Jul-01 06:14 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jul-01 06:14 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-Jul-01 06:14 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jul-01 06:14 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jul-01 06:14 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jul-01 06:14 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jul-01 06:14 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx   548426 b- defN 23-Jul-01 06:14 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jul-01 06:14 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jul-01 06:14 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jul-01 06:14 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jul-01 06:14 xsl/entities.ent
--rw-r--r--  2.0 unx     6281 b- defN 23-Jul-01 06:14 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jul-01 06:14 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jul-01 06:14 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    89128 b- defN 23-Jul-01 06:14 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jul-01 06:14 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jul-01 06:14 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx   612195 b- defN 23-Jul-01 06:14 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jul-01 06:14 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jul-01 06:14 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jul-01 06:14 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx   231265 b- defN 23-Jul-01 06:14 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jul-01 06:14 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jul-01 06:14 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx   112450 b- defN 23-Jul-01 06:14 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jul-01 06:14 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jul-01 06:14 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx   110044 b- defN 23-Jul-01 06:14 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jul-01 06:14 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jul-01 06:14 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx   544229 b- defN 23-Jul-01 06:14 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Jul-01 06:14 xsl/utilities/README.md
--rw-r--r--  2.0 unx     4926 b- defN 23-Jul-01 06:14 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx     4299 b- defN 23-Jul-01 06:14 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-Jul-01 06:14 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-Jul-01 06:14 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx      513 b- defN 23-Jul-01 06:14 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4760 b- defN 23-Jul-01 06:14 xsl/localizations/README.md
--rw-r--r--  2.0 unx    15866 b- defN 23-Jul-01 06:14 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx     2286 b- defN 23-Jul-01 06:14 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    16837 b- defN 23-Jul-01 06:14 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16534 b- defN 23-Jul-01 06:14 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    19185 b- defN 23-Jul-01 06:14 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16085 b- defN 23-Jul-01 06:14 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16349 b- defN 23-Jul-01 06:14 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16312 b- defN 23-Jul-01 06:14 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    17056 b- defN 23-Jul-01 06:14 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16252 b- defN 23-Jul-01 06:14 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    20481 b- defN 23-Jul-01 06:14 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    17081 b- defN 23-Jul-01 06:14 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    15582 b- defN 23-Jul-01 06:14 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17231 b- defN 23-Jul-01 06:14 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    19326 b- defN 23-Jul-01 06:14 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    16500 b- defN 23-Jul-01 06:14 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17301 b- defN 23-Jul-01 06:14 xsl/localizations/fi-FI.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 23-Jul-01 06:14 xsl/support/README.md
--rw-r--r--  2.0 unx     5065 b- defN 23-Jul-01 06:14 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     5800 b- defN 23-Jul-01 06:14 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jul-01 06:14 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx    10306 b- defN 23-Jul-01 06:14 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jul-01 06:14 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-Jul-01 06:14 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     2657 b- defN 23-Jul-01 06:14 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-Jul-01 06:14 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx      722 b- defN 23-Jul-01 06:14 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx    14482 b- defN 23-Jul-01 06:14 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jul-01 06:14 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jul-01 06:14 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jul-01 06:14 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jul-01 06:14 xsl/latex/pretext-latex-guide.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jul-01 06:14 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jul-01 06:14 script/mbx
--rw-r--r--  2.0 unx      481 b- defN 23-Jul-01 06:14 script/mjsre/README.md
--rw-r--r--  2.0 unx      116 b- defN 23-Jul-01 06:14 script/mjsre/package.json
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-01 06:14 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-Jul-01 06:14 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx     1180 b- defN 23-Jul-01 06:14 schema/README.md
--rw-r--r--  2.0 unx   101829 b- defN 23-Jul-01 06:14 schema/pretext.rng
--rw-r--r--  2.0 unx    34210 b- defN 23-Jul-01 06:14 schema/pretext-dev.rng
--rw-r--r--  2.0 unx      326 b- defN 23-Jul-01 06:14 schema/xml.xsd
--rw-r--r--  2.0 unx    25870 b- defN 23-Jul-01 06:14 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    17587 b- defN 23-Jul-01 06:14 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx   134043 b- defN 23-Jul-01 06:14 schema/pretext.xml
--rw-r--r--  2.0 unx     3135 b- defN 23-Jul-01 06:14 schema/build.sh
--rw-r--r--  2.0 unx    58086 b- defN 23-Jul-01 06:14 schema/pretext.rnc
--rw-r--r--  2.0 unx    18421 b- defN 23-Jul-01 06:14 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx   125135 b- defN 23-Jul-01 06:14 schema/pretext.xsd
--rw-r--r--  2.0 unx     1367 b- defN 23-Jul-01 06:14 pretext/README.md
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-01 06:14 pretext/__init__.py
--rw-r--r--  2.0 unx     1955 b- defN 23-Jul-01 06:14 pretext/module-test.py
--rw-r--r--  2.0 unx    30908 b- defN 23-Jul-01 06:14 pretext/pretext
--rw-r--r--  2.0 unx    35449 b- defN 23-Jul-01 06:14 pretext/braille_format.py
--rw-r--r--  2.0 unx   172492 b- defN 23-Jul-01 06:14 pretext/pretext.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jul-01 06:14 pretext/pretext.cfg
--rw-r--r--  2.0 unx     2608 b- defN 23-Jul-01 06:14 css/colors_default.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jul-01 06:14 css/pretext_add_on.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jul-01 06:14 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jul-01 06:14 css/kindle.css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jul-01 06:14 css/README.md
--rw-r--r--  2.0 unx     1362 b- defN 23-Jul-01 06:14 css/epub.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jul-01 06:14 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jul-01 06:14 css/pretext.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jul-01 06:14 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-01 06:14 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-01 06:14 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-01 06:14 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jul-01 06:14 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-01 06:14 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jul-01 06:14 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jul-01 06:14 css/style_soundwriting.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-01 06:14 css/colors_orange_navy.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jul-01 06:14 css/mathbook-3.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-01 06:14 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jul-01 06:14 css/setcolors.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jul-01 06:14 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-01 06:14 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-01 06:14 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jul-01 06:14 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jul-01 06:14 css/update_css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jul-01 06:14 css/style_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-01 06:14 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jul-01 06:14 css/colors_red_blue.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Jul-01 06:14 css/colors_maroon_grey.css
-142 files, 4837859 bytes uncompressed, 1024519 bytes compressed:  78.8%
+Zip file size: 1044427 bytes, number of entries: 142
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/utilities/
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jul-04 06:15 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jul-04 06:15 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jul-04 06:15 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jul-04 06:15 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jul-04 06:15 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jul-04 06:15 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jul-04 06:15 xsl/README.md
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jul-04 06:15 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jul-04 06:15 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jul-04 06:15 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jul-04 06:15 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jul-04 06:15 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jul-04 06:15 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jul-04 06:15 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx   548615 b- defN 23-Jul-04 06:15 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jul-04 06:15 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jul-04 06:15 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jul-04 06:15 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jul-04 06:15 xsl/entities.ent
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jul-04 06:15 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jul-04 06:15 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jul-04 06:15 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    94587 b- defN 23-Jul-04 06:15 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jul-04 06:15 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jul-04 06:15 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx   611681 b- defN 23-Jul-04 06:15 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jul-04 06:15 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jul-04 06:15 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jul-04 06:15 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx   231265 b- defN 23-Jul-04 06:15 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jul-04 06:15 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jul-04 06:15 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx   112450 b- defN 23-Jul-04 06:15 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jul-04 06:15 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jul-04 06:15 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx   113634 b- defN 23-Jul-04 06:15 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jul-04 06:15 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jul-04 06:15 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx   544229 b- defN 23-Jul-04 06:15 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jul-04 06:15 xsl/utilities/README.md
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jul-04 06:15 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jul-04 06:15 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jul-04 06:15 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-Jul-04 06:15 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx      513 b- defN 23-Jul-04 06:15 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4760 b- defN 23-Jul-04 06:15 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    15866 b- defN 23-Jul-04 06:15 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx     2286 b- defN 23-Jul-04 06:15 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    16837 b- defN 23-Jul-04 06:15 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16534 b- defN 23-Jul-04 06:15 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    19185 b- defN 23-Jul-04 06:15 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16085 b- defN 23-Jul-04 06:15 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    16349 b- defN 23-Jul-04 06:15 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16312 b- defN 23-Jul-04 06:15 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    17056 b- defN 23-Jul-04 06:15 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16252 b- defN 23-Jul-04 06:15 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    20481 b- defN 23-Jul-04 06:15 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    17081 b- defN 23-Jul-04 06:15 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    15582 b- defN 23-Jul-04 06:15 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17231 b- defN 23-Jul-04 06:15 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    19326 b- defN 23-Jul-04 06:15 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    16500 b- defN 23-Jul-04 06:15 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17301 b- defN 23-Jul-04 06:15 xsl/localizations/fi-FI.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 23-Jul-04 06:15 xsl/support/README.md
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jul-04 06:15 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jul-04 06:15 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Jul-04 06:15 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jul-04 06:15 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jul-04 06:15 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jul-04 06:15 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jul-04 06:15 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jul-04 06:15 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx      722 b- defN 23-Jul-04 06:15 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jul-04 06:15 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jul-04 06:15 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jul-04 06:15 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jul-04 06:15 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jul-04 06:15 xsl/latex/pretext-latex-guide.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Jul-04 06:15 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jul-04 06:15 script/mbx
+-rw-r--r--  2.0 unx      481 b- defN 23-Jul-04 06:15 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 23-Jul-04 06:15 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 06:15 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jul-04 06:15 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jul-04 06:15 schema/README.md
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jul-04 06:15 schema/pretext.rng
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jul-04 06:15 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx      326 b- defN 23-Jul-04 06:15 schema/xml.xsd
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jul-04 06:15 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jul-04 06:15 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jul-04 06:15 schema/pretext.xml
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jul-04 06:15 schema/build.sh
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jul-04 06:15 schema/pretext.rnc
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jul-04 06:15 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jul-04 06:15 schema/pretext.xsd
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jul-04 06:15 pretext/README.md
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 06:15 pretext/__init__.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jul-04 06:15 pretext/module-test.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jul-04 06:15 pretext/pretext
+-rw-r--r--  2.0 unx    36045 b- defN 23-Jul-04 06:15 pretext/braille_format.py
+-rw-r--r--  2.0 unx   172498 b- defN 23-Jul-04 06:15 pretext/pretext.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jul-04 06:15 pretext/pretext.cfg
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jul-04 06:15 css/colors_default.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jul-04 06:15 css/pretext_add_on.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Jul-04 06:15 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jul-04 06:15 css/kindle.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jul-04 06:15 css/README.md
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jul-04 06:15 css/epub.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jul-04 06:15 css/mathbook-content.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jul-04 06:15 css/pretext.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jul-04 06:15 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jul-04 06:15 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jul-04 06:15 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jul-04 06:15 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jul-04 06:15 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jul-04 06:15 css/mathbook-3.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jul-04 06:15 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jul-04 06:15 css/setcolors.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jul-04 06:15 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jul-04 06:15 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jul-04 06:15 css/update_css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jul-04 06:15 css/style_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-04 06:15 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jul-04 06:15 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jul-04 06:15 css/colors_maroon_grey.css
+142 files, 4847185 bytes uncompressed, 1026853 bytes compressed:  78.8%
```

#### xsl/pretext-common.xsl

##### xsl/pretext-common.xsl

```diff
@@ -1655,14 +1655,17 @@
   </xsl:template>
   <!-- Code Lines -->
   <!-- A "cline" is used to (optionally) structure hunks     -->
   <!-- of verbatim text.  Due to its simplicity, it should   -->
   <!-- be universal and the only efffect is to add a newline -->
   <!-- character, which the output format should recognize   -->
   <!-- via its own devices.                                  -->
+  <!-- NB: the newline provide by the last "cline" of a      -->
+  <!-- structure is used by some recursive text utilities as -->
+  <!-- a signal, such as the "braille-source-code" template. -->
   <xsl:template match="cline">
     <xsl:value-of select="."/>
     <xsl:text/>
   </xsl:template>
   <!-- ############## -->
   <!-- Lists of Names -->
   <!-- ############## -->
```

#### xsl/pretext-braille-preprint.xsl

##### xsl/pretext-braille-preprint.xsl

```diff
@@ -226,57 +226,48 @@
     </xsl:copy>
   </xsl:template>
   <!-- with /, so a plain generator can match others -->
   <xsl:template match="/pretext">
     <!-- Need an overall container   -->
     <!-- Maybe copy a language code? -->
     <brf>
-      <segment indentation="4" lines-after="1">Temporary Transcriber Notes</segment>
-      <!-- TODO: engineer bullet points (numbered list would vary?),    -->
-      <!-- formatted as individual notes helps delimit one from another -->
+      <!-- centered heading on line 1 -->
+      <segment centered="yes" lines-after="1">Transcriber Notes</segment>
+      <!-- Literal text for each note, control whitespace,  -->
+      <!-- etc here, since it will not be handled otherwise -->
       <xsl:if test="//c">
         <!-- See "c" template for explanation -->
-        <xsl:apply-templates select="." mode="transcriber-note">
-          <xsl:with-param name="message">
-            <xsl:text>Literal, or verbatim, computer code used in sentences is indicated by a set of transcriber-defined emphasis given by the following indicators, which all begin with the two cells dot-4 and dot-3456.  Single letter: 4-3456-23.  Begin, end word: 4-3456-2, 4-3456-3.  Begin, end phrase: 4-3456-2356, 4-3456-3.</xsl:text>
-          </xsl:with-param>
-        </xsl:apply-templates>
+        <segment indentation="2">
+          <xsl:text>Literal, or verbatim, computer code used in sentences is indicated by a set of transcriber-defined emphasis given by the following indicators, which all begin with the two cells dot-4 and dot-3456.  Single letter: 4-3456-23.  Begin, end word: 4-3456-2, 4-3456-3.  Begin, end phrase: 4-3456-2356, 4-3456-3.</xsl:text>
+        </segment>
       </xsl:if>
       <!--  -->
       <xsl:if test="//image">
-        <xsl:apply-templates select="." mode="transcriber-note">
-          <xsl:with-param name="message">
-            <xsl:text>Images are replaced by authors' descriptions, and then in an embossed version, a full (numbered) page comes next, which can be manually replaced by a tactile version of the image.</xsl:text>
-          </xsl:with-param>
-        </xsl:apply-templates>
+        <segment indentation="2">
+          <xsl:text>Images are replaced by authors' descriptions, and then in an embossed version, a full (numbered) page comes next, which can be manually replaced by a tactile version of the image.</xsl:text>
+        </segment>
       </xsl:if>
       <!--  -->
       <xsl:if test="//sidebyside">
-        <xsl:apply-templates select="." mode="transcriber-note">
-          <xsl:with-param name="message">
-            <xsl:text>A &quot;side-by-side&quot; is a horizontal layout of document elements.  The components of a side-by-side are called &quot;panels&quot;.  Typically panels are images or figures, but can also be items like program listings, tables, or paragraphs.  For braille, we let each panel use the full width of the page, so we announce the start, indicating the total number of panels.  Then we preface each panel with its number in the sequence.  Finally we announce the end because it may be hard to distinguish a final panel from the ensuing text.</xsl:text>
-          </xsl:with-param>
-        </xsl:apply-templates>
+        <segment indentation="2">
+          <xsl:text>A &quot;side-by-side&quot; is a horizontal layout of document elements.  The components of a side-by-side are called &quot;panels&quot;.  Typically panels are images or figures, but can also be items like program listings, tables, or paragraphs.  For braille, we let each panel use the full width of the page, so we announce the start, indicating the total number of panels.  Then we preface each panel with its number in the sequence.  Finally we announce the end because it may be hard to distinguish a final panel from the ensuing text.</xsl:text>
+        </segment>
       </xsl:if>
       <!--  -->
       <!-- automatically infers we have a note already for "sidebyside" -->
       <xsl:if test="//sbsgroup">
-        <xsl:apply-templates select="." mode="transcriber-note">
-          <xsl:with-param name="message">
-            <xsl:text>A &quot;side-by-side group&quot; is a sequence down the page of &quot;side-by-side&quot; (see previous note).  We announce the start with the number of side-by-side in the group to expect, and let the beginning and ending notes for each side-by-side delineate the sequence.</xsl:text>
-          </xsl:with-param>
-        </xsl:apply-templates>
+        <segment indentation="2">
+          <xsl:text>A &quot;side-by-side group&quot; is a sequence down the page of &quot;side-by-side&quot; (see previous note).  We announce the start with the number of side-by-side in the group to expect, and let the beginning and ending notes for each side-by-side delineate the sequence.</xsl:text>
+        </segment>
       </xsl:if>
       <!-- mention how "tabular" are implenented and suggest possible improvements-->
       <xsl:if test="//tabular">
-        <xsl:apply-templates select="." mode="transcriber-note">
-          <xsl:with-param name="message">
-            <xsl:text>Tabular material is always implemented using a &quot;linear table format&quot;.  A human transcriber may be able to improve small tables, or larger tables that could use multiple pages when embossed, by using a different format.</xsl:text>
-          </xsl:with-param>
-        </xsl:apply-templates>
+        <segment indentation="2">
+          <xsl:text>Tabular material is always implemented using a &quot;linear table format&quot;.  A human transcriber may be able to improve small tables, or larger tables that could use multiple pages when embossed, by using a different format.</xsl:text>
+        </segment>
       </xsl:if>
       <!-- process segments and blocks of "brf" -->
       <xsl:apply-templates select="*"/>
     </brf>
   </xsl:template>
   <!-- ######### -->
   <!-- Divisions -->
@@ -1549,19 +1540,186 @@
   <!-- Drop a mark at sight, Need to devise an        -->
   <!-- add-on to division-processing to make endnotes -->
   <!-- [BANA-2016] 16.1.4(g): (print observations)  -->
   <!-- In a note section, either at the end of each -->
   <!-- chapter or at the back of the book.          -->
   <!-- [BANA-2016] 16.1.5(c): (braille placement)   -->
   <!-- At the end of the chapter or volume.         -->
-  <!-- See BANA 16.2.2 for superscripted number (two-cell indicator, number sign, number). -->
+  <!-- BANA 16.2.2: superscripted number          -->
+  <!-- (two-cell indicator, number sign, number). -->
+  <!-- TODO: collect footnote *content* at division ends -->
   <xsl:template match="fn">
-    <xsl:text>[</xsl:text>
+    <!--  5-6  3-5  -->
+    <xsl:text>⠰⠔</xsl:text>
+    <!-- A number sign is supplied by liblouis translation -->
+    <!-- 2-4-5-6  U+283C                                   -->
     <xsl:apply-templates select="." mode="number"/>
-    <xsl:text>]</xsl:text>
+    <!-- trailing space necessary to end superscript?  -->
+    <!-- will get merged with any that already exists? -->
+    <xsl:text/>
+  </xsl:template>
+  <!-- ################# -->
+  <!-- Verbatim, Program -->
+  <!-- ################# -->
+  <!-- Various templates elsewhere manipulate large chunks of verbatim text, -->
+  <!-- such as for a "program".  We leverage those as much as possible.      -->
+  <!-- Ideally we easily get a chunk of text, given as a sequence of lines   -->
+  <!-- defined by newline characters.   The recursive "braille-source-code"  -->
+  <!-- template makes a "segment" for each line, this will allow for runover -->
+  <!-- and *code* indentation without any ambiguity.  So most of the braille -->
+  <!-- formatting happens in this template.                                  -->
+  <!--                                                                       -->
+  <!-- IMPORTANT: ensure that $text has a final newline character.           -->
+  <xsl:template name="braille-source-code">
+    <xsl:param name="text"/>
+    <xsl:choose>
+      <!-- $text always ends in a newline, so final recursive call will    -->
+      <!-- have an empty string.  This is the indication that we are done. -->
+      <xsl:when test="$text = ''"/>
+      <!-- Nonempty $text, so split it, and recurse -->
+      <xsl:otherwise>
+        <segment indentation="0" runover="0">
+          <code>
+            <xsl:value-of select="substring-before($text, '
+')"/>
+          </code>
+        </segment>
+        <xsl:call-template name="braille-source-code">
+          <xsl:with-param name="text" select="substring-after($text, '
+')"/>
+        </xsl:call-template>
+      </xsl:otherwise>
+    </xsl:choose>
+  </xsl:template>
+  <!-- A "cd" is structured with "cline" or not.  We do not sanitize, that   -->
+  <!-- tis what the "cline"element is for - control over leading whitespace. -->
+  <!-- We provide a final newline here for a bare "cd", otherwise the        -->
+  <!-- "cline" template provides it.                                         -->
+  <xsl:template match="cd">
+    <block breakable="no">
+      <xsl:call-template name="braille-source-code">
+        <xsl:with-param name="text">
+          <xsl:choose>
+            <xsl:when test="cline">
+              <xsl:apply-templates select="cline"/>
+            </xsl:when>
+            <xsl:otherwise>
+              <xsl:value-of select="."/>
+              <xsl:text/>
+            </xsl:otherwise>
+          </xsl:choose>
+        </xsl:with-param>
+      </xsl:call-template>
+    </block>
+  </xsl:template>
+  <!-- "pre" and "pre[cline]" are handled by the "interior" -->
+  <!-- modal template in -common.                           -->
+  <!-- "pre" uses "sanitize-text", which provides a final   -->
+  <!-- newline, while "pre[cline]" uses the base "cline"    -->
+  <!-- template, which also provides a final newline.       -->
+  <xsl:template match="pre">
+    <block breakable="no">
+      <xsl:call-template name="braille-source-code">
+        <xsl:with-param name="text">
+          <xsl:apply-templates select="." mode="interior"/>
+        </xsl:with-param>
+      </xsl:call-template>
+    </block>
+  </xsl:template>
+  <!-- A "program" gets a lot of treatment in other formats to recognize   -->
+  <!-- the language an author specifies and then do some sort of syntax    -->
+  <!-- highlighting with fonts and colors.  That would be hard in braille, -->
+  <!-- and we don't know of a good tool anyway.  So we just echo the       -->
+  <!-- "input" portion.                                                    -->
+  <!-- "sanitize-text" provides a final newline, always                    -->
+  <xsl:template match="program">
+    <block breakable="no">
+      <xsl:call-template name="braille-source-code">
+        <xsl:with-param name="text">
+          <xsl:call-template name="sanitize-text">
+            <xsl:with-param name="text" select="input"/>
+          </xsl:call-template>
+        </xsl:with-param>
+      </xsl:call-template>
+    </block>
+  </xsl:template>
+  <!-- For a "console" session, we work hardest on the "input", pulling in -->
+  <!-- a preceding prompt, and considering the possibility of no "output". -->
+  <!-- For "output", if extant, we provide necessary separators.           -->
+  <xsl:template match="console">
+    <!-- entire session as a block -->
+    <block breakable="no" lines-before="1" lines-after="1">
+      <!-- respect authored order, so don't split these -->
+      <xsl:apply-templates select="input|output"/>
+    </block>
+  </xsl:template>
+  <xsl:template match="console/input">
+    <xsl:variable name="console-input">
+      <!-- prompt first, if provided; author provides -->
+      <!-- any space that prompt would create         -->
+      <xsl:value-of select="preceding-sibling::*[1][self::prompt]"/>
+      <!-- remainder of the input -->
+      <xsl:call-template name="sanitize-text">
+        <xsl:with-param name="text" select="."/>
+      </xsl:call-template>
+    </xsl:variable>
+    <!-- now feed to braille-ification -->
+    <xsl:call-template name="braille-source-code">
+      <xsl:with-param name="text" select="$console-input"/>
+    </xsl:call-template>
+    <!-- add a blank line, only when not provided by the output -->
+    <xsl:if test="not(following-sibling::*[1][self::output])">
+      <segment lines-before="1"/>
+    </xsl:if>
+  </xsl:template>
+  <xsl:template match="console/output">
+    <xsl:variable name="console-output">
+      <!-- separate from the input -->
+      <!-- NB: newline here necessary for textual version -->
+      <xsl:text>---------------</xsl:text>
+      <!-- remainder of the input -->
+      <xsl:call-template name="sanitize-text">
+        <xsl:with-param name="text" select="."/>
+      </xsl:call-template>
+    </xsl:variable>
+    <!-- now feed to braille-ification -->
+    <xsl:call-template name="braille-source-code">
+      <xsl:with-param name="text" select="$console-output"/>
+    </xsl:call-template>
+    <!-- and a blank line to help with session -->
+    <segment lines-before="1"/>
+  </xsl:template>
+  <!-- Sage cells rely on per-conversion overrides of presumed   -->
+  <!-- abstract templates, to handle the numerous possibilities. -->
+  <!-- Using a long line to simulate input/output split          -->
+  <xsl:template match="sage" mode="sage-active-markup">
+    <xsl:param name="in"/>
+    <xsl:param name="out"/>
+    <block breakable="no" lines-before="1" lines-after="1">
+      <xsl:call-template name="braille-source-code">
+        <xsl:with-param name="text" select="$in"/>
+      </xsl:call-template>
+      <xsl:if test="not($out = '')">
+        <segment>
+          <xsl:text>-----------------</xsl:text>
+        </segment>
+        <xsl:call-template name="braille-source-code">
+          <xsl:with-param name="text" select="$out"/>
+        </xsl:call-template>
+      </xsl:if>
+    </block>
+  </xsl:template>
+  <!-- Display only, just input -->
+  <xsl:template name="sage-display-markup">
+    <xsl:param name="in"/>
+    <block breakable="no" lines-before="1" lines-after="1">
+      <xsl:call-template name="braille-source-code">
+        <xsl:with-param name="text" select="$in"/>
+      </xsl:call-template>
+    </block>
   </xsl:template>
   <!-- ############# -->
   <!-- Miscellaneous -->
   <!-- ############# -->
   <!-- Containers that have zero metadata (no title, etc.) -->
   <xsl:template match="statement|introduction|conclusion">
     <xsl:apply-templates select="*"/>
@@ -1727,97 +1885,54 @@
   <xsl:template match="title|subtitle|shorttitle|plaintitle|creator">
     <xsl:apply-imports/>
   </xsl:template>
   <!-- captions get killed in -common so we don't need to see them here -->
   <xsl:template match="caption">
     <xsl:apply-imports/>
   </xsl:template>
-  <!-- Larger structures, needing implementation, *along with* interior -->
-  <!-- structures.  We report AND include a textual place holder.       -->
+  <!-- We expect the simple template in -common to be active -->
+  <xsl:template match="cline">
+    <xsl:apply-imports/>
+  </xsl:template>
+  <!-- Action is in -common, this will catch all occurences? -->
   <xsl:template match="sage">
-    <xsl:text>SAGECELL</xsl:text>
+    <xsl:apply-imports/>
   </xsl:template>
+  <!-- Larger structures, needing implementation, *along with* interior -->
+  <!-- structures.  We report AND include a textual place holder.       -->
   <xsl:template match="notation-list">
     <xsl:text>NOTATIONLIST</xsl:text>
   </xsl:template>
   <xsl:template match="index-list">
     <xsl:text>INDEXLIST</xsl:text>
   </xsl:template>
-  <xsl:template match="cd">
-    <segment>CODE DISPLAY</segment>
-  </xsl:template>
-  <xsl:template match="pre">
-    <segment>PREFORMATTED TEXT</segment>
-  </xsl:template>
-  <xsl:template match="program">
-    <segment>PROGRAM</segment>
-  </xsl:template>
-  <xsl:template match="console">
-    <segment>CONSOLE</segment>
-  </xsl:template>
   <xsl:template match="poem">
     <segment>POEM</segment>
   </xsl:template>
   <!-- Next two are not structures, so as "text" -->
   <xsl:template match="quantity">
     <xsl:text>QUANTITY</xsl:text>
   </xsl:template>
   <xsl:template match="kbd">
     <xsl:text>KBD</xsl:text>
   </xsl:template>
   <xsl:template name="missing-warning">
-    <xsl:if test="//sage">
-      <xsl:call-template name="missing-implementation">
-        <xsl:with-param name="element" select="'sage'"/>
-        <xsl:with-param name="ntimes" select="count(//sage)"/>
-      </xsl:call-template>
-    </xsl:if>
-    <!--  -->
     <xsl:if test="//notation-list">
       <xsl:call-template name="missing-implementation">
         <xsl:with-param name="element" select="'notation-list'"/>
         <xsl:with-param name="ntimes" select="count(//notation-list)"/>
       </xsl:call-template>
     </xsl:if>
     <!--  -->
     <xsl:if test="//index-list">
       <xsl:call-template name="missing-implementation">
         <xsl:with-param name="element" select="'index-list'"/>
         <xsl:with-param name="ntimes" select="count(//index-list)"/>
       </xsl:call-template>
     </xsl:if>
-    <!--  -->
-    <xsl:if test="//cd">
-      <xsl:call-template name="missing-implementation">
-        <xsl:with-param name="element" select="'cd'"/>
-        <xsl:with-param name="ntimes" select="count(//cd)"/>
-      </xsl:call-template>
-    </xsl:if>
-    <!--  -->
-    <xsl:if test="//pre">
-      <xsl:call-template name="missing-implementation">
-        <xsl:with-param name="element" select="'pre'"/>
-        <xsl:with-param name="ntimes" select="count(//pre)"/>
-      </xsl:call-template>
-    </xsl:if>
-    <!--  -->
-    <xsl:if test="//program">
-      <xsl:call-template name="missing-implementation">
-        <xsl:with-param name="element" select="'program'"/>
-        <xsl:with-param name="ntimes" select="count(//program)"/>
-      </xsl:call-template>
-    </xsl:if>
-    <!--  -->
-    <xsl:if test="//console">
-      <xsl:call-template name="missing-implementation">
-        <xsl:with-param name="element" select="'console'"/>
-        <xsl:with-param name="ntimes" select="count(//console)"/>
-      </xsl:call-template>
-    </xsl:if>
-    <!--  -->
     <xsl:if test="//poem">
       <xsl:call-template name="missing-implementation">
         <xsl:with-param name="element" select="'poem'"/>
         <xsl:with-param name="ntimes" select="count(//poem)"/>
       </xsl:call-template>
     </xsl:if>
     <!--  -->
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -629,62 +629,48 @@
   <!-- at all, it gets built by mining content from other places     -->
   <xsl:template match="solutions" mode="structural-division-inner-content">
     <xsl:param name="heading-level"/>
     <xsl:apply-templates select="." mode="solutions">
       <xsl:with-param name="heading-level" select="$heading-level"/>
     </xsl:apply-templates>
   </xsl:template>
+  <!-- This is identical to the default "structural-division-inner-content" -->
+  <!-- template just below, excepting there are modifications for Runestone -->
+  <!-- to accomodate timed exams and group work.                            -->
   <xsl:template match="exercises" mode="structural-division-inner-content">
     <xsl:param name="heading-level"/>
-    <!-- this is identical to the default template -->
     <xsl:variable name="the-exercises">
       <xsl:apply-templates select="*">
         <xsl:with-param name="heading-level" select="$heading-level"/>
       </xsl:apply-templates>
-      <!-- only at "section" level. only when building for a Runestone server -->
-      <xsl:apply-templates select="." mode="runestone-progress-indicator"/>
     </xsl:variable>
     <xsl:choose>
-      <!-- some extra wrapping for timed exercises -->
-      <!-- presence of @time-limit is the signal   -->
+      <xsl:when test="@time-limit and (@group-work = 'yes')">
+        <xsl:message>PTX:ERROR:   an &quot;exercises&quot; division cannot simultaneously be a timed exam AND group work</xsl:message>
+        <xsl:apply-templates select="." mode="location-report"/>
+      </xsl:when>
+      <xsl:when test="@group-work = 'yes'">
+        <!-- the actual list of exercises -->
+        <xsl:copy-of select="$the-exercises"/>
+        <!-- group selection and submission features, if hosted on Runestone -->
+        <xsl:apply-templates select="." mode="runestone-group-work"/>
+      </xsl:when>
+      <!-- some extra wrapping for timed exercises      -->
+      <!-- so we pass the $the-exercises as a parameter -->
+      <!-- presence of @time-limit is the signal        -->
       <xsl:when test="@time-limit">
-        <!-- TODO: make this a template and move to RS-specific file -->
-        <div class="timedAssessment">
-          <ul data-component="timedAssessment" data-question_label="">
-            <!-- a Runestone id -->
-            <!-- TODO: use attribute template in RS file -->
-            <xsl:attribute name="id">
-              <xsl:apply-templates select="." mode="runestone-id"/>
-            </xsl:attribute>
-            <!-- one mandatory attribute -->
-            <xsl:attribute name="data-time">
-              <xsl:value-of select="@time-limit"/>
-            </xsl:attribute>
-            <!-- result, timer, feedback, pause are *on* by  -->
-            <!-- default if a PreTeXt attribute is "no" then -->
-            <!-- issue empty "data-no-*" Runestone attribute -->
-            <xsl:if test="@results = 'no'">
-              <xsl:attribute name="data-no-result"/>
-            </xsl:if>
-            <xsl:if test="@timer = 'no'">
-              <xsl:attribute name="data-no-timer"/>
-            </xsl:if>
-            <xsl:if test="@feedback = 'no'">
-              <xsl:attribute name="data-no-feedback"/>
-            </xsl:if>
-            <xsl:if test="@pause = 'no'">
-              <xsl:attribute name="data-no-pause"/>
-            </xsl:if>
-            <!-- the actual list of exercises -->
-            <xsl:copy-of select="$the-exercises"/>
-          </ul>
-        </div>
+        <xsl:apply-templates select="." mode="runestone-timed-exam">
+          <xsl:with-param name="the-exercises" select="$the-exercises"/>
+        </xsl:apply-templates>
       </xsl:when>
       <xsl:otherwise>
+        <!-- the actual list of exercises -->
         <xsl:copy-of select="$the-exercises"/>
+        <!-- only at "section" level. only when building for a Runestone server -->
+        <xsl:apply-templates select="." mode="runestone-progress-indicator"/>
       </xsl:otherwise>
     </xsl:choose>
   </xsl:template>
   <!-- Only &STRUCTURAL; elements will pass through here, but we -->
   <!-- can't limit the match (without explicit exclusions), this -->
   <!-- is the default.  Which is to just apply templates to      -->
   <!-- elements within the division. Optional: add RS progress.  -->
```

#### xsl/pretext-runestone.xsl

##### xsl/pretext-runestone.xsl

```diff
@@ -462,14 +462,83 @@
         of
         <span id="scprogressposs"/>
         activities on this page.
         <div id="subchapterprogress" aria-label="Page progress"/>
       </div>
     </xsl:if>
   </xsl:template>
+  <!-- A timed exam requires markup that wraps an entire collection -->
+  <!-- of exercises, so we pass the exercises in as a parameter     -->
+  <xsl:template match="exercises" mode="runestone-timed-exam">
+    <xsl:param name="the-exercises"/>
+    <!-- Since the component wraps the exercises, we do not need any  -->
+    <!-- restriction about being at teh Runestone "subchapter" level. -->
+    <xsl:if test="$b-host-runestone">
+      <div class="timedAssessment">
+        <ul data-component="timedAssessment" data-question_label="">
+          <!-- a Runestone id -->
+          <xsl:apply-templates select="." mode="runestone-id-attribute"/>
+          <!-- one mandatory attribute -->
+          <xsl:attribute name="data-time">
+            <xsl:value-of select="@time-limit"/>
+          </xsl:attribute>
+          <!-- result, timer, feedback, pause are *on* by  -->
+          <!-- default if a PreTeXt attribute is "no" then -->
+          <!-- issue empty "data-no-*" Runestone attribute -->
+          <xsl:if test="@results = 'no'">
+            <xsl:attribute name="data-no-result"/>
+          </xsl:if>
+          <xsl:if test="@timer = 'no'">
+            <xsl:attribute name="data-no-timer"/>
+          </xsl:if>
+          <xsl:if test="@feedback = 'no'">
+            <xsl:attribute name="data-no-feedback"/>
+          </xsl:if>
+          <xsl:if test="@pause = 'no'">
+            <xsl:attribute name="data-no-pause"/>
+          </xsl:if>
+          <!-- the actual list of exercises -->
+          <xsl:copy-of select="$the-exercises"/>
+          <!-- only at "section" level. only when building for a Runestone server -->
+          <xsl:apply-templates select="." mode="runestone-progress-indicator"/>
+        </ul>
+      </div>
+    </xsl:if>
+  </xsl:template>
+  <!-- An "exercises" division can be a group work exercise, by virtue -->
+  <!-- of selection and submission features at the bottom of the page. -->
+  <!-- NB: this assumes that the "exercises" is an entire page, so     -->
+  <!-- checks if it is a subdivision of a "chapter" (or "appendix").   -->
+  <xsl:template match="exercises" mode="runestone-group-work">
+    <xsl:if test="$b-host-runestone and (parent::chapter or parent::appendix)">
+      <div class="runestone">
+        <div data-component="groupsub">
+          <!-- the Runestone id -->
+          <xsl:apply-templates select="." mode="runestone-id-attribute"/>
+          <xsl:attribute name="data-size_limit">
+            <xsl:choose>
+              <xsl:when test="@group-size">
+                <xsl:value-of select="@group-size"/>
+              </xsl:when>
+              <xsl:otherwise>
+                <xsl:text>3</xsl:text>
+              </xsl:otherwise>
+            </xsl:choose>
+          </xsl:attribute>
+          <!-- students select their partners in their group -->
+          <div>
+            <select multiple="" class="assignment_partner_select" style="width: 100%"/>
+          </div>
+          <!-- and a submit button once done -->
+          <div class="groupsub_button"/>
+          <div class="para">The Submit Group button will submit the answer for each each question on this page for each member of your group. It also logs you as the official group submitter.</div>
+        </div>
+      </div>
+    </xsl:if>
+  </xsl:template>
   <!-- ################## -->
   <!-- Runestone Manifest -->
   <!-- ################## -->
   <!-- HTML ID and real title for each chapter and section -->
   <!-- A PTX "section" is a Runestone "subchapter"         -->
   <!-- Document hierarchy is preserved in XML structure    -->
   <!-- TODO: add exercises as "question"                   -->
```

#### pretext/braille_format.py

```diff
@@ -750,14 +750,26 @@
         return louis.translateString(["en-ueb-g2.ctb"], aline, None, 0)
 
     def process_block(self, blk):
 
         if blk.ownpage and self.cursor.embossing():
             self.advance_page()
 
+        # We don't want to start block material right at the bottom of
+        # the page when there are not enough lines to really get moving.
+        # Never start when there is one line left.  Most box material needs
+        # three lines, a preceding blank line, a box line, and a heading
+        # (maybe four lines? but three seems OK experimentally).
+        # Likely this needs refinement.
+        initial_lines = 1
+        if blk.box:
+            initial_lines += 2
+        if (self.cursor.remaining_lines() < initial_lines) and self.cursor.embossing():
+            self.advance_page()
+
         # Lines before (but not if at the start of a page)
         if not(self.cursor.at_page_start()):
             for i in range(blk.lines_before):
                 self.blank_line()
 
         if blk.box == "standard":
             top_line = "7" * self.line_buffer.text_width
```

#### pretext/pretext.py

```diff
@@ -2037,15 +2037,15 @@
     numAttempt = 0
     maxAttempts = 10  # In case failure is not due to blocked ports.
     while looking_for_port and numAttempt < maxAttempts:
         try:
             numAttempt = numAttempt + 1
             log.info(f"Opening subprocess http.server with port={port}")
             # -u so that stdout and stderr are not cached
-            server = subprocess.Popen(["python", "-u", "-m", "http.server", f"{port}", "-d", tmp_dir], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+            server = subprocess.Popen([sys.executable, "-u", "-m", "http.server", f"{port}", "-d", tmp_dir], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
             # Check if terminated. Allow 1 second to start-up.
             try:
                 result = server.wait(1)
                 log.debug(f"Server startup failed")
                 port = random.randint(49152, 65535)
                 log.debug(f"Trying port {port} instead")
             # The exception is success because process did not terminate.
```

### Comparing `pretext-1.6.1.dev20230701/pretext/generate.py` & `pretext-1.6.1.dev20230704/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pretext/project.py` & `pretext-1.6.1.dev20230704/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pretext/templates/__init__.py` & `pretext-1.6.1.dev20230704/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pretext/templates/resources/.gitignore` & `pretext-1.6.1.dev20230704/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pretext/templates/resources/article.zip` & `pretext-1.6.1.dev20230704/pretext/templates/resources/article.zip`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160110 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 source/
--rw-r--r--  2.0 unx       86 b- defN 23-Jul-01 06:13 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-01 06:14 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-01 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-01 06:14 .gitignore
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-01 06:13 assets/frog.jpg
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-01 06:14 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-01 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jul-01 06:13 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jul-01 06:13 source/main.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-Jul-01 06:13 source/section-1.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 source/
+-rw-r--r--  2.0 unx       86 b- defN 23-Jul-04 06:15 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-04 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-04 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-04 06:15 .gitignore
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jul-04 06:15 assets/frog.jpg
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-04 06:15 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-04 06:15 publication/publication.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jul-04 06:15 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jul-04 06:15 source/main.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-Jul-04 06:15 source/section-1.ptx
 14 files, 164841 bytes uncompressed, 158588 bytes compressed:  3.8%
```

### Comparing `pretext-1.6.1.dev20230701/pretext/templates/resources/book.zip` & `pretext-1.6.1.dev20230704/pretext/templates/resources/book.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7616 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 source/
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-01 06:13 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-01 06:14 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-01 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-01 06:14 .gitignore
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-01 06:14 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6114 b- defN 23-Jul-01 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jul-01 06:13 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-04 06:15 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-04 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-04 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-04 06:15 .gitignore
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-04 06:15 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jul-04 06:15 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jul-04 06:15 source/main.ptx
 10 files, 15809 bytes uncompressed, 6522 bytes compressed:  58.7%
```

### Comparing `pretext-1.6.1.dev20230701/pretext/templates/resources/demo.zip` & `pretext-1.6.1.dev20230704/pretext/templates/resources/demo.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173309 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 source/
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-01 06:13 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-01 06:14 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-01 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-01 06:14 .gitignore
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-01 06:13 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jul-01 06:13 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-01 06:14 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6092 b- defN 23-Jul-01 06:13 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 source/images/
--rw-r--r--  2.0 unx     1115 b- defN 23-Jul-01 06:13 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jul-01 06:13 source/backmatter.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jul-01 06:13 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jul-01 06:13 source/ch-empty.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jul-01 06:13 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jul-01 06:13 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jul-01 06:13 source/docinfo.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jul-01 06:13 source/main.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jul-01 06:13 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jul-01 06:13 source/frontmatter.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jul-01 06:13 source/ch-generate.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jul-01 06:13 source/ch-features.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-Jul-01 06:13 source/ex-first.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jul-01 06:13 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jul-01 06:13 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jul-01 06:13 source/sec-features.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-Jul-01 06:13 source/images/cflag.asy
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-01 06:13 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jul-01 06:13 source/images/tikz.tex
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-01 06:13 source/images/sageplot2d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-04 06:15 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-04 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-04 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-04 06:15 .gitignore
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jul-04 06:15 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jul-04 06:15 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-04 06:15 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jul-04 06:15 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 source/images/
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jul-04 06:15 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jul-04 06:15 source/backmatter.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jul-04 06:15 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jul-04 06:15 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jul-04 06:15 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jul-04 06:15 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jul-04 06:15 source/docinfo.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jul-04 06:15 source/main.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jul-04 06:15 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jul-04 06:15 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jul-04 06:15 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jul-04 06:15 source/ch-features.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jul-04 06:15 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jul-04 06:15 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jul-04 06:15 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Jul-04 06:15 source/sec-features.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-Jul-04 06:15 source/images/cflag.asy
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-04 06:15 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jul-04 06:15 source/images/tikz.tex
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-04 06:15 source/images/sageplot2d.sage
 34 files, 190104 bytes uncompressed, 169353 bytes compressed:  10.9%
```

### Comparing `pretext-1.6.1.dev20230701/pretext/templates/resources/devcontainer.json` & `pretext-1.6.1.dev20230704/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pretext/templates/resources/hello.zip` & `pretext-1.6.1.dev20230704/pretext/templates/resources/hello.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4657 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 source/
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-01 06:13 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-Jul-01 06:13 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-01 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-01 06:14 .gitignore
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-01 06:14 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-01 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jul-01 06:13 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 source/
+-rw-r--r--  2.0 unx       69 b- defN 23-Jul-04 06:15 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jul-04 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-04 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-04 06:15 .gitignore
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-04 06:15 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-04 06:15 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-Jul-04 06:15 source/main.ptx
 10 files, 7820 bytes uncompressed, 3563 bytes compressed:  54.4%
```

### Comparing `pretext-1.6.1.dev20230701/pretext/templates/resources/project.ptx` & `pretext-1.6.1.dev20230704/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pretext/templates/resources/slideshow.zip` & `pretext-1.6.1.dev20230704/pretext/templates/resources/slideshow.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8392 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:14 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-01 06:13 xsl/
--rw-r--r--  2.0 unx      784 b- defN 23-Jul-01 06:13 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jul-01 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-01 06:14 .gitignore
--rw-r--r--  2.0 unx      190 b- defN 23-Jul-01 06:13 xsl/slides.xsl
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-01 06:14 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     2097 b- defN 23-Jul-01 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jul-01 06:13 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-04 06:15 xsl/
+-rw-r--r--  2.0 unx      784 b- defN 23-Jul-04 06:15 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jul-04 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-04 06:15 .gitignore
+-rw-r--r--  2.0 unx      190 b- defN 23-Jul-04 06:15 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-04 06:15 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jul-04 06:15 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jul-04 06:15 source/main.ptx
 11 files, 20407 bytes uncompressed, 7204 bytes compressed:  64.7%
```

### Comparing `pretext-1.6.1.dev20230701/pretext/utils.py` & `pretext-1.6.1.dev20230704/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230701/pyproject.toml` & `pretext-1.6.1.dev20230704/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.6.1.dev20230701"
+version = "1.6.1.dev20230704"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.6.1.dev20230701/PKG-INFO` & `pretext-1.6.1.dev20230704/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.6.1.dev20230701
+Version: 1.6.1.dev20230704
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

