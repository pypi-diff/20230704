# Comparing `tmp/django-registration-3.3.tar.gz` & `tmp/django-registration-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-registration-3.3.tar", last modified: Sat May 28 07:31:02 2022, max compression
+gzip compressed data, was "django-registration-3.4.tar", last modified: Tue Jul  4 01:25:24 2023, max compression
```

## Comparing `django-registration-3.3.tar` & `django-registration-3.4.tar`

### file list

```diff
@@ -1,206 +1,215 @@
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.480893 django-registration-3.3/
--rw-r--r--   0 james      (503) staff       (20)     1102 2018-01-21 12:32:28.000000 django-registration-3.3/AUTHORS
--rw-r--r--   0 james      (503) staff       (20)     1523 2022-05-28 07:04:58.000000 django-registration-3.3/LICENSE
--rw-r--r--   0 james      (503) staff       (20)      135 2020-02-16 19:24:54.000000 django-registration-3.3/MANIFEST.in
--rw-r--r--   0 james      (503) staff       (20)     1694 2022-05-28 07:31:02.481035 django-registration-3.3/PKG-INFO
--rw-r--r--   0 james      (503) staff       (20)      578 2020-12-12 09:40:37.000000 django-registration-3.3/README.rst
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.443836 django-registration-3.3/docs/
--rw-r--r--   0 james      (503) staff       (20)     3019 2018-01-21 12:32:28.000000 django-registration-3.3/docs/Makefile
--rw-r--r--   0 james      (503) staff       (20)     9825 2020-01-26 21:43:52.000000 django-registration-3.3/docs/activation-workflow.rst
--rw-r--r--   0 james      (503) staff       (20)     1291 2022-05-28 07:05:12.000000 django-registration-3.3/docs/conf.py
--rw-r--r--   0 james      (503) staff       (20)     9783 2020-01-26 21:18:30.000000 django-registration-3.3/docs/custom-user.rst
--rw-r--r--   0 james      (503) staff       (20)      289 2018-09-02 13:00:29.000000 django-registration-3.3/docs/deprecations.rst
--rw-r--r--   0 james      (503) staff       (20)     1093 2018-09-02 13:00:29.000000 django-registration-3.3/docs/exceptions.rst
--rw-r--r--   0 james      (503) staff       (20)    10562 2022-05-28 07:06:14.000000 django-registration-3.3/docs/faq.rst
--rw-r--r--   0 james      (503) staff       (20)     4516 2020-01-26 22:03:56.000000 django-registration-3.3/docs/forms.rst
--rw-r--r--   0 james      (503) staff       (20)     1699 2020-09-22 08:32:22.000000 django-registration-3.3/docs/index.rst
--rw-r--r--   0 james      (503) staff       (20)     1833 2022-05-28 07:05:45.000000 django-registration-3.3/docs/install.rst
--rw-r--r--   0 james      (503) staff       (20)     2985 2018-01-21 12:32:28.000000 django-registration-3.3/docs/make.bat
--rw-r--r--   0 james      (503) staff       (20)     2987 2020-09-21 07:02:57.000000 django-registration-3.3/docs/one-step-workflow.rst
--rw-r--r--   0 james      (503) staff       (20)    12203 2021-06-20 23:27:16.000000 django-registration-3.3/docs/quickstart.rst
--rw-r--r--   0 james      (503) staff       (20)     7223 2020-01-26 22:07:41.000000 django-registration-3.3/docs/security.rst
--rw-r--r--   0 james      (503) staff       (20)     1834 2018-09-03 11:30:54.000000 django-registration-3.3/docs/settings.rst
--rw-r--r--   0 james      (503) staff       (20)     2676 2018-09-03 11:31:22.000000 django-registration-3.3/docs/signals.rst
--rw-r--r--   0 james      (503) staff       (20)      622 2022-05-28 07:24:51.000000 django-registration-3.3/docs/spelling_wordlist.txt
--rw-r--r--   0 james      (503) staff       (20)    13857 2022-05-28 07:18:04.000000 django-registration-3.3/docs/upgrade.rst
--rw-r--r--   0 james      (503) staff       (20)     8292 2020-01-02 07:25:53.000000 django-registration-3.3/docs/validators.rst
--rw-r--r--   0 james      (503) staff       (20)     6316 2020-01-26 21:52:05.000000 django-registration-3.3/docs/views.rst
--rw-r--r--   0 james      (503) staff       (20)     2728 2021-06-22 00:12:33.000000 django-registration-3.3/runtests.py
--rw-r--r--   0 james      (503) staff       (20)      410 2022-05-28 07:31:02.481715 django-registration-3.3/setup.cfg
--rw-r--r--   0 james      (503) staff       (20)     1478 2022-05-28 07:06:33.000000 django-registration-3.3/setup.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.423238 django-registration-3.3/src/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.446360 django-registration-3.3/src/django_registration/
--rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/__init__.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.449557 django-registration-3.3/src/django_registration/backends/
--rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/backends/__init__.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.450617 django-registration-3.3/src/django_registration/backends/activation/
--rw-r--r--   0 james      (503) staff       (20)      364 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/backends/activation/__init__.py
--rw-r--r--   0 james      (503) staff       (20)     1125 2020-12-12 07:50:04.000000 django-registration-3.3/src/django_registration/backends/activation/urls.py
--rw-r--r--   0 james      (503) staff       (20)     5734 2020-12-12 07:50:04.000000 django-registration-3.3/src/django_registration/backends/activation/views.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.451722 django-registration-3.3/src/django_registration/backends/one_step/
--rw-r--r--   0 james      (503) staff       (20)      380 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/backends/one_step/__init__.py
--rw-r--r--   0 james      (503) staff       (20)      741 2020-12-12 07:50:04.000000 django-registration-3.3/src/django_registration/backends/one_step/urls.py
--rw-r--r--   0 james      (503) staff       (20)     1104 2020-12-12 07:50:04.000000 django-registration-3.3/src/django_registration/backends/one_step/views.py
--rw-r--r--   0 james      (503) staff       (20)      485 2019-10-13 08:50:03.000000 django-registration-3.3/src/django_registration/exceptions.py
--rw-r--r--   0 james      (503) staff       (20)     3390 2020-12-12 07:50:04.000000 django-registration-3.3/src/django_registration/forms.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.433780 django-registration-3.3/src/django_registration/locale/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.424209 django-registration-3.3/src/django_registration/locale/ar/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.452753 django-registration-3.3/src/django_registration/locale/ar/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     2135 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2531 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.424605 django-registration-3.3/src/django_registration/locale/bg/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.453515 django-registration-3.3/src/django_registration/locale/bg/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     2302 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2682 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.424900 django-registration-3.3/src/django_registration/locale/ca/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.454326 django-registration-3.3/src/django_registration/locale/ca/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1953 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2454 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.425342 django-registration-3.3/src/django_registration/locale/cs/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.454928 django-registration-3.3/src/django_registration/locale/cs/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1963 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2393 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.425653 django-registration-3.3/src/django_registration/locale/da/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.455779 django-registration-3.3/src/django_registration/locale/da/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1803 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2228 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.425982 django-registration-3.3/src/django_registration/locale/de/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.456346 django-registration-3.3/src/django_registration/locale/de/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1999 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2426 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.426280 django-registration-3.3/src/django_registration/locale/el/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.457074 django-registration-3.3/src/django_registration/locale/el/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     2424 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2846 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.426648 django-registration-3.3/src/django_registration/locale/en/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.457651 django-registration-3.3/src/django_registration/locale/en/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      367 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     1721 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.426930 django-registration-3.3/src/django_registration/locale/es/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.458421 django-registration-3.3/src/django_registration/locale/es/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1949 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2383 2020-09-21 07:02:57.000000 django-registration-3.3/src/django_registration/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.427165 django-registration-3.3/src/django_registration/locale/es_AR/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.459008 django-registration-3.3/src/django_registration/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1849 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2265 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.427399 django-registration-3.3/src/django_registration/locale/fa/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.459777 django-registration-3.3/src/django_registration/locale/fa/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     2450 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2882 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.427729 django-registration-3.3/src/django_registration/locale/fr/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.460381 django-registration-3.3/src/django_registration/locale/fr/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     2012 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     3593 2020-09-21 07:02:57.000000 django-registration-3.3/src/django_registration/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.428120 django-registration-3.3/src/django_registration/locale/he/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.460976 django-registration-3.3/src/django_registration/locale/he/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1896 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2305 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.428461 django-registration-3.3/src/django_registration/locale/hr/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.461570 django-registration-3.3/src/django_registration/locale/hr/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1939 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2329 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.428784 django-registration-3.3/src/django_registration/locale/is/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.462245 django-registration-3.3/src/django_registration/locale/is/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1476 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/is/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     1899 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.429133 django-registration-3.3/src/django_registration/locale/it/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.462931 django-registration-3.3/src/django_registration/locale/it/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     2029 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2525 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.429501 django-registration-3.3/src/django_registration/locale/ja/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.463764 django-registration-3.3/src/django_registration/locale/ja/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     2035 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2425 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.429790 django-registration-3.3/src/django_registration/locale/ko/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.464720 django-registration-3.3/src/django_registration/locale/ko/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     2030 2021-04-01 05:00:01.000000 django-registration-3.3/src/django_registration/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2588 2021-04-01 05:00:01.000000 django-registration-3.3/src/django_registration/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.430042 django-registration-3.3/src/django_registration/locale/nb/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.465539 django-registration-3.3/src/django_registration/locale/nb/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1891 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2303 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.430294 django-registration-3.3/src/django_registration/locale/nl/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.466411 django-registration-3.3/src/django_registration/locale/nl/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1898 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2279 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.430764 django-registration-3.3/src/django_registration/locale/pl/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.467206 django-registration-3.3/src/django_registration/locale/pl/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1769 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2213 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.431160 django-registration-3.3/src/django_registration/locale/pt/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.467984 django-registration-3.3/src/django_registration/locale/pt/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1895 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2290 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.431475 django-registration-3.3/src/django_registration/locale/pt_BR/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.468695 django-registration-3.3/src/django_registration/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1796 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2217 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.432032 django-registration-3.3/src/django_registration/locale/ru/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.469512 django-registration-3.3/src/django_registration/locale/ru/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     2470 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2877 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.432442 django-registration-3.3/src/django_registration/locale/sl/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.470099 django-registration-3.3/src/django_registration/locale/sl/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1889 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2281 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.432798 django-registration-3.3/src/django_registration/locale/sr/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.470700 django-registration-3.3/src/django_registration/locale/sr/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1966 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2357 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.433112 django-registration-3.3/src/django_registration/locale/sv/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.471269 django-registration-3.3/src/django_registration/locale/sv/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1687 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2129 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.433372 django-registration-3.3/src/django_registration/locale/tr_TR/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.471861 django-registration-3.3/src/django_registration/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1945 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2359 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/tr_TR/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.433623 django-registration-3.3/src/django_registration/locale/zh_CN/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.472434 django-registration-3.3/src/django_registration/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1669 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2045 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.433881 django-registration-3.3/src/django_registration/locale/zh_TW/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.473017 django-registration-3.3/src/django_registration/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1669 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     2045 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.473596 django-registration-3.3/src/django_registration/migrations/
--rw-r--r--   0 james      (503) staff       (20)      745 2020-12-12 07:50:04.000000 django-registration-3.3/src/django_registration/migrations/0001_initial.py
--rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.3/src/django_registration/migrations/__init__.py
--rw-r--r--   0 james      (503) staff       (20)      304 2020-12-12 12:22:33.000000 django-registration-3.3/src/django_registration/signals.py
--rw-r--r--   0 james      (503) staff       (20)     9218 2020-12-12 07:50:04.000000 django-registration-3.3/src/django_registration/validators.py
--rw-r--r--   0 james      (503) staff       (20)     5428 2021-04-01 05:00:01.000000 django-registration-3.3/src/django_registration/views.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.449265 django-registration-3.3/src/django_registration.egg-info/
--rw-r--r--   0 james      (503) staff       (20)     1694 2022-05-28 07:31:01.000000 django-registration-3.3/src/django_registration.egg-info/PKG-INFO
--rw-r--r--   0 james      (503) staff       (20)     5572 2022-05-28 07:31:02.000000 django-registration-3.3/src/django_registration.egg-info/SOURCES.txt
--rw-r--r--   0 james      (503) staff       (20)        1 2022-05-28 07:31:01.000000 django-registration-3.3/src/django_registration.egg-info/dependency_links.txt
--rw-r--r--   0 james      (503) staff       (20)        1 2022-05-28 07:31:00.000000 django-registration-3.3/src/django_registration.egg-info/not-zip-safe
--rw-r--r--   0 james      (503) staff       (20)       39 2022-05-28 07:31:02.000000 django-registration-3.3/src/django_registration.egg-info/requires.txt
--rw-r--r--   0 james      (503) staff       (20)       20 2022-05-28 07:31:02.000000 django-registration-3.3/src/django_registration.egg-info/top_level.txt
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.475984 django-registration-3.3/tests/
--rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.3/tests/__init__.py
--rw-r--r--   0 james      (503) staff       (20)     8458 2020-01-26 22:22:38.000000 django-registration-3.3/tests/base.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.476724 django-registration-3.3/tests/migrations/
--rw-r--r--   0 james      (503) staff       (20)     3287 2020-01-05 10:43:59.000000 django-registration-3.3/tests/migrations/0001_initial.py
--rw-r--r--   0 james      (503) staff       (20)        0 2020-01-05 09:03:55.000000 django-registration-3.3/tests/migrations/__init__.py
--rw-r--r--   0 james      (503) staff       (20)     1785 2020-01-05 10:41:39.000000 django-registration-3.3/tests/models.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.434721 django-registration-3.3/tests/templates/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.479126 django-registration-3.3/tests/templates/django_registration/
--rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.3/tests/templates/django_registration/activation_complete.html
--rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.3/tests/templates/django_registration/activation_email_body.txt
--rw-r--r--   0 james      (503) staff       (20)       12 2018-09-02 13:00:29.000000 django-registration-3.3/tests/templates/django_registration/activation_email_subject.txt
--rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.3/tests/templates/django_registration/activation_failed.html
--rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.3/tests/templates/django_registration/registration_closed.html
--rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.3/tests/templates/django_registration/registration_complete.html
--rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.3/tests/templates/django_registration/registration_form.html
--rw-r--r--   0 james      (503) staff       (20)     9482 2020-09-21 07:27:26.000000 django-registration-3.3/tests/test_activation_workflow.py
--rw-r--r--   0 james      (503) staff       (20)    13439 2020-09-21 07:27:16.000000 django-registration-3.3/tests/test_forms.py
--rw-r--r--   0 james      (503) staff       (20)     2270 2020-01-05 10:55:59.000000 django-registration-3.3/tests/test_one_step_workflow.py
--rw-r--r--   0 james      (503) staff       (20)     5168 2021-04-01 05:00:01.000000 django-registration-3.3/tests/test_views.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-28 07:31:02.480556 django-registration-3.3/tests/urls/
--rw-r--r--   0 james      (503) staff       (20)        0 2020-01-05 10:34:51.000000 django-registration-3.3/tests/urls/__init__.py
--rw-r--r--   0 james      (503) staff       (20)     1441 2020-01-05 10:37:25.000000 django-registration-3.3/tests/urls/custom_user_activation.py
--rw-r--r--   0 james      (503) staff       (20)     1076 2020-01-05 10:37:30.000000 django-registration-3.3/tests/urls/custom_user_one_step.py
--rw-r--r--   0 james      (503) staff       (20)     1433 2020-12-12 07:50:04.000000 django-registration-3.3/tests/urls/view_tests.py
--rw-r--r--   0 james      (503) staff       (20)      352 2019-10-13 08:53:22.000000 django-registration-3.3/tests/views.py
--rw-r--r--   0 james      (503) staff       (20)     6618 2022-05-28 07:13:29.000000 django-registration-3.3/tox.ini
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.748335 django-registration-3.4/
+-rw-r--r--   0 james      (503) staff       (20)      299 2023-06-10 07:20:29.000000 django-registration-3.4/.editorconfig
+-rw-r--r--   0 james      (503) staff       (20)      107 2023-06-10 07:20:29.000000 django-registration-3.4/.flake8
+-rw-r--r--   0 james      (503) staff       (20)     1041 2023-06-10 07:20:29.000000 django-registration-3.4/.pre-commit-config.yaml
+-rw-r--r--   0 james      (503) staff       (20)      295 2023-06-10 07:20:29.000000 django-registration-3.4/.readthedocs.yaml
+-rw-r--r--   0 james      (503) staff       (20)     1102 2018-01-21 12:32:28.000000 django-registration-3.4/AUTHORS
+-rw-r--r--   0 james      (503) staff       (20)     1523 2022-05-28 07:04:58.000000 django-registration-3.4/LICENSE
+-rw-r--r--   0 james      (503) staff       (20)      293 2023-06-10 07:20:29.000000 django-registration-3.4/MANIFEST.in
+-rw-r--r--   0 james      (503) staff       (20)     1877 2023-07-04 01:25:24.748204 django-registration-3.4/PKG-INFO
+-rw-r--r--   0 james      (503) staff       (20)      578 2020-12-12 09:40:37.000000 django-registration-3.4/README.rst
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.735934 django-registration-3.4/docs/
+-rw-r--r--   0 james      (503) staff       (20)     3019 2018-01-21 12:32:28.000000 django-registration-3.4/docs/Makefile
+-rw-r--r--   0 james      (503) staff       (20)     9820 2023-06-18 07:59:21.000000 django-registration-3.4/docs/activation-workflow.rst
+-rw-r--r--   0 james      (503) staff       (20)     1640 2023-07-04 01:13:13.000000 django-registration-3.4/docs/conf.py
+-rw-r--r--   0 james      (503) staff       (20)     9788 2023-06-18 08:00:03.000000 django-registration-3.4/docs/custom-user.rst
+-rw-r--r--   0 james      (503) staff       (20)      290 2023-06-11 23:07:37.000000 django-registration-3.4/docs/deprecations.rst
+-rw-r--r--   0 james      (503) staff       (20)      106 2023-06-10 07:20:29.000000 django-registration-3.4/docs/docs_settings.py
+-rw-r--r--   0 james      (503) staff       (20)     1088 2023-06-11 23:09:54.000000 django-registration-3.4/docs/exceptions.rst
+-rw-r--r--   0 james      (503) staff       (20)    10835 2023-06-18 08:11:37.000000 django-registration-3.4/docs/faq.rst
+-rw-r--r--   0 james      (503) staff       (20)     4506 2023-06-18 08:02:40.000000 django-registration-3.4/docs/forms.rst
+-rw-r--r--   0 james      (503) staff       (20)     1699 2023-06-11 23:11:08.000000 django-registration-3.4/docs/index.rst
+-rw-r--r--   0 james      (503) staff       (20)     2228 2023-06-10 07:20:29.000000 django-registration-3.4/docs/install.rst
+-rw-r--r--   0 james      (503) staff       (20)     2985 2018-01-21 12:32:28.000000 django-registration-3.4/docs/make.bat
+-rw-r--r--   0 james      (503) staff       (20)     2995 2023-06-18 08:03:26.000000 django-registration-3.4/docs/one-step-workflow.rst
+-rw-r--r--   0 james      (503) staff       (20)    12288 2023-06-16 23:25:38.000000 django-registration-3.4/docs/quickstart.rst
+-rw-r--r--   0 james      (503) staff       (20)     7234 2023-06-11 23:16:43.000000 django-registration-3.4/docs/security.rst
+-rw-r--r--   0 james      (503) staff       (20)     1847 2023-06-18 08:10:10.000000 django-registration-3.4/docs/settings.rst
+-rw-r--r--   0 james      (503) staff       (20)     2683 2023-06-18 08:05:09.000000 django-registration-3.4/docs/signals.rst
+-rw-r--r--   0 james      (503) staff       (20)      630 2023-06-12 01:29:22.000000 django-registration-3.4/docs/spelling_wordlist.txt
+-rw-r--r--   0 james      (503) staff       (20)    15013 2023-07-04 01:04:24.000000 django-registration-3.4/docs/upgrade.rst
+-rw-r--r--   0 james      (503) staff       (20)     8294 2023-06-18 08:08:07.000000 django-registration-3.4/docs/validators.rst
+-rw-r--r--   0 james      (503) staff       (20)     6281 2023-06-18 08:09:16.000000 django-registration-3.4/docs/views.rst
+-rw-r--r--   0 james      (503) staff       (20)    11068 2023-06-10 22:06:31.000000 django-registration-3.4/noxfile.py
+-rw-r--r--   0 james      (503) staff       (20)     2366 2023-06-10 22:20:29.000000 django-registration-3.4/pyproject.toml
+-rw-r--r--   0 james      (503) staff       (20)      288 2023-06-10 07:20:29.000000 django-registration-3.4/runtests.py
+-rw-r--r--   0 james      (503) staff       (20)       38 2023-07-04 01:25:24.748378 django-registration-3.4/setup.cfg
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.727816 django-registration-3.4/src/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.736624 django-registration-3.4/src/django_registration/
+-rw-r--r--   0 james      (503) staff       (20)       86 2023-07-04 01:13:01.000000 django-registration-3.4/src/django_registration/__init__.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.737360 django-registration-3.4/src/django_registration/backends/
+-rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/backends/__init__.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.737713 django-registration-3.4/src/django_registration/backends/activation/
+-rw-r--r--   0 james      (503) staff       (20)      364 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/backends/activation/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)     1125 2020-12-12 07:50:04.000000 django-registration-3.4/src/django_registration/backends/activation/urls.py
+-rw-r--r--   0 james      (503) staff       (20)     5972 2023-06-10 07:20:29.000000 django-registration-3.4/src/django_registration/backends/activation/views.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.738079 django-registration-3.4/src/django_registration/backends/one_step/
+-rw-r--r--   0 james      (503) staff       (20)      380 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/backends/one_step/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)      741 2020-12-12 07:50:04.000000 django-registration-3.4/src/django_registration/backends/one_step/urls.py
+-rw-r--r--   0 james      (503) staff       (20)     1194 2023-06-10 07:20:29.000000 django-registration-3.4/src/django_registration/backends/one_step/views.py
+-rw-r--r--   0 james      (503) staff       (20)      452 2023-06-10 07:20:29.000000 django-registration-3.4/src/django_registration/exceptions.py
+-rw-r--r--   0 james      (503) staff       (20)     3840 2023-06-12 06:50:34.000000 django-registration-3.4/src/django_registration/forms.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.731762 django-registration-3.4/src/django_registration/locale/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.728191 django-registration-3.4/src/django_registration/locale/ar/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.738318 django-registration-3.4/src/django_registration/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     2135 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2531 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.728307 django-registration-3.4/src/django_registration/locale/bg/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.738569 django-registration-3.4/src/django_registration/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     2302 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2682 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.728419 django-registration-3.4/src/django_registration/locale/ca/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.738801 django-registration-3.4/src/django_registration/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1953 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2454 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.728532 django-registration-3.4/src/django_registration/locale/cs/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.739061 django-registration-3.4/src/django_registration/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1963 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2393 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.728652 django-registration-3.4/src/django_registration/locale/da/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.739306 django-registration-3.4/src/django_registration/locale/da/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1803 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2228 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.728762 django-registration-3.4/src/django_registration/locale/de/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.739530 django-registration-3.4/src/django_registration/locale/de/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1999 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2426 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.728897 django-registration-3.4/src/django_registration/locale/el/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.739764 django-registration-3.4/src/django_registration/locale/el/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     2424 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2846 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.729022 django-registration-3.4/src/django_registration/locale/en/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.739996 django-registration-3.4/src/django_registration/locale/en/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      367 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     1721 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.729151 django-registration-3.4/src/django_registration/locale/es/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.740232 django-registration-3.4/src/django_registration/locale/es/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1949 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2383 2020-09-21 07:02:57.000000 django-registration-3.4/src/django_registration/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.729265 django-registration-3.4/src/django_registration/locale/es_AR/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.740458 django-registration-3.4/src/django_registration/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1849 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2265 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.729384 django-registration-3.4/src/django_registration/locale/fa/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.740696 django-registration-3.4/src/django_registration/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     2450 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2882 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.729501 django-registration-3.4/src/django_registration/locale/fr/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.740920 django-registration-3.4/src/django_registration/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     2012 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     3593 2020-09-21 07:02:57.000000 django-registration-3.4/src/django_registration/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.729642 django-registration-3.4/src/django_registration/locale/he/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.741157 django-registration-3.4/src/django_registration/locale/he/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1896 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2305 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.729773 django-registration-3.4/src/django_registration/locale/hr/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.741382 django-registration-3.4/src/django_registration/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1939 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2329 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.729907 django-registration-3.4/src/django_registration/locale/id/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.741630 django-registration-3.4/src/django_registration/locale/id/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     2039 2023-05-22 06:08:44.000000 django-registration-3.4/src/django_registration/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2561 2023-05-22 06:08:44.000000 django-registration-3.4/src/django_registration/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.730025 django-registration-3.4/src/django_registration/locale/is/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.741861 django-registration-3.4/src/django_registration/locale/is/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1476 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/is/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     1899 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.730162 django-registration-3.4/src/django_registration/locale/it/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.742087 django-registration-3.4/src/django_registration/locale/it/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     2029 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2525 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.730286 django-registration-3.4/src/django_registration/locale/ja/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.742322 django-registration-3.4/src/django_registration/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     2035 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2425 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.730398 django-registration-3.4/src/django_registration/locale/ko/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.742540 django-registration-3.4/src/django_registration/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     2030 2021-04-01 05:00:01.000000 django-registration-3.4/src/django_registration/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2588 2021-04-01 05:00:01.000000 django-registration-3.4/src/django_registration/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.730531 django-registration-3.4/src/django_registration/locale/nb/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.742770 django-registration-3.4/src/django_registration/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1891 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2303 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.730649 django-registration-3.4/src/django_registration/locale/nl/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.742987 django-registration-3.4/src/django_registration/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1898 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2279 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.730757 django-registration-3.4/src/django_registration/locale/pl/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.743221 django-registration-3.4/src/django_registration/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1769 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2213 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.730876 django-registration-3.4/src/django_registration/locale/pt/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.743449 django-registration-3.4/src/django_registration/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1895 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2290 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.730983 django-registration-3.4/src/django_registration/locale/pt_BR/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.743669 django-registration-3.4/src/django_registration/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1796 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2217 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.731097 django-registration-3.4/src/django_registration/locale/ru/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.743902 django-registration-3.4/src/django_registration/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     2470 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2877 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.731232 django-registration-3.4/src/django_registration/locale/sl/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.744136 django-registration-3.4/src/django_registration/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1889 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2281 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.731356 django-registration-3.4/src/django_registration/locale/sr/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.744362 django-registration-3.4/src/django_registration/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1966 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2357 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.731468 django-registration-3.4/src/django_registration/locale/sv/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.744591 django-registration-3.4/src/django_registration/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1687 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2129 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.731578 django-registration-3.4/src/django_registration/locale/tr_TR/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.744819 django-registration-3.4/src/django_registration/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1945 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2359 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/tr_TR/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.731692 django-registration-3.4/src/django_registration/locale/zh_CN/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.745049 django-registration-3.4/src/django_registration/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1669 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2045 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.731808 django-registration-3.4/src/django_registration/locale/zh_TW/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.745267 django-registration-3.4/src/django_registration/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1669 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     2045 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.745502 django-registration-3.4/src/django_registration/migrations/
+-rw-r--r--   0 james      (503) staff       (20)      775 2023-06-10 07:20:29.000000 django-registration-3.4/src/django_registration/migrations/0001_initial.py
+-rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.4/src/django_registration/migrations/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)      304 2020-12-12 12:22:33.000000 django-registration-3.4/src/django_registration/signals.py
+-rw-r--r--   0 james      (503) staff       (20)     9362 2023-06-11 23:03:55.000000 django-registration-3.4/src/django_registration/validators.py
+-rw-r--r--   0 james      (503) staff       (20)     5645 2023-06-10 07:20:29.000000 django-registration-3.4/src/django_registration/views.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.737228 django-registration-3.4/src/django_registration.egg-info/
+-rw-r--r--   0 james      (503) staff       (20)     1877 2023-07-04 01:25:24.000000 django-registration-3.4/src/django_registration.egg-info/PKG-INFO
+-rw-r--r--   0 james      (503) staff       (20)     5741 2023-07-04 01:25:24.000000 django-registration-3.4/src/django_registration.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (503) staff       (20)        1 2023-07-04 01:25:24.000000 django-registration-3.4/src/django_registration.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (503) staff       (20)      232 2023-07-04 01:25:24.000000 django-registration-3.4/src/django_registration.egg-info/requires.txt
+-rw-r--r--   0 james      (503) staff       (20)       20 2023-07-04 01:25:24.000000 django-registration-3.4/src/django_registration.egg-info/top_level.txt
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.746484 django-registration-3.4/tests/
+-rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.4/tests/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)     8728 2023-06-12 01:34:58.000000 django-registration-3.4/tests/base.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.746728 django-registration-3.4/tests/migrations/
+-rw-r--r--   0 james      (503) staff       (20)     3317 2023-06-10 07:20:29.000000 django-registration-3.4/tests/migrations/0001_initial.py
+-rw-r--r--   0 james      (503) staff       (20)        0 2020-01-05 09:03:55.000000 django-registration-3.4/tests/migrations/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)     1849 2023-06-10 07:20:29.000000 django-registration-3.4/tests/models.py
+-rw-r--r--   0 james      (503) staff       (20)     1482 2023-06-10 07:20:29.000000 django-registration-3.4/tests/settings.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.732119 django-registration-3.4/tests/templates/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.747514 django-registration-3.4/tests/templates/django_registration/
+-rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.4/tests/templates/django_registration/activation_complete.html
+-rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.4/tests/templates/django_registration/activation_email_body.txt
+-rw-r--r--   0 james      (503) staff       (20)       12 2018-09-02 13:00:29.000000 django-registration-3.4/tests/templates/django_registration/activation_email_subject.txt
+-rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.4/tests/templates/django_registration/activation_failed.html
+-rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.4/tests/templates/django_registration/registration_closed.html
+-rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.4/tests/templates/django_registration/registration_complete.html
+-rw-r--r--   0 james      (503) staff       (20)        0 2018-09-02 13:00:29.000000 django-registration-3.4/tests/templates/django_registration/registration_form.html
+-rw-r--r--   0 james      (503) staff       (20)     9282 2023-06-12 01:39:08.000000 django-registration-3.4/tests/test_activation_workflow.py
+-rw-r--r--   0 james      (503) staff       (20)    13742 2023-06-12 06:50:23.000000 django-registration-3.4/tests/test_forms.py
+-rw-r--r--   0 james      (503) staff       (20)     2247 2023-06-12 01:53:54.000000 django-registration-3.4/tests/test_one_step_workflow.py
+-rw-r--r--   0 james      (503) staff       (20)     5381 2023-06-12 02:00:24.000000 django-registration-3.4/tests/test_views.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-04 01:25:24.748005 django-registration-3.4/tests/urls/
+-rw-r--r--   0 james      (503) staff       (20)        0 2020-01-05 10:34:51.000000 django-registration-3.4/tests/urls/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)     1554 2023-06-10 07:20:29.000000 django-registration-3.4/tests/urls/custom_user_activation.py
+-rw-r--r--   0 james      (503) staff       (20)     1189 2023-06-10 07:20:29.000000 django-registration-3.4/tests/urls/custom_user_one_step.py
+-rw-r--r--   0 james      (503) staff       (20)     1433 2020-12-12 07:50:04.000000 django-registration-3.4/tests/urls/view_tests.py
+-rw-r--r--   0 james      (503) staff       (20)      451 2023-06-10 07:20:29.000000 django-registration-3.4/tests/views.py
```

### Comparing `django-registration-3.3/AUTHORS` & `django-registration-3.4/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/LICENSE` & `django-registration-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/PKG-INFO` & `django-registration-3.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 Metadata-Version: 2.1
 Name: django-registration
