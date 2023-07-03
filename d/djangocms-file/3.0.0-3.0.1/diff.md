# Comparing `tmp/djangocms-file-3.0.0.tar.gz` & `tmp/djangocms-file-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangocms-file-3.0.0.tar", last modified: Wed Sep  2 13:39:41 2020, max compression
+gzip compressed data, was "djangocms-file-3.0.1.tar", last modified: Mon Jul  3 23:34:32 2023, max compression
```

## Comparing `djangocms-file-3.0.0.tar` & `djangocms-file-3.0.1.tar`

### file list

```diff
@@ -1,340 +1,342 @@
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:41.105624 djangocms-file-3.0.0/
--rw-r--r--   0 finalangel   (501) staff       (20)     1475 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/LICENSE
--rw-r--r--   0 finalangel   (501) staff       (20)      151 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/MANIFEST.in
--rw-r--r--   0 finalangel   (501) staff       (20)     5473 2020-09-02 13:39:41.105165 djangocms-file-3.0.0/PKG-INFO
--rw-r--r--   0 finalangel   (501) staff       (20)     3398 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/README.rst
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.834978 djangocms-file-3.0.0/djangocms_file/
--rw-r--r--   0 finalangel   (501) staff       (20)       22 2020-09-02 13:38:46.000000 djangocms-file-3.0.0/djangocms_file/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)     1687 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/cms_plugins.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.788535 djangocms-file-3.0.0/djangocms_file/locale/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.769796 djangocms-file-3.0.0/djangocms_file/locale/af/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.854379 djangocms-file-3.0.0/djangocms_file/locale/af/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      419 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/af/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1812 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/af/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.770109 djangocms-file-3.0.0/djangocms_file/locale/ar/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.978013 djangocms-file-3.0.0/djangocms_file/locale/ar/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      601 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1968 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.770332 djangocms-file-3.0.0/djangocms_file/locale/be/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.985871 djangocms-file-3.0.0/djangocms_file/locale/be/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      558 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/be/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1951 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/be/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.770549 djangocms-file-3.0.0/djangocms_file/locale/bg/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.002536 djangocms-file-3.0.0/djangocms_file/locale/bg/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      519 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1886 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.770758 djangocms-file-3.0.0/djangocms_file/locale/bn/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.020204 djangocms-file-3.0.0/djangocms_file/locale/bn/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      417 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/bn/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1810 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/bn/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.770967 djangocms-file-3.0.0/djangocms_file/locale/ca/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.040370 djangocms-file-3.0.0/djangocms_file/locale/ca/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      515 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1882 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.771386 djangocms-file-3.0.0/djangocms_file/locale/cmn/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.042579 djangocms-file-3.0.0/djangocms_file/locale/cmn/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      423 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/cmn/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1816 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/cmn/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.771621 djangocms-file-3.0.0/djangocms_file/locale/cs/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.057786 djangocms-file-3.0.0/djangocms_file/locale/cs/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      540 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1907 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.771854 djangocms-file-3.0.0/djangocms_file/locale/cy/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.077601 djangocms-file-3.0.0/djangocms_file/locale/cy/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      460 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/cy/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1853 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/cy/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.772068 djangocms-file-3.0.0/djangocms_file/locale/da/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.092227 djangocms-file-3.0.0/djangocms_file/locale/da/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      511 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1878 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.772301 djangocms-file-3.0.0/djangocms_file/locale/de/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.108042 djangocms-file-3.0.0/djangocms_file/locale/de/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)     1684 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     2296 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.772578 djangocms-file-3.0.0/djangocms_file/locale/el/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.122817 djangocms-file-3.0.0/djangocms_file/locale/el/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      519 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1886 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.772793 djangocms-file-3.0.0/djangocms_file/locale/en/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.130791 djangocms-file-3.0.0/djangocms_file/locale/en/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)     1502 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     2110 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.773009 djangocms-file-3.0.0/djangocms_file/locale/es/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.144040 djangocms-file-3.0.0/djangocms_file/locale/es/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      417 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1810 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.773231 djangocms-file-3.0.0/djangocms_file/locale/es_AR/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.158281 djangocms-file-3.0.0/djangocms_file/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      534 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1901 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.773446 djangocms-file-3.0.0/djangocms_file/locale/es_BO/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.166543 djangocms-file-3.0.0/djangocms_file/locale/es_BO/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      532 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/es_BO/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1899 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/es_BO/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.773658 djangocms-file-3.0.0/djangocms_file/locale/es_DO/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.168468 djangocms-file-3.0.0/djangocms_file/locale/es_DO/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      444 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/es_DO/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1837 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/es_DO/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.773877 djangocms-file-3.0.0/djangocms_file/locale/et/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.177338 djangocms-file-3.0.0/djangocms_file/locale/et/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      514 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1881 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.774111 djangocms-file-3.0.0/djangocms_file/locale/eu/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.192346 djangocms-file-3.0.0/djangocms_file/locale/eu/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      518 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1885 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.774486 djangocms-file-3.0.0/djangocms_file/locale/fa/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.199830 djangocms-file-3.0.0/djangocms_file/locale/fa/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      510 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1877 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.774785 djangocms-file-3.0.0/djangocms_file/locale/fi/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.208461 djangocms-file-3.0.0/djangocms_file/locale/fi/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      517 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1884 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.775143 djangocms-file-3.0.0/djangocms_file/locale/fr/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.223614 djangocms-file-3.0.0/djangocms_file/locale/fr/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      415 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1808 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.775409 djangocms-file-3.0.0/djangocms_file/locale/ga/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.237694 djangocms-file-3.0.0/djangocms_file/locale/ga/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      453 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ga/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1846 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ga/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.775652 djangocms-file-3.0.0/djangocms_file/locale/gl/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.251748 djangocms-file-3.0.0/djangocms_file/locale/gl/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      418 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1811 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.775875 djangocms-file-3.0.0/djangocms_file/locale/gu/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.265884 djangocms-file-3.0.0/djangocms_file/locale/gu/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      418 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/gu/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1811 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/gu/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.776100 djangocms-file-3.0.0/djangocms_file/locale/he/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.280630 djangocms-file-3.0.0/djangocms_file/locale/he/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      516 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1883 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.776315 djangocms-file-3.0.0/djangocms_file/locale/hi/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.295109 djangocms-file-3.0.0/djangocms_file/locale/hi/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      522 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/hi/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1889 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/hi/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.776600 djangocms-file-3.0.0/djangocms_file/locale/hr/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.310115 djangocms-file-3.0.0/djangocms_file/locale/hr/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      590 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1957 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.776858 djangocms-file-3.0.0/djangocms_file/locale/hu/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.323620 djangocms-file-3.0.0/djangocms_file/locale/hu/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      516 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1883 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.777087 djangocms-file-3.0.0/djangocms_file/locale/id/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.338220 djangocms-file-3.0.0/djangocms_file/locale/id/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      413 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1806 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.777312 djangocms-file-3.0.0/djangocms_file/locale/is/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.356462 djangocms-file-3.0.0/djangocms_file/locale/is/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      538 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/is/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1905 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.777557 djangocms-file-3.0.0/djangocms_file/locale/is_IS/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.370383 djangocms-file-3.0.0/djangocms_file/locale/is_IS/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      457 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/is_IS/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1850 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/is_IS/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.777772 djangocms-file-3.0.0/djangocms_file/locale/it/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.384504 djangocms-file-3.0.0/djangocms_file/locale/it/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      417 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1810 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.778002 djangocms-file-3.0.0/djangocms_file/locale/ja/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.399062 djangocms-file-3.0.0/djangocms_file/locale/ja/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      515 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1882 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.778216 djangocms-file-3.0.0/djangocms_file/locale/ka/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.412771 djangocms-file-3.0.0/djangocms_file/locale/ka/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      518 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ka/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1885 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ka/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.778428 djangocms-file-3.0.0/djangocms_file/locale/kk/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.420231 djangocms-file-3.0.0/djangocms_file/locale/kk/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      509 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/kk/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1876 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/kk/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.778686 djangocms-file-3.0.0/djangocms_file/locale/km/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.434725 djangocms-file-3.0.0/djangocms_file/locale/km/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      515 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/km/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1882 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/km/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.778901 djangocms-file-3.0.0/djangocms_file/locale/ko/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.449698 djangocms-file-3.0.0/djangocms_file/locale/ko/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      409 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1802 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.779121 djangocms-file-3.0.0/djangocms_file/locale/ko_KR/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.465566 djangocms-file-3.0.0/djangocms_file/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      521 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1888 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.779338 djangocms-file-3.0.0/djangocms_file/locale/ku_IQ/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.479296 djangocms-file-3.0.0/djangocms_file/locale/ku_IQ/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      532 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ku_IQ/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1899 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ku_IQ/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.779562 djangocms-file-3.0.0/djangocms_file/locale/lt/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.493385 djangocms-file-3.0.0/djangocms_file/locale/lt/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      581 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1948 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.779774 djangocms-file-3.0.0/djangocms_file/locale/lv/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.507338 djangocms-file-3.0.0/djangocms_file/locale/lv/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      452 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/lv/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1845 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.779983 djangocms-file-3.0.0/djangocms_file/locale/mn/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.521707 djangocms-file-3.0.0/djangocms_file/locale/mn/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      419 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1812 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/mn/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.780201 djangocms-file-3.0.0/djangocms_file/locale/mn_MN/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.535909 djangocms-file-3.0.0/djangocms_file/locale/mn_MN/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      436 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/mn_MN/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1829 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/mn_MN/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.780446 djangocms-file-3.0.0/djangocms_file/locale/mt/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.549144 djangocms-file-3.0.0/djangocms_file/locale/mt/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      490 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/mt/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1883 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/mt/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.780837 djangocms-file-3.0.0/djangocms_file/locale/nb/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.563627 djangocms-file-3.0.0/djangocms_file/locale/nb/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      522 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1889 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.781075 djangocms-file-3.0.0/djangocms_file/locale/nl/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.577818 djangocms-file-3.0.0/djangocms_file/locale/nl/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)     1676 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     2288 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.781308 djangocms-file-3.0.0/djangocms_file/locale/no/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.592426 djangocms-file-3.0.0/djangocms_file/locale/no/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      514 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/no/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1881 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/no/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.781532 djangocms-file-3.0.0/djangocms_file/locale/pl/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.606572 djangocms-file-3.0.0/djangocms_file/locale/pl/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      570 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1937 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.781802 djangocms-file-3.0.0/djangocms_file/locale/pt/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.620814 djangocms-file-3.0.0/djangocms_file/locale/pt/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      520 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1887 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.782124 djangocms-file-3.0.0/djangocms_file/locale/pt_BR/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.635345 djangocms-file-3.0.0/djangocms_file/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      533 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1900 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.782356 djangocms-file-3.0.0/djangocms_file/locale/ro/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.651076 djangocms-file-3.0.0/djangocms_file/locale/ro/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      558 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1925 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.782580 djangocms-file-3.0.0/djangocms_file/locale/ru/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.665861 djangocms-file-3.0.0/djangocms_file/locale/ru/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      655 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     2022 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.782810 djangocms-file-3.0.0/djangocms_file/locale/sk/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.681300 djangocms-file-3.0.0/djangocms_file/locale/sk/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      541 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1908 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.783123 djangocms-file-3.0.0/djangocms_file/locale/sl/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.695047 djangocms-file-3.0.0/djangocms_file/locale/sl/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      471 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1864 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.783397 djangocms-file-3.0.0/djangocms_file/locale/sl_SI/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.710887 djangocms-file-3.0.0/djangocms_file/locale/sl_SI/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      588 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sl_SI/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1955 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sl_SI/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.783676 djangocms-file-3.0.0/djangocms_file/locale/sq/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.725629 djangocms-file-3.0.0/djangocms_file/locale/sq/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      418 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1811 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.783976 djangocms-file-3.0.0/djangocms_file/locale/sq_AL/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.744085 djangocms-file-3.0.0/djangocms_file/locale/sq_AL/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      434 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sq_AL/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1827 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sq_AL/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.784226 djangocms-file-3.0.0/djangocms_file/locale/sr/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.758051 djangocms-file-3.0.0/djangocms_file/locale/sr/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      491 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1884 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.784514 djangocms-file-3.0.0/djangocms_file/locale/sr@latin/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.772104 djangocms-file-3.0.0/djangocms_file/locale/sr@latin/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      607 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sr@latin/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1974 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sr@latin/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.784911 djangocms-file-3.0.0/djangocms_file/locale/sv/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.785650 djangocms-file-3.0.0/djangocms_file/locale/sv/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      512 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1879 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.785205 djangocms-file-3.0.0/djangocms_file/locale/ta/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.799497 djangocms-file-3.0.0/djangocms_file/locale/ta/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      415 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ta/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1808 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ta/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.785514 djangocms-file-3.0.0/djangocms_file/locale/th/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.813271 djangocms-file-3.0.0/djangocms_file/locale/th/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      407 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/th/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1800 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.785929 djangocms-file-3.0.0/djangocms_file/locale/th_TH/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.828081 djangocms-file-3.0.0/djangocms_file/locale/th_TH/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      424 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/th_TH/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1817 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/th_TH/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.786308 djangocms-file-3.0.0/djangocms_file/locale/tlh/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.842367 djangocms-file-3.0.0/djangocms_file/locale/tlh/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      418 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/tlh/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1811 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/tlh/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.786563 djangocms-file-3.0.0/djangocms_file/locale/tr/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.856394 djangocms-file-3.0.0/djangocms_file/locale/tr/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      513 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1880 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.786794 djangocms-file-3.0.0/djangocms_file/locale/ug/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.869681 djangocms-file-3.0.0/djangocms_file/locale/ug/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      409 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ug/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1802 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ug/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.787012 djangocms-file-3.0.0/djangocms_file/locale/uk/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.883031 djangocms-file-3.0.0/djangocms_file/locale/uk/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      593 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1960 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.787231 djangocms-file-3.0.0/djangocms_file/locale/ur/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.896487 djangocms-file-3.0.0/djangocms_file/locale/ur/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      414 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ur/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1807 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/ur/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.787461 djangocms-file-3.0.0/djangocms_file/locale/vi/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.914322 djangocms-file-3.0.0/djangocms_file/locale/vi/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      413 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1806 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.787707 djangocms-file-3.0.0/djangocms_file/locale/vi_VN/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.936387 djangocms-file-3.0.0/djangocms_file/locale/vi_VN/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      430 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/vi_VN/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1823 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/vi_VN/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.788095 djangocms-file-3.0.0/djangocms_file/locale/zh/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.953549 djangocms-file-3.0.0/djangocms_file/locale/zh/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      410 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1803 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.788379 djangocms-file-3.0.0/djangocms_file/locale/zh_CN/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:40.989373 djangocms-file-3.0.0/djangocms_file/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      522 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1889 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.788620 djangocms-file-3.0.0/djangocms_file/locale/zh_TW/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:41.003504 djangocms-file-3.0.0/djangocms_file/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 finalangel   (501) staff       (20)      523 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 finalangel   (501) staff       (20)     1890 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:41.057656 djangocms-file-3.0.0/djangocms_file/migrations/
--rw-r--r--   0 finalangel   (501) staff       (20)     1088 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/migrations/0001_initial.py
--rw-r--r--   0 finalangel   (501) staff       (20)     1131 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/migrations/0002_auto_20151202_1551.py
--rw-r--r--   0 finalangel   (501) staff       (20)      507 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/migrations/0003_remove_related_name_for_cmsplugin_ptr.py
--rw-r--r--   0 finalangel   (501) staff       (20)      544 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/migrations/0004_set_related_name_for_cmsplugin_ptr.py
--rw-r--r--   0 finalangel   (501) staff       (20)      555 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/migrations/0005_auto_20160119_1534.py
--rw-r--r--   0 finalangel   (501) staff       (20)     1302 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/migrations/0006_migrate_to_filer.py
--rw-r--r--   0 finalangel   (501) staff       (20)     2278 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/migrations/0007_adapted_fields.py
--rw-r--r--   0 finalangel   (501) staff       (20)     1748 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/migrations/0008_add_folder.py
--rw-r--r--   0 finalangel   (501) staff       (20)      427 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/migrations/0009_fixed_null_fields.py
--rw-r--r--   0 finalangel   (501) staff       (20)      493 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/migrations/0010_removed_null_fields.py
--rw-r--r--   0 finalangel   (501) staff       (20)      722 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/migrations/0011_auto_20181211_0357.py
--rw-r--r--   0 finalangel   (501) staff       (20)        0 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/migrations/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)     5497 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/djangocms_file/models.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.789037 djangocms-file-3.0.0/djangocms_file/templates/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.789120 djangocms-file-3.0.0/djangocms_file/templates/djangocms_file/
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:41.063217 djangocms-file-3.0.0/djangocms_file/templates/djangocms_file/default/
--rw-r--r--   0 finalangel   (501) staff       (20)      886 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/templates/djangocms_file/default/file.html
--rw-r--r--   0 finalangel   (501) staff       (20)      839 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/djangocms_file/templates/djangocms_file/default/folder.html
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:39.843447 djangocms-file-3.0.0/djangocms_file.egg-info/
--rw-r--r--   0 finalangel   (501) staff       (20)     5473 2020-09-02 13:39:39.000000 djangocms-file-3.0.0/djangocms_file.egg-info/PKG-INFO
--rw-r--r--   0 finalangel   (501) staff       (20)     8273 2020-09-02 13:39:39.000000 djangocms-file-3.0.0/djangocms_file.egg-info/SOURCES.txt
--rw-r--r--   0 finalangel   (501) staff       (20)        1 2020-09-02 13:39:39.000000 djangocms-file-3.0.0/djangocms_file.egg-info/dependency_links.txt
--rw-r--r--   0 finalangel   (501) staff       (20)        1 2020-09-02 13:39:39.000000 djangocms-file-3.0.0/djangocms_file.egg-info/not-zip-safe
--rw-r--r--   0 finalangel   (501) staff       (20)       64 2020-09-02 13:39:39.000000 djangocms-file-3.0.0/djangocms_file.egg-info/requires.txt
--rw-r--r--   0 finalangel   (501) staff       (20)       21 2020-09-02 13:39:39.000000 djangocms-file-3.0.0/djangocms_file.egg-info/top_level.txt
--rw-r--r--   0 finalangel   (501) staff       (20)       38 2020-09-02 13:39:41.105759 djangocms-file-3.0.0/setup.cfg
--rw-r--r--   0 finalangel   (501) staff       (20)     1604 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/setup.py
-drwxr-xr-x   0 finalangel   (501) staff       (20)        0 2020-09-02 13:39:41.103174 djangocms-file-3.0.0/tests/
--rw-r--r--   0 finalangel   (501) staff       (20)        0 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/tests/__init__.py
--rw-r--r--   0 finalangel   (501) staff       (20)     3235 2020-08-14 13:37:27.000000 djangocms-file-3.0.0/tests/helpers.py
--rw-r--r--   0 finalangel   (501) staff       (20)      429 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/tests/settings.py
--rw-r--r--   0 finalangel   (501) staff       (20)      885 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/tests/test_migrations.py
--rw-r--r--   0 finalangel   (501) staff       (20)     3997 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/tests/test_models.py
--rw-r--r--   0 finalangel   (501) staff       (20)     3115 2020-09-02 08:23:22.000000 djangocms-file-3.0.0/tests/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.534199 djangocms-file-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-03 23:34:32.534199 djangocms-file-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.502199 djangocms-file-3.0.1/djangocms_file/locale/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/af/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/af/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/be/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/be/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/be/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/be/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/bn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/bn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/bn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/cmn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/cmn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/cmn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/cmn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/cy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/cy/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/cy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/es_BO/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/es_BO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/es_BO/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/es_BO/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/es_DO/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file/locale/es_DO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/es_DO/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/es_DO/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/ga/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/ga/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ga/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ga/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/gu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/gu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/gu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/gu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/hi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/hi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.506199 djangocms-file-3.0.1/djangocms_file/locale/is/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/is/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/is/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/is_IS/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/is_IS/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/is_IS/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/is_IS/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.522199 djangocms-file-3.0.1/djangocms_file/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ka/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ka/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/kk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/kk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/kk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/kk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/km/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/km/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/km/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/km/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/ku_IQ/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/ku_IQ/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ku_IQ/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ku_IQ/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/mn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/mn_MN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/mn_MN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/mn_MN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/mn_MN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/mt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/mt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/mt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/mt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/no/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/no/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.526199 djangocms-file-3.0.1/djangocms_file/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/sl_SI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/sl_SI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sl_SI/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sl_SI/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/sq_AL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/sq_AL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sq_AL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sq_AL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.510199 djangocms-file-3.0.1/djangocms_file/locale/sr@latin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/sr@latin/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sr@latin/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sr@latin/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/ta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ta/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ta/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/th/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/th_TH/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/th_TH/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/th_TH/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/th_TH/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/tlh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/tlh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/tlh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/tlh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/ug/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/ug/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ug/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ug/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/ur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.530199 djangocms-file-3.0.1/djangocms_file/locale/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ur/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/ur/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.534199 djangocms-file-3.0.1/djangocms_file/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/vi_VN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.534199 djangocms-file-3.0.1/djangocms_file/locale/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/vi_VN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/vi_VN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.534199 djangocms-file-3.0.1/djangocms_file/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.534199 djangocms-file-3.0.1/djangocms_file/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.534199 djangocms-file-3.0.1/djangocms_file/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.534199 djangocms-file-3.0.1/djangocms_file/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/0002_auto_20151202_1551.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/0003_remove_related_name_for_cmsplugin_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/0004_set_related_name_for_cmsplugin_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/0005_auto_20160119_1534.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/0006_migrate_to_filer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/0007_adapted_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/0008_add_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/0009_fixed_null_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/0010_removed_null_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/0011_auto_20181211_0357.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/0012_alter_file_cmsplugin_ptr_alter_folder_cmsplugin_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.514199 djangocms-file-3.0.1/djangocms_file/templates/djangocms_file/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.534199 djangocms-file-3.0.1/djangocms_file/templates/djangocms_file/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/templates/djangocms_file/default/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/djangocms_file/templates/djangocms_file/default/folder.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.518199 djangocms-file-3.0.1/djangocms_file.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-03 23:34:32.000000 djangocms-file-3.0.1/djangocms_file.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-07-03 23:34:32.000000 djangocms-file-3.0.1/djangocms_file.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:34:32.000000 djangocms-file-3.0.1/djangocms_file.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 23:34:32.000000 djangocms-file-3.0.1/djangocms_file.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-03 23:34:32.000000 djangocms-file-3.0.1/djangocms_file.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 23:34:32.000000 djangocms-file-3.0.1/djangocms_file.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 23:34:32.534199 djangocms-file-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:32.534199 djangocms-file-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-03 23:34:23.000000 djangocms-file-3.0.1/tests/test_plugins.py
```

### Comparing `djangocms-file-3.0.0/LICENSE` & `djangocms-file-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/PKG-INFO` & `djangocms-file-3.0.1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,135 +1,116 @@
-Metadata-Version: 1.1
-Name: djangocms-file
-Version: 3.0.0
-Summary: Adds file plugin to django CMS
-Home-page: https://github.com/divio/djangocms-file
-Author: Divio AG
-Author-email: info@divio.ch
-License: BSD-3-Clause
-Description: ===============
-        django CMS File
-        ===============
-        
-        |pypi| |build| |coverage|
-        
-        **django CMS File** is a set of plugins for `django CMS <http://django-cms.org>`_
-        that allow you to add files to your site You can either choose a single file or
-        an entire folder.
-        
-        It uses files managed by `Django Filer <https://github.com/divio/django-filer>`_.
-        
-        This addon is compatible with `Divio Cloud <http://divio.com>`_ and is also available on the
-        `django CMS Marketplace <https://marketplace.django-cms.org/en/addons/browse/djangocms-file/>`_
-        for easy installation.
-        
-        .. image:: preview.gif
-        
-        
-        Contributing
-        ============
-        
-        This is a an open-source project. We'll be delighted to receive your
-        feedback in the form of issues and pull requests. Before submitting your
-        pull request, please review our `contribution guidelines
-        <http://docs.django-cms.org/en/latest/contributing/index.html>`_.
-        
-        We're grateful to all contributors who have helped create and maintain this package.
-        Contributors are listed at the `contributors <https://github.com/divio/djangocms-file/graphs/contributors>`_
-        section.
-        
-        One of the easiest contributions you can make is helping to translate this addon on
-        `Transifex <https://www.transifex.com/projects/p/djangocms-file/>`_.
-        
-        
-        Documentation
-        =============
-        
-        See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-file/blob/master/setup.py>`_
-        file for additional dependencies:
-        
-        |python| |django| |djangocms|
-        
-        * Django Filer 1.7 or higher
-        
-        Make sure `django-filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
-        is installed and configured appropriately.
-        
-        
-        Installation
-        ------------
-        
-        For a manual install:
-        
-        * run ``pip install djangocms-file``
-        * add ``djangocms_file`` to your ``INSTALLED_APPS``
-        * run ``python manage.py migrate djangocms_file``
-        
-        
-        Configuration
-        -------------
-        
-        Note that the provided templates are very minimal by design. You are encouraged
-        to adapt and override them to your project's requirements.
-        
-        This addon provides a ``default`` template for all instances. You can provide
-        additional template choices by adding a ``DJANGOCMS_FILE_TEMPLATES``
-        setting::
-        
-            DJANGOCMS_FILE_TEMPLATES = [
-                ('feature', _('Featured Version')),
-            ]
-        
-        You'll need to create the `feature` folder inside ``templates/djangocms_file/``
-        otherwise you will get a *template does not exist* error. You can do this by
-        copying the ``default`` folder inside that directory and renaming it to
-        ``feature``.
-        
-        
-        Running Tests
-        -------------
-        
-        You can run tests by executing::
-        
-            virtualenv env
-            source env/bin/activate
-            pip install -r test_requirements/base.txt
-            python setup.py test
-        
-        
-        .. |pypi| image:: https://badge.fury.io/py/djangocms-file.svg
-            :target: http://badge.fury.io/py/djangocms-file
-        .. |build| image:: https://travis-ci.org/divio/djangocms-file.svg?branch=master
-            :target: https://travis-ci.org/divio/djangocms-file
-        .. |coverage| image:: https://codecov.io/gh/divio/djangocms-file/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/divio/djangocms-file
-        
-        .. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
-            :target: https://pypi.org/project/djangocms-file/
-        .. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
-            :target: https://www.djangoproject.com/
-        .. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
-            :target: https://www.django-cms.org/
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django CMS
-Classifier: Framework :: Django CMS :: 3.7
-Classifier: Framework :: Django CMS :: 3.8
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
+===============
+django CMS File
+===============
+
+|pypi| |build| |coverage| |python| |django| |djangocms|
+
+**django CMS File** is a set of plugins for `django CMS <http://django-cms.org>`_
+that allow you to add files to your site You can either choose a single file or
+an entire folder.
+
+It uses files managed by `Django Filer <https://github.com/divio/django-filer>`_.
+
+This addon is compatible with `Divio Cloud <http://divio.com>`_
+for easy installation.
+
+.. image:: preview.gif
+
+
+Contributing
+============
+
+This is a an open-source project. We'll be delighted to receive your
+feedback in the form of issues and pull requests. Before submitting your
+pull request, please review our `contribution guidelines
+<http://docs.django-cms.org/en/latest/contributing/index.html>`_.
+
+We're grateful to all contributors who have helped create and maintain this package.
+Contributors are listed at the `contributors <https://github.com/divio/djangocms-file/graphs/contributors>`_
+section.
+
+One of the easiest contributions you can make is helping to translate this addon on
+`Transifex <https://www.transifex.com/projects/p/djangocms-file/>`_.
+
+
+Documentation
+=============
+
+See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-file/blob/master/setup.py>`_
+file for additional dependencies:
+
+* Django Filer 1.7 or higher
+
+Make sure `django-filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
+is installed and configured appropriately.
+
+
+Installation
+------------
+
+For a manual install:
+
+* run ``pip install djangocms-file``
+* add ``djangocms_file`` to your ``INSTALLED_APPS``
+* run ``python manage.py migrate djangocms_file``
+
+
+Configuration
+-------------
+
+Note that the provided templates are very minimal by design. You are encouraged
+to adapt and override them to your project's requirements.
+
+This addon provides a ``default`` template for all instances. You can provide
+additional template choices by adding a ``DJANGOCMS_FILE_TEMPLATES``
+setting::
+
+    DJANGOCMS_FILE_TEMPLATES = [
+        ('feature', _('Featured Version')),
+    ]
+
+You'll need to create the ``feature`` folder inside ``templates/djangocms_file/``
+otherwise you will get a *template does not exist* error. You can do this by
+copying the ``default`` folder inside that directory and renaming it to
+``feature``.
+
+
+Running Tests
+-------------
+
+You can run tests by executing::
+
+    virtualenv env
+    source env/bin/activate
+    pip install -r test_requirements/base.txt
+    python setup.py test
+
+
+.. |pypi| image:: https://badge.fury.io/py/djangocms-file.svg
+    :target: http://badge.fury.io/py/djangocms-file
+.. |build| image:: https://travis-ci.org/django-cms/djangocms-file.svg?branch=master
+    :target: https://travis-ci.org/divio/djangocms-file
+.. |coverage| image:: https://codecov.io/gh/django-cms/djangocms-file/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/divio/djangocms-file
+
+.. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
+    :target: https://pypi.org/project/djangocms-file/
+.. |django| image:: https://img.shields.io/badge/django-2.2--4.0-blue.svg
+    :target: https://www.djangoproject.com/
+.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
+    :target: https://www.django-cms.org/
+
+
+Updating from `cmsplugin-filer <https://github.com/django-cms/cmsplugin-filer>`_
+--------------------------------------------------------------------------------
+
+Historically, `cmsplugin-filer` was used to create file, folder, image, link, teaser & video plugins on your django CMS projects. Now `cmsplugin-filer` has been archived, you can still migrate your old instances without having to copy them manually to the new `djangocms-<file|picture|link|...>` plugins.
+
+There's a third-party management command that supports your migration:
+
+`migrate_cmsplugin_filer.py <https://gist.github.com/corentinbettiol/84a6ea7e4d047fc01861b0af15fd60f0>`_
+
+This management command is only a starting point. It *has* worked out of the box for some people, but we encourage you to read the code, understand what it does, and test it on a development environment before running it on your production server.
+
+The management command is only configured to transfer your `cmsplugin_link`, `cmsplugin_file`, `cmsplugin_folder` and `cmsplugin_image` plugins to modern `djangocms_*` plugins. If you need to transfer other `cmsplugin_*` plugins, you'll have to write your own code.
+
+Alternatively you can use the `deprecate_cmsplugin_filer <https://github.com/ImaginaryLandscape/deprecate_cmsplugin_filer>`_ app, which only adds a small migration that transfer the old `cmsplugin-filer` plugins instances to the new `djangocms-<file|picture|link|...>` plugins.
```

### Comparing `djangocms-file-3.0.0/djangocms_file/cms_plugins.py` & `djangocms-file-3.0.1/djangocms_file/cms_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from django.utils.translation import gettext_lazy as _
-
 from cms.plugin_base import CMSPluginBase
 from cms.plugin_pool import plugin_pool
