# Comparing `tmp/capypdf-0.3.0.tar.gz` & `tmp/capypdf-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capypdf-0.3.0.tar", last modified: Sat Jun 10 18:45:46 2023, max compression
+gzip compressed data, was "capypdf-0.4.0.tar", last modified: Tue Jul  4 17:32:50 2023, max compression
```

## Comparing `capypdf-0.3.0.tar` & `capypdf-0.4.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-rw-rw-   0        0        0      348 1970-01-01 00:00:00.000000 capypdf-0.3.0/.clang-format
--rw-rw-rw-   0        0        0       88 1970-01-01 00:00:00.000000 capypdf-0.3.0/.gitignore
--rw-rw-rw-   0        0        0    11358 1970-01-01 00:00:00.000000 capypdf-0.3.0/COPYING
--rw-rw-rw-   0        0        0      195 1970-01-01 00:00:00.000000 capypdf-0.3.0/compilefuzz.sh
--rw-rw-rw-   0        0        0    10810 1970-01-01 00:00:00.000000 capypdf-0.3.0/images/1bit_alpha.png
--rw-rw-rw-   0        0        0     1650 1970-01-01 00:00:00.000000 capypdf-0.3.0/images/1bit_noalpha.png
--rw-rw-rw-   0        0        0    13448 1970-01-01 00:00:00.000000 capypdf-0.3.0/images/cmyk_tiff.tif
--rw-rw-rw-   0        0        0    38408 1970-01-01 00:00:00.000000 capypdf-0.3.0/images/comic-colors.png
--rw-rw-rw-   0        0        0     3260 1970-01-01 00:00:00.000000 capypdf-0.3.0/images/comic-lines.png
--rw-rw-rw-   0        0        0     3189 1970-01-01 00:00:00.000000 capypdf-0.3.0/images/comic-richblack.png
--rw-rw-rw-   0        0        0   118339 1970-01-01 00:00:00.000000 capypdf-0.3.0/images/flame_gradient.png
--rw-rw-rw-   0        0        0    57042 1970-01-01 00:00:00.000000 capypdf-0.3.0/images/gray_alpha.png
--rw-rw-rw-   0        0        0   267304 1970-01-01 00:00:00.000000 capypdf-0.3.0/images/object_gradient.png
--rw-rw-rw-   0        0        0    28468 1970-01-01 00:00:00.000000 capypdf-0.3.0/images/simple.jpg
--rw-rw-rw-   0        0        0    12147 1970-01-01 00:00:00.000000 capypdf-0.3.0/include/capypdf.h.in
--rw-rw-rw-   0        0        0      167 1970-01-01 00:00:00.000000 capypdf-0.3.0/include/meson.build
--rw-rw-rw-   0        0        0      949 1970-01-01 00:00:00.000000 capypdf-0.3.0/meson.build
--rw-rw-rw-   0        0        0      731 1970-01-01 00:00:00.000000 capypdf-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0    15887 1970-01-01 00:00:00.000000 capypdf-0.3.0/python/capypdf.py
--rw-rw-rw-   0        0        0       67 1970-01-01 00:00:00.000000 capypdf-0.3.0/python/meson.build
--rw-rw-rw-   0        0        0     1296 1970-01-01 00:00:00.000000 capypdf-0.3.0/readme.md
--rw-rw-rw-   0        0        0     8277 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/cover.cpp
--rw-rw-rw-   0        0        0     2508 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/errorhandling.cpp
--rw-rw-rw-   0        0        0     5626 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/errorhandling.hpp
--rw-rw-rw-   0        0        0     2092 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/fembedtest.cpp
--rw-rw-rw-   0        0        0      972 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/fontfuzz.cpp
--rw-rw-rw-   0        0        0     6769 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/fontgen.cpp
--rw-rw-rw-   0        0        0     6179 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/fontsubsetter.cpp
--rw-rw-rw-   0        0        0     2232 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/fontsubsetter.hpp
--rw-rw-rw-   0        0        0     1495 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/fonttester.cpp
--rw-rw-rw-   0        0        0     2512 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/formtest.cpp
--rw-rw-rw-   0        0        0     2189 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/formxobj.cpp
--rw-rw-rw-   0        0        0    32206 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/ft_subsetter.cpp
--rw-rw-rw-   0        0        0     5339 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/ft_subsetter.hpp
--rw-rw-rw-   0        0        0     3297 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/gstategen.cpp
--rw-rw-rw-   0        0        0     1615 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/icctest.cpp
--rw-rw-rw-   0        0        0    12122 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/imageops.cpp
--rw-rw-rw-   0        0        0     1605 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/imageops.hpp
--rw-rw-rw-   0        0        0     4985 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/imagetest.cpp
--rw-rw-rw-   0        0        0     1899 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/labtest.cpp
--rw-rw-rw-   0        0        0    10289 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/loremipsum.cpp
--rw-rw-rw-   0        0        0     2741 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/main.cpp
--rw-rw-rw-   0        0        0     2453 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/meson.build
--rw-rw-rw-   0        0        0     1647 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/outlinetest.cpp
--rw-rw-rw-   0        0        0     3238 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pathgen.cpp
--rw-rw-rw-   0        0        0     3929 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/patterngen.cpp
--rw-rw-rw-   0        0        0    16101 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfcapi.cpp
--rw-rw-rw-   0        0        0     6610 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfcolorconverter.cpp
--rw-rw-rw-   0        0        0     2530 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfcolorconverter.hpp
--rw-rw-rw-   0        0        0     6186 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfcommon.hpp
--rw-rw-rw-   0        0        0    54988 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfdocument.cpp
--rw-rw-rw-   0        0        0    13455 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfdocument.hpp
--rw-rw-rw-   0        0        0    32093 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfdrawcontext.cpp
--rw-rw-rw-   0        0        0     9429 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfdrawcontext.hpp
--rw-rw-rw-   0        0        0     7629 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfgen.cpp
--rw-rw-rw-   0        0        0     5629 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfgen.hpp
--rw-rw-rw-   0        0        0    11242 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfparser.cpp
--rw-rw-rw-   0        0        0     4778 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfparser.hpp
--rw-rw-rw-   0        0        0     4139 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdftext.hpp
--rw-rw-rw-   0        0        0    19213 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/pdfviewer.cpp
--rw-rw-rw-   0        0        0     2338 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/presentation.cpp
--rw-rw-rw-   0        0        0     1587 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/subtype.cpp
--rw-rw-rw-   0        0        0     2996 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/tifftest.cpp
--rw-rw-rw-   0        0        0     7686 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/utils.cpp
--rw-rw-rw-   0        0        0     1284 1970-01-01 00:00:00.000000 capypdf-0.3.0/src/utils.hpp
--rw-rw-rw-   0        0        0       84 1970-01-01 00:00:00.000000 capypdf-0.3.0/subprojects/.gitignore
--rw-rw-rw-   0        0        0      552 1970-01-01 00:00:00.000000 capypdf-0.3.0/subprojects/fmt.wrap
--rw-rw-rw-   0        0        0      334 1970-01-01 00:00:00.000000 capypdf-0.3.0/subprojects/freetype2.wrap
--rw-rw-rw-   0        0        0      406 1970-01-01 00:00:00.000000 capypdf-0.3.0/subprojects/lcms2.wrap
--rw-rw-rw-   0        0        0      678 1970-01-01 00:00:00.000000 capypdf-0.3.0/subprojects/libjpeg-turbo.wrap
--rw-rw-rw-   0        0        0      589 1970-01-01 00:00:00.000000 capypdf-0.3.0/subprojects/libpng.wrap
--rw-rw-rw-   0        0        0      468 1970-01-01 00:00:00.000000 capypdf-0.3.0/subprojects/libtiff.wrap
--rw-rw-rw-   0        0        0      559 1970-01-01 00:00:00.000000 capypdf-0.3.0/subprojects/zlib.wrap
--rw-rw-rw-   0        0        0     9463 1970-01-01 00:00:00.000000 capypdf-0.3.0/test/capypdftests.py
--rw-rw-rw-   0        0        0     1278 1970-01-01 00:00:00.000000 capypdf-0.3.0/test/ctest.c
--rw-rw-rw-   0        0        0      174 1970-01-01 00:00:00.000000 capypdf-0.3.0/test/meson.build
--rw-rw-rw-   0        0        0     3072 1970-01-01 00:00:00.000000 capypdf-0.3.0/testoutput/python_icccolor.png
--rw-rw-rw-   0        0        0    15829 1970-01-01 00:00:00.000000 capypdf-0.3.0/testoutput/python_image.png
--rw-rw-rw-   0        0        0     4941 1970-01-01 00:00:00.000000 capypdf-0.3.0/testoutput/python_path.png
--rw-rw-rw-   0        0        0     4777 1970-01-01 00:00:00.000000 capypdf-0.3.0/testoutput/python_simple.png
--rw-rw-rw-   0        0        0     4072 1970-01-01 00:00:00.000000 capypdf-0.3.0/testoutput/python_text.png
--rw-rw-rw-   0        0        0     3329 1970-01-01 00:00:00.000000 capypdf-0.3.0/testoutput/python_textobj.png
--rw-r--r--   0        0        0    14797 1970-01-01 00:00:00.000000 capypdf-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      348 1970-01-01 00:00:00.000000 capypdf-0.4.0/.clang-format
+-rw-rw-rw-   0        0        0       88 1970-01-01 00:00:00.000000 capypdf-0.4.0/.gitignore
+-rw-rw-rw-   0        0        0    11358 1970-01-01 00:00:00.000000 capypdf-0.4.0/COPYING
+-rw-rw-rw-   0        0        0      195 1970-01-01 00:00:00.000000 capypdf-0.4.0/compilefuzz.sh
+-rw-rw-rw-   0        0        0    10810 1970-01-01 00:00:00.000000 capypdf-0.4.0/images/1bit_alpha.png
+-rw-rw-rw-   0        0        0     1650 1970-01-01 00:00:00.000000 capypdf-0.4.0/images/1bit_noalpha.png
+-rw-rw-rw-   0        0        0    13448 1970-01-01 00:00:00.000000 capypdf-0.4.0/images/cmyk_tiff.tif
+-rw-rw-rw-   0        0        0    38408 1970-01-01 00:00:00.000000 capypdf-0.4.0/images/comic-colors.png
+-rw-rw-rw-   0        0        0     3260 1970-01-01 00:00:00.000000 capypdf-0.4.0/images/comic-lines.png
+-rw-rw-rw-   0        0        0     3189 1970-01-01 00:00:00.000000 capypdf-0.4.0/images/comic-richblack.png
+-rw-rw-rw-   0        0        0   118339 1970-01-01 00:00:00.000000 capypdf-0.4.0/images/flame_gradient.png
+-rw-rw-rw-   0        0        0    57042 1970-01-01 00:00:00.000000 capypdf-0.4.0/images/gray_alpha.png
+-rw-rw-rw-   0        0        0   267304 1970-01-01 00:00:00.000000 capypdf-0.4.0/images/object_gradient.png
+-rw-rw-rw-   0        0        0    28468 1970-01-01 00:00:00.000000 capypdf-0.4.0/images/simple.jpg
+-rw-rw-rw-   0        0        0    16274 1970-01-01 00:00:00.000000 capypdf-0.4.0/include/capypdf.h.in
+-rw-rw-rw-   0        0        0      167 1970-01-01 00:00:00.000000 capypdf-0.4.0/include/meson.build
+-rw-rw-rw-   0        0        0      949 1970-01-01 00:00:00.000000 capypdf-0.4.0/meson.build
+-rw-rw-rw-   0        0        0      731 1970-01-01 00:00:00.000000 capypdf-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0    21475 1970-01-01 00:00:00.000000 capypdf-0.4.0/python/capypdf.py
+-rw-rw-rw-   0        0        0       67 1970-01-01 00:00:00.000000 capypdf-0.4.0/python/meson.build
+-rw-rw-rw-   0        0        0     1298 1970-01-01 00:00:00.000000 capypdf-0.4.0/readme.md
+-rw-rw-rw-   0        0        0     8299 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/cover.cpp
+-rw-rw-rw-   0        0        0     2538 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/errorhandling.cpp
+-rw-rw-rw-   0        0        0     5641 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/errorhandling.hpp
+-rw-rw-rw-   0        0        0     3256 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/fembedtest.cpp
+-rw-rw-rw-   0        0        0      972 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/fontfuzz.cpp
+-rw-rw-rw-   0        0        0     7549 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/fontgen.cpp
+-rw-rw-rw-   0        0        0     6179 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/fontsubsetter.cpp
+-rw-rw-rw-   0        0        0     2232 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/fontsubsetter.hpp
+-rw-rw-rw-   0        0        0     1501 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/fonttester.cpp
+-rw-rw-rw-   0        0        0     2498 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/formtest.cpp
+-rw-rw-rw-   0        0        0     2175 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/formxobj.cpp
+-rw-rw-rw-   0        0        0    32206 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/ft_subsetter.cpp
+-rw-rw-rw-   0        0        0     5339 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/ft_subsetter.hpp
+-rw-rw-rw-   0        0        0     3303 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/gstategen.cpp
+-rw-rw-rw-   0        0        0     1656 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/icctest.cpp
+-rw-rw-rw-   0        0        0    12122 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/imageops.cpp
+-rw-rw-rw-   0        0        0     1605 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/imageops.hpp
+-rw-rw-rw-   0        0        0     4989 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/imagetest.cpp
+-rw-rw-rw-   0        0        0     1921 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/labtest.cpp
+-rw-rw-rw-   0        0        0    10289 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/loremipsum.cpp
+-rw-rw-rw-   0        0        0     2741 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/main.cpp
+-rw-rw-rw-   0        0        0     2453 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/meson.build
+-rw-rw-rw-   0        0        0     1649 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/outlinetest.cpp
+-rw-rw-rw-   0        0        0     3240 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pathgen.cpp
+-rw-rw-rw-   0        0        0     5178 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/patterngen.cpp
+-rw-rw-rw-   0        0        0    23650 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfcapi.cpp
+-rw-rw-rw-   0        0        0     6610 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfcolorconverter.cpp
+-rw-rw-rw-   0        0        0     2530 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfcolorconverter.hpp
+-rw-rw-rw-   0        0        0     8216 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfcommon.hpp
+-rw-rw-rw-   0        0        0    64982 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfdocument.cpp
+-rw-rw-rw-   0        0        0    14308 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfdocument.hpp
+-rw-rw-rw-   0        0        0    34772 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfdrawcontext.cpp
+-rw-rw-rw-   0        0        0     9982 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfdrawcontext.hpp
+-rw-rw-rw-   0        0        0     7696 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfgen.cpp
+-rw-rw-rw-   0        0        0     6047 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfgen.hpp
+-rw-rw-rw-   0        0        0    11242 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfparser.cpp
+-rw-rw-rw-   0        0        0     4778 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfparser.hpp
+-rw-rw-rw-   0        0        0     4553 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdftext.hpp
+-rw-rw-rw-   0        0        0    19213 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/pdfviewer.cpp
+-rw-rw-rw-   0        0        0     4188 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/presentation.cpp
+-rw-rw-rw-   0        0        0     1573 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/subtype.cpp
+-rw-rw-rw-   0        0        0     2996 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/tifftest.cpp
+-rw-rw-rw-   0        0        0     7686 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/utils.cpp
+-rw-rw-rw-   0        0        0     1284 1970-01-01 00:00:00.000000 capypdf-0.4.0/src/utils.hpp
+-rw-rw-rw-   0        0        0       84 1970-01-01 00:00:00.000000 capypdf-0.4.0/subprojects/.gitignore
+-rw-rw-rw-   0        0        0      552 1970-01-01 00:00:00.000000 capypdf-0.4.0/subprojects/fmt.wrap
+-rw-rw-rw-   0        0        0      334 1970-01-01 00:00:00.000000 capypdf-0.4.0/subprojects/freetype2.wrap
+-rw-rw-rw-   0        0        0      406 1970-01-01 00:00:00.000000 capypdf-0.4.0/subprojects/lcms2.wrap
+-rw-rw-rw-   0        0        0      678 1970-01-01 00:00:00.000000 capypdf-0.4.0/subprojects/libjpeg-turbo.wrap
+-rw-rw-rw-   0        0        0      589 1970-01-01 00:00:00.000000 capypdf-0.4.0/subprojects/libpng.wrap
+-rw-rw-rw-   0        0        0      468 1970-01-01 00:00:00.000000 capypdf-0.4.0/subprojects/libtiff.wrap
+-rw-rw-rw-   0        0        0      559 1970-01-01 00:00:00.000000 capypdf-0.4.0/subprojects/zlib.wrap
+-rw-rw-rw-   0        0        0     9587 1970-01-01 00:00:00.000000 capypdf-0.4.0/test/capypdftests.py
+-rw-rw-rw-   0        0        0     1278 1970-01-01 00:00:00.000000 capypdf-0.4.0/test/ctest.c
+-rw-rw-rw-   0        0        0      174 1970-01-01 00:00:00.000000 capypdf-0.4.0/test/meson.build
+-rw-rw-rw-   0        0        0     3072 1970-01-01 00:00:00.000000 capypdf-0.4.0/testoutput/python_icccolor.png
+-rw-rw-rw-   0        0        0    15829 1970-01-01 00:00:00.000000 capypdf-0.4.0/testoutput/python_image.png
+-rw-rw-rw-   0        0        0     4941 1970-01-01 00:00:00.000000 capypdf-0.4.0/testoutput/python_path.png
+-rw-rw-rw-   0        0        0     4777 1970-01-01 00:00:00.000000 capypdf-0.4.0/testoutput/python_simple.png
+-rw-rw-rw-   0        0        0     4072 1970-01-01 00:00:00.000000 capypdf-0.4.0/testoutput/python_text.png
+-rw-rw-rw-   0        0        0     3329 1970-01-01 00:00:00.000000 capypdf-0.4.0/testoutput/python_textobj.png
+-rw-rw-rw-   0        0        0     8328 1970-01-01 00:00:00.000000 capypdf-0.4.0/tools/presentationtool.py
+-rw-r--r--   0        0        0    14799 1970-01-01 00:00:00.000000 capypdf-0.4.0/PKG-INFO
```

### Comparing `capypdf-0.3.0/COPYING` & `capypdf-0.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/images/1bit_alpha.png` & `capypdf-0.4.0/images/1bit_alpha.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/images/1bit_noalpha.png` & `capypdf-0.4.0/images/1bit_noalpha.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/images/cmyk_tiff.tif` & `capypdf-0.4.0/images/cmyk_tiff.tif`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/images/comic-colors.png` & `capypdf-0.4.0/images/comic-colors.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/images/comic-lines.png` & `capypdf-0.4.0/images/comic-lines.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/images/comic-richblack.png` & `capypdf-0.4.0/images/comic-richblack.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/images/flame_gradient.png` & `capypdf-0.4.0/images/flame_gradient.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/images/gray_alpha.png` & `capypdf-0.4.0/images/gray_alpha.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/images/object_gradient.png` & `capypdf-0.4.0/images/object_gradient.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/images/simple.jpg` & `capypdf-0.4.0/images/simple.jpg`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/meson.build` & `capypdf-0.4.0/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project('capypdf', 'cpp', 'c',
-  version: '0.3.0',
+  version: '0.4.0',
   default_options : ['cpp_std=c++23'])
 
 version = meson.project_version()
 varr = version.split('.')
 cdata = configuration_data()
 cdata.set_quoted('CAPYPDF_VERSION_STR', version)
 cdata.set('CAPYPDF_VERSION_MAJOR', varr[0])
```

### Comparing `capypdf-0.3.0/pyproject.toml` & `capypdf-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = 'mesonpy'
 requires = ['meson-python']
 
 [project]
 name = 'capypdf'
-version = '0.3.0'
+version = '0.4.0'
 description = 'A color managed PDF generation library tech preview'
 readme = 'README.md'
 requires-python = '>=3.8'
 license = {file = 'COPYING'}
 authors = [
   {name = 'Jussi Pakkanen', email = 'jpakkane@gmail.com'},
 ]
```

### Comparing `capypdf-0.3.0/python/capypdf.py` & `capypdf-0.4.0/python/capypdf.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,28 +29,41 @@
     Bevel = 2
 
 class Colorspace(Enum):
     DeviceRGB = 0
     DeviceGray = 1
     DeviceCMYK = 2
 
-class PageTransitionType(Enum):
+class TransitionType(Enum):
     Split = 0
     Blinds = 1
     Box = 2
     Wipe = 3
     Dissolve = 4
     Glitter = 5
     R = 6
     Fly = 7
     Push = 8
     Cover = 9
     Uncover = 10
     Fade = 11
 
+class PageBox(Enum):
+    Media = 0
+    Crop = 1
+    Bleed = 2
+    Trim = 3
+    Art = 4
+
+class RenderingIntent(Enum):
+    Relative_Colorimetric = 0
+    ABSOLUTE_Colorimetric = 1
+    Saturation = 2
+    Perceptual = 3
+
 class CapyPDFException(Exception):
     def __init__(*args, **kwargs):
         Exception.__init__(*args, **kwargs)
 
 ec_type = ctypes.c_int32
 enum_type = ctypes.c_int32
 
@@ -59,55 +72,78 @@
 
 class ImageId(ctypes.Structure):
     _fields_ = [('id', ctypes.c_int32)]
 
 class IccColorSpaceId(ctypes.Structure):
     _fields_ = [('id', ctypes.c_int32)]
 
