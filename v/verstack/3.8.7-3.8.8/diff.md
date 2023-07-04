# Comparing `tmp/verstack-3.8.7.tar.gz` & `tmp/verstack-3.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verstack-3.8.7.tar", last modified: Tue Jul  4 17:03:06 2023, max compression
+gzip compressed data, was "verstack-3.8.8.tar", last modified: Tue Jul  4 19:43:48 2023, max compression
```

## Comparing `verstack-3.8.7.tar` & `verstack-3.8.8.tar`

### file list

```diff
@@ -1,537 +1,537 @@
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.492540 verstack-3.8.7/
--rwxrwxrwx   0 danil      (501) staff       (20)      174 2021-11-08 12:56:11.000000 verstack-3.8.7/.readthedocs.yaml
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.394676 verstack-3.8.7/.vscode/
--rwxrwxrwx   0 danil      (501) staff       (20)      179 2023-06-12 05:32:34.000000 verstack-3.8.7/.vscode/settings.json
--rwxrwxrwx   0 danil      (501) staff       (20)     1071 2020-09-18 21:03:44.000000 verstack-3.8.7/LICENSE.txt
--rwxrwxrwx   0 danil      (501) staff       (20)      106 2020-09-18 21:51:05.000000 verstack-3.8.7/MANIFEST
--rw-r--r--   0 danil      (501) staff       (20)     3363 2023-07-04 17:03:06.492643 verstack-3.8.7/PKG-INFO
--rwxrwxrwx   0 danil      (501) staff       (20)     2268 2023-07-04 17:01:41.000000 verstack-3.8.7/README.rst
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.394832 verstack-3.8.7/dist/
--rwxrwxrwx   0 danil      (501) staff       (20)     7308 2020-09-18 21:51:05.000000 verstack-3.8.7/dist/verstack-0.1.0.tar.gz
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.395877 verstack-3.8.7/docs/
--rwxrwxrwx   0 danil      (501) staff       (20)      692 2023-02-12 13:53:02.000000 verstack-3.8.7/docs/Doc_update_manual.txt
--rwxrwxrwx   0 danil      (501) staff       (20)      638 2020-09-20 09:39:03.000000 verstack-3.8.7/docs/Makefile
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.386908 verstack-3.8.7/docs/build/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.397363 verstack-3.8.7/docs/build/doctrees/
--rwxrwxrwx   0 danil      (501) staff       (20)    26942 2020-09-20 12:30:25.000000 verstack-3.8.7/docs/build/doctrees/README.doctree
--rwxrwxrwx   0 danil      (501) staff       (20)   539532 2023-05-03 17:21:05.000000 verstack-3.8.7/docs/build/doctrees/environment.pickle
--rwxrwxrwx   0 danil      (501) staff       (20)   386763 2023-05-03 17:21:05.000000 verstack-3.8.7/docs/build/doctrees/index.doctree
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.399311 verstack-3.8.7/docs/build/html/
--rwxrwxrwx   0 danil      (501) staff       (20)      230 2023-05-03 17:21:06.000000 verstack-3.8.7/docs/build/html/.buildinfo
--rwxrwxrwx   0 danil      (501) staff       (20)        0 2020-09-20 11:46:51.000000 verstack-3.8.7/docs/build/html/.nojekyll
--rwxrwxrwx   0 danil      (501) staff       (20)    20042 2020-09-20 12:35:34.000000 verstack-3.8.7/docs/build/html/README.html
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.399729 verstack-3.8.7/docs/build/html/_sources/
--rwxrwxrwx   0 danil      (501) staff       (20)     6117 2020-09-19 13:46:17.000000 verstack-3.8.7/docs/build/html/_sources/README.md.txt
--rwxrwxrwx   0 danil      (501) staff       (20)     6298 2020-09-20 09:22:18.000000 verstack-3.8.7/docs/build/html/_sources/README.rst.txt
--rwxrwxrwx   0 danil      (501) staff       (20)    73602 2023-05-03 17:00:23.000000 verstack-3.8.7/docs/build/html/_sources/index.rst.txt
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.406345 verstack-3.8.7/docs/build/html/_static/
--rwxrwxrwx   0 danil      (501) staff       (20)    11185 2020-09-20 11:40:14.000000 verstack-3.8.7/docs/build/html/_static/alabaster.css
--rwxrwxrwx   0 danil      (501) staff       (20)    14813 2023-05-03 17:21:06.000000 verstack-3.8.7/docs/build/html/_static/basic.css
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.406787 verstack-3.8.7/docs/build/html/_static/css/
--rwxrwxrwx   0 danil      (501) staff       (20)    13353 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/css/bootstrap-theme.min.css
--rwxrwxrwx   0 danil      (501) staff       (20)   102105 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/css/bootstrap.min.css
--rwxrwxrwx   0 danil      (501) staff       (20)       42 2018-10-08 18:31:32.000000 verstack-3.8.7/docs/build/html/_static/custom.css
--rwxrwxrwx   0 danil      (501) staff       (20)     4472 2023-05-03 17:20:59.000000 verstack-3.8.7/docs/build/html/_static/doctools.js
--rwxrwxrwx   0 danil      (501) staff       (20)      420 2023-05-03 17:21:06.000000 verstack-3.8.7/docs/build/html/_static/documentation_options.js
--rwxrwxrwx   0 danil      (501) staff       (20)      286 2020-02-10 16:38:31.000000 verstack-3.8.7/docs/build/html/_static/file.png
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.419042 verstack-3.8.7/docs/build/html/_static/fonts/
--rwxrwxrwx   0 danil      (501) staff       (20)    18173 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    47724 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    31552 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    21624 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    21280 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    76169 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    45116 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    25740 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    18079 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400italic.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    80212 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400italic.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    34740 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400italic.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    20488 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400italic.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    20859 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    76108 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    43948 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    25232 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    18177 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700italic.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    79742 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700italic.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    34360 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700italic.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    20472 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700italic.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    16639 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    58571 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    29288 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19216 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    15864 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400italic.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    58853 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400italic.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    26644 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400italic.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    18396 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400italic.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    16716 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    57996 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    29704 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19332 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    16849 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700italic.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    58214 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700italic.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    28932 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700italic.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19444 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700italic.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    24132 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    95257 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    42116 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    26804 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    22002 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400italic.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    70885 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400italic.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    38736 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400italic.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    25372 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400italic.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    27033 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    96461 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    47276 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    30532 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    25348 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700italic.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   107048 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700italic.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    44008 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700italic.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    28060 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700italic.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    14004 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_400.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    61056 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_400.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    27916 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_400.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    15640 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_400.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    13750 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_700.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    59518 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_700.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    27696 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_700.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    15340 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_700.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    20290 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    62850 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    41236 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    23292 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.419204 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.427564 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/
--rwxrwxrwx   0 danil      (501) staff       (20)    30858 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    57401 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    30680 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19788 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    34166 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    60750 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    33960 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    21940 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    30602 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    58215 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    30404 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19972 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    33758 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    61071 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    33532 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    21824 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    34798 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    62096 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    34612 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    22416 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    29794 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    56447 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    29612 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19396 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    34578 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    62430 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    34368 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    22444 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    29934 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    58495 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    29744 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19624 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    30350 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    57560 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    30156 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19736 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    34866 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    62044 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    34644 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    22332 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)     5151 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/open-sans/stylesheet.css
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.428556 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.429819 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/
--rwxrwxrwx   0 danil      (501) staff       (20)   111902 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   113630 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   112362 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   112866 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   112354 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   113510 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot
--rwxrwxrwx   0 danil      (501) staff       (20)     4616 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/LICENSE.txt
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.431103 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/
--rwxrwxrwx   0 danil      (501) staff       (20)    91216 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    92760 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    89720 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    91424 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    91276 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    93144 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf
--rwxrwxrwx   0 danil      (501) staff       (20)     1081 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/README.md
--rwxrwxrwx   0 danil      (501) staff       (20)     4402 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/ReadMe.html
--rwxrwxrwx   0 danil      (501) staff       (20)    11781 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.432728 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/
--rwxrwxrwx   0 danil      (501) staff       (20)   111572 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   113320 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   112004 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   112528 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   112048 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   113168 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.387930 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.433818 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/
--rwxrwxrwx   0 danil      (501) staff       (20)    48788 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    51188 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    47136 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    49672 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    48972 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    51272 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.434938 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/
--rwxrwxrwx   0 danil      (501) staff       (20)    49496 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    51924 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    48784 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    50792 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    49604 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    51772 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)      404 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/bower.json
--rwxrwxrwx   0 danil      (501) staff       (20)     2429 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/source-serif-pro.css
--rwxrwxrwx   0 danil      (501) staff       (20)    18299 2023-05-03 17:21:06.000000 verstack-3.8.7/docs/build/html/_static/guzzle.css
--rwxrwxrwx   0 danil      (501) staff       (20)     1912 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-example.png
--rwxrwxrwx   0 danil      (501) staff       (20)     1478 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-important.png
--rwxrwxrwx   0 danil      (501) staff       (20)     1234 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-javascript-example.png
--rwxrwxrwx   0 danil      (501) staff       (20)     1086 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-json-example.png
--rwxrwxrwx   0 danil      (501) staff       (20)     1526 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-lconf-example.png
--rwxrwxrwx   0 danil      (501) staff       (20)     2331 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-note.png
--rwxrwxrwx   0 danil      (501) staff       (20)      679 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-optional.png
--rwxrwxrwx   0 danil      (501) staff       (20)      759 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-python-example.png
--rwxrwxrwx   0 danil      (501) staff       (20)     1701 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-seealso.png
--rwxrwxrwx   0 danil      (501) staff       (20)     1082 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-shell-example.png
--rwxrwxrwx   0 danil      (501) staff       (20)     1912 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-text-example.png
--rwxrwxrwx   0 danil      (501) staff       (20)      587 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-tip.png
--rwxrwxrwx   0 danil      (501) staff       (20)     2271 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-todo.png
--rwxrwxrwx   0 danil      (501) staff       (20)     1962 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/icon-warning.png
--rwxrwxrwx   0 danil      (501) staff       (20)   280364 2020-02-10 16:38:31.000000 verstack-3.8.7/docs/build/html/_static/jquery-3.4.1.js
--rwxrwxrwx   0 danil      (501) staff       (20)   287630 2020-09-20 11:51:08.000000 verstack-3.8.7/docs/build/html/_static/jquery-3.5.1.js
--rwxrwxrwx   0 danil      (501) staff       (20)     3510 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/jquery.cookie.js
--rwxrwxrwx   0 danil      (501) staff       (20)    92634 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/jquery.js
--rwxrwxrwx   0 danil      (501) staff       (20)   138746 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/jquery.min.map
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.435508 verstack-3.8.7/docs/build/html/_static/js/
--rwxrwxrwx   0 danil      (501) staff       (20)    55329 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/js/bootstrap.js
--rwxrwxrwx   0 danil      (501) staff       (20)    29182 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/build/html/_static/js/bootstrap.min.js
--rwxrwxrwx   0 danil      (501) staff       (20)     4758 2023-05-03 17:21:06.000000 verstack-3.8.7/docs/build/html/_static/language_data.js
--rwxrwxrwx   0 danil      (501) staff       (20)    14747 2020-09-20 11:42:10.000000 verstack-3.8.7/docs/build/html/_static/local_fonts.css
--rwxrwxrwx   0 danil      (501) staff       (20)       90 2020-02-10 16:38:31.000000 verstack-3.8.7/docs/build/html/_static/minus.png
--rwxrwxrwx   0 danil      (501) staff       (20)    27652 2020-09-20 11:45:40.000000 verstack-3.8.7/docs/build/html/_static/p_sphinx_theme.css
--rwxrwxrwx   0 danil      (501) staff       (20)    17752 2020-09-20 11:45:40.000000 verstack-3.8.7/docs/build/html/_static/p_sphinx_theme.js
--rwxrwxrwx   0 danil      (501) staff       (20)       90 2020-02-10 16:38:31.000000 verstack-3.8.7/docs/build/html/_static/plus.png
--rwxrwxrwx   0 danil      (501) staff       (20)     4846 2023-05-03 17:21:06.000000 verstack-3.8.7/docs/build/html/_static/pygments.css
--rwxrwxrwx   0 danil      (501) staff       (20)    18215 2023-05-03 17:20:59.000000 verstack-3.8.7/docs/build/html/_static/searchtools.js
--rwxrwxrwx   0 danil      (501) staff       (20)    67692 2021-05-11 23:58:54.000000 verstack-3.8.7/docs/build/html/_static/underscore-1.12.0.js
--rwxrwxrwx   0 danil      (501) staff       (20)    68420 2021-08-12 13:47:18.000000 verstack-3.8.7/docs/build/html/_static/underscore-1.13.1.js
--rwxrwxrwx   0 danil      (501) staff       (20)    35168 2020-02-10 16:38:31.000000 verstack-3.8.7/docs/build/html/_static/underscore-1.3.1.js
--rwxrwxrwx   0 danil      (501) staff       (20)    19358 2021-05-11 23:58:54.000000 verstack-3.8.7/docs/build/html/_static/underscore.js
--rwxrwxrwx   0 danil      (501) staff       (20)     3388 2023-05-03 17:21:05.000000 verstack-3.8.7/docs/build/html/genindex.html
--rwxrwxrwx   0 danil      (501) staff       (20)   162215 2023-05-03 17:21:05.000000 verstack-3.8.7/docs/build/html/index.html
--rwxrwxrwx   0 danil      (501) staff       (20)      254 2023-05-03 17:21:06.000000 verstack-3.8.7/docs/build/html/objects.inv
--rwxrwxrwx   0 danil      (501) staff       (20)     4500 2023-05-03 17:21:06.000000 verstack-3.8.7/docs/build/html/search.html
--rwxrwxrwx   0 danil      (501) staff       (20)    16283 2023-05-03 17:21:06.000000 verstack-3.8.7/docs/build/html/searchindex.js
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.435765 verstack-3.8.7/docs/guzzle_sphinx_theme/
--rwxrwxrwx   0 danil      (501) staff       (20)     4856 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/__init__.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.435941 verstack-3.8.7/docs/guzzle_sphinx_theme/__pycache__/
--rwxrwxrwx   0 danil      (501) staff       (20)     5478 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/__pycache__/__init__.cpython-37.pyc
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.437178 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/
--rwxrwxrwx   0 danil      (501) staff       (20)      828 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/comments.html
--rwxrwxrwx   0 danil      (501) staff       (20)      323 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/globaltoc.html
--rwxrwxrwx   0 danil      (501) staff       (20)     5778 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/layout.html
--rwxrwxrwx   0 danil      (501) staff       (20)      206 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/localtoc.html
--rwxrwxrwx   0 danil      (501) staff       (20)       92 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/logo-text.html
--rwxrwxrwx   0 danil      (501) staff       (20)     1695 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/search.html
--rwxrwxrwx   0 danil      (501) staff       (20)      521 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/searchbox.html
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.437696 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.438075 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/
--rwxrwxrwx   0 danil      (501) staff       (20)    13353 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap-theme.min.css
--rwxrwxrwx   0 danil      (501) staff       (20)   102105 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap.min.css
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.439121 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/
--rwxrwxrwx   0 danil      (501) staff       (20)    20290 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    62850 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    41236 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    23292 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.439301 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.448174 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/
--rwxrwxrwx   0 danil      (501) staff       (20)    30858 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    57401 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    30680 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19788 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    34166 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    60750 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    33960 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    21940 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    30602 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    58215 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    30404 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19972 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    33758 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    61071 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    33532 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    21824 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    34798 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    62096 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    34612 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    22416 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    29794 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    56447 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    29612 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19396 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    34578 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    62430 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    34368 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    22444 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    29934 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    58495 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    29744 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19624 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    30350 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    57560 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    30156 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19736 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    34866 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    62044 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    34644 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    22332 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)     5151 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/stylesheet.css
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.449061 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.450149 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/
--rwxrwxrwx   0 danil      (501) staff       (20)   111902 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   113630 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   112362 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   112866 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   112354 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   113510 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot
--rwxrwxrwx   0 danil      (501) staff       (20)     4616 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/LICENSE.txt
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.451281 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/
--rwxrwxrwx   0 danil      (501) staff       (20)    91216 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    92760 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    89720 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    91424 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    91276 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    93144 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf
--rwxrwxrwx   0 danil      (501) staff       (20)     1081 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/README.md
--rwxrwxrwx   0 danil      (501) staff       (20)     4402 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/ReadMe.html
--rwxrwxrwx   0 danil      (501) staff       (20)    11781 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/SourceSerifProReadMe.html
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.452394 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/
--rwxrwxrwx   0 danil      (501) staff       (20)   111572 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   113320 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   112004 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   112528 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   112048 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   113168 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.389667 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.453379 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/
--rwxrwxrwx   0 danil      (501) staff       (20)    48788 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    51188 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    47136 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    49672 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    48972 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    51272 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.454367 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/
--rwxrwxrwx   0 danil      (501) staff       (20)    49496 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    51924 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    48784 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    50792 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    49604 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    51772 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)      404 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/bower.json
--rwxrwxrwx   0 danil      (501) staff       (20)     2429 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/source-serif-pro.css
--rwxrwxrwx   0 danil      (501) staff       (20)    18300 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/guzzle.css_t
--rwxrwxrwx   0 danil      (501) staff       (20)    92634 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.js
--rwxrwxrwx   0 danil      (501) staff       (20)   138746 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.min.map
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.455235 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/
--rwxrwxrwx   0 danil      (501) staff       (20)    55329 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.js
--rwxrwxrwx   0 danil      (501) staff       (20)    29182 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.min.js
--rwxrwxrwx   0 danil      (501) staff       (20)      649 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/theme.conf
--rwxrwxrwx   0 danil      (501) staff       (20)      799 2020-09-20 09:39:03.000000 verstack-3.8.7/docs/make.bat
--rwxrwxrwx   0 danil      (501) staff       (20)       57 2023-05-04 06:42:41.000000 verstack-3.8.7/docs/requirements.txt
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.455657 verstack-3.8.7/docs/source/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.390109 verstack-3.8.7/docs/source/_build/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.457872 verstack-3.8.7/docs/source/_build/html/
--rwxrwxrwx   0 danil      (501) staff       (20)      230 2022-02-10 20:51:20.000000 verstack-3.8.7/docs/source/_build/html/.buildinfo
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.458776 verstack-3.8.7/docs/source/_build/html/.doctrees/
--rwxrwxrwx   0 danil      (501) staff       (20)    34100 2022-02-10 20:51:19.000000 verstack-3.8.7/docs/source/_build/html/.doctrees/environment.pickle
--rwxrwxrwx   0 danil      (501) staff       (20)   233769 2022-02-10 20:51:19.000000 verstack-3.8.7/docs/source/_build/html/.doctrees/index.doctree
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.459196 verstack-3.8.7/docs/source/_build/html/_sources/
--rwxrwxrwx   0 danil      (501) staff       (20)    42285 2022-02-10 20:51:17.000000 verstack-3.8.7/docs/source/_build/html/_sources/index.rst.txt
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.462746 verstack-3.8.7/docs/source/_build/html/_static/
--rwxrwxrwx   0 danil      (501) staff       (20)    14652 2022-02-10 20:51:20.000000 verstack-3.8.7/docs/source/_build/html/_static/basic.css
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.463172 verstack-3.8.7/docs/source/_build/html/_static/css/
--rwxrwxrwx   0 danil      (501) staff       (20)    13353 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/css/bootstrap-theme.min.css
--rwxrwxrwx   0 danil      (501) staff       (20)   102105 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/css/bootstrap.min.css
--rwxrwxrwx   0 danil      (501) staff       (20)     9592 2021-05-11 23:58:54.000000 verstack-3.8.7/docs/source/_build/html/_static/doctools.js
--rwxrwxrwx   0 danil      (501) staff       (20)      355 2022-02-10 20:51:20.000000 verstack-3.8.7/docs/source/_build/html/_static/documentation_options.js
--rwxrwxrwx   0 danil      (501) staff       (20)      286 2021-05-11 23:58:54.000000 verstack-3.8.7/docs/source/_build/html/_static/file.png
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.464116 verstack-3.8.7/docs/source/_build/html/_static/fonts/
--rwxrwxrwx   0 danil      (501) staff       (20)    20290 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    62850 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    41236 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    23292 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.464290 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.473952 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/
--rwxrwxrwx   0 danil      (501) staff       (20)    30858 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    57401 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    30680 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19788 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    34166 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    60750 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    33960 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    21940 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    30602 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    58215 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    30404 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19972 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    33758 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    61071 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    33532 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    21824 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    34798 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    62096 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    34612 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    22416 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    29794 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    56447 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    29612 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19396 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    34578 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    62430 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    34368 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    22444 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    29934 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    58495 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    29744 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19624 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    30350 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    57560 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    30156 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    19736 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    34866 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot
--rwxrwxrwx   0 danil      (501) staff       (20)    62044 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg
--rwxrwxrwx   0 danil      (501) staff       (20)    34644 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)    22332 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff
--rwxrwxrwx   0 danil      (501) staff       (20)     5151 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/stylesheet.css
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.475619 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.476882 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/
--rwxrwxrwx   0 danil      (501) staff       (20)   111902 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   113630 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   112362 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   112866 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   112354 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot
--rwxrwxrwx   0 danil      (501) staff       (20)   113510 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot
--rwxrwxrwx   0 danil      (501) staff       (20)     4616 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/LICENSE.txt
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.478041 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/
--rwxrwxrwx   0 danil      (501) staff       (20)    91216 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    92760 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    89720 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    91424 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    91276 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf
--rwxrwxrwx   0 danil      (501) staff       (20)    93144 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf
--rwxrwxrwx   0 danil      (501) staff       (20)     1081 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/README.md
--rwxrwxrwx   0 danil      (501) staff       (20)     4402 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/ReadMe.html
--rwxrwxrwx   0 danil      (501) staff       (20)    11781 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.479442 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/
--rwxrwxrwx   0 danil      (501) staff       (20)   111572 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   113320 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   112004 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   112528 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   112048 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf
--rwxrwxrwx   0 danil      (501) staff       (20)   113168 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.391700 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.480652 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/
--rwxrwxrwx   0 danil      (501) staff       (20)    48788 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    51188 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    47136 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    49672 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    48972 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    51272 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.481876 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/
--rwxrwxrwx   0 danil      (501) staff       (20)    49496 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    51924 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    48784 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    50792 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    49604 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)    51772 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff
--rwxrwxrwx   0 danil      (501) staff       (20)      404 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/bower.json
--rwxrwxrwx   0 danil      (501) staff       (20)     2429 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/source-serif-pro.css
--rwxrwxrwx   0 danil      (501) staff       (20)    18299 2022-02-10 20:51:20.000000 verstack-3.8.7/docs/source/_build/html/_static/guzzle.css
--rwxrwxrwx   0 danil      (501) staff       (20)   287630 2021-05-11 23:58:54.000000 verstack-3.8.7/docs/source/_build/html/_static/jquery-3.5.1.js
--rwxrwxrwx   0 danil      (501) staff       (20)    92634 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/jquery.js
--rwxrwxrwx   0 danil      (501) staff       (20)   138746 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/jquery.min.map
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.483229 verstack-3.8.7/docs/source/_build/html/_static/js/
--rwxrwxrwx   0 danil      (501) staff       (20)    55329 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/js/bootstrap.js
--rwxrwxrwx   0 danil      (501) staff       (20)    29182 2020-09-20 11:50:32.000000 verstack-3.8.7/docs/source/_build/html/_static/js/bootstrap.min.js
--rwxrwxrwx   0 danil      (501) staff       (20)    10854 2022-02-10 20:51:20.000000 verstack-3.8.7/docs/source/_build/html/_static/language_data.js
--rwxrwxrwx   0 danil      (501) staff       (20)       90 2021-05-11 23:58:54.000000 verstack-3.8.7/docs/source/_build/html/_static/minus.png
--rwxrwxrwx   0 danil      (501) staff       (20)       90 2021-05-11 23:58:54.000000 verstack-3.8.7/docs/source/_build/html/_static/plus.png
--rwxrwxrwx   0 danil      (501) staff       (20)     4846 2022-02-10 20:51:20.000000 verstack-3.8.7/docs/source/_build/html/_static/pygments.css
--rwxrwxrwx   0 danil      (501) staff       (20)    16578 2021-05-11 23:58:54.000000 verstack-3.8.7/docs/source/_build/html/_static/searchtools.js
--rwxrwxrwx   0 danil      (501) staff       (20)    67692 2021-05-11 23:58:54.000000 verstack-3.8.7/docs/source/_build/html/_static/underscore-1.12.0.js
--rwxrwxrwx   0 danil      (501) staff       (20)    19358 2021-05-11 23:58:54.000000 verstack-3.8.7/docs/source/_build/html/_static/underscore.js
--rwxrwxrwx   0 danil      (501) staff       (20)     3419 2022-02-10 20:51:20.000000 verstack-3.8.7/docs/source/_build/html/genindex.html
--rwxrwxrwx   0 danil      (501) staff       (20)   101829 2022-02-10 20:51:19.000000 verstack-3.8.7/docs/source/_build/html/index.html
--rwxrwxrwx   0 danil      (501) staff       (20)      254 2022-02-10 20:51:20.000000 verstack-3.8.7/docs/source/_build/html/objects.inv
--rwxrwxrwx   0 danil      (501) staff       (20)     4531 2022-02-10 20:51:20.000000 verstack-3.8.7/docs/source/_build/html/search.html
--rwxrwxrwx   0 danil      (501) staff       (20)     6846 2022-02-10 20:51:20.000000 verstack-3.8.7/docs/source/_build/html/searchindex.js
--rwxrwxrwx   0 danil      (501) staff       (20)     5224 2023-05-03 17:20:38.000000 verstack-3.8.7/docs/source/conf.py
--rwxrwxrwx   0 danil      (501) staff       (20)    73841 2023-07-04 17:01:31.000000 verstack-3.8.7/docs/source/index.rst
--rwxrwxrwx   0 danil      (501) staff       (20)      548 2023-02-12 13:52:00.000000 verstack-3.8.7/increment_version.py
--rwxrwxrwx   0 danil      (501) staff       (20)   253628 2023-02-12 13:48:06.000000 verstack-3.8.7/logo.png
--rwxrwxrwx   0 danil      (501) staff       (20)   200067 2023-02-12 13:48:04.000000 verstack-3.8.7/logo.pxd
--rwxrwxrwx   0 danil      (501) staff       (20)     1703 2023-02-12 13:53:15.000000 verstack-3.8.7/package_update_instructions.txt
--rwxrwxrwx   0 danil      (501) staff       (20)      306 2023-07-04 16:34:54.000000 verstack-3.8.7/requirements.txt
--rwxrwxrwx   0 danil      (501) staff       (20)       80 2023-07-04 17:03:06.493182 verstack-3.8.7/setup.cfg
--rwxrwxrwx   0 danil      (501) staff       (20)     2235 2023-07-04 17:03:02.000000 verstack-3.8.7/setup.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.485602 verstack-3.8.7/verstack/
--rwxrwxrwx   0 danil      (501) staff       (20)    39819 2023-01-16 10:00:49.000000 verstack-3.8.7/verstack/DateParser.py
--rwxrwxrwx   0 danil      (501) staff       (20)    24790 2023-05-03 13:58:53.000000 verstack-3.8.7/verstack/FeatureSelector.py
--rwxrwxrwx   0 danil      (501) staff       (20)     7756 2022-04-29 08:46:57.000000 verstack-3.8.7/verstack/Multicore.py
--rwxrwxrwx   0 danil      (501) staff       (20)    18447 2022-12-09 20:53:43.000000 verstack-3.8.7/verstack/NaNImputer.py
--rwxrwxrwx   0 danil      (501) staff       (20)    33143 2022-12-09 20:16:44.000000 verstack-3.8.7/verstack/NaNImputerLegacy.py
--rwxrwxrwx   0 danil      (501) staff       (20)    12408 2022-12-19 10:43:57.000000 verstack-3.8.7/verstack/PandasOptimizer.py
--rwxrwxrwx   0 danil      (501) staff       (20)     8816 2023-03-28 10:21:12.000000 verstack-3.8.7/verstack/ThreshTuner.py
--rwxrwxrwx   0 danil      (501) staff       (20)      980 2022-12-19 08:48:26.000000 verstack-3.8.7/verstack/__init__.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.487815 verstack-3.8.7/verstack/categoric_encoders/
--rwxrwxrwx   0 danil      (501) staff       (20)     5115 2022-04-29 12:08:27.000000 verstack-3.8.7/verstack/categoric_encoders/Factorizer.py
--rwxrwxrwx   0 danil      (501) staff       (20)     4669 2022-04-28 10:31:19.000000 verstack-3.8.7/verstack/categoric_encoders/FrequencyEncoder.py
--rwxrwxrwx   0 danil      (501) staff       (20)     7499 2023-01-11 14:23:40.000000 verstack-3.8.7/verstack/categoric_encoders/MeanTargetEncoder.py
--rwxrwxrwx   0 danil      (501) staff       (20)     6647 2022-04-28 09:22:13.000000 verstack-3.8.7/verstack/categoric_encoders/OneHotEncoder.py
--rwxrwxrwx   0 danil      (501) staff       (20)     7352 2022-04-28 09:22:53.000000 verstack-3.8.7/verstack/categoric_encoders/WeightOfEvidenceEncoder.py
--rwxrwxrwx   0 danil      (501) staff       (20)        0 2021-12-07 14:06:33.000000 verstack-3.8.7/verstack/categoric_encoders/__init__.py
--rwxrwxrwx   0 danil      (501) staff       (20)     2173 2021-12-06 19:04:49.000000 verstack-3.8.7/verstack/categoric_encoders/args_validators.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.488796 verstack-3.8.7/verstack/lgbm_optuna_tuning/
--rwxrwxrwx   0 danil      (501) staff       (20)    50648 2023-07-04 13:09:22.000000 verstack-3.8.7/verstack/lgbm_optuna_tuning/LGBMTuner.py
--rwxrwxrwx   0 danil      (501) staff       (20)        0 2021-12-22 20:41:08.000000 verstack-3.8.7/verstack/lgbm_optuna_tuning/__init__.py
--rwxrwxrwx   0 danil      (501) staff       (20)     1865 2023-06-22 10:27:54.000000 verstack-3.8.7/verstack/lgbm_optuna_tuning/args_validators.py
--rwxrwxrwx   0 danil      (501) staff       (20)    17393 2023-06-22 10:27:35.000000 verstack-3.8.7/verstack/lgbm_optuna_tuning/lgb_metrics.py
--rwxrwxrwx   0 danil      (501) staff       (20)      859 2021-12-21 19:02:16.000000 verstack-3.8.7/verstack/lgbm_optuna_tuning/optuna_tools.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.489910 verstack-3.8.7/verstack/stacking/
--rwxrwxrwx   0 danil      (501) staff       (20)    30222 2022-12-11 11:13:47.000000 verstack-3.8.7/verstack/stacking/Stacker.py
--rwxrwxrwx   0 danil      (501) staff       (20)        0 2022-04-04 06:15:43.000000 verstack-3.8.7/verstack/stacking/__init__.py
--rwxrwxrwx   0 danil      (501) staff       (20)     2371 2022-05-04 09:07:10.000000 verstack-3.8.7/verstack/stacking/args_validators.py
--rwxrwxrwx   0 danil      (501) staff       (20)     3627 2022-04-05 06:23:16.000000 verstack-3.8.7/verstack/stacking/generate_default_layers.py
--rwxrwxrwx   0 danil      (501) staff       (20)     5546 2023-07-04 17:01:11.000000 verstack-3.8.7/verstack/stacking/kerasModel.py
--rwxrwxrwx   0 danil      (501) staff       (20)     3033 2022-12-11 11:14:24.000000 verstack-3.8.7/verstack/stacking/load_stacker.py
--rwxrwxrwx   0 danil      (501) staff       (20)     7657 2022-04-28 09:37:07.000000 verstack-3.8.7/verstack/stacking/optimise_params.py
--rwxrwxrwx   0 danil      (501) staff       (20)     8946 2023-02-12 14:01:23.000000 verstack-3.8.7/verstack/stratified_continuous_split.py
--rwxrwxrwx   0 danil      (501) staff       (20)     3523 2022-06-09 19:16:34.000000 verstack-3.8.7/verstack/tools.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.492402 verstack-3.8.7/verstack/unittest/
--rwxrwxrwx   0 danil      (501) staff       (20)    25047 2023-05-03 13:08:18.000000 verstack-3.8.7/verstack/unittest/boston_train.parquet
--rwxrwxrwx   0 danil      (501) staff       (20)     2443 2023-01-16 10:07:03.000000 verstack-3.8.7/verstack/unittest/common.py
--rwxrwxrwx   0 danil      (501) staff       (20)      373 2023-01-16 10:07:50.000000 verstack-3.8.7/verstack/unittest/test_DateParser.py
--rwxrwxrwx   0 danil      (501) staff       (20)      939 2022-12-06 11:05:04.000000 verstack-3.8.7/verstack/unittest/test_Factorizer.py
--rwxrwxrwx   0 danil      (501) staff       (20)      984 2022-12-06 11:13:56.000000 verstack-3.8.7/verstack/unittest/test_FrequencyEncoder.py
--rwxrwxrwx   0 danil      (501) staff       (20)      881 2023-06-12 05:44:26.000000 verstack-3.8.7/verstack/unittest/test_LGBMTuner.py
--rwxrwxrwx   0 danil      (501) staff       (20)      791 2022-12-06 11:20:55.000000 verstack-3.8.7/verstack/unittest/test_MeanTargetEncoder.py
--rwxrwxrwx   0 danil      (501) staff       (20)      600 2022-12-06 11:33:00.000000 verstack-3.8.7/verstack/unittest/test_Multicore.py
--rwxrwxrwx   0 danil      (501) staff       (20)      393 2022-12-06 11:34:15.000000 verstack-3.8.7/verstack/unittest/test_NaNImputer.py
--rwxrwxrwx   0 danil      (501) staff       (20)      531 2022-12-06 11:35:42.000000 verstack-3.8.7/verstack/unittest/test_OneHotEncoder.py
--rwxrwxrwx   0 danil      (501) staff       (20)      414 2022-12-19 09:08:24.000000 verstack-3.8.7/verstack/unittest/test_PandasOptimizer.py
--rwxrwxrwx   0 danil      (501) staff       (20)      336 2022-12-06 11:37:18.000000 verstack-3.8.7/verstack/unittest/test_Printer.py
--rwxrwxrwx   0 danil      (501) staff       (20)     1726 2022-12-11 12:01:19.000000 verstack-3.8.7/verstack/unittest/test_Stacker.py
--rwxrwxrwx   0 danil      (501) staff       (20)      710 2022-12-13 07:01:40.000000 verstack-3.8.7/verstack/unittest/test_ThreshTuner.py
--rwxrwxrwx   0 danil      (501) staff       (20)      863 2022-12-06 14:19:28.000000 verstack-3.8.7/verstack/unittest/test_WeightOfEvidenceEncoder.py
--rwxrwxrwx   0 danil      (501) staff       (20)      501 2023-05-03 13:08:40.000000 verstack-3.8.7/verstack/unittest/test_stratified_continuous_split.py
--rwxrwxrwx   0 danil      (501) staff       (20)     1370 2022-12-06 14:58:08.000000 verstack-3.8.7/verstack/unittest/unittesting_manual.txt
--rwxrwxrwx   0 danil      (501) staff       (20)       21 2023-07-04 17:01:37.000000 verstack-3.8.7/verstack/version.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 17:03:06.486578 verstack-3.8.7/verstack.egg-info/
--rwxrwxrwx   0 danil      (501) staff       (20)     3363 2023-07-04 17:03:06.000000 verstack-3.8.7/verstack.egg-info/PKG-INFO
--rwxrwxrwx   0 danil      (501) staff       (20)    31441 2023-07-04 17:03:06.000000 verstack-3.8.7/verstack.egg-info/SOURCES.txt
--rwxrwxrwx   0 danil      (501) staff       (20)        1 2023-07-04 17:03:06.000000 verstack-3.8.7/verstack.egg-info/dependency_links.txt
--rwxrwxrwx   0 danil      (501) staff       (20)      291 2023-07-04 17:03:06.000000 verstack-3.8.7/verstack.egg-info/requires.txt
--rwxrwxrwx   0 danil      (501) staff       (20)        9 2023-07-04 17:03:06.000000 verstack-3.8.7/verstack.egg-info/top_level.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.368751 verstack-3.8.8/
+-rwxrwxrwx   0 danil      (501) staff       (20)      174 2021-11-08 12:56:11.000000 verstack-3.8.8/.readthedocs.yaml
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.285213 verstack-3.8.8/.vscode/
+-rwxrwxrwx   0 danil      (501) staff       (20)      179 2023-06-12 05:32:34.000000 verstack-3.8.8/.vscode/settings.json
+-rwxrwxrwx   0 danil      (501) staff       (20)     1071 2020-09-18 21:03:44.000000 verstack-3.8.8/LICENSE.txt
+-rwxrwxrwx   0 danil      (501) staff       (20)      106 2020-09-18 21:51:05.000000 verstack-3.8.8/MANIFEST
+-rw-r--r--   0 danil      (501) staff       (20)     3363 2023-07-04 19:43:48.368847 verstack-3.8.8/PKG-INFO
+-rwxrwxrwx   0 danil      (501) staff       (20)     2268 2023-07-04 19:41:11.000000 verstack-3.8.8/README.rst
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.285345 verstack-3.8.8/dist/
+-rwxrwxrwx   0 danil      (501) staff       (20)     7308 2020-09-18 21:51:05.000000 verstack-3.8.8/dist/verstack-0.1.0.tar.gz
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.285826 verstack-3.8.8/docs/
+-rwxrwxrwx   0 danil      (501) staff       (20)      692 2023-02-12 13:53:02.000000 verstack-3.8.8/docs/Doc_update_manual.txt
+-rwxrwxrwx   0 danil      (501) staff       (20)      638 2020-09-20 09:39:03.000000 verstack-3.8.8/docs/Makefile
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.278002 verstack-3.8.8/docs/build/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.286457 verstack-3.8.8/docs/build/doctrees/
+-rwxrwxrwx   0 danil      (501) staff       (20)    26942 2020-09-20 12:30:25.000000 verstack-3.8.8/docs/build/doctrees/README.doctree
+-rwxrwxrwx   0 danil      (501) staff       (20)   539532 2023-05-03 17:21:05.000000 verstack-3.8.8/docs/build/doctrees/environment.pickle
+-rwxrwxrwx   0 danil      (501) staff       (20)   386763 2023-05-03 17:21:05.000000 verstack-3.8.8/docs/build/doctrees/index.doctree
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.287669 verstack-3.8.8/docs/build/html/
+-rwxrwxrwx   0 danil      (501) staff       (20)      230 2023-05-03 17:21:06.000000 verstack-3.8.8/docs/build/html/.buildinfo
+-rwxrwxrwx   0 danil      (501) staff       (20)        0 2020-09-20 11:46:51.000000 verstack-3.8.8/docs/build/html/.nojekyll
+-rwxrwxrwx   0 danil      (501) staff       (20)    20042 2020-09-20 12:35:34.000000 verstack-3.8.8/docs/build/html/README.html
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.288043 verstack-3.8.8/docs/build/html/_sources/
+-rwxrwxrwx   0 danil      (501) staff       (20)     6117 2020-09-19 13:46:17.000000 verstack-3.8.8/docs/build/html/_sources/README.md.txt
+-rwxrwxrwx   0 danil      (501) staff       (20)     6298 2020-09-20 09:22:18.000000 verstack-3.8.8/docs/build/html/_sources/README.rst.txt
+-rwxrwxrwx   0 danil      (501) staff       (20)    73602 2023-05-03 17:00:23.000000 verstack-3.8.8/docs/build/html/_sources/index.rst.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.295291 verstack-3.8.8/docs/build/html/_static/
+-rwxrwxrwx   0 danil      (501) staff       (20)    11185 2020-09-20 11:40:14.000000 verstack-3.8.8/docs/build/html/_static/alabaster.css
+-rwxrwxrwx   0 danil      (501) staff       (20)    14813 2023-05-03 17:21:06.000000 verstack-3.8.8/docs/build/html/_static/basic.css
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.295807 verstack-3.8.8/docs/build/html/_static/css/
+-rwxrwxrwx   0 danil      (501) staff       (20)    13353 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/css/bootstrap-theme.min.css
+-rwxrwxrwx   0 danil      (501) staff       (20)   102105 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/css/bootstrap.min.css
+-rwxrwxrwx   0 danil      (501) staff       (20)       42 2018-10-08 18:31:32.000000 verstack-3.8.8/docs/build/html/_static/custom.css
+-rwxrwxrwx   0 danil      (501) staff       (20)     4472 2023-05-03 17:20:59.000000 verstack-3.8.8/docs/build/html/_static/doctools.js
+-rwxrwxrwx   0 danil      (501) staff       (20)      420 2023-05-03 17:21:06.000000 verstack-3.8.8/docs/build/html/_static/documentation_options.js
+-rwxrwxrwx   0 danil      (501) staff       (20)      286 2020-02-10 16:38:31.000000 verstack-3.8.8/docs/build/html/_static/file.png
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.306392 verstack-3.8.8/docs/build/html/_static/fonts/
+-rwxrwxrwx   0 danil      (501) staff       (20)    18173 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Droid_Sans_Mono_400.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    47724 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Droid_Sans_Mono_400.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    31552 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Droid_Sans_Mono_400.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    21624 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Droid_Sans_Mono_400.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    21280 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    76169 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    45116 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    25740 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    18079 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400italic.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    80212 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400italic.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    34740 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400italic.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    20488 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400italic.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    20859 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    76108 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    43948 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    25232 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    18177 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700italic.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    79742 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700italic.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    34360 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700italic.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    20472 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700italic.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    16639 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    58571 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    29288 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19216 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    15864 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400italic.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    58853 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400italic.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    26644 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400italic.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    18396 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400italic.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    16716 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    57996 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    29704 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19332 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    16849 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700italic.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    58214 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700italic.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    28932 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700italic.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19444 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700italic.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    24132 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    95257 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    42116 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    26804 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    22002 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400italic.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    70885 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400italic.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    38736 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400italic.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    25372 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400italic.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    27033 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    96461 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    47276 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    30532 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    25348 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700italic.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   107048 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700italic.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    44008 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700italic.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    28060 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700italic.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    14004 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_400.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    61056 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_400.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    27916 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_400.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    15640 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_400.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    13750 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_700.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    59518 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_700.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    27696 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_700.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    15340 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_700.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    20290 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/glyphicons-halflings-regular.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    62850 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/glyphicons-halflings-regular.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    41236 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/glyphicons-halflings-regular.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    23292 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.306533 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.314183 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/
+-rwxrwxrwx   0 danil      (501) staff       (20)    30858 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    57401 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    30680 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19788 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    34166 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    60750 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    33960 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    21940 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    30602 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    58215 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    30404 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19972 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    33758 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    61071 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    33532 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    21824 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    34798 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    62096 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    34612 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    22416 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    29794 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    56447 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    29612 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19396 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    34578 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    62430 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    34368 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    22444 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    29934 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    58495 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    29744 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19624 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    30350 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    57560 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    30156 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19736 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    34866 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    62044 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    34644 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    22332 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)     5151 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/open-sans/stylesheet.css
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.315330 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.316983 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/
+-rwxrwxrwx   0 danil      (501) staff       (20)   111902 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   113630 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   112362 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   112866 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   112354 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   113510 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)     4616 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/LICENSE.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.318392 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/
+-rwxrwxrwx   0 danil      (501) staff       (20)    91216 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    92760 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    89720 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    91424 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    91276 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    93144 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)     1081 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/README.md
+-rwxrwxrwx   0 danil      (501) staff       (20)     4402 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/ReadMe.html
+-rwxrwxrwx   0 danil      (501) staff       (20)    11781 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.319903 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/
+-rwxrwxrwx   0 danil      (501) staff       (20)   111572 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   113320 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   112004 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   112528 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   112048 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   113168 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.278950 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.321148 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/
+-rwxrwxrwx   0 danil      (501) staff       (20)    48788 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    51188 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    47136 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    49672 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    48972 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    51272 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.322267 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/
+-rwxrwxrwx   0 danil      (501) staff       (20)    49496 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    51924 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    48784 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    50792 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    49604 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    51772 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)      404 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/bower.json
+-rwxrwxrwx   0 danil      (501) staff       (20)     2429 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/source-serif-pro.css
+-rwxrwxrwx   0 danil      (501) staff       (20)    18299 2023-05-03 17:21:06.000000 verstack-3.8.8/docs/build/html/_static/guzzle.css
+-rwxrwxrwx   0 danil      (501) staff       (20)     1912 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-example.png
+-rwxrwxrwx   0 danil      (501) staff       (20)     1478 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-important.png
+-rwxrwxrwx   0 danil      (501) staff       (20)     1234 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-javascript-example.png
+-rwxrwxrwx   0 danil      (501) staff       (20)     1086 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-json-example.png
+-rwxrwxrwx   0 danil      (501) staff       (20)     1526 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-lconf-example.png
+-rwxrwxrwx   0 danil      (501) staff       (20)     2331 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-note.png
+-rwxrwxrwx   0 danil      (501) staff       (20)      679 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-optional.png
+-rwxrwxrwx   0 danil      (501) staff       (20)      759 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-python-example.png
+-rwxrwxrwx   0 danil      (501) staff       (20)     1701 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-seealso.png
+-rwxrwxrwx   0 danil      (501) staff       (20)     1082 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-shell-example.png
+-rwxrwxrwx   0 danil      (501) staff       (20)     1912 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-text-example.png
+-rwxrwxrwx   0 danil      (501) staff       (20)      587 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-tip.png
+-rwxrwxrwx   0 danil      (501) staff       (20)     2271 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-todo.png
+-rwxrwxrwx   0 danil      (501) staff       (20)     1962 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/icon-warning.png
+-rwxrwxrwx   0 danil      (501) staff       (20)   280364 2020-02-10 16:38:31.000000 verstack-3.8.8/docs/build/html/_static/jquery-3.4.1.js
+-rwxrwxrwx   0 danil      (501) staff       (20)   287630 2020-09-20 11:51:08.000000 verstack-3.8.8/docs/build/html/_static/jquery-3.5.1.js
+-rwxrwxrwx   0 danil      (501) staff       (20)     3510 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/jquery.cookie.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    92634 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/jquery.js
+-rwxrwxrwx   0 danil      (501) staff       (20)   138746 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/jquery.min.map
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.322627 verstack-3.8.8/docs/build/html/_static/js/
+-rwxrwxrwx   0 danil      (501) staff       (20)    55329 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/js/bootstrap.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    29182 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/build/html/_static/js/bootstrap.min.js
+-rwxrwxrwx   0 danil      (501) staff       (20)     4758 2023-05-03 17:21:06.000000 verstack-3.8.8/docs/build/html/_static/language_data.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    14747 2020-09-20 11:42:10.000000 verstack-3.8.8/docs/build/html/_static/local_fonts.css
+-rwxrwxrwx   0 danil      (501) staff       (20)       90 2020-02-10 16:38:31.000000 verstack-3.8.8/docs/build/html/_static/minus.png
+-rwxrwxrwx   0 danil      (501) staff       (20)    27652 2020-09-20 11:45:40.000000 verstack-3.8.8/docs/build/html/_static/p_sphinx_theme.css
+-rwxrwxrwx   0 danil      (501) staff       (20)    17752 2020-09-20 11:45:40.000000 verstack-3.8.8/docs/build/html/_static/p_sphinx_theme.js
+-rwxrwxrwx   0 danil      (501) staff       (20)       90 2020-02-10 16:38:31.000000 verstack-3.8.8/docs/build/html/_static/plus.png
+-rwxrwxrwx   0 danil      (501) staff       (20)     4846 2023-05-03 17:21:06.000000 verstack-3.8.8/docs/build/html/_static/pygments.css
+-rwxrwxrwx   0 danil      (501) staff       (20)    18215 2023-05-03 17:20:59.000000 verstack-3.8.8/docs/build/html/_static/searchtools.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    67692 2021-05-11 23:58:54.000000 verstack-3.8.8/docs/build/html/_static/underscore-1.12.0.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    68420 2021-08-12 13:47:18.000000 verstack-3.8.8/docs/build/html/_static/underscore-1.13.1.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    35168 2020-02-10 16:38:31.000000 verstack-3.8.8/docs/build/html/_static/underscore-1.3.1.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    19358 2021-05-11 23:58:54.000000 verstack-3.8.8/docs/build/html/_static/underscore.js
+-rwxrwxrwx   0 danil      (501) staff       (20)     3388 2023-05-03 17:21:05.000000 verstack-3.8.8/docs/build/html/genindex.html
+-rwxrwxrwx   0 danil      (501) staff       (20)   162215 2023-05-03 17:21:05.000000 verstack-3.8.8/docs/build/html/index.html
+-rwxrwxrwx   0 danil      (501) staff       (20)      254 2023-05-03 17:21:06.000000 verstack-3.8.8/docs/build/html/objects.inv
+-rwxrwxrwx   0 danil      (501) staff       (20)     4500 2023-05-03 17:21:06.000000 verstack-3.8.8/docs/build/html/search.html
+-rwxrwxrwx   0 danil      (501) staff       (20)    16283 2023-05-03 17:21:06.000000 verstack-3.8.8/docs/build/html/searchindex.js
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.322783 verstack-3.8.8/docs/guzzle_sphinx_theme/
+-rwxrwxrwx   0 danil      (501) staff       (20)     4856 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/__init__.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.322930 verstack-3.8.8/docs/guzzle_sphinx_theme/__pycache__/
+-rwxrwxrwx   0 danil      (501) staff       (20)     5478 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/__pycache__/__init__.cpython-37.pyc
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.324665 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/
+-rwxrwxrwx   0 danil      (501) staff       (20)      828 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/comments.html
+-rwxrwxrwx   0 danil      (501) staff       (20)      323 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/globaltoc.html
+-rwxrwxrwx   0 danil      (501) staff       (20)     5778 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/layout.html
+-rwxrwxrwx   0 danil      (501) staff       (20)      206 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/localtoc.html
+-rwxrwxrwx   0 danil      (501) staff       (20)       92 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/logo-text.html
+-rwxrwxrwx   0 danil      (501) staff       (20)     1695 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/search.html
+-rwxrwxrwx   0 danil      (501) staff       (20)      521 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/searchbox.html
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.325246 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.325615 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/
+-rwxrwxrwx   0 danil      (501) staff       (20)    13353 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap-theme.min.css
+-rwxrwxrwx   0 danil      (501) staff       (20)   102105 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap.min.css
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.326379 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/
+-rwxrwxrwx   0 danil      (501) staff       (20)    20290 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    62850 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    41236 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    23292 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.326546 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.333407 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/
+-rwxrwxrwx   0 danil      (501) staff       (20)    30858 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    57401 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    30680 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19788 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    34166 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    60750 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    33960 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    21940 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    30602 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    58215 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    30404 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19972 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    33758 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    61071 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    33532 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    21824 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    34798 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    62096 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    34612 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    22416 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    29794 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    56447 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    29612 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19396 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    34578 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    62430 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    34368 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    22444 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    29934 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    58495 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    29744 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19624 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    30350 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    57560 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    30156 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19736 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    34866 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    62044 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    34644 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    22332 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)     5151 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/stylesheet.css
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.334348 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.335539 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/
+-rwxrwxrwx   0 danil      (501) staff       (20)   111902 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   113630 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   112362 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   112866 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   112354 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   113510 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)     4616 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/LICENSE.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.336707 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/
+-rwxrwxrwx   0 danil      (501) staff       (20)    91216 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    92760 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    89720 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    91424 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    91276 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    93144 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)     1081 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/README.md
+-rwxrwxrwx   0 danil      (501) staff       (20)     4402 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/ReadMe.html
+-rwxrwxrwx   0 danil      (501) staff       (20)    11781 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/SourceSerifProReadMe.html
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.337805 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/
+-rwxrwxrwx   0 danil      (501) staff       (20)   111572 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   113320 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   112004 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   112528 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   112048 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   113168 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.280391 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.338897 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/
+-rwxrwxrwx   0 danil      (501) staff       (20)    48788 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    51188 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    47136 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    49672 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    48972 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    51272 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.340316 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/
+-rwxrwxrwx   0 danil      (501) staff       (20)    49496 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    51924 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    48784 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    50792 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    49604 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    51772 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)      404 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/bower.json
+-rwxrwxrwx   0 danil      (501) staff       (20)     2429 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/source-serif-pro.css
+-rwxrwxrwx   0 danil      (501) staff       (20)    18300 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/guzzle.css_t
+-rwxrwxrwx   0 danil      (501) staff       (20)    92634 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.js
+-rwxrwxrwx   0 danil      (501) staff       (20)   138746 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.min.map
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.340674 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/
+-rwxrwxrwx   0 danil      (501) staff       (20)    55329 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    29182 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.min.js
+-rwxrwxrwx   0 danil      (501) staff       (20)      649 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/theme.conf
+-rwxrwxrwx   0 danil      (501) staff       (20)      799 2020-09-20 09:39:03.000000 verstack-3.8.8/docs/make.bat
+-rwxrwxrwx   0 danil      (501) staff       (20)       57 2023-05-04 06:42:41.000000 verstack-3.8.8/docs/requirements.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.340970 verstack-3.8.8/docs/source/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.280849 verstack-3.8.8/docs/source/_build/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.341857 verstack-3.8.8/docs/source/_build/html/
+-rwxrwxrwx   0 danil      (501) staff       (20)      230 2022-02-10 20:51:20.000000 verstack-3.8.8/docs/source/_build/html/.buildinfo
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.342150 verstack-3.8.8/docs/source/_build/html/.doctrees/
+-rwxrwxrwx   0 danil      (501) staff       (20)    34100 2022-02-10 20:51:19.000000 verstack-3.8.8/docs/source/_build/html/.doctrees/environment.pickle
+-rwxrwxrwx   0 danil      (501) staff       (20)   233769 2022-02-10 20:51:19.000000 verstack-3.8.8/docs/source/_build/html/.doctrees/index.doctree
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.342553 verstack-3.8.8/docs/source/_build/html/_sources/
+-rwxrwxrwx   0 danil      (501) staff       (20)    42285 2022-02-10 20:51:17.000000 verstack-3.8.8/docs/source/_build/html/_sources/index.rst.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.344999 verstack-3.8.8/docs/source/_build/html/_static/
+-rwxrwxrwx   0 danil      (501) staff       (20)    14652 2022-02-10 20:51:20.000000 verstack-3.8.8/docs/source/_build/html/_static/basic.css
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.345301 verstack-3.8.8/docs/source/_build/html/_static/css/
+-rwxrwxrwx   0 danil      (501) staff       (20)    13353 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/css/bootstrap-theme.min.css
+-rwxrwxrwx   0 danil      (501) staff       (20)   102105 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/css/bootstrap.min.css
+-rwxrwxrwx   0 danil      (501) staff       (20)     9592 2021-05-11 23:58:54.000000 verstack-3.8.8/docs/source/_build/html/_static/doctools.js
+-rwxrwxrwx   0 danil      (501) staff       (20)      355 2022-02-10 20:51:20.000000 verstack-3.8.8/docs/source/_build/html/_static/documentation_options.js
+-rwxrwxrwx   0 danil      (501) staff       (20)      286 2021-05-11 23:58:54.000000 verstack-3.8.8/docs/source/_build/html/_static/file.png
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.345945 verstack-3.8.8/docs/source/_build/html/_static/fonts/
+-rwxrwxrwx   0 danil      (501) staff       (20)    20290 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    62850 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    41236 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    23292 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.346099 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.352922 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/
+-rwxrwxrwx   0 danil      (501) staff       (20)    30858 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    57401 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    30680 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19788 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    34166 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    60750 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    33960 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    21940 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    30602 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    58215 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    30404 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19972 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    33758 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    61071 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    33532 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    21824 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    34798 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    62096 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    34612 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    22416 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    29794 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    56447 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    29612 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19396 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    34578 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    62430 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    34368 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    22444 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    29934 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    58495 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    29744 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19624 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    30350 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    57560 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    30156 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    19736 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    34866 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)    62044 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg
+-rwxrwxrwx   0 danil      (501) staff       (20)    34644 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)    22332 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)     5151 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/stylesheet.css
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.353744 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.354839 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/
+-rwxrwxrwx   0 danil      (501) staff       (20)   111902 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   113630 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   112362 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   112866 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   112354 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)   113510 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot
+-rwxrwxrwx   0 danil      (501) staff       (20)     4616 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/LICENSE.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.356284 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/
+-rwxrwxrwx   0 danil      (501) staff       (20)    91216 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    92760 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    89720 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    91424 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    91276 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)    93144 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf
+-rwxrwxrwx   0 danil      (501) staff       (20)     1081 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/README.md
+-rwxrwxrwx   0 danil      (501) staff       (20)     4402 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/ReadMe.html
+-rwxrwxrwx   0 danil      (501) staff       (20)    11781 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.357696 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/
+-rwxrwxrwx   0 danil      (501) staff       (20)   111572 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   113320 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   112004 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   112528 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   112048 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf
+-rwxrwxrwx   0 danil      (501) staff       (20)   113168 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.282539 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.359010 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/
+-rwxrwxrwx   0 danil      (501) staff       (20)    48788 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    51188 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    47136 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    49672 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    48972 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    51272 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.360277 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/
+-rwxrwxrwx   0 danil      (501) staff       (20)    49496 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    51924 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    48784 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    50792 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    49604 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)    51772 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff
+-rwxrwxrwx   0 danil      (501) staff       (20)      404 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/bower.json
+-rwxrwxrwx   0 danil      (501) staff       (20)     2429 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/source-serif-pro.css
+-rwxrwxrwx   0 danil      (501) staff       (20)    18299 2022-02-10 20:51:20.000000 verstack-3.8.8/docs/source/_build/html/_static/guzzle.css
+-rwxrwxrwx   0 danil      (501) staff       (20)   287630 2021-05-11 23:58:54.000000 verstack-3.8.8/docs/source/_build/html/_static/jquery-3.5.1.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    92634 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/jquery.js
+-rwxrwxrwx   0 danil      (501) staff       (20)   138746 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/jquery.min.map
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.360700 verstack-3.8.8/docs/source/_build/html/_static/js/
+-rwxrwxrwx   0 danil      (501) staff       (20)    55329 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/js/bootstrap.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    29182 2020-09-20 11:50:32.000000 verstack-3.8.8/docs/source/_build/html/_static/js/bootstrap.min.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    10854 2022-02-10 20:51:20.000000 verstack-3.8.8/docs/source/_build/html/_static/language_data.js
+-rwxrwxrwx   0 danil      (501) staff       (20)       90 2021-05-11 23:58:54.000000 verstack-3.8.8/docs/source/_build/html/_static/minus.png
+-rwxrwxrwx   0 danil      (501) staff       (20)       90 2021-05-11 23:58:54.000000 verstack-3.8.8/docs/source/_build/html/_static/plus.png
+-rwxrwxrwx   0 danil      (501) staff       (20)     4846 2022-02-10 20:51:20.000000 verstack-3.8.8/docs/source/_build/html/_static/pygments.css
+-rwxrwxrwx   0 danil      (501) staff       (20)    16578 2021-05-11 23:58:54.000000 verstack-3.8.8/docs/source/_build/html/_static/searchtools.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    67692 2021-05-11 23:58:54.000000 verstack-3.8.8/docs/source/_build/html/_static/underscore-1.12.0.js
+-rwxrwxrwx   0 danil      (501) staff       (20)    19358 2021-05-11 23:58:54.000000 verstack-3.8.8/docs/source/_build/html/_static/underscore.js
+-rwxrwxrwx   0 danil      (501) staff       (20)     3419 2022-02-10 20:51:20.000000 verstack-3.8.8/docs/source/_build/html/genindex.html
+-rwxrwxrwx   0 danil      (501) staff       (20)   101829 2022-02-10 20:51:19.000000 verstack-3.8.8/docs/source/_build/html/index.html
+-rwxrwxrwx   0 danil      (501) staff       (20)      254 2022-02-10 20:51:20.000000 verstack-3.8.8/docs/source/_build/html/objects.inv
+-rwxrwxrwx   0 danil      (501) staff       (20)     4531 2022-02-10 20:51:20.000000 verstack-3.8.8/docs/source/_build/html/search.html
+-rwxrwxrwx   0 danil      (501) staff       (20)     6846 2022-02-10 20:51:20.000000 verstack-3.8.8/docs/source/_build/html/searchindex.js
+-rwxrwxrwx   0 danil      (501) staff       (20)     5224 2023-05-03 17:20:38.000000 verstack-3.8.8/docs/source/conf.py
+-rwxrwxrwx   0 danil      (501) staff       (20)    75112 2023-07-04 19:41:11.000000 verstack-3.8.8/docs/source/index.rst
+-rwxrwxrwx   0 danil      (501) staff       (20)      548 2023-02-12 13:52:00.000000 verstack-3.8.8/increment_version.py
+-rwxrwxrwx   0 danil      (501) staff       (20)   253628 2023-02-12 13:48:06.000000 verstack-3.8.8/logo.png
+-rwxrwxrwx   0 danil      (501) staff       (20)   200067 2023-02-12 13:48:04.000000 verstack-3.8.8/logo.pxd
+-rwxrwxrwx   0 danil      (501) staff       (20)     1703 2023-02-12 13:53:15.000000 verstack-3.8.8/package_update_instructions.txt
+-rwxrwxrwx   0 danil      (501) staff       (20)      306 2023-07-04 16:34:54.000000 verstack-3.8.8/requirements.txt
+-rwxrwxrwx   0 danil      (501) staff       (20)       80 2023-07-04 19:43:48.369094 verstack-3.8.8/setup.cfg
+-rwxrwxrwx   0 danil      (501) staff       (20)     2235 2023-07-04 19:43:43.000000 verstack-3.8.8/setup.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.362573 verstack-3.8.8/verstack/
+-rwxrwxrwx   0 danil      (501) staff       (20)    39819 2023-01-16 10:00:49.000000 verstack-3.8.8/verstack/DateParser.py
+-rwxrwxrwx   0 danil      (501) staff       (20)    24790 2023-05-03 13:58:53.000000 verstack-3.8.8/verstack/FeatureSelector.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     7756 2022-04-29 08:46:57.000000 verstack-3.8.8/verstack/Multicore.py
+-rwxrwxrwx   0 danil      (501) staff       (20)    18447 2022-12-09 20:53:43.000000 verstack-3.8.8/verstack/NaNImputer.py
+-rwxrwxrwx   0 danil      (501) staff       (20)    33143 2022-12-09 20:16:44.000000 verstack-3.8.8/verstack/NaNImputerLegacy.py
+-rwxrwxrwx   0 danil      (501) staff       (20)    12408 2022-12-19 10:43:57.000000 verstack-3.8.8/verstack/PandasOptimizer.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     8816 2023-03-28 10:21:12.000000 verstack-3.8.8/verstack/ThreshTuner.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      980 2022-12-19 08:48:26.000000 verstack-3.8.8/verstack/__init__.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.364395 verstack-3.8.8/verstack/categoric_encoders/
+-rwxrwxrwx   0 danil      (501) staff       (20)     5115 2022-04-29 12:08:27.000000 verstack-3.8.8/verstack/categoric_encoders/Factorizer.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     4669 2022-04-28 10:31:19.000000 verstack-3.8.8/verstack/categoric_encoders/FrequencyEncoder.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     7499 2023-01-11 14:23:40.000000 verstack-3.8.8/verstack/categoric_encoders/MeanTargetEncoder.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     6647 2022-04-28 09:22:13.000000 verstack-3.8.8/verstack/categoric_encoders/OneHotEncoder.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     7352 2022-04-28 09:22:53.000000 verstack-3.8.8/verstack/categoric_encoders/WeightOfEvidenceEncoder.py
+-rwxrwxrwx   0 danil      (501) staff       (20)        0 2021-12-07 14:06:33.000000 verstack-3.8.8/verstack/categoric_encoders/__init__.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     2173 2021-12-06 19:04:49.000000 verstack-3.8.8/verstack/categoric_encoders/args_validators.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.365159 verstack-3.8.8/verstack/lgbm_optuna_tuning/
+-rwxrwxrwx   0 danil      (501) staff       (20)    51067 2023-07-04 19:37:44.000000 verstack-3.8.8/verstack/lgbm_optuna_tuning/LGBMTuner.py
+-rwxrwxrwx   0 danil      (501) staff       (20)        0 2021-12-22 20:41:08.000000 verstack-3.8.8/verstack/lgbm_optuna_tuning/__init__.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     1865 2023-06-22 10:27:54.000000 verstack-3.8.8/verstack/lgbm_optuna_tuning/args_validators.py
+-rwxrwxrwx   0 danil      (501) staff       (20)    17393 2023-06-22 10:27:35.000000 verstack-3.8.8/verstack/lgbm_optuna_tuning/lgb_metrics.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      859 2021-12-21 19:02:16.000000 verstack-3.8.8/verstack/lgbm_optuna_tuning/optuna_tools.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.366289 verstack-3.8.8/verstack/stacking/
+-rwxrwxrwx   0 danil      (501) staff       (20)    30222 2022-12-11 11:13:47.000000 verstack-3.8.8/verstack/stacking/Stacker.py
+-rwxrwxrwx   0 danil      (501) staff       (20)        0 2022-04-04 06:15:43.000000 verstack-3.8.8/verstack/stacking/__init__.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     2371 2022-05-04 09:07:10.000000 verstack-3.8.8/verstack/stacking/args_validators.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     3627 2022-04-05 06:23:16.000000 verstack-3.8.8/verstack/stacking/generate_default_layers.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     5546 2023-07-04 17:01:11.000000 verstack-3.8.8/verstack/stacking/kerasModel.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     3033 2022-12-11 11:14:24.000000 verstack-3.8.8/verstack/stacking/load_stacker.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     7657 2022-04-28 09:37:07.000000 verstack-3.8.8/verstack/stacking/optimise_params.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     8946 2023-02-12 14:01:23.000000 verstack-3.8.8/verstack/stratified_continuous_split.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     3523 2022-06-09 19:16:34.000000 verstack-3.8.8/verstack/tools.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.368620 verstack-3.8.8/verstack/unittest/
+-rwxrwxrwx   0 danil      (501) staff       (20)    25047 2023-05-03 13:08:18.000000 verstack-3.8.8/verstack/unittest/boston_train.parquet
+-rwxrwxrwx   0 danil      (501) staff       (20)     2443 2023-01-16 10:07:03.000000 verstack-3.8.8/verstack/unittest/common.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      373 2023-01-16 10:07:50.000000 verstack-3.8.8/verstack/unittest/test_DateParser.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      939 2022-12-06 11:05:04.000000 verstack-3.8.8/verstack/unittest/test_Factorizer.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      984 2022-12-06 11:13:56.000000 verstack-3.8.8/verstack/unittest/test_FrequencyEncoder.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      881 2023-06-12 05:44:26.000000 verstack-3.8.8/verstack/unittest/test_LGBMTuner.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      791 2022-12-06 11:20:55.000000 verstack-3.8.8/verstack/unittest/test_MeanTargetEncoder.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      600 2022-12-06 11:33:00.000000 verstack-3.8.8/verstack/unittest/test_Multicore.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      393 2022-12-06 11:34:15.000000 verstack-3.8.8/verstack/unittest/test_NaNImputer.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      531 2022-12-06 11:35:42.000000 verstack-3.8.8/verstack/unittest/test_OneHotEncoder.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      414 2022-12-19 09:08:24.000000 verstack-3.8.8/verstack/unittest/test_PandasOptimizer.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      336 2022-12-06 11:37:18.000000 verstack-3.8.8/verstack/unittest/test_Printer.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     1726 2022-12-11 12:01:19.000000 verstack-3.8.8/verstack/unittest/test_Stacker.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      710 2022-12-13 07:01:40.000000 verstack-3.8.8/verstack/unittest/test_ThreshTuner.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      863 2022-12-06 14:19:28.000000 verstack-3.8.8/verstack/unittest/test_WeightOfEvidenceEncoder.py
+-rwxrwxrwx   0 danil      (501) staff       (20)      501 2023-05-03 13:08:40.000000 verstack-3.8.8/verstack/unittest/test_stratified_continuous_split.py
+-rwxrwxrwx   0 danil      (501) staff       (20)     1370 2022-12-06 14:58:08.000000 verstack-3.8.8/verstack/unittest/unittesting_manual.txt
+-rwxrwxrwx   0 danil      (501) staff       (20)       21 2023-07-04 19:41:11.000000 verstack-3.8.8/verstack/version.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-07-04 19:43:48.363378 verstack-3.8.8/verstack.egg-info/
+-rwxrwxrwx   0 danil      (501) staff       (20)     3363 2023-07-04 19:43:48.000000 verstack-3.8.8/verstack.egg-info/PKG-INFO
+-rwxrwxrwx   0 danil      (501) staff       (20)    31441 2023-07-04 19:43:48.000000 verstack-3.8.8/verstack.egg-info/SOURCES.txt
+-rwxrwxrwx   0 danil      (501) staff       (20)        1 2023-07-04 19:43:48.000000 verstack-3.8.8/verstack.egg-info/dependency_links.txt
+-rwxrwxrwx   0 danil      (501) staff       (20)      291 2023-07-04 19:43:48.000000 verstack-3.8.8/verstack.egg-info/requires.txt
+-rwxrwxrwx   0 danil      (501) staff       (20)        9 2023-07-04 19:43:48.000000 verstack-3.8.8/verstack.egg-info/top_level.txt
```

### Comparing `verstack-3.8.7/LICENSE.txt` & `verstack-3.8.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/PKG-INFO` & `verstack-3.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: verstack
-Version: 3.8.7
+Version: 3.8.8
 Summary: Machine learning tools to make a Data Scientist's work more efficient
 Home-page: https://github.com/DanilZherebtsov/verstack