+from django.utils.translation import gettext_lazy as _
 
 from .models import File, Folder
 
 
 class FilePlugin(CMSPluginBase):
     model = File
     name = _('File')
```

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/af/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/af/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ar/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ar/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/be/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/be/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/be/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/be/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/bg/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/bg/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/bn/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/bn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ca/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ca/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/cmn/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/cmn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/cs/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/cs/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/cy/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/cy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/da/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/de/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/de/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/el/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/el/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/en/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/en/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/es/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/es_AR/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/es_AR/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/es_BO/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/es_BO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/es_BO/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/es_BO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/es_DO/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/es_DO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/et/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/et/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/eu/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/eu/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/fa/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/fi/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/fi/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/fr/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ga/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ga/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/gl/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/gu/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/gu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/he/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/he/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/hi/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/hi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/hi/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/hr/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/hr/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/hu/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/hu/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/id/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/is/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/is/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/is/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/is_IS/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/is_IS/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/it/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ja/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ja/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ka/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/ka/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ka/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/kk/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/kk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/km/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/km/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/km/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/km/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ko/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ko_KR/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ko_KR/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ku_IQ/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/ku_IQ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ku_IQ/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ku_IQ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/lt/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/lt/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/lv/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/mn/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/mn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/mn_MN/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/mn_MN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/mt/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/mt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/nb/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/nb/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/nl/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/nl/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/no/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/no/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/no/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/no/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/pl/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/pl/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/pt/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/pt/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/pt_BR/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/pt_BR/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ro/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ro/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ru/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ru/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/sk/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/sk/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/sl/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/sl_SI/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/sl_SI/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/sl_SI/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/sl_SI/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/sq/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/sq_AL/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/sq_AL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/sr/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/sr@latin/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/sr@latin/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/sr@latin/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/sr@latin/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/sv/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/sv/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ta/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ta/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/th/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/th/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/th_TH/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/th_TH/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/tlh/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/tlh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/tr/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/tr/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ug/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ug/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/uk/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/uk/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/ur/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/ur/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/vi/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/vi_VN/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/vi_VN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/zh/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/zh_CN/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/zh_CN/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/zh_TW/LC_MESSAGES/django.mo` & `djangocms-file-3.0.1/djangocms_file/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/locale/zh_TW/LC_MESSAGES/django.po` & `djangocms-file-3.0.1/djangocms_file/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/migrations/0001_initial.py` & `djangocms-file-3.0.1/djangocms_file/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/migrations/0002_auto_20151202_1551.py` & `djangocms-file-3.0.1/djangocms_file/migrations/0002_auto_20151202_1551.py`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/migrations/0004_set_related_name_for_cmsplugin_ptr.py` & `djangocms-file-3.0.1/djangocms_file/migrations/0004_set_related_name_for_cmsplugin_ptr.py`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/migrations/0005_auto_20160119_1534.py` & `djangocms-file-3.0.1/djangocms_file/migrations/0005_auto_20160119_1534.py`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/migrations/0006_migrate_to_filer.py` & `djangocms-file-3.0.1/djangocms_file/migrations/0006_migrate_to_filer.py`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/migrations/0007_adapted_fields.py` & `djangocms-file-3.0.1/djangocms_file/migrations/0007_adapted_fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/migrations/0008_add_folder.py` & `djangocms-file-3.0.1/djangocms_file/migrations/0008_add_folder.py`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/migrations/0011_auto_20181211_0357.py` & `djangocms-file-3.0.1/djangocms_file/migrations/0011_auto_20181211_0357.py`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/djangocms_file/models.py` & `djangocms-file-3.0.1/djangocms_file/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """
 Enables the user to add a "File" plugin that displays a file wrapped by
 an <anchor> tag.
 """
+from cms.models import CMSPlugin
 from django.conf import settings
 from django.db import models
 from django.utils.translation import gettext
 from django.utils.translation import gettext_lazy as _
-
-from cms.models import CMSPlugin
-
 from djangocms_attributes_field.fields import AttributesField
 from filer.fields.file import FilerFileField
 from filer.fields.folder import FilerFolderField
 
-
 LINK_TARGET = (
     ('_self', _('Open in same window')),
     ('_blank', _('Open in new window')),
     ('_parent', _('Delegate to parent')),
     ('_top', _('Delegate to top')),
 )
 
@@ -35,15 +32,15 @@
     return choices
 
 
 class AbstractFile(CMSPlugin):
     """
     Renders a file wrapped by an anchor
     """
-    search_fields = ('name',)
+    search_fields = ('file_name',)
 
     template = models.CharField(
         verbose_name=_('Template'),
         choices=get_templates(),
         default=get_templates()[0][0],
         max_length=255,
     )
```