-Version: 3.3
-Summary: An extensible user-registration application for Django
-Home-page: https://github.com/ubernostrum/django-registration/
-Author: James Bennett
-Author-email: james@b-list.org
+Version: 3.4
+Summary: An extensible user-registration application for Django.
+Author-email: James Bennett <james@b-list.org>
+License: BSD-3-Clause
+Project-URL: documentation, https://django-registration.readthedocs.io/
+Project-URL: homepage, https://github.com/ubernostrum/django-registration
+Keywords: django,security,auth,authentication
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: tests
 License-File: LICENSE
+License-File: AUTHORS
 
 .. -*-restructuredtext-*-
 
 .. image:: https://github.com/ubernostrum/django-registration/workflows/CI/badge.svg
    :alt: CI status image
    :target: https://github.com/ubernostrum/django-registration/actions?query=workflow%3ACI
```

### Comparing `django-registration-3.3/README.rst` & `django-registration-3.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/docs/Makefile` & `django-registration-3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/docs/activation-workflow.rst` & `django-registration-3.4/docs/activation-workflow.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,255 +1,240 @@
 .. _activation-workflow:
 .. module:: django_registration.backends.activation
 
 The two-step activation workflow
 ================================
 
 The two-step activation workflow, found in
-`django_registration.backends.activation`, implements a two-step
-registration process: a user signs up, an inactive account is created,
-and an email is sent containing an activation link which must be
-clicked to make the account active.
+``django_registration.backends.activation``, implements a two-step registration
+process: a user signs up, an inactive account is created, and an email is sent
+containing an activation link which must be clicked to make the account active.
 
 
 Behavior and configuration
 --------------------------
 
-A default URLconf is provided, which you can
-:func:`~django.urls.include` in your URL configuration; that URLconf
-is `django_registration.backends.activation.urls`. For example, to
-place user registration under the URL prefix `/accounts/`, you could
-place the following in your root URLconf:
+A default URLconf is provided, which you can :func:`~django.urls.include` in
+your URL configuration; that URLconf is
+``django_registration.backends.activation.urls``. For example, to place user
+registration under the URL prefix ``/accounts/``, you could place the following
+in your root URLconf:
 
 .. code-block:: python
 
    from django.urls import include, path
 
    urlpatterns = [
        # Other URL patterns ...
        path('accounts/', include('django_registration.backends.activation.urls')),
        path('accounts/', include('django.contrib.auth.urls')),
        # More URL patterns ...
    ]
 
-That also sets up the views from `django.contrib.auth` (login, logout,
-password reset, etc.).
+That also sets up the views from ``django.contrib.auth`` (login, logout, password
+reset, etc.).
 
-This workflow makes use of up to three settings (click for details on
-each):
+This workflow makes use of up to three settings (click for details on each):
 
 * :data:`~django.conf.settings.ACCOUNT_ACTIVATION_DAYS`
 
 * :data:`~django.conf.settings.REGISTRATION_OPEN`
 
-* :data:`~django.conf.settings.REGISTRATION_SALT` (see also :ref:`note
-  below <salt-security>`)
+* :data:`~django.conf.settings.REGISTRATION_SALT` (see also :ref:`note below
+  <salt-security>`)
 
 By default, this workflow uses
-:class:`~django_registration.forms.RegistrationForm` as its form class
-for user registration; this can be overridden by passing the keyword
-argument `form_class` to the registration view.
+:class:`~django_registration.forms.RegistrationForm` as its form class for user
+registration; this can be overridden by passing the keyword argument
+``form_class`` to the registration view.
 
 
 Views
 -----
 
 .. currentmodule:: django_registration.backends.activation.views
 
-Two views are provided to implement the signup/activation
-process. These subclass :ref:`the base views of django-registration
-<views>`, so anything that can be overridden/customized there can
-equally be overridden/customized here. There are some additional
-customization points specific to this implementation, which are listed
-below.
+Two views are provided to implement the signup/activation process. These
+subclass :ref:`the base views of django-registration <views>`, so anything that
+can be overridden/customized there can equally be overridden/customized
+here. There are some additional customization points specific to this
+implementation, which are listed below.
 
 For an overview of the templates used by these views (other than those
-specified below), and their context variables, see :ref:`the quick
-start guide <default-templates>`.
+specified below), and their context variables, see :ref:`the quick start guide
+<default-templates>`.
 
 
 .. class:: RegistrationView
 
    A subclass of :class:`django_registration.views.RegistrationView`
    implementing the signup portion of this workflow.
 
    Important customization points unique to this class are:
 
    .. method:: create_inactive_user(form)
 
       Creates and returns an inactive user account, and calls
-      :meth:`send_activation_email()` to send the email with the
-      activation key. The argument `form` is a valid registration
-      form instance passed from
-      :meth:`~django_registration.views.RegistrationView.register()`.
+      :meth:`send_activation_email()` to send the email with the activation
+      key. The argument ``form`` is a valid registration form instance passed
+      from :meth:`~django_registration.views.RegistrationView.register()`.
 
       :param django_registration.forms.RegistrationForm form: The registration form.
       :rtype: django.contrib.auth.models.AbstractUser
 
    .. method:: get_activation_key(user)
 
-      Given an instance of the user model, generates and returns an
-      activation key (a string) for that user account.
+      Given an instance of the user model, generates and returns an activation
+      key (a string) for that user account.
 
       :param django.contrib.auth.models.AbstractUser user: The new user account.
       :rtype: str
 
    .. method:: get_email_context(activation_key)
 
-      Returns a dictionary of values to be used as template context
-      when generating the activation email.
+      Returns a dictionary of values to be used as template context when
+      generating the activation email.
 
       :param str activation_key: The activation key for the new user account.
       :rtype: dict
 
    .. method:: send_activation_email(user)
 
-      Given an inactive user account, generates and sends the
-      activation email for that account.
+      Given an inactive user account, generates and sends the activation email
+      for that account.
 
       :param django.contrib.auth.models.AbstractUser user: The new user account.
       :rtype: None
-      
+
    .. attribute:: email_body_template
 
-      A string specifying the template to use for the body of the
-      activation email. Default is
-      `"django_registration/activation_email_body.txt"`.
+      A string specifying the template to use for the body of the activation
+      email. Default is ``"django_registration/activation_email_body.txt"``.
 
    .. attribute:: email_subject_template
 
-      A string specifying the template to use for the subject of the
-      activation email. Default is
-      `"django_registration/activation_email_subject.txt"`. Note that, to
-      avoid `header-injection vulnerabilities
+      A string specifying the template to use for the subject of the activation
+      email. Default is
+      ``"django_registration/activation_email_subject.txt"``. Note that, to avoid
+      `header-injection vulnerabilities
       <https://en.wikipedia.org/wiki/Email_injection>`_, the result of
-      rendering this template will be forced into a single line of
-      text, stripping newline characters.
+      rendering this template will be forced into a single line of text,
+      stripping newline characters.
 
 .. class:: ActivationView
 
-   A subclass of :class:`django_registration.views.ActivationView`
-   implementing the activation portion of this workflow.
+   A subclass of :class:`django_registration.views.ActivationView` implementing
+   the activation portion of this workflow.
 
    Errors in activating the user account will raise
-   :exc:`~django_registration.exceptions.ActivationError`, with one
-   of the following values for the exception's `code`:
+   :exc:`~django_registration.exceptions.ActivationError`, with one of the
+   following values for the exception's ``code``:
 
-   `"already_activated"`
+   ``"already_activated"``
        Indicates the account has already been activated.
-   
-   `"bad_username"`
-       Indicates the username decoded from the activation key is
-       invalid (does not correspond to any user account).
 
-   `"expired"`
+   ``"bad_username"``
+       Indicates the username decoded from the activation key is invalid (does
+       not correspond to any user account).
+
+   ``"expired"``
        Indicates the account/activation key has expired.
 
-   `"invalid_key"`
+   ``"invalid_key"``
       Generic indicator that the activation key was invalid.
 
    Important customization points unique to this class are:
 
    .. method:: get_user(username)
 
-      Given a username (determined by the activation key), looks up
-      and returns the corresponding instance of the user model. If no
-      such account exists, raises
-      :exc:`~django_registration.exceptions.ActivationError` as
+      Given a username (determined by the activation key), looks up and returns
+      the corresponding instance of the user model. If no such account exists,
+      raises :exc:`~django_registration.exceptions.ActivationError` as
       described above. In the base implementation, checks the
-      :attr:`~django.contrib.auth.models.User.is_active` field to
-      avoid re-activating already-active accounts, and raises
+      :attr:`~django.contrib.auth.models.User.is_active` field to avoid
+      re-activating already-active accounts, and raises
       :exc:`~django_registration.exceptions.ActivationError` with code
-      `already_activated` to indicate this case.
+      ``already_activated`` to indicate this case.
 
       :param str username: The username of the new user account.
       :rtype: django.contrib.auth.models.AbstractUser
       :raises django_registration.exceptions.ActivationError: if no
          matching inactive user account exists.
-      
+
    .. method:: validate_key(activation_key)
 
-      Given the activation key, verifies that it carries a valid
-      signature and a timestamp no older than the number of days
-      specified in the setting `ACCOUNT_ACTIVATION_DAYS`, and
-      returns the username from the activation key. Raises
-      :exc:`~django_registration.exceptions.ActivationError`, as
-      described above, if the activation key has an invalid signature
-      or if the timestamp is too old.
+      Given the activation key, verifies that it carries a valid signature and
+      a timestamp no older than the number of days specified in the setting
+      ``ACCOUNT_ACTIVATION_DAYS``, and returns the username from the activation
+      key. Raises :exc:`~django_registration.exceptions.ActivationError`, as
+      described above, if the activation key has an invalid signature or if the
+      timestamp is too old.
 
       :param str activation_key: The activation key for the new user account.
       :rtype: str
       :raises django_registration.exceptions.ActivationError: if the
          activation key has an invalid signature or is expired.
 
    .. note:: **URL patterns for activation**
 
-      Although the actual value used in the activation key is the new
-      user account's username, the URL pattern for
-      :class:`~views.ActivationView` does not need to match all
-      possible legal characters in a username. The activation key that
-      will be sent to the user (and thus matched in the URL) is
-      produced by :func:`django.core.signing.dumps()`, which
-      base64-encodes its output. Thus, the only characters this
-      pattern needs to match are those from `the URL-safe base64
-      alphabet <http://tools.ietf.org/html/rfc4648#section-5>`_, plus
-      the colon ("`:`") which is used as a separator.
+      Although the actual value used in the activation key is the new user
+      account's username, the URL pattern for :class:`~views.ActivationView`
+      does not need to match all possible legal characters in a username. The
+      activation key that will be sent to the user (and thus matched in the
+      URL) is produced by :func:`django.core.signing.dumps()`, which
+      base64-encodes its output. Thus, the only characters this pattern needs
+      to match are those from `the URL-safe base64 alphabet
+      <http://tools.ietf.org/html/rfc4648#section-5>`_, plus the colon ("``:``")
+      which is used as a separator.
 
       The default URL pattern for the activation view in
-      `django_registration.backends.activation.urls` handles this for
-      you.
+      ``django_registration.backends.activation.urls`` handles this for you.
 
 
 How it works
 ------------
 
-When a user signs up, the activation workflow creates a new user
-instance to represent the account, and sets the `is_active` field to
-:data:`False`. It then sends an email to the address provided during
-signup, containing a link to activate the account. When the user
-clicks the link, the activation view sets `is_active` to :data:`True`,
-after which the user can log in.
-
-The activation key is the username of the new account, signed using
-`Django's cryptographic signing tools
-<https://docs.djangoproject.com/en/stable/topics/signing/>`_
-(specifically, :func:`~django.core.signing.dumps()` is used, to
-produce a guaranteed-URL-safe value). The activation process includes
-verification of the signature prior to activation, as well as
-verifying that the user is activating within the permitted window (as
-specified in the setting
-:data:`~django.conf.settings.ACCOUNT_ACTIVATION_DAYS`, mentioned
-above), through use of Django's
-:class:`~django.core.signing.TimestampSigner`.
+When a user signs up, the activation workflow creates a new user instance to
+represent the account, and sets the ``is_active`` field to :data:`False`. It then
+sends an email to the address provided during signup, containing a link to
+activate the account. When the user clicks the link, the activation view sets
+``is_active`` to :data:`True`, after which the user can log in.
+
+The activation key is the username of the new account, signed using `Django's
+cryptographic signing tools
+<https://docs.djangoproject.com/en/stable/topics/signing/>`_ (specifically,
+:func:`~django.core.signing.dumps()` is used, to produce a guaranteed-URL-safe
+value). The activation process includes verification of the signature prior to
+activation, as well as verifying that the user is activating within the
+permitted window (as specified in the setting
+:data:`~django.conf.settings.ACCOUNT_ACTIVATION_DAYS`, mentioned above),
+through use of Django's :class:`~django.core.signing.TimestampSigner`.
 
 
 Security considerations
 -----------------------
 
-The activation key emailed to the user in the activation workflow
-is a value obtained by using Django's cryptographic signing tools. The
-activation key is of the form::
+The activation key emailed to the user in the activation workflow is a value
+obtained by using Django's cryptographic signing tools. The activation key is
+of the form::
 
     encoded_username:timestamp:signature
 
-where `encoded_username` is the username of the new account,
-`timestamp` is the timestamp of the time the user registered, and
-`signature` is an HMAC of the username and timestamp. The username and
-HMAC will be URL-safe base64 encoded; the timestamp will be base62
-encoded.
+where ``encoded_username`` is the username of the new account, ``timestamp`` is the
+timestamp of the time the user registered, and ``signature`` is an HMAC of the
+username and timestamp. The username and HMAC will be URL-safe base64 encoded;
+the timestamp will be base62 encoded.
 
 Django's implementation uses the value of the
 :data:`~django.conf.settings.SECRET_KEY` setting as the key for HMAC;
-additionally, it permits the specification of a salt value which can
-be used to "namespace" different uses of HMAC across a Django-powered
-site.
+additionally, it permits the specification of a salt value which can be used to
+"namespace" different uses of HMAC across a Django-powered site.
 
 .. _salt-security:
 
 The activation workflow will use the value (a string) of the setting
-:data:`~django.conf.settings.REGISTRATION_SALT` as the salt,
-defaulting to the string `"registration"` if that setting is not
-specified. This value does *not* need to be kept secret (only
-:data:`~django.conf.settings.SECRET_KEY` does); it serves only to
-ensure that other parts of a site which also produce signed values
-from user input could not be used as a way to generate activation keys
+:data:`~django.conf.settings.REGISTRATION_SALT` as the salt, defaulting to the
+string ``"registration"`` if that setting is not specified. This value does *not*
+need to be kept secret (only :data:`~django.conf.settings.SECRET_KEY` does); it
+serves only to ensure that other parts of a site which also produce signed
+values from user input could not be used as a way to generate activation keys
 for arbitrary usernames (and vice-versa).
```

### Comparing `django-registration-3.3/docs/conf.py` & `django-registration-3.4/docs/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,37 @@
+"""
+Configuration file for the Sphinx documentation builder:
+
+https://www.sphinx-doc.org/
+
+"""
 import os
 import sys
 
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
-
-extensions = ["sphinx.ext.intersphinx"]
+extensions = [
+    "notfound.extension",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.viewcode",
+    "sphinxcontrib_django",
+    "sphinxext.opengraph",
+    "sphinx_copybutton",
+    "sphinx_inline_tabs",
+]
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 project = "django-registration"
-copyright = "2007-2022, James Bennett"
-version = "3.3"
-release = "3.3"
+copyright = "2007, James Bennett"
+version = "3.4"
+release = "3.4"
 exclude_trees = ["_build"]
 pygments_style = "sphinx"
 htmlhelp_basename = "django-registrationdoc"
+html_theme = "furo"
 latex_documents = [
     (
         "index",
         "django-registration.tex",
         "django-registration Documentation",
         "James Bennett",
         "manual",
@@ -28,23 +42,25 @@
     "django": (
         "https://docs.djangoproject.com/en/stable/",
         "https://docs.djangoproject.com/en/stable/_objects/",
     ),
     "python": ("https://docs.python.org/3", None),
 }
 
-if not on_rtd:
-    import sphinx_rtd_theme
-
-    html_theme = "sphinx_rtd_theme"
-    html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
-
 # Spelling check needs an additional module that is not installed by default.
 # Add it only if spelling check is requested so docs can be generated without it.
 if "spelling" in sys.argv:
     extensions.append("sphinxcontrib.spelling")
 
 # Spelling language.
 spelling_lang = "en_US"
 
 # Location of word list.
 spelling_word_list_filename = "spelling_wordlist.txt"
+
+# OGP metadata configuration.
+ogp_enable_meta_description = True
+ogp_site_url = "https://django-registration.readthedocs.io/"
+
+# Django settings for sphinxcontrib-django.
+sys.path.insert(0, os.path.abspath("."))
+django_settings = "docs_settings"
```

### Comparing `django-registration-3.3/docs/custom-user.rst` & `django-registration-3.4/docs/custom-user.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,194 +1,184 @@
 .. _custom-user:
 
 Custom user models
 ==================
 
-Django's built-in auth system provides a default model for user
-accounts, but also supports replacing that default with `a custom user
-model
+Django's built-in auth system provides a default model for user accounts, but
+also supports replacing that default with `a custom user model
 <https://docs.djangoproject.com/en/stable/topics/auth/customizing/#substituting-a-custom-user-model>`_. Many
-projects choose to use a custom user model from the start of their
-development, even if it begins as a copy of the default model, in
-order to avoid the difficulty of migrating to a custom user model
-later on.
-
-In general, django-registration will work with a custom user model,
-though at least some additional configuration is always required in
-order to do so. If you are using a custom user model, please read this
-document thoroughly *before* using django-registration, in order to
-ensure you've taken all the necessary steps to ensure support.
-
-The process for using a custom user model with django-registration can
-be summarized as follows:
-
-1. Compare your custom user model to the assumptions made by the
-   built-in registration workflows.
-
-2. If your user model is compatible with those assumptions, write a
-   short subclass of
-   :class:`~django_registration.forms.RegistrationForm` pointed at
+projects choose to use a custom user model from the start of their development,
+even if it begins as a copy of the default model, in order to avoid the
+difficulty of migrating to a custom user model later on.
+
+In general, django-registration will work with a custom user model, though at
+least some additional configuration is always required in order to do so. If
+you are using a custom user model, please read this document thoroughly
+*before* using django-registration, in order to ensure you've taken all the
+necessary steps to ensure support.
+
+The process for using a custom user model with django-registration can be
+summarized as follows:
+
+1. Compare your custom user model to the assumptions made by the built-in
+   registration workflows.
+
+2. If your user model is compatible with those assumptions, write a short
+   subclass of :class:`~django_registration.forms.RegistrationForm` pointed at
    your user model, and instruct django-registration to use that form.
 
-3. If your user model is *not* compatible with those assumptions,
-   either write subclasses of the appropriate views in
-   django-registration which will be compatible with your user model,
-   or modify your user model to be compatible with the built-in views.
+3. If your user model is *not* compatible with those assumptions, either write
+   subclasses of the appropriate views in django-registration which will be
+   compatible with your user model, or modify your user model to be compatible
+   with the built-in views.
 
 These steps are covered in more detail below.
 
 
 Compatibility of the built-in workflows with custom user models
 ---------------------------------------------------------------
 
-Django provides a number of helpers to make it easier for code to
-generically work with custom user models, and django-registration
-makes use of these. However, the built-in registration workflows must
-still make *some* assumptions about the structure of your user model
-in order to work with it. If you intend to use one of
-django-registration's built-in registration workflows, please
-carefully read the appropriate section to see what it expects from
-your user model.
+Django provides a number of helpers to make it easier for code to generically
+work with custom user models, and django-registration makes use of
+these. However, the built-in registration workflows must still make *some*
+assumptions about the structure of your user model in order to work with it. If
+you intend to use one of django-registration's built-in registration workflows,
+please carefully read the appropriate section to see what it expects from your
+user model.
 
 
 The two-step activation workflow
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-:ref:`The two-step activation workflow <activation-workflow>` requires
-that the following be true of your user model:
+:ref:`The two-step activation workflow <activation-workflow>` requires that the
+following be true of your user model:
 
 * Your user model must set the attribute
-  :attr:`~django.contrib.auth.models.CustomUser.USERNAME_FIELD` to
-  indicate the field used as the username.
+  :attr:`~django.contrib.auth.models.CustomUser.USERNAME_FIELD` to indicate the
+  field used as the username.
 
 * Your user model must have a field (of some textual type, ideally
-  :class:`~django.db.models.EmailField`) for storing an email address,
-  and it must define the method
-  :meth:`~django.contrib.auth.models.AbstractBaseUser.get_email_field_name`
-  to indicate the name of the email field.
-
-* The username and email fields must be distinct. If you wish to use
-  the email address as the username, you will need to write your own
-  completely custom registration form.
+  :class:`~django.db.models.EmailField`) for storing an email address, and it
+  must define the method
+  :meth:`~django.contrib.auth.models.AbstractBaseUser.get_email_field_name` to
+  indicate the name of the email field.
+
+* The username and email fields must be distinct. If you wish to use the email
+  address as the username, you will need to write your own completely custom
+  registration form.
 
 * Your user model must have a field named
-  :attr:`~django.contrib.auth.models.User.is_active`, and that field
-  must be a :class:`~django.db.models.BooleanField` indicating whether
-  the user's account is active.
+  :attr:`~django.contrib.auth.models.User.is_active`, and that field must be a
+  :class:`~django.db.models.BooleanField` indicating whether the user's account
+  is active.
 
 If your user model is a subclass of Django's
-:class:`~django.contrib.auth.models.AbstractBaseUser`, all of the
-above will be automatically handled for you.
+:class:`~django.contrib.auth.models.AbstractBaseUser`, all of the above will be
+automatically handled for you.
 
 If your custom user model defines additional fields beyond the minimum
-requirements, you'll either need to ensure that all of those fields
-are optional (i.e., can be `NULL` in your database, or provide a
-suitable default value defined in the model), or specify the correct
-list of fields to display in your
-:class:`~django_registration.forms.RegistrationForm` subclass.
+requirements, you'll either need to ensure that all of those fields are
+optional (i.e., can be ``NULL`` in your database, or provide a suitable default
+value defined in the model), or specify the correct list of fields to display
+in your :class:`~django_registration.forms.RegistrationForm` subclass.
 
 
 The one-step workflow
 ~~~~~~~~~~~~~~~~~~~~~
 
 :ref:`The one-step workflow <one-step-workflow>` places the following
 requirements on your user model:
 
 * Your user model must set the attribute