+class OptionalContentGroupId(ctypes.Structure):
+    _fields_ = [('id', ctypes.c_int32)]
+
+
 cfunc_types = (
 
 ('capy_options_new', [ctypes.c_void_p]),
 ('capy_options_destroy', [ctypes.c_void_p]),
 ('capy_options_set_colorspace', [ctypes.c_void_p, enum_type]),
 ('capy_options_set_title', [ctypes.c_void_p, ctypes.c_char_p]),
 ('capy_options_set_author', [ctypes.c_void_p, ctypes.c_char_p]),
-('capy_options_set_mediabox',
-    [ctypes.c_void_p, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
+('capy_options_set_pagebox',
+    [ctypes.c_void_p, enum_type, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
 
 ('capy_generator_new', [ctypes.c_char_p, ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_add_page', [ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_embed_jpg', [ctypes.c_void_p, ctypes.c_char_p, ctypes.c_void_p]),
 ('capy_generator_load_icc_profile', [ctypes.c_void_p, ctypes.c_char_p, ctypes.c_void_p]),
 ('capy_generator_load_font', [ctypes.c_void_p, ctypes.c_char_p, ctypes.c_void_p]),
 ('capy_generator_write', [ctypes.c_void_p]),
+('capy_generator_add_optional_content_group', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_generator_destroy', [ctypes.c_void_p]),
 ('capy_generator_utf8_text_width', [ctypes.c_void_p, ctypes.c_char_p, FontId, ctypes.c_double, ctypes.POINTER(ctypes.c_double)]),
 
 ('capy_page_draw_context_new', [ctypes.c_void_p, ctypes.c_void_p]),
+('capy_dc_add_simple_navigation', [ctypes.c_void_p, ctypes.c_void_p, ctypes.c_int32, ctypes.c_void_p]),
+('capy_dc_cmd_b', [ctypes.c_void_p]),
 ('capy_dc_cmd_B', [ctypes.c_void_p]),
+('capy_dc_cmd_bstar', [ctypes.c_void_p]),
 ('capy_dc_cmd_Bstar', [ctypes.c_void_p]),
+('capy_dc_cmd_BDC_ocg', [ctypes.c_void_p, OptionalContentGroupId]),
 ('capy_dc_cmd_c', [ctypes.c_void_p,
     ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
 ('capy_dc_cmd_cm', [ctypes.c_void_p,
     ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
+('capy_dc_cmd_EMC', [ctypes.c_void_p]),
 ('capy_dc_cmd_f', [ctypes.c_void_p]),
+('capy_dc_cmd_fstar', [ctypes.c_void_p]),
+('capy_dc_cmd_G', [ctypes.c_void_p, ctypes.c_double]),
+('capy_dc_cmd_g', [ctypes.c_void_p, ctypes.c_double]),
 ('capy_dc_cmd_h', [ctypes.c_void_p]),
+('capy_dc_cmd_i', [ctypes.c_void_p, ctypes.c_double]),
 ('capy_dc_cmd_J', [ctypes.c_void_p, enum_type]),
 ('capy_dc_cmd_j', [ctypes.c_void_p, enum_type]),
 ('capy_dc_cmd_k', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
 ('capy_dc_cmd_K', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
 ('capy_dc_cmd_l', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double]),
 ('capy_dc_cmd_m', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double]),
+('capy_dc_cmd_M', [ctypes.c_void_p, ctypes.c_double]),
+('capy_dc_cmd_n', [ctypes.c_void_p]),
 ('capy_dc_cmd_q', [ctypes.c_void_p]),
 ('capy_dc_cmd_Q', [ctypes.c_void_p]),
 ('capy_dc_cmd_RG', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
 ('capy_dc_cmd_rg', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
 ('capy_dc_cmd_re', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
+('capy_dc_cmd_ri', [ctypes.c_void_p, enum_type]),
+('capy_dc_cmd_s', [ctypes.c_void_p]),
 ('capy_dc_cmd_S', [ctypes.c_void_p]),
+('capy_dc_cmd_v', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
 ('capy_dc_cmd_w', [ctypes.c_void_p, ctypes.c_double]),
+('capy_dc_cmd_W', [ctypes.c_void_p]),
+('capy_dc_cmd_Wstar', [ctypes.c_void_p]),
+('capy_dc_cmd_y', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
+
 ('capy_dc_draw_image',
     [ctypes.c_void_p, ImageId]),
 ('capy_dc_render_utf8_text',
     [ctypes.c_void_p, ctypes.c_char_p, FontId, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
 ('capy_dc_render_text_obj',
     [ctypes.c_void_p, ctypes.c_void_p]),
 ('capy_dc_set_icc_stroke', [ctypes.c_void_p, IccColorSpaceId, ctypes.POINTER(ctypes.c_double), ctypes.c_int32]),
@@ -117,17 +153,29 @@
 
 ('capy_text_new', [ctypes.c_void_p]),
 ('capy_text_destroy', [ctypes.c_void_p]),
 ('capy_text_new', [ctypes.c_void_p]),
 ('capy_text_cmd_Tc', [ctypes.c_void_p, ctypes.c_double]),
 ('capy_text_cmd_Td', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double]),
 ('capy_text_cmd_Tf', [ctypes.c_void_p, FontId, ctypes.c_double]),
+('capy_text_cmd_TL', [ctypes.c_void_p, ctypes.c_double]),
+('capy_text_cmd_Tstar', [ctypes.c_void_p]),
+('capy_text_render_utf8_text', [ctypes.c_void_p, ctypes.c_char_p]),
+('capy_text_nonstroke_color', [ctypes.c_void_p, ctypes.c_void_p]),
+
+('capy_color_new', [ctypes.c_void_p]),
+('capy_color_destroy', [ctypes.c_void_p]),
+('capy_color_set_rgb', [ctypes.c_void_p, ctypes.c_double, ctypes.c_double, ctypes.c_double]),
+('capy_color_set_gray', [ctypes.c_void_p, ctypes.c_double]),
+
+('capy_transition_new', [ctypes.c_void_p, enum_type, ctypes.c_double]),
+('capy_transition_destroy', [ctypes.c_void_p]),
 
-('capy_page_transition_new', [ctypes.c_void_p, enum_type, ctypes.c_double]),
-('capy_page_transition_destroy', [ctypes.c_void_p]),
+('capy_optional_content_group_new', [ctypes.c_void_p, ctypes.c_char_p]),
+('capy_optional_content_group_destroy', [ctypes.c_void_p]),
 
 )
 
 if os.name == 'nt':
     libfile_name = 'capypdf-0.dll'
 else:
     libfile_name = 'libcapypdf.so'
@@ -204,16 +252,16 @@
 
     def set_author(self, title):
         if not isinstance(title, str):
             raise CapyPDFException('Author must be an Unicode string.')
         bytes = title.encode('UTF-8')
         check_error(libfile.capy_options_set_author(self, bytes))
 
-    def set_mediabox(self, x, y, w, h):
-        check_error(libfile.capy_options_set_mediabox(self, x, y, w, h))
+    def set_pagebox(self, boxtype, x1, y1, x2, y2):
+        check_error(libfile.capy_options_set_pagebox(self, boxtype.value, x1, y1, x2, y2))
 
 class DrawContext:
     def __init__(self, generator):
         dcptr = ctypes.c_void_p()
         check_error(libfile.capy_page_draw_context_new(generator, ctypes.pointer(dcptr)))
         self._as_parameter_ = dcptr
         self.generator = generator
@@ -229,32 +277,58 @@
             self.generator.add_page(self)
         finally:
             self.generator = None # Not very elegant.
 
     def push_gstate(self):
         return StateContextManager(self)
 
+    def cmd_b(self):
+        check_error(libfile.capy_dc_cmd_b(self))
+
     def cmd_B(self):
         check_error(libfile.capy_dc_cmd_B(self))
 
+    def cmd_bstar(self):
+        check_error(libfile.capy_dc_cmd_bstar(self))
+
     def cmd_Bstar(self):
         check_error(libfile.capy_dc_cmd_Bstar(self))
 
+    def cmd_BDC(self, ocg):
+        if not isinstance(ocg, OptionalContentGroupId):
+            raise CapyPDFException('Argument must be an optional content group ID.')
+        check_error(libfile.capy_dc_cmd_BDC_ocg(self, ocg))
+
     def cmd_c(self, x1, y1, x2, y2, x3, y3):
         check_error(libfile.capy_dc_cmd_c(self, x1, y1, x2, y2, x3, y3))
 
     def cmd_cm(self, m1, m2, m3, m4, m5, m6):
         check_error(libfile.capy_dc_cmd_cm(self, m1, m2, m3, m4, m5, m6))
 
+    def cmd_EMC(self):
+        check_error(libfile.capy_dc_cmd_EMC(self))
+
     def cmd_f(self):
         check_error(libfile.capy_dc_cmd_f(self))
 
+    def cmd_fstar(self):
+        check_error(libfile.capy_dc_cmd_fstar(self))
+
+    def cmd_G(self, gray):
+        check_error(libfile.capy_dc_cmd_G(self, gray))
+
+    def cmd_g(self):
+        check_error(libfile.capy_dc_cmd_g(self, gray))
+
     def cmd_h(self):
         check_error(libfile.capy_dc_cmd_h(self))
 
+    def cmd_i(self, flatness):
+        check_error(libfile.capy_dc_cmd_i(self, flatness))
+
     def cmd_J(self, cap_style):
         check_error(libfile.capy_dc_cmd_J(self, cap_style.value))
 
     def cmd_j(self, join_style):
         check_error(libfile.capy_dc_cmd_j(self, join_style.value))
 
     def cmd_k(self, c, m, y, k):
@@ -262,37 +336,63 @@
 
     def cmd_K(self, c, m, y, k):
         check_error(libfile.capy_dc_cmd_K(self, c, m, y, k))
 
     def cmd_l(self, x, y):
         check_error(libfile.capy_dc_cmd_l(self, x, y))
 
+    def cmd_m(self, x, y):
+        check_error(libfile.capy_dc_cmd_m(self, x, y))
+
+    def cmd_M(self, miterlimit):
+        check_error(libfile.capy_dc_cmd_M(self, miterlimit))
+
+    def cmd_n(self):
+        check_error(libfile.capy_dc_cmd_n(self))
+
     def cmd_q(self):
         check_error(libfile.capy_dc_cmd_q(self))
 
     def cmd_Q(self):
         check_error(libfile.capy_dc_cmd_Q(self))
 
+    def cmd_re(self, x, y, w, h):
+        check_error(libfile.capy_dc_cmd_re(self, x, y, w, h))
+
     def cmd_RG(self, r, g, b):
         check_error(libfile.capy_dc_cmd_RG(self, r, g, b))
 
     def cmd_rg(self, r, g, b):
         check_error(libfile.capy_dc_cmd_rg(self, r, g, b))
 
-    def cmd_m(self, x, y):
-        check_error(libfile.capy_dc_cmd_m(self, x, y))
+    def cmd_ri(self, ri):
+        if not isinstance(ri, RenderingIntent):
+            raise CapyPDFException('Argument must be a RenderingIntent.')
+        check_error(libfile.capy_dc_cmd_ri(self, ri.value))
 
-    def cmd_re(self, x, y, w, h):
-        check_error(libfile.capy_dc_cmd_re(self, x, y, w, h))
+    def cmd_s(self):
+        check_error(libfile.capy_dc_cmd_s(self))
+
+    def cmd_S(self):
+        check_error(libfile.capy_dc_cmd_S(self))
+
+    def cmd_v(self, x2, y2, x3, y3):
+        check_error(libfile.capy_dc_cmd_v(self, x2, y2, x3, y3))
 
     def cmd_w(self, line_width):
         check_error(libfile.capy_dc_cmd_w(self, line_width))
 
-    def cmd_S(self):
-        check_error(libfile.capy_dc_cmd_S(self))
+    def cmd_W(self):
+        check_error(libfile.capy_dc_cmd_W(self))
+
+    def cmd_Wstar(self):
+        check_error(libfile.capy_dc_cmd_Wstar(self))
+
+    def cmd_y(self, x1, y1, x3, y3):
+        check_error(libfile.capy_dc_cmd_y(self, x1, y1, x3, y3))
 
     def set_icc_stroke(self, iccid, values):
         if not isinstance(values, list):
             raise CapyPDFException('Icc color value argument must be an array.')
         num_entries = len(values)
         doublearray = ctypes.c_double * num_entries
         doublevalues = doublearray(*tuple(values))
@@ -319,27 +419,37 @@
 
     def draw_image(self, iid):
         if not isinstance(iid, ImageId):
             raise CapyPDFException('Image id argument is not an image id object.')
         check_error(libfile.capy_dc_draw_image(self, iid))
 
     def set_page_transition(self, tr):
-        if not isinstance(tr, PageTransition):
+        if not isinstance(tr, Transition):
             raise CapyPDFException('Argument is not a transition object.')
         check_error(libfile.capy_dc_set_page_transition(self, tr))
 
     def translate(self, xtran, ytran):
         self.cmd_cm(1.0, 0, 0, 1.0, xtran, ytran)
 
     def scale(self, xscale, yscale):
         self.cmd_cm(xscale, 0, 0, yscale, 0, 0)
 
     def rotate(self, angle):
         self.cmd_cm(math.cos(angle), math.sin(angle), -math.sin(angle), math.cos(angle), 0.0, 0.0)
 
+    def add_simple_navigation(self, ocgs, transition=None):
+        arraytype = len(ocgs)*OptionalContentGroupId
+        arr = arraytype(*tuple(ocgs))
+        if transition is not None and not isinstance(transition, Transition):
+            raise CapyPDFException('Transition argument must be a transition object.')
+        check_error(libfile.capy_dc_add_simple_navigation(self,
+                                                          ctypes.pointer(arr),
+                                                          len(ocgs),
+                                                          transition))
+
 class StateContextManager:
     def __init__(self, ctx):
         self.ctx = ctx
         ctx.cmd_q()
 
     def __enter__(self):
         return self
@@ -405,14 +515,19 @@
         if not isinstance(font, FontId):
             raise CapyPDFException('Argument not a colorspace object.')
         w = ctypes.c_double()
         bytes = text.encode('UTF-8')
         check_error(libfile.capy_generator_utf8_text_width(self, bytes, font, pointsize, ctypes.pointer(w)))
         return w.value
 
+    def add_optional_content_group(self, ocg):
+        ocgid = OptionalContentGroupId()
+        check_error(libfile.capy_generator_add_optional_content_group(self, ocg, ctypes.pointer(ocgid)))
+        return ocgid
+
 class Text:
     def __init__(self):
         self._as_parameter_ = None
         opt = ctypes.c_void_p()
         check_error(libfile.capy_text_new(ctypes.pointer(opt)))
         self._as_parameter_ = opt
 
@@ -422,29 +537,68 @@
 
     def render_text(self, text):
         if not isinstance(text, str):
             raise CapyPDFException('Text must be a Unicode string.')
         bytes = text.encode('UTF-8')
         check_error(libfile.capy_text_render_utf8_text(self, bytes))
 
+    def nonstroke_color(self, color):
+        check_error(libfile.capy_text_nonstroke_color(self, color))
+
     def cmd_Tc(self, spacing):
         check_error(libfile.capy_text_cmd_Tc(self, spacing))
 
     def cmd_Td(self, x, y):
         check_error(libfile.capy_text_cmd_Td(self, x, y))
 
     def cmd_Tf(self, fontid, ptsize):
         if not isinstance(fontid, FontId):
             raise CapyPDFException('Font id is not a font object.')
         check_error(libfile.capy_text_cmd_Tf(self, fontid, ptsize))
 
-class PageTransition:
+    def cmd_TL(self, leading):
+        check_error(libfile.capy_text_cmd_TL(self, leading))
+
+    def cmd_Tstar(self):
+        check_error(libfile.capy_text_cmd_Tstar(self))
+
+class Color:
+    def __init__(self):
+        self._as_parameter_ = None
+        opt = ctypes.c_void_p()
+        check_error(libfile.capy_color_new(ctypes.pointer(opt)))
+        self._as_parameter_ = opt
+
+    def __del__(self):
+        if self._as_parameter_ is not None:
+            check_error(libfile.capy_color_destroy(self))
+
+    def set_rgb(self, r, g, b):
+        check_error(libfile.capy_color_set_rgb(self, r, g, b))
+
+    def set_gray(self, r, g, b):
+        check_error(libfile.capy_color_set_gray(self, r, g, b))
+
+
+class Transition:
     def __init__(self, ttype, duration):
         self._as_parameter_ = None
         opt = ctypes.c_void_p()
-        if not isinstance(ttype, PageTransitionType):
+        if not isinstance(ttype, TransitionType):
             raise CapyPDFException('Argument is not a transition type.')
-        check_error(libfile.capy_page_transition_new(ctypes.pointer(opt), ttype.value, duration))
+        check_error(libfile.capy_transition_new(ctypes.pointer(opt), ttype.value, duration))
+        self._as_parameter_ = opt
+
+    def __del__(self):
+        check_error(libfile.capy_transition_destroy(self))
+
+
+class OptionalContentGroup:
+    def __init__(self, name):
+        self._as_parameter_ = None
+        in_bytes = name.encode('ASCII')
+        opt = ctypes.c_void_p()
+        check_error(libfile.capy_optional_content_group_new(ctypes.pointer(opt), in_bytes))
         self._as_parameter_ = opt
 
     def __del__(self):
-        check_error(libfile.capy_page_transition_destroy(self))
+        check_error(libfile.capy_optional_content_group_destroy(self))
```

### Comparing `capypdf-0.3.0/readme.md` & `capypdf-0.4.0/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# A4PDF
+# CapyPDF
 
 This is a library for generating PDF files. It aims to be very low level.
 It does not have its own document model, it merely exposes PDF primitives
 directly.
 
 ## Features
```

### Comparing `capypdf-0.3.0/src/cover.cpp` & `capypdf-0.4.0/src/cover.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -120,19 +120,20 @@
 }
 
 } // namespace
 
 int main(int, char **) {
     PdfGenerationData opts;
 
-    opts.mediabox.x = opts.mediabox.y = 0;
-    opts.mediabox.w = paper_width;
-    opts.mediabox.h = paper_height;
+    opts.mediabox.x1 = opts.mediabox.y1 = 0;
+    opts.mediabox.x2 = paper_width;
+    opts.mediabox.y2 = paper_height;
 
-    opts.trimbox = PdfBox{margin, margin, paper_width - 2 * margin, paper_height - 2 * margin};
+    opts.trimbox =
+        PdfRectangle{margin, margin, paper_width - 2 * margin, paper_height - 2 * margin};
     opts.title = "Book cover generation experiment with utf-8 (ö).";
     opts.author = "G. R. Aphicdesigner";
     opts.output_colorspace = CAPYPDF_CS_DEVICE_CMYK;
     opts.prof.cmyk_profile_file =
         "/home/jpakkane/Downloads/temp/Adobe ICC Profiles (end-user)/CMYK/UncoatedFOGRA29.icc";
 
     try {
@@ -143,20 +144,20 @@
         {
             auto ctxguard = gen.guarded_page_context();
             auto &ctx = ctxguard.ctx;
             ctx.cmd_w(1.0);
             ctx.set_nonstroke_color(DeviceRGBColor{0.9, 0.9, 0.9});
             ctx.cmd_re(margin - bleed,
                        margin - bleed,
-                       opts.mediabox.w - 2 * (margin - bleed),
-                       opts.mediabox.h - 2 * (margin - bleed));
+                       opts.mediabox.x2 - 2 * (margin - bleed),
+                       opts.mediabox.y2 - 2 * (margin - bleed));
             ctx.cmd_f();
             ctx.set_nonstroke_color(DeviceRGBColor{0.9, 0.2, 0.2});
             ctx.cmd_re(
-                margin, margin, opts.mediabox.w - 2 * (margin), opts.mediabox.h - 2 * (margin));
+                margin, margin, opts.mediabox.x2 - 2 * (margin), opts.mediabox.y2 - 2 * (margin));
             ctx.cmd_f();
             ctx.set_nonstroke_color(DeviceRGBColor{0.2, 0.9, 0.2});
             ctx.cmd_re(paper_width / 2 - spine_w / 2, margin, spine_w, page_h);
             ctx.cmd_f();
             ctx.set_nonstroke_color(DeviceRGBColor{0, 0, 0});
             {
                 auto pop = ctx.push_gstate();
```

### Comparing `capypdf-0.3.0/src/errorhandling.cpp` & `capypdf-0.4.0/src/errorhandling.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 "Annotations (including widgets) can only be used once.",
 "Structures can only be used once.",
 "Operation prohibited by current output intent.",
 "Output color profile not defined.",
 "Output intent identifier missing.",
 "Draw state end mismatch.",
 "URI must be ASCII.",
+"OCG not used on this page.",
 };
 
 // clang-format on
 
 const char *error_text(ErrorCode ec) noexcept {
     const int index = (int32_t)ec;
     if(index < 0 || (std::size_t)index >= error_texts.size()) {
```

### Comparing `capypdf-0.3.0/src/errorhandling.hpp` & `capypdf-0.4.0/src/errorhandling.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     AnnotationReuse,
     StructureReuse,
     BadOperationForIntent,
     OutputProfileMissing,
     MissingIntentIdentifier,
     DrawStateEndMismatch,
     UriNotAscii,
+    UnusedOcg,
     // When you add an error code here, also add the string representation in the .cpp file.
     NumErrors,
 };
 
 const char *error_text(ErrorCode ec) noexcept;
 
 [[noreturn]] void printandabort(ErrorCode ec) noexcept;
```

### Comparing `capypdf-0.3.0/src/fembedtest.cpp` & `capypdf-0.4.0/src/fonttester.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright 2023 Jussi Pakkanen
+ * Copyright 2022 Jussi Pakkanen
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     http://www.apache.org/licenses/LICENSE-2.0
  *
@@ -11,48 +11,47 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #include <pdfgen.hpp>
+
+#include <vector>
+#include <string>
+#include <variant>
+
+#include <cassert>
+#include <cstdint>
+#include <cstdio>
 #include <cmath>
-#include <span>
 
 using namespace capypdf;
 
 int main(int argc, char **argv) {
-    PdfGenerationData opts;
-
-    opts.mediabox.w = opts.mediabox.h = 200;
-    opts.title = "File embedding test";
-    opts.author = "Test Person";
-    {
-        GenPopper genpop("fembed_test.pdf", opts);
-        PdfGen &gen = *genpop.g;
-        auto efid = gen.embed_file("embed.txt").value();
-        auto fileannoid =
-            gen.create_annotation(PdfRectangle{35, 95, 45, 105}, FileAttachmentAnnotation{efid})
-                .value();
-        {
-            auto ctxguard = gen.guarded_page_context();
-            auto &ctx = ctxguard.ctx;
-
-            ctx.render_pdfdoc_text_builtin(
-                "<- an embedded file.", CAPY_FONT_HELVETICA, 12, 50, 100);
-            ctx.annotate(fileannoid);
-            auto textannoid = gen.create_annotation(PdfRectangle{150, 60, 180, 90},
-                                                    TextAnnotation{"This is a text annotation"})
-                                  .value();
-            ctx.annotate(textannoid);
-            ctx.cmd_rg(0, 0, 1);
-            ctx.render_pdfdoc_text_builtin("Link", CAPY_FONT_HELVETICA, 12, 10, 10);
-            auto linkannoid =
-                gen.create_annotation(PdfRectangle{10, 10, 32, 20},
-                                      UriAnnotation{"https://github.com/mesonbuild/meson"})
-                    .value();
-            ctx.annotate(linkannoid);
-        }
+    const char *fontfile;
+    const char *text;
+    if(argc > 1) {
+        fontfile = argv[1];
+    } else {
+        fontfile = "/usr/share/fonts/truetype/noto/NotoSans-Regular.ttf";
+    }
+    if(argc > 2) {
+        text = argv[2];
+    } else {
+        text = "MiW.";
     }
 
+    PdfGenerationData opts;
+    opts.mediabox = PdfRectangle{0, 0, 200, 30};
+    GenPopper genpop("fonttester.pdf", opts);
+    PdfGen &gen = *genpop.g;
+
+    auto ctxguard = gen.guarded_page_context();
+    auto &ctx = ctxguard.ctx;
+
+    auto textfont = gen.load_font(fontfile).value();
+    if(ctx.render_utf8_text(text, textfont, 12, 10, 10) != ErrorCode::NoError) {
+        printf("FAIL.\n");
+    }
     return 0;
 }
```

### Comparing `capypdf-0.3.0/src/fontfuzz.cpp` & `capypdf-0.4.0/src/fontfuzz.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/fontsubsetter.cpp` & `capypdf-0.4.0/src/fontsubsetter.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/fontsubsetter.hpp` & `capypdf-0.4.0/src/fontsubsetter.hpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/fonttester.cpp` & `capypdf-0.4.0/src/icctest.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright 2022 Jussi Pakkanen
+ * Copyright 2023 Jussi Pakkanen
  *
  * Licensed under the Apache License, Version 2.0 (the "License");
  * you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at
  *
  *     http://www.apache.org/licenses/LICENSE-2.0
  *
@@ -11,47 +11,38 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #include <pdfgen.hpp>
-
-#include <vector>
-#include <string>
-#include <variant>
-
-#include <cassert>
-#include <cstdint>
-#include <cstdio>
 #include <cmath>
 
 using namespace capypdf;
 
 int main(int argc, char **argv) {
-    const char *fontfile;
-    const char *text;
-    if(argc > 1) {
-        fontfile = argv[1];
-    } else {
-        fontfile = "/usr/share/fonts/truetype/noto/NotoSans-Regular.ttf";
-    }
-    if(argc > 2) {
-        text = argv[2];
-    } else {
-        text = "MiW.";
-    }
-
     PdfGenerationData opts;
-    opts.mediabox = PdfBox{0, 0, 200, 30};
-    GenPopper genpop("fonttester.pdf", opts);
-    PdfGen &gen = *genpop.g;
-
-    auto ctxguard = gen.guarded_page_context();
-    auto &ctx = ctxguard.ctx;
-
-    auto textfont = gen.load_font(fontfile).value();
-    if(ctx.render_utf8_text(text, textfont, 12, 10, 10) != ErrorCode::NoError) {
-        printf("FAIL.\n");
+
+    std::filesystem::path icc_file{argc == 1 ? "/usr/share/color/icc/colord/AdobeRGB1998.icc"
+                                             : argv[2]};
+    opts.mediabox.x2 = opts.mediabox.y2 = 200;
+    opts.title = "ICC test";
+    opts.author = "Test Person";
+    opts.output_colorspace = CAPYPDF_CS_DEVICE_RGB;
+    {
+        GenPopper genpop("icc_test.pdf", opts);
+        PdfGen &gen = *genpop.g;
+        auto ctxguard = gen.guarded_page_context();
+        auto &ctx = ctxguard.ctx;
+        auto icc_id = gen.load_icc_file(icc_file).value();
+
+        const std::array<double, 3> blueish{0.1, 0.2, 0.9};
+        const std::vector<double> reddish{0.8, 0.3, 0.1};
+        ctx.set_stroke_color(icc_id, blueish.data(), (int32_t)blueish.size());
+        ctx.set_nonstroke_color(icc_id, reddish.data(), (int32_t)reddish.size());
+
+        ctx.cmd_w(5);
+        ctx.cmd_re(40, 40, 120, 120);
+        ctx.cmd_B();
     }
     return 0;
 }
```

### Comparing `capypdf-0.3.0/src/formtest.cpp` & `capypdf-0.4.0/src/formtest.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,28 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #include <pdfgen.hpp>
 #include <cmath>
-#include <span>
 
 using namespace capypdf;
 
 int main(int argc, char **argv) {
     PdfGenerationData opts;
 
-    opts.mediabox.w = opts.mediabox.h = 200;
+    opts.mediabox.x2 = opts.mediabox.y2 = 200;
     opts.title = "Form XObject test";
     opts.author = "Test Person";
     opts.output_colorspace = CAPYPDF_CS_DEVICE_RGB;
     {
         GenPopper genpop("form_test.pdf", opts);
         PdfGen &gen = *genpop.g;
-        CapyPdF_FormXObjectId offstate, onstate;
+        CapyPDF_FormXObjectId offstate, onstate;
         {
             PdfDrawContext xobj = gen.new_form_xobject(10, 10);
             xobj.cmd_BMC("/Tx");
             xobj.cmd_EMC();
             auto rv = gen.add_form_xobject(xobj);
             if(!rv) {
                 fprintf(stderr, "%s\n", error_text(rv.error()));
```

### Comparing `capypdf-0.3.0/src/formxobj.cpp` & `capypdf-0.4.0/src/formxobj.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,28 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #include <pdfgen.hpp>
 #include <cmath>
-#include <span>
 
 using namespace capypdf;
 
 int main(int argc, char **argv) {
     PdfGenerationData opts;
 
-    opts.mediabox.w = opts.mediabox.h = 200;
+    opts.mediabox.x2 = opts.mediabox.y2 = 200;
     opts.title = "Acroform  test";
     opts.author = "Test Person";
     opts.output_colorspace = CAPYPDF_CS_DEVICE_RGB;
     {
         GenPopper genpop("foxbj_test.pdf", opts);
         PdfGen &gen = *genpop.g;
-        CapyPdF_FormXObjectId xid;
+        CapyPDF_FormXObjectId xid;
         {
             PdfDrawContext xobj = gen.new_form_xobject(10, 10);
             xobj.cmd_w(1);
             xobj.cmd_re(0, 0, 10, 10);
             xobj.cmd_S();
             xobj.cmd_w(2);
             xobj.cmd_m(2, 2);
```

### Comparing `capypdf-0.3.0/src/ft_subsetter.cpp` & `capypdf-0.4.0/src/ft_subsetter.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/ft_subsetter.hpp` & `capypdf-0.4.0/src/ft_subsetter.hpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/gstategen.cpp` & `capypdf-0.4.0/src/gstategen.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -40,28 +40,28 @@
 int main(int argc, char **argv) {
     if(argc != 3) {
         printf("%s <bg file> <fg file>\n", argv[0]);
         return 1;
     }
     PdfGenerationData opts;
     opts.output_colorspace = CAPYPDF_CS_DEVICE_RGB;
-    opts.mediabox.x = opts.mediabox.y = 0;
-    opts.mediabox.w = 300;
-    opts.mediabox.h = 300;
+    opts.mediabox.x1 = opts.mediabox.y1 = 0;
+    opts.mediabox.x2 = 300;
+    opts.mediabox.y2 = 300;
     GenPopper genpop("gstate.pdf", opts);
     PdfGen &gen = *genpop.g;
     auto ctxguard = gen.guarded_page_context();
     auto &ctx = ctxguard.ctx;
     GraphicsState gs;
     gs.blend_mode = CAPY_BM_MULTIPLY;
     gs.intent = CAPY_RI_PERCEPTUAL;
     auto bg_img = gen.load_image(argv[1]).value();
     auto fg_img = gen.load_image(argv[2]).value();
     ctx.cmd_q();
-    ctx.scale(opts.mediabox.w, opts.mediabox.h);
+    ctx.scale(opts.mediabox.x2, opts.mediabox.y2);
     ctx.draw_image(bg_img);
     ctx.cmd_Q();
     // There are 16 blend modes.
     const int imsize = 40;
     CAPYPDF_Blend_Mode bm = CAPY_BM_NORMAL;
     for(int j = 3; j >= 0; --j) {
         for(int i = 0; i < 4; ++i) {
```

### Comparing `capypdf-0.3.0/src/icctest.cpp` & `capypdf-0.4.0/src/subtype.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -11,37 +11,38 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #include <pdfgen.hpp>
+#include <errorhandling.hpp>
 #include <cmath>
-#include <span>
+
 using namespace capypdf;
 
 int main(int argc, char **argv) {
     PdfGenerationData opts;
 
-    const char *icc_file = argc == 1 ? "/usr/share/color/icc/colord/AdobeRGB1998.icc" : argv[2];
-    opts.mediabox.w = opts.mediabox.h = 200;
-    opts.title = "ICC test";
+    opts.mediabox.x2 = opts.mediabox.y2 = 200;
+    opts.title = "Form XObject test";
     opts.author = "Test Person";
     opts.output_colorspace = CAPYPDF_CS_DEVICE_RGB;
+    opts.subtype = IntentSubtype::SUBTYPE_PDFA;
+    opts.intent_condition_identifier = "sRGB IEC61966-2.1";
+    opts.prof.rgb_profile_file = "/usr/share/color/icc/ghostscript/srgb.icc";
     {
-        GenPopper genpop("icc_test.pdf", opts);
+        GenPopper genpop("apdf_test.pdf", opts);
         PdfGen &gen = *genpop.g;
-        auto ctxguard = gen.guarded_page_context();
-        auto &ctx = ctxguard.ctx;
-        auto icc_id = gen.load_icc_file(icc_file).value();
-
-        const std::array<double, 3> blueish{0.1, 0.2, 0.9};
-        const std::vector<double> reddish{0.8, 0.3, 0.1};
-        ctx.set_stroke_color(icc_id, blueish.data(), (int32_t)blueish.size());
-        ctx.set_nonstroke_color(icc_id, reddish.data(), (int32_t)reddish.size());
-
-        ctx.cmd_w(5);
-        ctx.cmd_re(40, 40, 120, 120);
-        ctx.cmd_B();
+
+        {
+            auto ctxguard = gen.guarded_page_context();
+            auto &ctx = ctxguard.ctx;
+
+            auto font =
+                gen.load_font("/usr/share/fonts/truetype/liberation/LiberationSans-Regular.ttf")
+                    .value();
+            ctx.render_utf8_text("This is a PDF/A-3 document.", font, 12, 20, 94);
+        }
     }
     return 0;
 }
```

### Comparing `capypdf-0.3.0/src/imageops.cpp` & `capypdf-0.4.0/src/imageops.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/imageops.hpp` & `capypdf-0.4.0/src/imageops.hpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/imagetest.cpp` & `capypdf-0.4.0/src/imagetest.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     std::filesystem::path datadir = argc > 1 ? argv[1] : "../pdfgen/images";
     std::filesystem::path jpg = datadir / "simple.jpg";
     std::filesystem::path png_1bit_noalpha = datadir / "1bit_noalpha.png";
     std::filesystem::path png_1bit_alpha = datadir / "1bit_alpha.png";
     std::filesystem::path png_gray{datadir / "gray_alpha.png"};
     std::filesystem::path cmyk_tif{datadir / "cmyk_tiff.tif"};
-    opts.mediabox.w = opts.mediabox.h = 200;
+    opts.mediabox.x2 = opts.mediabox.y2 = 200;
     opts.title = "PDF image test";
     opts.author = "Test Person";
     opts.output_colorspace = CAPYPDF_CS_DEVICE_RGB;
     {
         GenPopper genpop("image_test.pdf", opts);
         PdfGen &gen = *genpop.g;
         auto ctxguard = gen.guarded_page_context();
@@ -78,15 +78,15 @@
     std::filesystem::path datadir = argc > 1 ? argv[1] : "../pdfgen/images";
     const char *icc_out =
         "/home/jpakkane/Downloads/temp/Adobe ICC Profiles (end-user)/CMYK/UncoatedFOGRA29.icc";
     PdfGenerationData opts;
     std::filesystem::path lines = datadir / "comic-lines.png";
     std::filesystem::path richblack = datadir / "comic-richblack.png";
     std::filesystem::path colors = datadir / "comic-colors.png";
-    opts.mediabox.w = opts.mediabox.h = 200;
+    opts.mediabox.x2 = opts.mediabox.y2 = 200;
     opts.title = "PDF image masking test";
     opts.author = "Test Person";
     opts.output_colorspace = CAPYPDF_CS_DEVICE_CMYK;
     opts.prof.cmyk_profile_file = icc_out;
     {
         GenPopper genpop("imagemask_test.pdf", opts);
         PdfGen &gen = *genpop.g;
```

### Comparing `capypdf-0.3.0/src/labtest.cpp` & `capypdf-0.4.0/src/labtest.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #include <cmath>
 
 using namespace capypdf;
 
 int main(int, char **) {
     PdfGenerationData opts;
 
-    opts.mediabox.w = opts.mediabox.h = 200;
+    opts.mediabox.x2 = opts.mediabox.y2 = 200;
     opts.title = "L*a*b* test";
     opts.author = "Test Person";
     opts.output_colorspace = CAPYPDF_CS_DEVICE_RGB;
     {
         GenPopper genpop("lab_test.pdf", opts);
         PdfGen &gen = *genpop.g;
         auto ctxguard = gen.guarded_page_context();
@@ -38,18 +38,19 @@
         const double radius = 40;
         const double num_balls = 16;
         double max_ab = 127;
         for(int i = 0; i < num_balls; ++i) {
             auto pop = ctx.push_gstate();
             LabColor lc;
             const double angle = 2 * M_PI * i / num_balls;
+            lc.id = labid;
             lc.l = 50;
             lc.a = max_ab * cos(angle);
             lc.b = max_ab * sin(angle);
-            ctx.set_nonstroke_color(labid, lc);
+            ctx.set_nonstroke_color(lc);
             ctx.translate(cos(angle) * radius, sin(angle) * radius);
             ctx.translate(50, 50);
             ctx.scale(ball_size, ball_size);
             ctx.draw_unit_circle();
             ctx.cmd_f();
         }
     }
```

### Comparing `capypdf-0.3.0/src/loremipsum.cpp` & `capypdf-0.4.0/src/loremipsum.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         if(rc != ErrorCode::NoError) {                                                             \
             std::abort();                                                                          \
         }                                                                                          \
     }
 
 namespace {
 
-CapyPdF_StructureItemId document_root;
+CapyPDF_StructureItemId document_root;
 
 // #define YOLO
 
 #ifdef YOLO
 const std::vector<std::string> column1{
     "Lorem ipsum dolor sit amet, consectetur",
 };
@@ -127,15 +127,15 @@
 
 double cm2pt(double cm) { return cm * 28.346; }
 // double pt2cm(double pt) { return pt / 28.346; }
 
 int num_spaces(const std::string_view s) { return std::count(s.begin(), s.end(), ' '); }
 
 double
-text_width(const std::string_view s, capypdf::PdfGen &gen, CapyPdF_FontId fid, double pointsize) {
+text_width(const std::string_view s, capypdf::PdfGen &gen, CapyPDF_FontId fid, double pointsize) {
     double total_w = 0;
     for(const char c : s) {
         // ASCII FTW!
         const auto w = *gen.glyph_advance(fid, pointsize, c);
         total_w += w;
     }
     return total_w;
@@ -146,15 +146,15 @@
 } // namespace
 
 using namespace capypdf;
 
 void render_column(const std::vector<std::string> &text_lines,
                    PdfGen &gen,
                    PdfDrawContext &ctx,
-                   CapyPdF_FontId textfont,
+                   CapyPDF_FontId textfont,
                    double textsize,
                    double leading,
                    double column_left,
                    double column_top) {
     const double target_width = cm2pt(8);
     auto textobj = PdfText();
     CHCK(textobj.cmd_Tf(textfont, textsize));
```

### Comparing `capypdf-0.3.0/src/main.cpp` & `capypdf-0.4.0/src/main.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/meson.build` & `capypdf-0.4.0/src/meson.build`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/outlinetest.cpp` & `capypdf-0.4.0/src/outlinetest.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #include <cmath>
 
 using namespace capypdf;
 
 int main(int, char **) {
     PdfGenerationData opts;
 
-    opts.mediabox.w = opts.mediabox.h = 200;
+    opts.mediabox.x2 = opts.mediabox.y2 = 200;
     opts.title = "Outline test";
     opts.author = "Test Person";
     opts.output_colorspace = CAPYPDF_CS_DEVICE_RGB;
     {
         GenPopper genpop("outline_test.pdf", opts);
         PdfGen &gen = *genpop.g;
         std::unique_ptr<PdfDrawContext> g{gen.new_page_draw_context()};
```

### Comparing `capypdf-0.3.0/src/pathgen.cpp` & `capypdf-0.4.0/src/pathgen.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         ctx.set_nonstroke_color(DeviceRGBColor{0, 1, 0});
         ctx.set_stroke_color(DeviceRGBColor{0.5, 0.1, 0.5});
         draw_intersect_shape(ctx);
         ctx.cmd_Bstar();
     }
 }
 
-void clipping(PdfDrawContext &ctx, CapyPdF_ImageId image) {
+void clipping(PdfDrawContext &ctx, CapyPDF_ImageId image) {
     ctx.cmd_w(0.1);
     {
         auto pop = ctx.push_gstate();
 
         draw_intersect_shape(ctx);
         ctx.cmd_Wstar();
         ctx.cmd_n();
@@ -91,15 +91,15 @@
     }
 }
 
 int main(int argc, char **argv) {
     PdfGenerationData opts;
 
     const char *image = argc > 1 ? argv[1] : "../pdfgen/images/flame_gradient.png";
-    opts.mediabox.w = opts.mediabox.h = 200;
+    opts.mediabox.x2 = opts.mediabox.y2 = 200;
     opts.title = "PDF path test";
     opts.author = "Test Person";
     opts.output_colorspace = CAPYPDF_CS_DEVICE_RGB;
     {
         GenPopper genpop("path_test.pdf", opts);
         PdfGen &gen = *genpop.g;
         auto ctxp = gen.guarded_page_context();
```

### Comparing `capypdf-0.3.0/src/pdfcapi.cpp` & `capypdf-0.4.0/src/pdfcapi.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -18,387 +18,580 @@
 #include <cstring>
 #include <pdfgen.hpp>
 #include <pdfdrawcontext.hpp>
 #include <errorhandling.hpp>
 
 using namespace capypdf;
 
-CAPYPDF_EC capy_options_new(CapyPdF_Options **out_ptr) CAPYPDF_NOEXCEPT {
-    *out_ptr = reinterpret_cast<CapyPdF_Options *>(new PdfGenerationData());
+CAPYPDF_EC capy_options_new(CapyPDF_Options **out_ptr) CAPYPDF_NOEXCEPT {
+    *out_ptr = reinterpret_cast<CapyPDF_Options *>(new PdfGenerationData());
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_EC capy_options_destroy(CapyPdF_Options *opt) CAPYPDF_NOEXCEPT {
+CAPYPDF_EC capy_options_destroy(CapyPDF_Options *opt) CAPYPDF_NOEXCEPT {
     delete reinterpret_cast<PdfGenerationData *>(opt);
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_EC capy_options_set_title(CapyPdF_Options *opt, const char *utf8_title) CAPYPDF_NOEXCEPT {
+CAPYPDF_EC capy_options_set_title(CapyPDF_Options *opt, const char *utf8_title) CAPYPDF_NOEXCEPT {
     reinterpret_cast<PdfGenerationData *>(opt)->title = utf8_title;
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_options_set_author(CapyPdF_Options *opt,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_options_set_author(CapyPDF_Options *opt,
                                                   const char *utf8_author) CAPYPDF_NOEXCEPT {
     reinterpret_cast<PdfGenerationData *>(opt)->author = utf8_author;
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_options_set_mediabox(
-    CapyPdF_Options *opt, double x, double y, double w, double h) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC capy_options_set_pagebox(CapyPDF_Options *opt,
+                                                   CAPYPDF_Page_Box boxtype,
+                                                   double x1,
+                                                   double y1,
+                                                   double x2,
+                                                   double y2) CAPYPDF_NOEXCEPT {
     auto opts = reinterpret_cast<PdfGenerationData *>(opt);
-    opts->mediabox.x = x;
-    opts->mediabox.y = y;
-    opts->mediabox.w = w;
-    opts->mediabox.h = h;
+    switch(boxtype) {
+    case CAPY_BOX_MEDIA:
+        opts->mediabox.x1 = x1;
+        opts->mediabox.y1 = y1;
+        opts->mediabox.x2 = x2;
+        opts->mediabox.y2 = y2;
+        break;
+    case CAPY_BOX_CROP:
+        opts->cropbox = PdfRectangle{x1, y1, x2, y2};
+        break;
+    case CAPY_BOX_BLEED:
+        opts->bleedbox = PdfRectangle{x1, y1, x2, y2};
+        break;
+    case CAPY_BOX_TRIM:
+        opts->trimbox = PdfRectangle{x1, y1, x2, y2};
+        break;
+    case CAPY_BOX_ART:
+        opts->artbox = PdfRectangle{x1, y1, x2, y2};
+        break;
+    default:
+        return (CAPYPDF_EC)ErrorCode::BadEnum;
+    }
+
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_options_set_colorspace(CapyPdF_Options *opt,
-                                                      enum CapyPdF_Colorspace cs) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC capy_options_set_colorspace(CapyPDF_Options *opt,
+                                                      enum CapyPDF_Colorspace cs) CAPYPDF_NOEXCEPT {
     auto opts = reinterpret_cast<PdfGenerationData *>(opt);
     opts->output_colorspace = cs;
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
 CAPYPDF_EC capy_generator_new(const char *filename,
-                              const CapyPdF_Options *options,
-                              CapyPdF_Generator **out_ptr) CAPYPDF_NOEXCEPT {
+                              const CapyPDF_Options *options,
+                              CapyPDF_Generator **out_ptr) CAPYPDF_NOEXCEPT {
     CHECK_NULL(filename);
     CHECK_NULL(options);
     CHECK_NULL(out_ptr);
     auto opts = reinterpret_cast<const PdfGenerationData *>(options);
     auto genconstruct = PdfGen::construct(filename, *opts);
     if(!genconstruct) {
         return (CAPYPDF_EC)genconstruct.error();
     }
-    *out_ptr = reinterpret_cast<CapyPdF_Generator *>(genconstruct.value().release());
+    *out_ptr = reinterpret_cast<CapyPDF_Generator *>(genconstruct.value().release());
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_EC capy_generator_add_page(CapyPdF_Generator *g,
-                                   CapyPdF_DrawContext *dctx) CAPYPDF_NOEXCEPT {
+CAPYPDF_EC capy_generator_add_page(CapyPDF_Generator *g,
+                                   CapyPDF_DrawContext *dctx) CAPYPDF_NOEXCEPT {
     auto *gen = reinterpret_cast<PdfGen *>(g);
     auto *ctx = reinterpret_cast<PdfDrawContext *>(dctx);
 
     auto rc = gen->add_page(*ctx);
     if(rc) {
         return (CAPYPDF_EC)ErrorCode::NoError;
     }
     return (CAPYPDF_EC)rc.error();
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_generator_embed_jpg(CapyPdF_Generator *g,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_generator_embed_jpg(CapyPDF_Generator *g,
                                                    const char *fname,
-                                                   CapyPdF_ImageId *iid) CAPYPDF_NOEXCEPT {
+                                                   CapyPDF_ImageId *iid) CAPYPDF_NOEXCEPT {
     auto *gen = reinterpret_cast<PdfGen *>(g);
     auto res = gen->embed_jpg(fname);
     if(res) {
         *iid = res.value();
         return (CAPYPDF_EC)ErrorCode::NoError;
     }
     return (CAPYPDF_EC)res.error();
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_generator_load_font(CapyPdF_Generator *g,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_generator_load_font(CapyPDF_Generator *g,
                                                    const char *fname,
-                                                   CapyPdF_FontId *fid) CAPYPDF_NOEXCEPT {
+                                                   CapyPDF_FontId *fid) CAPYPDF_NOEXCEPT {
     auto *gen = reinterpret_cast<PdfGen *>(g);
     auto rc = gen->load_font(fname);
     if(rc) {
         *fid = rc.value();
         return (CAPYPDF_EC)ErrorCode::NoError;
     }
     return (CAPYPDF_EC)rc.error();
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_generator_load_image(CapyPdF_Generator *g,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_generator_load_image(CapyPDF_Generator *g,
                                                     const char *fname,
-                                                    CapyPdF_ImageId *iid) CAPYPDF_NOEXCEPT {
+                                                    CapyPDF_ImageId *iid) CAPYPDF_NOEXCEPT {
     auto *gen = reinterpret_cast<PdfGen *>(g);
     auto load_result = gen->load_image(fname);
     if(load_result) {
         *iid = load_result.value();
         return (CAPYPDF_EC)ErrorCode::NoError;
     }
     return (CAPYPDF_EC)load_result.error();
 }
 
 CAPYPDF_PUBLIC CAPYPDF_EC capy_generator_load_icc_profile(
-    CapyPdF_Generator *g, const char *fname, CapyPdF_IccColorSpaceId *iid) CAPYPDF_NOEXCEPT {
+    CapyPDF_Generator *g, const char *fname, CapyPDF_IccColorSpaceId *iid) CAPYPDF_NOEXCEPT {
     auto *gen = reinterpret_cast<PdfGen *>(g);
     auto res = gen->load_icc_file(fname);
     if(res) {
         *iid = res.value();
         return (CAPYPDF_EC)ErrorCode::NoError;
     }
     return (CAPYPDF_EC)res.error();
 }
 
-CAPYPDF_EC capy_generator_write(CapyPdF_Generator *generator) CAPYPDF_NOEXCEPT {
+CAPYPDF_EC capy_generator_write(CapyPDF_Generator *generator) CAPYPDF_NOEXCEPT {
     auto *g = reinterpret_cast<PdfGen *>(generator);
     auto rc = g->write();
     if(rc) {
         return (CAPYPDF_EC)ErrorCode::NoError;
     }
     return (CAPYPDF_EC)rc.error();
 }
 
-CAPYPDF_EC capy_generator_destroy(CapyPdF_Generator *generator) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC
+capy_generator_add_optional_content_group(CapyPDF_Generator *generator,
+                                          const CapyPDF_OptionalContentGroup *ocg,
+                                          CapyPDF_OptionalContentGroupId *ocgid) CAPYPDF_NOEXCEPT {
+    auto *g = reinterpret_cast<PdfGen *>(generator);
+    const auto *group = reinterpret_cast<const OptionalContentGroup *>(ocg);
+    auto rc = g->add_optional_content_group(*group);
+    if(rc) {
+        *ocgid = rc.value();
+        return (CAPYPDF_EC)ErrorCode::NoError;
+    }
+    return (CAPYPDF_EC)rc.error();
+}
+
+CAPYPDF_EC capy_generator_destroy(CapyPDF_Generator *generator) CAPYPDF_NOEXCEPT {
     auto *g = reinterpret_cast<PdfGen *>(generator);
     delete g;
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_generator_utf8_text_width(CapyPdF_Generator *generator,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_generator_utf8_text_width(CapyPDF_Generator *generator,
                                                          const char *utf8_text,
-                                                         CapyPdF_FontId font,
+                                                         CapyPDF_FontId font,
                                                          double pointsize,
                                                          double *width) CAPYPDF_NOEXCEPT {
     auto *g = reinterpret_cast<PdfGen *>(generator);
     auto rc = g->utf8_text_width(utf8_text, font, pointsize);
     if(rc) {
         *width = rc.value();
         return (CAPYPDF_EC)ErrorCode::NoError;
     }
     return (CAPYPDF_EC)rc.error();
 }
 
 // Draw Context
 
-CAPYPDF_EC capy_page_draw_context_new(CapyPdF_Generator *g,
-                                      CapyPdF_DrawContext **out_ptr) CAPYPDF_NOEXCEPT {
+CAPYPDF_EC capy_page_draw_context_new(CapyPDF_Generator *g,
+                                      CapyPDF_DrawContext **out_ptr) CAPYPDF_NOEXCEPT {
     auto *gen = reinterpret_cast<PdfGen *>(g);
-    *out_ptr = reinterpret_cast<CapyPdF_DrawContext *>(gen->new_page_draw_context());
+    *out_ptr = reinterpret_cast<CapyPDF_DrawContext *>(gen->new_page_draw_context());
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_B(CapyPdF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_b(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_b();
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_B(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_B();
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_Bstar(CapyPdF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_bstar(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_bstar();
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_Bstar(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_Bstar();
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_c(CapyPdF_DrawContext *ctx,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_BDC_ocg(
+    CapyPDF_DrawContext *ctx, CapyPDF_OptionalContentGroupId ocgid) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_BDC(ocgid);
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_c(CapyPDF_DrawContext *ctx,
                                         double x1,
                                         double y1,
                                         double x2,
                                         double y2,
                                         double x3,
                                         double y3) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_c(x1, y1, x2, y2, x3, y3);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_cm(CapyPdF_DrawContext *ctx,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_cm(CapyPDF_DrawContext *ctx,
                                          double m1,
                                          double m2,
                                          double m3,
                                          double m4,
                                          double m5,
                                          double m6) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_cm(m1, m2, m3, m4, m5, m6);
 }
 
-CAPYPDF_EC capy_dc_cmd_f(CapyPdF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_EMC(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_EMC();
+}
+
+CAPYPDF_EC capy_dc_cmd_f(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_f();
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_S(CapyPdF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+CAPYPDF_EC capy_dc_cmd_fstar(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    return (CAPYPDF_EC)c->cmd_S();
+    return (CAPYPDF_EC)c->cmd_fstar();
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_G(CapyPDF_DrawContext *ctx, double gray) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_G(gray);
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_g(CapyPDF_DrawContext *ctx, double gray) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_g(gray);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_h(CapyPdF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_h(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_h();
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_j(CapyPdF_DrawContext *ctx,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_i(CapyPDF_DrawContext *ctx,
+                                        double flatness) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_i(flatness);
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_j(CapyPDF_DrawContext *ctx,
                                         CAPYPDF_Line_Join join_style) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_j(join_style);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_J(CapyPdF_DrawContext *ctx,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_J(CapyPDF_DrawContext *ctx,
                                         CAPYPDF_Line_Cap cap_style) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_J(cap_style);
 }
 
 CAPYPDF_PUBLIC CAPYPDF_EC
-capy_dc_cmd_k(CapyPdF_DrawContext *ctx, double c, double m, double y, double k) CAPYPDF_NOEXCEPT {
+capy_dc_cmd_k(CapyPDF_DrawContext *ctx, double c, double m, double y, double k) CAPYPDF_NOEXCEPT {
     auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)dc->cmd_k(c, m, y, k);
 }
 
 CAPYPDF_PUBLIC CAPYPDF_EC
-capy_dc_cmd_K(CapyPdF_DrawContext *ctx, double c, double m, double y, double k) CAPYPDF_NOEXCEPT {
+capy_dc_cmd_K(CapyPDF_DrawContext *ctx, double c, double m, double y, double k) CAPYPDF_NOEXCEPT {
     auto dc = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)dc->cmd_K(c, m, y, k);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_l(CapyPdF_DrawContext *ctx,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_l(CapyPDF_DrawContext *ctx,
                                         double x,
                                         double y) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_l(x, y);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_m(CapyPdF_DrawContext *ctx,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_m(CapyPDF_DrawContext *ctx,
                                         double x,
                                         double y) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_m(x, y);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_q(CapyPdF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_M(CapyPDF_DrawContext *ctx,
+                                        double miterlimit) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_M(miterlimit);
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_n(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_n();
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_q(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_q();
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_Q(CapyPdF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_Q(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_Q();
 }
 
 CAPYPDF_EC
-capy_dc_cmd_re(CapyPdF_DrawContext *ctx, double x, double y, double w, double h) CAPYPDF_NOEXCEPT {
+capy_dc_cmd_re(CapyPDF_DrawContext *ctx, double x, double y, double w, double h) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_re(x, y, w, h);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_w(CapyPdF_DrawContext *ctx,
+CAPYPDF_EC
+capy_dc_cmd_RG(CapyPDF_DrawContext *ctx, double r, double g, double b) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    DeviceRGBColor rgb{r, g, b};
+    c->set_stroke_color(rgb);
+    return (CAPYPDF_EC)ErrorCode::NoError;
+}
+
+CAPYPDF_EC
+capy_dc_cmd_rg(CapyPDF_DrawContext *ctx, double r, double g, double b) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    DeviceRGBColor rgb{r, g, b};
+    c->set_nonstroke_color(rgb);
+    return (CAPYPDF_EC)ErrorCode::NoError;
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_ri(CapyPDF_DrawContext *ctx,
+                                         CapyPDF_Rendering_Intent ri) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_ri(ri);
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_s(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_s();
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_S(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_S();
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_v(
+    CapyPDF_DrawContext *ctx, double x2, double y2, double x3, double y3) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_v(x2, y2, x3, y3);
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_w(CapyPDF_DrawContext *ctx,
                                         double line_width) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->cmd_w(line_width);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_set_icc_stroke(CapyPdF_DrawContext *ctx,
-                                                 CapyPdF_IccColorSpaceId icc_id,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_W(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_W();
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_Wstar(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_Wstar();
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_cmd_y(
+    CapyPDF_DrawContext *ctx, double x1, double y1, double x3, double y3) CAPYPDF_NOEXCEPT {
+    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
+    return (CAPYPDF_EC)c->cmd_y(x1, y1, x3, y3);
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_set_icc_stroke(CapyPDF_DrawContext *ctx,
+                                                 CapyPDF_IccColorSpaceId icc_id,
                                                  double *values,
                                                  int32_t num_values) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->set_stroke_color(icc_id, values, num_values);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_set_icc_nonstroke(CapyPdF_DrawContext *ctx,
-                                                    CapyPdF_IccColorSpaceId icc_id,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_set_icc_nonstroke(CapyPDF_DrawContext *ctx,
+                                                    CapyPDF_IccColorSpaceId icc_id,
                                                     double *values,
                                                     int32_t num_values) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->set_nonstroke_color(icc_id, values, num_values);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_draw_image(CapyPdF_DrawContext *ctx,
-                                             CapyPdF_ImageId iid) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_draw_image(CapyPDF_DrawContext *ctx,
+                                             CapyPDF_ImageId iid) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)c->draw_image(iid);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_render_utf8_text(CapyPdF_DrawContext *ctx,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_render_utf8_text(CapyPDF_DrawContext *ctx,
                                                    const char *text,
-                                                   CapyPdF_FontId fid,
+                                                   CapyPDF_FontId fid,
                                                    double point_size,
                                                    double x,
                                                    double y) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     c->render_utf8_text(text, fid, point_size, x, y);
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_EC
-capy_dc_cmd_RG(CapyPdF_DrawContext *ctx, double r, double g, double b) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    DeviceRGBColor rgb{r, g, b};
-    c->set_stroke_color(rgb);
-    return (CAPYPDF_EC)ErrorCode::NoError;
-}
-
-CAPYPDF_EC
-capy_dc_cmd_rg(CapyPdF_DrawContext *ctx, double r, double g, double b) CAPYPDF_NOEXCEPT {
-    auto c = reinterpret_cast<PdfDrawContext *>(ctx);
-    DeviceRGBColor rgb{r, g, b};
-    c->set_nonstroke_color(rgb);
-    return (CAPYPDF_EC)ErrorCode::NoError;
-}
-
-CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_render_text_obj(CapyPdF_DrawContext *ctx,
-                                                  CapyPdF_Text *text) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_render_text_obj(CapyPDF_DrawContext *ctx,
+                                                  CapyPDF_Text *text) CAPYPDF_NOEXCEPT {
     auto c = reinterpret_cast<PdfDrawContext *>(ctx);
     auto t = reinterpret_cast<PdfText *>(text);
     return (CAPYPDF_EC)c->render_text(*t);
 }
 
 CAPYPDF_PUBLIC CAPYPDF_EC capy_dc_set_page_transition(
-    CapyPdF_DrawContext *dc, CAPYPDF_PageTransition *transition) CAPYPDF_NOEXCEPT {
+    CapyPDF_DrawContext *dc, CapyPDF_Transition *transition) CAPYPDF_NOEXCEPT {
     auto ctx = reinterpret_cast<PdfDrawContext *>(dc);
-    auto t = reinterpret_cast<PageTransition *>(transition);
+    auto t = reinterpret_cast<Transition *>(transition);
     auto rc = ctx->set_transition(*t);
     return (CAPYPDF_EC)(rc ? ErrorCode::NoError : rc.error());
 }
 
-CAPYPDF_EC capy_dc_destroy(CapyPdF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC
+capy_dc_add_simple_navigation(CapyPDF_DrawContext *dc,
+                              const CapyPDF_OptionalContentGroupId *ocgarray,
+                              int32_t array_size,
+                              const CapyPDF_Transition *tr) CAPYPDF_NOEXCEPT {
+    auto ctx = reinterpret_cast<PdfDrawContext *>(dc);
+    std::optional<Transition> transition;
+    if(tr) {
+        transition = *reinterpret_cast<const Transition *>(tr);
+    }
+    std::span<const CapyPDF_OptionalContentGroupId> ocgspan(ocgarray, ocgarray + array_size);
+    auto rc = ctx->add_simple_navigation(ocgspan, transition);
+    if(rc) {
+        return (CAPYPDF_EC)ErrorCode::NoError;
+    }
+    return (CAPYPDF_EC)rc.error();
+}
+
+CAPYPDF_EC capy_dc_destroy(CapyPDF_DrawContext *ctx) CAPYPDF_NOEXCEPT {
     delete reinterpret_cast<PdfDrawContext *>(ctx);
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_text_new(CapyPdF_Text **out_ptr) CAPYPDF_NOEXCEPT {
-    *out_ptr = reinterpret_cast<CapyPdF_Text *>(new capypdf::PdfText());
+CAPYPDF_PUBLIC CAPYPDF_EC capy_text_new(CapyPDF_Text **out_ptr) CAPYPDF_NOEXCEPT {
+    *out_ptr = reinterpret_cast<CapyPDF_Text *>(new capypdf::PdfText());
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_text_render_utf8_text(CapyPdF_Text *text,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_text_render_utf8_text(CapyPDF_Text *text,
                                                      const char *utf8_text) CAPYPDF_NOEXCEPT {
     auto *t = reinterpret_cast<PdfText *>(text);
     return (CAPYPDF_EC)t->render_text(std::string_view(utf8_text, strlen(utf8_text)));
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_text_cmd_Tc(CapyPdF_Text *text, double spacing) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC capy_text_nonstroke_color(CapyPDF_Text *text,
+                                                    const CapyPDF_Color *color) CAPYPDF_NOEXCEPT {
+    auto *t = reinterpret_cast<PdfText *>(text);
+    const auto *c = reinterpret_cast<const Color *>(color);
+    return (CAPYPDF_EC)t->nonstroke_color(*c);
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_text_cmd_Tc(CapyPDF_Text *text, double spacing) CAPYPDF_NOEXCEPT {
     auto *t = reinterpret_cast<PdfText *>(text);
     return (CAPYPDF_EC)t->cmd_Tc(spacing);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_text_cmd_Td(CapyPdF_Text *text,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_text_cmd_Td(CapyPDF_Text *text,
                                            double x,
                                            double y) CAPYPDF_NOEXCEPT {
     auto *t = reinterpret_cast<PdfText *>(text);
     return (CAPYPDF_EC)t->cmd_Td(x, y);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_text_cmd_Tf(CapyPdF_Text *text,
-                                           CapyPdF_FontId font,
+CAPYPDF_PUBLIC CAPYPDF_EC capy_text_cmd_Tf(CapyPDF_Text *text,
+                                           CapyPDF_FontId font,
                                            double pointsize) CAPYPDF_NOEXCEPT {
     auto *t = reinterpret_cast<PdfText *>(text);
     return (CAPYPDF_EC)t->cmd_Tf(font, pointsize);
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_text_destroy(CapyPdF_Text *text) CAPYPDF_NOEXCEPT {
+CAPYPDF_PUBLIC CAPYPDF_EC capy_text_cmd_TL(CapyPDF_Text *text, double leading) CAPYPDF_NOEXCEPT {
+    auto *t = reinterpret_cast<PdfText *>(text);
+    return (CAPYPDF_EC)t->cmd_TL(leading);
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_text_cmd_Tstar(CapyPDF_Text *text) CAPYPDF_NOEXCEPT {
+    auto *t = reinterpret_cast<PdfText *>(text);
+    return (CAPYPDF_EC)t->cmd_Tstar();
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_text_destroy(CapyPDF_Text *text) CAPYPDF_NOEXCEPT {
     delete reinterpret_cast<PdfText *>(text);
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_page_transition_new(CAPYPDF_PageTransition **out_ptr,
-                                                   CAPYPDF_Transition_Type type,
-                                                   double duration) CAPYPDF_NOEXCEPT {
-    auto pt = new PageTransition{};
+CAPYPDF_PUBLIC CAPYPDF_EC capy_color_new(CapyPDF_Color **out_ptr) CAPYPDF_NOEXCEPT {
+    *out_ptr = reinterpret_cast<CapyPDF_Color *>(new capypdf::Color(DeviceRGBColor{0, 0, 0}));
+    return (CAPYPDF_EC)ErrorCode::NoError;
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_color_destroy(CapyPDF_Color *color) CAPYPDF_NOEXCEPT {
+    delete reinterpret_cast<capypdf::Color *>(color);
+    return (CAPYPDF_EC)ErrorCode::NoError;
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_color_set_rgb(CapyPDF_Color *c, double r, double g, double b)
+    CAPYPDF_NOEXCEPT {
+    *reinterpret_cast<capypdf::Color *>(c) = DeviceRGBColor{r, g, b};
+    return (CAPYPDF_EC)ErrorCode::NoError;
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_color_set_gray(CapyPDF_Color *c, double v) CAPYPDF_NOEXCEPT {
+    *reinterpret_cast<capypdf::Color *>(c) = DeviceGrayColor{v};
+    return (CAPYPDF_EC)ErrorCode::NoError;
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_transition_new(CapyPDF_Transition **out_ptr,
+                                              CAPYPDF_Transition_Type type,
+                                              double duration) CAPYPDF_NOEXCEPT {
+    auto pt = new Transition{};
     pt->type = type;
     pt->duration = duration;
-    *out_ptr = reinterpret_cast<CAPYPDF_PageTransition *>(pt);
+    *out_ptr = reinterpret_cast<CapyPDF_Transition *>(pt);
+    return (CAPYPDF_EC)ErrorCode::NoError;
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_transition_destroy(CapyPDF_Transition *transition) CAPYPDF_NOEXCEPT {
+    delete reinterpret_cast<Transition *>(transition);
+    return (CAPYPDF_EC)ErrorCode::NoError;
+}
+
+CAPYPDF_PUBLIC CAPYPDF_EC capy_optional_content_group_new(CapyPDF_OptionalContentGroup **out_ptr,
+                                                          const char *name) CAPYPDF_NOEXCEPT {
+    // FIXME check for ASCIIness (or even more strict?)
+    auto *ocg = new OptionalContentGroup();
+    ocg->name = name;
+    *out_ptr = reinterpret_cast<CapyPDF_OptionalContentGroup *>(ocg);
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
-CAPYPDF_PUBLIC CAPYPDF_EC capy_page_transition_destroy(CAPYPDF_PageTransition *transition)
+CAPYPDF_PUBLIC CAPYPDF_EC capy_optional_content_group_destroy(CapyPDF_OptionalContentGroup *ocg)
     CAPYPDF_NOEXCEPT {
-    delete reinterpret_cast<PageTransition *>(transition);
+    delete reinterpret_cast<OptionalContentGroup *>(ocg);
     return (CAPYPDF_EC)ErrorCode::NoError;
 }
 
 const char *capy_error_message(CAPYPDF_EC error_code) CAPYPDF_NOEXCEPT {
     return error_text((ErrorCode)error_code);
 }
```

### Comparing `capypdf-0.3.0/src/pdfcolorconverter.cpp` & `capypdf-0.4.0/src/pdfcolorconverter.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/pdfcolorconverter.hpp` & `capypdf-0.4.0/src/pdfcolorconverter.hpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/pdfdocument.cpp` & `capypdf-0.4.0/src/pdfdocument.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #include <pdfdocument.hpp>
 #include <utils.hpp>
 #include <pdfdrawcontext.hpp>
 
 #include <cassert>
 #include <array>
 #include <map>
+#include <bit>
 #include <filesystem>
 #include <algorithm>
 #include <fmt/core.h>
 #include <ft2build.h>
 #include FT_FREETYPE_H
 #include FT_FONT_FORMATS_H
 #include FT_OPENTYPE_VALIDATE_H
@@ -54,26 +55,31 @@
     // Freetype segfaults if you give it a null pointer.
     if(face) {
         return FT_Done_Face(face);
     }
     return 0;
 }
 
-const char PDF_header[] = "%PDF-1.7\n\xe5\xf6\xc4\xd6\n";
+const char PDF_header[] = "%PDF-1.7\n%\xe5\xf6\xc4\xd6\n";
 
-const std::array<const char *, 9> font_names{
+const std::array<const char *, 14> font_names{
     "Times-Roman",
     "Helvetica",
     "Courier",
+    "Symbol",
     "Times-Roman-Bold",
     "Helvetica-Bold",
     "Courier-Bold",
+    "ZapfDingbats",
     "Times-Italic",
     "Helvetica-Oblique",
     "Courier-Oblique",
+    "Times-BoldItalic",
+    "Helvetica-BoldOblique",
+    "Courier-BoldOblique",
 };
 
 const std::array<const char *, 16> blend_mode_names{
     "Normal",
     "Multiply",
     "Screen",
     "Overlay",
@@ -93,16 +99,16 @@
 
 const std::array<const char *, 3> colorspace_names{
     "/DeviceRGB",
     "/DeviceGray",
     "/DeviceCMYK",
 };
 
-void write_box(auto &appender, const char *boxname, const capypdf::PdfBox &box) {
-    fmt::format_to(appender, "  /{} [ {} {} {} {} ]\n", boxname, box.x, box.y, box.w, box.h);
+void write_rectangle(auto &appender, const char *boxname, const capypdf::PdfRectangle &box) {
+    fmt::format_to(appender, "  /{} [ {} {} {} {} ]\n", boxname, box.x1, box.y1, box.x2, box.y2);
 }
 
 std::string fontname2pdfname(std::string_view original) {
     std::string out;
     out.reserve(original.size());
     for(const auto c : original) {
         if(c == ' ') {
@@ -186,14 +192,123 @@
 CMapName currentdict /CMap defineresource pop
 end
 end
 )";
     return buf;
 }
 
+std::string serialize_shade4(const ShadingType4 &shade) {
+    std::string s;
+    for(const auto &e : shade.elements) {
+        double xratio = (e.sp.p.x - shade.minx) / (shade.maxx - shade.minx);
+        double yratio = (e.sp.p.y - shade.miny) / (shade.maxy - shade.miny);
+        uint32_t xval = std::numeric_limits<uint32_t>::max() * xratio;
+        uint32_t yval = std::numeric_limits<uint32_t>::max() * yratio;
+        char flag = (char)e.flag;
+        assert(flag >= 0 && flag < 3);
+
+        xval = std::byteswap(xval);
+        yval = std::byteswap(yval);
+        //  FIXME: Assumes rgb is between 0 and 1;
+        const char *ptr;
+        ptr = (const char *)(&flag);
+        s.append(ptr, ptr + sizeof(char));
+        ptr = (const char *)(&xval);
+        s.append(ptr, ptr + sizeof(xval));
+        ptr = (const char *)(&yval);
+        s.append(ptr, ptr + sizeof(yval));
+
+        uint16_t rval = std::numeric_limits<uint16_t>::max() * e.sp.c.r.v();
+        uint16_t gval = std::numeric_limits<uint16_t>::max() * e.sp.c.g.v();
+        uint16_t bval = std::numeric_limits<uint16_t>::max() * e.sp.c.b.v();
+        rval = std::byteswap(rval);
+        gval = std::byteswap(gval);
+        bval = std::byteswap(bval);
+
+        ptr = (const char *)(&rval);
+        s.append(ptr, ptr + sizeof(uint16_t));
+        ptr = (const char *)(&gval);
+        s.append(ptr, ptr + sizeof(uint16_t));
+        ptr = (const char *)(&bval);
+        s.append(ptr, ptr + sizeof(uint16_t));
+    }
+    return s;
+}
+
+std::string serialize_shade6(const ShadingType6 &shade) {
+    std::string s;
+    for(const auto &eh : shade.elements) {
+        assert(std::holds_alternative<FullCoonsPatch>(eh));
+        const auto &e = std::get<FullCoonsPatch>(eh);
+        char flag = 0; //(char)e.flag;
+        assert(flag >= 0 && flag < 3);
+        const char *ptr;
+        ptr = (const char *)(&flag);
+        s.append(ptr, ptr + sizeof(char));
+
+        for(const auto &p : e.p) {
+            double xratio = (p.x - shade.minx) / (shade.maxx - shade.minx);
+            double yratio = (p.y - shade.miny) / (shade.maxy - shade.miny);
+            uint32_t xval = std::numeric_limits<uint32_t>::max() * xratio;
+            uint32_t yval = std::numeric_limits<uint32_t>::max() * yratio;
+
+            xval = std::byteswap(xval);
+            yval = std::byteswap(yval);
+            ptr = (const char *)(&xval);
+            s.append(ptr, ptr + sizeof(xval));
+            ptr = (const char *)(&yval);
+            s.append(ptr, ptr + sizeof(yval));
+        }
+        for(const auto &c : e.c) {
+            uint16_t rval = std::numeric_limits<uint16_t>::max() * c.r.v();
+            uint16_t gval = std::numeric_limits<uint16_t>::max() * c.g.v();
+            uint16_t bval = std::numeric_limits<uint16_t>::max() * c.b.v();
+            rval = std::byteswap(rval);
+            gval = std::byteswap(gval);
+            bval = std::byteswap(bval);
+
+            ptr = (const char *)(&rval);
+            s.append(ptr, ptr + sizeof(uint16_t));
+            ptr = (const char *)(&gval);
+            s.append(ptr, ptr + sizeof(uint16_t));
+            ptr = (const char *)(&bval);
+            s.append(ptr, ptr + sizeof(uint16_t));
+        }
+    }
+    return s;
+}
+
+void serialize_trans(std::back_insert_iterator<std::string> buf_append,
+                     const Transition &t,
+                     std::string_view indent) {
+    fmt::format_to(buf_append, "{}/Trans <<\n", indent);
+    if(t.type) {
+        fmt::format_to(buf_append, "{}  /S {}\n", indent, transition_names.at((int32_t)*t.type));
+    }
+    if(t.duration) {
+        fmt::format_to(buf_append, "{}  /D {}\n", indent, *t.duration);
+    }
+    if(t.Dm) {
+        fmt::format_to(buf_append, "{}  /Dm {}\n", indent, *t.Dm ? "/H" : "/V");
+    }
+    if(t.Di) {
+        fmt::format_to(buf_append, "{}  /Di {}\n", indent, *t.Di);
+    }
+    if(t.M) {
+        fmt::format_to(buf_append, "{}  /M {}\n", indent, *t.M ? "/I" : "/O");
+    }
+    if(t.SS) {
+        fmt::format_to(buf_append, "{}  /SS {}\n", indent, *t.SS);
+    }
+    if(t.B) {
+        fmt::format_to(buf_append, "{}  /B {}\n", indent, *t.B ? "true" : "false");
+    }
+    fmt::format_to(buf_append, "{}>>\n", indent);
+}
+
 } // namespace
 
 const std::array<const char *, 4> rendering_intent_names{
     "RelativeColorimetric",
     "AbsoluteColorimetric",
     "Saturation",
     "Perceptual",
@@ -258,18 +373,19 @@
                                   colorspace_names.at((int)opts.output_colorspace));
     return add_object(FullPDFObject{std::move(buf), ""});
 }
 
 rvoe<NoReturnValue>
 PdfDocument::add_page(std::string resource_data,
                       std::string page_data,
-                      const std::unordered_set<CapyPdF_FormWidgetId> &fws,
-                      const std::unordered_set<CapyPdF_AnnotationId> &annots,
-                      const std::unordered_set<CapyPdF_StructureItemId> &structs,
-                      const std::optional<PageTransition> &transition) {
+                      const std::unordered_set<CapyPDF_FormWidgetId> &fws,
+                      const std::unordered_set<CapyPDF_AnnotationId> &annots,
+                      const std::unordered_set<CapyPDF_StructureItemId> &structs,
+                      const std::optional<Transition> &transition,
+                      const std::vector<SubPageNavigation> &subnav) {
     for(const auto &a : fws) {
         if(form_use.find(a) != form_use.cend()) {
             RETERR(AnnotationReuse);
         }
     }
     for(const auto &a : annots) {
         if(annotation_use.find(a) != annotation_use.cend()) {
@@ -285,17 +401,20 @@
     const auto commands_num = add_object(FullPDFObject{std::move(page_data), ""});
     DelayedPage p;
     p.page_num = (int32_t)pages.size();
     for(const auto &a : fws) {
         p.used_form_widgets.push_back(a);
     }
     for(const auto &a : annots) {
-        p.used_annotations.push_back(CapyPdF_AnnotationId{a});
+        p.used_annotations.push_back(CapyPDF_AnnotationId{a});
     }
     p.transition = transition;
+    if(!subnav.empty()) {
+        p.subnav_root = create_subnavigation(subnav);
+    }
     const auto page_num = add_object(std::move(p));
     for(const auto &fw : fws) {
         form_use[fw] = page_num;
     }
     for(const auto &a : annots) {
         annotation_use[a] = page_num;
     }
@@ -308,14 +427,95 @@
 
 void PdfDocument::add_form_xobject(std::string xobj_dict, std::string xobj_stream) {
     const auto xobj_num = add_object(FullPDFObject{std::move(xobj_dict), std::move(xobj_stream)});
 
     form_xobjects.emplace_back(FormXObjectInfo{xobj_num});
 }
 
+int32_t PdfDocument::create_subnavigation(const std::vector<SubPageNavigation> &subnav) {
+    assert(!subnav.empty());
+    const int32_t root_obj = document_objects.size();
+    {
+        std::string rootbuf{
+            R"(<<
+  /Type /NavNode
+  /NA <<
+    /S /SetOCGState
+    /State [ /OFF
+)"};
+        auto rootapp = std::back_inserter(rootbuf);
+        for(const auto &i : subnav) {
+            fmt::format_to(rootapp, "      {} 0 R\n", ocg_object_number(i.id));
+        }
+        rootbuf += "    ]\n  >>\n";
+        fmt::format_to(rootapp, "  /Next {} 0 R\n", root_obj + 1);
+        rootbuf += R"(  /PA <<
+    /S /SetOCGState
+    /State [ /ON
+)";
+        for(const auto &i : subnav) {
+            fmt::format_to(rootapp, "      {} 0 R\n", ocg_object_number(i.id));
+        }
+        rootbuf += "    ]\n  >>\n";
+        fmt::format_to(rootapp, "  /Prev {} 0 R\n>>\n", root_obj + 1 + subnav.size());
+
+        add_object(FullPDFObject{std::move(rootbuf), ""});
+    }
+    int32_t first_obj = document_objects.size();
+
+    for(size_t i = 0; i < subnav.size(); ++i) {
+        const auto &sn = subnav[i];
+        std::string buf = R"(<<
+  /Type /NavNode
+)";
+        auto app = std::back_inserter(buf);
+        buf += "  /NA  <<\n";
+        fmt::format_to(app,
+                       R"(    /S /SetOCGState
+    /State [ /ON {} 0 R ]
+)",
+                       ocg_object_number(sn.id));
+        if(sn.tr) {
+            buf += R"(    /Next <<
+      /S /Trans
+)";
+            serialize_trans(app, *sn.tr, "      ");
+            buf += "    >>\n";
+        }
+
+        buf += "  >>\n";
+        fmt::format_to(app, "  /Next {} 0 R\n", first_obj + i + 1);
+        if(i > 0) {
+            fmt::format_to(app,
+                           R"(  /PA <<
+    /S /SetOCGState
+    /State [ /OFF {} 0 R ]
+  >>
+)",
+                           ocg_object_number(subnav[i - 1].id));
+            fmt::format_to(app, "  /Prev {} 0 R\n", first_obj + i - 1);
+        }
+        buf += ">>\n";
+        add_object(FullPDFObject{std::move(buf), ""});
+    }
+    add_object(FullPDFObject{fmt::format(R"(<<
+  /Type /NavNode
+  /PA <<
+    /S /SetOCGState
+    /State [ /OFF {} 0 R ]
+  >>
+  /Prev {} 0 R
+>>
+)",
+                                         ocg_object_number(subnav.back().id),
+                                         first_obj + subnav.size() - 1),
+                             ""});
+    return root_obj;
+}
+
 int32_t PdfDocument::add_object(ObjectType object) {
     auto object_num = (int32_t)document_objects.size();
     document_objects.push_back(std::move(object));
     return object_num;
 }
 
 SeparationId PdfDocument::create_separation(std::string_view name,
@@ -371,15 +571,15 @@
         lab.bmin,
         lab.bmax);
 
     add_object(FullPDFObject{std::move(buf), {}});
     return LabId{(int32_t)document_objects.size() - 1};
 }
 
-rvoe<CapyPdF_IccColorSpaceId> PdfDocument::load_icc_file(const char *fname) {
+rvoe<CapyPDF_IccColorSpaceId> PdfDocument::load_icc_file(const std::filesystem::path &fname) {
     ERC(contents, load_file(fname));
     const auto iccid = find_icc_profile(contents);
     if(iccid) {
         return *iccid;
     }
     ERC(num_channels, cm.get_num_channels(contents));
     return store_icc_profile(contents, num_channels);
@@ -448,27 +648,27 @@
                    R"(<<
   /Type /Page
   /Parent {} 0 R
   /Group {} 0 R
 )",
                    pages_object,
                    page_group_object);
-    write_box(buf_append, "MediaBox", opts.mediabox);
+    write_rectangle(buf_append, "MediaBox", opts.mediabox);
 
     if(opts.cropbox) {
-        write_box(buf_append, "CropBox", *opts.cropbox);
+        write_rectangle(buf_append, "CropBox", *opts.cropbox);
     }
     if(opts.bleedbox) {
-        write_box(buf_append, "BleedBox", *opts.bleedbox);
+        write_rectangle(buf_append, "BleedBox", *opts.bleedbox);
     }
     if(opts.trimbox) {
-        write_box(buf_append, "TrimBox", *opts.trimbox);
+        write_rectangle(buf_append, "TrimBox", *opts.trimbox);
     }
     if(opts.artbox) {
-        write_box(buf_append, "ArtBox", *opts.artbox);
+        write_rectangle(buf_append, "ArtBox", *opts.artbox);
     }
     fmt::format_to(buf_append,
                    R"(  /Contents {} 0 R
   /Resources {} 0 R
 )",
                    p.commands_obj_num,
                    p.resource_obj_num);
@@ -481,50 +681,32 @@
         for(const auto &a : dp.used_annotations) {
             fmt::format_to(buf_append, "    {} 0 R\n", annotations.at(a.id));
         }
         buf += "  ]\n";
     }
     if(dp.transition) {
         const auto &t = *dp.transition;
-        buf += "  /Trans <<\n";
-        if(t.type) {
-            fmt::format_to(buf_append, "    /S {}\n", transition_names.at((int32_t)*t.type));
-        }
-        if(t.duration) {
-            fmt::format_to(buf_append, "    /D {}\n", *t.duration);
-        }
-        if(t.Dm) {
-            fmt::format_to(buf_append, "    /Dm {}\n", *t.Dm ? "/H" : "/V");
-        }
-        if(t.Di) {
-            fmt::format_to(buf_append, "    /Di {}\n", *t.Di);
-        }
-        if(t.M) {
-            fmt::format_to(buf_append, "    /M {}\n", *t.M ? "/I" : "/O");
-        }
-        if(t.SS) {
-            fmt::format_to(buf_append, "    /SS {}\n", *t.SS);
-        }
-        if(t.B) {
-            fmt::format_to(buf_append, "    /B {}\n", *t.B ? "true" : "false");
-        }
-        buf += "  >>\n";
+        serialize_trans(buf_append, t, "  ");
+    }
+
+    if(dp.subnav_root) {
+        fmt::format_to(buf_append, "  /PresSteps {} 0 R\n", dp.subnav_root.value());
     }
     buf += ">>\n";
 
     return write_finished_object(p.page_obj_num, buf, "");
 }
 
 rvoe<NoReturnValue> PdfDocument::write_pages_root() {
     std::string buf;
     auto buf_append = std::back_inserter(buf);
     buf = fmt::format(R"(<<
   /Type /Pages
   /Kids [
-  )");
+)");
     for(const auto &i : pages) {
         fmt::format_to(buf_append, "    {} 0 R\n", i.page_obj_num);
     }
     fmt::format_to(buf_append, "  ]\n  /Count {}\n>>\n", pages.size());
     return write_finished_object(pages_object, buf, "");
 }
 
@@ -588,14 +770,25 @@
 )";
         for(const auto &i : form_widgets) {
             fmt::format_to(app, "      {} 0 R\n", i);
         }
         buf += "      ]\n  >>\n";
         buf += "  /NeedAppearances true\n";
     }
+    if(!ocg_items.empty()) {
+        buf += R"(  /OCProperties <<
+    /OCGs [
+)";
+        for(const auto &o : ocg_items) {
+            fmt::format_to(app, "      {} 0 R\n", o);
+        }
+        buf += "    ]\n";
+        buf += "    /D << /BaseState /ON >>\n";
+        buf += "  >>\n";
+    }
     buf += ">>\n";
     add_object(FullPDFObject{buf, ""});
     return NoReturnValue{};
 }
 
 void PdfDocument::create_output_intent() {
     std::string buf;
@@ -674,19 +867,19 @@
     assert(catalog_obj_num == (int32_t)document_objects.size());
     // FIXME: add output intents here. PDF spec 14.11.5
     return add_object(FullPDFObject{std::move(buf), ""});
 }
 
 void PdfDocument::create_structure_root_dict() {
     std::string buf;
-    std::optional<CapyPdF_StructureItemId> rootobj;
+    std::optional<CapyPDF_StructureItemId> rootobj;
 
     for(int32_t i = 0; i < (int32_t)structure_items.size(); ++i) {
         if(!structure_items[i].parent) {
-            rootobj = CapyPdF_StructureItemId{i};
+            rootobj = CapyPDF_StructureItemId{i};
             break;
         }
         // FIXME, check that there is only one.
     }
     assert(rootobj);
     // /ParentTree
     buf = fmt::format(R"(<<
@@ -1005,38 +1198,103 @@
   /A <<
     /S /URI
     /URI {}
   >>
 )",
                        uri_as_str,
                        uri_as_str);
+    } else if(std::holds_alternative<ScreenAnnotation>(annotation.sub)) {
+        auto &sa = std::get<ScreenAnnotation>(annotation.sub);
+        int32_t media_filespec = embedded_files.at(sa.mediafile.id).filespec_obj;
+        if(!sa.times) {
+            fmt::format_to(app,
+                           R"(  /Subtype /Screen
+  /A <<
+    /Type /Action
+    /S /Rendition
+    /OP 0
+    /AN {} 0 R
+    /R <<
+      /Type /Rendition
+      /S /MR
+      /C <<
+        /Type /MediaClip
+        /CT ({})
+        /S /MCD
+        /D {} 0 R
+        /P << /TF (TEMPALWAYS) >>
+      >>
+    >>
+  >>
+)",
+                           obj_num,
+                           sa.mimetype,
+                           media_filespec);
+        } else {
+            // NOTE! This should work but does not. Acrobat reader will error
+            // out if there are any entries in the MH dictionary, regardless whether they
+            // are time or frame dictionaries.
+            fmt::format_to(app,
+                           R"(  /Subtype /Screen
+  /A <<
+    /Type /Action
+    /S /Rendition
+    /OP 0
+    /AN {} 0 R
+    /R <<
+      /Type /Rendition
+      /S /MR
+      /C <<
+        /Type /MediaClip
+        /S /MCS
+        /D <<
+          /Type /MediaClip
+          /CT ({})
+          /S /MCD
+          /D {} 0 R
+          /P << /TF (TEMPALWAYS) >>
+        >>
+        /MH <<
+          /B << /S /T /T << /S /S /V {} >> >>
+          /E << /S /T /T << /S /S /V {} >> >>
+        >>
+      >>
+    >>
+  >>
+)",
+                           obj_num,
+                           sa.mimetype,
+                           media_filespec,
+                           sa.times->starttime,
+                           sa.times->endtime);
+        }
     } else {
         std::abort();
     }
     dict += ">>\n";
     ERCV(write_finished_object(obj_num, dict, ""));
     return NoReturnValue{};
 }
 
 rvoe<NoReturnValue> PdfDocument::write_delayed_structure_item(int obj_num,
                                                               const DelayedStructItem &dsi) {
-    std::vector<CapyPdF_StructureItemId> children;
+    std::vector<CapyPDF_StructureItemId> children;
     const auto &si = structure_items.at(dsi.sid.id);
     assert(structure_root_object);
     int32_t parent_object = *structure_root_object;
     if(si.parent) {
         parent_object = structure_items.at(si.parent->id).obj_id;
     }
 
     // Yes, this is O(n^2). I got lazy.
     for(int32_t i = 0; i < (int32_t)structure_items.size(); ++i) {
         if(structure_items[i].parent) {
             auto current_parent = structure_items.at(structure_items[i].parent->id).obj_id;
             if(current_parent == si.obj_id) {
-                children.emplace_back(CapyPdF_StructureItemId{i});
+                children.emplace_back(CapyPDF_StructureItemId{i});
             }
         }
     }
     std::string dict = fmt::format(R"(<<
   /Type /StructElem
   /S /{}
   /P {} 0 R
@@ -1077,44 +1335,44 @@
     if(buf.back() != '\n') {
         buf += '\n';
     }
     buf += "endobj\n";
     return write_bytes(buf);
 }
 
-std::optional<CapyPdF_IccColorSpaceId> PdfDocument::find_icc_profile(std::string_view contents) {
+std::optional<CapyPDF_IccColorSpaceId> PdfDocument::find_icc_profile(std::string_view contents) {
     for(size_t i = 0; i < icc_profiles.size(); ++i) {
         const auto &obj = document_objects.at(icc_profiles.at(i).object_num);
         assert(std::holds_alternative<DeflatePDFObject>(obj));
         const auto &iccobj = std::get<DeflatePDFObject>(obj);
         if(iccobj.stream == contents) {
-            return CapyPdF_IccColorSpaceId{(int32_t)i};
+            return CapyPDF_IccColorSpaceId{(int32_t)i};
         }
     }
     return {};
 }
 
-CapyPdF_IccColorSpaceId PdfDocument::store_icc_profile(std::string_view contents,
+CapyPDF_IccColorSpaceId PdfDocument::store_icc_profile(std::string_view contents,
                                                        int32_t num_channels) {
     auto existing = find_icc_profile(contents);
     assert(!existing);
     if(contents.empty()) {
-        return CapyPdF_IccColorSpaceId{-1};
+        return CapyPDF_IccColorSpaceId{-1};
     }
     std::string buf;
     fmt::format_to(std::back_inserter(buf),
                    R"(<<
   /N {}
 )",
                    num_channels);
     auto stream_obj_id = add_object(DeflatePDFObject{std::move(buf), std::string{contents}});
     auto obj_id =
         add_object(FullPDFObject{fmt::format("[ /ICCBased {} 0 R ]\n", stream_obj_id), ""});
     icc_profiles.emplace_back(IccInfo{stream_obj_id, obj_id, num_channels});
-    return CapyPdF_IccColorSpaceId{(int32_t)icc_profiles.size() - 1};
+    return CapyPDF_IccColorSpaceId{(int32_t)icc_profiles.size() - 1};
 }
 
 rvoe<NoReturnValue> PdfDocument::write_bytes(const char *buf, size_t buf_size) {
     if(fwrite(buf, 1, buf_size, ofile) != buf_size) {
         perror(nullptr);
         RETERR(FileWriteError);
     }
@@ -1136,49 +1394,49 @@
     }
     if(!opts.author.empty()) {
         obj_data.dictionary += "  /Author ";
         ERC(authorstr, utf8_to_pdfmetastr(opts.author));
         obj_data.dictionary += authorstr;
         obj_data.dictionary += "\n";
     }
-    obj_data.dictionary += "  /Producer (A4PDF " CAPYPDF_VERSION_STR ")\n";
+    obj_data.dictionary += "  /Producer (CapyPDF " CAPYPDF_VERSION_STR ")\n";
     obj_data.dictionary += "  /CreationDate ";
     obj_data.dictionary += current_date_string();
     obj_data.dictionary += '\n';
     obj_data.dictionary += ">>\n";
     add_object(std::move(obj_data));
     return NoReturnValue{};
 }
 
-CapyPdF_FontId PdfDocument::get_builtin_font_id(CapyPdF_Builtin_Fonts font) {
+CapyPDF_FontId PdfDocument::get_builtin_font_id(CapyPDF_Builtin_Fonts font) {
     auto it = builtin_fonts.find(font);
     if(it != builtin_fonts.end()) {
         return it->second;
     }
     std::string font_dict;
     fmt::format_to(std::back_inserter(font_dict),
                    R"(<<
   /Type /Font
   /Subtype /Type1
   /BaseFont /{}
 >>
 )",
                    font_names[font]);
     font_objects.push_back(FontInfo{-1, -1, add_object(FullPDFObject{font_dict, ""}), size_t(-1)});
-    auto fontid = CapyPdF_FontId{(int32_t)font_objects.size() - 1};
+    auto fontid = CapyPDF_FontId{(int32_t)font_objects.size() - 1};
     builtin_fonts[font] = fontid;
     return fontid;
 }
 
 uint32_t PdfDocument::glyph_for_codepoint(FT_Face face, uint32_t ucs4) {
     assert(face);
     return FT_Get_Char_Index(face, ucs4);
 }
 
-rvoe<SubsetGlyph> PdfDocument::get_subset_glyph(CapyPdF_FontId fid, uint32_t glyph) {
+rvoe<SubsetGlyph> PdfDocument::get_subset_glyph(CapyPDF_FontId fid, uint32_t glyph) {
     SubsetGlyph fss;
     ERC(blub, fonts.at(fid.id).subsets.get_glyph_subset(glyph));
     fss.ss.fid = fid;
     if(true) {
         fss.ss.subset_id = blub.subset;
         fss.glyph_id = blub.offset;
     } else {
@@ -1188,40 +1446,40 @@
             std::abort();
         }
         fss.glyph_id = glyph;
     }
     return fss;
 }
 
-rvoe<CapyPdF_ImageId> PdfDocument::load_image(const std::filesystem::path &fname) {
+rvoe<CapyPDF_ImageId> PdfDocument::load_image(const std::filesystem::path &fname) {
     ERC(image, load_image_file(fname));
     if(std::holds_alternative<rgb_image>(image)) {
         return process_rgb_image(std::get<rgb_image>(image));
     } else if(std::holds_alternative<gray_image>(image)) {
         return process_gray_image(std::get<gray_image>(image));
     } else if(std::holds_alternative<mono_image>(image)) {
         return process_mono_image(std::get<mono_image>(image));
     } else if(std::holds_alternative<cmyk_image>(image)) {
         return process_cmyk_image(std::get<cmyk_image>(image));
     } else {
         RETERR(UnsupportedFormat);
     }
 }
 
-rvoe<CapyPdF_ImageId> PdfDocument::load_mask_image(const std::filesystem::path &fname) {
+rvoe<CapyPDF_ImageId> PdfDocument::load_mask_image(const std::filesystem::path &fname) {
     ERC(image, load_image_file(fname));
     if(!std::holds_alternative<mono_image>(image)) {
         RETERR(UnsupportedFormat);
     }
     auto &im = std::get<mono_image>(image);
     return add_image_object(
         im.w, im.h, 1, CAPYPDF_CS_DEVICE_GRAY, std::optional<int32_t>{}, true, im.pixels);
 }
 
-rvoe<CapyPdF_ImageId> PdfDocument::add_image_object(int32_t w,
+rvoe<CapyPDF_ImageId> PdfDocument::add_image_object(int32_t w,
                                                     int32_t h,
                                                     int32_t bits_per_component,
                                                     ColorspaceType colorspace,
                                                     std::optional<int32_t> smask_id,
                                                     bool is_mask,
                                                     std::string_view uncompressed_bytes) {
     std::string buf;
@@ -1241,16 +1499,16 @@
                    h,
                    bits_per_component,
                    compressed.size());
     // An image may only have ImageMask or ColorSpace key, not both.
     if(is_mask) {
         buf += "  /ImageMask true\n";
     } else {
-        if(std::holds_alternative<CapyPdF_Colorspace>(colorspace)) {
-            const auto &cs = std::get<CapyPdF_Colorspace>(colorspace);
+        if(std::holds_alternative<CapyPDF_Colorspace>(colorspace)) {
+            const auto &cs = std::get<CapyPDF_Colorspace>(colorspace);
             fmt::format_to(app, "  /ColorSpace {}\n", colorspace_names.at(cs));
         } else if(std::holds_alternative<int32_t>(colorspace)) {
             const auto icc_obj = std::get<int32_t>(colorspace);
             fmt::format_to(app, "  /ColorSpace {} 0 R\n", icc_obj);
         } else {
             fprintf(stderr, "Unknown colorspace.");
             std::abort();
@@ -1258,29 +1516,29 @@
     }
     if(smask_id) {
         fmt::format_to(app, "  /SMask {} 0 R\n", smask_id.value());
     }
     buf += ">>\n";
     auto im_id = add_object(FullPDFObject{std::move(buf), std::move(compressed)});
     image_info.emplace_back(ImageInfo{{w, h}, im_id});
-    return CapyPdF_ImageId{(int32_t)image_info.size() - 1};
+    return CapyPDF_ImageId{(int32_t)image_info.size() - 1};
 }
 
-rvoe<CapyPdF_ImageId> PdfDocument::process_mono_image(const mono_image &image) {
+rvoe<CapyPDF_ImageId> PdfDocument::process_mono_image(const mono_image &image) {
     std::optional<int32_t> smask_id;
     if(image.alpha) {
         ERC(imobj,
             add_image_object(image.w, image.h, 1, CAPYPDF_CS_DEVICE_GRAY, {}, false, *image.alpha));
         smask_id = image_info.at(imobj.id).obj;
     }
     return add_image_object(
         image.w, image.h, 1, CAPYPDF_CS_DEVICE_GRAY, smask_id, false, image.pixels);
 }
 
-rvoe<CapyPdF_ImageId> PdfDocument::process_rgb_image(const rgb_image &image) {
+rvoe<CapyPDF_ImageId> PdfDocument::process_rgb_image(const rgb_image &image) {
     std::optional<int32_t> smask_id;
     if(image.alpha) {
         ERC(imobj,
             add_image_object(image.w, image.h, 8, CAPYPDF_CS_DEVICE_GRAY, {}, false, *image.alpha));
         smask_id = image_info.at(imobj.id).obj;
     }
     switch(opts.output_colorspace) {
@@ -1302,29 +1560,29 @@
             image.w, image.h, 8, CAPYPDF_CS_DEVICE_CMYK, smask_id, false, converted_pixels);
     }
     default:
         RETERR(Unreachable);
     }
 }
 
-rvoe<CapyPdF_ImageId> PdfDocument::process_gray_image(const gray_image &image) {
+rvoe<CapyPDF_ImageId> PdfDocument::process_gray_image(const gray_image &image) {
     std::optional<int32_t> smask_id;
 
     // Fixme: maybe do color conversion from whatever-gray to a known gray colorspace?
 
     if(image.alpha) {
         ERC(imgobj,
             add_image_object(image.w, image.h, 8, CAPYPDF_CS_DEVICE_GRAY, {}, false, *image.alpha));
         smask_id = image_info.at(imgobj.id).obj;
     }
     return add_image_object(
         image.w, image.h, 8, CAPYPDF_CS_DEVICE_GRAY, smask_id, false, image.pixels);
 }
 
-rvoe<CapyPdF_ImageId> PdfDocument::process_cmyk_image(const cmyk_image &image) {
+rvoe<CapyPDF_ImageId> PdfDocument::process_cmyk_image(const cmyk_image &image) {
     std::optional<int32_t> smask_id;
     ColorspaceType cs;
     if(image.icc) {
         auto oldicc = find_icc_profile(*image.icc);
         if(oldicc) {
             cs = icc_profiles.at(oldicc->id).object_num;
         } else {
@@ -1338,15 +1596,15 @@
         ERC(imobj,
             add_image_object(image.w, image.h, 8, CAPYPDF_CS_DEVICE_GRAY, {}, false, *image.alpha));
         smask_id = image_info.at(imobj.id).obj;
     }
     return add_image_object(image.w, image.h, 8, cs, smask_id, false, image.pixels);
 }
 
-rvoe<CapyPdF_ImageId> PdfDocument::embed_jpg(const std::filesystem::path &fname) {
+rvoe<CapyPDF_ImageId> PdfDocument::embed_jpg(const std::filesystem::path &fname) {
     ERC(jpg, load_jpg(fname));
     std::string buf;
     fmt::format_to(std::back_inserter(buf),
                    R"(<<
   /Type /XObject
   /Subtype /Image
   /ColorSpace /DeviceRGB
@@ -1358,15 +1616,15 @@
 >>
 )",
                    jpg.w,
                    jpg.h,
                    jpg.file_contents.length());
     auto im_id = add_object(FullPDFObject{std::move(buf), std::move(jpg.file_contents)});
     image_info.emplace_back(ImageInfo{{jpg.w, jpg.h}, im_id});
-    return CapyPdF_ImageId{(int32_t)image_info.size() - 1};
+    return CapyPDF_ImageId{(int32_t)image_info.size() - 1};
 }
 
 GstateId PdfDocument::add_graphics_state(const GraphicsState &state) {
     const int32_t id = (int32_t)document_objects.size();
     std::string buf{
         R"(<<
   /Type /ExtGState
@@ -1417,17 +1675,16 @@
     buf += "]\n";
     buf += "  /C1 [ ";
     for(const auto d : func.C1) {
         fmt::format_to(resource_appender, "{} ", d);
     }
     buf += "]\n";
     buf += ">>\n";
-    add_object(FullPDFObject{std::move(buf), {}});
 
-    return FunctionId{(int32_t)document_objects.size()};
+    return FunctionId{add_object(FullPDFObject{std::move(buf), {}})};
 }
 
 ShadingId PdfDocument::add_shading(const ShadingType2 &shade) {
     const int shadingtype = 2;
     std::string buf = fmt::format(
         R"(<<
   /ShadingType {}
@@ -1442,17 +1699,16 @@
         shade.x0,
         shade.y0,
         shade.x1,
         shade.y1,
         shade.function.id,
         shade.extend0 ? "true" : "false",
         shade.extend1 ? "true" : "false");
-    add_object(FullPDFObject{std::move(buf), {}});
 
-    return ShadingId{(int32_t)document_objects.size()};
+    return ShadingId{add_object(FullPDFObject{std::move(buf), {}})};
 }
 
 ShadingId PdfDocument::add_shading(const ShadingType3 &shade) {
     const int shadingtype = 3;
     std::string buf = fmt::format(
         R"(<<
   /ShadingType {}
@@ -1469,49 +1725,121 @@
         shade.r0,
         shade.x1,
         shade.y1,
         shade.r1,
         shade.function.id,
         shade.extend0 ? "true" : "false",
         shade.extend1 ? "true" : "false");
-    add_object(FullPDFObject{std::move(buf), {}});
 
-    return ShadingId{(int32_t)document_objects.size()};
+    return ShadingId{add_object(FullPDFObject{std::move(buf), {}})};
+}
+
+ShadingId PdfDocument::add_shading(const ShadingType4 &shade) {
+    const int shadingtype = 4;
+    std::string serialized = serialize_shade4(shade);
+    std::string buf = fmt::format(
+        R"(<<
+  /ShadingType {}
+  /ColorSpace {}
+  /BitsPerCoordinate 32
+  /BitsPerComponent 16
+  /BitsPerFlag 8
+  /Decode [
+    {} {}
+    {} {}
+    {} {}
+    {} {}
+    {} {}
+  ]
+  /Length {}
+>>
+)",
+        shadingtype,
+        colorspace_names.at((int)shade.colorspace),
+        shade.minx,
+        shade.maxx,
+        shade.miny,
+        shade.maxy,
+        0,
+        1,
+        0,
+        1,
+        0,
+        1,
+        serialized.length());
+
+    return ShadingId{add_object(FullPDFObject{std::move(buf), std::move(serialized)})};
+}
+
+ShadingId PdfDocument::add_shading(const ShadingType6 &shade) {
+    const int shadingtype = 6;
+    std::string serialized = serialize_shade6(shade);
+    std::string buf = fmt::format(
+        R"(<<
+  /ShadingType {}
+  /ColorSpace {}
+  /BitsPerCoordinate 32
+  /BitsPerComponent 16
+  /BitsPerFlag 8
+  /Decode [
+    {} {}
+    {} {}
+    {} {}
+    {} {}
+    {} {}
+  ]
+  /Length {}
+>>
+)",
+        shadingtype,
+        colorspace_names.at((int)shade.colorspace),
+        shade.minx,
+        shade.maxx,
+        shade.miny,
+        shade.maxy,
+        0,
+        1,
+        0,
+        1,
+        0,
+        1,
+        serialized.length());
+
+    return ShadingId{add_object(FullPDFObject{std::move(buf), std::move(serialized)})};
 }
 
 PatternId PdfDocument::add_pattern(std::string_view pattern_dict, std::string_view commands) {
-    add_object(FullPDFObject{std::string(pattern_dict), std::string(commands)});
-    return PatternId{(int32_t)document_objects.size()};
+    return PatternId{add_object(FullPDFObject{std::string(pattern_dict), std::string(commands)})};
 }
 
 OutlineId PdfDocument::add_outline(std::string_view title_utf8,
                                    PageId dest,
                                    std::optional<OutlineId> parent) {
     const auto cur_id = (int32_t)outlines.items.size();
     const auto par_id = parent.value_or(OutlineId{-1}).id;
     outlines.parent[cur_id] = par_id;
     outlines.children[par_id].push_back(cur_id);
     outlines.items.emplace_back(Outline{std::string{title_utf8}, dest, parent});
     return OutlineId{cur_id};
 }
 
-rvoe<CapyPdF_FormWidgetId> PdfDocument::create_form_checkbox(PdfBox loc,
-                                                             CapyPdF_FormXObjectId onstate,
-                                                             CapyPdF_FormXObjectId offstate,
+rvoe<CapyPDF_FormWidgetId> PdfDocument::create_form_checkbox(PdfBox loc,
+                                                             CapyPDF_FormXObjectId onstate,
+                                                             CapyPDF_FormXObjectId offstate,
                                                              std::string_view partial_name) {
     CHECK_INDEXNESS_V(onstate.id, form_xobjects);
     CHECK_INDEXNESS_V(offstate.id, form_xobjects);
     DelayedCheckboxWidgetAnnotation formobj{
         (int32_t)form_widgets.size(), loc, onstate, offstate, std::string{partial_name}};
     auto obj_id = add_object(std::move(formobj));
     form_widgets.push_back(obj_id);
-    return CapyPdF_FormWidgetId{(int32_t)form_widgets.size() - 1};
+    return CapyPDF_FormWidgetId{(int32_t)form_widgets.size() - 1};
 }
 
-rvoe<CapyPdF_EmbeddedFileId> PdfDocument::embed_file(const std::filesystem::path &fname) {
+rvoe<CapyPDF_EmbeddedFileId> PdfDocument::embed_file(const std::filesystem::path &fname) {
     ERC(contents, load_file(fname));
     std::string dict = fmt::format(R"(<<
   /Type /EmbeddedFile
   /Length {}
 >>)",
                                    contents.size());
     auto fileobj_id = add_object(FullPDFObject{std::move(dict), std::move(contents)});
@@ -1521,55 +1849,68 @@
   /EF << /F {} 0 R >>
 >>
 )",
                        pdfstring_quote(fname.filename().string()),
                        fileobj_id);
     auto filespec_id = add_object(FullPDFObject{std::move(dict), ""});
     embedded_files.emplace_back(EmbeddedFileObject{filespec_id, fileobj_id});
-    return CapyPdF_EmbeddedFileId{(int32_t)embedded_files.size() - 1};
+    return CapyPDF_EmbeddedFileId{(int32_t)embedded_files.size() - 1};
 }
 
-rvoe<CapyPdF_AnnotationId> PdfDocument::create_annotation(PdfRectangle rect,
+rvoe<CapyPDF_AnnotationId> PdfDocument::create_annotation(PdfRectangle rect,
                                                           AnnotationSubType sub) {
     if(std::holds_alternative<UriAnnotation>(sub)) {
         auto &u = std::get<UriAnnotation>(sub);
         if(!is_ascii(u.uri)) {
             RETERR(UriNotAscii);
         }
     }
     auto annot_id = (int32_t)annotations.size();
     auto obj_id = add_object(DelayedAnnotation{annot_id, rect, std::move(sub)});
     annotations.push_back((int32_t)obj_id);
-    return CapyPdF_AnnotationId{annot_id};
+    return CapyPDF_AnnotationId{annot_id};
 }
 
-rvoe<CapyPdF_StructureItemId>
+rvoe<CapyPDF_StructureItemId>
 PdfDocument::add_structure_item(std::string_view stype,
-                                std::optional<CapyPdF_StructureItemId> parent) {
+                                std::optional<CapyPDF_StructureItemId> parent) {
     if(parent) {
         CHECK_INDEXNESS_V(parent->id, structure_items);
     }
     auto stritem_id = (int32_t)structure_items.size();
     auto obj_id = add_object(DelayedStructItem{stritem_id});
     structure_items.push_back(StructItem{obj_id, std::string(stype), parent});
-    return CapyPdF_StructureItemId{(int32_t)structure_items.size() - 1};
+    return CapyPDF_StructureItemId{(int32_t)structure_items.size() - 1};
+}
+
+rvoe<CapyPDF_OptionalContentGroupId>
+PdfDocument::add_optional_content_group(const OptionalContentGroup &g) {
+    auto id = add_object(FullPDFObject{fmt::format(R"(<<
+  /Type /OCG
+  /Name {}
+>>
+)",
+                                                   pdfstring_quote(g.name)),
+                                       ""});
+    ocg_items.push_back(id);
+    return CapyPDF_OptionalContentGroupId{(int32_t)ocg_items.size() - 1};
 }
 
 std::optional<double>
-PdfDocument::glyph_advance(CapyPdF_FontId fid, double pointsize, uint32_t codepoint) const {
+PdfDocument::glyph_advance(CapyPDF_FontId fid, double pointsize, uint32_t codepoint) const {
     FT_Face face = fonts.at(fid.id).fontdata.face.get();
     FT_Set_Char_Size(face, 0, pointsize * 64, 300, 300);
     if(FT_Load_Char(face, codepoint, FT_LOAD_NO_HINTING | FT_LOAD_NO_BITMAP) != 0) {
         return {};
     }
     const auto font_unit_advance = face->glyph->metrics.horiAdvance;
     return (font_unit_advance / 64.0) / 300.0 * 72.0;
 }
 
-rvoe<CapyPdF_FontId> PdfDocument::load_font(FT_Library ft, const std::filesystem::path &fname) {
+rvoe<CapyPDF_FontId> PdfDocument::load_font(FT_Library ft, const std::filesystem::path &fname) {
     ERC(fontdata, load_and_parse_truetype_font(fname));
     TtfFont ttf{std::unique_ptr<FT_FaceRec_, FT_Error (*)(FT_Face)>{nullptr, guarded_face_close},
                 std::move(fontdata)};
     FT_Face face;
     auto error = FT_New_Face(ft, fname.string().c_str(), 0, &face);
     if(error) {
         // By default Freetype is compiled without
@@ -1607,22 +1948,22 @@
     }
     auto font_source_id = fonts.size();
     ERC(fss, FontSubsetter::construct(fname, face));
     fonts.emplace_back(FontThingy{std::move(ttf), std::move(fss)});
 
     const int32_t subset_num = 0;
     auto subfont_data_obj =
-        add_object(DelayedSubsetFontData{CapyPdF_FontId{(int32_t)font_source_id}, subset_num});
+        add_object(DelayedSubsetFontData{CapyPDF_FontId{(int32_t)font_source_id}, subset_num});
     auto subfont_descriptor_obj = add_object(DelayedSubsetFontDescriptor{
-        CapyPdF_FontId{(int32_t)font_source_id}, subfont_data_obj, subset_num});
+        CapyPDF_FontId{(int32_t)font_source_id}, subfont_data_obj, subset_num});
     auto subfont_cmap_obj =
-        add_object(DelayedSubsetCMap{CapyPdF_FontId{(int32_t)font_source_id}, subset_num});
+        add_object(DelayedSubsetCMap{CapyPDF_FontId{(int32_t)font_source_id}, subset_num});
     auto subfont_obj = add_object(DelayedSubsetFont{
-        CapyPdF_FontId{(int32_t)font_source_id}, subfont_descriptor_obj, subfont_cmap_obj});
+        CapyPDF_FontId{(int32_t)font_source_id}, subfont_descriptor_obj, subfont_cmap_obj});
     (void)subfont_obj;
-    CapyPdF_FontId fid{(int32_t)fonts.size() - 1};
+    CapyPDF_FontId fid{(int32_t)fonts.size() - 1};
     font_objects.push_back(
         FontInfo{subfont_data_obj, subfont_descriptor_obj, subfont_obj, fonts.size() - 1});
     return fid;
 }
 
 } // namespace capypdf
```

### Comparing `capypdf-0.3.0/src/pdfdocument.hpp` & `capypdf-0.4.0/src/pdfdocument.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -84,42 +84,43 @@
 
 struct DeflatePDFObject {
     std::string unclosed_dictionary;
     std::string stream;
 };
 
 struct DelayedSubsetFontData {
-    CapyPdF_FontId fid;
+    CapyPDF_FontId fid;
     int32_t subset_id;
 };
 
 struct DelayedSubsetCMap {
-    CapyPdF_FontId fid;
+    CapyPDF_FontId fid;
     int32_t subset_id;
 };
 
 struct DelayedSubsetFontDescriptor {
-    CapyPdF_FontId fid;
+    CapyPDF_FontId fid;
     int32_t subfont_data_obj;
     int32_t subset_num;
 };
 
 struct DelayedSubsetFont {
-    CapyPdF_FontId fid;
+    CapyPDF_FontId fid;
     int32_t subfont_descriptor_obj;
     int32_t subfont_cmap_obj;
 };
 
 struct DelayedPages {};
 
 struct DelayedPage {
     int32_t page_num;
-    std::vector<CapyPdF_FormWidgetId> used_form_widgets;
-    std::vector<CapyPdF_AnnotationId> used_annotations;
-    std::optional<PageTransition> transition;
+    std::vector<CapyPDF_FormWidgetId> used_form_widgets;
+    std::vector<CapyPDF_AnnotationId> used_annotations;
+    std::optional<Transition> transition;
+    std::optional<int32_t> subnav_root;
 };
 
 struct SubsetGlyph {
     FontSubset ss;
     uint8_t glyph_id;
 };
 
@@ -143,23 +144,23 @@
 enum IntentSubtype {
     SUBTYPE_PDFX,
     SUBTYPE_PDFA,
     // SUBTYPE_PDFE,
 };
 
 struct PdfGenerationData {
-    PdfBox mediabox = PdfBox::a4();
-    std::optional<PdfBox> cropbox;
-    std::optional<PdfBox> bleedbox;
-    std::optional<PdfBox> trimbox;
-    std::optional<PdfBox> artbox;
+    PdfRectangle mediabox = PdfRectangle::a4();
+    std::optional<PdfRectangle> cropbox;
+    std::optional<PdfRectangle> bleedbox;
+    std::optional<PdfRectangle> trimbox;
+    std::optional<PdfRectangle> artbox;
 
     std::string title;
     std::string author;
-    CapyPdF_Colorspace output_colorspace = CAPYPDF_CS_DEVICE_RGB;
+    CapyPDF_Colorspace output_colorspace = CAPYPDF_CS_DEVICE_RGB;
     ColorProfiles prof;
     std::optional<IntentSubtype> subtype;
     std::string intent_condition_identifier;
 };
 
 struct Outline {
     std::string title;
@@ -173,20 +174,20 @@
 };
 
 class PdfGen;
 class PdfDrawContext;
 struct ColorPatternBuilder;
 
 struct DelayedCheckboxWidgetAnnotation {
-    CapyPdF_FormWidgetId widget;
+    CapyPDF_FormWidgetId widget;
 
     // Annotation dict values.
     PdfBox rect;
-    CapyPdF_FormXObjectId on;
-    CapyPdF_FormXObjectId off;
+    CapyPDF_FormXObjectId on;
+    CapyPDF_FormXObjectId off;
     // uint32_t F; // Annotation flags;
 
     // Field dict values.
     std::string T;
 };
 
 struct OutlineData {
@@ -199,41 +200,53 @@
     int32_t filespec_obj;
     int32_t contents_obj;
 };
 
 // Other types here.
 
 struct FileAttachmentAnnotation {
-    CapyPdF_EmbeddedFileId fileid;
+    CapyPDF_EmbeddedFileId fileid;
 };
 
 struct TextAnnotation {
     std::string content;
 };
 
 struct UriAnnotation {
     std::string uri;
 };
 
-typedef std::variant<TextAnnotation, FileAttachmentAnnotation, UriAnnotation> AnnotationSubType;
+struct ClipTimes {
+    double starttime;
+    double endtime;
+};
+
+struct ScreenAnnotation {
+    CapyPDF_EmbeddedFileId mediafile;
+    std::string mimetype;
+    std::optional<ClipTimes> times;
+};
+
+typedef std::variant<TextAnnotation, FileAttachmentAnnotation, UriAnnotation, ScreenAnnotation>
+    AnnotationSubType;
 
 struct DelayedAnnotation {
-    CapyPdF_AnnotationId id;
+    CapyPDF_AnnotationId id;
     PdfRectangle rect;
     AnnotationSubType sub;
 };
 
 struct DelayedStructItem {
-    CapyPdF_StructureItemId sid;
+    CapyPDF_StructureItemId sid;
 };
 
 struct StructItem {
     int32_t obj_id;
     std::string stype;
-    std::optional<CapyPdF_StructureItemId> parent;
+    std::optional<CapyPDF_StructureItemId> parent;
 };
 
 typedef std::variant<DummyIndexZero,
                      FullPDFObject,
                      DeflatePDFObject,
                      DelayedSubsetFontData,
                      DelayedSubsetFontDescriptor,
@@ -242,15 +255,15 @@
                      DelayedPages,
                      DelayedPage,
                      DelayedCheckboxWidgetAnnotation, // FIXME, convert to hold all widgets
                      DelayedAnnotation,
                      DelayedStructItem>
     ObjectType;
 
-typedef std::variant<CapyPdF_Colorspace, int32_t> ColorspaceType;
+typedef std::variant<CapyPDF_Colorspace, int32_t> ColorspaceType;
 
 class PdfDocument {
 public:
     static rvoe<PdfDocument> construct(const PdfGenerationData &d, PdfColorConverter cm);
 
     PdfDocument(PdfDocument &&o) = default;
 
@@ -258,88 +271,99 @@
     friend class PdfDrawContext;
 
     rvoe<NoReturnValue> write_to_file(FILE *output_file);
 
     // Pages
     rvoe<NoReturnValue> add_page(std::string resource_data,
                                  std::string page_data,
-                                 const std::unordered_set<CapyPdF_FormWidgetId> &form_widgets,
-                                 const std::unordered_set<CapyPdF_AnnotationId> &annots,
-                                 const std::unordered_set<CapyPdF_StructureItemId> &structs,
-                                 const std::optional<PageTransition> &transition);
+                                 const std::unordered_set<CapyPDF_FormWidgetId> &form_widgets,
+                                 const std::unordered_set<CapyPDF_AnnotationId> &annots,
+                                 const std::unordered_set<CapyPDF_StructureItemId> &structs,
+                                 const std::optional<Transition> &transition,
+                                 const std::vector<SubPageNavigation> &subnav);
 
     // Form XObjects
     void add_form_xobject(std::string xobj_data, std::string xobj_stream);
 
     // Colors
     SeparationId create_separation(std::string_view name, const DeviceCMYKColor &fallback);
     LabId add_lab_colorspace(const LabColorSpace &lab);
-    rvoe<CapyPdF_IccColorSpaceId> load_icc_file(const char *fname);
+    rvoe<CapyPDF_IccColorSpaceId> load_icc_file(const std::filesystem::path &fname);
 
     // Fonts
-    rvoe<CapyPdF_FontId> load_font(FT_Library ft, const std::filesystem::path &fname);
-    rvoe<SubsetGlyph> get_subset_glyph(CapyPdF_FontId fid, uint32_t glyph);
+    rvoe<CapyPDF_FontId> load_font(FT_Library ft, const std::filesystem::path &fname);
+    rvoe<SubsetGlyph> get_subset_glyph(CapyPDF_FontId fid, uint32_t glyph);
     uint32_t glyph_for_codepoint(FT_Face face, uint32_t ucs4);
-    CapyPdF_FontId get_builtin_font_id(CapyPdF_Builtin_Fonts font);
+    CapyPDF_FontId get_builtin_font_id(CapyPDF_Builtin_Fonts font);
 
     // Images
-    rvoe<CapyPdF_ImageId> load_image(const std::filesystem::path &fname);
-    rvoe<CapyPdF_ImageId> load_mask_image(const std::filesystem::path &fname);
-    rvoe<CapyPdF_ImageId> embed_jpg(const std::filesystem::path &fname);
+    rvoe<CapyPDF_ImageId> load_image(const std::filesystem::path &fname);
+    rvoe<CapyPDF_ImageId> load_mask_image(const std::filesystem::path &fname);
+    rvoe<CapyPDF_ImageId> embed_jpg(const std::filesystem::path &fname);
 
     // Graphics states
     GstateId add_graphics_state(const GraphicsState &state);
 
     // Functions
     FunctionId add_function(const FunctionType2 &func);
 
     // Shading
     ShadingId add_shading(const ShadingType2 &shade);
     ShadingId add_shading(const ShadingType3 &shade);
+    ShadingId add_shading(const ShadingType4 &shade);
+    ShadingId add_shading(const ShadingType6 &shade);
 
     // Patterns
     PatternId add_pattern(std::string_view pattern_dict, std::string_view commands);
 
     // Outlines
     OutlineId
     add_outline(std::string_view title_utf8, PageId dest, std::optional<OutlineId> parent);
 
     // Forms
-    rvoe<CapyPdF_FormWidgetId> create_form_checkbox(PdfBox loc,
-                                                    CapyPdF_FormXObjectId onstate,
-                                                    CapyPdF_FormXObjectId offstate,
+    rvoe<CapyPDF_FormWidgetId> create_form_checkbox(PdfBox loc,
+                                                    CapyPDF_FormXObjectId onstate,
+                                                    CapyPDF_FormXObjectId offstate,
                                                     std::string_view partial_name);
 
     // Raw files
-    rvoe<CapyPdF_EmbeddedFileId> embed_file(const std::filesystem::path &fname);
+    rvoe<CapyPDF_EmbeddedFileId> embed_file(const std::filesystem::path &fname);
 
     // Annotations.
-    rvoe<CapyPdF_AnnotationId> create_annotation(PdfRectangle rect, AnnotationSubType subtype);
+    rvoe<CapyPDF_AnnotationId> create_annotation(PdfRectangle rect, AnnotationSubType subtype);
 
     // Structure items
-    rvoe<CapyPdF_StructureItemId> add_structure_item(std::string_view stype,
-                                                     std::optional<CapyPdF_StructureItemId> parent);
+    rvoe<CapyPDF_StructureItemId> add_structure_item(std::string_view stype,
+                                                     std::optional<CapyPDF_StructureItemId> parent);
+
+    // Optional content groups
+    rvoe<CapyPDF_OptionalContentGroupId> add_optional_content_group(const OptionalContentGroup &g);
 
     std::optional<double>
-    glyph_advance(CapyPdF_FontId fid, double pointsize, uint32_t codepoint) const;
+    glyph_advance(CapyPDF_FontId fid, double pointsize, uint32_t codepoint) const;
 
 private:
     PdfDocument(const PdfGenerationData &d, PdfColorConverter cm);
     rvoe<NoReturnValue> init();
 
     rvoe<NoReturnValue> write_to_file_impl();
 
     int32_t add_object(ObjectType object);
 
-    int32_t image_object_number(CapyPdF_ImageId iid) { return image_info.at(iid.id).obj; }
-    int32_t font_object_number(CapyPdF_FontId fid) { return font_objects.at(fid.id).font_obj; }
+    int32_t create_subnavigation(const std::vector<SubPageNavigation> &subnav);
+
+    int32_t image_object_number(CapyPDF_ImageId iid) { return image_info.at(iid.id).obj; }
+    int32_t font_object_number(CapyPDF_FontId fid) { return font_objects.at(fid.id).font_obj; }
     int32_t separation_object_number(SeparationId sid) { return separation_objects.at(sid.id); }
+    int32_t ocg_object_number(CapyPDF_OptionalContentGroupId ocgid) {
+        return ocg_items.at(ocgid.id);
+    }
 
-    std::optional<CapyPdF_IccColorSpaceId> find_icc_profile(std::string_view contents);
-    CapyPdF_IccColorSpaceId store_icc_profile(std::string_view contents, int32_t num_channels);
+    std::optional<CapyPDF_IccColorSpaceId> find_icc_profile(std::string_view contents);
+    CapyPDF_IccColorSpaceId store_icc_profile(std::string_view contents, int32_t num_channels);
 
     rvoe<std::vector<uint64_t>> write_objects();
 
     rvoe<NoReturnValue> create_catalog();
     void create_output_intent();
     rvoe<int32_t> create_name_dict();
     rvoe<int32_t> create_outlines();
@@ -375,52 +399,53 @@
                                           int32_t font_descriptor_obj,
                                           int32_t tounicode_obj);
     rvoe<NoReturnValue> write_checkbox_widget(int obj_num,
                                               const DelayedCheckboxWidgetAnnotation &checkbox);
     rvoe<NoReturnValue> write_annotation(int obj_num, const DelayedAnnotation &annotation);
     rvoe<NoReturnValue> write_delayed_structure_item(int obj_num, const DelayedStructItem &p);
 
-    rvoe<CapyPdF_ImageId> add_image_object(int32_t w,
+    rvoe<CapyPDF_ImageId> add_image_object(int32_t w,
                                            int32_t h,
                                            int32_t bits_per_component,
                                            ColorspaceType colorspace,
                                            std::optional<int32_t> smask_id,
                                            bool is_mask,
                                            std::string_view uncompressed_bytes);
 
-    rvoe<CapyPdF_ImageId> process_rgb_image(const rgb_image &image);
-    rvoe<CapyPdF_ImageId> process_gray_image(const gray_image &image);
-    rvoe<CapyPdF_ImageId> process_mono_image(const mono_image &image);
-    rvoe<CapyPdF_ImageId> process_cmyk_image(const cmyk_image &image);
+    rvoe<CapyPDF_ImageId> process_rgb_image(const rgb_image &image);
+    rvoe<CapyPDF_ImageId> process_gray_image(const gray_image &image);
+    rvoe<CapyPDF_ImageId> process_mono_image(const mono_image &image);
+    rvoe<CapyPDF_ImageId> process_cmyk_image(const cmyk_image &image);
 
     int32_t create_page_group();
     void pad_subset_fonts();
     void pad_subset_until_space(std::vector<TTGlyphs> &subset_glyphs);
 
     PdfGenerationData opts;
     PdfColorConverter cm;
     std::vector<ObjectType> document_objects;
     std::vector<PageOffsets> pages; // Refers to object num.
     std::vector<ImageInfo> image_info;
-    std::unordered_map<CapyPdF_Builtin_Fonts, CapyPdF_FontId> builtin_fonts;
+    std::unordered_map<CapyPDF_Builtin_Fonts, CapyPDF_FontId> builtin_fonts;
     std::vector<FontInfo> font_objects;
     std::vector<int32_t> separation_objects;
     std::vector<FontThingy> fonts;
     OutlineData outlines;
     std::vector<IccInfo> icc_profiles;
     std::vector<FormXObjectInfo> form_xobjects;
     std::vector<int32_t> form_widgets;
     std::vector<EmbeddedFileObject> embedded_files;
     std::vector<int32_t> annotations;
     std::vector<StructItem> structure_items;
+    std::vector<int32_t> ocg_items;
     // A form widget can be used on one and only one page.
-    std::unordered_map<CapyPdF_FormWidgetId, int32_t> form_use;
-    std::unordered_map<CapyPdF_AnnotationId, int32_t> annotation_use;
-    std::unordered_map<CapyPdF_StructureItemId, int32_t> structure_use;
-    std::optional<CapyPdF_IccColorSpaceId> output_profile;
+    std::unordered_map<CapyPDF_FormWidgetId, int32_t> form_use;
+    std::unordered_map<CapyPDF_AnnotationId, int32_t> annotation_use;
+    std::unordered_map<CapyPDF_StructureItemId, int32_t> structure_use;
+    std::optional<CapyPDF_IccColorSpaceId> output_profile;
     std::optional<int32_t> output_intent_object;
     std::optional<int32_t> structure_root_object;
     int32_t pages_object;
     int32_t page_group_object;
 
     FILE *ofile = nullptr;
 };
```

### Comparing `capypdf-0.3.0/src/pdfdrawcontext.cpp` & `capypdf-0.4.0/src/pdfdrawcontext.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #include <pdfdrawcontext.hpp>
 #include <pdfgen.hpp>
 #include <ft2build.h>
+#include <string_view>
 #include FT_FREETYPE_H
 #include FT_IMAGE_H
 #include <utils.hpp>
 #include <lcms2.h>
 #include <fmt/core.h>
 #include <array>
 #include <cmath>
@@ -86,15 +87,17 @@
     used_fonts.clear();
     used_colorspaces.clear();
     used_gstates.clear();
     used_shadings.clear();
     used_patterns.clear();
     used_widgets.clear();
     used_annotations.clear();
+    used_ocgs.clear();
     ind.clear();
+    sub_navigations.clear();
     transition.reset();
     is_finalized = false;
     uses_all_colorspace = false;
 }
 
 std::string PdfDrawContext::build_resource_dict() {
     std::string resources;
@@ -156,27 +159,35 @@
     if(!used_patterns.empty()) {
         resources += "  /Pattern <<\n";
         for(const auto &s : used_patterns) {
             fmt::format_to(resource_appender, "    /Pattern-{} {} 0 R\n", s, s);
         }
         resources += "  >>\n";
     }
+    if(!used_ocgs.empty()) {
+        resources += "  /Properties <<\n";
+        for(const auto &ocg : used_ocgs) {
+            auto objnum = doc->ocg_object_number(ocg);
+            fmt::format_to(resource_appender, "    /oc{} {} 0 R\n", objnum, objnum);
+        }
+        resources += "  >>\n";
+    }
     resources += ">>\n";
     return resources;
 }
 
-ErrorCode PdfDrawContext::add_form_widget(CapyPdF_FormWidgetId widget) {
+ErrorCode PdfDrawContext::add_form_widget(CapyPDF_FormWidgetId widget) {
     if(used_widgets.find(widget) != used_widgets.end()) {
         return ErrorCode::AnnotationReuse;
     }
     used_widgets.insert(widget);
     return ErrorCode::NoError;
 }
 
-ErrorCode PdfDrawContext::annotate(CapyPdF_AnnotationId annotation) {
+ErrorCode PdfDrawContext::annotate(CapyPDF_AnnotationId annotation) {
     if(used_annotations.find(annotation) != used_annotations.end()) {
         return ErrorCode::AnnotationReuse;
     }
     used_annotations.insert(annotation);
     return ErrorCode::NoError;
 }
 
@@ -205,28 +216,36 @@
 
 ErrorCode PdfDrawContext::cmd_Bstar() {
     commands += ind;
     commands += "B*\n";
     return ErrorCode::NoError;
 }
 
-ErrorCode PdfDrawContext::cmd_BDC(CapyPdF_StructureItemId sid) {
+ErrorCode PdfDrawContext::cmd_BDC(CapyPDF_StructureItemId sid) {
     ++marked_depth;
     used_structures.insert(sid);
     fmt::format_to(cmd_appender,
                    R"({}/P << /MCID {} >>
 {}BDC
 )",
                    ind,
                    sid.id,
                    ind);
     indent(DrawStateType::MarkedContent);
     return ErrorCode::NoError;
 }
 
+ErrorCode PdfDrawContext::cmd_BDC(CapyPDF_OptionalContentGroupId ocgid) {
+    ++marked_depth;
+    used_ocgs.insert(ocgid);
+    fmt::format_to(cmd_appender, "{}/OC /oc{} BDC\n", ind, doc->ocg_object_number(ocgid));
+    indent(DrawStateType::MarkedContent);
+    return ErrorCode::NoError;
+}
+
 ErrorCode PdfDrawContext::cmd_BMC(std::string_view tag) {
     if(tag.empty() || tag.front() != '/') {
         std::abort();
     }
     ++marked_depth;
     fmt::format_to(cmd_appender, "{}{} BMC\n", ind, tag);
     indent(DrawStateType::MarkedContent);
@@ -275,15 +294,15 @@
     for(size_t i = 0; i < dash_array_length; ++i) {
         fmt::format_to(cmd_appender, "{} ", dash_array[i]);
     }
     fmt::format_to(cmd_appender, " ] {} d\n", phase);
     return ErrorCode::NoError;
 }
 
-ErrorCode PdfDrawContext::cmd_Do(CapyPdF_FormXObjectId fxoid) {
+ErrorCode PdfDrawContext::cmd_Do(CapyPDF_FormXObjectId fxoid) {
     if(context_type != CAPY_DC_PAGE) {
         return ErrorCode::InvalidDrawContextType;
     }
     CHECK_INDEXNESS(fxoid.id, doc->form_xobjects);
     fmt::format_to(cmd_appender, "{}/FXO{} Do\n", ind, doc->form_xobjects[fxoid.id].xobj_num);
     used_form_xobjects.insert(doc->form_xobjects[fxoid.id].xobj_num);
     return ErrorCode::NoError;
@@ -432,15 +451,15 @@
     CHECK_COLORCOMPONENT(r);
     CHECK_COLORCOMPONENT(g);
     CHECK_COLORCOMPONENT(b);
     fmt::format_to(cmd_appender, "{}{} {} {} rg\n", ind, r, g, b);
     return ErrorCode::NoError;
 }
 
-ErrorCode PdfDrawContext::cmd_ri(CapyPdF_Rendering_Intent ri) {
+ErrorCode PdfDrawContext::cmd_ri(CapyPDF_Rendering_Intent ri) {
     CHECK_ENUM(ri, CAPY_RI_PERCEPTUAL);
     fmt::format_to(cmd_appender, "{}/{} ri\n", ind, rendering_intent_names.at((int)ri));
     return ErrorCode::NoError;
 }
 
 ErrorCode PdfDrawContext::cmd_s() {
     commands += ind;
@@ -467,15 +486,15 @@
 ErrorCode PdfDrawContext::cmd_sh(ShadingId shid) {
     CHECK_INDEXNESS(shid.id, doc->document_objects);
     used_shadings.insert(shid.id);
     fmt::format_to(cmd_appender, "{}/SH{} sh\n", ind, shid.id);
     return ErrorCode::NoError;
 }
 
-ErrorCode PdfDrawContext::cmd_Tr(CapyPdF_Text_Mode mode) {
+ErrorCode PdfDrawContext::cmd_Tr(CapyPDF_Text_Mode mode) {
     CHECK_ENUM(mode, CAPY_TEXT_CLIP);
     fmt::format_to(cmd_appender, "{}{} Tr\n", ind, (int)mode);
     return ErrorCode::NoError;
 }
 
 ErrorCode PdfDrawContext::cmd_v(double x2, double y2, double x3, double y3) {
     fmt::format_to(cmd_appender, "{}{} {} {} {} v\n", ind, x2, y2, x3, y3);
@@ -503,14 +522,37 @@
 }
 
 ErrorCode PdfDrawContext::cmd_y(double x1, double y1, double x3, double y3) {
     fmt::format_to(cmd_appender, "{}{} {} {} {} y\n", ind, x1, y1, x3, y3);
     return ErrorCode::NoError;
 }
 
+ErrorCode PdfDrawContext::set_stroke_color(const Color &c) {
+    if(std::holds_alternative<DeviceRGBColor>(c)) {
+        return set_stroke_color(std::get<DeviceRGBColor>(c));
+    } else if(std::holds_alternative<DeviceGrayColor>(c)) {
+        return set_stroke_color(std::get<DeviceGrayColor>(c));
+    } else {
+        // Implement the rest later.
+        std::abort();
+    }
+    return ErrorCode::NoError;
+}
+
+ErrorCode PdfDrawContext::set_nonstroke_color(const Color &c) {
+    if(std::holds_alternative<DeviceRGBColor>(c)) {
+        return set_nonstroke_color(std::get<DeviceRGBColor>(c));
+    } else if(std::holds_alternative<DeviceGrayColor>(c)) {
+        return set_nonstroke_color(std::get<DeviceGrayColor>(c));
+    } else {
+        std::abort();
+    }
+    return ErrorCode::NoError;
+}
+
 ErrorCode PdfDrawContext::set_stroke_color(const DeviceRGBColor &c) {
     switch(doc->opts.output_colorspace) {
     case CAPYPDF_CS_DEVICE_RGB: {
         cmd_RG(c.r.v(), c.g.v(), c.b.v());
         break;
     }
     case CAPYPDF_CS_DEVICE_GRAY: {
@@ -527,15 +569,15 @@
         return cmyk_var.error();
         break;
     }
     }
     return ErrorCode::NoError;
 }
 
-ErrorCode PdfDrawContext::set_nonstroke_color(CapyPdF_IccColorSpaceId icc_id,
+ErrorCode PdfDrawContext::set_nonstroke_color(CapyPDF_IccColorSpaceId icc_id,
                                               const double *values,
                                               int32_t num_values) {
     CHECK_INDEXNESS(icc_id.id, doc->icc_profiles);
     const auto &icc_info = doc->icc_profiles.at(icc_id.id);
     if(icc_info.num_channels != num_values) {
         return ErrorCode::IncorrectColorChannelCount;
     }
@@ -544,15 +586,15 @@
     for(int32_t i = 0; i < num_values; ++i) {
         fmt::format_to(cmd_appender, "{:} ", values[i]);
     }
     fmt::format_to(cmd_appender, "scn\n", icc_info.object_num);
     return ErrorCode::NoError;
 }
 
-ErrorCode PdfDrawContext::set_stroke_color(CapyPdF_IccColorSpaceId icc_id,
+ErrorCode PdfDrawContext::set_stroke_color(CapyPDF_IccColorSpaceId icc_id,
                                            const double *values,
                                            int32_t num_values) {
     CHECK_INDEXNESS(icc_id.id, doc->icc_profiles);
     const auto &icc_info = doc->icc_profiles.at(icc_id.id);
     if(icc_info.num_channels != num_values) {
         return ErrorCode::IncorrectColorChannelCount;
     }
@@ -622,39 +664,39 @@
     used_colorspaces.insert(idnum);
     std::string csname = fmt::format("/CSpace{}", idnum);
     cmd_cs(csname);
     cmd_scn(value.v());
     return ErrorCode::NoError;
 }
 
-ErrorCode PdfDrawContext::set_stroke_color(LabId lid, const LabColor &c) {
-    CHECK_INDEXNESS(lid.id, doc->document_objects);
-    used_colorspaces.insert(lid.id);
-    std::string csname = fmt::format("/CSpace{}", lid.id);
+ErrorCode PdfDrawContext::set_stroke_color(const LabColor &c) {
+    CHECK_INDEXNESS(c.id.id, doc->document_objects);
+    used_colorspaces.insert(c.id.id);
+    std::string csname = fmt::format("/CSpace{}", c.id.id);
     cmd_CS(csname);
     fmt::format_to(cmd_appender, "{}{:f} {:f} {:f} SCN\n", ind, c.l, c.a, c.b);
     return ErrorCode::NoError;
 }
 
-ErrorCode PdfDrawContext::set_nonstroke_color(LabId lid, const LabColor &c) {
-    CHECK_INDEXNESS(lid.id, doc->document_objects);
-    used_colorspaces.insert(lid.id);
-    std::string csname = fmt::format("/CSpace{}", lid.id);
+ErrorCode PdfDrawContext::set_nonstroke_color(const LabColor &c) {
+    CHECK_INDEXNESS(c.id.id, doc->document_objects);
+    used_colorspaces.insert(c.id.id);
+    std::string csname = fmt::format("/CSpace{}", c.id.id);
     cmd_cs(csname);
     fmt::format_to(cmd_appender, "{}{:f} {:f} {:f} scn\n", ind, c.l, c.a, c.b);
     return ErrorCode::NoError;
 }
 
 void PdfDrawContext::set_all_stroke_color() {
     uses_all_colorspace = true;
     cmd_CS("/All");
     cmd_SCN(1.0);
 }
 
-ErrorCode PdfDrawContext::draw_image(CapyPdF_ImageId im_id) {
+ErrorCode PdfDrawContext::draw_image(CapyPDF_ImageId im_id) {
     CHECK_INDEXNESS(im_id.id, doc->image_info);
     auto obj_num = doc->image_object_number(im_id);
     used_images.insert(obj_num);
     fmt::format_to(cmd_appender, "{}/Image{} Do\n", ind, obj_num);
     return ErrorCode::NoError;
 }
 
@@ -663,25 +705,25 @@
 void PdfDrawContext::translate(double xtran, double ytran) { cmd_cm(1.0, 0, 0, 1.0, xtran, ytran); }
 
 void PdfDrawContext::rotate(double angle) {
     cmd_cm(cos(angle), sin(angle), -sin(angle), cos(angle), 0.0, 0.0);
 }
 
 ErrorCode PdfDrawContext::render_utf8_text(
-    std::string_view text, CapyPdF_FontId fid, double pointsize, double x, double y) {
+    std::string_view text, CapyPDF_FontId fid, double pointsize, double x, double y) {
     PdfText t;
     t.cmd_Tf(fid, pointsize);
     t.cmd_Td(x, y);
     t.render_text(text);
     return render_text(t);
 }
 
 rvoe<NoReturnValue> PdfDrawContext::serialize_charsequence(const std::vector<CharItem> &charseq,
                                                            std::string &serialisation,
-                                                           CapyPdF_FontId &current_font,
+                                                           CapyPDF_FontId &current_font,
                                                            int32_t &current_subset,
                                                            double &current_pointsize) {
     std::back_insert_iterator<std::string> app = std::back_inserter(serialisation);
     bool is_first = true;
     for(const auto &e : charseq) {
         if(std::holds_alternative<double>(e)) {
             if(is_first) {
@@ -719,15 +761,15 @@
     }
     serialisation += "] TJ\n";
     return NoReturnValue{};
 }
 
 ErrorCode PdfDrawContext::utf8_to_kerned_chars(std::string_view utf8_text,
                                                std::vector<CharItem> &charseq,
-                                               CapyPdF_FontId fid) {
+                                               CapyPDF_FontId fid) {
     CHECK_INDEXNESS(fid.id, doc->font_objects);
     if(utf8_text.empty()) {
         return ErrorCode::NoError;
     }
     FT_Face face = doc->fonts.at(doc->font_objects.at(fid.id).font_index_tmp).fontdata.face.get();
     if(!face) {
         return ErrorCode::BuiltinFontNotSupported;
@@ -762,15 +804,15 @@
 }
 
 ErrorCode PdfDrawContext::render_text(const PdfText &textobj) {
     std::string serialisation{ind + "BT\n"};
     indent(DrawStateType::Text);
     std::back_insert_iterator<std::string> app = std::back_inserter(serialisation);
     int32_t current_subset{-1};
-    CapyPdF_FontId current_font{-1};
+    CapyPDF_FontId current_font{-1};
     double current_pointsize{-1};
     for(const auto &e : textobj.get_events()) {
         if(std::holds_alternative<TStar_arg>(e)) {
             serialisation += ind;
             serialisation += "T*\n";
         } else if(std::holds_alternative<Tc_arg>(e)) {
             const auto &tc = std::get<Tc_arg>(e);
@@ -816,42 +858,52 @@
             fmt::format_to(app, "{}{} Ts\n", ind, ts.rise);
         } else if(std::holds_alternative<Tw_arg>(e)) {
             const auto &tw = std::get<Tw_arg>(e);
             fmt::format_to(app, "{}{} Tw\n", ind, tw.width);
         } else if(std::holds_alternative<Tz_arg>(e)) {
             const auto &tz = std::get<Tz_arg>(e);
             fmt::format_to(app, "{}{} Tz\n", ind, tz.scaling);
-        } else if(std::holds_alternative<CapyPdF_StructureItemId>(e)) {
-            const auto &sid = std::get<CapyPdF_StructureItemId>(e);
+        } else if(std::holds_alternative<CapyPDF_StructureItemId>(e)) {
+            const auto &sid = std::get<CapyPDF_StructureItemId>(e);
             used_structures.insert(sid);
             fmt::format_to(app, "{}/P << /MCID {} >>\n{}BDC\n", ind, sid.id, ind);
             indent(DrawStateType::MarkedContent);
         } else if(std::holds_alternative<Emc_arg>(e)) {
             auto rc = dedent(DrawStateType::MarkedContent);
             if(!rc) {
                 return rc.error();
             }
             fmt::format_to(app, "{}EMC\n", ind);
+        } else if(std::holds_alternative<Stroke_arg>(e)) {
+            // const auto &sarg = std::get<Stroke_arg>(e);
+            std::abort();
+        } else if(std::holds_alternative<Nonstroke_arg>(e)) {
+            // FIXME: make a function to create color commands
+            // as text and use that here and in the actual set_X_color methods.
+            const auto &nsarg = std::get<Nonstroke_arg>(e);
+            assert(std::holds_alternative<DeviceRGBColor>(nsarg.c));
+            auto &rgb = std::get<DeviceRGBColor>(nsarg.c);
+            fmt::format_to(app, "{}{} {} {} rg\n", ind, rgb.r.v(), rgb.g.v(), rgb.b.v());
         } else {
-            fprintf(stderr, "Not implemented yet.\n");
+            fprintf(stderr, "Text feature implemented yet.\n");
             std::abort();
         }
     }
     auto rc = dedent(DrawStateType::Text);
     if(!rc) {
         return rc.error();
     }
     serialisation += ind;
     serialisation += "ET\n";
     commands += serialisation;
     return ErrorCode::NoError;
 }
 
 void PdfDrawContext::render_raw_glyph(
-    uint32_t glyph, CapyPdF_FontId fid, double pointsize, double x, double y) {
+    uint32_t glyph, CapyPDF_FontId fid, double pointsize, double x, double y) {
     auto &font_data = doc->font_objects.at(fid.id);
     // used_fonts.insert(font_data.font_obj);
 
     const auto font_glyph_id = doc->glyph_for_codepoint(
         doc->fonts.at(font_data.font_index_tmp).fontdata.face.get(), glyph);
     fmt::format_to(cmd_appender,
                    R"({}BT
@@ -869,15 +921,15 @@
                    y,
                    ind,
                    font_glyph_id,
                    ind);
 }
 
 ErrorCode PdfDrawContext::render_glyphs(const std::vector<PdfGlyph> &glyphs,
-                                        CapyPdF_FontId fid,
+                                        CapyPDF_FontId fid,
                                         double pointsize) {
     CHECK_INDEXNESS(fid.id, doc->font_objects);
     double prev_x = 0;
     double prev_y = 0;
     if(glyphs.empty()) {
         return ErrorCode::NoError;
     }
@@ -909,15 +961,15 @@
             cmd_appender, "  <{:02x}> Tj\n", (unsigned char)current_subset_glyph.glyph_id);
     }
     fmt::format_to(cmd_appender, "{}ET\n", ind);
     return ErrorCode::NoError;
 }
 
 ErrorCode PdfDrawContext::render_pdfdoc_text_builtin(const char *pdfdoc_encoded_text,
-                                                     CapyPdF_Builtin_Fonts font_id,
+                                                     CapyPDF_Builtin_Fonts font_id,
                                                      double pointsize,
                                                      double x,
                                                      double y) {
     if(doc->opts.subtype) {
         return ErrorCode::BadOperationForIntent;
     }
     auto font_object = doc->font_object_number(doc->get_builtin_font_id(font_id));
@@ -949,16 +1001,36 @@
     cmd_c(0.5, -control, control, -0.5, 0, -0.5);
     cmd_c(-control, -0.5, -0.5, -control, -0.5, 0);
     cmd_c(-0.5, control, -control, 0.5, 0, 0.5);
 }
 
 void PdfDrawContext::draw_unit_box() { cmd_re(-0.5, -0.5, 1, 1); }
 
-rvoe<NoReturnValue> PdfDrawContext::set_transition(const PageTransition &tr) {
+rvoe<NoReturnValue> PdfDrawContext::set_transition(const Transition &tr) {
     if(context_type != CAPY_DC_PAGE) {
         RETERR(InvalidDrawContextType);
     }
     transition = tr;
     return NoReturnValue{};
 }
 
+rvoe<NoReturnValue>
+PdfDrawContext::add_simple_navigation(std::span<const CapyPDF_OptionalContentGroupId> navs,
+                                      const std::optional<Transition> &tr) {
+    if(context_type != CAPY_DC_PAGE) {
+        RETERR(InvalidDrawContextType);
+    }
+    if(!sub_navigations.empty()) {
+        std::abort();
+    }
+    for(const auto &sn : navs) {
+        if(used_ocgs.find(sn) == used_ocgs.end()) {
+            RETERR(UnusedOcg);
+        }
+    }
+    for(const auto &sn : navs) {
+        sub_navigations.emplace_back(SubPageNavigation{sn, tr});
+    }
+    return NoReturnValue();
+}
+
 } // namespace capypdf
```

### Comparing `capypdf-0.3.0/src/pdfdrawcontext.hpp` & `capypdf-0.4.0/src/pdfdrawcontext.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 #include <pdfcommon.hpp>
 #include <pdftext.hpp>
 #include <errorhandling.hpp>
 #include <pdfcolorconverter.hpp>
 #include <pdfdocument.hpp>
 #include <string>
+#include <string_view>
 #include <unordered_set>
 #include <vector>
 #include <optional>
 #include <span>
 #include <stack>
 
 template<> struct std::hash<capypdf::FontSubset> {
@@ -93,22 +94,23 @@
     // All methods that begin with cmd_ map directly to the PDF primitive with the same name.
 
     // They are in the same order as in Annex A of the PDF spec.
     ErrorCode cmd_b();
     ErrorCode cmd_B();
     ErrorCode cmd_bstar();
     ErrorCode cmd_Bstar();
-    ErrorCode cmd_BDC(CapyPdF_StructureItemId sid);
+    ErrorCode cmd_BDC(CapyPDF_StructureItemId sid);
+    ErrorCode cmd_BDC(CapyPDF_OptionalContentGroupId id);
     ErrorCode cmd_BMC(std::string_view tag);
     ErrorCode cmd_c(double x1, double y1, double x2, double y2, double x3, double y3);
     ErrorCode cmd_cm(double m1, double m2, double m3, double m4, double m5, double m6);
     ErrorCode cmd_CS(std::string_view cspace_name);
     ErrorCode cmd_cs(std::string_view cspace_name);
     ErrorCode cmd_d(double *dash_array, size_t dash_array_length, double phase);
-    ErrorCode cmd_Do(CapyPdF_FormXObjectId fxoid);
+    ErrorCode cmd_Do(CapyPDF_FormXObjectId fxoid);
     ErrorCode cmd_EMC();
     ErrorCode cmd_f();
     // ErrorCode cmd_F(); PDF spec says this is obsolete.
     ErrorCode cmd_fstar();
     ErrorCode cmd_G(double gray);
     ErrorCode cmd_g(double gray);
     ErrorCode cmd_gs(GstateId id);
@@ -123,99 +125,107 @@
     ErrorCode cmd_M(double miterlimit);
     ErrorCode cmd_n();
     ErrorCode cmd_q(); // Save
     ErrorCode cmd_Q(); // Restore
     ErrorCode cmd_re(double x, double y, double w, double h);
     ErrorCode cmd_RG(double r, double g, double b);
     ErrorCode cmd_rg(double r, double g, double b);
-    ErrorCode cmd_ri(CapyPdF_Rendering_Intent ri);
+    ErrorCode cmd_ri(CapyPDF_Rendering_Intent ri);
     ErrorCode cmd_s();
     ErrorCode cmd_S();
     ErrorCode cmd_SCN(double value);
     ErrorCode cmd_scn(double value);
     ErrorCode cmd_sh(ShadingId shid);
-    ErrorCode cmd_Tr(CapyPdF_Text_Mode mode);
+    ErrorCode cmd_Tr(CapyPDF_Text_Mode mode);
     ErrorCode cmd_v(double x2, double y2, double x3, double y3);
     ErrorCode cmd_w(double w);
     ErrorCode cmd_W();
     ErrorCode cmd_Wstar();
     ErrorCode cmd_y(double x1, double y1, double x3, double y3);
 
+    ErrorCode set_stroke_color(const Color &c);
+    ErrorCode set_nonstroke_color(const Color &c);
+
     ErrorCode set_stroke_color(const DeviceRGBColor &c);
     ErrorCode set_nonstroke_color(const DeviceRGBColor &c);
-    ErrorCode set_stroke_color(LabId lid, const LabColor &c);
+    ErrorCode set_stroke_color(const LabColor &c);
     ErrorCode
-    set_stroke_color(CapyPdF_IccColorSpaceId icc_id, const double *values, int32_t num_values);
-    ErrorCode set_nonstroke_color(LabId lid, const LabColor &c);
+    set_stroke_color(CapyPDF_IccColorSpaceId icc_id, const double *values, int32_t num_values);
+    ErrorCode set_nonstroke_color(const LabColor &c);
     ErrorCode set_nonstroke_color(const DeviceGrayColor &c);
     ErrorCode set_nonstroke_color(PatternId id);
     ErrorCode
-    set_nonstroke_color(CapyPdF_IccColorSpaceId icc_id, const double *values, int32_t num_values);
+    set_nonstroke_color(CapyPDF_IccColorSpaceId icc_id, const double *values, int32_t num_values);
     ErrorCode set_separation_stroke_color(SeparationId id, LimitDouble value);
     ErrorCode set_separation_nonstroke_color(SeparationId id, LimitDouble value);
     void set_all_stroke_color();
-    ErrorCode draw_image(CapyPdF_ImageId obj_num);
+    ErrorCode draw_image(CapyPDF_ImageId obj_num);
     void scale(double xscale, double yscale);
     void translate(double xtran, double ytran);
     void rotate(double angle);
     ErrorCode render_utf8_text(
-        std::string_view text, CapyPdF_FontId fid, double pointsize, double x, double y);
+        std::string_view text, CapyPDF_FontId fid, double pointsize, double x, double y);
     ErrorCode render_text(const PdfText &textobj);
-    void render_raw_glyph(uint32_t glyph, CapyPdF_FontId fid, double pointsize, double x, double y);
+    void render_raw_glyph(uint32_t glyph, CapyPDF_FontId fid, double pointsize, double x, double y);
     ErrorCode
-    render_glyphs(const std::vector<PdfGlyph> &glyphs, CapyPdF_FontId fid, double pointsize);
+    render_glyphs(const std::vector<PdfGlyph> &glyphs, CapyPDF_FontId fid, double pointsize);
     ErrorCode render_pdfdoc_text_builtin(const char *pdfdoc_encoded_text,
-                                         CapyPdF_Builtin_Fonts font_id,
+                                         CapyPDF_Builtin_Fonts font_id,
                                          double pointsize,
                                          double x,
                                          double y);
 
     void draw_unit_circle();
     void draw_unit_box();
 
     void clear();
 
-    ErrorCode add_form_widget(CapyPdF_FormWidgetId widget);
-    ErrorCode annotate(CapyPdF_AnnotationId annotation);
+    ErrorCode add_form_widget(CapyPDF_FormWidgetId widget);
+    ErrorCode annotate(CapyPDF_AnnotationId annotation);
 
     CAPYPDF_Draw_Context_Type draw_context_type() const { return context_type; }
     PdfDocument &get_doc() { return *doc; }
 
     std::string build_resource_dict();
     std::string_view get_command_stream() { return commands; }
 
     void set_form_xobject_size(double w, double h);
     double get_form_xobj_w() const { return form_xobj_w; }
     double get_form_xobj_h() const { return form_xobj_h; }
 
     int32_t marked_content_depth() const { return marked_depth; }
 
-    const std::unordered_set<CapyPdF_FormWidgetId> &get_form_usage() const { return used_widgets; }
-    const std::unordered_set<CapyPdF_AnnotationId> &get_annotation_usage() const {
+    const std::unordered_set<CapyPDF_FormWidgetId> &get_form_usage() const { return used_widgets; }
+    const std::unordered_set<CapyPDF_AnnotationId> &get_annotation_usage() const {
         return used_annotations;
     }
-    const std::unordered_set<CapyPdF_StructureItemId> &get_structure_usage() const {
+    const std::unordered_set<CapyPDF_StructureItemId> &get_structure_usage() const {
         return used_structures;
     }
 
-    const std::optional<PageTransition> &get_transition() const { return transition; }
+    const std::optional<Transition> &get_transition() const { return transition; }
+
+    const std::vector<SubPageNavigation> &get_subpage_navigation() const { return sub_navigations; }
 
     bool has_unclosed_state() const { return !dstates.empty(); }
 
-    rvoe<NoReturnValue> set_transition(const PageTransition &tr);
+    rvoe<NoReturnValue> set_transition(const Transition &tr);
+
+    rvoe<NoReturnValue> add_simple_navigation(std::span<const CapyPDF_OptionalContentGroupId> navs,
+                                              const std::optional<Transition> &tr);
 
 private:
     rvoe<NoReturnValue> serialize_charsequence(const std::vector<CharItem> &charseq,
                                                std::string &serialisation,
-                                               CapyPdF_FontId &current_font,
+                                               CapyPDF_FontId &current_font,
                                                int32_t &current_subset,
                                                double &current_pointsize);
     ErrorCode utf8_to_kerned_chars(std::string_view utf8_text,
                                    std::vector<CharItem> &charseq,
-                                   CapyPdF_FontId fid);
+                                   CapyPDF_FontId fid);
 
     void indent(DrawStateType dtype) {
         dstates.push(dtype);
         ind += "  ";
     }
 
     rvoe<NoReturnValue> dedent(DrawStateType dtype) {
@@ -243,19 +253,22 @@
     std::unordered_set<FontSubset> used_subset_fonts;
     std::unordered_set<int32_t> used_fonts;
     std::unordered_set<int32_t> used_colorspaces;
     std::unordered_set<int32_t> used_gstates;
     std::unordered_set<int32_t> used_shadings;
     std::unordered_set<int32_t> used_patterns;
     std::unordered_set<int32_t> used_form_xobjects;
-    std::unordered_set<CapyPdF_FormWidgetId> used_widgets;
-    std::unordered_set<CapyPdF_AnnotationId> used_annotations;
-    std::unordered_set<CapyPdF_StructureItemId> used_structures;
+    std::unordered_set<CapyPDF_FormWidgetId> used_widgets;
+    std::unordered_set<CapyPDF_AnnotationId> used_annotations;
+    std::unordered_set<CapyPDF_StructureItemId> used_structures;
+    std::unordered_set<CapyPDF_OptionalContentGroupId> used_ocgs;
+    std::vector<SubPageNavigation> sub_navigations;
+
     std::stack<DrawStateType> dstates;
-    std::optional<PageTransition> transition;
+    std::optional<Transition> transition;
     // Reminder: If you add stuff  here, also add them to .clear().
     bool is_finalized = false;
     bool uses_all_colorspace = false;
     double form_xobj_w = -1;
     double form_xobj_h = -1;
     int32_t marked_depth = 0;
     std::string ind;
```

### Comparing `capypdf-0.3.0/src/pdfgen.cpp` & `capypdf-0.4.0/src/pdfgen.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -53,27 +53,27 @@
         break;
     }
     default:
         std::abort();
     }
 }
 
-rvoe<std::unique_ptr<PdfGen>> PdfGen::construct(const char *ofname, const PdfGenerationData &d) {
+rvoe<std::unique_ptr<PdfGen>> PdfGen::construct(const std::filesystem::path &ofname,
+                                                const PdfGenerationData &d) {
     FT_Library ft_;
     auto error = FT_Init_FreeType(&ft_);
     if(error) {
         RETERR(FreeTypeError);
     }
     std::unique_ptr<FT_LibraryRec_, FT_Error (*)(FT_LibraryRec_ *)> ft(ft_, FT_Done_FreeType);
-    std::filesystem::path opath(ofname);
     ERC(cm,
         PdfColorConverter::construct(
             d.prof.rgb_profile_file, d.prof.gray_profile_file, d.prof.cmyk_profile_file));
     ERC(pdoc, PdfDocument::construct(d, std::move(cm)));
-    return std::unique_ptr<PdfGen>(new PdfGen(std::move(opath), std::move(ft), std::move(pdoc)));
+    return std::unique_ptr<PdfGen>(new PdfGen(ofname, std::move(ft), std::move(pdoc)));
 }
 
 PdfGen::~PdfGen() {
     pdoc.font_objects.clear();
     pdoc.fonts.clear();
 }
 
@@ -148,34 +148,35 @@
     assert(std::holds_alternative<SerializedBasicContext>(sc_var));
     auto &sc = std::get<SerializedBasicContext>(sc_var);
     ERCV(pdoc.add_page(std::move(sc.dict),
                        std::move(sc.commands),
                        ctx.get_form_usage(),
                        ctx.get_annotation_usage(),
                        ctx.get_structure_usage(),
-                       ctx.get_transition()));
+                       ctx.get_transition(),
+                       ctx.get_subpage_navigation()));
     ctx.clear();
     return PageId{(int32_t)pdoc.pages.size() - 1};
 }
 
-rvoe<CapyPdF_FormXObjectId> PdfGen::add_form_xobject(PdfDrawContext &ctx) {
+rvoe<CapyPDF_FormXObjectId> PdfGen::add_form_xobject(PdfDrawContext &ctx) {
     if(ctx.draw_context_type() != CAPY_DC_FORM_XOBJECT) {
         RETERR(InvalidDrawContextType);
     }
     if(ctx.marked_content_depth() != 0) {
         RETERR(UnclosedMarkedContent);
     }
     auto sc_var = ctx.serialize();
     assert(std::holds_alternative<SerializedXObject>(sc_var));
     auto &sc = std::get<SerializedXObject>(sc_var);
     pdoc.add_form_xobject(std::move(sc.dict), std::move(sc.stream));
     ctx.clear();
-    CapyPdF_FormXObjectId fxoid;
+    CapyPDF_FormXObjectId fxoid;
     fxoid.id = (int32_t)pdoc.form_xobjects.size() - 1;
-    return rvoe<CapyPdF_FormXObjectId>{fxoid};
+    return rvoe<CapyPDF_FormXObjectId>{fxoid};
 }
 
 rvoe<PatternId> PdfGen::add_pattern(ColorPatternBuilder &cp) {
     if(cp.pctx.draw_context_type() != CAPY_DC_COLOR_TILING) {
         RETERR(InvalidDrawContextType);
     }
     if(cp.pctx.marked_content_depth() != 0) {
@@ -216,15 +217,15 @@
 }
 
 ColorPatternBuilder PdfGen::new_color_pattern_builder(double w, double h) {
     return ColorPatternBuilder{PdfDrawContext{&pdoc, &pdoc.cm, CAPY_DC_COLOR_TILING}, w, h};
 }
 
 rvoe<double>
-PdfGen::utf8_text_width(const char *utf8_text, CapyPdF_FontId fid, double pointsize) const {
+PdfGen::utf8_text_width(const char *utf8_text, CapyPDF_FontId fid, double pointsize) const {
     if(utf8_text[0] == '\0') {
         return 0;
     }
     double w = 0;
     FT_Face face = pdoc.fonts.at(pdoc.font_objects.at(fid.id).font_index_tmp).fontdata.face.get();
     if(!face) {
         RETERR(BuiltinFontNotSupported);
```

### Comparing `capypdf-0.3.0/src/pdfgen.hpp` & `capypdf-0.4.0/src/pdfgen.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -44,113 +44,119 @@
     DrawContextPopper(const DrawContextPopper &) = delete;
 
     ~DrawContextPopper();
 };
 
 class PdfGen {
 public:
-    static rvoe<std::unique_ptr<PdfGen>> construct(const char *ofname, const PdfGenerationData &d);
+    static rvoe<std::unique_ptr<PdfGen>> construct(const std::filesystem::path &ofname,
+                                                   const PdfGenerationData &d);
     PdfGen(PdfGen &&o) = default;
     ~PdfGen();
 
     rvoe<NoReturnValue> write();
-    void new_page();
 
-    rvoe<CapyPdF_ImageId> load_image(const std::filesystem::path &fname) {
+    rvoe<CapyPDF_ImageId> load_image(const std::filesystem::path &fname) {
         return pdoc.load_image(fname);
     }
-    rvoe<CapyPdF_ImageId> load_mask_image(const std::filesystem::path &fname) {
+    rvoe<CapyPDF_ImageId> load_mask_image(const std::filesystem::path &fname) {
         return pdoc.load_mask_image(fname);
     }
-    rvoe<CapyPdF_ImageId> embed_jpg(const std::filesystem::path &fname) {
+    rvoe<CapyPDF_ImageId> embed_jpg(const std::filesystem::path &fname) {
         return pdoc.embed_jpg(fname);
     }
-    rvoe<CapyPdF_EmbeddedFileId> embed_file(const std::filesystem::path &fname) {
+    rvoe<CapyPDF_EmbeddedFileId> embed_file(const std::filesystem::path &fname) {
         return pdoc.embed_file(fname);
     }
-    rvoe<CapyPdF_FontId> load_font(const std::filesystem::path &fname) {
+    rvoe<CapyPDF_FontId> load_font(const std::filesystem::path &fname) {
         return pdoc.load_font(ft.get(), fname);
     };
 
-    ImageSize get_image_info(CapyPdF_ImageId img_id) { return pdoc.image_info.at(img_id.id).s; }
+    ImageSize get_image_info(CapyPDF_ImageId img_id) { return pdoc.image_info.at(img_id.id).s; }
     SeparationId create_separation(std::string_view name, const DeviceCMYKColor &fallback) {
         return pdoc.create_separation(name, fallback);
     }
     GstateId add_graphics_state(const GraphicsState &state) {
         return pdoc.add_graphics_state(state);
     }
 
     FunctionId add_function(const FunctionType2 &func) { return pdoc.add_function(func); }
 
     ShadingId add_shading(const ShadingType2 &shade) { return pdoc.add_shading(shade); }
     ShadingId add_shading(const ShadingType3 &shade) { return pdoc.add_shading(shade); }
+    ShadingId add_shading(const ShadingType4 &shade) { return pdoc.add_shading(shade); }
+    ShadingId add_shading(const ShadingType6 &shade) { return pdoc.add_shading(shade); }
 
     LabId add_lab_colorspace(const LabColorSpace &lab) { return pdoc.add_lab_colorspace(lab); }
 
-    rvoe<CapyPdF_IccColorSpaceId> load_icc_file(const char *fname) {
+    rvoe<CapyPDF_IccColorSpaceId> load_icc_file(const std::filesystem::path &fname) {
         return pdoc.load_icc_file(fname);
     }
 
-    rvoe<CapyPdF_FormWidgetId> create_form_checkbox(PdfBox loc,
-                                                    CapyPdF_FormXObjectId onstate,
-                                                    CapyPdF_FormXObjectId offstate,
+    rvoe<CapyPDF_FormWidgetId> create_form_checkbox(PdfBox loc,
+                                                    CapyPDF_FormXObjectId onstate,
+                                                    CapyPDF_FormXObjectId offstate,
                                                     std::string_view partial_name) {
         return pdoc.create_form_checkbox(loc, onstate, offstate, partial_name);
     }
 
-    rvoe<CapyPdF_AnnotationId> create_annotation(PdfRectangle rect, AnnotationSubType subtype) {
+    rvoe<CapyPDF_AnnotationId> create_annotation(PdfRectangle rect, AnnotationSubType subtype) {
         return pdoc.create_annotation(rect, std::move(subtype));
     }
 
     DrawContextPopper guarded_page_context();
     PdfDrawContext *new_page_draw_context();
 
     PdfDrawContext new_form_xobject(double w, double h) {
         return PdfDrawContext(&this->pdoc, &pdoc.cm, CAPY_DC_FORM_XOBJECT, w, h);
     }
 
     ColorPatternBuilder new_color_pattern_builder(double w, double h);
 
     rvoe<PageId> add_page(PdfDrawContext &ctx);
-    rvoe<CapyPdF_FormXObjectId> add_form_xobject(PdfDrawContext &ctx);
+    rvoe<CapyPDF_FormXObjectId> add_form_xobject(PdfDrawContext &ctx);
     rvoe<PatternId> add_pattern(ColorPatternBuilder &cp);
 
     OutlineId
     add_outline(std::string_view title_utf8, PageId dest, std::optional<OutlineId> parent) {
         return pdoc.add_outline(title_utf8, dest, parent);
     }
 
-    rvoe<CapyPdF_StructureItemId>
-    add_structure_item(std::string_view stype, std::optional<CapyPdF_StructureItemId> parent) {
+    rvoe<CapyPDF_StructureItemId>
+    add_structure_item(std::string_view stype, std::optional<CapyPDF_StructureItemId> parent) {
         return pdoc.add_structure_item(stype, parent);
     }
 
+    rvoe<CapyPDF_OptionalContentGroupId> add_optional_content_group(const OptionalContentGroup &g) {
+        return pdoc.add_optional_content_group(g);
+    }
+
     int32_t num_pages() const { return (int32_t)pdoc.pages.size(); }
 
     std::optional<double>
-    glyph_advance(CapyPdF_FontId fid, double pointsize, uint32_t codepoint) const {
+    glyph_advance(CapyPDF_FontId fid, double pointsize, uint32_t codepoint) const {
         return pdoc.glyph_advance(fid, pointsize, codepoint);
     }
 
-    rvoe<double> utf8_text_width(const char *utf8_text, CapyPdF_FontId fid, double pointsize) const;
+    rvoe<double> utf8_text_width(const char *utf8_text, CapyPDF_FontId fid, double pointsize) const;
 
 private:
     PdfGen(std::filesystem::path ofilename,
            std::unique_ptr<FT_LibraryRec_, FT_Error (*)(FT_LibraryRec_ *)> ft,
            PdfDocument pdoc)
         : ofilename(std::move(ofilename)), ft(std::move(ft)), pdoc(std::move(pdoc)) {}
 
     std::filesystem::path ofilename;
     std::unique_ptr<FT_LibraryRec_, FT_Error (*)(FT_LibraryRec_ *)> ft;
     PdfDocument pdoc;
 };
 
 struct GenPopper {
     std::unique_ptr<PdfGen> g;
-    GenPopper(const char *ofname, const PdfGenerationData &d) : g() {
+    GenPopper(const std::filesystem::path &ofname, const PdfGenerationData &d) : g() {
         auto rc = PdfGen::construct(ofname, d);
         if(!rc) {
             fprintf(stderr, "%s\n", error_text(rc.error()));
             std::abort();
         }
         g = std::move(rc.value());
     }
```

### Comparing `capypdf-0.3.0/src/pdfparser.cpp` & `capypdf-0.4.0/src/pdfparser.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/pdfparser.hpp` & `capypdf-0.4.0/src/pdfparser.hpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/pdftext.hpp` & `capypdf-0.4.0/src/pdftext.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 };
 
 struct TD_arg {
     double tx, ty;
 };
 
 struct Tf_arg {
-    CapyPdF_FontId font;
+    CapyPDF_FontId font;
     double pointsize;
 };
 
 struct Text_arg {
     std::string utf8_text;
 };
 
@@ -59,15 +59,15 @@
 };
 
 struct Tm_arg {
     double a, b, c, d, e, f;
 };
 
 struct Tr_arg {
-    CapyPdF_Text_Mode rmode;
+    CapyPDF_Text_Mode rmode;
 };
 
 struct Ts_arg {
     double rise;
 };
 
 struct Tw_arg {
@@ -76,36 +76,46 @@
 
 struct Tz_arg {
     double scaling;
 };
 
 struct Emc_arg {};
 
+struct Stroke_arg {
+    Color c;
+};
+
+struct Nonstroke_arg {
+    Color c;
+};
+
 typedef std::variant<TStar_arg,
                      Tc_arg,
                      Td_arg,
                      TD_arg,
                      Tf_arg,
                      Text_arg,
                      TJ_arg,
                      TL_arg,
                      Tm_arg,
                      Tr_arg,
                      Ts_arg,
                      Tw_arg,
                      Tz_arg,
-                     CapyPdF_StructureItemId,
-                     Emc_arg>
+                     CapyPDF_StructureItemId,
+                     Emc_arg,
+                     Stroke_arg,
+                     Nonstroke_arg>
     TextEvent;
 
 class PdfText {
 public:
     PdfText(){};
 
-    ErrorCode cmd_BDC(CapyPdF_StructureItemId sid) {
+    ErrorCode cmd_BDC(CapyPDF_StructureItemId sid) {
         events.emplace_back(sid);
         return ErrorCode::NoError;
     }
 
     ErrorCode cmd_EMC() {
         events.emplace_back(Emc_arg{});
         return ErrorCode::NoError;
@@ -127,15 +137,15 @@
     }
 
     ErrorCode cmd_TD(double tx, double ty) {
         events.emplace_back(TD_arg{tx, ty});
         return ErrorCode::NoError;
     }
 
-    ErrorCode cmd_Tf(CapyPdF_FontId font, double pointsize) {
+    ErrorCode cmd_Tf(CapyPDF_FontId font, double pointsize) {
         events.emplace_back(Tf_arg{font, pointsize});
         return ErrorCode::NoError;
     }
 
     ErrorCode render_text(std::string_view utf8_text) {
         events.emplace_back(Text_arg{std::string{utf8_text}});
         return ErrorCode::NoError;
@@ -154,15 +164,15 @@
     }
 
     ErrorCode cmd_TM(double a, double b, double c, double d, double e, double f) {
         events.emplace_back(Tm_arg{a, b, c, d, e, f});
         return ErrorCode::NoError;
     }
 
-    ErrorCode cmd_Tr(CapyPdF_Text_Mode rmode) {
+    ErrorCode cmd_Tr(CapyPDF_Text_Mode rmode) {
         events.emplace_back(Tr_arg{rmode});
         return ErrorCode::NoError;
     }
 
     ErrorCode cmd_Ts(double rise) {
         events.emplace_back(Ts_arg{rise});
         return ErrorCode::NoError;
@@ -174,14 +184,24 @@
     }
 
     ErrorCode cmd_Tz(double scaling) {
         events.emplace_back(Tz_arg{scaling});
         return ErrorCode::NoError;
     }
 
+    ErrorCode stroke_color(const Color &c) {
+        events.emplace_back(Stroke_arg{c});
+        return ErrorCode::NoError;
+    }
+
+    ErrorCode nonstroke_color(const Color &c) {
+        events.emplace_back(Nonstroke_arg{c});
+        return ErrorCode::NoError;
+    }
+
     const std::vector<TextEvent> &get_events() const { return events; }
 
 private:
     std::vector<TextEvent> events;
 };
 
 } // namespace capypdf
```

### Comparing `capypdf-0.3.0/src/pdfviewer.cpp` & `capypdf-0.4.0/src/pdfviewer.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/tifftest.cpp` & `capypdf-0.4.0/src/tifftest.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/utils.cpp` & `capypdf-0.4.0/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/src/utils.hpp` & `capypdf-0.4.0/src/utils.hpp`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/subprojects/fmt.wrap` & `capypdf-0.4.0/subprojects/fmt.wrap`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/subprojects/libjpeg-turbo.wrap` & `capypdf-0.4.0/subprojects/libjpeg-turbo.wrap`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/subprojects/libpng.wrap` & `capypdf-0.4.0/subprojects/libpng.wrap`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/subprojects/zlib.wrap` & `capypdf-0.4.0/subprojects/zlib.wrap`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/test/capypdftests.py` & `capypdf-0.4.0/test/capypdftests.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                 ctx.cmd_rg(1.0, 0.0, 0.0)
                 ctx.cmd_re(10, 10, 100, 100)
                 ctx.cmd_f()
 
     @validate_image('python_text', 400, 400)
     def test_text(self, ofilename, w, h):
         opts = capypdf.Options()
-        opts.set_mediabox(0, 0, w, h)
+        opts.set_pagebox(capypdf.PageBox.Media, 0, 0, w, h)
         with capypdf.Generator(ofilename, opts) as g:
             fid = g.load_font(noto_fontdir / 'NotoSans-Regular.ttf')
             with g.page_draw_context() as ctx:
                 ctx.render_text('Av, Tv, kerning yo.', fid, 12, 50, 150)
 
     def test_error(self):
         ofile = pathlib.Path('delme.pdf')
@@ -133,15 +133,15 @@
                 ctx.cmd_J(capypdf.LineCapStyle.Round)
                 ctx.cmd_j(capypdf.LineJoinStyle.Bevel)
         ofile.unlink()
 
     @validate_image('python_image', 200, 200)
     def test_images(self, ofilename, w, h):
         opts = capypdf.Options()
-        opts.set_mediabox(0, 0, w, h)
+        opts.set_pagebox(capypdf.PageBox.Media, 0, 0, w, h)
         with capypdf.Generator(ofilename, opts) as g:
             bg_img = g.embed_jpg(image_dir / 'simple.jpg')
             mono_img = g.load_image(image_dir / '1bit_noalpha.png')
             gray_img = g.load_image(image_dir / 'gray_alpha.png')
             with g.page_draw_context() as ctx:
                 with ctx.push_gstate():
                     ctx.translate(10, 10)
@@ -156,15 +156,15 @@
                     ctx.translate(110, 110)
                     ctx.scale(80, 80)
                     ctx.draw_image(gray_img)
 
     @validate_image('python_path', 200, 200)
     def test_path(self, ofilename, w, h):
         opts = capypdf.Options()
-        opts.set_mediabox(0, 0, w, h)
+        opts.set_pagebox(capypdf.PageBox.Media, 0, 0, w, h)
         with capypdf.Generator(ofilename, opts) as g:
             with g.page_draw_context() as ctx:
                 with ctx.push_gstate():
                     ctx.cmd_w(5)
                     ctx.cmd_J(capypdf.LineCapStyle.Round)
                     ctx.cmd_m(10, 10);
                     ctx.cmd_c(80, 10, 20, 90, 90, 90);
@@ -195,46 +195,46 @@
                     ctx.cmd_RG(0.5, 0.1, 0.5)
                     draw_intersect_shape(ctx)
                     ctx.cmd_Bstar()
 
     @validate_image('python_textobj', 200, 200)
     def test_text(self, ofilename, w, h):
         opts = capypdf.Options()
-        opts.set_mediabox(0, 0, w, h)
+        opts.set_pagebox(capypdf.PageBox.Media, 0, 0, w, h)
         with capypdf.Generator(ofilename, opts) as g:
             font = g.load_font(noto_fontdir / 'NotoSerif-Regular.ttf')
             with g.page_draw_context() as ctx:
                 t = capypdf.Text()
                 t.cmd_Tf(font, 12.0)
                 t.cmd_Td(10.0, 100.0)
                 t.render_text('Using text object!')
                 ctx.render_text_obj(t)
 
     @validate_image('python_icccolor', 200, 200)
     def test_icc(self, ofilename, w, h):
         opts = capypdf.Options()
-        opts.set_mediabox(0, 0, w, h)
+        opts.set_pagebox(capypdf.PageBox.Media, 0, 0, w, h)
         with capypdf.Generator(ofilename, opts) as g:
             cs = g.load_icc_profile('/usr/share/color/icc/colord/AdobeRGB1998.icc')
             with g.page_draw_context() as ctx:
                 ctx.set_icc_stroke(cs, [0.1, 0.2, 0.8])
                 ctx.set_icc_nonstroke(cs, [0.7, 0.2, 0.6])
                 ctx.cmd_w(2)
                 ctx.cmd_re(10, 10, 80, 80)
                 ctx.cmd_B()
 
     @cleanup('transitions.pdf')
     def test_transitions(self, ofilename):
         opts = capypdf.Options()
-        opts.set_mediabox(0, 0, 160, 90)
+        opts.set_pagebox(capypdf.PageBox.Media, 0, 0, 160, 90)
         with capypdf.Generator(ofilename, opts) as g:
             with g.page_draw_context() as ctx:
                 pass
             with g.page_draw_context() as ctx:
-                tr = capypdf.PageTransition(capypdf.PageTransitionType.Blinds, 1.0)
+                tr = capypdf.Transition(capypdf.TransitionType.Blinds, 1.0)
                 ctx.set_page_transition(tr)
                 ctx.cmd_rg(0.5, 0.5, 0.5)
                 ctx.cmd_re(0, 0, 160, 90)
                 ctx.cmd_f()
 
 
 if __name__ == "__main__":
```

### Comparing `capypdf-0.3.0/test/ctest.c` & `capypdf-0.4.0/test/ctest.c`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,16 @@
  */
 
 #include <capypdf.h>
 #include <stdio.h>
 
 int main() {
     CAPYPDF_EC rc;
-    CapyPdF_Generator *gen;
-    CapyPdF_Options *opt;
+    CapyPDF_Generator *gen;
+    CapyPDF_Options *opt;
 
     if((rc = capy_options_new(&opt)) != 0) {
         fprintf(stderr, "%s\n", capy_error_message(rc));
         return 1;
     }
 
     if((rc = capy_generator_new("dummy.pdf", opt, &gen)) != 0) {
```

### Comparing `capypdf-0.3.0/testoutput/python_icccolor.png` & `capypdf-0.4.0/testoutput/python_icccolor.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/testoutput/python_image.png` & `capypdf-0.4.0/testoutput/python_image.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/testoutput/python_path.png` & `capypdf-0.4.0/testoutput/python_path.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/testoutput/python_simple.png` & `capypdf-0.4.0/testoutput/python_simple.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/testoutput/python_text.png` & `capypdf-0.4.0/testoutput/python_text.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/testoutput/python_textobj.png` & `capypdf-0.4.0/testoutput/python_textobj.png`

 * *Files identical despite different names*

### Comparing `capypdf-0.3.0/PKG-INFO` & `capypdf-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capypdf
-Version: 0.3.0
+Version: 0.4.0
 Summary: A color managed PDF generation library tech preview
 Author-Email: Jussi Pakkanen <jpakkane@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,15 +209,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C++
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# A4PDF
+# CapyPDF
 
 This is a library for generating PDF files. It aims to be very low level.
 It does not have its own document model, it merely exposes PDF primitives
 directly.
 
 ## Features
```