### Comparing `djangocms-file-3.0.0/djangocms_file/templates/djangocms_file/default/file.html` & `djangocms-file-3.0.1/djangocms_file/templates/djangocms_file/default/file.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <a href="{{ instance.file_src.url }}"
     {% if instance.link_target %} target="{{ instance.link_target }}"{% endif %}
     {% if instance.link_title %} title="{{ instance.link_title }}"{% endif %}
-    {{ instance.attributes_str }}>
+    {{ instance.attributes_str }}>
     {% if instance.file_name %}
         {{ instance.file_name }}
     {% else %}
         {{ instance.file_src.label }}
     {% endif %}
     {% if instance.show_file_size %}
         <span>{{ instance.file_src.size|filesizeformat }}</span>
@@ -13,14 +13,14 @@
 </a>
 
 {% comment %}
     # https://github.com/divio/django-filer/blob/master/filer/models/filemodels.py
     {{ instance.file_src }}
     {{ instance.file_src.extension }}
     # Available variables:
-    {{ instance.template }}
+    {{ instance.template }}
     {{ instance.file_name }}
     {{ instance.link_target }}
     {{ instance.link_title }}
     {{ instance.show_file_size }}
-    {{ instance.attributes_str }}
+    {{ instance.attributes_str }}
 {% endcomment %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 % if instance.link_target %} target="{{ instance.link_target }}"{% endif %} {%
 if instance.link_title %} title="{{ instance.link_title }}"{% endif %} {
-{Â instance.attributes_str }}> {% if instance.file_name %} {
-{ instance.file_name }} {% else %} {{ instance.file_src.label }} {% endif %} {%
-if instance.show_file_size %} {{ instance.file_src.size|filesizeformat }} {%
-endif %}
+{ instance.attributes_str }}> {% if instance.file_name %} {{ instance.file_name
+}} {% else %} {{ instance.file_src.label }} {% endif %} {% if
+instance.show_file_size %} {{ instance.file_src.size|filesizeformat }} {% endif
+%}
  {% comment %} # https://github.com/divio/django-filer/blob/master/filer/
 models/filemodels.py {{ instance.file_src }} {{ instance.file_src.extension }}