-  :attr:`~django.contrib.auth.models.CustomUser.USERNAME_FIELD` to
-  indicate the field used as the username.
+  :attr:`~django.contrib.auth.models.CustomUser.USERNAME_FIELD` to indicate the
+  field used as the username.
 
-* It must define a textual field named `password` for storing the
-  user's password.
+* It must define a textual field named ``password`` for storing the user's
+  password.
 
-Also note that the base
-:class:`~django_registration.forms.RegistrationForm` includes and
-requires an email field, so either provide that field on your model
-and set the
+Also note that the base :class:`~django_registration.forms.RegistrationForm`
+includes and requires an email field, so either provide that field on your
+model and set the
 :meth:`~django.contrib.auth.models.AbstractBaseUser.get_email_field_name`
 attribute to indicate which field it is, or subclass
-:class:`~django_registration.forms.RegistrationForm` and override to
-remove the `email` field or make it optional.
+:class:`~django_registration.forms.RegistrationForm` and override to remove the
+`email` field or make it optional.
 
 If your user model is a subclass of Django's
-:class:`~django.contrib.auth.models.AbstractBaseUser`, all of the
-above will be automatically handled for you.
+:class:`~django.contrib.auth.models.AbstractBaseUser`, all of the above will be
+automatically handled for you.
 
 If your custom user model defines additional fields beyond the minimum
-requirements, you'll either need to ensure that all of those fields
-are optional (i.e., can be `NULL` in your database, or provide a
-suitable default value defined in the model), or specify the correct
-list of fields to display in your
-:class:`~django_registration.forms.RegistrationForm` subclass.
-
-Because the one-step workflow logs in the new account immediately
-after creating it, you also must either use Django's
-:class:`~django.contrib.auth.backends.ModelBackend` as an
-`authentication backend
+requirements, you'll either need to ensure that all of those fields are
+optional (i.e., can be ``NULL`` in your database, or provide a suitable default
+value defined in the model), or specify the correct list of fields to display
+in your :class:`~django_registration.forms.RegistrationForm` subclass.
+
+Because the one-step workflow logs in the new account immediately after
+creating it, you also must either use Django's
+:class:`~django.contrib.auth.backends.ModelBackend` as an `authentication
+backend
 <https://docs.djangoproject.com/en/stable/topics/auth/customizing/#other-authentication-sources>`_,
 or use an authentication backend which accepts a combination of
-`USERNAME_FIELD` and `password` as sufficient credentials to
-authenticate a user.
+``USERNAME_FIELD`` and ``password`` as sufficient credentials to authenticate a
+user.
 
 
 Writing your form subclass
 --------------------------
 
-The base :class:`~django_registration.views.RegistrationView` contains
+The base :class:`~djangqo_registration.views.RegistrationView` contains
 code which compares the declared model of your registration form with
 the user model of your Django installation. If these are not the same
 model, the view will deliberately crash by raising an
 :exc:`~django.core.exceptions.ImproperlyConfigured` exception, with an
 error message alerting you to the problem.
 
