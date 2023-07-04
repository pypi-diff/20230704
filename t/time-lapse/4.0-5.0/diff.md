# Comparing `tmp/time_lapse-4.0.tar.gz` & `tmp/time_lapse-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_lapse-4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "time_lapse-5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `time_lapse-4.0.tar` & `time_lapse-5.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0      274 2022-01-17 10:30:52.246163 time_lapse-4.0/.editorconfig
--rw-r--r--   0        0        0      250 2023-06-23 06:58:58.776606 time_lapse-4.0/.github/dependabot.yml
--rw-r--r--   0        0        0      432 2022-12-16 18:40:51.232478 time_lapse-4.0/.github/workflows/demo.yml
--rw-r--r--   0        0        0      983 2023-06-16 15:03:59.334837 time_lapse-4.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0       72 2022-01-17 10:30:52.246658 time_lapse-4.0/.gitignore
--rw-r--r--   0        0        0     1069 2022-01-17 10:30:52.246784 time_lapse-4.0/LICENSE
--rw-r--r--   0        0        0      781 2023-06-16 15:03:59.335188 time_lapse-4.0/Makefile
--rw-r--r--   0        0        0     3972 2022-12-16 18:40:51.288312 time_lapse-4.0/README.md
--rw-r--r--   0        0        0      106 2022-01-17 10:30:52.247371 time_lapse-4.0/demo/Makefile
--rw-r--r--   0        0        0    47653 2022-01-17 10:30:52.247772 time_lapse-4.0/demo/source/S60_050504_181349.jpg
--rw-r--r--   0        0        0    47989 2022-01-17 10:30:52.248224 time_lapse-4.0/demo/source/S60_050504_181449.jpg
--rw-r--r--   0        0        0    48213 2022-01-17 10:30:52.248657 time_lapse-4.0/demo/source/S60_050504_181549.jpg
--rw-r--r--   0        0        0    48206 2022-01-17 10:30:52.249109 time_lapse-4.0/demo/source/S60_050504_181649.jpg
--rw-r--r--   0        0        0    48291 2022-01-17 10:30:52.249544 time_lapse-4.0/demo/source/S60_050504_181749.jpg
--rw-r--r--   0        0        0    48140 2022-01-17 10:30:52.249879 time_lapse-4.0/demo/source/S60_050504_181849.jpg
--rw-r--r--   0        0        0    48733 2022-01-17 10:30:52.250320 time_lapse-4.0/demo/source/S60_050504_181949.jpg
--rw-r--r--   0        0        0    49385 2022-01-17 10:30:52.250787 time_lapse-4.0/demo/source/S60_050504_182049.jpg
--rw-r--r--   0        0        0    49778 2022-01-17 10:30:52.251132 time_lapse-4.0/demo/source/S60_050504_182149.jpg
--rw-r--r--   0        0        0    50554 2022-01-17 10:30:52.251491 time_lapse-4.0/demo/source/S60_050504_182249.jpg
--rw-r--r--   0        0        0    51313 2022-01-17 10:30:52.252097 time_lapse-4.0/demo/source/S60_050504_182349.jpg
--rw-r--r--   0        0        0    51550 2022-01-17 10:30:52.252669 time_lapse-4.0/demo/source/S60_050504_182449.jpg
--rw-r--r--   0        0        0    51972 2022-01-17 10:30:52.253049 time_lapse-4.0/demo/source/S60_050504_182549.jpg
--rw-r--r--   0        0        0    52344 2022-01-17 10:30:52.253503 time_lapse-4.0/demo/source/S60_050504_182649.jpg
--rw-r--r--   0        0        0    52423 2022-01-17 10:30:52.253818 time_lapse-4.0/demo/source/S60_050504_182749.jpg
--rw-r--r--   0        0        0    52739 2022-01-17 10:30:52.254242 time_lapse-4.0/demo/source/S60_050504_182849.jpg
--rw-r--r--   0        0        0    52795 2022-01-17 10:30:52.254679 time_lapse-4.0/demo/source/S60_050504_182949.jpg
--rw-r--r--   0        0        0    52615 2022-01-17 10:30:52.255101 time_lapse-4.0/demo/source/S60_050504_183049.jpg
--rw-r--r--   0        0        0    52194 2022-01-17 10:30:52.255424 time_lapse-4.0/demo/source/S60_050504_183149.jpg
--rw-r--r--   0        0        0    51880 2022-01-17 10:30:52.255828 time_lapse-4.0/demo/source/S60_050504_183249.jpg
--rw-r--r--   0        0        0    52125 2022-01-17 10:30:52.256144 time_lapse-4.0/demo/source/S60_050504_183349.jpg
--rw-r--r--   0        0        0    52215 2022-01-17 10:30:52.256552 time_lapse-4.0/demo/source/S60_050504_183449.jpg
--rw-r--r--   0        0        0    52445 2022-01-17 10:30:52.256862 time_lapse-4.0/demo/source/S60_050504_183549.jpg
--rw-r--r--   0        0        0    52529 2022-01-17 10:30:52.257276 time_lapse-4.0/demo/source/S60_050504_183649.jpg
--rw-r--r--   0        0        0    52935 2022-01-17 10:30:52.257600 time_lapse-4.0/demo/source/S60_050504_183749.jpg
--rw-r--r--   0        0        0    52965 2022-01-17 10:30:52.257930 time_lapse-4.0/demo/source/S60_050504_184017.jpg
--rw-r--r--   0        0        0    52445 2022-01-17 10:30:52.258247 time_lapse-4.0/demo/source/S60_050504_184117.jpg
--rw-r--r--   0        0        0    52212 2022-01-17 10:30:52.258555 time_lapse-4.0/demo/source/S60_050504_184217.jpg
--rw-r--r--   0        0        0    52202 2022-01-17 10:30:52.258963 time_lapse-4.0/demo/source/S60_050504_184317.jpg
--rw-r--r--   0        0        0    51929 2022-01-17 10:30:52.259366 time_lapse-4.0/demo/source/S60_050504_184417.jpg
--rw-r--r--   0        0        0    52125 2022-01-17 10:30:52.259678 time_lapse-4.0/demo/source/S60_050504_184517.jpg
--rw-r--r--   0        0        0    51591 2022-01-17 10:30:52.259984 time_lapse-4.0/demo/source/S60_050504_184617.jpg
--rw-r--r--   0        0        0    51855 2022-01-17 10:30:52.260285 time_lapse-4.0/demo/source/S60_050504_184717.jpg
--rw-r--r--   0        0        0    51873 2022-01-17 10:30:52.260580 time_lapse-4.0/demo/source/S60_050504_184817.jpg
--rw-r--r--   0        0        0    52124 2022-01-17 10:30:52.260883 time_lapse-4.0/demo/source/S60_050504_184917.jpg
--rw-r--r--   0        0        0    52149 2022-01-17 10:30:52.261183 time_lapse-4.0/demo/source/S60_050504_185017.jpg
--rw-r--r--   0        0        0    51641 2022-01-17 10:30:52.261451 time_lapse-4.0/demo/source/S60_050504_185117.jpg
--rw-r--r--   0        0        0    52029 2022-01-17 10:30:52.261786 time_lapse-4.0/demo/source/S60_050504_185217.jpg
--rw-r--r--   0        0        0    52155 2022-01-17 10:30:52.262164 time_lapse-4.0/demo/source/S60_050504_185317.jpg
--rw-r--r--   0        0        0    51904 2022-01-17 10:30:52.262459 time_lapse-4.0/demo/source/S60_050504_185417.jpg
--rw-r--r--   0        0        0    51874 2022-01-17 10:30:52.262749 time_lapse-4.0/demo/source/S60_050504_185517.jpg
--rw-r--r--   0        0        0    52336 2022-01-17 10:30:52.263016 time_lapse-4.0/demo/source/S60_050504_185617.jpg
--rw-r--r--   0        0        0    52336 2022-01-17 10:30:52.263278 time_lapse-4.0/demo/source/S60_050504_185717.jpg
--rw-r--r--   0        0        0    51972 2022-01-17 10:30:52.263557 time_lapse-4.0/demo/source/S60_050504_185817.jpg
--rw-r--r--   0        0        0    51917 2022-01-17 10:30:52.263837 time_lapse-4.0/demo/source/S60_050504_185917.jpg
--rw-r--r--   0        0        0    51871 2022-01-17 10:30:52.264111 time_lapse-4.0/demo/source/S60_050504_190017.jpg
--rw-r--r--   0        0        0    52177 2022-01-17 10:30:52.264378 time_lapse-4.0/demo/source/S60_050504_190117.jpg
--rw-r--r--   0        0        0    52092 2022-01-17 10:30:52.264649 time_lapse-4.0/demo/source/S60_050504_190217.jpg
--rw-r--r--   0        0        0    51864 2022-01-17 10:30:52.264925 time_lapse-4.0/demo/source/S60_050504_190317.jpg
--rw-r--r--   0        0        0    52200 2022-01-17 10:30:52.265199 time_lapse-4.0/demo/source/S60_050504_190417.jpg
--rw-r--r--   0        0        0    51954 2022-01-17 10:30:52.265462 time_lapse-4.0/demo/source/S60_050504_190517.jpg
--rw-r--r--   0        0        0    52033 2022-01-17 10:30:52.265730 time_lapse-4.0/demo/source/S60_050504_190617.jpg
--rw-r--r--   0        0        0    52688 2022-01-17 10:30:52.265994 time_lapse-4.0/demo/source/S60_050504_190717.jpg
--rw-r--r--   0        0        0    52338 2022-01-17 10:30:52.266273 time_lapse-4.0/demo/source/S60_050504_190817.jpg
--rw-r--r--   0        0        0    52243 2022-01-17 10:30:52.266545 time_lapse-4.0/demo/source/S60_050504_190917.jpg
--rw-r--r--   0        0        0    52578 2022-01-17 10:30:52.266809 time_lapse-4.0/demo/source/S60_050504_191017.jpg
--rw-r--r--   0        0        0    53033 2022-01-17 10:30:52.267093 time_lapse-4.0/demo/source/S60_050504_191117.jpg
--rw-r--r--   0        0        0    52802 2022-01-17 10:30:52.267357 time_lapse-4.0/demo/source/S60_050504_191217.jpg
--rw-r--r--   0        0        0    52858 2022-01-17 10:30:52.267639 time_lapse-4.0/demo/source/S60_050504_191417.jpg
--rw-r--r--   0        0        0    52802 2022-01-17 10:30:52.267922 time_lapse-4.0/demo/source/S60_050504_191517.jpg
--rw-r--r--   0        0        0    52941 2022-01-17 10:30:52.268192 time_lapse-4.0/demo/source/S60_050504_191617.jpg
--rw-r--r--   0        0        0    52973 2022-01-17 10:30:52.268468 time_lapse-4.0/demo/source/S60_050504_191717.jpg
--rw-r--r--   0        0        0    53037 2022-01-17 10:30:52.268760 time_lapse-4.0/demo/source/S60_050504_191817.jpg
--rw-r--r--   0        0        0    52912 2022-01-17 10:30:52.269032 time_lapse-4.0/demo/source/S60_050504_191917.jpg
--rw-r--r--   0        0        0    52819 2022-01-17 10:30:52.269288 time_lapse-4.0/demo/source/S60_050504_192017.jpg
--rw-r--r--   0        0        0    53355 2022-01-17 10:30:52.269541 time_lapse-4.0/demo/source/S60_050504_192117.jpg
--rw-r--r--   0        0        0    53243 2022-01-17 10:30:52.269788 time_lapse-4.0/demo/source/S60_050504_192217.jpg
--rw-r--r--   0        0        0    53250 2022-01-17 10:30:52.270037 time_lapse-4.0/demo/source/S60_050504_192317.jpg
--rw-r--r--   0        0        0    53299 2022-01-17 10:30:52.270277 time_lapse-4.0/demo/source/S60_050504_192417.jpg
--rw-r--r--   0        0        0    53519 2022-01-17 10:30:52.270532 time_lapse-4.0/demo/source/S60_050504_192517.jpg
--rw-r--r--   0        0        0     2538 2023-06-24 13:07:45.049828 time_lapse-4.0/pyproject.toml
--rw-r--r--   0        0        0       14 2023-06-23 13:01:19.764663 time_lapse-4.0/requirements-ruff.txt
--rw-r--r--   0        0        0        0 2022-01-17 10:30:52.274345 time_lapse-4.0/tests/__init__.py
--rw-r--r--   0        0        0       61 2022-01-17 10:30:52.274470 time_lapse-4.0/time_lapse/__init__.py
--rw-r--r--   0        0        0     3629 2023-06-16 15:03:59.335692 time_lapse-4.0/time_lapse/check_interval.py
--rw-r--r--   0        0        0     1834 2023-06-16 15:14:40.513817 time_lapse-4.0/time_lapse/cli.py
--rw-r--r--   0        0        0      306 2023-06-16 15:03:59.336314 time_lapse-4.0/time_lapse/detect_audio.py
--rwxr-xr-x   0        0        0    98228 2022-01-17 10:30:52.275448 time_lapse-4.0/time_lapse/fonts/Jost-400-Book.ttf
--rwxr-xr-x   0        0        0     3627 2022-01-17 10:30:52.275875 time_lapse-4.0/time_lapse/fonts/LICENSE.md
--rw-r--r--   0        0        0     2271 2023-06-16 15:03:59.336503 time_lapse-4.0/time_lapse/output.py
--rw-r--r--   0        0        0        0 2023-06-16 15:03:59.336545 time_lapse-4.0/time_lapse/py.typed
--rw-r--r--   0        0        0     1131 2023-06-16 15:03:59.336751 time_lapse-4.0/time_lapse/source.py
--rw-r--r--   0        0        0      693 2023-06-16 15:03:59.336913 time_lapse-4.0/time_lapse/watermark.py
--rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 time_lapse-4.0/PKG-INFO
+-rw-r--r--   0        0        0      274 2022-01-17 10:30:52.246163 time_lapse-5.0/.editorconfig
+-rw-r--r--   0        0        0      250 2023-06-23 06:58:58.776606 time_lapse-5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      432 2022-12-16 18:40:51.232478 time_lapse-5.0/.github/workflows/demo.yml
+-rw-r--r--   0        0        0      987 2023-07-04 13:50:47.863337 time_lapse-5.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       72 2022-01-17 10:30:52.246658 time_lapse-5.0/.gitignore
+-rw-r--r--   0        0        0     1069 2022-01-17 10:30:52.246784 time_lapse-5.0/LICENSE
+-rw-r--r--   0        0        0      618 2023-07-04 15:16:02.013777 time_lapse-5.0/Makefile
+-rw-r--r--   0        0        0     3986 2023-07-04 14:42:57.635402 time_lapse-5.0/README.md
+-rw-r--r--   0        0        0      106 2022-01-17 10:30:52.247371 time_lapse-5.0/demo/Makefile
+-rw-r--r--   0        0        0    47653 2022-01-17 10:30:52.247772 time_lapse-5.0/demo/source/S60_050504_181349.jpg
+-rw-r--r--   0        0        0    47989 2022-01-17 10:30:52.248224 time_lapse-5.0/demo/source/S60_050504_181449.jpg
+-rw-r--r--   0        0        0    48213 2022-01-17 10:30:52.248657 time_lapse-5.0/demo/source/S60_050504_181549.jpg
+-rw-r--r--   0        0        0    48206 2022-01-17 10:30:52.249109 time_lapse-5.0/demo/source/S60_050504_181649.jpg
+-rw-r--r--   0        0        0    48291 2022-01-17 10:30:52.249544 time_lapse-5.0/demo/source/S60_050504_181749.jpg
+-rw-r--r--   0        0        0    48140 2022-01-17 10:30:52.249879 time_lapse-5.0/demo/source/S60_050504_181849.jpg
+-rw-r--r--   0        0        0    48733 2022-01-17 10:30:52.250320 time_lapse-5.0/demo/source/S60_050504_181949.jpg
+-rw-r--r--   0        0        0    49385 2022-01-17 10:30:52.250787 time_lapse-5.0/demo/source/S60_050504_182049.jpg
+-rw-r--r--   0        0        0    49778 2022-01-17 10:30:52.251132 time_lapse-5.0/demo/source/S60_050504_182149.jpg
+-rw-r--r--   0        0        0    50554 2022-01-17 10:30:52.251491 time_lapse-5.0/demo/source/S60_050504_182249.jpg
+-rw-r--r--   0        0        0    51313 2022-01-17 10:30:52.252097 time_lapse-5.0/demo/source/S60_050504_182349.jpg
+-rw-r--r--   0        0        0    51550 2022-01-17 10:30:52.252669 time_lapse-5.0/demo/source/S60_050504_182449.jpg
+-rw-r--r--   0        0        0    51972 2022-01-17 10:30:52.253049 time_lapse-5.0/demo/source/S60_050504_182549.jpg
+-rw-r--r--   0        0        0    52344 2022-01-17 10:30:52.253503 time_lapse-5.0/demo/source/S60_050504_182649.jpg
+-rw-r--r--   0        0        0    52423 2022-01-17 10:30:52.253818 time_lapse-5.0/demo/source/S60_050504_182749.jpg
+-rw-r--r--   0        0        0    52739 2022-01-17 10:30:52.254242 time_lapse-5.0/demo/source/S60_050504_182849.jpg
+-rw-r--r--   0        0        0    52795 2022-01-17 10:30:52.254679 time_lapse-5.0/demo/source/S60_050504_182949.jpg
+-rw-r--r--   0        0        0    52615 2022-01-17 10:30:52.255101 time_lapse-5.0/demo/source/S60_050504_183049.jpg
+-rw-r--r--   0        0        0    52194 2022-01-17 10:30:52.255424 time_lapse-5.0/demo/source/S60_050504_183149.jpg
+-rw-r--r--   0        0        0    51880 2022-01-17 10:30:52.255828 time_lapse-5.0/demo/source/S60_050504_183249.jpg
+-rw-r--r--   0        0        0    52125 2022-01-17 10:30:52.256144 time_lapse-5.0/demo/source/S60_050504_183349.jpg
+-rw-r--r--   0        0        0    52215 2022-01-17 10:30:52.256552 time_lapse-5.0/demo/source/S60_050504_183449.jpg
+-rw-r--r--   0        0        0    52445 2022-01-17 10:30:52.256862 time_lapse-5.0/demo/source/S60_050504_183549.jpg
+-rw-r--r--   0        0        0    52529 2022-01-17 10:30:52.257276 time_lapse-5.0/demo/source/S60_050504_183649.jpg
+-rw-r--r--   0        0        0    52935 2022-01-17 10:30:52.257600 time_lapse-5.0/demo/source/S60_050504_183749.jpg
+-rw-r--r--   0        0        0    52965 2022-01-17 10:30:52.257930 time_lapse-5.0/demo/source/S60_050504_184017.jpg
+-rw-r--r--   0        0        0    52445 2022-01-17 10:30:52.258247 time_lapse-5.0/demo/source/S60_050504_184117.jpg
+-rw-r--r--   0        0        0    52212 2022-01-17 10:30:52.258555 time_lapse-5.0/demo/source/S60_050504_184217.jpg
+-rw-r--r--   0        0        0    52202 2022-01-17 10:30:52.258963 time_lapse-5.0/demo/source/S60_050504_184317.jpg
+-rw-r--r--   0        0        0    51929 2022-01-17 10:30:52.259366 time_lapse-5.0/demo/source/S60_050504_184417.jpg
+-rw-r--r--   0        0        0    52125 2022-01-17 10:30:52.259678 time_lapse-5.0/demo/source/S60_050504_184517.jpg
+-rw-r--r--   0        0        0    51591 2022-01-17 10:30:52.259984 time_lapse-5.0/demo/source/S60_050504_184617.jpg
+-rw-r--r--   0        0        0    51855 2022-01-17 10:30:52.260285 time_lapse-5.0/demo/source/S60_050504_184717.jpg
+-rw-r--r--   0        0        0    51873 2022-01-17 10:30:52.260580 time_lapse-5.0/demo/source/S60_050504_184817.jpg
+-rw-r--r--   0        0        0    52124 2022-01-17 10:30:52.260883 time_lapse-5.0/demo/source/S60_050504_184917.jpg
+-rw-r--r--   0        0        0    52149 2022-01-17 10:30:52.261183 time_lapse-5.0/demo/source/S60_050504_185017.jpg
+-rw-r--r--   0        0        0    51641 2022-01-17 10:30:52.261451 time_lapse-5.0/demo/source/S60_050504_185117.jpg
+-rw-r--r--   0        0        0    52029 2022-01-17 10:30:52.261786 time_lapse-5.0/demo/source/S60_050504_185217.jpg
+-rw-r--r--   0        0        0    52155 2022-01-17 10:30:52.262164 time_lapse-5.0/demo/source/S60_050504_185317.jpg
+-rw-r--r--   0        0        0    51904 2022-01-17 10:30:52.262459 time_lapse-5.0/demo/source/S60_050504_185417.jpg
+-rw-r--r--   0        0        0    51874 2022-01-17 10:30:52.262749 time_lapse-5.0/demo/source/S60_050504_185517.jpg
+-rw-r--r--   0        0        0    52336 2022-01-17 10:30:52.263016 time_lapse-5.0/demo/source/S60_050504_185617.jpg
+-rw-r--r--   0        0        0    52336 2022-01-17 10:30:52.263278 time_lapse-5.0/demo/source/S60_050504_185717.jpg
+-rw-r--r--   0        0        0    51972 2022-01-17 10:30:52.263557 time_lapse-5.0/demo/source/S60_050504_185817.jpg
+-rw-r--r--   0        0        0    51917 2022-01-17 10:30:52.263837 time_lapse-5.0/demo/source/S60_050504_185917.jpg
+-rw-r--r--   0        0        0    51871 2022-01-17 10:30:52.264111 time_lapse-5.0/demo/source/S60_050504_190017.jpg
+-rw-r--r--   0        0        0    52177 2022-01-17 10:30:52.264378 time_lapse-5.0/demo/source/S60_050504_190117.jpg
+-rw-r--r--   0        0        0    52092 2022-01-17 10:30:52.264649 time_lapse-5.0/demo/source/S60_050504_190217.jpg
+-rw-r--r--   0        0        0    51864 2022-01-17 10:30:52.264925 time_lapse-5.0/demo/source/S60_050504_190317.jpg
+-rw-r--r--   0        0        0    52200 2022-01-17 10:30:52.265199 time_lapse-5.0/demo/source/S60_050504_190417.jpg
+-rw-r--r--   0        0        0    51954 2022-01-17 10:30:52.265462 time_lapse-5.0/demo/source/S60_050504_190517.jpg
+-rw-r--r--   0        0        0    52033 2022-01-17 10:30:52.265730 time_lapse-5.0/demo/source/S60_050504_190617.jpg
+-rw-r--r--   0        0        0    52688 2022-01-17 10:30:52.265994 time_lapse-5.0/demo/source/S60_050504_190717.jpg
+-rw-r--r--   0        0        0    52338 2022-01-17 10:30:52.266273 time_lapse-5.0/demo/source/S60_050504_190817.jpg
+-rw-r--r--   0        0        0    52243 2022-01-17 10:30:52.266545 time_lapse-5.0/demo/source/S60_050504_190917.jpg
+-rw-r--r--   0        0        0    52578 2022-01-17 10:30:52.266809 time_lapse-5.0/demo/source/S60_050504_191017.jpg
+-rw-r--r--   0        0        0    53033 2022-01-17 10:30:52.267093 time_lapse-5.0/demo/source/S60_050504_191117.jpg
+-rw-r--r--   0        0        0    52802 2022-01-17 10:30:52.267357 time_lapse-5.0/demo/source/S60_050504_191217.jpg
+-rw-r--r--   0        0        0    52858 2022-01-17 10:30:52.267639 time_lapse-5.0/demo/source/S60_050504_191417.jpg
+-rw-r--r--   0        0        0    52802 2022-01-17 10:30:52.267922 time_lapse-5.0/demo/source/S60_050504_191517.jpg
+-rw-r--r--   0        0        0    52941 2022-01-17 10:30:52.268192 time_lapse-5.0/demo/source/S60_050504_191617.jpg
+-rw-r--r--   0        0        0    52973 2022-01-17 10:30:52.268468 time_lapse-5.0/demo/source/S60_050504_191717.jpg
+-rw-r--r--   0        0        0    53037 2022-01-17 10:30:52.268760 time_lapse-5.0/demo/source/S60_050504_191817.jpg
+-rw-r--r--   0        0        0    52912 2022-01-17 10:30:52.269032 time_lapse-5.0/demo/source/S60_050504_191917.jpg
+-rw-r--r--   0        0        0    52819 2022-01-17 10:30:52.269288 time_lapse-5.0/demo/source/S60_050504_192017.jpg
+-rw-r--r--   0        0        0    53355 2022-01-17 10:30:52.269541 time_lapse-5.0/demo/source/S60_050504_192117.jpg
+-rw-r--r--   0        0        0    53243 2022-01-17 10:30:52.269788 time_lapse-5.0/demo/source/S60_050504_192217.jpg
+-rw-r--r--   0        0        0    53250 2022-01-17 10:30:52.270037 time_lapse-5.0/demo/source/S60_050504_192317.jpg
+-rw-r--r--   0        0        0    53299 2022-01-17 10:30:52.270277 time_lapse-5.0/demo/source/S60_050504_192417.jpg
+-rw-r--r--   0        0        0    53519 2022-01-17 10:30:52.270532 time_lapse-5.0/demo/source/S60_050504_192517.jpg
+-rw-r--r--   0        0        0     2784 2023-07-04 15:14:56.425562 time_lapse-5.0/pyproject.toml
+-rw-r--r--   0        0        0       14 2023-06-23 13:01:19.764663 time_lapse-5.0/requirements-ruff.txt
+-rw-r--r--   0        0        0        0 2022-01-17 10:30:52.274345 time_lapse-5.0/tests/__init__.py
+-rw-r--r--   0        0        0       61 2022-01-17 10:30:52.274470 time_lapse-5.0/time_lapse/__init__.py
+-rw-r--r--   0        0        0     3629 2023-06-16 15:03:59.335692 time_lapse-5.0/time_lapse/check_interval.py
+-rw-r--r--   0        0        0     1847 2023-07-04 14:32:12.927031 time_lapse-5.0/time_lapse/cli.py
+-rw-r--r--   0        0        0      306 2023-06-16 15:03:59.336314 time_lapse-5.0/time_lapse/detect_audio.py
+-rwxr-xr-x   0        0        0    98228 2022-01-17 10:30:52.275448 time_lapse-5.0/time_lapse/fonts/Jost-400-Book.ttf
+-rwxr-xr-x   0        0        0     3627 2022-01-17 10:30:52.275875 time_lapse-5.0/time_lapse/fonts/LICENSE.md
+-rw-r--r--   0        0        0     2271 2023-06-16 15:03:59.336503 time_lapse-5.0/time_lapse/output.py
+-rw-r--r--   0        0        0        0 2023-06-16 15:03:59.336545 time_lapse-5.0/time_lapse/py.typed
+-rw-r--r--   0        0        0     1131 2023-06-16 15:03:59.336751 time_lapse-5.0/time_lapse/source.py
+-rw-r--r--   0        0        0      693 2023-06-16 15:03:59.336913 time_lapse-5.0/time_lapse/watermark.py
+-rw-r--r--   0        0        0     5050 1970-01-01 00:00:00.000000 time_lapse-5.0/PKG-INFO
```

### Comparing `time_lapse-4.0/.github/workflows/tests.yml` & `time_lapse-5.0/.github/workflows/tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,25 @@
           cache: 'pip'
           cache-dependency-path: 'requirements-ruff.txt'
       - run: make ruffinstall
       - run: make rufftest
         env:
           RUFF_FORMAT: github
 