-# Available variables: {{Â instance.template }} {{ instance.file_name }} {
+# Available variables: {{ instance.template }} {{ instance.file_name }} {
 { instance.link_target }} {{ instance.link_title }} {{ instance.show_file_size
-}} {{Â instance.attributes_str }} {% endcomment %}
+}} {{ instance.attributes_str }} {% endcomment %}
```

### Comparing `djangocms-file-3.0.0/djangocms_file/templates/djangocms_file/default/folder.html` & `djangocms-file-3.0.1/djangocms_file/templates/djangocms_file/default/folder.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load i18n %}
 
 {% for file in folder_files %}
     <a href="{{ file.url }}"
         {% if instance.link_target %} target="{{ instance.link_target }}"{% endif %}
-        {{ instance.attributes_str }}>
+        {{ instance.attributes_str }}>
         {{ file }}
         {% if instance.show_file_size %}
             <span>{{ file.size|filesizeformat }}</span>
         {% endif %}
     </a>
     {% if not forloop.last %}<br>{% endif %}
 {% empty %}
@@ -15,12 +15,12 @@
 {% endfor %}
 
 {% comment %}
     # https://github.com/divio/django-filer/blob/master/filer/models/filemodels.py
     {{ instance.folder_src }}
     {{ instance.get_files }} or {{ folder_files }}
     # Available variables:
-    {{ instance.template }}
+    {{ instance.template }}
     {{ instance.link_target }}
     {{ instance.show_file_size }}
-    {{ instance.attributes_str }}
+    {{ instance.attributes_str }}
 {% endcomment %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% load i18n %} {% for file in folder_files %}
 % if instance.link_target %} target="{{ instance.link_target }}"{% endif %} {
-{Â instance.attributes_str }}> {{ file }} {% if instance.show_file_size %} {
+{ instance.attributes_str }}> {{ file }} {% if instance.show_file_size %} {
 { file.size|filesizeformat }} {% endif %}
  {% if not forloop.last %}
 {% endif %} {% empty %}
 {% trans "No files were found in the specified folder." %}
 {% endfor %} {% comment %} # https://github.com/divio/django-filer/blob/master/
 filer/models/filemodels.py {{ instance.folder_src }} {{ instance.get_files }}
-or {{ folder_files }} # Available variables: {{Â instance.template }} {
+or {{ folder_files }} # Available variables: {{ instance.template }} {
 { instance.link_target }} {{ instance.show_file_size }} {
-{Â instance.attributes_str }} {% endcomment %}
+{ instance.attributes_str }} {% endcomment %}
```

### Comparing `djangocms-file-3.0.0/djangocms_file.egg-info/PKG-INFO` & `djangocms-file-3.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,155 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: djangocms-file
-Version: 3.0.0
+Version: 3.0.1
 Summary: Adds file plugin to django CMS