-Download-URL: https://github.com/DanilZherebtsov/verstack/archive/refs/tags/3.8.7.tar.gz
+Download-URL: https://github.com/DanilZherebtsov/verstack/archive/refs/tags/3.8.8.tar.gz
 Author: Danil Zherebtsov
 Author-email: danil.com@me.com
 License: MIT
 Keywords: impute,missing,values,stratify,nan,continuous,multiprocessing,concurrent,timer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 .. image:: logo.png
 
-**verstack 3.8.7** is a set of Machine learning tools to make a Data Scientist's work efficient.
+**verstack 3.8.8** is a set of Machine learning tools to make a Data Scientist's work efficient.
 
 The package contains multiple tools for: training & tuning machine learning models, creating ensembles, working with datetime objects, data transformation & wrangling, imputing missing values, concurrency work and many more.
 
 Please refer to the `official documentation <https://verstack.readthedocs.io>`_ for more information.
 
 The project was created by Danil Zherebtsov in 2020.
```

### Comparing `verstack-3.8.7/README.rst` & `verstack-3.8.8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 .. image:: logo.png
 
-**verstack 3.8.7** is a set of Machine learning tools to make a Data Scientist's work efficient.
+**verstack 3.8.8** is a set of Machine learning tools to make a Data Scientist's work efficient.
 
 The package contains multiple tools for: training & tuning machine learning models, creating ensembles, working with datetime objects, data transformation & wrangling, imputing missing values, concurrency work and many more.
 
 Please refer to the `official documentation <https://verstack.readthedocs.io>`_ for more information.
 
 The project was created by Danil Zherebtsov in 2020.