-  mypytest:
+  typingtest:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.11'
           cache: 'pip'
           cache-dependency-path: 'pyproject.toml'
       - run: make devinstall
-      - run: make mypytest
+      - run: make typingtest
 
   unittest:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
```

### Comparing `time_lapse-4.0/LICENSE` & `time_lapse-5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/README.md` & `time_lapse-5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 =============
 
 Using time-lapse to find tif files, and create a movie called 'test_movie'
 with 24 fps and deflickered:
 
     from time_lapse import output, source
 
-    source_input = source.get_input(['*.tif'], fps=24, deflicker=10)
+    source_input = source.get_input(['*.tif'], fps=24, deflicker=10, filters=None)
     output.create_outputs(source_input, 'test_movie', verbose=False)
 
 Inspection
 ----------
 
 By passing `verbose=True` to create outputs the following ffmpeg-python
 inspection methods will be performed.
```

### Comparing `time_lapse-4.0/demo/source/S60_050504_181349.jpg` & `time_lapse-5.0/demo/source/S60_050504_181349.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_181449.jpg` & `time_lapse-5.0/demo/source/S60_050504_181449.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_181549.jpg` & `time_lapse-5.0/demo/source/S60_050504_181549.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_181649.jpg` & `time_lapse-5.0/demo/source/S60_050504_181649.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_181749.jpg` & `time_lapse-5.0/demo/source/S60_050504_181749.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_181849.jpg` & `time_lapse-5.0/demo/source/S60_050504_181849.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_181949.jpg` & `time_lapse-5.0/demo/source/S60_050504_181949.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_182049.jpg` & `time_lapse-5.0/demo/source/S60_050504_182049.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_182149.jpg` & `time_lapse-5.0/demo/source/S60_050504_182149.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_182249.jpg` & `time_lapse-5.0/demo/source/S60_050504_182249.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_182349.jpg` & `time_lapse-5.0/demo/source/S60_050504_182349.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_182449.jpg` & `time_lapse-5.0/demo/source/S60_050504_182449.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_182549.jpg` & `time_lapse-5.0/demo/source/S60_050504_182549.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_182649.jpg` & `time_lapse-5.0/demo/source/S60_050504_182649.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_182749.jpg` & `time_lapse-5.0/demo/source/S60_050504_182749.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_182849.jpg` & `time_lapse-5.0/demo/source/S60_050504_182849.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_182949.jpg` & `time_lapse-5.0/demo/source/S60_050504_182949.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_183049.jpg` & `time_lapse-5.0/demo/source/S60_050504_183049.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_183149.jpg` & `time_lapse-5.0/demo/source/S60_050504_183149.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_183249.jpg` & `time_lapse-5.0/demo/source/S60_050504_183249.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_183349.jpg` & `time_lapse-5.0/demo/source/S60_050504_183349.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_183449.jpg` & `time_lapse-5.0/demo/source/S60_050504_183449.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_183549.jpg` & `time_lapse-5.0/demo/source/S60_050504_183549.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_183649.jpg` & `time_lapse-5.0/demo/source/S60_050504_183649.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_183749.jpg` & `time_lapse-5.0/demo/source/S60_050504_183749.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_184017.jpg` & `time_lapse-5.0/demo/source/S60_050504_184017.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_184117.jpg` & `time_lapse-5.0/demo/source/S60_050504_184117.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_184217.jpg` & `time_lapse-5.0/demo/source/S60_050504_184217.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_184317.jpg` & `time_lapse-5.0/demo/source/S60_050504_184317.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_184417.jpg` & `time_lapse-5.0/demo/source/S60_050504_184417.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_184517.jpg` & `time_lapse-5.0/demo/source/S60_050504_184517.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_184617.jpg` & `time_lapse-5.0/demo/source/S60_050504_184617.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_184717.jpg` & `time_lapse-5.0/demo/source/S60_050504_184717.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_184817.jpg` & `time_lapse-5.0/demo/source/S60_050504_184817.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_184917.jpg` & `time_lapse-5.0/demo/source/S60_050504_184917.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_185017.jpg` & `time_lapse-5.0/demo/source/S60_050504_185017.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_185117.jpg` & `time_lapse-5.0/demo/source/S60_050504_185117.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_185217.jpg` & `time_lapse-5.0/demo/source/S60_050504_185217.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_185317.jpg` & `time_lapse-5.0/demo/source/S60_050504_185317.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_185417.jpg` & `time_lapse-5.0/demo/source/S60_050504_185417.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_185517.jpg` & `time_lapse-5.0/demo/source/S60_050504_185517.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_185617.jpg` & `time_lapse-5.0/demo/source/S60_050504_185617.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_185717.jpg` & `time_lapse-5.0/demo/source/S60_050504_185717.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_185817.jpg` & `time_lapse-5.0/demo/source/S60_050504_185817.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_185917.jpg` & `time_lapse-5.0/demo/source/S60_050504_185917.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_190017.jpg` & `time_lapse-5.0/demo/source/S60_050504_190017.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_190117.jpg` & `time_lapse-5.0/demo/source/S60_050504_190117.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_190217.jpg` & `time_lapse-5.0/demo/source/S60_050504_190217.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_190317.jpg` & `time_lapse-5.0/demo/source/S60_050504_190317.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_190417.jpg` & `time_lapse-5.0/demo/source/S60_050504_190417.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_190517.jpg` & `time_lapse-5.0/demo/source/S60_050504_190517.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_190617.jpg` & `time_lapse-5.0/demo/source/S60_050504_190617.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_190717.jpg` & `time_lapse-5.0/demo/source/S60_050504_190717.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_190817.jpg` & `time_lapse-5.0/demo/source/S60_050504_190817.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_190917.jpg` & `time_lapse-5.0/demo/source/S60_050504_190917.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_191017.jpg` & `time_lapse-5.0/demo/source/S60_050504_191017.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_191117.jpg` & `time_lapse-5.0/demo/source/S60_050504_191117.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_191217.jpg` & `time_lapse-5.0/demo/source/S60_050504_191217.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_191417.jpg` & `time_lapse-5.0/demo/source/S60_050504_191417.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_191517.jpg` & `time_lapse-5.0/demo/source/S60_050504_191517.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_191617.jpg` & `time_lapse-5.0/demo/source/S60_050504_191617.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_191717.jpg` & `time_lapse-5.0/demo/source/S60_050504_191717.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_191817.jpg` & `time_lapse-5.0/demo/source/S60_050504_191817.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_191917.jpg` & `time_lapse-5.0/demo/source/S60_050504_191917.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_192017.jpg` & `time_lapse-5.0/demo/source/S60_050504_192017.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_192117.jpg` & `time_lapse-5.0/demo/source/S60_050504_192117.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_192217.jpg` & `time_lapse-5.0/demo/source/S60_050504_192217.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_192317.jpg` & `time_lapse-5.0/demo/source/S60_050504_192317.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_192417.jpg` & `time_lapse-5.0/demo/source/S60_050504_192417.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/demo/source/S60_050504_192517.jpg` & `time_lapse-5.0/demo/source/S60_050504_192517.jpg`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/pyproject.toml` & `time_lapse-5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['flit_core>=3.9']
 build-backend = 'flit_core.buildapi'
 
 [project]
 name = 'time-lapse'
-version = '4.0'
+version = '5.0'
 description = 'Time-lapse movie assembly'
 readme = 'README.md'
 requires-python = '>=3.11'
 license = {file = 'LICENSE'}
 authors = [
     {name = 'Arne de Laat', email = 'arne@delaat.net'},
 ]
@@ -34,17 +34,20 @@
 ]
 
 [project.optional-dependencies]
 graph = [
     'graphviz',
 ]
 dev = [
-    'coverage',
-    'flit',
-    'mypy',
+    'black==23.3.0',
+    'coverage==7.2.7',
+    'mypy==1.4.1',
+]
+publish = [
+    'flit==3.9.0',
 ]
 
 [project.urls]
 Homepage = 'https://arne.delaat.net/timelapse.html'
 Repository = 'https://github.com/153957/time-lapse'
 
 [project.scripts]
@@ -76,23 +79,27 @@
     'E221', 'E222', 'E223', 'E224', 'E225', 'E226', 'E227', 'E228',
     'E231',
     'E251', 'E252',
     'E261', 'E262', 'E265', 'E266',
     'E271', 'E272', 'E273', 'E274', 'E275',
 ]
 ignore = [
+    'ANN101',  # No need to add type to self
     'D',  # Ignore docstring checks
+    'EM',  # Allow messages directly in exceptions
     'FBT001',  # Allow positional for boolean arguments
     'FBT002',  # Allow default value for boolean arguments
     'PD',  # Not using pandas
     'PLR0913',  # Allow functions with many arguments
+    'PT',  # Not using pytest
     'Q000',  # Use single quotes
     'RET504',  # Allow variable assignment before return
     'SIM108',  # Allow if-else block instead of ternary
     'T201',  # Allow using print
+    'TRY003',  # Specific messages for common exception classes
 ]
 
 [tool.ruff.isort]
 lines-between-types = 1
 section-order = [
     'future',
     'standard-library',
```