-This will happen automatically if you attempt to use
-django-registration with a custom user model and also attempt to use
-the default, unmodified
-:class:`~django-registration.forms.RegistrationForm`. This is, again,
-a deliberate design feature of django-registration, and not a bug:
-django-registration has no way of knowing in advance if your user
-model is compatible with the assumptions made by the built-in
-registration workflows (see above), so it requires you to take the
-explicit step of replacing the default registration form as a way of
-confirming you've manually checked the compatibility of your user
-model.
-
-In the case where your user model is compatible with the default
-behavior of django-registration, you will be able to subclass
-:class:`~django_registration.forms.RegistrationForm`, set it to use
-your custom user model as the model, and then configure the views in
-django-registration to use your form subclass. For example, you might
-do the following (in a `forms.py` module somewhere in your codebase --
-do **not** directly edit django-registration's code):
+This will happen automatically if you attempt to use django-registration with a
+custom user model and also attempt to use the default, unmodified
+:class:`~django-registration.forms.RegistrationForm`. This is, again, a
+deliberate design feature of django-registration, and not a bug:
+django-registration has no way of knowing in advance if your user model is
+compatible with the assumptions made by the built-in registration workflows
+(see above), so it requires you to take the explicit step of replacing the
+default registration form as a way of confirming you've manually checked the
+compatibility of your user model.
+
+In the case where your user model is compatible with the default behavior of
+django-registration, you will be able to subclass
+:class:`~django_registration.forms.RegistrationForm`, set it to use your custom
+user model as the model, and then configure the views in django-registration to
+use your form subclass. For example, you might do the following (in a
+``forms.py`` module somewhere in your codebase -- do **not** directly edit
+django-registration's code):
 
 .. code-block:: python
 
     from django_registration.forms import RegistrationForm
 
     from mycustomuserapp.models import MyCustomUser
 
-    
+
     class MyCustomUserForm(RegistrationForm):
         class Meta(RegistrationForm.Meta):
             model = MyCustomUser
 
-You may also need to specify the fields to include in the form, if the
-set of fields to include is different from the default set specified
-by the base :class:`~django_registration.forms.RegistrationForm`.
-
-Then in your URL configuration (example here uses the two-step
-activation workflow), configure the registration view to use the form
-class you wrote:
+You may also need to specify the fields to include in the form, if the set of
+fields to include is different from the default set specified by the base
+:class:`~django_registration.forms.RegistrationForm`.
+
+Then in your URL configuration (example here uses the two-step activation
+workflow), configure the registration view to use the form class you wrote:
 
 .. code-block:: python
 
     from django.urls import include, path
 
     from django_registration.backends.activation.views import RegistrationView
-    
+
     from mycustomuserapp.forms import MyCustomUserForm
 
 
     urlpatterns = [
         # ... other URL patterns here
         path('accounts/register/',
             RegistrationView.as_view(
@@ -202,35 +192,32 @@
 	# ... more URL patterns
     ]
 
 
 Incompatible user models
 ------------------------
 
-If your custom user model is not compatible with the built-in
-workflows of django-registration, you have several options.
+If your custom user model is not compatible with the built-in workflows of
+django-registration, you have several options.
 
-One is to subclass the built-in form and view classes of
-django-registration and make the necessary adjustments to achieve
-compatibility with your user model. For example, if you want to use
-the two-step activation workflow, but your user model uses a
-completely different way of marking accounts active/inactive (compared
-to the the assumed `is_active` field), you might write subclasses of
-that workflow's
-:class:`~django_registration.backends.activation.views.RegistrationView`
-and
-:class:`~django_registration.backends.activation.views.ActivationView`
-which make use of your user model's mechanism for marking accounts
-active/inactive, and then use those views along with an appropriate
-subclass of :class:`~django_registration.forms.RegistrationForm`.
-
-Or, if the incompatibilities are relatively minor and you don't mind
-making the change, you might use Django's migration framework to
-adjust your custom user model to match the assumptions made by
-django-registration's built-in workflows, thus allowing them to be
-used unmodified.
-
-Finally, it may sometimes be the case that a given user model requires
-a completely custom set of form and view classes to
-support. Typically, this will also involve an account-registration
-process far enough from what django-registration's built-in workflows
-provide that you would be writing your own workflow in any case.
+One is to subclass the built-in form and view classes of django-registration
+and make the necessary adjustments to achieve compatibility with your user
+model. For example, if you want to use the two-step activation workflow, but
+your user model uses a completely different way of marking accounts
+active/inactive (compared to the the assumed ``is_active`` field), you might
+write subclasses of that workflow's
+:class:`~django_registration.backends.activation.views.RegistrationView` and
+:class:`~django_registration.backends.activation.views.ActivationView` which
+make use of your user model's mechanism for marking accounts active/inactive,
+and then use those views along with an appropriate subclass of
+:class:`~django_registration.forms.RegistrationForm`.
+
+Or, if the incompatibilities are relatively minor and you don't mind making the
+change, you might use Django's migration framework to adjust your custom user
+model to match the assumptions made by django-registration's built-in
+workflows, thus allowing them to be used unmodified.
+
+Finally, it may sometimes be the case that a given user model requires a
+completely custom set of form and view classes to support. Typically, this will
+also involve an account-registration process far enough from what
+django-registration's built-in workflows provide that you would be writing your
+own workflow in any case.
```

### Comparing `django-registration-3.3/docs/exceptions.rst` & `django-registration-3.4/docs/exceptions.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 .. _exceptions:
 .. module:: django_registration.exceptions
 
 
 Exception classes
 =================
 
-django-registration provides two base exception classes to signal
-errors which occur during the signup or activation processes.
+django-registration provides two base exception classes to signal errors which
+occur during the signup or activation processes.
 
 .. exception:: RegistrationError(message, code, params)
 
-   Base exception class for all exceptions raised in
-   django-registration. No code in django-registration will raise this
-   exception directly; it serves solely to provide a distinguishing
-   parent class for other errors. Arguments passed when the exception
-   is raised will be stored and exposed as attributes of the same
-   names on the exception object:
+   Base exception class for all exceptions raised in django-registration. No
+   code in django-registration will raise this exception directly; it serves
+   solely to provide a distinguishing parent class for other errors. Arguments
+   passed when the exception is raised will be stored and exposed as attributes
+   of the same names on the exception object:
 
    :param str message: A human-readable error message.
    :param str code: A short but unique identifier used by subclasses
          to distinguish different error conditions.
    :param dict params: Arbitrary key-value data to associate with the error.
 
 
 .. exception:: ActivationError(message, code, params)
 
-   Exception class to indicate errors during account
-   activation. Subclass of :exc:`RegistrationError` and inherits its
-   attributes.
+   Exception class to indicate errors during account activation. Subclass of
+   :exc:`RegistrationError` and inherits its attributes.
```

### Comparing `django-registration-3.3/docs/faq.rst` & `django-registration-3.4/docs/faq.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,255 +1,261 @@
 .. _faq:
 
 Frequently-asked questions
 ==========================
 
-The following are miscellaneous common questions and answers related
-to installing/using django-registration, culled from bug reports,
-emails and other sources.
+The following are miscellaneous common questions and answers related to
+installing/using django-registration, culled from bug reports, emails and other
+sources.
 
 
 General
 -------
 
 This doesn't work with custom user models! It crashes as soon as I try to use one!
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-django-registration can work perfectly well with a custom user model,
-but this does require you to do a bit more work. Please thoroughly
-read :ref:`the documentation for how to use custom user models
-<custom-user>` before filing a bug.
+django-registration can work perfectly well with a custom user model, but this
+does require you to do a bit more work. Please thoroughly read :ref:`the
+documentation for how to use custom user models <custom-user>` before filing a
+bug.
 
 Please also note that, as explained in that documentation, by default
-django-registration will crash if you try to use a custom user model
-without following the documentation. This is not a bug; it is done
-deliberately to ensure you read and follow the documentation.
+django-registration will crash if you try to use a custom user model without
+following the documentation. This is not a bug; it is done deliberately to
+ensure you read and follow the documentation.
 
 How can I support social-media and other auth schemes, like Facebook or GitHub?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-By using `django-allauth
-<https://pypi.python.org/pypi/django-allauth>`_. No single application
-can or should provide a universal API for every authentication system
-ever developed; django-registration sticks to making it easy to
-implement typical signup workflows using Django's default model-based
-authentication system, while apps like `django-allauth` handle
-integration with third-party authentication services far more
-effectively.
+By using `django-allauth <https://pypi.python.org/pypi/django-allauth>`_. No
+single application can or should provide a universal API for every
+authentication system ever developed; django-registration sticks to making it
+easy to implement typical signup workflows using Django's default model-based
+authentication system, while apps like ``django-allauth`` handle integration with
+third-party authentication services far more effectively.
 
 What license is django-registration under?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-django-registration is offered under a three-clause BSD-style license;
-this is `an OSI-approved open-source license
-<http://www.opensource.org/licenses/bsd-license.php>`_, and allows you
-a large degree of freedom in modifying and redistributing the
-code. For the full terms, see the file `LICENSE` which came with
-your copy of django-registration; if you did not receive a copy of
-this file, you can view it online at
+django-registration is offered under a three-clause BSD-style license; this is
+`an OSI-approved open-source license
+<http://www.opensource.org/licenses/bsd-license.php>`_, and allows you a large
+degree of freedom in modifying and redistributing the code. For the full terms,
+see the file ``LICENSE`` which came with your copy of django-registration; if you
+did not receive a copy of this file, you can view it online at
 <https://github.com/ubernostrum/django-registration/blob/master/LICENSE>.
 
 What versions of Django and Python are supported?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-As of django-registration |release|, Django 3.2 and 4.0 are
-supported, on Python 3.7 (Django 3.2 only), 3.8, 3.9, and 3.10. Note
-that Django 3.2's support for Python 3.10 was added in Django 3.2.9,
-so you may experience issues with Python 3.10 and earlier Django 3.2
-versions.
+As of django-registration |release|, Django 3.2 and 4.0 are supported, on
+Python 3.7 (Django 3.2 only), 3.8, 3.9, and 3.10. Note that Django 3.2's
+support for Python 3.10 was added in Django 3.2.9, so you may experience issues
+with Python 3.10 and earlier Django 3.2 versions.
 
 
 I found a bug or want to make an improvement!
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. important:: **Reporting security issues**
 
-   If you believe you have found a security issue in
-   django-registration, please do *not* use the public GitHub issue
-   tracker to report it. Instead, you can `contact the author
-   privately <https://www.b-list.org/contact/>`_ to report the issue.
-
-The canonical development repository for django-registration is online
-at <https://github.com/ubernostrum/django-registration>. Issues and
-pull requests can both be filed there.
-
-If you'd like to contribute to django-registration, that's great! Just
-please remember that pull requests should include tests and
-documentation for any changes made, and that following `PEP 8
-<https://www.python.org/dev/peps/pep-0008/>`_ is mandatory. Pull
-requests without documentation won't be merged, and PEP 8 style
-violations or test coverage below 100% are both configured to break
-the build.
+   If you believe you have found a security issue in django-registration,
+   please do *not* use the public GitHub issue tracker to report it. Instead,
+   you can `contact the author privately <https://www.b-list.org/contact/>`_ to
+   report the issue.
+
+The canonical development repository for django-registration is online at
+<https://github.com/ubernostrum/django-registration>. Issues and pull requests
+can both be filed there.
+
+If you'd like to contribute to django-registration, that's great! Just please
+remember that pull requests should include tests and documentation for any
+changes made, and that following `PEP 8
+<https://www.python.org/dev/peps/pep-0008/>`_ is mandatory. Pull requests
+without documentation won't be merged, and PEP 8 style violations or test
+coverage below 100% are both configured to break the build.
 
 How secure is django-registration?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Over the course of django-registration's history so far, there has
-been one security issue reported which required a new release to
-remedy. This doesn't mean, though, that django-registration is
-perfectly secure: much will depend on ensuring best practices in
-deployment and server configuration, and there could always be
-security issues that just haven't been recognized yet.
-
-django-registration does, however, try to avoid common security
-issues:
-
-* django-registration |release| only supports versions of Django which
-  were receiving upstream security support at the time of release.
-
-* django-registration does not attempt to generate or store passwords,
-  and does not transmit credentials which could be used to log in (the
-  only "credential" ever sent out by django-registration is an
-  activation key used in the two-step activation workflow, and that
-  key can only be used to make an account active; it cannot be used to
-  log in).
-
-* django-registration works with Django's own security features
-  (including cryptographic features) where possible, rather than
-  reinventing its own.
+Over the course of django-registration's history so far, there has been one
+security issue reported which required a new release to remedy. This doesn't
+mean, though, that django-registration is perfectly secure: much will depend on
+ensuring best practices in deployment and server configuration, and there could
+always be security issues that just haven't been recognized yet.
+
+django-registration does, however, try to avoid common security issues:
+
+* django-registration |release| only supports versions of Django which were
+  receiving upstream security support at the time of release.
+
+* django-registration does not attempt to generate or store passwords, and does
+  not transmit credentials which could be used to log in (the only "credential"
+  ever sent out by django-registration is an activation key used in the
+  two-step activation workflow, and that key can only be used to make an
+  account active; it cannot be used to log in).
+
+* django-registration works with Django's own security features (including
+  cryptographic features) where possible, rather than reinventing its own.
 
 For more details, see :ref:`the security guide <security>`.
 
 How do I run the tests?
 ~~~~~~~~~~~~~~~~~~~~~~~
 
-django-registration's tests are run using `tox
-<https://tox.readthedocs.io/>`_, but typical installation of
-django-registration (via `pip install django-registration`) will not
-install the tests.
-
-To run the tests, download the source (`.tar.gz`) distribution of
-django-registration |release| from `its page on the Python Package
-Index <https://pypi.org/project/django-registration/>`_, unpack it
-(`tar zxvf django-registration-|release|.tar.gz` on most Unix-like
-operating systems), and in the unpacked directory run `tox`.
-
-Note that you will need to have `tox` installed already (`pip
-install tox`), and to run the full test matrix you will need to have
-each supported version of Python available. To run only the tests for
-a specific Python version and Django version, you can invoke `tox`
-with the `-e` flag. For example, to run tests for Python 3.6 and
-Django 2.0: `tox -e py36-django20`.
+django-registration's tests are run using `nox <https://nox.thea.codes/>`_, but
+typical installation of django-registration (via ``pip install
+django-registration``) will not install the tests.
+
+To run the tests, download the source (``.tar.gz``) distribution of
+django-registration |release| from `its page on the Python Package Index
+<https://pypi.org/project/django-registration/>`_, unpack it (``tar zxvf
+django-registration-|version|.tar.gz`` on most Unix-like operating systems),
+and in the unpacked directory run the following at a command prompt:
+
+.. tab:: macOS/Linux/other Unix
+
+   .. code-block:: shell
+
+      python -m pip install nox
+      python -m nox
+
+.. tab:: Windows
+
+   .. code-block:: shell
+
+      py -m pip install nox
+      py -m nox
+
+Note that to run the full test matrix you will need to have each supported
+version of Python available. To run only specific test tasks, you can invoke
+``nox`` with the ``-s`` flag to select a single test task, ``-t`` to run all
+tasks matching a particular tag (like ``docs``), or ``--python`` passing a
+Python version to run only tasks for that version. For example, to run tests
+for Python 3.10 only, you could run:
+
+.. tab:: macOS/Linux/other Unix
+
+   .. code-block:: shell
+
+      python -m nox --python "3.10"
+
+.. tab:: Windows
+
+   .. code-block:: shell
+
+      py -m nox --python "3.10"
+
+By default, ``nox`` will only run the tasks whose associated Python versions
+are available on your system. For example, if you have only Python 3.8 and 3.9
+installed, test runs for Python 3.7, 3.10, and 3.11 would be skipped.
+
 
-   
 Installation and setup
 ----------------------
 
 How do I install django-registration?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Full instructions are available in :ref:`the installation guide
-<install>`. For configuration, see :ref:`the quick start guide
-<quickstart>`.
+Full instructions are available in :ref:`the installation guide <install>`. For
+configuration, see :ref:`the quick start guide <quickstart>`.
 
 Does django-registration come with any sample templates I can use right away?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 No, for two reasons:
 
-1. Providing default templates with an application is ranges from hard
-   to impossible, because different sites can have such wildly
-   different design and template structure. Any attempt to provide
-   templates which would work with all the possibilities would
-   probably end up working with none of them.
+1. Providing default templates with an application is ranges from hard to
+   impossible, because different sites can have such wildly different design
+   and template structure. Any attempt to provide templates which would work
+   with all the possibilities would probably end up working with none of them.
 
 2. A number of things in django-registration depend on the specific
-   registration workflow you use, including the variables which end up
-   in template contexts. Since django-registration has no way of
-   knowing in advance what workflow you're going to be using, it also
-   has no way of knowing what your templates will need to look like.
-
-Fortunately, however, django-registration has good documentation which
-explains what context variables will be available to templates, and so
-it should be easy for anyone who knows Django's template system to
-create templates which integrate with their own site.
+   registration workflow you use, including the variables which end up in
+   template contexts. Since django-registration has no way of knowing in
+   advance what workflow you're going to be using, it also has no way of
+   knowing what your templates will need to look like.
+
+Fortunately, however, django-registration has good documentation which explains
+what context variables will be available to templates, and so it should be easy
+for anyone who knows Django's template system to create templates which
+integrate with their own site.
 
 
 Configuration
 -------------
 
 Do I need to rewrite the views to change the way they behave?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Not always. Any behavior controlled by an attribute on a class-based
-view can be changed by passing a different value for that attribute in
-the URLconf. See `Django's class-based view documentation
+Not always. Any behavior controlled by an attribute on a class-based view can
+be changed by passing a different value for that attribute in the URLconf. See
+`Django's class-based view documentation
 <https://docs.djangoproject.com/en/stable/topics/class-based-views/#simple-usage-in-your-urlconf>`_
 for examples of this.
 
-For more complex or fine-grained control, you will likely want to
-subclass :class:`~django_registration.views.RegistrationView` or
-:class:`~django_registration.views.ActivationView`, or both, add your
-custom logic to your subclasses, and then create a URLconf which makes
-use of your subclasses.
-    
+For more complex or fine-grained control, you will likely want to subclass
+:class:`~django_registration.views.RegistrationView` or
+:class:`~django_registration.views.ActivationView`, or both, add your custom
+logic to your subclasses, and then create a URLconf which makes use of your
+subclasses.
+
 I don't want to write my own URLconf because I don't want to write patterns for all the auth views!
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 You're in luck, then; Django provides a URLconf for this, at
-`django.contrib.auth.urls`.
+``django.contrib.auth.urls``.
 
 I don't like the names you've given to the URL patterns!
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-In that case, you should feel free to set up your own URLconf which
-uses the names you want.
+In that case, you should feel free to set up your own URLconf which uses the
+names you want.
 
 I'm using a custom user model; how do I make that work?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 See :ref:`the custom user documentation <custom-user>`.
 
 
 Tips and tricks
 ---------------
 
 How do I close user signups?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 If you haven't modified the behavior of the
-:meth:`~django_registration.views.RegistrationView.registration_allowed`
-method in :class:`~django_registration.views.RegistrationView`, you can
-use the setting :data:`~django.conf.settings.REGISTRATION_OPEN` to
-control this; when the setting is `True`, or isn't supplied,
-user registration will be permitted. When the setting is
-`False`, user registration will not be permitted.
+:meth:`~django_registration.views.RegistrationView.registration_allowed` method
+in :class:`~django_registration.views.RegistrationView`, you can use the
+setting :data:`~django.conf.settings.REGISTRATION_OPEN` to control this; when
+the setting is :data:`True`, or isn't supplied, user registration will be
+permitted. When the setting is :data:`False`, user registration will not be
+permitted.
 
 How do I log a user in immediately after registration or activation?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Take a look at the implementation of :ref:`the one-step workflow
-<one-step-workflow>`, which logs a user in immediately after
-registration.
+<one-step-workflow>`, which logs a user in immediately after registration.
 
 How do I manually activate a user?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-In :ref:`the two-step activation workflow <activation-workflow>`,
-toggle the `is_active` field of the user in the admin.
+In :ref:`the two-step activation workflow <activation-workflow>`, toggle the
+``is_active`` field of the user in the admin.
 
 How do I delete expired unactivated accounts?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Perform a query for those accounts, and call the `delete()` method
-of the resulting `QuerySet`. Since django-registration doesn't know
-in advance what your definition of "expired" will be, it leaves this
-step to you.
-
-How do I allow Unicode in usernames?
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Use Python 3. Django's username validation allows any word character
-plus some additional characters, but the definition of "word
-character" depends on the Python version in use. On Python 2, only
-ASCII will be permitted; on Python 3, usernames containing word
-characters matched by a regex with the :data:`re.UNICODE` flag will be
-accepted.
+Perform a query for those accounts, and call the ``delete()`` method of the
+resulting ``QuerySet``. Since django-registration doesn't know in advance what
+your definition of "expired" will be, it leaves this step to you.
 
 How do I tell why an account's activation failed?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-If you're using :ref:`the two-step activation workflow
-<activation-workflow>`, the template context will contain a variable
-`activation_error` containing the information passed when the
-:exc:`~django_registration.exceptions.ActivationError` was
-raised. This will indicate what caused the failure.
+If you're using :ref:`the two-step activation workflow <activation-workflow>`,
+the template context will contain a variable `activation_error` containing the
+information passed when the
+:exc:`~django_registration.exceptions.ActivationError` was raised. This will
+indicate what caused the failure.
```

### Comparing `django-registration-3.3/docs/forms.rst` & `django-registration-3.4/docs/forms.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,108 @@
 .. _forms:
 .. module:: django_registration.forms
 
 Base form classes
 =================
 
-Several form classes are provided with django-registration,
-covering common cases for gathering account information and
-implementing common constraints for user registration. These forms
-were designed with django-registration's built-in registration
-workflows in mind, but may also be useful in other situations.
+Several form classes are provided with django-registration, covering common
+cases for gathering account information and implementing common constraints for
+user registration. These forms were designed with django-registration's
+built-in registration workflows in mind, but may also be useful in other
+situations.
 
 
 .. class:: RegistrationForm
 
-   A form for registering an account. This is a subclass of Django's
-   built-in :class:`~django.contrib.auth.forms.UserCreationForm`, and
-   has the following fields, all of which are required:
+   A form for registering an account. This is a subclass of Django's built-in
+   :class:`~django.contrib.auth.forms.UserCreationForm`, and has the following
+   fields, all of which are required:
 
-   `username`
+   ``username``
        The username to use for the new account.
 
-   `email`
+   ``email``
       The email address to use for the new account.
 
-   `password1`
+   ``password1``
       The password to use for the new account.
 
-   `password2`
-      The password to use for the new account, repeated to catch
-      typos.
+   ``password2``
+      The password to use for the new account, repeated to catch typos.
 
    .. note:: **Validation of usernames**
 
-      Django supplies a default regex-based validator for usernames in
-      its base :class:`~django.contrib.auth.models.AbstractBaseUser`
-      implementation, allowing any word character along with the
-      following set of additional characters: `.`, `@`, `+`, and
-      `-`.
+      Django supplies a default regex-based validator for usernames in its base
+      :class:`~django.contrib.auth.models.AbstractBaseUser` implementation,
+      allowing any word character along with the following set of additional
+      characters: ``.``, ``@``, ``+``, and ``-``.
 
       Because it's a subclass of Django's
       :class:`~django.contrib.auth.forms.UserCreationForm`,
-      :class:`RegistrationForm` will inherit the base validation
-      defined by Django. It also applies some custom validators to the
-      username:
-      :class:`~django_registration.validators.ReservedNameValidator`,
-      and
+      :class:`RegistrationForm` will inherit the base validation defined by
+      Django. It also applies some custom validators to the username:
+      :class:`~django_registration.validators.ReservedNameValidator`, and
       :func:`~django_registration.validators.validate_confusables`.
 
    .. note:: **Validation of email addresses**
 
       django-registration applies two additional validators --
       :class:`~django_registration.validators.HTML5EmailValidator` and
-      :func:`~django_registration.validators.validate_confusables_email`
-      -- to the email address.
+      :func:`~django_registration.validators.validate_confusables_email` -- to
+      the email address.
 
       The HTML5 validator uses `the HTML5 email-validation rule
       <https://html.spec.whatwg.org/multipage/input.html#e-mail-state-(type=email)>`_
-      (as implemented on HTML's `input type="email"`), which is more
-      restrictive than the email RFCs. The purpose of this validator
-      is twofold: to match the behavior of HTML5, and to simplify
-      django-registration's other validators. The full RFC grammar for
-      email addresses is enormously complex despite most of its
-      features rarely if ever being used legitimately, so disallowing
-      those features allows other validators to interact with a much
-      simpler format, ensuring performance, reliability and safety.
+      (as implemented on HTML's ``input type="email"``), which is more
+      restrictive than the email RFCs. The purpose of this validator is
+      twofold: to match the behavior of HTML5, and to simplify
+      django-registration's other validators. The full RFC grammar for email
+      addresses is enormously complex despite most of its features rarely if
+      ever being used legitimately, so disallowing those features allows other
+      validators to interact with a much simpler format, ensuring performance,
+      reliability and safety.
 
    .. note:: **Custom user models**
 
       If you are using `a custom user model
       <https://docs.djangoproject.com/en/stable/topics/auth/customizing/#substituting-a-custom-user-model>`_,
-      you **must** subclass this form and tell it to use your custom
-      user model instead of Django's default user model. If you do
-      not, django-registration will deliberately crash with an error
-      message reminding you to do this. See :ref:`the custom user
-      compatibility guide <custom-user>` for details.
+      you **must** subclass this form and tell it to use your custom user model
+      instead of Django's default user model. If you do not,
+      django-registration will deliberately crash with an error message
+      reminding you to do this. See :ref:`the custom user compatibility guide
+      <custom-user>` for details.
 
 .. class:: RegistrationFormCaseInsensitive
 
-   A subclass of :class:`RegistrationForm` which enforces
-   case-insensitive uniqueness of usernames, by applying
-   :class:`~django_registration.validators.CaseInsensitiveUnique`
-   to the username field.
+   A subclass of :class:`RegistrationForm` which enforces case-insensitive
+   uniqueness of usernames, by applying
+   :class:`~django_registration.validators.CaseInsensitiveUnique` to the
+   username field.
 
    .. note:: **Unicode case handling**
 
-     This form will normalize the username value to form NFKC,
-     matching Django's default approach to Unicode normalization. it
-     will then case fold the value, and use a case-insensitive
-     (`iexact`) lookup to determine if a user with the same username
-     already exists; the results of this query may depend on the
-     quality of your database's Unicode implementation, and on
-     configuration details. The results may also be surprising to
-     developers who are primarily used to English/ASCII text, as
-     Unicode's case rules can be quite complex.
+     This form will normalize the username value to form NFKC, matching
+     Django's default approach to Unicode normalization. it will then case fold
+     the value, and use a case-insensitive (``iexact``) lookup to determine if a
+     user with the same username already exists; the results of this query may
+     depend on the quality of your database's Unicode implementation, and on
+     configuration details. The results may also be surprising to developers
+     who are primarily used to English/ASCII text, as Unicode's case rules can
+     be quite complex.
 
 
 .. class:: RegistrationFormTermsOfService
 
-   A subclass of :class:`RegistrationForm` which adds one additional,
-   required field:
+   A subclass of :class:`RegistrationForm` which adds one additional, required
+   field:
 
-   `tos`
-       A checkbox indicating agreement to the site's terms of
-       service/user agreement.
+   ``tos``
+       A checkbox indicating agreement to the site's terms of service/user
+       agreement.
 
 
 .. class:: RegistrationFormUniqueEmail
 
-   A subclass of :class:`RegistrationForm` which enforces uniqueness
-   of email addresses in addition to uniqueness of usernames, by
-   applying
-   :class:`~django_registration.validators.CaseInsensitiveUnique` to
-   the email field.
+   A subclass of :class:`RegistrationForm` which enforces uniqueness of email
+   addresses in addition to uniqueness of usernames, by applying
+   :class:`~django_registration.validators.CaseInsensitiveUnique` to the email
+   field.
```

### Comparing `django-registration-3.3/docs/index.rst` & `django-registration-3.4/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 .. _index:
 
 django-registration |release|
 =============================
 
-django-registration is an extensible application providing user
-registration functionality for `Django
-<https://www.djangoproject.com/>`_-powered Web sites.
-
-Although nearly all aspects of the registration process are
-customizable, out-of-the-box support is provided for two common use
-cases:
+django-registration is an extensible application providing user registration
+functionality for `Django <https://www.djangoproject.com/>`_-powered Web sites.
+
+Although nearly all aspects of the registration process are customizable,
+out-of-the-box support is provided for two common use cases:
 
 * Two-phase registration, consisting of initial signup followed by a
   confirmation email with instructions for activating the new account.
 
-* One-phase registration, where a user signs up and is immediately
-  active and logged in.
+* One-phase registration, where a user signs up and is immediately active and
+  logged in.
 
-To get up and running quickly, :ref:`install django-registration
-<install>`, then read :ref:`the quick start guide <quickstart>`, which
-describes the steps necessary to configure django-registration for the
-built-in workflows. For more detailed information, including how to
-customize the registration process (and support for alternate
-registration systems), read through the documentation listed below.
+To get up and running quickly, :ref:`install django-registration <install>`,
+then read :ref:`the quick start guide <quickstart>`, which describes the steps
+necessary to configure django-registration for the built-in workflows. For more
+detailed information, including how to customize the registration process (and
+support for alternate registration systems), read through the documentation
+listed below.
 
 
 .. toctree::
    :caption: Installation and configuration
    :maxdepth: 1
 
    install
```

### Comparing `django-registration-3.3/docs/make.bat` & `django-registration-3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/docs/one-step-workflow.rst` & `django-registration-3.4/docs/one-step-workflow.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,86 @@
 .. _one-step-workflow:
 .. module:: django_registration.backends.one_step
 
 The one-step workflow
 =====================
 
-As an alternative to :ref:`the two-step (registration and activation)
-workflow <activation-workflow>`, django-registration bundles a
-one-step registration workflow in
-`django_registration.backends.one_step`. This workflow consists of
+As an alternative to :ref:`the two-step (registration and activation) workflow
+<activation-workflow>`, django-registration bundles a one-step registration
+workflow in ``django_registration.backends.one_step``. This workflow consists of
 as few steps as possible:
 
 1. A user signs up by filling out a registration form.
 
 2. The user's account is created and is active immediately, with no
    intermediate confirmation or activation step.
 
 3. The new user is logged in immediately.
 
 
 Configuration
 -------------
 
 To use this workflow, include the URLconf
-`django_registration.backends.one_step.urls` somewhere in your site's
-own URL configuration. For example:
+``django_registration.backends.one_step.urls`` somewhere in your site's own URL
+configuration. For example:
 
 .. code-block:: python
 
    from django.urls import include, path
 
    urlpatterns = [
        # Other URL patterns ...
        path('accounts/', include('django_registration.backends.one_step.urls')),
        path('accounts/', include('django.contrib.auth.urls')),
        # More URL patterns ...
    ]
 
-To control whether registration of new accounts is allowed, you can
-specify the setting :data:`~django.conf.settings.REGISTRATION_OPEN`.
+To control whether registration of new accounts is allowed, you can specify the
+setting :data:`~django.conf.settings.REGISTRATION_OPEN`.
 
-Upon successful registration, the user will be redirected to the
-site's home page -- the URL `/`. This can be changed by subclassing
-:class:`django_registration.backends.one_step.views.RegistrationView`
-and overriding the method
-:meth:`~django_registration.views.RegistrationView.get_success_url`
-or setting the attribute
-:attr:`~django_registration.views.RegistrationView.success_url`. You
-can also do this in a URLconf. For example:
+Upon successful registration, the user will be redirected to the site's home
+page -- the URL ``/``. This can be changed by subclassing
+:class:`django_registration.backends.one_step.views.RegistrationView` and
+overriding the method
+:meth:`~django_registration.views.RegistrationView.get_success_url` or setting
+the attribute
+:attr:`~django_registration.views.RegistrationView.success_url`. You can also
+do this in a URLconf. For example:
 
 .. code-block:: python
 
-   from django.conf.urls import include, url
+   from django.urls import include, path
 
    from django_registration.backends.one_step.views import RegistrationView
 
    urlpatterns = [
        # Other URL patterns ...
        path('accounts/register/',
            RegistrationView.as_view(success_url='/profile/'),
 	   name='django_registration_register'),
        path('accounts/', include('django_registration.backends.one_step.urls')),
        path('accounts/', include('django.contrib.auth.urls')),
        # More URL patterns ...
    ]
 
 The default form class used for account registration will be
-:class:`django_registration.forms.RegistrationForm`, although this can
-be overridden by supplying a custom URL pattern for the registration
-view and passing the keyword argument `form_class`, or by subclassing
-:class:`django_registration.backends.one_step.views.RegistrationView`
-and either overriding
-:attr:`~django_registration.views.RegistrationView.form_class` or
-implementing
-:meth:`~django_registration.views.RegistrationView.get_form_class()`,
-and specifying the custom subclass in your URL patterns.
+:class:`django_registration.forms.RegistrationForm`, although this can be
+overridden by supplying a custom URL pattern for the registration view and
+passing the keyword argument ``form_class``, or by subclassing
+:class:`django_registration.backends.one_step.views.RegistrationView` and
+either overriding
+:attr:`~django_registration.views.RegistrationView.form_class` or implementing
+:meth:`~django_registration.views.RegistrationView.get_form_class()`, and
+specifying the custom subclass in your URL patterns.
 
 
 Templates
 ---------
 
 The one-step workflow uses two templates:
 
-* `django_registration/registration_form.html`.
-* `django_registration/registration_closed.html`
+* ``django_registration/registration_form.html``.
+* ``django_registration/registration_closed.html``
 
-See :ref:`the quick start guide <default-form-template>` for details
-of these templates.
+See :ref:`the quick start guide <default-form-template>` for details of these
+templates.
```

### Comparing `django-registration-3.3/docs/quickstart.rst` & `django-registration-3.4/docs/quickstart.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,335 +1,318 @@
 .. _quickstart:
 
 Quick start guide
 =================
 
-First you'll need to have Django and django-registration
-installed; for details on that, see :ref:`the installation guide
-<install>`.
+First you'll need to have Django and django-registration installed; for details
+on that, see :ref:`the installation guide <install>`.
 
-The next steps will depend on which registration workflow you'd like
-to use. There are two workflows built into django-registration:
+The next steps will depend on which registration workflow you'd like to
+use. There are two workflows built into django-registration:
 
 * :ref:`The two-step activation workflow <activation-workflow>`, which
-  implements a two-step process: a user signs up, then is emailed an
-  activation link and must click it to activate the account.
+  implements a two-step process: a user signs up, then is emailed an activation
+  link and must click it to activate the account.
 
-* :ref:`The one-step workflow <one-step-workflow>`, in which a user
-  signs up and their account is immediately active and logged in.
+* :ref:`The one-step workflow <one-step-workflow>`, in which a user signs up
+  and their account is immediately active and logged in.
 
-If you want a signup process other than what's provided by these
-built-in workflows, please see the documentation for the base
-:ref:`view <views>` and :ref:`form <forms>` classes, which you can
-subclass to implement your own preferred user registration flow and
-rules. The guide below covers use of the built-in workflows.
-
-Regardless of which registration workflow you choose to use, you
-should add `"django_registration"` to your
-:data:`~django.conf.settings.INSTALLED_APPS` setting.
+If you want a signup process other than what's provided by these built-in
+workflows, please see the documentation for the base :ref:`view <views>` and
+:ref:`form <forms>` classes, which you can subclass to implement your own
+preferred user registration flow and rules. The guide below covers use of the
+built-in workflows.
+
+Regardless of which registration workflow you choose to use, you should add
+`"django_registration"` to your :data:`~django.conf.settings.INSTALLED_APPS`
+setting.
 
 .. important:: **Django's authentication system must be installed**
 
-   Before proceeding with either of the recommended built-in
-   workflows, you'll need to ensure `django.contrib.auth` has been
-   installed (by adding it to
-   :data:`~django.conf.settings.INSTALLED_APPS` and running `manage.py
-   migrate` to install needed database tables). Also, if you're making
-   use of `a custom user model
+   Before proceeding with either of the recommended built-in workflows, you'll
+   need to ensure ``django.contrib.auth`` has been installed (by adding it to
+   :data:`~django.conf.settings.INSTALLED_APPS` and running ``manage.py
+   migrate`` to install needed database tables). Also, if you're making use of
+   `a custom user model
    <https://docs.djangoproject.com/en/stable/topics/auth/customizing/#substituting-a-custom-user-model>`_,
-   you'll probably want to pause and read :ref:`the custom user
-   compatibility guide <custom-user>` before using
-   django-registration.
+   you'll probably want to pause and read :ref:`the custom user compatibility
+   guide <custom-user>` before using django-registration.
 
 .. note:: **Additional steps for account security**
 
-   While django-registration does what it can to secure the user
-   signup process, its scope is deliberately limited; please read
-   :ref:`the security documentation <security>` for recommendations on
-   steps to secure user accounts beyond what django-registration alone
-   can do.
+   While django-registration does what it can to secure the user signup
+   process, its scope is deliberately limited; please read :ref:`the security
+   documentation <security>` for recommendations on steps to secure user
+   accounts beyond what django-registration alone can do.
 
 
 Configuring the two-step activation workflow
 --------------------------------------------
 
-The configuration process for using the two-step activation workflow
-is straightforward: you'll need to specify a couple of settings,
-connect some URLs and create a few templates.
+The configuration process for using the two-step activation workflow is
+straightforward: you'll need to specify a couple of settings, connect some URLs
+and create a few templates.
 
 
 Required settings
 ~~~~~~~~~~~~~~~~~
 
 Begin by adding the following setting to your Django settings file:
 
-:data:`~django.conf.settings.ACCOUNT_ACTIVATION_DAYS`
-    This is the number of days users will have to activate their
-    accounts after registering. If a user does not activate within
-    that period, the account will remain permanently inactive unless a
-    site administrator manually activates it.
+:data:`~django.conf.settings.ACCOUNT_ACTIVATION_DAYS` This is the number of
+    days users will have to activate their accounts after registering. If a
+    user does not activate within that period, the account will remain
+    permanently inactive unless a site administrator manually activates it.
 
-For example, you might have something like the following in your
-Django settings::
+For example, you might have something like the following in your Django
+settings::
 
     ACCOUNT_ACTIVATION_DAYS = 7 # One-week activation window
 
 
 Setting up URLs
 ~~~~~~~~~~~~~~~
 
-Each bundled registration workflow in django-registration includes a
-Django URLconf which sets up URL patterns for :ref:`the views in
-django-registration <views>`. The URLconf for the two-step activation
-workflow can be found at
-`django_registration.backends.activation.urls`. For example, to place
-the registration URLs under the prefix `/accounts/`, you could add the
-following to your project's root URLconf:
+Each bundled registration workflow in django-registration includes a Django
+URLconf which sets up URL patterns for :ref:`the views in django-registration
+<views>`. The URLconf for the two-step activation workflow can be found at
+``django_registration.backends.activation.urls``. For example, to place the
+registration URLs under the prefix ``/accounts/``, you could add the following
+to your project's root URLconf:
 
 .. code-block:: python
 
    from django.urls import include, path
 
    urlpatterns = [
        # Other URL patterns ...
        path('accounts/', include('django_registration.backends.activation.urls')),
        path('accounts/', include('django.contrib.auth.urls')),
        # More URL patterns ...
    ]
 
 Users would then be able to register by visiting the URL
-`/accounts/register/`, log in (once activated) at
-`/accounts/login/`, etc.
+``/accounts/register/``, log in (once activated) at ``/accounts/login/``, etc.
 
-The sample URL configuration above also sets up the built-in auth
-views included in Django (login, logout, password reset, etc.) via the
-`django.contrib.auth.urls` URLconf.
+The sample URL configuration above also sets up the built-in auth views
+included in Django (login, logout, password reset, etc.) via the
+``django.contrib.auth.urls`` URLconf.
 
 The following URL names are defined by
-`django_registration.backends.activation.urls`:
+``django_registration.backends.activation.urls``:
 
-* `django_registration_register` is the account-registration view.
+* ``django_registration_register`` is the account-registration view.
 
-* `django_registration_complete` is the post-registration success
-  message.
+* ``django_registration_complete`` is the post-registration success message.
 
-* `django_registration_activate` is the account-activation view.
+* ``django_registration_activate`` is the account-activation view.
 
-* `django_registration_activation_complete` is the post-activation
-  success message.
+* ``django_registration_activation_complete`` is the post-activation success
+  message.
 
-* `django_registration_disallowed` is a message indicating registration is
-  not currently permitted.
+* ``django_registration_disallowed`` is a message indicating registration is not
+  currently permitted.
 
 
 .. _default-templates:
 
 Required templates
 ~~~~~~~~~~~~~~~~~~
 
-You will also need to create several templates required by
-django-registration, and possibly additional templates required by
-views in `django.contrib.auth`. The templates required by
-django-registration are as follows; note that, with the exception of
-the templates used for account activation emails, all of these are
-rendered using a :class:`~django.template.RequestContext` and so will
-also receive any additional variables provided by `context processors
+You will also need to create several templates required by django-registration,
+and possibly additional templates required by views in
+``django.contrib.auth``. The templates required by django-registration are as
+follows; note that, with the exception of the templates used for account
+activation emails, all of these are rendered using a
+:class:`~django.template.RequestContext` and so will also receive any
+additional variables provided by `context processors
 <https://docs.djangoproject.com/en/stable/ref/templates/api/#id1>`_.
 
 
 .. _default-form-template:
 
-`django_registration/registration_form.html`
-````````````````````````````````````````````
+``django_registration/registration_form.html``
+``````````````````````````````````````````````
 
-Used to show the form users will fill out to register. By default, has
-the following context:
+Used to show the form users will fill out to register. By default, has the
+following context:
 
-`form`
+``form``
     The registration form. This will likely be a subclass of
     :class:`~django_registration.forms.RegistrationForm`; consult
     `Django's forms documentation
     <https://docs.djangoproject.com/en/stable/topics/forms/>`_ for
     information on how to display this in a template.
 
 
-`django_registration/registration_complete.html`
-````````````````````````````````````````````````
+``django_registration/registration_complete.html``
+``````````````````````````````````````````````````
 
-Used after successful completion of the registration form. This
-template has no context variables of its own, and should inform the
-user that an email containing account-activation information has been
-sent.
+Used after successful completion of the registration form. This template has no
+context variables of its own, and should inform the user that an email
+containing account-activation information has been sent.
 
 
-`django_registration/registration_closed.html`
-``````````````````````````````````````````````````
+``django_registration/registration_closed.html``
+````````````````````````````````````````````````
 
-Used when registration of new user accounts is disabled. This template
-has no context variables of its own.
+Used when registration of new user accounts is disabled. This template has no
+context variables of its own.
 
 
-`django_registration/activation_failed.html`
-````````````````````````````````````````````
+``django_registration/activation_failed.html``
+``````````````````````````````````````````````
 
 Used if account activation fails. Has the following context:
 
-`activation_error`
+``activation_error``
     A :class:`dict` containing the information supplied to the
-    :exc:`~django_registration.exceptions.ActivationError` which
-    occurred during activation. See the documentation for that
-    exception for a description of the keys, and the documentation for
-    :class:`~django_registration.backends.activation.views.ActivationView`
-    for the specific values used in different failure situations.
+    :exc:`~django_registration.exceptions.ActivationError` which occurred
+    during activation. See the documentation for that exception for a
+    description of the keys, and the documentation for
+    :class:`~django_registration.backends.activation.views.ActivationView` for
+    the specific values used in different failure situations.
 
 
-`django_registration/activation_complete.html`
-``````````````````````````````````````````````
+``django_registration/activation_complete.html``
+````````````````````````````````````````````````
 
 Used after successful account activation. This template has no context
-variables of its own, and should inform the user that their account is
-now active.
+variables of its own, and should inform the user that their account is now
+active.
 
 
-`django_registration/activation_email_subject.txt`
-``````````````````````````````````````````````````
+``django_registration/activation_email_subject.txt``
+````````````````````````````````````````````````````
 
-Used to generate the subject line of the activation email. Because the
-subject line of an email must be a single line of text, any output
-from this template will be forcibly condensed to a single line before
-being used. This template has the following context:
+Used to generate the subject line of the activation email. Because the subject
+line of an email must be a single line of text, any output from this template
+will be forcibly condensed to a single line before being used. This template
+has the following context:
 
-`activation_key`
+``activation_key``
     The activation key for the new account, as a string.
 
-`expiration_days`
-    The number of days remaining during which the account may be
-    activated, as an integer.
-
-`request`
-    The :class:`~django.http.HttpRequest` object representing the
-    request in which the user registered.
-
-`scheme`
-    The protocol scheme used during registration, as a string; will be
-    either `'http'` or `'https'`.
-
-`site`
-    An object representing the site on which the user registered;
-    depending on whether `django.contrib.sites` is installed, this may
-    be an instance of either :class:`django.contrib.sites.models.Site`
-    (if the sites application is installed) or
-    :class:`django.contrib.sites.requests.RequestSite` (if
+``expiration_days``
+    The number of days remaining during which the account may be activated, as
+    an integer.
+
+``request``
+    The :class:`~django.http.HttpRequest` object representing the request in
+    which the user registered.
+
+``scheme``
+    The protocol scheme used during registration, as a string; will be either
+    ``'http'`` or ``'https'``.
+
+``site``
+    An object representing the site on which the user registered; depending on
+    whether ``django.contrib.sites`` is installed, this may be an instance of
+    either :class:`django.contrib.sites.models.Site` (if the sites application
+    is installed) or :class:`django.contrib.sites.requests.RequestSite` (if
     not). Consult `the documentation for the Django sites framework
-    <https://docs.djangoproject.com/en/stable/ref/contrib/sites/>`_
-    for details regarding these objects' interfaces.
+    <https://docs.djangoproject.com/en/stable/ref/contrib/sites/>`_ for details
+    regarding these objects' interfaces.
 
-`user`
+``user``
     The newly-created user object.
 
 
-`django_registration/activation_email_body.txt`
-```````````````````````````````````````````````
+``django_registration/activation_email_body.txt``
+`````````````````````````````````````````````````
 
-Used to generate the body of the activation email. Should display a
-link the user can click to activate the account. This template has the
-following context:
+Used to generate the body of the activation email. Should display a link the
+user can click to activate the account. This template has the following
+context:
 
-`activation_key`
+``activation_key``
     The activation key for the new account, as a string.
 
-`expiration_days`
-    The number of days remaining during which the account may be
-    activated, as an integer.
-
-`request`
-    The :class:`~django.http.HttpRequest` object representing the
-    request in which the user registered.
-
-`scheme`
-    The protocol scheme used during registration, as a string; will be
-    either `'http'` or `'https'`.
-
-`site`
-    An object representing the site on which the user registered;
-    depending on whether `django.contrib.sites` is installed, this may
-    be an instance of either :class:`django.contrib.sites.models.Site`
-    (if the sites application is installed) or
-    :class:`django.contrib.sites.requests.RequestSite` (if
+``expiration_days``
+    The number of days remaining during which the account may be activated, as
+    an integer.
+
+``request``
+    The :class:`~django.http.HttpRequest` object representing the request in
+    which the user registered.
+
+``scheme``
+    The protocol scheme used during registration, as a string; will be either
+    `'http'` or `'https'`.
+
+``site``
+    An object representing the site on which the user registered; depending on
+    whether `django.contrib.sites` is installed, this may be an instance of
+    either :class:`django.contrib.sites.models.Site` (if the sites application
+    is installed) or :class:`django.contrib.sites.requests.RequestSite` (if
     not). Consult `the documentation for the Django sites framework
-    <https://docs.djangoproject.com/en/stable/ref/contrib/sites/>`_
-    for details regarding these objects.
+    <https://docs.djangoproject.com/en/stable/ref/contrib/sites/>`_ for details
+    regarding these objects.
 
-`user`
+``user``
     The newly-created user object.
 
-Note that the templates used to generate the account activation email
-use the extension `.txt`, not `.html`. Due to widespread antipathy
-toward and interoperability problems with HTML email,
-django-registration produces plain-text email, and so these templates
-should output plain text rather than HTML.
-
-To make use of the views from `django.contrib.auth` (which are set up
-for you by the example URL configuration above), you will also need to
-create the templates required by those views. Consult `the
-documentation for Django's authentication system
-<https://docs.djangoproject.com/en/stable/topics/auth/>`_ for details
-regarding these templates.
+Note that the templates used to generate the account activation email use the
+extension ``.txt``, not ``.html``. Due to widespread antipathy toward and
+interoperability problems with HTML email, django-registration produces
+plain-text email, and so these templates should output plain text rather than
+HTML.
+
+To make use of the views from ``django.contrib.auth`` (which are set up for you
+by the example URL configuration above), you will also need to create the
+templates required by those views. Consult `the documentation for Django's
+authentication system <https://docs.djangoproject.com/en/stable/topics/auth/>`_
+for details regarding these templates.
 
 
 Configuring the one-step workflow
 --------------------------------------------
 
-Also included is a :ref:`one-step registration workflow
-<one-step-workflow>`, where a user signs up and their account is
-immediately active and logged in.
+Also included is a :ref:`one-step registration workflow <one-step-workflow>`,
+where a user signs up and their account is immediately active and logged in.
 
-You will need to configure URLs to use the one-step workflow; the
-easiest way is to :func:`~django.urls.include` the URLconf
+You will need to configure URLs to use the one-step workflow; the easiest way
+is to :func:`~django.urls.include` the URLconf
 `django_registration.backends.one_step.urls` somewhere in your URL
-configuration. For example, to place the URLs under the prefix
-`/accounts/` in your URL structure:
+configuration. For example, to place the URLs under the prefix `/accounts/` in
+your URL structure:
 
 .. code-block:: python
 
    from django.urls import include, path
 
    urlpatterns = [
        # Other URL patterns ...
        path('accounts/', include('django_registration.backends.one_step.urls')),
        path('accounts/', include('django.contrib.auth.urls')),
        # More URL patterns ...
    ]
 
-Users could then register accounts by visiting the URL
-`/accounts/register/`.
+Users could then register accounts by visiting the URL ``/accounts/register/``.
 
 The following URL names are defined by
-`django_registration.backends.one_step.urls`:
+``django_registration.backends.one_step.urls``:
 
-* `django_registration_register` is the account-registration view.
+* ``django_registration_register`` is the account-registration view.
 
-* `django_registration_complete` is the post-registration success
-  message.
+* ``django_registration_complete`` is the post-registration success message.
 
-* `django_registration_disallowed` is a message indicating registration is
-  not currently permitted.
+* ``django_registration_disallowed`` is a message indicating registration is not
+  currently permitted.
 
-This URLconf will also configure the appropriate URLs for the rest of
-the built-in `django.contrib.auth` views (log in, log out, password
-reset, etc.).
+This URLconf will also configure the appropriate URLs for the rest of the
+built-in `django.contrib.auth` views (log in, log out, password reset, etc.).
 
 Finally, you will need to create following templates:
 
-* `django_registration/registration_form.html`
-* `django_registration/registration_complete.html`
-* `django_registration/registration_closed.html`
-
-See :ref:`the documentation above <default-form-template>` for details
-of these templates.
-
-To make use of the views from `django.contrib.auth` (which are set up
-for you by the example URL configuration above), you will also need to
-create the templates required by those views. Consult `the
-documentation for Django's authentication system
-<https://docs.djangoproject.com/en/stable/topics/auth/>`_ for details
-regarding these templates.
+* ``django_registration/registration_form.html``
+* ``django_registration/registration_complete.html``
+* ``django_registration/registration_closed.html``
+
+See :ref:`the documentation above <default-form-template>` for details of these
+templates.
+
+To make use of the views from ``django.contrib.auth`` (which are set up for you
+by the example URL configuration above), you will also need to create the
+templates required by those views. Consult `the documentation for Django's
+authentication system <https://docs.djangoproject.com/en/stable/topics/auth/>`_
+for details regarding these templates.
```

### Comparing `django-registration-3.3/docs/security.rst` & `django-registration-3.4/docs/security.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,165 +2,155 @@
 
 
 Security guide
 ==============
 
 .. important:: **Reporting security issues**
 
-   If you believe you have found a security issue in
-   django-registration, please do *not* use the public GitHub issue
-   tracker to report it. Instead, you can `contact the author
-   privately <https://www.b-list.org/contact/>`_ to report the issue.
-
-Anything related to users or user accounts has security implications
-and represents a large source of potential security issues. This
-document is not an exhaustive guide to those implications and issues,
-and makes no guarantees that your particular use of Django or
-django-registration will be safe; instead, it provides a set of
-recommendations, and explanations for why django-registration does
-certain things or recommends particular approaches. Using this
-software responsibly is, ultimately, up to you.
-
-Before continuing with this document, you should ensure that you've
-read and understood `Django's security documentation
-<https://docs.djangoproject.com/en/stable/#security>`_.  Django
-provides a good overview of common security issues in the general
-field of web development, and an explanation of how it helps to
-protect against them or provides tools to help you do so.
+   If you believe you have found a security issue in django-registration,
+   please do *not* use the public GitHub issue tracker to report it. Instead,
+   you can `contact the author privately <https://www.b-list.org/contact/>`_ to
+   report the issue.
+
+Anything related to users or user accounts has security implications and
+represents a large source of potential security issues. This document is not an
+exhaustive guide to those implications and issues, and makes no guarantees that
+your particular use of Django or django-registration will be safe; instead, it
+provides a set of recommendations, and explanations for why django-registration
+does certain things or recommends particular approaches. Using this software
+responsibly is, ultimately, up to you.
+
+Before continuing with this document, you should ensure that you've read and
+understood `Django's security documentation
+<https://docs.djangoproject.com/en/stable/#security>`_.  Django provides a good
+overview of common security issues in the general field of web development, and
+an explanation of how it helps to protect against them or provides tools to
+help you do so.
 
-You should also ensure you're following Django's security
-recommendations. You can check for many common issues by running::
+You should also ensure you're following Django's security recommendations. You
+can check for many common issues by running::
 
     python manage.py check --tag security
 
 on your codebase.
 
 
 Recommendation: use the two-step activation workflow
 ----------------------------------------------------
 
-Two user-signup workflows are included in django-registration, along
-with support for writing your own. If you choose to use one of the
-included workflows, :ref:`the two-step activation workflow
-<activation-workflow>` is the recommended default.
-
-The activation workflow provides a verification step -- the user must
-click a link sent to the email address they used to register -- which
-can serve as an impediment to automated account creation for malicious
-purposes.
-
-The activation workflow generates an activation key which consists of
-the new account's username and the timestamp of the signup, verified
-using `Django's cryptographic signing tools
-<https://docs.djangoproject.com/en/1.11/topics/signing/>`_ which in
-turn use `the HMAC implementation from the Python standard library
-<https://docs.python.org/3/library/hmac.html>`_. Thus,
-django-registration is not inventing or building any new cryptography,
-but only using existing/vetted implementations in an approved and
-standard manner.
-
-Additionally, the activation workflow takes steps to ensure that its
-use of HMAC does not act as an `oracle
-<https://en.wikipedia.org/wiki/Oracle_attack>`_. Several parts of
-Django use the signing tools, and third-party applications are free to
-use them as well, so django-registration makes use of the ability to
-supply a salt value for the purpose of "namespacing" HMAC usage. Thus
-an activation token generated by django-registration's activation
-workflow should not be usable for attacks against other HMAC-carrying
-values generated by the same installation of Django.
+Two user-signup workflows are included in django-registration, along with
+support for writing your own. If you choose to use one of the included
+workflows, :ref:`the two-step activation workflow <activation-workflow>` is the
+recommended default.
+
+The activation workflow provides a verification step -- the user must click a
+link sent to the email address they used to register -- which can serve as an
+impediment to automated account creation for malicious purposes.
+
+The activation workflow generates an activation key which consists of the new
+account's username and the timestamp of the signup, verified using `Django's
+cryptographic signing tools
+<https://docs.djangoproject.com/en/1.11/topics/signing/>`_ which in turn use
+`the HMAC implementation from the Python standard library
+<https://docs.python.org/3/library/hmac.html>`_. Thus, django-registration is
+not inventing or building any new cryptography, but only using existing/vetted
+implementations in an approved and standard manner.
+
+Additionally, the activation workflow takes steps to ensure that its use of
+HMAC does not act as an `oracle
+<https://en.wikipedia.org/wiki/Oracle_attack>`_. Several parts of Django use
+the signing tools, and third-party applications are free to use them as well,
+so django-registration makes use of the ability to supply a salt value for the
+purpose of "namespacing" HMAC usage. Thus an activation token generated by
+django-registration's activation workflow should not be usable for attacks
+against other HMAC-carrying values generated by the same installation of
+Django.
 
 
 Restrictions on user names: reserved names
 ------------------------------------------
 
-By default, django-registration applies a list of reserved names, and
-does not permit users to create accounts using those names (see
-:class:`~django_registration.validators.ReservedNameValidator`). The
-default list of reserved names includes many names that could cause
-confusion or even inappropriate access. These reserved names fall into
-several categories:
-
-* Usernames which could allow a user to impersonate or be seen as a
-  site administrator. For example, `'admin'` or `'administrator'`.
-
-* Usernames corresponding to standard/protocol-specific email
-  addresses (relevant for sites where creating an account also creates
-  an email address with that username). For example, `'webmaster'`.
-
-* Usernames corresponding to standard/sensitive subdomain names
-  (relevant for sites where creating an account also creates a
-  subdomain corresponding to the username). For example, `'ftp'` or
-  `'autodiscover'`.
-
-* Usernames which correspond to sensitive URLs (relevant for sites
-  where user profiles appear at a URL containing the username). For
-  example, `'contact'` or `'buy'`.
+By default, django-registration applies a list of reserved names, and does not
+permit users to create accounts using those names (see
+:class:`~django_registration.validators.ReservedNameValidator`). The default
+list of reserved names includes many names that could cause confusion or even
+inappropriate access. These reserved names fall into several categories:
+
+* Usernames which could allow a user to impersonate or be seen as a site
+  administrator. For example, ``"admin"`` or ``"administrator"``.
+
+* Usernames corresponding to standard/protocol-specific email addresses
+  (relevant for sites where creating an account also creates an email address
+  with that username). For example, ``"webmaster"``.
+
+* Usernames corresponding to standard/sensitive subdomain names (relevant for
+  sites where creating an account also creates a subdomain corresponding to the
+  username). For example, ``"ftp"`` or ``"autodiscover"``.
+
+* Usernames which correspond to sensitive URLs (relevant for sites where user
+  profiles appear at a URL containing the username). For example, ``"contact"``
+  or ``"buy"``.
 
-It is strongly recommended that you leave the reserved-name validation
-enabled.
+It is strongly recommended that you leave the reserved-name validation enabled.
 
 
 Restrictions on user names and email addresses: Unicode
 -------------------------------------------------------
 
-By default, django-registration permits the use of a wide range of
-Unicode in usernames and email addresses. However, to prevent some
-types of Unicode-related attacks, django-registration will not permit
-certain specific uses of Unicode characters.
-
-For example, while the username `'admin'` cannot normally be
-registered (see above), a user might still attempt to register a name
-that appears visually identical, by substituting a Cyrillic 'a' or
-other similar-appearing character for the first character. This is a
-`homograph attack
+By default, django-registration permits the use of a wide range of Unicode in
+usernames and email addresses. However, to prevent some types of
+Unicode-related attacks, django-registration will not permit certain specific
+uses of Unicode characters.
+
+For example, while the username ``"admin"`` cannot normally be registered (see
+above), a user might still attempt to register a name that appears visually
+identical, by substituting a Cyrillic "a or other similar-appearing character
+for the first character. This is a `homograph attack
 <https://en.wikipedia.org/wiki/IDN_homograph_attack>`_.
 
-To prevent homograph attacks, django-registration applies the
-following rule to usernames, and to the local-part and the domain of
-email addresses:
-
-* If the submitted value is mixed-script (contains characters from
-  multiple different scripts, as in the above example which would mix
-  Cyrillic and Latin characters), and
+To prevent homograph attacks, django-registration applies the following rule to
+usernames, and to the local-part and the domain of email addresses:
 
-* If the submitted value contains characters appearing in the Unicode
-  Visually Confusable Characters file,
+* If the submitted value is mixed-script (contains characters from multiple
+  different scripts, as in the above example which would mix Cyrillic and Latin
+  characters), and
+
+* If the submitted value contains characters appearing in the Unicode Visually
+  Confusable Characters file,
 
 * Then the value will be rejected.
 
 See :func:`~django_registration.validators.validate_confusables` and
 :func:`~django_registration.validators.validate_confusables_email`.
 
 This should not interfere with legitimate use of Unicode, or of
-non-English/non-Latin characters in usernames and email addresses. To
-avoid a common false-positive situation, the local-part and domain of
-an email address are checked independently of each other.
+non-English/non-Latin characters in usernames and email addresses. To avoid a
+common false-positive situation, the local-part and domain of an email address
+are checked independently of each other.
 
 It is strongly recommended that you leave this validation enabled.
 
 
 Additional steps to secure user accounts
 ----------------------------------------
 
-The scope of django-registration is solely the implementation of
-user-signup workflows, which limits the ways in which
-django-registration alone can protect your users. Other features of
-Django itself, or of other third-party applications, can provide
-significant increases in protection.
+The scope of django-registration is solely the implementation of user-signup
+workflows, which limits the ways in which django-registration alone can protect
+your users. Other features of Django itself, or of other third-party
+applications, can provide significant increases in protection.
 
 In particular, it is recommended that you:
 
-* Prevent the use of common passwords. You can catch some common
-  passwords by enabling Django's
+* Prevent the use of common passwords. You can catch some common passwords by
+  enabling Django's
   :class:`~django.contrib.auth.password_validation.CommonPasswordValidator`,
-  which uses a list of twenty thousand common passwords. A more
-  comprehensive option is the password validator and other utilities
-  from `pwned-passwords-django
-  <https://pwned-passwords-django.readthedocs.io/en/stable/>`_, which
-  checks against a database containing (as of mid-2018) over half a
-  billion passwords found in data breaches.
-
-* Use two-factor authentication via authenticator applications or
-  hardware security keys (*not* SMS). The package `django-two-factor
-  <https://django-two-factor-auth.readthedocs.io/en/stable/>`_
-  provides integration for two-factor authentication into Django's
-  auth framework.
+  which uses a list of twenty thousand common passwords. A more comprehensive
+  option is the password validator and other utilities from
+  `pwned-passwords-django
+  <https://pwned-passwords-django.readthedocs.io/en/stable/>`_, which checks
+  against a database containing (as of mid-2018) over half a billion passwords
+  found in data breaches.
+
+* Use two-factor authentication via authenticator applications or hardware
+  security keys (*not* SMS). The package `django-two-factor
+  <https://django-two-factor-auth.readthedocs.io/en/stable/>`_ provides
+  integration for two-factor authentication into Django's auth framework.
```

### Comparing `django-registration-3.3/docs/settings.rst` & `django-registration-3.4/docs/settings.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 .. _settings:
 .. module:: django.conf.settings
 
 
 Custom settings
 ===============
 
-Although the choice of registration workflow does not necessarily
-require changes to your Django settings (as registration workflows are
-selected by including the appropriate URL patterns in your root
-URLconf), the built-in workflows of django-registration make use
-of several custom settings.
+Although the choice of registration workflow does not necessarily require
+changes to your Django settings (as registration workflows are selected by
+including the appropriate URL patterns in your root URLconf), the built-in
+workflows of django-registration make use of several custom settings.
 
 
 .. data:: ACCOUNT_ACTIVATION_DAYS
 
-   An :class:`int` indicating how long (in days) after signup an
-   account has in which to activate.
+   An :class:`int` indicating how long (in days) after signup an account has in
+   which to activate.
 
    Used by:
 
    * :ref:`The two-step activation workflow <activation-workflow>`
 
 
 .. data:: REGISTRATION_OPEN
 
-   A :class:`bool` indicating whether registration of new accounts is
-   currently permitted.
+   A :class:`bool` indicating whether registration of new accounts is currently
+   permitted.
 
-   A default of `True` is assumed when this setting is not supplied,
-   so specifying it is optional unless you want to temporarily close
-   registration (in which case, set it to `False`).
+   A default of :data:`True` is assumed when this setting is not supplied, so
+   specifying it is optional unless you want to temporarily close registration
+   (in which case, set it to :data:`False`).
 
-   Used by: 
+   Used by:
 
    * :ref:`The two-step activation workflow <activation-workflow>`
 
    * :ref:`The one-step workflow <one-step-workflow>`
 
-   Third-party workflows wishing to use an alternate method of
-   determining whether registration is allowed should subclass
+   Third-party workflows wishing to use an alternate method of determining
+   whether registration is allowed should subclass
    :class:`django_registration.views.RegistrationView` (or a subclass of it
    from an existing workflow) and override
    :meth:`~django_registration.views.RegistrationView.registration_allowed`.
 
 
 .. data:: REGISTRATION_SALT
 
-   A :class:`str` used as an additional "salt" in the process of
-   generating signed activation keys.
+   A :class:`str` used as an additional "salt" in the process of generating
+   signed activation keys.
 
-   This setting is optional, and a default of `"registration"` will
-   be used if not specified. The value of this setting does not need
-   to be kept secret; see :ref:`the note about this salt value and
-   security <salt-security>` for details.
+   This setting is optional, and a default of ``"registration"`` will be used if
+   not specified. The value of this setting does not need to be kept secret;
+   see :ref:`the note about this salt value and security <salt-security>` for
+   details.
 
    Used by:
 
    * :ref:`The two-step activation workflow <activation-workflow>`
```

### Comparing `django-registration-3.3/docs/signals.rst` & `django-registration-3.4/docs/signals.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,69 @@
 .. _signals:
 .. module:: django_registration.signals
 
 
 Signals used by django-registration
 ===================================
 
-Much of django-registration's customizability comes through the
-ability to write and use different workflows for user
-registration. However, there are many cases where only a small bit of
-additional logic needs to be injected into the registration process,
-and writing a custom workflow to support this represents an
-unnecessary amount of work. A more lightweight customization option is
-provided through two custom signals which the built-in registration
-workflows send, and custom workflows are encouraged to send, at
-specific points during the registration process; functions listening
-for these signals can then add whatever logic is needed.
-
-For general documentation on signals and the Django dispatcher,
-consult `Django's signals documentation
-<http://docs.djangoproject.com/en/stable/topics/signals/>`_. This
-documentation assumes that you are familiar with how signals work and
-the process of writing and connecting functions which will listen for
-signals.
+Much of django-registration's customizability comes through the ability to
+write and use different workflows for user registration. However, there are
+many cases where only a small bit of additional logic needs to be injected into
+the registration process, and writing a custom workflow to support this
+represents an unnecessary amount of work. A more lightweight customization
+option is provided through two custom signals which the built-in registration
+workflows send, and custom workflows are encouraged to send, at specific points
+during the registration process; functions listening for these signals can then
+add whatever logic is needed.
+
+For general documentation on signals and the Django dispatcher, consult
+`Django's signals documentation
+<http://docs.djangoproject.com/en/stable/topics/signals/>`_. This documentation
+assumes that you are familiar with how signals work and the process of writing
+and connecting functions which will listen for signals.
 
 
 .. data:: user_activated
 
    Sent when a user account is activated (not applicable to all
    workflows). Provides the following arguments:
 
-   `sender`
-       The :class:`~django_registration.views.ActivationView` subclass used
-       to activate the user.
+   ``sender``
+       The :class:`~django_registration.views.ActivationView` subclass used to
+       activate the user.
 
-   `user`
+   ``user``
         A user-model instance representing the activated account.
 
-   `request`
+   ``request``
        The :class:`~django.http.HttpRequest` in which the account was
        activated.
 
    This signal is automatically sent for you by the base
-   :class:`~django_registration.views.ActivationView`, so unless
-   you've overridden its
-   :meth:`~django.views.generic.base.TemplateView.get` method in a
-   subclass you should not need to explicitly send it.
+   :class:`~django_registration.views.ActivationView`, so unless you've
+   overridden its :meth:`~django.views.generic.base.TemplateView.get` method in
+   a subclass you should not need to explicitly send it.
 
 
 .. data:: user_registered
 
    Sent when a new user account is registered. Provides the following
    arguments:
 
-   `sender`
+   ``sender``
        The :class:`~django_registration.views.RegistrationView` subclass used
        to register the account.
 
-   `user`
+   ``user``
         A user-model instance representing the new account.
 
-   `request`
-        The :class:`~django.http.HttpRequest` in which the new account
-        was registered.
+   ``request``
+        The :class:`~django.http.HttpRequest` in which the new account was
+        registered.
 
    This signal is **not** automatically sent for you by the base
-   :class:`~django_registration.views.RegistrationView`. It is sent by
-   the subclasses implemented for the three included registration
-   workflows, but if you write your own subclass of
-   :class:`~django_registration.views.RegistrationView`, you'll need
-   to send this signal as part of the implementation of the
-   :meth:`~django_registration.views.RegistrationView.register`
-   method.
+   :class:`~django_registration.views.RegistrationView`. It is sent by the
+   subclasses implemented for the three included registration workflows, but if
+   you write your own subclass of
+   :class:`~django_registration.views.RegistrationView`, you'll need to send
+   this signal as part of the implementation of the
+   :meth:`~django_registration.views.RegistrationView.register` method.
```

### Comparing `django-registration-3.3/docs/spelling_wordlist.txt` & `django-registration-3.4/docs/spelling_wordlist.txt`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 auth
 authenticator
 autoconfig
 backend
 backends
 Backend
 Backends
+Bluesky
 blog
 boolean
 bugfixes
 checkbox
 cleanupregistration
 codebase
 confusable
```

### Comparing `django-registration-3.3/docs/upgrade.rst` & `django-registration-3.4/docs/upgrade.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,345 +1,346 @@
 .. _upgrade:
 
 
 Upgrading from previous versions
 ================================
 
-The current release series of django-registration is the 3.x series,
-which is not backwards-compatible with the django-registration 2.x
-release series.
+The current release series of django-registration is the 3.x series, which is
+not backwards-compatible with the django-registration 2.x release series.
 
 
 Changes within the 3.x series
 -----------------------------
 
-Within the 3.x release series, there have been several minor changes
-and improvements, documented here along with the version in which they
-occurred.
+Within the 3.x release series, there have been several minor changes and
+improvements, documented here along with the version in which they occurred.
+
+django-registration 3.4
+~~~~~~~~~~~~~~~~~~~~~~~
+
+* The :ref:`reserved names list <reserved-names>` has a new entry: ``"xrpc"``,
+  which is used in domain-ownership verification by Bluesky/AT protocol.
+
+* Validation of the email field in registration forms no longer applies
+  Django's default email validator, instead applying only django-registration's
+  :class:`~django_registration.validators.HTML5EmailValidator` and
+  :func:`~django_registration.validators.validate_confusables_email`. Since
+  django-registration's validators are significantly stricter, this does not
+  actually change the set of email addresses which will be accepted; all it
+  does is prevent a duplicate error message displaying when both the default
+  Django validator and the django-registration validators reject the email
+  address. See `GitHub issue #238
+  <https://github.com/ubernostrum/django-registration/issues/238>`_.
+
+* The supported Python and Django versions are changed to: Django 3.2, 4.1, and
+  4.2, on Python 3.7 (Django 3.2 only), 3.8, 3.9, 3.10, and 3.11 (Django 4.1
+  and 4.2 only).
 
 django-registration 3.3
 ~~~~~~~~~~~~~~~~~~~~~~~
 
-This release contains no new features or bugfixes. The supported
-Python and Django versions are changed to:
+This release contains no new features or bugfixes. The supported Python and
+Django versions are changed to:
 
 * Django 3.2 and 4.0, on Python 3.7 (Django 3.2 only), 3.8, 3.9, and 3.10.
 
 django-registration 3.2
 ~~~~~~~~~~~~~~~~~~~~~~~
 
-This release contains no new features or bugfixes. The supported
-Python and Django versions are changed to:
+This release contains no new features or bugfixes. The supported Python and
+Django versions are changed to:
 
 * Django 2.2, 3.1, and 3.2, on Python 3.6, 3.7, 3.8, and 3.9.
 
-Python 3.5 reached the end of its upstream support cycle in September
-2020, and is no longer supported. Django 3.0 reached the end of its
-upstream support cycle in May 2021, and is no longer supported.
+Python 3.5 reached the end of its upstream support cycle in September 2020, and
+is no longer supported. Django 3.0 reached the end of its upstream support
+cycle in May 2021, and is no longer supported.
 
 django-registration 3.1.2
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 This release fixes a security issue with low severity.
 
 Prior to 3.1.2, django-registration did not apply Django's
-:func:`~django.views.decorators.debug.sensitive_post_parameters`
-decorator to the base
-:class:`~django_registration.views.RegistrationView`. This meant that
-if detailed error reports, such as `Django's error reports emailed to
-site staff
+:func:`~django.views.decorators.debug.sensitive_post_parameters` decorator to
+the base :class:`~django_registration.views.RegistrationView`. This meant that
+if detailed error reports, such as `Django's error reports emailed to site
+staff
 <https://docs.djangoproject.com/en/3.1/howto/error-reporting/#email-reports>`_,
-were enabled, and a server-side error occurred during account
-registration, the generated error report would include all fields
-submitted in the HTTP request, some of which are potentially sensitive
-depending on the user-account model and registration workflow in use.
+were enabled, and a server-side error occurred during account registration, the
+generated error report would include all fields submitted in the HTTP request,
+some of which are potentially sensitive depending on the user-account model and
+registration workflow in use.
 
-This issue is CVE-2021-21416 and GitHub security advisory
-GHSA-58c7-px5v-82hh.
+This issue is CVE-2021-21416 and GitHub security advisory GHSA-58c7-px5v-82hh.
 
 Thanks to Martin Morgenstern for reporting this issue.
 
 Django-registration 3.1
 ~~~~~~~~~~~~~~~~~~~~~~~
 
-* When an attempt was made to use django-registration with a custom
-  user model, but *without* explicitly subclassing
-  :class:`~django_registration.forms.RegistrationForm` to point to
-  that user model, previously the result would be a cryptic exception
-  and error message raised from within Django, complaining about
-  trying to work with the swapped-out user
-  model. :class:`~django_registration.views.RegistrationView` now
-  explicitly raises
-  :exc:`~django.core.exceptions.ImproperlyConfigured` with an
-  informative error message to make it clear what has happened, and
-  directs the developer to the documentation for using custom user
-  models in django-registration.
+* When an attempt was made to use django-registration with a custom user model,
+  but *without* explicitly subclassing
+  :class:`~django_registration.forms.RegistrationForm` to point to that user
+  model, previously the result would be a cryptic exception and error message
+  raised from within Django, complaining about trying to work with the
+  swapped-out user model. :class:`~django_registration.views.RegistrationView`
+  now explicitly raises :exc:`~django.core.exceptions.ImproperlyConfigured`
+  with an informative error message to make it clear what has happened, and
+  directs the developer to the documentation for using custom user models in
+  django-registration.
 
 * A new validator,
-  :class:`~django_registration.validators.HTML5EmailValidator`, is
-  included and is applied by default to the email field of
-  :class:`~django_registration.forms.RegistrationForm`. The HTML5
-  email address grammar is more restrictive than the RFC grammar, but
-  primarily in disallowing rare and problematic features.
-
-* Support for Python 2 was dropped, as Python 2 is EOL as of
-  2020-01-01. As a result, support for Django 1.11 (EOL April 2020)
-  was also dropped; the minimum supported Django version is now 2.2.
+  :class:`~django_registration.validators.HTML5EmailValidator`, is included and
+  is applied by default to the email field of
+  :class:`~django_registration.forms.RegistrationForm`. The HTML5 email address
+  grammar is more restrictive than the RFC grammar, but primarily in
+  disallowing rare and problematic features.
+
+* Support for Python 2 was dropped, as Python 2 is EOL as of 2020-01-01. As a
+  result, support for Django 1.11 (EOL April 2020) was also dropped; the
+  minimum supported Django version is now 2.2.
 
 
 django-registration 3.0.1
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * The :ref:`custom validators <validators>` are now serializable.
 
-* Although no code changes were required, this release officially
-  marks itself compatible with Python 3.7 and with django 2.2.
+* Although no code changes were required, this release officially marks itself
+  compatible with Python 3.7 and with django 2.2.
 
 
 Changes between django-registration 2.x and 3.x
 -----------------------------------------------
 
 Module renaming
 ~~~~~~~~~~~~~~~
 
 Prior to 3.x, django-registration installed a Python module named
-`registration`. To avoid silent incompatibilities, and to conform to
-more recent best practices, django-registration 3.x now installs a
-module named `django_registration`. Attempts to import from the
-`registration` module will immediately fail with :exc:`ImportError`.
+``registration``. To avoid silent incompatibilities, and to conform to more
+recent best practices, django-registration 3.x now installs a module named
+``django_registration``. Attempts to import from the ``registration`` module will
+immediately fail with :exc:`ImportError`.
 
 Many installations will be able to adapt by replacing references to
-`registration` with references to `django_registration`.
+``registration`` with references to ``django_registration``.
 
 
 Removal of model-based workflow
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The two-step model-based signup workflow, which has been present since
-the first public release of django-registration in 2007, has now been
-removed. In its place, it is recommended that you use :ref:`the
-two-step activation workflow <activation-workflow>` instead, as that
-workflow requires no server-side storage of additional data beyond the
-user account itself.
+The two-step model-based signup workflow, which has been present since the
+first public release of django-registration in 2007, has now been removed. In
+its place, it is recommended that you use :ref:`the two-step activation
+workflow <activation-workflow>` instead, as that workflow requires no
+server-side storage of additional data beyond the user account itself.
 
 
 Renaming of two-step activation workflow
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-:ref:`The two-step activation workflow <activation-workflow>` was
-previously found at `registration.backends.hmac`; it has been
-renamed and is now found at `registration.backends.activation`.
+:ref:`The two-step activation workflow <activation-workflow>` was previously
+found at ``registration.backends.hmac``; it has been renamed and is now found at
+``registration.backends.activation``.
 
 
 Renaming of one-step workflow
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-:ref:`The one-step workflow <one-step-workflow>` was previously found
-at `registration.backends.simple`; it has been renamed and is now
-found at `registration.backends.one_step`.
+:ref:`The one-step workflow <one-step-workflow>` was previously found at
+``registration.backends.simple``; it has been renamed and is now found at
+``registration.backends.one_step``.
 
 
 Removal of auth URLs
 ~~~~~~~~~~~~~~~~~~~~
 
-Prior to 3.x, django-registration's default URLconf modules for its
-built-in workflows would attempt to include the Django auth views
-(login, logout, password reset, etc.) for you. This became untenable
-with the rewrite of Django's auth views to be class-based, as it
-required detecting the set of auth views and choosing a set of URL
-patterns at runtime.
-
-As a result, auth views are no longer automatically configured for
-you; if you want them, :func:`~django.urls.include` the URLconf
-`django.contrib.auth.urls` at a location of your choosing.
+Prior to 3.x, django-registration's default URLconf modules for its built-in
+workflows would attempt to include the Django auth views (login, logout,
+password reset, etc.) for you. This became untenable with the rewrite of
+Django's auth views to be class-based, as it required detecting the set of auth
+views and choosing a set of URL patterns at runtime.
+
+As a result, auth views are no longer automatically configured for you; if you
+want them, :func:`~django.urls.include` the URLconf ``django.contrib.auth.urls``
+at a location of your choosing.
 
 
 Distinguishing activation failure conditions
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Prior to 3.x, failures to activate a user account (in workflows which
-use activation) all simply returned `None` in place of the activated
-account. This meant it was not possible to determine, from inspecting
-the result, what exactly caused the failure.
+Prior to 3.x, failures to activate a user account (in workflows which use
+activation) all simply returned :data:`None` in place of the activated
+account. This meant it was not possible to determine, from inspecting the
+result, what exactly caused the failure.
 
 In django-registration 3.x, activation failures raise an exception --
-:exc:`~django_registration.exceptions.ActivationError` -- with a
-message and code (such as `"expired"`), to indicate the cause of
-failure. This exception is caught by
-:class:`~django_registration.views.ActivationView` and turned into the
-template context variable `activation_error`.
+:exc:`~django_registration.exceptions.ActivationError` -- with a message and
+code (such as ``"expired"``), to indicate the cause of failure. This exception is
+caught by :class:`~django_registration.views.ActivationView` and turned into
+the template context variable ``activation_error``.
 
 
 Changes to custom user support
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Support for custom user models has been brought more in line with the
-features Django offers. This affects compatibility of custom user
-models with django-registration's default forms and views. In
-particular, custom user models should now provide, in addition to
+Support for custom user models has been brought more in line with the features
+Django offers. This affects compatibility of custom user models with
+django-registration's default forms and views. In particular, custom user
+models should now provide, in addition to
 :attr:`~django.contrib.auth.CustomUser.USERNAME_FIELD`, the
 :meth:`~django.contrib.auth.models.AbstractBaseUser.get_username` and
 :meth:`~django.contrib.auth.models.AbstractBaseUser.get_email_field_name`
-methods. See :ref:`the custom user documentation <custom-user>` for
-details.
+methods. See :ref:`the custom user documentation <custom-user>` for details.
 
 
-Changes to `success_url`
+Changes to ``success_url``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Both the registration and activation views mimic Django's own generic
-views in supporting a choice of ways to specify where to redirect
-after a successful registration or activation; you can either set the
-attribute
-:attr:`~django_registration.views.RegistrationView.success_url` on the
-view class, or implement the method
-:meth:`~django_registration.views.RegistrationView.get_success_url`
-. However, there is a key difference between the base Django
-generic-view version of this, and the version in django-registration:
-when calling a
-:meth:`~django_registration.views.RegistrationView.get_success_url`
-method, django-registration passes the user account as an argument.
+Both the registration and activation views mimic Django's own generic views in
+supporting a choice of ways to specify where to redirect after a successful
+registration or activation; you can either set the attribute
+:attr:`~django_registration.views.RegistrationView.success_url` on the view
+class, or implement the method
+:meth:`~django_registration.views.RegistrationView.get_success_url` . However,
+there is a key difference between the base Django generic-view version of this,
+and the version in django-registration: when calling a
+:meth:`~django_registration.views.RegistrationView.get_success_url` method,
+django-registration passes the user account as an argument.
 
 This is incompatible with the behavior of Django's base
 :class:`~django.views.generic.edit.FormMixin`, which expects
-:meth:`~django.views.generic.edit.FormMixin.get_success_url` to take
-zero arguments.
+:meth:`~django.views.generic.edit.FormMixin.get_success_url` to take zero
+arguments.
 
 Also, earlier versions of django-registration allowed
 :attr:`~django_registration.views.RegistrationView.success_url` and
-:meth:`~django_registration.views.RegistrationView.get_success_url` to
-provide either a string URL, or a tuple of `(viewname, args,
-kwargs)` to pass to Django's :func:`~django.urls.reverse` helper, in
-order to work around issues caused by calling
-:func:`~django.urls.reverse` at the level of a class attribute.
-
-In django-registration 3.x, the `user` argument to
-:meth:`~django_registration.views.RegistrationView.get_success_url` is
-now optional, meaning :class:`~django.views.generic.edit.FormMixin`'s
-default behavior is now compatible with any
+:meth:`~django_registration.views.RegistrationView.get_success_url` to provide
+either a string URL, or a tuple of ``(viewname, args, kwargs)`` to pass to
+Django's :func:`~django.urls.reverse` helper, in order to work around issues
+caused by calling :func:`~django.urls.reverse` at the level of a class
+attribute.
+
+In django-registration 3.x, the ``user`` argument to
+:meth:`~django_registration.views.RegistrationView.get_success_url` is now
+optional, meaning :class:`~django.views.generic.edit.FormMixin`'s default
+behavior is now compatible with any
 :meth:`~django_registration.views.RegistrationView.get_success_url`
 implementation that doesn't require the user object; as a result,
-implementations which don't rely on the user object should either
-switch to specifying
-:attr:`~django_registration.views.RegistrationView.success_url` as an
-attribute, or change their own signature to `get_success_url(self,
-user=None)`.
+implementations which don't rely on the user object should either switch to
+specifying :attr:`~django_registration.views.RegistrationView.success_url` as
+an attribute, or change their own signature to ``get_success_url(self,
+user=None)``.
 
 Also, the ability to supply the 3-tuple of arguments for
 :func:`~django.urls.reverse` has been removed; both
 :attr:`~django_registration.views.RegistrationView.success_url` and
-:meth:`~django_registration.views.RegistrationView.get_success_url`
-now *must* be/return either a string, or a lazy object that resolves
-to a string. To avoid class-level calls to
-:func:`~django.urls.reverse`, use `django.urls.reverse_lazy()`
-instead.
+:meth:`~django_registration.views.RegistrationView.get_success_url` now *must*
+be/return either a string, or a lazy object that resolves to a string. To avoid
+class-level calls to :func:`~django.urls.reverse`, use
+``django.urls.reverse_lazy()`` instead.
 
 
 Removed "no free email" form
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Earlier versions of django-registration included a form class,
-`RegistrationFormNoFreeEmail`, which attempted to forbid user
-signups using common free/throwaway email providers. Since this is a
-pointless task (the number of possible domains of such providers is
-ever-growing), this form class has been removed.
+``RegistrationFormNoFreeEmail``, which attempted to forbid user signups using
+common free/throwaway email providers. Since this is a pointless task (the
+number of possible domains of such providers is ever-growing), this form class
+has been removed.
 
 
 Template names
 ~~~~~~~~~~~~~~
 
-Since django-registration's Python module has been renamed from
-`registration` to `django_registration`, its default template
-folder has also been renamed, from `registration` to
-`django_registration`. Additionally, the following templates have
-undergone name changes:
-
-* The default template name for the body of the activation email in
-  the two-step activation workflow is now
-  `django_registration/activation_email_body.txt` (previously, it
-  was `registration/activation_email.txt`)
+Since django-registration's Python module has been renamed from ``registration``
+to ``django_registration``, its default template folder has also been renamed,
+from ``registration`` to ``django_registration``. Additionally, the following
+templates have undergone name changes:
+
+* The default template name for the body of the activation email in the
+  two-step activation workflow is now
+  ``django_registration/activation_email_body.txt`` (previously, it was
+  ``registration/activation_email.txt``)
 
 * The default template name for
-  :class:`~django_registration.views.ActivationView` and its
-  subclasses is now `django_registration/activation_failed.html`
-  (previously, it was `registration/activate.html`).
+  :class:`~django_registration.views.ActivationView` and its subclasses is now
+  ``django_registration/activation_failed.html`` (previously, it was
+  ``registration/activate.html``).
 
 
 Renaming of URL patterns
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
-Prior to 3.x, django-registration's included URLconf modules provided
-URL pattern names beginning with `"registration"`. For example:
-`"registration_register"`. In 3.x, these are all renamed to begin
-with `"django_registration"`. For example:
-`"django_registration_register"`.
+Prior to 3.x, django-registration's included URLconf modules provided URL
+pattern names beginning with ``"registration"``. For example:
+``"registration_register"``. In 3.x, these are all renamed to begin with
+``"django_registration"``. For example: ``"django_registration_register"``.
 
-Removal of `cleanupregistration` management command
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Removal of ``cleanupregistration`` management command
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The "cleanupregistration" management command, and the
 RegistrationProfile.objects.delete_expired_users() and
-RegistrationProfile.objects.expired() methods, were removed
-in django-registration 3.0.
-Deployments which need a way to identify and delete
-expired accounts should determine how they wish to do so
-and implement their own methods for this.
+RegistrationProfile.objects.expired() methods, were removed in
+django-registration 3.0.  Deployments which need a way to identify and delete
+expired accounts should determine how they wish to do so and implement their
+own methods for this.
 
 Other changes
 ~~~~~~~~~~~~~
 
-The URLconf `registration.urls` has been removed; it was an alias
-for the URLconf of the model-based workflow, which has also been
-removed.
+The URLconf ``registration.urls`` has been removed; it was an alias for the
+URLconf of the model-based workflow, which has also been removed.
 
-The compatibility alias `registration.backends.default`, which also
-pointed to the model-based workflow, has been removed.
+The compatibility alias ``registration.backends.default``, which also pointed to
+the model-based workflow, has been removed.
 
 
 Changes during the 2.x release series
 -------------------------------------
 
-One major change occurred between django-registration 2.0 and 2.1: the
-addition in version 2.1 of the
+One major change occurred between django-registration 2.0 and 2.1: the addition
+in version 2.1 of the
 :class:`~django_registration.validators.ReservedNameValidator`, which is now
-used by default on :class:`~django_registration.forms.RegistrationForm` and
-its subclasses.
+used by default on :class:`~django_registration.forms.RegistrationForm` and its
+subclasses.
 
-This is technically backwards-incompatible, since a set of usernames
-which previously could be registered now cannot be registered, but was
-included because the security benefits outweigh the edge cases of the
-now-disallowed usernames. If you need to allow users to register with
-usernames forbidden by this validator, see its documentation for notes
-on how to customize or disable it.
-
-In 2.2, the behavior of the `RegistrationProfile.expired()` method
-was clarified to accommodate user expectations; it does *not* return
-(and thus, `RegistrationProfile.delete_expired_users()` does not
-delete) profiles of users who had successfully activated.
+This is technically backwards-incompatible, since a set of usernames which
+previously could be registered now cannot be registered, but was included
+because the security benefits outweigh the edge cases of the now-disallowed
+usernames. If you need to allow users to register with usernames forbidden by
+this validator, see its documentation for notes on how to customize or disable
+it.
+
+In 2.2, the behavior of the ``RegistrationProfile.expired()`` method was
+clarified to accommodate user expectations; it does *not* return (and thus,
+``RegistrationProfile.delete_expired_users()`` does not delete) profiles of users
+who had successfully activated.
 
 In django-registration 2.3, the new validators
 :func:`~django_registration.validators.validate_confusables` and
-:func:`~django_registration.validators.validate_confusables_email` were
-added, and are applied by default to the username field and email
-field, respectively, of registration forms. This may cause some
-usernames which previously were accepted to no longer be accepted, but
-like the reserved-name validator this change was made because its
-security benefits significantly outweigh the edge cases in which it
-might disallow an otherwise-acceptable username or email address. If
-for some reason you need to allow registration with usernames or email
-addresses containing potentially dangerous use of Unicode, you can
-subclass the registration form and remove these validators, though
-doing so is not recommended.
+:func:`~django_registration.validators.validate_confusables_email` were added,
+and are applied by default to the username field and email field, respectively,
+of registration forms. This may cause some usernames which previously were
+accepted to no longer be accepted, but like the reserved-name validator this
+change was made because its security benefits significantly outweigh the edge
+cases in which it might disallow an otherwise-acceptable username or email
+address. If for some reason you need to allow registration with usernames or
+email addresses containing potentially dangerous use of Unicode, you can
+subclass the registration form and remove these validators, though doing so is
+not recommended.
 
 
 Versions prior to 2.0
 ---------------------
 
-A 1.0 release of django-registration existed, but the 2.x series was
-compatible with it.
+A 1.0 release of django-registration existed, but the 2.x series was compatible
+with it.
 
-Prior to 1.0, the most widely-adopted version of django-registration
-was 0.8; the changes from 0.8 to 2.x were large and significant, and
-if any installations on 0.8 still exist and wish to upgrade to more
-recent versions, it is likely the most effective route will be to
-discard all code using 0.8 and start over from scratch with a 3.x
-release.
+Prior to 1.0, the most widely-adopted version of django-registration was 0.8;
+the changes from 0.8 to 2.x were large and significant, and if any
+installations on 0.8 still exist and wish to upgrade to more recent versions,
+it is likely the most effective route will be to discard all code using 0.8 and
+start over from scratch with a 3.x release.
```

### Comparing `django-registration-3.3/docs/validators.rst` & `django-registration-3.4/docs/validators.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 .. _validators:
 .. module:: django_registration.validators
 
 Validation utilities
 ====================
 
-To ease the process of validating user registration data,
-django-registration includes some validation-related data and
-utilities.
+To ease the process of validating user registration data, django-registration
+includes some validation-related data and utilities.
 
 
 Error messages
 --------------
 
-Several error messages are available as constants. All of them are
-marked for translation; most have translations already provided in
-django-registration.
+Several error messages are available as constants. All of them are marked for
+translation; most have translations already provided in django-registration.
 
 .. data:: DUPLICATE_EMAIL
 
    Error message raised by
    :class:`~django_registration.forms.RegistrationFormUniqueEmail` when the
    supplied email address is not unique.
 
 .. data:: DUPLICATE_USERNAME
 
    Error message raised by
-   :class:`~django_registration.validators.CaseInsensitiveValidator`
-   when the supplied username is not unique. This is the same string
-   raised by Django's default
-   :class:`~django.contrib.auth.models.User` model for a non-unique
+   :class:`~django_registration.validators.CaseInsensitiveValidator` when the
+   supplied username is not unique. This is the same string raised by Django's
+   default :class:`~django.contrib.auth.models.User` model for a non-unique
    username.
 
 .. data:: RESERVED_NAME
 
    Error message raised by
    :class:`~django_registration.validators.ReservedNameValidator` when it is
    given a value that is a reserved name.
@@ -40,184 +37,178 @@
 .. data:: TOS_REQUIRED
 
    Error message raised by
    :class:`~django_registration.forms.RegistrationFormTermsOfService` when
    the terms-of-service field is not checked.
 
 
+.. _reserved-names:
+
 Rejecting "reserved" usernames
 ------------------------------
 
 By default, django-registration treats some usernames as reserved.
 
 .. note:: **Why reserved names are reserved**
 
-   Many Web applications enable per-user URLs (to display account
-   information), and some may also create email addresses or even
-   subdomains, based on a user's username. While this is often useful,
-   it also represents a risk: a user might register a name which
-   conflicts with an important URL, email address or subdomain, and
-   this might give that user control over it.
+   Many Web applications enable per-user URLs (to display account information),
+   and some may also create email addresses or even subdomains, based on a
+   user's username. While this is often useful, it also represents a risk: a
+   user might register a name which conflicts with an important URL, email
+   address or subdomain, and this might give that user control over it.
 
-   django-registration includes a list of reserved names, and rejects
-   them as usernames by default, in order to avoid this issue.
+   django-registration includes a list of reserved names, and rejects them as
+   usernames by default, in order to avoid this issue.
 
 .. class:: ReservedNameValidator(reserved_names)
 
    A callable validator class (see `Django's validators documentation
    <https://docs.djangoproject.com/en/stable/ref/validators/>`_) which
    prohibits the use of a reserved name as the value.
 
    By default, this validator is applied to the username field of
    :class:`django_registration.forms.RegistrationForm` and all of its
-   subclasses. This validator is attached to the list of validators
-   for the username field, so to remove it (not recommended), subclass
+   subclasses. This validator is attached to the list of validators for the
+   username field, so to remove it (not recommended), subclass
    :class:`~django_registration.forms.RegistrationForm` and override
-   `__init__()` to change the set of validators on the username field.
+   ``__init__()`` to change the set of validators on the username field.
 
-   If you want to supply your own custom list of reserved names, you
-   can subclass :class:`~django_registration.forms.RegistrationForm`
-   and set the attribute `reserved_names` to the list of values you
-   want to disallow.
+   If you want to supply your own custom list of reserved names, you can
+   subclass :class:`~django_registration.forms.RegistrationForm` and set the
+   attribute ``reserved_names`` to the list of values you want to disallow.
 
    The default list of reserved names, if you don't specify one, is
    :data:`~django_registration.validators.DEFAULT_RESERVED_NAMES`. The
    validator will also reject any value beginning with the string
-   `".well-known"` (see `RFC 5785
-   <https://www.ietf.org/rfc/rfc5785.txt>`_).
+   ``".well-known"`` (see `RFC 5785 <https://www.ietf.org/rfc/rfc5785.txt>`_).
 
    :param list reserved_names: A list of reserved names to forbid.
    :raises django.core.exceptions.ValidationError: if the provided
       value is reserved.
 
 Several constants are provided which are used by this validator:
 
 .. data:: CA_ADDRESSES
 
-   A list of email usernames commonly used by certificate authorities
-   when verifying identity.
+   A list of email usernames commonly used by certificate authorities when
+   verifying identity.
 
 .. data:: NOREPLY_ADDRESSES
 
-   A list of common email usernames used for automated messages from a
-   Web site (such as "noreply" and "mailer-daemon").
+   A list of common email usernames used for automated messages from a Web site
+   (such as "noreply" and "mailer-daemon").
 
 .. data:: PROTOCOL_HOSTNAMES
 
-   A list of protocol-specific hostnames sites commonly want to
-   reserve, such as "www" and "mail".
+   A list of protocol-specific hostnames sites commonly want to reserve, such
+   as "www" and "mail".
 
 .. data:: OTHER_SENSITIVE_NAMES
 
-   Other names, not covered by any of the other lists, which have the
-   potential to conflict with common URLs or subdomains, such as
-   "blog" and "docs".
+   Other names, not covered by any of the other lists, which have the potential
+   to conflict with common URLs or subdomains, such as "blog" and "docs".
 
 .. data:: RFC_2142
 
    A list of common email usernames specified by `RFC 2142
    <https://www.ietf.org/rfc/rfc2142.txt>`_.
 
 .. data:: SENSITIVE_FILENAMES
 
-   A list of common filenames with important meanings, such that
-   usernames should not be allowed to conflict with them (such as
-   "favicon.ico" and "robots.txt").
+   A list of common filenames with important meanings, such that usernames
+   should not be allowed to conflict with them (such as "favicon.ico" and
+   "robots.txt").
 
 .. data:: SPECIAL_HOSTNAMES
 
-   A list of hostnames with reserved or special meaning (such as
-   "autoconfig", used by some email clients to automatically discover
-   configuration data for a domain).
+   A list of hostnames with reserved or special meaning (such as "autoconfig",
+   used by some email clients to automatically discover configuration data for
+   a domain).
 
 .. data:: DEFAULT_RESERVED_NAMES
 
-   A list made of the concatenation of all of the above lists, used as
-   the default set of reserved names for
+   A list made of the concatenation of all of the above lists, used as the
+   default set of reserved names for
    :class:`~django_registration.validators.ReservedNameValidator`.
 
 
 Protecting against homograph attacks
 ------------------------------------
 
-By default, Django permits a broad range of Unicode to be used in
-usernames; while this is useful for serving a worldwide audience, it
-also creates the possibility of `homograph attacks
-<https://en.wikipedia.org/wiki/IDN_homograph_attack>`_ through the use
-of characters which are easily visually confused for each other (for
-example: "pаypаl" containing a Cyrillic "а", visually
-indistinguishable in many fonts from a Latin "а").
+By default, Django permits a broad range of Unicode to be used in usernames;
+while this is useful for serving a worldwide audience, it also creates the
+possibility of `homograph attacks
+<https://en.wikipedia.org/wiki/IDN_homograph_attack>`_ through the use of
+characters which are easily visually confused for each other (for example:
+"pаypаl" containing a Cyrillic "а", visually indistinguishable in many fonts
+from a Latin "а").
 
-To protect against this, django-registration applies some validation
-rules to usernames and email addresses.
+To protect against this, django-registration applies some validation rules to
+usernames and email addresses.
 
 .. function:: validate_confusables(value)
 
-   A custom validator which prohibits the use of
-   dangerously-confusable usernames.
+   A custom validator which prohibits the use of dangerously-confusable
+   usernames.
 
-   This validator will reject any mixed-script value (as defined by
-   Unicode 'Script' property) which also contains one or more
-   characters that appear in the Unicode Visually Confusable
-   Characters file.
+   This validator will reject any mixed-script value (as defined by Unicode
+   'Script' property) which also contains one or more characters that appear in
+   the Unicode Visually Confusable Characters file.
 
-   This validator is enabled by default on the username field of
-   registration forms.
+   This validator is enabled by default on the username field of registration
+   forms.
 
    :param str value: The username value to validate (non-string
       usernames will not be checked)
    :raises django.core.exceptions.ValidationError: if the value is mixed-script confusable
 
 .. function:: validate_confusables_email(value)
 
-   A custom validator which prohibits the use of
-   dangerously-confusable email address.
+   A custom validator which prohibits the use of dangerously-confusable email
+   address.
 
-   This validator will reject any email address where either the
-   local-part of the domain is -- when considered in isolation --
-   dangerously confusable. A string is dangerously confusable if it is
-   a mixed-script value (as defined by Unicode 'Script' property)
-   which also contains one or more characters that appear in the
-   Unicode Visually Confusable Characters file.
+   This validator will reject any email address where either the local-part or
+   the domain is -- when considered in isolation -- dangerously confusable. A
+   string is dangerously confusable if it is a mixed-script value (as defined
+   by Unicode 'Script' property) which also contains one or more characters
+   that appear in the Unicode Visually Confusable Characters file.
 
-   This validator is enabled by default on the email field of
-   registration forms.
+   This validator is enabled by default on the email field of registration
+   forms.
 
    :param str value: The email address to validate
    :raises django.core.exceptions.ValidationError: if the value is mixed-script confusable
 
 
 Other validators
 ----------------
 
 .. class:: CaseInsensitiveUnique(model, field_name)
 
    A callable validator class (see `Django's validators documentation
-   <https://docs.djangoproject.com/en/stable/ref/validators/>`_) which
-   enforces case-insensitive uniqueness on a given field of a
-   particular model. Used by
-   :class:`~django_registration.forms.RegistrationFormCaseInsensitive`
-   for case-insensitive username uniqueness, and
-   :class:`~django_registration.forms.RegistrationFormUniqueEmail` for
-   unique email addresses.
+   <https://docs.djangoproject.com/en/stable/ref/validators/>`_) which enforces
+   case-insensitive uniqueness on a given field of a particular model. Used by
+   :class:`~django_registration.forms.RegistrationFormCaseInsensitive` for
+   case-insensitive username uniqueness, and
+   :class:`~django_registration.forms.RegistrationFormUniqueEmail` for unique
+   email addresses.
 
    :param django.db.models.Model model: The model class to query
       against for uniqueness checks.
    :param str field_name: The field name to perform the uniqueness
       check against.
    :raises django.core.exceptions.ValidationError: if the value is not
       unique.
 
 .. class:: HTML5EmailValidator
 
    A callable validator class (see `Django's validators documentation
-   <https://docs.djangoproject.com/en/stable/ref/validators/>`_) which
-   enforces the `HTML5 email address format
+   <https://docs.djangoproject.com/en/stable/ref/validators/>`_) which enforces
+   the `HTML5 email address format
    <https://html.spec.whatwg.org/multipage/input.html#e-mail-state-(type=email)>`_. The
-   format used by HTML5's `input type="email"` is deliberately more
-   restrictive than what is permitted by the latest email RFCs;
-   specifically, HTML5's validation rule disallows a number of rare
-   and problematic features -- such as embedded comments and
-   quoted-string inclusion of otherwise-illegal characters -- which
-   are technically legal to have in an email address but which now
-   mostly serve to confuse or complicate parsers, rather than to
-   provide actual utility.
+   format used by HTML5's ``input type="email"`` is deliberately more
+   restrictive than what is permitted by the latest email RFCs; specifically,
+   HTML5's validation rule disallows a number of rare and problematic features
+   -- such as embedded comments and quoted-string inclusion of
+   otherwise-illegal characters -- which are technically legal to have in an
+   email address but which now mostly serve to confuse or complicate parsers,
+   rather than to provide actual utility.
```

### Comparing `django-registration-3.3/docs/views.rst` & `django-registration-3.4/docs/views.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,161 +1,153 @@
 .. _views:
 .. module:: django_registration.views
 
 Base view classes
 =================
 
 In order to allow the utmost flexibility in customizing and supporting
-different workflows, django-registration makes use of Django's
-support for `class-based views
+different workflows, django-registration makes use of Django's support for
+`class-based views
 <https://docs.djangoproject.com/en/stable/topics/class-based-views/>`_. Included
-in django-registration are two base classes which can be
-subclassed to implement many types of registration workflows.
+in django-registration are two base classes which can be subclassed to
+implement many types of registration workflows.
 
-The built-in workflows in django-registration provide their own
-subclasses of these views, and the documentation for those workflows
-will indicate customization points specific to those subclasses. The
-following reference covers useful attributes and methods of the base
-classes, for use in writing your own custom registration workflows.
+The built-in workflows in django-registration provide their own subclasses of
+these views, and the documentation for those workflows will indicate
+customization points specific to those subclasses. The following reference
+covers useful attributes and methods of the base classes, for use in writing
+your own custom registration workflows.
 
 .. class:: RegistrationView
 
-   A subclass of Django's :class:`~django.views.generic.edit.FormView`
-   which provides the infrastructure for supporting user registration.
+   A subclass of Django's :class:`~django.views.generic.edit.FormView` which
+   provides the infrastructure for supporting user registration.
 
    Standard attributes and methods of
-   :class:`~django.views.generic.edit.FormView` can be overridden to
-   control behavior as described in Django's documentation, with the
-   exception of :meth:`get_success_url`, which must use the signature
-   documented below.
+   :class:`~django.views.generic.edit.FormView` can be overridden to control
+   behavior as described in Django's documentation, with the exception of
+   :meth:`get_success_url`, which must use the signature documented below.
 
    When writing your own subclass, one method is required:
 
    .. method:: register(form)
 
-      Implement your registration logic here. `form` will be the
-      (already-validated) form filled out by the user during the
-      registration process (i.e., a valid instance of
+      Implement your registration logic here. ``form`` will be the
+      (already-validated) form filled out by the user during the registration
+      process (i.e., a valid instance of
       :class:`~django_registration.forms.RegistrationForm` or a subclass of
       it).
 
-      This method should return the newly-registered user instance,
-      and should send the signal
-      :data:`django_registration.signals.user_registered`. Note that this is
-      not automatically done for you when writing your own custom
+      This method should return the newly-registered user instance, and should
+      send the signal :data:`django_registration.signals.user_registered`. Note
+      that this is not automatically done for you when writing your own custom
       subclass, so you must send this signal manually.
 
       :param django_registration.forms.RegistrationForm form: The registration form to use.
       :rtype: django.contrib.auth.models.AbstractUser
 
    Useful optional places to override or customize on subclasses are:
 
    .. attribute:: disallowed_url
 
       The URL to redirect to when registration is disallowed. Can be a
       hard-coded string, the string resulting from calling Django's
-      :func:`~django.urls.reverse` helper, or the lazy object produced
-      by Django's :func:`~django.urls.reverse_lazy` helper. Default
-      value is the result of calling :func:`~django.urls.reverse_lazy`
-      with the URL name `'registration_disallowed'`.
-      
+      :func:`~django.urls.reverse` helper, or the lazy object produced by
+      Django's :func:`~django.urls.reverse_lazy` helper. Default value is the
+      result of calling :func:`~django.urls.reverse_lazy` with the URL name
+      ``'registration_disallowed'``.
+
    .. attribute:: form_class
 
-      The form class to use for user registration. Can be overridden
-      on a per-request basis (see below). Should be the actual class
-      object; by default, this class is
+      The form class to use for user registration. Can be overridden on a
+      per-request basis (see below). Should be the actual class object; by
+      default, this class is
       :class:`django_registration.forms.RegistrationForm`.
 
    .. attribute:: success_url
 
-      The URL to redirect to after successful registration. Can be a
-      hard-coded string, the string resulting from calling Django's
-      :func:`~django.urls.reverse` helper, or the lazy object produced
-      by Django's :func:`~django.urls.reverse_lazy` helper. Can be
-      overridden on a per-request basis (see below). Default value is
-      `None`; subclasses must override and provide this.
+      The URL to redirect to after successful registration. Can be a hard-coded
+      string, the string resulting from calling Django's
+      :func:`~django.urls.reverse` helper, or the lazy object produced by
+      Django's :func:`~django.urls.reverse_lazy` helper. Can be overridden on a
+      per-request basis (see below). Default value is :data:`None`; subclasses
+      must override and provide this.
 
    .. attribute:: template_name
 
-      The template to use for user registration. Should be a
-      string. Default value is
-      `'django_registration/registration_form.html'`.
+      The template to use for user registration. Should be a string. Default
+      value is ``'django_registration/registration_form.html'``.
 
    .. method:: get_form_class()
 
-      Select a form class to use on a per-request basis. If not
-      overridden, will use :attr:`~form_class`. Should be the actual
-      class object.
+      Select a form class to use on a per-request basis. If not overridden,
+      will use :attr:`~form_class`. Should be the actual class object.
 
       :rtype: django_registration.forms.RegistrationForm
 
    .. method:: get_success_url(user)
 
       Return a URL to redirect to after successful registration, on a
       per-request or per-user basis. If not overridden, will use
       :attr:`~success_url`. Should return a value of the same type as
       :attr:`success_url` (see above).
-      
+
       :param django.contrib.auth.models.AbstractUser user: The new user account.
       :rtype: str
 
    .. method:: registration_allowed()
 
-      Should indicate whether user registration is allowed, either in
-      general or for this specific request. Default value is the value
-      of the setting :data:`~django.conf.settings.REGISTRATION_OPEN`.
+      Should indicate whether user registration is allowed, either in general
+      or for this specific request. Default value is the value of the setting
+      :data:`~django.conf.settings.REGISTRATION_OPEN`.
 
       :rtype: bool
 
 
 .. class:: ActivationView
 
-   A subclass of Django's
-   :class:`~django.views.generic.base.TemplateView` which provides
-   support for a separate account-activation step, in workflows which
-   require that.
+   A subclass of Django's :class:`~django.views.generic.base.TemplateView`
+   which provides support for a separate account-activation step, in workflows
+   which require that.
 
    One method is required:
 
    .. method:: activate(*args, **kwargs)
 
-      Implement your activation logic here. You are free to configure
-      your URL patterns to pass any set of positional or keyword
-      arguments to :class:`ActivationView`, and they will in turn be
-      passed to this method.
+      Implement your activation logic here. You are free to configure your URL
+      patterns to pass any set of positional or keyword arguments to
+      :class:`ActivationView`, and they will in turn be passed to this method.
 
       This method should return the newly-activated user instance (if
       activation was successful), or raise
-      :class:`~django_registration.exceptions.ActivationError` (if
-      activation was not successful).
+      :class:`~django_registration.exceptions.ActivationError` (if activation
+      was not successful).
 
       :rtype: django.contrib.auth.models.AbstractUser
       :raises django_registration.exceptions.ActivationError: if activation fails.
-      
+
    Useful places to override or customize on an
    :class:`ActivationView` subclass are:
 
    .. attribute:: success_url
 
-      The URL to redirect to after successful activation. Can be a
-      hard-coded string, the string resulting from calling Django's
-      :func:`~django.urls.reverse` helper, or the lazy object produced
-      by Django's :func:`~django.urls.reverse_lazy` helper. Can be
-      overridden on a per-request basis (see below). Default value is
-      `None`; subclasses must override and provide this.
+      The URL to redirect to after successful activation. Can be a hard-coded
+      string, the string resulting from calling Django's
+      :func:`~django.urls.reverse` helper, or the lazy object produced by
+      Django's :func:`~django.urls.reverse_lazy` helper. Can be overridden on a
+      per-request basis (see below). Default value is :data:`None`; subclasses
+      must override and provide this.
 
    .. attribute:: template_name
 
       The template to use after failed user activation. Should be a
-      string. Default value is
-      `'django_registration/activation_failed.html'`.
+      string. Default value is ``'django_registration/activation_failed.html'``.
 
    .. method:: get_success_url(user)
 
-      Return a URL to redirect to after successful activation, on a
-      per-request or per-user basis. If not overridden, will use
+      Return a URL to redirect to after successful activation, on a per-request
+      or per-user basis. If not overridden, will use
       :attr:`~success_url`. Should return a value of the same type as
       :attr:`success_url` (see above).
 
       :param django.contrib.auth.models.AbstractUser user: The activated user account.
       :rtype: str
-
```

### Comparing `django-registration-3.3/src/django_registration/backends/activation/urls.py` & `django-registration-3.4/src/django_registration/backends/activation/urls.py`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/backends/activation/views.py` & `django-registration-3.4/src/django_registration/backends/activation/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     """
 
     email_body_template = "django_registration/activation_email_body.txt"
     email_subject_template = "django_registration/activation_email_subject.txt"
     success_url = reverse_lazy("django_registration_complete")
 
     def register(self, form):
+        """
+        Register the new user account.
+
+        """
         new_user = self.create_inactive_user(form)
         signals.user_registered.send(
             sender=self.__class__, user=new_user, request=self.request
         )
         return new_user
 
     def create_inactive_user(self, form):
@@ -115,27 +119,32 @@
     )
     BAD_USERNAME_MESSAGE = _("The account you attempted to activate is invalid.")
     EXPIRED_MESSAGE = _("This account has expired.")
     INVALID_KEY_MESSAGE = _("The activation key you provided is invalid.")
     success_url = reverse_lazy("django_registration_activation_complete")
 
     def activate(self, *args, **kwargs):
+        """
+        Attempt to activate the user account.
+
+        """
         username = self.validate_key(kwargs.get("activation_key"))
         user = self.get_user(username)
         user.is_active = True
         user.save()
         return user
 
     def validate_key(self, activation_key):
         """
         Verify that the activation key is valid and within the
         permitted activation time window, returning the username if
         valid or raising ``ActivationError`` if not.
 
         """
+        # pylint: disable=raise-missing-from
         try:
             username = signing.loads(
                 activation_key,
                 salt=REGISTRATION_SALT,
                 max_age=settings.ACCOUNT_ACTIVATION_DAYS * 86400,
             )
             return username
@@ -151,14 +160,15 @@
     def get_user(self, username):
         """
         Given the verified username, look up and return the
         corresponding user account if it exists, or raising
         ``ActivationError`` if it doesn't.
 
         """
+        # pylint: disable=invalid-name,raise-missing-from
         User = get_user_model()
         try:
             user = User.objects.get(**{User.USERNAME_FIELD: username})
             if user.is_active:
                 raise ActivationError(
                     self.ALREADY_ACTIVATED_MESSAGE, code="already_activated"
                 )
```

### Comparing `django-registration-3.3/src/django_registration/backends/one_step/urls.py` & `django-registration-3.4/src/django_registration/backends/one_step/urls.py`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/backends/one_step/views.py` & `django-registration-3.4/src/django_registration/backends/one_step/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     useful account), and is immediately signed up and logged in.
 
     """
 
     success_url = reverse_lazy("django_registration_complete")
 
     def register(self, form):
+        """
+        Register the new user account and immediately log it in.
+
+        """
         new_user = form.save()
         new_user = authenticate(
             **{
                 User.USERNAME_FIELD: new_user.get_username(),
                 "password": form.cleaned_data["password1"],
             }
         )
```

### Comparing `django-registration-3.3/src/django_registration/forms.py` & `django-registration-3.4/src/django_registration/forms.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     Subclasses should feel free to add any additional validation they
     need, but should take care when overriding ``save()`` to respect
     the ``commit=False`` argument, as several registration workflows
     will make use of it to create inactive user accounts.
 
     """
 
+    # pylint: disable=too-few-public-methods
+
     class Meta(UserCreationForm.Meta):
         fields = [
             User.USERNAME_FIELD,
             User.get_email_field_name(),
             "password1",
             "password2",
         ]
@@ -52,17 +54,23 @@
         else:
             reserved_names = validators.DEFAULT_RESERVED_NAMES
         username_validators = [
             validators.ReservedNameValidator(reserved_names),
             validators.validate_confusables,
         ]
         self.fields[User.USERNAME_FIELD].validators.extend(username_validators)
-        self.fields[email_field].validators.extend(
-            (validators.HTML5EmailValidator(), validators.validate_confusables_email)
-        )
+        # django-registration's email validation is significantly stricter than Django's
+        # default email validation, which means that leaving Django's default validation
+        # on only causes confusion due to duplicate error messages (see GitHub issue
+        # #238). So we apply only the django-registration validators, not the default
+        # Django validator, on the email field.
+        self.fields[email_field].validators = [
+            validators.HTML5EmailValidator(),
+            validators.validate_confusables_email,
+        ]
         self.fields[email_field].required = True
 
 
 class RegistrationFormCaseInsensitive(RegistrationForm):
     """
     Subclass of ``RegistrationForm`` enforcing case-insensitive
     uniqueness of usernames.
```

### Comparing `django-registration-3.3/src/django_registration/locale/ar/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/ar/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/bg/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/bg/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/ca/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/ca/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/cs/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/cs/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/da/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/da/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/de/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/de/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/el/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/el/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/en/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/es/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/es/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/es_AR/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/es_AR/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/fa/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/fa/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/fr/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/fr/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/he/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/he/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/hr/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/hr/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/is/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/is/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/is/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/it/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/it/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/ja/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/ja/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/ko/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/ko/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/nb/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/nb/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/nl/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/nl/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/pl/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/pl/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/pt/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/pt/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/pt_BR/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/pt_BR/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/ru/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/ru/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/sl/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/sl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/sl/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/sr/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/sr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/sr/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/sv/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/sv/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/tr_TR/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/tr_TR/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/zh_CN/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/zh_CN/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/zh_TW/LC_MESSAGES/django.mo` & `django-registration-3.4/src/django_registration/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/locale/zh_TW/LC_MESSAGES/django.po` & `django-registration-3.4/src/django_registration/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-registration-3.3/src/django_registration/migrations/0001_initial.py` & `django-registration-3.4/src/django_registration/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+# pylint: disable=invalid-name
 from __future__ import unicode_literals
 
 from django.conf import settings
 from django.db import migrations
 
 # django-registration 2.x included a model-based signup workflow which
 # needed to create a model to store data. In django-registration 3.x,
@@ -11,13 +12,12 @@
 # To avoid breaking existing sites with migrations which had
 # dependencies on that migration, and ensure they can safely reverse
 # and replay migrations, this migration is preserved, but is now a
 # no-op.
 
 
 class Migration(migrations.Migration):
-
     dependencies = [migrations.swappable_dependency(settings.AUTH_USER_MODEL)]
 
     operations = [
         migrations.RunPython(migrations.RunPython.noop, migrations.RunPython.noop)
     ]
```

### Comparing `django-registration-3.3/src/django_registration/validators.py` & `django-registration-3.4/src/django_registration/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Error messages, data and custom validation code used in
 django-registration's various user-registration form classes.
 
 """
+# pylint: disable=implicit-str-concat
 import re
 import unicodedata
 
 from confusable_homoglyphs import confusables
 from django.core.exceptions import ValidationError
 from django.core.validators import EmailValidator, RegexValidator
 from django.utils.deconstruct import deconstructible
@@ -186,14 +187,15 @@
     "subscribe",
     "terms",
     "tos",
     "user",
     "users",
     "weblog",
     "work",
+    "xrpc",  # Used by Bluesky/AT protocol for domain verification.
 ]
 
 
 DEFAULT_RESERVED_NAMES = (
     SPECIAL_HOSTNAMES
     + PROTOCOL_HOSTNAMES
     + CA_ADDRESSES
@@ -241,15 +243,15 @@
 
     def __call__(self, value):
         # Only run if the username is a string.
         if not isinstance(value, str):
             return
         value = unicodedata.normalize("NFKC", value).casefold()
         if self.model._default_manager.filter(
-            **{"{}__iexact".format(self.field_name): value}
+            **{f"{self.field_name}__iexact": value}
         ).exists():
             raise ValidationError(self.error_message, code="unique")
 
     def __eq__(self, other):
         return (
             self.model == other.model
             and self.field_name == other.field_name
@@ -260,14 +262,16 @@
 @deconstructible
 class HTML5EmailValidator(RegexValidator):
     """
     Validator which applies HTML5's email address rules.
 
     """
 
+    # pylint: disable=too-few-public-methods
+
     message = EmailValidator.message
     regex = re.compile(HTML5_EMAIL_RE)
 
 
 def validate_confusables(value):
     """
     Validator which disallows 'dangerous' usernames likely to
```

### Comparing `django-registration-3.3/src/django_registration/views.py` & `django-registration-3.4/src/django_registration/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 
         Most often this will be the case because Django has been
         configured to use a custom user model, but the developer has
         forgotten to also configure an appropriate custom registration
         form to match it.
 
         """
+        # pylint: disable=protected-access
         if form_class is None:
             form_class = self.get_form_class()
         form_model = form_class._meta.model
         user_model = get_user_model()
         if form_model._meta.label != user_model._meta.label:
             raise ImproperlyConfigured(
                 USER_MODEL_MISMATCH.format(
@@ -79,26 +80,30 @@
                     form=form_class,
                     form_model=form_model,
                     user_model=user_model,
                 )
             )
         return form_class(**self.get_form_kwargs())
 
-    def get_success_url(self, user=None):
+    def get_success_url(self, user=None):  # pylint: disable=unused-argument
         """
         Return the URL to redirect to after successful redirection.
 
         """
         # This is overridden solely to allow django-registration to
         # support passing the user account as an argument; otherwise,
         # the base FormMixin implementation, which accepts no
         # arguments, could be called and end up raising a TypeError.
         return super().get_success_url()
 
     def form_valid(self, form):
+        """
+        After successful form processing, redirect to the success URL.
+
+        """
         return HttpResponseRedirect(self.get_success_url(self.register(form)))
 
     def registration_allowed(self):
         """
         Override this to enable/disable user registration, either
         globally or on a per-request basis.
 
@@ -119,15 +124,15 @@
     Base class for user activation views.
 
     """
 
     success_url = None
     template_name = "django_registration/activation_failed.html"
 
-    def get_success_url(self, user=None):
+    def get_success_url(self, user=None):  # pylint: disable=unused-argument
         """
         Return the URL to redirect to after successful redirection.
 
         """
         return force_str(self.success_url)
 
     def get(self, *args, **kwargs):
@@ -136,19 +141,19 @@
         alone and implement activate(), which is called from this
         method.
 
         """
         extra_context = {}
         try:
             activated_user = self.activate(*args, **kwargs)
-        except ActivationError as e:
+        except ActivationError as exc:
             extra_context["activation_error"] = {
-                "message": e.message,
-                "code": e.code,
-                "params": e.params,
+                "message": exc.message,
+                "code": exc.code,
+                "params": exc.params,
             }
         else:
             signals.user_activated.send(
                 sender=self.__class__, user=activated_user, request=self.request
             )
             return HttpResponseRedirect(force_str(self.get_success_url(activated_user)))
         context_data = self.get_context_data()
```

### Comparing `django-registration-3.3/src/django_registration.egg-info/PKG-INFO` & `django-registration-3.4/src/django_registration.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 Metadata-Version: 2.1
 Name: django-registration
-Version: 3.3
-Summary: An extensible user-registration application for Django
-Home-page: https://github.com/ubernostrum/django-registration/
-Author: James Bennett
-Author-email: james@b-list.org
+Version: 3.4
+Summary: An extensible user-registration application for Django.
+Author-email: James Bennett <james@b-list.org>
+License: BSD-3-Clause
+Project-URL: documentation, https://django-registration.readthedocs.io/
+Project-URL: homepage, https://github.com/ubernostrum/django-registration
+Keywords: django,security,auth,authentication
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: tests
 License-File: LICENSE
+License-File: AUTHORS
 
 .. -*-restructuredtext-*-
 
 .. image:: https://github.com/ubernostrum/django-registration/workflows/CI/badge.svg
    :alt: CI status image
    :target: https://github.com/ubernostrum/django-registration/actions?query=workflow%3ACI
```

### Comparing `django-registration-3.3/src/django_registration.egg-info/SOURCES.txt` & `django-registration-3.4/src/django_registration.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+.editorconfig
+.flake8
+.pre-commit-config.yaml
+.readthedocs.yaml
 AUTHORS
 LICENSE
 MANIFEST.in
 README.rst
+noxfile.py
+pyproject.toml
 runtests.py
-setup.cfg
-setup.py
-tox.ini
 docs/Makefile
 docs/activation-workflow.rst
 docs/conf.py
 docs/custom-user.rst
 docs/deprecations.rst
+docs/docs_settings.py
 docs/exceptions.rst
 docs/faq.rst
 docs/forms.rst
 docs/index.rst
 docs/install.rst
 docs/make.bat
 docs/one-step-workflow.rst
@@ -31,15 +35,14 @@
 src/django_registration/forms.py
 src/django_registration/signals.py
 src/django_registration/validators.py
 src/django_registration/views.py
 src/django_registration.egg-info/PKG-INFO
 src/django_registration.egg-info/SOURCES.txt
 src/django_registration.egg-info/dependency_links.txt
-src/django_registration.egg-info/not-zip-safe
 src/django_registration.egg-info/requires.txt
 src/django_registration.egg-info/top_level.txt
 src/django_registration/backends/__init__.py
 src/django_registration/backends/activation/__init__.py
 src/django_registration/backends/activation/urls.py
 src/django_registration/backends/activation/views.py
 src/django_registration/backends/one_step/__init__.py
@@ -69,14 +72,16 @@
 src/django_registration/locale/fa/LC_MESSAGES/django.po
 src/django_registration/locale/fr/LC_MESSAGES/django.mo
 src/django_registration/locale/fr/LC_MESSAGES/django.po
 src/django_registration/locale/he/LC_MESSAGES/django.mo
 src/django_registration/locale/he/LC_MESSAGES/django.po
 src/django_registration/locale/hr/LC_MESSAGES/django.mo
 src/django_registration/locale/hr/LC_MESSAGES/django.po
+src/django_registration/locale/id/LC_MESSAGES/django.mo
+src/django_registration/locale/id/LC_MESSAGES/django.po
 src/django_registration/locale/is/LC_MESSAGES/django.mo
 src/django_registration/locale/is/LC_MESSAGES/django.po
 src/django_registration/locale/it/LC_MESSAGES/django.mo
 src/django_registration/locale/it/LC_MESSAGES/django.po
 src/django_registration/locale/ja/LC_MESSAGES/django.mo
 src/django_registration/locale/ja/LC_MESSAGES/django.po
 src/django_registration/locale/ko/LC_MESSAGES/django.mo
@@ -106,14 +111,15 @@
 src/django_registration/locale/zh_TW/LC_MESSAGES/django.mo
 src/django_registration/locale/zh_TW/LC_MESSAGES/django.po
 src/django_registration/migrations/0001_initial.py
 src/django_registration/migrations/__init__.py
 tests/__init__.py
 tests/base.py
 tests/models.py
+tests/settings.py
 tests/test_activation_workflow.py
 tests/test_forms.py
 tests/test_one_step_workflow.py
 tests/test_views.py
 tests/views.py
 tests/migrations/0001_initial.py
 tests/migrations/__init__.py
```

### Comparing `django-registration-3.3/tests/base.py` & `django-registration-3.4/tests/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,34 +10,37 @@
 from django.test import TestCase, override_settings
 from django.urls import reverse
 
 from django_registration import signals
 from django_registration.forms import RegistrationForm
 
 
-# django-registration needs to test that signals are sent at
-# registration and activation. Django -- as of 2.1 -- does not have a
-# test assertion built in to test whether a signal was or was not
-# sent. The code below is from a pull request submitted upstream to
-# Django to add assertSignalSent and assertSignalNotSent assertions to
-# Django's base test case class, and will be removed once it's been
-# integrated into Django and django-registration is only supporting
-# versions of Django which include it.
 class _AssertSignalSentContext:
+    """
+    Context manager for asserting a signal was sent.
+
+    """
+
     def __init__(self, test_case, signal, required_kwargs=None):
         self.test_case = test_case
         self.signal = signal
         self.required_kwargs = required_kwargs
 
     def _listener(self, sender, **kwargs):
+        """
+        Listener function which will capture the sent signal.
+
+        """
+        # pylint: disable=attribute-defined-outside-init
         self.signal_sent = True
         self.received_kwargs = kwargs
         self.sender = sender
 
     def __enter__(self):
+        # pylint: disable=attribute-defined-outside-init
         self.signal_sent = False
         self.received_kwargs = {}
         self.sender = None
         self.signal.connect(self._listener)
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
@@ -48,58 +51,82 @@
         if self.required_kwargs is not None:
             missing_kwargs = []
             for k in self.required_kwargs:
                 if k not in self.received_kwargs:
                     missing_kwargs.append(k)
             if missing_kwargs:
                 self.test_case.fail(
-                    "Signal missing required arguments: "
-                    "%s" % ",".join(missing_kwargs)
+                    f"Signal missing required arguments: {','.join(missing_kwargs)}"
                 )
 
 
 class _AssertSignalNotSentContext(_AssertSignalSentContext):
+    """
+    Context manager for asserting a signal was not sent.
+
+    """
+
+    # pylint: disable=too-few-public-methods
+
     def __exit__(self, exc_type, exc_value, traceback):
         self.signal.disconnect(self._listener)
         if self.signal_sent:
             self.test_case.fail("Signal was unexpectedly sent.")
 
 
 @override_settings(ACCOUNT_ACTIVATION_DAYS=7, REGISTRATION_OPEN=True)
 class RegistrationTestCase(TestCase):
     """
     Base class for test cases, defining valid data for registering a
     user account and looking up the account after creation.
 
     """
 
+    # pylint: disable=invalid-name
+
     @property
     def valid_data(self):
+        """
+        Return a set of valid data for user registration.
+
+        """
         User = get_user_model()
         return {
             User.USERNAME_FIELD: "alice",
             "email": "alice@example.com",
             "password1": "swordfish",
             "password2": "swordfish",
         }
 
     @property
     def user_lookup_kwargs(self):
+        """
+        Return query arguments for querying the user registered by ``valid_data``.
+
+        """
         User = get_user_model()
         return {User.USERNAME_FIELD: "alice"}
 
     @contextmanager
     def assertSignalSent(self, signal, required_kwargs=None):
-        with _AssertSignalSentContext(self, signal, required_kwargs) as cm:
-            yield cm
+        """
+        Assert a signal was sent.
+
+        """
+        with _AssertSignalSentContext(self, signal, required_kwargs) as signal_context:
+            yield signal_context
 
     @contextmanager
     def assertSignalNotSent(self, signal):
-        with _AssertSignalNotSentContext(self, signal) as cm:
-            yield cm
+        """
+        Assert a signal was not sent.
+
+        """
+        with _AssertSignalNotSentContext(self, signal) as signal_context:
+            yield signal_context
 
 
 class WorkflowTestCase(RegistrationTestCase):
     """
     Base class for the test cases which exercise the built-in
     workflows, including logic common to all of them (and which needs
     to be tested for each one).
@@ -108,15 +135,15 @@
 
     def test_registration_open(self):
         """
         ``REGISTRATION_OPEN``, when ``True``, permits registration.
 
         """
         resp = self.client.get(reverse("django_registration_register"))
-        self.assertEqual(200, resp.status_code)
+        assert resp.status_code == 200
 
     @override_settings(REGISTRATION_OPEN=False)
     def test_registration_closed(self):
         """
         ``REGISTRATION_OPEN``, when ``False``, disallows registration.
 
         """
@@ -131,17 +158,17 @@
     def test_registration_get(self):
         """
         HTTP ``GET`` to the registration view uses the appropriate
         template and populates a registration form into the context.
 
         """
         resp = self.client.get(reverse("django_registration_register"))
-        self.assertEqual(200, resp.status_code)
+        assert resp.status_code == 200
         self.assertTemplateUsed(resp, "django_registration/registration_form.html")
-        self.assertTrue(isinstance(resp.context["form"], RegistrationForm))
+        assert isinstance(resp.context["form"], RegistrationForm)
 
     def test_registration(self):
         """
         Registration creates a new account.
 
         """
         with self.assertSignalSent(signals.user_registered):
@@ -150,43 +177,48 @@
             )
 
         self.assertRedirects(resp, reverse("django_registration_complete"))
 
         user_model = get_user_model()
         new_user = user_model.objects.get(**self.user_lookup_kwargs)
 
-        self.assertTrue(new_user.check_password(self.valid_data["password1"]))
-        self.assertEqual(new_user.email, self.valid_data["email"])
+        assert new_user.check_password(self.valid_data["password1"])
+        assert new_user.email == self.valid_data["email"]
 
     def test_registration_failure(self):
         """
         Registering with invalid data fails.
 
         """
         data = self.valid_data.copy()
         data.update(password2="notsecret")
 
         with self.assertSignalNotSent(signals.user_registered):
             resp = self.client.post(reverse("django_registration_register"), data=data)
 
-        self.assertEqual(200, resp.status_code)
-        self.assertFalse(resp.context["form"].is_valid())
-        self.assertTrue(resp.context["form"].has_error("password2"))
+        assert resp.status_code == 200
+        assert not resp.context["form"].is_valid()
+        assert resp.context["form"].has_error("password2")
 
     def test_registration_signal(self):
+        """
+        Registering a new user account sends the registration signal.
+
+        """
+        # pylint: disable=invalid-name
         User = get_user_model()
-        with self.assertSignalSent(signals.user_registered) as cm:
+        with self.assertSignalSent(signals.user_registered) as signal_context:
             self.client.post(
                 reverse("django_registration_register"), data=self.valid_data
             )
-            self.assertEqual(
-                cm.received_kwargs["user"].get_username(),
-                self.valid_data[User.USERNAME_FIELD],
+            assert (
+                signal_context.received_kwargs["user"].get_username()
+                == self.valid_data[User.USERNAME_FIELD]
             )
-            self.assertTrue(isinstance(cm.received_kwargs["request"], HttpRequest))
+            assert isinstance(signal_context.received_kwargs["request"], HttpRequest)
 
 
 class ActivationTestCase(WorkflowTestCase):
     """
     Base class for testing the built-in workflows which involve an
     activation step.
 
@@ -203,44 +235,44 @@
         with self.assertSignalSent(signals.user_registered):
             super().test_registration()
 
         user_model = get_user_model()
         new_user = user_model.objects.get(**self.user_lookup_kwargs)
 
         # New user must not be active.
-        self.assertFalse(new_user.is_active)
+        assert not new_user.is_active
 
         # An activation email was sent.
-        self.assertEqual(len(mail.outbox), 1)
-        self.assertTrue("http" in mail.outbox[0].subject)
+        assert len(mail.outbox) == 1
+        assert "http" in mail.outbox[0].subject
 
     def test_registration_failure(self):
         """
         Registering with invalid data fails.
 
         """
         with self.assertSignalNotSent(signals.user_registered):
             super().test_registration_failure()
 
         # Activation email was not sent.
-        self.assertEqual(0, len(mail.outbox))
+        assert 0 == len(mail.outbox)
 
     def test_registration_no_sites(self):
         """
         Registration still functions properly when
         ``django.contrib.sites`` is not installed; the fallback will
         be a ``RequestSite`` instance.
 
         """
         with self.modify_settings(INSTALLED_APPS={"remove": ["django.contrib.sites"]}):
             with self.assertSignalSent(signals.user_registered):
                 resp = self.client.post(
                     reverse("django_registration_register"), data=self.valid_data
                 )
 
-            self.assertEqual(302, resp.status_code)
+            assert 302 == resp.status_code
 
             user_model = get_user_model()
             new_user = user_model.objects.get(**self.user_lookup_kwargs)
 
-            self.assertTrue(new_user.check_password(self.valid_data["password1"]))
-            self.assertEqual(new_user.email, self.valid_data["email"])
+            assert new_user.check_password(self.valid_data["password1"])
+            assert new_user.email == self.valid_data["email"]
```

### Comparing `django-registration-3.3/tests/migrations/0001_initial.py` & `django-registration-3.4/tests/migrations/0001_initial.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Generated by Django 3.0.1 on 2020-01-05 01:03
+# pylint: disable=invalid-name
 
 import django.contrib.auth.models
 import django.contrib.auth.validators
 import django.utils.timezone
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []  # type: list
 
     operations = [
         migrations.CreateModel(
             name="CustomUser",
```

### Comparing `django-registration-3.3/tests/models.py` & `django-registration-3.4/tests/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Custom user model for use in tests.
+
+"""
 from django.contrib.auth.base_user import AbstractBaseUser
 from django.contrib.auth.models import UserManager
 from django.contrib.auth.validators import UnicodeUsernameValidator
 from django.core.mail import send_mail
 from django.db import models
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
@@ -41,9 +45,12 @@
         help_text=_("Whether this user should be treated as active."),
     )
     date_joined = models.DateTimeField(_("date joined"), default=timezone.now)
 
     objects = UserManager()
 
     def email_user(self, subject, message, from_email=None, **kwargs):
-        """Send an email to this user."""
+        """
+        Send an email to this user.
+
+        """
         send_mail(subject, message, from_email, [self.email], **kwargs)
```

### Comparing `django-registration-3.3/tests/test_activation_workflow.py` & `django-registration-3.4/tests/test_activation_workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,24 +90,21 @@
                     "django_registration_activate",
                     args=(),
                     kwargs={"activation_key": activation_key},
                 )
             )
 
         # Second activation fails.
-        self.assertEqual(200, resp.status_code)
+        assert 200 == resp.status_code
         self.assertTemplateUsed(resp, "django_registration/activation_failed.html")
-        self.assertEqual(
-            resp.context["activation_error"],
-            {
-                "message": ActivationView.ALREADY_ACTIVATED_MESSAGE,
-                "code": "already_activated",
-                "params": None,
-            },
-        )
+        assert resp.context["activation_error"] == {
+            "message": ActivationView.ALREADY_ACTIVATED_MESSAGE,
+            "code": "already_activated",
+            "params": None,
+        }
 
     def test_bad_key(self):
         """
         An invalid activation key fails to activate.
 
         """
         user_model = get_user_model()
@@ -123,25 +120,22 @@
                     "django_registration_activate",
                     args=(),
                     kwargs={"activation_key": activation_key},
                 )
             )
 
         # Second activation fails.
-        self.assertEqual(200, resp.status_code)
+        assert 200 == resp.status_code
         self.assertTemplateUsed(resp, "django_registration/activation_failed.html")
-        self.assertTrue("activation_error" in resp.context)
-        self.assertEqual(
-            resp.context["activation_error"],
-            {
-                "message": ActivationView.INVALID_KEY_MESSAGE,
-                "code": "invalid_key",
-                "params": {"activation_key": activation_key},
-            },
-        )
+        assert "activation_error" in resp.context
+        assert resp.context["activation_error"] == {
+            "message": ActivationView.INVALID_KEY_MESSAGE,
+            "code": "invalid_key",
+            "params": {"activation_key": activation_key},
+        }
 
     # The timestamp calculation will error if USE_TZ=True, due to
     # trying to subtract a naive from an aware datetime. Since time
     # zones aren't relevant to the test, we just temporarily disable
     # time-zone support rather than do the more complex dance of
     # checking the setting and forcing everything to naive or aware.
     @override_settings(USE_TZ=False)
@@ -188,25 +182,22 @@
                 reverse(
                     "django_registration_activate",
                     args=(),
                     kwargs={"activation_key": activation_key},
                 )
             )
 
-        self.assertEqual(200, resp.status_code)
+        assert 200 == resp.status_code
         self.assertTemplateUsed(resp, "django_registration/activation_failed.html")
-        self.assertTrue("activation_error" in resp.context)
-        self.assertEqual(
-            resp.context["activation_error"],
-            {
-                "message": ActivationView.EXPIRED_MESSAGE,
-                "code": "expired",
-                "params": None,
-            },
-        )
+        assert "activation_error" in resp.context
+        assert resp.context["activation_error"] == {
+            "message": ActivationView.EXPIRED_MESSAGE,
+            "code": "expired",
+            "params": None,
+        }
 
     def test_nonexistent_activation(self):
         """
         A nonexistent username in an activation key will fail to
         activate.
 
         """
@@ -217,50 +208,51 @@
                 reverse(
                     "django_registration_activate",
                     args=(),
                     kwargs={"activation_key": activation_key},
                 )
             )
 
-        self.assertEqual(200, resp.status_code)
+        assert 200 == resp.status_code
         self.assertTemplateUsed(resp, "django_registration/activation_failed.html")
-        self.assertTrue("activation_error" in resp.context)
-        self.assertEqual(
-            resp.context["activation_error"],
-            {
-                "message": ActivationView.BAD_USERNAME_MESSAGE,
-                "code": "bad_username",
-                "params": None,
-            },
-        )
+        assert "activation_error" in resp.context
+        assert resp.context["activation_error"] == {
+            "message": ActivationView.BAD_USERNAME_MESSAGE,
+            "code": "bad_username",
+            "params": None,
+        }
 
     def test_activation_signal(self):
+        """
+        Activating a user account sends the activation signal.
+
+        """
         user_model = get_user_model()
 
         self.client.post(reverse("django_registration_register"), data=self.valid_data)
 
         activation_key = signing.dumps(
             obj=self.valid_data[user_model.USERNAME_FIELD], salt=REGISTRATION_SALT
         )
 
         with self.assertSignalSent(
             signals.user_activated, required_kwargs=["user", "request"]
-        ) as cm:
+        ) as signal_context:
             self.client.get(
                 reverse(
                     "django_registration_activate",
                     args=(),
                     kwargs={"activation_key": activation_key},
                 )
             )