```

### Comparing `verstack-3.8.7/dist/verstack-0.1.0.tar.gz` & `verstack-3.8.8/dist/verstack-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/Doc_update_manual.txt` & `verstack-3.8.8/docs/Doc_update_manual.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/Makefile` & `verstack-3.8.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/doctrees/README.doctree` & `verstack-3.8.8/docs/build/doctrees/README.doctree`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/doctrees/environment.pickle` & `verstack-3.8.8/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/doctrees/index.doctree` & `verstack-3.8.8/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/README.html` & `verstack-3.8.8/docs/build/html/README.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_sources/README.md.txt` & `verstack-3.8.8/docs/build/html/_sources/README.md.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_sources/README.rst.txt` & `verstack-3.8.8/docs/build/html/_sources/README.rst.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_sources/index.rst.txt` & `verstack-3.8.8/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/alabaster.css` & `verstack-3.8.8/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/basic.css` & `verstack-3.8.8/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/css/bootstrap-theme.min.css` & `verstack-3.8.8/docs/build/html/_static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/css/bootstrap.min.css` & `verstack-3.8.8/docs/build/html/_static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/doctools.js` & `verstack-3.8.8/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Droid_Sans_Mono_400.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Droid_Sans_Mono_400.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Droid_Sans_Mono_400.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Droid_Sans_Mono_400.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400italic.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400italic.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400italic.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400italic.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400italic.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400italic.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_400italic.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_400italic.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700italic.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700italic.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700italic.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700italic.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700italic.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700italic.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noticia_Text_700italic.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Noticia_Text_700italic.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400italic.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400italic.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400italic.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400italic.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400italic.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400italic.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_400italic.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_400italic.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700italic.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700italic.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700italic.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700italic.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700italic.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700italic.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Sans_700italic.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Sans_700italic.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400italic.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400italic.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400italic.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400italic.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400italic.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400italic.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_400italic.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_400italic.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700italic.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700italic.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700italic.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700italic.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700italic.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700italic.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Noto_Serif_700italic.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Noto_Serif_700italic.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_400.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_400.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_400.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_400.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_400.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_400.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_400.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_400.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_700.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_700.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_700.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_700.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_700.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_700.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/Source_Code_Pro_700.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/Source_Code_Pro_700.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/open-sans/stylesheet.css` & `verstack-3.8.8/docs/build/html/_static/fonts/open-sans/stylesheet.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/LICENSE.txt` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/README.md` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/README.md`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/ReadMe.html` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/ReadMe.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/fonts/source-serif-pro/source-serif-pro.css` & `verstack-3.8.8/docs/build/html/_static/fonts/source-serif-pro/source-serif-pro.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/guzzle.css` & `verstack-3.8.8/docs/build/html/_static/guzzle.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-example.png` & `verstack-3.8.8/docs/build/html/_static/icon-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-important.png` & `verstack-3.8.8/docs/build/html/_static/icon-important.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-javascript-example.png` & `verstack-3.8.8/docs/build/html/_static/icon-javascript-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-json-example.png` & `verstack-3.8.8/docs/build/html/_static/icon-json-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-lconf-example.png` & `verstack-3.8.8/docs/build/html/_static/icon-lconf-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-note.png` & `verstack-3.8.8/docs/build/html/_static/icon-note.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-optional.png` & `verstack-3.8.8/docs/build/html/_static/icon-optional.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-python-example.png` & `verstack-3.8.8/docs/build/html/_static/icon-python-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-seealso.png` & `verstack-3.8.8/docs/build/html/_static/icon-seealso.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-shell-example.png` & `verstack-3.8.8/docs/build/html/_static/icon-shell-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-text-example.png` & `verstack-3.8.8/docs/build/html/_static/icon-text-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-tip.png` & `verstack-3.8.8/docs/build/html/_static/icon-tip.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-todo.png` & `verstack-3.8.8/docs/build/html/_static/icon-todo.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/icon-warning.png` & `verstack-3.8.8/docs/build/html/_static/icon-warning.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/jquery-3.4.1.js` & `verstack-3.8.8/docs/build/html/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/jquery-3.5.1.js` & `verstack-3.8.8/docs/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/jquery.cookie.js` & `verstack-3.8.8/docs/build/html/_static/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/jquery.js` & `verstack-3.8.8/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/jquery.min.map` & `verstack-3.8.8/docs/build/html/_static/jquery.min.map`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/js/bootstrap.js` & `verstack-3.8.8/docs/build/html/_static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/js/bootstrap.min.js` & `verstack-3.8.8/docs/build/html/_static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/language_data.js` & `verstack-3.8.8/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/local_fonts.css` & `verstack-3.8.8/docs/build/html/_static/local_fonts.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/p_sphinx_theme.css` & `verstack-3.8.8/docs/build/html/_static/p_sphinx_theme.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/p_sphinx_theme.js` & `verstack-3.8.8/docs/build/html/_static/p_sphinx_theme.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/pygments.css` & `verstack-3.8.8/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/searchtools.js` & `verstack-3.8.8/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/underscore-1.12.0.js` & `verstack-3.8.8/docs/build/html/_static/underscore-1.12.0.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/underscore-1.13.1.js` & `verstack-3.8.8/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/underscore-1.3.1.js` & `verstack-3.8.8/docs/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/_static/underscore.js` & `verstack-3.8.8/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/genindex.html` & `verstack-3.8.8/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/index.html` & `verstack-3.8.8/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/search.html` & `verstack-3.8.8/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/build/html/searchindex.js` & `verstack-3.8.8/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/__init__.py` & `verstack-3.8.8/docs/guzzle_sphinx_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/__pycache__/__init__.cpython-37.pyc` & `verstack-3.8.8/docs/guzzle_sphinx_theme/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/comments.html` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/comments.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/layout.html` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/search.html` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/searchbox.html` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap-theme.min.css` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap.min.css` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/stylesheet.css` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/stylesheet.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/LICENSE.txt` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/README.md` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/README.md`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/ReadMe.html` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/ReadMe.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/SourceSerifProReadMe.html` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/SourceSerifProReadMe.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/source-serif-pro.css` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/source-serif-pro.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/guzzle.css_t` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/guzzle.css_t`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.js` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.min.map` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.min.map`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.js` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.min.js` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/theme.conf` & `verstack-3.8.8/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/make.bat` & `verstack-3.8.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/.doctrees/environment.pickle` & `verstack-3.8.8/docs/source/_build/html/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/.doctrees/index.doctree` & `verstack-3.8.8/docs/source/_build/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_sources/index.rst.txt` & `verstack-3.8.8/docs/source/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/basic.css` & `verstack-3.8.8/docs/source/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/css/bootstrap-theme.min.css` & `verstack-3.8.8/docs/source/_build/html/_static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/css/bootstrap.min.css` & `verstack-3.8.8/docs/source/_build/html/_static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/doctools.js` & `verstack-3.8.8/docs/source/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.svg` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/open-sans/stylesheet.css` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/open-sans/stylesheet.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/LICENSE.txt` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/README.md` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/README.md`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/ReadMe.html` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/ReadMe.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/fonts/source-serif-pro/source-serif-pro.css` & `verstack-3.8.8/docs/source/_build/html/_static/fonts/source-serif-pro/source-serif-pro.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/guzzle.css` & `verstack-3.8.8/docs/source/_build/html/_static/guzzle.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/jquery-3.5.1.js` & `verstack-3.8.8/docs/source/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/jquery.js` & `verstack-3.8.8/docs/source/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/jquery.min.map` & `verstack-3.8.8/docs/source/_build/html/_static/jquery.min.map`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/js/bootstrap.js` & `verstack-3.8.8/docs/source/_build/html/_static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/js/bootstrap.min.js` & `verstack-3.8.8/docs/source/_build/html/_static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/language_data.js` & `verstack-3.8.8/docs/source/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/pygments.css` & `verstack-3.8.8/docs/source/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/searchtools.js` & `verstack-3.8.8/docs/source/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/underscore-1.12.0.js` & `verstack-3.8.8/docs/source/_build/html/_static/underscore-1.12.0.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/_static/underscore.js` & `verstack-3.8.8/docs/source/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/genindex.html` & `verstack-3.8.8/docs/source/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/index.html` & `verstack-3.8.8/docs/source/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/search.html` & `verstack-3.8.8/docs/source/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/_build/html/searchindex.js` & `verstack-3.8.8/docs/source/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/conf.py` & `verstack-3.8.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/docs/source/index.rst` & `verstack-3.8.8/docs/source/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ############################
-verstack 3.8.7 Documentation
+verstack 3.8.8 Documentation
 ############################
 Machine learning tools to make a Data Scientist's work efficient
 
 veratack package contains the following tools:
 
 * **PandasOptimizer** oad a pandas.DataFrame with optimized datatypes (reduce RAM usage)
 * **Stacker** automated stacking ensemble configuration/train/features creation in train/test sets
@@ -21,22 +21,51 @@
  * **OneHotEncoder** represent categoric variable as a set of binary variables
  * **FrequencyEncoder** encode categoric variable by class frequencies
  * **MeanTargetEncoder** encode categoric variable by mean of the target variable
  * **WeightOfEvidenceEncoder** encode categoric variable as a weight of evidence of a binary target variable
 * **timer** convenient timer decorator to quickly measure and display time of any function execution
 * **Printer** a convenient function to set up and execute print statements based on the 'global' verbosity setting within large projects
 
+.. note:: **x86 installation**
 
-.. note:: 
+  $ ``pip install verstack``
+
+  $ ``pip install --upgrade verstack``
+
+.. note:: **ARM installation**
 
-  Getting verstack
+  Getting verstack for ARM architecture (M1/M2 macs) requires miniforge python environment, because AMR versions of ``lightgbm`` and ``tensorflow`` are not yet supported by ``pip`` and can only be installed with ``conda``. Below steps outiline installation of the correct miniforge python (3.10.12) environment with subsequent verstack installation.
+  
+  # install miniforge python environment
+  
+  $ ``pyenv install miniforge3-4.14.0-1``
+
+  $ ``pyenv global miniforge3-4.14.0-1``
 
+  # install verstack
+  
   $ ``pip install verstack``
 
-  $ ``pip install --upgrade verstack``
+  # uninstall lightgbm (which came with verstack via pip install lightgbm) which is not compatible with ARM
+  
+  $ ``pip uninstall lightgbm``
+
+  $ ``conda uninstall lightgbm``
+
+  # install lightgbm (from conda index) which is compatible with ARM
+  
+  $ ``conda install lightgbm``
+
+  # in case of tensorflow uncompatibility with ARM
+  
+  $ ``pip uninstall tensorflow``
+
+  $ ``conda uninstall tensorflow``
+
+  $ ``conda install tensorflow``
 
 
 ******************
 PandasOptimizer
 ******************
 
 Automated loader of a pandas.DataFrame with optimized data types. The resulting dataframe memory footprint is on average 20% of the original data footprint.
@@ -898,14 +927,18 @@
 
       Train features
     
     - ``y`` [pd.Series]
       
       Train labels
 
+    - ``optuna_study_params`` [dict, default=None]
+
+      Optuna study parameters. Please refer to the `Optuna docs <https://optuna.readthedocs.io/en/stable/reference/study.html#optuna.study.Study.optimize>`_ for the full list of parameters and their descriptions
+
 * ``fit_optimized(X, y)``
 
   Train model with tuned params on whole train data
 
     - ``X`` [np.array]
 
       Train features