### Comparing `time_lapse-4.0/time_lapse/check_interval.py` & `time_lapse-5.0/time_lapse/check_interval.py`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/time_lapse/cli.py` & `time_lapse-5.0/time_lapse/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import argparse
 
 from time_lapse import output, source
 
 
 def make_movie(
     name: str,
-    patterns: list[str],
+    patterns: list[str] | str,
     fps: int,
     deflicker: int,
-    watermark: list[str],
+    watermark: bool | list[str],
     verbose: bool,
     dryrun: bool,
     filters: list[tuple[str, dict[str, str]]] | None = None,
 ) -> None:
     source_input = source.get_input(patterns, fps, deflicker, filters)
     output.create_outputs(source_input, name, watermark=watermark, verbose=verbose, dryrun=dryrun)
```

### Comparing `time_lapse-4.0/time_lapse/fonts/Jost-400-Book.ttf` & `time_lapse-5.0/time_lapse/fonts/Jost-400-Book.ttf`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/time_lapse/fonts/LICENSE.md` & `time_lapse-5.0/time_lapse/fonts/LICENSE.md`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/time_lapse/output.py` & `time_lapse-5.0/time_lapse/output.py`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/time_lapse/source.py` & `time_lapse-5.0/time_lapse/source.py`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/time_lapse/watermark.py` & `time_lapse-5.0/time_lapse/watermark.py`

 * *Files identical despite different names*

### Comparing `time_lapse-4.0/PKG-INFO` & `time_lapse-5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: time-lapse
-Version: 4.0
+Version: 5.0
 Summary: Time-lapse movie assembly
 Keywords: ffmpeg,photography,time-lapse
 Author-email: Arne de Laat <arne@delaat.net>
 Maintainer-email: Arne de Laat <arne@delaat.net>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Requires-Dist: exifreader==0.1.1
 Requires-Dist: ffmpeg-python==0.2.0