-Home-page: https://github.com/divio/djangocms-file
+Home-page: https://github.com/django-cms/djangocms-file
 Author: Divio AG
 Author-email: info@divio.ch
+Maintainer: Django CMS Association and contributors
+Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
-Description: ===============
-        django CMS File
-        ===============
-        
-        |pypi| |build| |coverage|
-        
-        **django CMS File** is a set of plugins for `django CMS <http://django-cms.org>`_
-        that allow you to add files to your site You can either choose a single file or
-        an entire folder.
-        
-        It uses files managed by `Django Filer <https://github.com/divio/django-filer>`_.
-        
-        This addon is compatible with `Divio Cloud <http://divio.com>`_ and is also available on the
-        `django CMS Marketplace <https://marketplace.django-cms.org/en/addons/browse/djangocms-file/>`_
-        for easy installation.
-        
-        .. image:: preview.gif
-        
-        
-        Contributing
-        ============
-        
-        This is a an open-source project. We'll be delighted to receive your
-        feedback in the form of issues and pull requests. Before submitting your
-        pull request, please review our `contribution guidelines
-        <http://docs.django-cms.org/en/latest/contributing/index.html>`_.
-        
-        We're grateful to all contributors who have helped create and maintain this package.
-        Contributors are listed at the `contributors <https://github.com/divio/djangocms-file/graphs/contributors>`_
-        section.
-        
-        One of the easiest contributions you can make is helping to translate this addon on
-        `Transifex <https://www.transifex.com/projects/p/djangocms-file/>`_.
-        
-        
-        Documentation
-        =============
-        
-        See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-file/blob/master/setup.py>`_
-        file for additional dependencies:
-        
-        |python| |django| |djangocms|
-        
-        * Django Filer 1.7 or higher
-        
-        Make sure `django-filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
-        is installed and configured appropriately.
-        
-        
-        Installation
-        ------------
-        
-        For a manual install:
-        
-        * run ``pip install djangocms-file``
-        * add ``djangocms_file`` to your ``INSTALLED_APPS``
-        * run ``python manage.py migrate djangocms_file``
-        
-        
-        Configuration
-        -------------
-        
-        Note that the provided templates are very minimal by design. You are encouraged
-        to adapt and override them to your project's requirements.
-        
-        This addon provides a ``default`` template for all instances. You can provide
-        additional template choices by adding a ``DJANGOCMS_FILE_TEMPLATES``
-        setting::
-        
-            DJANGOCMS_FILE_TEMPLATES = [
-                ('feature', _('Featured Version')),
-            ]
-        
-        You'll need to create the `feature` folder inside ``templates/djangocms_file/``
-        otherwise you will get a *template does not exist* error. You can do this by
-        copying the ``default`` folder inside that directory and renaming it to
-        ``feature``.
-        
-        
-        Running Tests
-        -------------
-        
-        You can run tests by executing::
-        
-            virtualenv env
-            source env/bin/activate
-            pip install -r test_requirements/base.txt
-            python setup.py test
-        
-        
-        .. |pypi| image:: https://badge.fury.io/py/djangocms-file.svg
-            :target: http://badge.fury.io/py/djangocms-file
-        .. |build| image:: https://travis-ci.org/divio/djangocms-file.svg?branch=master
-            :target: https://travis-ci.org/divio/djangocms-file
-        .. |coverage| image:: https://codecov.io/gh/divio/djangocms-file/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/divio/djangocms-file
-        
-        .. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
-            :target: https://pypi.org/project/djangocms-file/
-        .. |django| image:: https://img.shields.io/badge/django-2.2,%203.0,%203.1-blue.svg
-            :target: https://www.djangoproject.com/
-        .. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
-            :target: https://www.django-cms.org/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django CMS
 Classifier: Framework :: Django CMS :: 3.7
 Classifier: Framework :: Django CMS :: 3.8