```

### Comparing `verstack-3.8.7/increment_version.py` & `verstack-3.8.8/increment_version.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/logo.png` & `verstack-3.8.8/logo.png`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/logo.pxd` & `verstack-3.8.8/logo.pxd`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/package_update_instructions.txt` & `verstack-3.8.8/package_update_instructions.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/setup.py` & `verstack-3.8.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   license='MIT',
   description = "Machine learning tools to make a Data Scientist's work more efficient",
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Danil Zherebtsov',
   author_email = 'danil.com@me.com',
   url = 'https://github.com/DanilZherebtsov/verstack',
-  download_url = 'https://github.com/DanilZherebtsov/verstack/archive/refs/tags/3.8.7.tar.gz',
+  download_url = 'https://github.com/DanilZherebtsov/verstack/archive/refs/tags/3.8.8.tar.gz',
   keywords = ['impute', 'missing', 'values', 'stratify', 'nan', 'continuous', 'multiprocessing', 'concurrent', 'timer'],
   install_requires=dependencies,
   classifiers=[
   'Development Status :: 4 - Beta',
   'Intended Audience :: Developers',
   'Topic :: Software Development :: Build Tools',
   'License :: OSI Approved :: MIT License',
```

### Comparing `verstack-3.8.7/verstack/DateParser.py` & `verstack-3.8.8/verstack/DateParser.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/FeatureSelector.py` & `verstack-3.8.8/verstack/FeatureSelector.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/Multicore.py` & `verstack-3.8.8/verstack/Multicore.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/NaNImputer.py` & `verstack-3.8.8/verstack/NaNImputer.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/NaNImputerLegacy.py` & `verstack-3.8.8/verstack/NaNImputerLegacy.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/PandasOptimizer.py` & `verstack-3.8.8/verstack/PandasOptimizer.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/ThreshTuner.py` & `verstack-3.8.8/verstack/ThreshTuner.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/__init__.py` & `verstack-3.8.8/verstack/__init__.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/categoric_encoders/Factorizer.py` & `verstack-3.8.8/verstack/categoric_encoders/Factorizer.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/categoric_encoders/FrequencyEncoder.py` & `verstack-3.8.8/verstack/categoric_encoders/FrequencyEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/categoric_encoders/MeanTargetEncoder.py` & `verstack-3.8.8/verstack/categoric_encoders/MeanTargetEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/categoric_encoders/OneHotEncoder.py` & `verstack-3.8.8/verstack/categoric_encoders/OneHotEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/categoric_encoders/WeightOfEvidenceEncoder.py` & `verstack-3.8.8/verstack/categoric_encoders/WeightOfEvidenceEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/categoric_encoders/args_validators.py` & `verstack-3.8.8/verstack/categoric_encoders/args_validators.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/lgbm_optuna_tuning/LGBMTuner.py` & `verstack-3.8.8/verstack/lgbm_optuna_tuning/LGBMTuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     'min_data_in_leaf', 'min_sum_hessian_in_leaf', 'bagging_fraction', 'feature_fraction',
     'max_delta_step', 'lambda_l1', 'lambda_l2', 'linear_lambda', 'min_gain_to_split',
     'drop_rate', 'top_rate', 'min_data_per_group', 'max_cat_threshold'
     ]
 
 class LGBMTuner:
 