-Requires-Dist: coverage ; extra == "dev"
-Requires-Dist: flit ; extra == "dev"
-Requires-Dist: mypy ; extra == "dev"
+Requires-Dist: black==23.3.0 ; extra == "dev"
+Requires-Dist: coverage==7.2.7 ; extra == "dev"
+Requires-Dist: mypy==1.4.1 ; extra == "dev"
 Requires-Dist: graphviz ; extra == "graph"
+Requires-Dist: flit==3.9.0 ; extra == "publish"
 Project-URL: Homepage, https://arne.delaat.net/timelapse.html
 Project-URL: Repository, https://github.com/153957/time-lapse
 Provides-Extra: dev
 Provides-Extra: graph
+Provides-Extra: publish
 
 Time-Lapse assembling
 =====================
 
 [![PyPI](https://img.shields.io/pypi/v/time-lapse)](https://pypi.org/project/time-lapse/)
 [![License](https://img.shields.io/github/license/153957/time-lapse)](https://github.com/153957/time-lapse/blob/main/LICENSE)
 [![Build](https://img.shields.io/github/actions/workflow/status/153957/time-lapse/tests.yml?branch=main)](https://github.com/153957/time-lapse/actions)
@@ -141,15 +143,15 @@
 =============
 
 Using time-lapse to find tif files, and create a movie called 'test_movie'
 with 24 fps and deflickered:
 
     from time_lapse import output, source
 
-    source_input = source.get_input(['*.tif'], fps=24, deflicker=10)
+    source_input = source.get_input(['*.tif'], fps=24, deflicker=10, filters=None)
     output.create_outputs(source_input, 'test_movie', verbose=False)
 
 Inspection
 ----------
 
 By passing `verbose=True` to create outputs the following ffmpeg-python
 inspection methods will be performed.
```