+Classifier: Framework :: Django CMS :: 3.9
+Classifier: Framework :: Django CMS :: 3.10
+Classifier: Framework :: Django CMS :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+===============
+django CMS File
+===============
+
+|pypi| |build| |coverage| |python| |django| |djangocms|
+
+**django CMS File** is a set of plugins for `django CMS <http://django-cms.org>`_
+that allow you to add files to your site You can either choose a single file or
+an entire folder.
+
+It uses files managed by `Django Filer <https://github.com/divio/django-filer>`_.
+
+This addon is compatible with `Divio Cloud <http://divio.com>`_
+for easy installation.
+
+.. image:: preview.gif
+
+
+Contributing
+============
+
+This is a an open-source project. We'll be delighted to receive your
+feedback in the form of issues and pull requests. Before submitting your
+pull request, please review our `contribution guidelines
+<http://docs.django-cms.org/en/latest/contributing/index.html>`_.
+
+We're grateful to all contributors who have helped create and maintain this package.
+Contributors are listed at the `contributors <https://github.com/divio/djangocms-file/graphs/contributors>`_
+section.
+
+One of the easiest contributions you can make is helping to translate this addon on
+`Transifex <https://www.transifex.com/projects/p/djangocms-file/>`_.
+
+
+Documentation
+=============
+
+See ``REQUIREMENTS`` in the `setup.py <https://github.com/divio/djangocms-file/blob/master/setup.py>`_
+file for additional dependencies:
+
+* Django Filer 1.7 or higher
+
+Make sure `django-filer <http://django-filer.readthedocs.io/en/latest/installation.html>`_
+is installed and configured appropriately.
+
+
+Installation
+------------
+
+For a manual install:
+
+* run ``pip install djangocms-file``
+* add ``djangocms_file`` to your ``INSTALLED_APPS``
+* run ``python manage.py migrate djangocms_file``
+
+
+Configuration
+-------------
+
+Note that the provided templates are very minimal by design. You are encouraged
+to adapt and override them to your project's requirements.
+
+This addon provides a ``default`` template for all instances. You can provide
+additional template choices by adding a ``DJANGOCMS_FILE_TEMPLATES``
+setting::
+
+    DJANGOCMS_FILE_TEMPLATES = [
+        ('feature', _('Featured Version')),
+    ]
+
+You'll need to create the ``feature`` folder inside ``templates/djangocms_file/``
+otherwise you will get a *template does not exist* error. You can do this by
+copying the ``default`` folder inside that directory and renaming it to
+``feature``.
+
+
+Running Tests
+-------------
+
+You can run tests by executing::
+
+    virtualenv env
+    source env/bin/activate
+    pip install -r test_requirements/base.txt
+    python setup.py test
+
+
+.. |pypi| image:: https://badge.fury.io/py/djangocms-file.svg
+    :target: http://badge.fury.io/py/djangocms-file
+.. |build| image:: https://travis-ci.org/django-cms/djangocms-file.svg?branch=master
+    :target: https://travis-ci.org/divio/djangocms-file
+.. |coverage| image:: https://codecov.io/gh/django-cms/djangocms-file/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/divio/djangocms-file
+
+.. |python| image:: https://img.shields.io/badge/python-3.5+-blue.svg
+    :target: https://pypi.org/project/djangocms-file/
+.. |django| image:: https://img.shields.io/badge/django-2.2--4.0-blue.svg
+    :target: https://www.djangoproject.com/
+.. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.7%2B-blue.svg
+    :target: https://www.django-cms.org/
+
+
+Updating from `cmsplugin-filer <https://github.com/django-cms/cmsplugin-filer>`_
+--------------------------------------------------------------------------------
+
+Historically, `cmsplugin-filer` was used to create file, folder, image, link, teaser & video plugins on your django CMS projects. Now `cmsplugin-filer` has been archived, you can still migrate your old instances without having to copy them manually to the new `djangocms-<file|picture|link|...>` plugins.
+
+There's a third-party management command that supports your migration:
+
+`migrate_cmsplugin_filer.py <https://gist.github.com/corentinbettiol/84a6ea7e4d047fc01861b0af15fd60f0>`_
+
+This management command is only a starting point. It *has* worked out of the box for some people, but we encourage you to read the code, understand what it does, and test it on a development environment before running it on your production server.
+
+The management command is only configured to transfer your `cmsplugin_link`, `cmsplugin_file`, `cmsplugin_folder` and `cmsplugin_image` plugins to modern `djangocms_*` plugins. If you need to transfer other `cmsplugin_*` plugins, you'll have to write your own code.
+
+Alternatively you can use the `deprecate_cmsplugin_filer <https://github.com/ImaginaryLandscape/deprecate_cmsplugin_filer>`_ app, which only adds a small migration that transfer the old `cmsplugin-filer` plugins instances to the new `djangocms-<file|picture|link|...>` plugins.
```

### Comparing `djangocms-file-3.0.0/djangocms_file.egg-info/SOURCES.txt` & `djangocms-file-3.0.1/djangocms_file.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 djangocms_file/__init__.py
 djangocms_file/cms_plugins.py
 djangocms_file/models.py
 djangocms_file.egg-info/PKG-INFO
 djangocms_file.egg-info/SOURCES.txt
 djangocms_file.egg-info/dependency_links.txt