-    __version__ = '1.2.0'
+    __version__ = '1.3.0'
 
     def __init__(self, **kwargs):
         '''
         Class to automatically tune LGBM model with optuna.
         
         Model type (regressor/classifier) is inferred based on target variable & metric.
         Init parameters and search space are inferred by built in logic.
@@ -1069,15 +1069,15 @@
                     elif self._all_ints(param_grid.values()):
                         self.search_space[param_name] = SearchSpace(Distribution.INTUNIFORM, low = param_grid['low'], high = param_grid['high'])
         if unsupported_params:
             self.printer.print(f'Following changed parameters are not supported for tuning: {unsupported_params}', order = 'error', trailing_blank_paragraph=True)
         self.grid = {key: value for key, value in self.grid.items() if key not in unsupported_params}
     
     @timer
-    def fit(self, X, y, optuna_params = None):
+    def fit(self, X, y, optuna_study_params = None):
         '''
         Find optimized parameters for LightGBM model based on training data and 
         metric (defined by user at __init__).
         
         Considering the lower-better strategy:
             Regression optimization metric
                 is selected based on eval_metric (passed by user at __init__), except for r2.
@@ -1095,14 +1095,17 @@
         
         Parameters
         ----------
         X : pd.DataFrame
             train features.
         y : pd.Series
             train labels.