-            self.assertEqual(
-                cm.received_kwargs["user"].get_username(),
-                self.valid_data[user_model.USERNAME_FIELD],
+            assert (
+                signal_context.received_kwargs["user"].get_username()
+                == self.valid_data[user_model.USERNAME_FIELD]
             )
-            self.assertTrue(isinstance(cm.received_kwargs["request"], HttpRequest))
+            assert isinstance(signal_context.received_kwargs["request"], HttpRequest)
 
 
 @override_settings(AUTH_USER_MODEL="tests.CustomUser")
 @override_settings(ROOT_URLCONF="tests.urls.custom_user_activation")
 class ActivationBackendCustomUserTests(ActivationBackendViewTests):
     """
     Runs the activation workflow's test suite, but with a custom user model.
```

### Comparing `django-registration-3.3/tests/test_forms.py` & `django-registration-3.4/tests/test_forms.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Exercise django-registration's built-in form classes.
 
 """
+
 import uuid
 
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ValidationError
 from django.test import modify_settings
 
 from django_registration import forms, validators
@@ -23,190 +24,204 @@
 
     def test_email_required(self):
         """
         The email address field is required.
 
         """
         form = forms.RegistrationForm()
-        self.assertTrue(form.fields["email"].required)
+        assert form.fields["email"].required
 
     def test_email_validation(self):
         """
         Stricter-than-RFC email validation is applied.
 
-        This test is necessary because of the combination of
-        HTML5EmailValidator and validate_confusables_email() in the
-        default validator set for the email field of RegistrationForm;
-        some technically-valid email addresses which nonetheless
-        usually indicate bad faith or at least mischief are to be
-        rejected before the confusables validator is applied.
+        This test is necessary because of the combination of HTML5EmailValidator and
+        validate_confusables_email() in the default validator set for the email field of
+        RegistrationForm; some technically-valid email addresses which nonetheless
+        usually indicate bad faith or at least mischief are to be rejected before the
+        confusables validator is applied.
 
         """
         user_model = get_user_model()
 
         for value in (
             "test@example.com",
             "test+test@example.com",
             "test.test@example.com",
             "test_test@example.com",
         ):
             user_data = self.valid_data.copy()
             user_data["email"] = value
             form = forms.RegistrationForm(data=user_data)
-            self.assertTrue(form.is_valid())
+            assert form.is_valid()
         for value in (
             "@@@example.com",
             "test:test@test@example.com",
             'test"test@example"test@example.com',
         ):
             user_data = self.valid_data.copy()
             user_data["email"] = value
             form = forms.RegistrationForm(data=user_data)
-            self.assertFalse(form.is_valid())
-            self.assertTrue(form.has_error(user_model.get_email_field_name()))
-            self.assertTrue(
+            assert not form.is_valid()
+            assert form.has_error(user_model.get_email_field_name())
+            assert (
                 str(validators.HTML5EmailValidator.message)
                 in form.errors[user_model.get_email_field_name()]
             )
 
+    def test_email_validated_once(self):
+        """
+        GitHub issue #238: Django's default email validator (and its error message)
+        should not be applied to the email field of the registration form, since our
+        validators are stricter and use the same message (which can cause confusing
+        duplicate errors).
+
+        """
+        user_model = get_user_model()
+        user_data = self.valid_data.copy()
+        user_data["email"] = "invalid_email"
+        form = forms.RegistrationForm(data=user_data)
+        email_field = user_model.get_email_field_name()
+        assert len(form.errors[email_field]) == 1
+
     def test_username_uniqueness(self):
         """
         Username uniqueness is enforced.
 
-        This test is necessary as of 2.1.x to ensure the base
-        UserCreationForm clean() continues to be called from the
-        overridden clean() in RegistrationForm.
+        This test is necessary as of 2.1.x to ensure the base UserCreationForm clean()
+        continues to be called from the overridden clean() in RegistrationForm.
 
         """
         user_data = self.valid_data.copy()
         del user_data["password1"]
         del user_data["password2"]
-        user_data["password"] = "swordfish"
+        user_data["password"] = "swordfish"  # nosec: B105
         user_model = get_user_model()
         existing_user = user_model(**user_data)
         existing_user.save()
         form = forms.RegistrationForm(data=self.valid_data.copy())
-        self.assertFalse(form.is_valid())
-        self.assertTrue(form.has_error(user_model.USERNAME_FIELD))
+        assert not form.is_valid()
+        assert form.has_error(user_model.USERNAME_FIELD)
 
     def test_reserved_names(self):
         """
         Reserved names are disallowed.
 
         """
         user_model = get_user_model()
         for reserved_name in validators.DEFAULT_RESERVED_NAMES:
             data = self.valid_data.copy()
             data[user_model.USERNAME_FIELD] = reserved_name
             form = forms.RegistrationForm(data=data)
-            self.assertFalse(form.is_valid())
-            self.assertTrue(form.has_error(user_model.USERNAME_FIELD))
-            self.assertTrue(
+            assert not form.is_valid()
+            assert form.has_error(user_model.USERNAME_FIELD)
+            assert (
                 str(validators.RESERVED_NAME) in form.errors[user_model.USERNAME_FIELD]
             )
 
     def test_confusable_usernames(self):
         """
-        Usernames containing dangerously confusable use of Unicode are
-        disallowed.
+        Usernames containing dangerously confusable use of Unicode are disallowed.
 
         """
         user_model = get_user_model()
         for dangerous_value in (
             "p\u0430yp\u0430l",
             "g\u043e\u043egle",
             "\u03c1ay\u03c1al",
         ):
             data = self.valid_data.copy()
             data[user_model.USERNAME_FIELD] = dangerous_value
             form = forms.RegistrationForm(data=data)
-            self.assertFalse(form.is_valid())
-            self.assertTrue(form.has_error(user_model.USERNAME_FIELD))
-            self.assertTrue(
-                str(validators.CONFUSABLE) in form.errors[user_model.USERNAME_FIELD]
-            )
+            assert not form.is_valid()
+            assert form.has_error(user_model.USERNAME_FIELD)
+            assert str(validators.CONFUSABLE) in form.errors[user_model.USERNAME_FIELD]
 
     def test_confusable_emails(self):
         """
-        Usernames containing dangerously confusable use of Unicode are
-        disallowed.
+        Usernames containing dangerously confusable use of Unicode are disallowed.
 
         """
         for dangerous_value in (
             "p\u0430yp\u0430l@example.com",
             "g\u043e\u043egle@example.com",
             "\u03c1y\u03c1al@example.com",
             "paypal@ex\u0430mple.com",
             "google@exam\u03c1le.com",
         ):
             data = self.valid_data.copy()
             data["email"] = dangerous_value
             form = forms.RegistrationForm(data=data)
-            self.assertFalse(form.is_valid())
-            self.assertTrue(form.has_error("email"))
-            self.assertTrue(str(validators.CONFUSABLE_EMAIL) in form.errors["email"])
+            assert not form.is_valid()
+            assert form.has_error("email")
+            assert str(validators.CONFUSABLE_EMAIL) in form.errors["email"]
 
     def test_custom_reserved_names(self):
         """
         Reserved names can be overridden by an attribute.
 
         """
         custom_reserved_names = ["foo", "bar", "eggs", "spam"]
 
         class CustomReservedNamesForm(forms.RegistrationForm):
+            """
+            Registration form with custom reserved-names list.
+
+            """
+
             reserved_names = custom_reserved_names
 
         user_model = get_user_model()
         for reserved_name in custom_reserved_names:
             data = self.valid_data.copy()
             data[user_model.USERNAME_FIELD] = reserved_name
             form = CustomReservedNamesForm(data=data)
-            self.assertFalse(form.is_valid())
-            self.assertTrue(form.has_error(user_model.USERNAME_FIELD))
-            self.assertTrue(
+            assert not form.is_valid()
+            assert form.has_error(user_model.USERNAME_FIELD)
+            assert (
                 str(validators.RESERVED_NAME) in form.errors[user_model.USERNAME_FIELD]
             )
 
     def test_reserved_name_non_string(self):
         """
-        GitHub issue #82: reserved-name validator should not attempt
-        to validate a non-string 'username'.
+        GitHub issue #82: reserved-name validator should not attempt to validate a
+        non-string 'username'.
 
         """
         validator = validators.ReservedNameValidator()
         for value in (123456, 1.7, uuid.uuid4()):
-            self.assertTrue(validator(value) is None)
+            assert validator(value) is None
 
     def test_reserved_name_validator_eq(self):
         """
-        Test ReservedNameValidator __eq__ method.
-        __eq__ is necessary for serializing custom user models that use
-        the validator.
+        Test ReservedNameValidator's __eq__() method.
+
+        __eq__() is necessary for serializing custom user models that use the validator.
 
         """
         validator = validators.ReservedNameValidator()
         validator_same = validators.ReservedNameValidator()
-        self.assertTrue(validator.__eq__(validator_same))
+        assert validator == validator_same
 
         validator_different = validators.ReservedNameValidator(reserved_names=[])
-        self.assertFalse(validator.__eq__(validator_different))
+        assert validator != validator_different
 
     def test_email_validator(self):
         """
         Test the HTMl5 email address validator.
 
         """
         validator = validators.HTML5EmailValidator()
         for value in (
             "test@example.com",
             "test+test@example.com",
             "test.test@example.com",
             "test_test@example.com",
         ):
-            self.assertTrue(validator(value) is None)
+            assert validator(value) is None
         for value in (
             "@@@example.com",
             "test:test@test@example.com",
             'test"test@example"test@example.com',
         ):
             with self.assertRaisesMessage(ValidationError, str(validator.message)):
                 validator(value)
@@ -219,15 +234,15 @@
         user_model = get_user_model()
         validator = validators.CaseInsensitiveUnique(
             user_model,
             user_model.USERNAME_FIELD,
             validators.DUPLICATE_USERNAME,
         )
         for value in (123456, 1.7, uuid.uuid4()):
-            self.assertTrue(validator(value) is None)
+            assert validator(value) is None
 
         base_creation_data = self.valid_data.copy()
         base_creation_data["password"] = base_creation_data["password1"]
         del base_creation_data["password1"]
         del base_creation_data["password2"]
 
         test_names = [("alice", "ALICE"), ("ALICE", "alice"), ("Alice", "alice")]
@@ -242,36 +257,36 @@
                 ValidationError, str(validators.DUPLICATE_USERNAME)
             ):
                 validator(conflict)
             existing_user.delete()
 
     def test_case_insensitive_validator_eq(self):
         """
-        Test CaseInsensitiveUnique __eq__ method.
-        __eq__ is necessary for serializing custom user models that use
-        the validator.
+        Test CaseInsensitiveUnique's __eq__() method.
+
+        __eq__() is necessary for serializing custom user models that use the validator.
 
         """
         user_model = get_user_model()
         validator = validators.CaseInsensitiveUnique(
             user_model,
             user_model.USERNAME_FIELD,
             validators.DUPLICATE_USERNAME,
         )
         validator_same = validators.CaseInsensitiveUnique(
             user_model,
             user_model.USERNAME_FIELD,
             validators.DUPLICATE_USERNAME,
         )
-        self.assertTrue(validator.__eq__(validator_same))
+        assert validator == validator_same
 
         validator_different = validators.CaseInsensitiveUnique(
             user_model, "not username field", validators.DUPLICATE_USERNAME
         )
-        self.assertFalse(validator.__eq__(validator_different))
+        assert validator != validator_different
 
     def test_case_insensitive_form(self):
         """
         Test the case-insensitive registration form.
 
         """
         base_creation_data = self.valid_data.copy()
@@ -285,62 +300,60 @@
             ("Alice", "alice"),
             ("AlIcE", "aLiCe"),
             ("STRASSBURGER", "straßburger"),
         ]
 
         user_model = get_user_model()
 
-        for name, conflict in test_names:
+        for name, _conflict in test_names:
             creation_data = base_creation_data.copy()
             creation_data[user_model.USERNAME_FIELD] = name
             existing_user = user_model(**creation_data)
             existing_user.save()
             user_data = self.valid_data.copy()
             user_data[user_model.USERNAME_FIELD] = name
             form = forms.RegistrationFormCaseInsensitive(data=user_data)
-            self.assertFalse(form.is_valid())
-            self.assertTrue(form.has_error(user_model.USERNAME_FIELD))
-            self.assertEqual(
-                [str(validators.DUPLICATE_USERNAME)],
-                form.errors[user_model.USERNAME_FIELD],
-            )
-            self.assertEqual(1, len(form.errors[user_model.USERNAME_FIELD]))
+            assert not form.is_valid()
+            assert form.has_error(user_model.USERNAME_FIELD)
+            assert [str(validators.DUPLICATE_USERNAME)] == form.errors[
+                user_model.USERNAME_FIELD
+            ]
+            assert 1 == len(form.errors[user_model.USERNAME_FIELD])
 
     def test_tos_field(self):
         """
-        The terms-of-service field on RegistrationFormTermsOfService
-        is required.
+        The terms-of-service field on RegistrationFormTermsOfService is required.
 
         """
         form = forms.RegistrationFormTermsOfService(data=self.valid_data.copy())
-        self.assertFalse(form.is_valid())
-        self.assertTrue(form.has_error("tos"))
-        self.assertEqual(form.errors["tos"], [str(validators.TOS_REQUIRED)])
+        assert not form.is_valid()
+        assert form.has_error("tos")
+        assert form.errors["tos"] == [str(validators.TOS_REQUIRED)]
 
     def test_email_uniqueness(self):
         """
         Email uniqueness is enforced by RegistrationFormUniqueEmail.
 
         """
         user_model = get_user_model()
         user_model.objects.create(
             username="bob",
             email=self.valid_data["email"],
             password=self.valid_data["password1"],
         )
 
         form = forms.RegistrationFormUniqueEmail(data=self.valid_data.copy())
-        self.assertFalse(form.is_valid())
-        self.assertTrue(form.has_error("email"))
-        self.assertEqual(form.errors["email"], [str(validators.DUPLICATE_EMAIL)])
+        assert not form.is_valid()
+        assert form.has_error("email")
+        assert form.errors["email"] != [str(validators.DUPLICATE_EMAIL)]
 
         data = self.valid_data.copy()
         data.update(email="bob@example.com")
         form = forms.RegistrationFormUniqueEmail(data=data)
-        self.assertTrue(form.is_valid())
+        assert form.is_valid()
 
     def test_confusables_validator(self):
         """
         Test the confusable-username validator standalone.
 
         """
         for dangerous_value in (
```

### Comparing `django-registration-3.3/tests/test_views.py` & `django-registration-3.4/tests/test_views.py`

 * *Files 17% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     def test_user_mismatch_breaks_view(self):
         """
         When RegistrationView detects a mismatch between the model used by
         its form class and the configured user model, it raises
         ImproperlyConfigured.
 
         """
+        # pylint: disable=no-member,protected-access
         for view_class in (
             base_views.RegistrationView,
             activation_views.RegistrationView,
             one_step_views.RegistrationView,
         ):
             for form_class in (
                 forms.RegistrationForm,
@@ -102,15 +103,22 @@
 
 class BuggyRegistrationView(base_views.RegistrationView):
     """
     Registration view that simulates an unhandled exception.
 
     """
 
+    # pylint: disable=abstract-method
+
     def registration_allowed(self):
+        """
+        Raise an exception as early as possible, when django-registration is checking
+        if registration will even be allowed.
+
+        """
         raise RegistrationError("catch me if you can")
 
 
 buggy_view = BuggyRegistrationView.as_view()
 
 
 @override_settings(ADMINS=[("Admin", "admin@localhost")])
@@ -134,25 +142,31 @@
         request = self.factory.post("/raise/", data=self.valid_data)
         request.user = AnonymousUser()
         # we cannot use self.assertRaises(...) here because of sys.exc_info()
         try:
             buggy_view(request)
             self.fail("expected exception not thrown")
         except RegistrationError as error:
-            self.assertEqual(str(error), "catch me if you can")
+            assert str(error) == "catch me if you can"
             # based on code in Django (tests/view_tests/views.py)
             self.logger.error(
-                "Internal Server Error: %s" % request.path,
+                f"Internal Server Error: {request.path}",
                 exc_info=sys.exc_info(),
                 extra={"status_code": 500, "request": request},
             )
-        self.assertEqual(len(mail.outbox), 1)
+        assert len(mail.outbox) == 1
         email = mail.outbox[0]
-        self.assertIn("RegistrationError at /raise/", email.body)
-        self.assertIn("catch me if you can", email.body)
-        self.assertIn("No GET data", email.body)
-        self.assertNotIn("No POST data", email.body)
-        self.assertIn("password1", email.body)
-        self.assertIn("password2", email.body)
-        self.assertNotIn(self.valid_data["password1"], email.body)
-        self.assertNotIn(self.valid_data["password2"], email.body)
-        self.assertNotIn(self.valid_data["email"], email.body)
+        for expected_string in (
+            "RegistrationError at /raise/",
+            "catch me if you can",
+            "No GET data",
+            "password1",
+            "password2",
+        ):
+            assert expected_string in email.body
+        for unexpected_string in (
+            "No POST data",
+            self.valid_data["password1"],
+            self.valid_data["password2"],
+            self.valid_data["email"],
+        ):
+            assert unexpected_string not in email.body
```

### Comparing `django-registration-3.3/tests/urls/custom_user_activation.py` & `django-registration-3.4/tests/urls/custom_user_activation.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 from django_registration.backends.activation import views
 from django_registration.forms import RegistrationForm
 
 from ..models import CustomUser
 
 
 class CustomUserRegistrationForm(RegistrationForm):
+    """
+    Registration form for the custom user model.
+
+    """
+
+    # pylint: disable=too-few-public-methods
+
     class Meta(RegistrationForm.Meta):
         model = CustomUser
 
 
 urlpatterns = [
     path(
         "activate/complete/",
```

### Comparing `django-registration-3.3/tests/urls/custom_user_one_step.py` & `django-registration-3.4/tests/urls/custom_user_one_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 from django_registration.backends.one_step import views
 from django_registration.forms import RegistrationForm
 
 from ..models import CustomUser
 
 
 class CustomUserRegistrationForm(RegistrationForm):
+    """
+    Registration form for the custom user model.
+
+    """
+
+    # pylint: disable=too-few-public-methods
+
     class Meta(RegistrationForm.Meta):
         model = CustomUser
 
 
 urlpatterns = [
     path(
         "register/",
```

### Comparing `django-registration-3.3/tests/urls/view_tests.py` & `django-registration-3.4/tests/urls/view_tests.py`

 * *Files identical despite different names*