@@ -166,14 +167,15 @@
 djangocms_file/migrations/0005_auto_20160119_1534.py
 djangocms_file/migrations/0006_migrate_to_filer.py
 djangocms_file/migrations/0007_adapted_fields.py
 djangocms_file/migrations/0008_add_folder.py
 djangocms_file/migrations/0009_fixed_null_fields.py
 djangocms_file/migrations/0010_removed_null_fields.py
 djangocms_file/migrations/0011_auto_20181211_0357.py
+djangocms_file/migrations/0012_alter_file_cmsplugin_ptr_alter_folder_cmsplugin_ptr.py
 djangocms_file/migrations/__init__.py
 djangocms_file/templates/djangocms_file/default/file.html
 djangocms_file/templates/djangocms_file/default/folder.html
 tests/__init__.py
 tests/helpers.py
 tests/settings.py
 tests/test_migrations.py
```

### Comparing `djangocms-file-3.0.0/tests/helpers.py` & `djangocms-file-3.0.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/tests/test_migrations.py` & `djangocms-file-3.0.1/tests/test_migrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             'interactive': False,
             'dry_run': True,
             'stdout': output,
             'check_changes': True,
         }
 
         try:
-            call_command('makemigrations', **options)
+            call_command('makemigrations', 'djangocms_file', **options)
         except SystemExit as e:
             status_code = str(e)
         else:
             # the "no changes" exit code is 0
             status_code = '0'
 
         if status_code == '1':
```

### Comparing `djangocms-file-3.0.0/tests/test_models.py` & `djangocms-file-3.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-file-3.0.0/tests/test_plugins.py` & `djangocms-file-3.0.1/tests/test_plugins.py`

 * *Files identical despite different names*