+        optuna_study_params : dict, optional
+            Parameters for optuna study. The default is None. Custom optuna.study.create_study parameters
+            https://optuna.readthedocs.io/en/stable/reference/generated/optuna.study.create_study.html
 
         Returns
         -------
         None.
 
         '''
         validate_features_argument(X)
@@ -1122,17 +1125,21 @@
         self._init_params_on_input(len(X), y)
         # update the predefined params with custom params passed by user
         self._init_params.update(self.custom_lgbm_params)
         self._align_grid_and_search_space()
         self._set_optuna_verbosity(self.verbosity)
         
         sampler = optuna.samplers.TPESampler(seed=self.seed)
+        
         optuna_params = {'pruner':optuna.pruners.MedianPruner(n_warmup_steps=5),
                          'sampler':sampler,
                          'direction':'minimize'}
+        # incorporate user defined params if passed
+        if optuna_study_params is not None:
+            optuna_params.update(optuna_study_params)
         study = optuna.create_study(**optuna_params)#get_study_direction(metric))
 
         optimization_function = partial(self._objective, X = X.values, y = y.values)
 
         study.optimize(optimization_function, n_trials = self.trials)
 
         # populate the learned params into the suggested params
```

### Comparing `verstack-3.8.7/verstack/lgbm_optuna_tuning/args_validators.py` & `verstack-3.8.8/verstack/lgbm_optuna_tuning/args_validators.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/lgbm_optuna_tuning/lgb_metrics.py` & `verstack-3.8.8/verstack/lgbm_optuna_tuning/lgb_metrics.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/lgbm_optuna_tuning/optuna_tools.py` & `verstack-3.8.8/verstack/lgbm_optuna_tuning/optuna_tools.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/stacking/Stacker.py` & `verstack-3.8.8/verstack/stacking/Stacker.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/stacking/args_validators.py` & `verstack-3.8.8/verstack/stacking/args_validators.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/stacking/generate_default_layers.py` & `verstack-3.8.8/verstack/stacking/generate_default_layers.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/stacking/kerasModel.py` & `verstack-3.8.8/verstack/stacking/kerasModel.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/stacking/load_stacker.py` & `verstack-3.8.8/verstack/stacking/load_stacker.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/stacking/optimise_params.py` & `verstack-3.8.8/verstack/stacking/optimise_params.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/stratified_continuous_split.py` & `verstack-3.8.8/verstack/stratified_continuous_split.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/tools.py` & `verstack-3.8.8/verstack/tools.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/unittest/boston_train.parquet` & `verstack-3.8.8/verstack/unittest/boston_train.parquet`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/unittest/common.py` & `verstack-3.8.8/verstack/unittest/common.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/unittest/test_Factorizer.py` & `verstack-3.8.8/verstack/unittest/test_Factorizer.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/unittest/test_FrequencyEncoder.py` & `verstack-3.8.8/verstack/unittest/test_FrequencyEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/unittest/test_LGBMTuner.py` & `verstack-3.8.8/verstack/unittest/test_LGBMTuner.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/unittest/test_MeanTargetEncoder.py` & `verstack-3.8.8/verstack/unittest/test_MeanTargetEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/unittest/test_Multicore.py` & `verstack-3.8.8/verstack/unittest/test_Multicore.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/unittest/test_OneHotEncoder.py` & `verstack-3.8.8/verstack/unittest/test_OneHotEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/unittest/test_Stacker.py` & `verstack-3.8.8/verstack/unittest/test_Stacker.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/unittest/test_ThreshTuner.py` & `verstack-3.8.8/verstack/unittest/test_ThreshTuner.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/unittest/test_WeightOfEvidenceEncoder.py` & `verstack-3.8.8/verstack/unittest/test_WeightOfEvidenceEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack/unittest/unittesting_manual.txt` & `verstack-3.8.8/verstack/unittest/unittesting_manual.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.8.7/verstack.egg-info/PKG-INFO` & `verstack-3.8.8/verstack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: verstack
-Version: 3.8.7
+Version: 3.8.8
 Summary: Machine learning tools to make a Data Scientist's work more efficient
 Home-page: https://github.com/DanilZherebtsov/verstack
-Download-URL: https://github.com/DanilZherebtsov/verstack/archive/refs/tags/3.8.7.tar.gz
+Download-URL: https://github.com/DanilZherebtsov/verstack/archive/refs/tags/3.8.8.tar.gz
 Author: Danil Zherebtsov
 Author-email: danil.com@me.com
 License: MIT
 Keywords: impute,missing,values,stratify,nan,continuous,multiprocessing,concurrent,timer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 .. image:: logo.png
 
-**verstack 3.8.7** is a set of Machine learning tools to make a Data Scientist's work efficient.
+**verstack 3.8.8** is a set of Machine learning tools to make a Data Scientist's work efficient.
 
 The package contains multiple tools for: training & tuning machine learning models, creating ensembles, working with datetime objects, data transformation & wrangling, imputing missing values, concurrency work and many more.
 
 Please refer to the `official documentation <https://verstack.readthedocs.io>`_ for more information.
 
 The project was created by Danil Zherebtsov in 2020.
```

### Comparing `verstack-3.8.7/verstack.egg-info/SOURCES.txt` & `verstack-3.8.8/verstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

