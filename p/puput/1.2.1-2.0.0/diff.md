# Comparing `tmp/puput-1.2.1.tar.gz` & `tmp/puput-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puput-1.2.1.tar", last modified: Tue May 16 15:37:39 2023, max compression
+gzip compressed data, was "puput-2.0.0.tar", last modified: Tue Jul  4 07:28:01 2023, max compression
```

## Comparing `puput-1.2.1.tar` & `puput-2.0.0.tar`

### file list

```diff
@@ -1,149 +1,150 @@
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.241129 puput-1.2.1/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      256 2023-05-11 13:28:16.000000 puput-1.2.1/AUTHORS
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     1063 2022-12-21 15:02:58.000000 puput-1.2.1/LICENSE
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      264 2022-12-21 15:02:58.000000 puput-1.2.1/MANIFEST.in
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3754 2023-05-16 15:37:39.241129 puput-1.2.1/PKG-INFO
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     2818 2023-05-15 15:26:50.000000 puput-1.2.1/README.rst
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.221129 puput-1.2.1/puput/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      673 2023-05-16 15:34:27.000000 puput-1.2.1/puput/__init__.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     5750 2023-05-15 15:26:50.000000 puput-1.2.1/puput/abstracts.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      234 2022-12-21 15:02:58.000000 puput-1.2.1/puput/apps.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     2159 2022-12-21 15:02:58.000000 puput-1.2.1/puput/comments.py
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.221129 puput-1.2.1/puput/conf/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      553 2022-12-21 15:02:58.000000 puput-1.2.1/puput/conf/__init__.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)       66 2022-12-21 15:02:58.000000 puput-1.2.1/puput/conf/defaults.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3152 2022-12-21 15:02:58.000000 puput-1.2.1/puput/feeds.py
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/ar/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.221129 puput-1.2.1/puput/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     4400 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/ar/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     5912 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/ar/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/ca/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.221129 puput-1.2.1/puput/locale/ca/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3278 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/ca/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     4949 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/ca/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/de/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.221129 puput-1.2.1/puput/locale/de/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3323 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     4974 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/en/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.221129 puput-1.2.1/puput/locale/en/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      378 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3975 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/es/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.221129 puput-1.2.1/puput/locale/es/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3025 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     4909 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/fr/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.225129 puput-1.2.1/puput/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3187 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     5029 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/it/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.225129 puput-1.2.1/puput/locale/it/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3299 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     4970 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/ja/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.225129 puput-1.2.1/puput/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3789 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/ja/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     5365 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/nl/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.225129 puput-1.2.1/puput/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      421 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     4022 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/pl/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.225129 puput-1.2.1/puput/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3432 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     5006 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/pt_BR/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.225129 puput-1.2.1/puput/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3319 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     5053 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/pt_PT/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.225129 puput-1.2.1/puput/locale/pt_PT/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      378 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/pt_PT/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3975 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/pt_PT/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/locale/ru/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.225129 puput-1.2.1/puput/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3249 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     5278 2022-12-21 15:02:58.000000 puput-1.2.1/puput/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.225129 puput-1.2.1/puput/management/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)        0 2022-12-21 15:02:58.000000 puput-1.2.1/puput/management/__init__.py
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.225129 puput-1.2.1/puput/management/commands/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)        0 2022-12-21 15:02:58.000000 puput-1.2.1/puput/management/commands/__init__.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     1118 2022-12-21 15:02:58.000000 puput-1.2.1/puput/management/commands/puput_initial_data.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      964 2022-12-21 15:02:58.000000 puput-1.2.1/puput/managers.py
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.229129 puput-1.2.1/puput/migrations/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     7008 2022-12-21 15:02:58.000000 puput-1.2.1/puput/migrations/0001_initial.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     1504 2022-12-21 15:02:58.000000 puput-1.2.1/puput/migrations/0002_auto_20150919_0925.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      441 2022-12-21 15:02:58.000000 puput-1.2.1/puput/migrations/0003_add_short_feed_description_to_blog_page.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      521 2022-12-21 15:02:58.000000 puput-1.2.1/puput/migrations/0004_auto_20170912_0928.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      517 2022-12-21 15:02:58.000000 puput-1.2.1/puput/migrations/0005_blogpage_main_color.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      476 2023-05-11 13:28:16.000000 puput-1.2.1/puput/migrations/0006_entrypage_markdown_body.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      445 2023-05-15 15:26:50.000000 puput-1.2.1/puput/migrations/0007_alter_entrypage_body.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)        0 2022-12-21 15:02:58.000000 puput-1.2.1/puput/migrations/__init__.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     6063 2023-05-11 13:28:16.000000 puput-1.2.1/puput/models.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3331 2022-12-21 15:02:58.000000 puput-1.2.1/puput/routes.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      632 2022-12-21 15:02:58.000000 puput-1.2.1/puput/signals.py
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/static/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.229129 puput-1.2.1/puput/static/colorful/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      111 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/colorful/arrow.gif
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      965 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/colorful/colorPicker.css
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/static/puput/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.229129 puput-1.2.1/puput/static/puput/css/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)   110143 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/css/bootstrap.min.css
--rw-rw-r--   0 csalom    (1001) csalom    (1001)    21984 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/css/font-awesome.min.css
--rw-rw-r--   0 csalom    (1001) csalom    (1001)    10929 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/css/puput.css
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.233129 puput-1.2.1/puput/static/puput/fonts/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)    85908 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/fonts/FontAwesome.otf
--rw-rw-r--   0 csalom    (1001) csalom    (1001)    56006 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 csalom    (1001) csalom    (1001)   287007 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 csalom    (1001) csalom    (1001)   112160 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 csalom    (1001) csalom    (1001)    65452 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/fonts/fontawesome-webfont.woff
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.233129 puput-1.2.1/puput/static/puput/js/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.233129 puput-1.2.1/puput/static/puput/js/comments/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      103 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/js/comments/disqus.js
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      376 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/js/comments/update_entry_comments.js
--rwxrwxr-x   0 csalom    (1001) csalom    (1001)    93868 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/js/jquery.min.js
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3285 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/js/js.cookie.js
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      558 2022-12-21 15:02:58.000000 puput-1.2.1/puput/static/puput/js/puput.js
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.233129 puput-1.2.1/puput/templates/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.233129 puput-1.2.1/puput/templates/el_pagination/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)       87 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/el_pagination/current_link.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      159 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/el_pagination/page_link.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      409 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/el_pagination/show_more.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      117 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/el_pagination/show_pages.html
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.237129 puput-1.2.1/puput/templates/puput/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     5957 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/base.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     4098 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/blog_page.html
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.237129 puput-1.2.1/puput/templates/puput/comments/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     1127 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/comments/disqus.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      136 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/comments/django_comments.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      901 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/entry_links.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3613 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/entry_page.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      150 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/entry_page_header.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     1235 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/related_entries.html
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.237129 puput-1.2.1/puput/templates/puput/tags/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      977 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/tags/archives_list.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      303 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/tags/categories_list.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     1215 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/tags/entries_list.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      121 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/tags/post_to_linkedin.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      278 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/puput/tags/tags_list.html
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      385 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/sitemap.xml
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.213129 puput-1.2.1/puput/templates/wagtailadmin/
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.237129 puput-1.2.1/puput/templates/wagtailadmin/pages/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      541 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templates/wagtailadmin/pages/_editor_css.html
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.237129 puput-1.2.1/puput/templatetags/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)        0 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templatetags/__init__.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     4351 2022-12-21 15:02:58.000000 puput-1.2.1/puput/templatetags/puput_tags.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3147 2022-12-21 15:02:58.000000 puput-1.2.1/puput/urls.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     1730 2022-12-21 15:02:58.000000 puput-1.2.1/puput/utils.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     2833 2022-12-21 15:02:58.000000 puput-1.2.1/puput/views.py
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     1759 2022-12-21 15:02:58.000000 puput-1.2.1/puput/wagtail_hooks.py
-drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-05-16 15:37:39.221129 puput-1.2.1/puput.egg-info/
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3754 2023-05-16 15:37:39.000000 puput-1.2.1/puput.egg-info/PKG-INFO
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     3437 2023-05-16 15:37:39.000000 puput-1.2.1/puput.egg-info/SOURCES.txt
--rw-rw-r--   0 csalom    (1001) csalom    (1001)        1 2023-05-16 15:37:39.000000 puput-1.2.1/puput.egg-info/dependency_links.txt
--rw-rw-r--   0 csalom    (1001) csalom    (1001)      136 2023-05-16 15:37:39.000000 puput-1.2.1/puput.egg-info/requires.txt
--rw-rw-r--   0 csalom    (1001) csalom    (1001)        6 2023-05-16 15:37:39.000000 puput-1.2.1/puput.egg-info/top_level.txt
--rw-rw-r--   0 csalom    (1001) csalom    (1001)       38 2023-05-16 15:37:39.241129 puput-1.2.1/setup.cfg
--rw-rw-r--   0 csalom    (1001) csalom    (1001)     1881 2023-05-16 15:31:14.000000 puput-1.2.1/setup.py
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.356312 puput-2.0.0/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      256 2023-05-11 13:28:16.000000 puput-2.0.0/AUTHORS
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     1063 2022-12-21 15:02:58.000000 puput-2.0.0/LICENSE
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      264 2022-12-21 15:02:58.000000 puput-2.0.0/MANIFEST.in
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3626 2023-07-04 07:28:01.356312 puput-2.0.0/PKG-INFO
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     2651 2023-06-02 09:04:17.000000 puput-2.0.0/README.rst
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.344312 puput-2.0.0/puput/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      668 2023-07-04 07:19:42.000000 puput-2.0.0/puput/__init__.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     5710 2023-06-02 09:04:17.000000 puput-2.0.0/puput/abstracts.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      234 2022-12-21 15:02:58.000000 puput-2.0.0/puput/apps.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     2159 2022-12-21 15:02:58.000000 puput-2.0.0/puput/comments.py
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.344312 puput-2.0.0/puput/conf/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      553 2022-12-21 15:02:58.000000 puput-2.0.0/puput/conf/__init__.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)       66 2022-12-21 15:02:58.000000 puput-2.0.0/puput/conf/defaults.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3147 2023-06-02 09:04:17.000000 puput-2.0.0/puput/feeds.py
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/ar/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.344312 puput-2.0.0/puput/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     4400 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     5912 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/ar/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/ca/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/locale/ca/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3278 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/ca/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     4949 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/ca/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/de/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3323 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     4974 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/en/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      378 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3975 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/es/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3025 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     4909 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/fr/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3187 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     5029 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/it/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3299 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     4970 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/ja/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3789 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     5365 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/nl/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      421 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     4022 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/pl/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3432 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     5006 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/pt_BR/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3319 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     5053 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/pt_PT/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/locale/pt_PT/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      378 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3975 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/pt_PT/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/locale/ru/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3249 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     5278 2022-12-21 15:02:58.000000 puput-2.0.0/puput/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/management/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)        0 2022-12-21 15:02:58.000000 puput-2.0.0/puput/management/__init__.py
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/management/commands/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)        0 2022-12-21 15:02:58.000000 puput-2.0.0/puput/management/commands/__init__.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     1113 2023-06-02 11:20:41.000000 puput-2.0.0/puput/management/commands/puput_initial_data.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      959 2023-06-02 09:04:17.000000 puput-2.0.0/puput/managers.py
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/migrations/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     6993 2023-06-02 09:04:17.000000 puput-2.0.0/puput/migrations/0001_initial.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     1494 2023-06-02 09:04:17.000000 puput-2.0.0/puput/migrations/0002_auto_20150919_0925.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      441 2022-12-21 15:02:58.000000 puput-2.0.0/puput/migrations/0003_add_short_feed_description_to_blog_page.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      521 2022-12-21 15:02:58.000000 puput-2.0.0/puput/migrations/0004_auto_20170912_0928.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      517 2022-12-21 15:02:58.000000 puput-2.0.0/puput/migrations/0005_blogpage_main_color.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      476 2023-05-11 13:28:16.000000 puput-2.0.0/puput/migrations/0006_entrypage_markdown_body.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      445 2023-05-15 15:26:50.000000 puput-2.0.0/puput/migrations/0007_alter_entrypage_body.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      593 2023-06-02 09:04:17.000000 puput-2.0.0/puput/migrations/0008_alter_tagentrypage_tag.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)        0 2022-12-21 15:02:58.000000 puput-2.0.0/puput/migrations/__init__.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     6051 2023-06-02 09:04:17.000000 puput-2.0.0/puput/models.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3326 2023-06-02 09:04:17.000000 puput-2.0.0/puput/routes.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      632 2022-12-21 15:02:58.000000 puput-2.0.0/puput/signals.py
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.340312 puput-2.0.0/puput/static/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.348312 puput-2.0.0/puput/static/colorful/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      111 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/colorful/arrow.gif
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      965 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/colorful/colorPicker.css
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.344312 puput-2.0.0/puput/static/puput/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.352312 puput-2.0.0/puput/static/puput/css/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)   110143 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/puput/css/bootstrap.min.css
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)    21984 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/puput/css/font-awesome.min.css
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)    10929 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/puput/css/puput.css
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.352312 puput-2.0.0/puput/static/puput/fonts/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)    85908 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/puput/fonts/FontAwesome.otf
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)    56006 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/puput/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)   287007 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/puput/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)   112160 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/puput/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)    65452 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/puput/fonts/fontawesome-webfont.woff
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.352312 puput-2.0.0/puput/static/puput/js/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.352312 puput-2.0.0/puput/static/puput/js/comments/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      103 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/puput/js/comments/disqus.js
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      376 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/puput/js/comments/update_entry_comments.js
+-rwxrwxr-x   0 csalom    (1001) csalom    (1001)    85577 2023-06-05 11:36:17.000000 puput-2.0.0/puput/static/puput/js/jquery.min.js
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3285 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/puput/js/js.cookie.js
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      558 2022-12-21 15:02:58.000000 puput-2.0.0/puput/static/puput/js/puput.js
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.352312 puput-2.0.0/puput/templates/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.352312 puput-2.0.0/puput/templates/el_pagination/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)       87 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/el_pagination/current_link.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      159 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/el_pagination/page_link.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      409 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/el_pagination/show_more.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      117 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/el_pagination/show_pages.html
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.352312 puput-2.0.0/puput/templates/puput/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     5957 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/base.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     4098 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/blog_page.html
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.352312 puput-2.0.0/puput/templates/puput/comments/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     1127 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/comments/disqus.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      136 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/comments/django_comments.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      901 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/entry_links.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3613 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/entry_page.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      150 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/entry_page_header.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     1235 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/related_entries.html
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.356312 puput-2.0.0/puput/templates/puput/tags/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      977 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/tags/archives_list.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      303 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/tags/categories_list.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     1215 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/tags/entries_list.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      121 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/tags/post_to_linkedin.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      278 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/puput/tags/tags_list.html
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      385 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/sitemap.xml
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.344312 puput-2.0.0/puput/templates/wagtailadmin/
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.356312 puput-2.0.0/puput/templates/wagtailadmin/pages/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      541 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templates/wagtailadmin/pages/_editor_css.html
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.356312 puput-2.0.0/puput/templatetags/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)        0 2022-12-21 15:02:58.000000 puput-2.0.0/puput/templatetags/__init__.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     4346 2023-06-02 09:04:17.000000 puput-2.0.0/puput/templatetags/puput_tags.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3142 2023-06-02 09:16:06.000000 puput-2.0.0/puput/urls.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     1730 2022-12-21 15:02:58.000000 puput-2.0.0/puput/utils.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     2823 2023-06-02 09:04:17.000000 puput-2.0.0/puput/views.py
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     1754 2023-06-02 09:04:17.000000 puput-2.0.0/puput/wagtail_hooks.py
+drwxrwxr-x   0 csalom    (1001) csalom    (1001)        0 2023-07-04 07:28:01.344312 puput-2.0.0/puput.egg-info/
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3626 2023-07-04 07:28:01.000000 puput-2.0.0/puput.egg-info/PKG-INFO
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     3485 2023-07-04 07:28:01.000000 puput-2.0.0/puput.egg-info/SOURCES.txt
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)        1 2023-07-04 07:28:01.000000 puput-2.0.0/puput.egg-info/dependency_links.txt
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)      162 2023-07-04 07:28:01.000000 puput-2.0.0/puput.egg-info/requires.txt
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)        6 2023-07-04 07:28:01.000000 puput-2.0.0/puput.egg-info/top_level.txt
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)       38 2023-07-04 07:28:01.356312 puput-2.0.0/setup.cfg
+-rw-rw-r--   0 csalom    (1001) csalom    (1001)     1956 2023-06-05 11:25:13.000000 puput-2.0.0/setup.py
```

### Comparing `puput-1.2.1/LICENSE` & `puput-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/PKG-INFO` & `puput-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: puput
-Version: 1.2.1
+Version: 2.0.0
 Summary: A Django blog app implemented in Wagtail.
 Home-page: http://github.com/APSL/puput
 Author: Marc Tudurí
 Author-email: marctc@gmail.com
 Keywords: django wagtail puput blog cms app
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -68,22 +69,19 @@
 
 .. image:: http://i.imgur.com/d13sGI3.png
 
 Examples of blog sites made with Puput
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * `Open Study Room <https://openstudyroom.org/blog/>`_
-* `Ncora Blog <https://www.ncora.com/blog/>`_
-* `Ncora TV <https://www.ncora.com/tv/>`_
 * `APSL <https://www.apsl.net/blog/>`_
 * `Nautic Advisor <https://www.nauticadvisor.com/blog/>`_
 * `Trespams <http://trespams.com/blog/>`_
 * `Body Therapy <http://bodytherapy.ru/blog/>`_
 * `Astro <http://www.mallorcasoft.es/blog/>`_
-* `Kontrabando Film Festival <https://www.kontrabandofilmfestival.org/blog/>`_
 * `IP/DE <https://ipde.com/>`_
 
 Setup
 ~~~~~
 
 The setup process is explained `here <http://puput.readthedocs.io/en/latest/setup.html>`_.
```

### Comparing `puput-1.2.1/README.rst` & `puput-2.0.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -42,22 +42,19 @@
 
 .. image:: http://i.imgur.com/d13sGI3.png
 
 Examples of blog sites made with Puput
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * `Open Study Room <https://openstudyroom.org/blog/>`_
-* `Ncora Blog <https://www.ncora.com/blog/>`_
-* `Ncora TV <https://www.ncora.com/tv/>`_
 * `APSL <https://www.apsl.net/blog/>`_
 * `Nautic Advisor <https://www.nauticadvisor.com/blog/>`_
 * `Trespams <http://trespams.com/blog/>`_
 * `Body Therapy <http://bodytherapy.ru/blog/>`_
 * `Astro <http://www.mallorcasoft.es/blog/>`_
-* `Kontrabando Film Festival <https://www.kontrabandofilmfestival.org/blog/>`_
 * `IP/DE <https://ipde.com/>`_
 
 Setup
 ~~~~~
 
 The setup process is explained `here <http://puput.readthedocs.io/en/latest/setup.html>`_.
```

### Comparing `puput-1.2.1/puput/__init__.py` & `puput-2.0.0/puput/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 __author__ = "Marc Tudurí"
 __email__ = "marctc@gmail.com"
-__version__ = "1.2.1"
+__version__ = "2.0.0"
 
 PUPUT_APPS = (
     # Wagtail apps
     "wagtail.contrib.legacy.richtext",
-    "wagtail.core",
     "wagtail.admin",
     "wagtail.documents",
     "wagtail.snippets",
     "wagtail.users",
     "wagtail.images",
     "wagtail.embeds",
     "wagtail.search",
     "wagtail.sites",
     "wagtail.contrib.redirects",
     "wagtail.contrib.forms",
     "wagtail.contrib.sitemaps",
     "wagtail.contrib.routable_page",
+    "wagtail",
     # Third-party apps
     "taggit",
     "modelcluster",
     "django_social_share",
     # Puput apps
     "puput",
     "wagtailmarkdown",
```

### Comparing `puput-1.2.1/puput/abstracts.py` & `puput-2.0.0/puput/abstracts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import datetime
 
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
-from wagtail.admin.edit_handlers import (
+from wagtail.admin.panels import (
     FieldPanel,
     MultiFieldPanel,
     InlinePanel,
-    PageChooserPanel,
 )
-from wagtail.core.fields import RichTextField
+from wagtail.fields import RichTextField
 from modelcluster.contrib.taggit import ClusterTaggableManager
 from wagtailmarkdown.fields import MarkdownField
 from colorful.fields import RGBColorField
 
 from .utils import get_image_model_path
 import markdown
 
@@ -137,15 +136,15 @@
         MultiFieldPanel(
             [
                 FieldPanel("tags"),
                 InlinePanel("entry_categories", label=_("Categories")),
                 InlinePanel(
                     "related_entrypage_from",
                     label=_("Related Entries"),
-                    panels=[PageChooserPanel("entrypage_to")],
+                    panels=[FieldPanel("entrypage_to")],
                 ),
             ],
             heading=_("Metadata"),
         ),
     ]
 
     class Meta:
```

### Comparing `puput-1.2.1/puput/comments.py` & `puput-2.0.0/puput/comments.py`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/conf/__init__.py` & `puput-2.0.0/puput/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/feeds.py` & `puput-2.0.0/puput/feeds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from mimetypes import guess_type
 from urllib.parse import urljoin
 
 from django import http
 from django.contrib.syndication.views import Feed
 from django.utils.feedgenerator import Rss201rev2Feed
 from django.template.defaultfilters import truncatewords_html
-from wagtail.core.models import Site
+from wagtail.models import Site
 
 from .models import BlogPage
 
 
 class BlogPageFeedGenerator(Rss201rev2Feed):
     def add_root_elements(self, handler):
         super(BlogPageFeedGenerator, self).add_root_elements(handler)
```

### Comparing `puput-1.2.1/puput/locale/ar/LC_MESSAGES/django.mo` & `puput-2.0.0/puput/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/ar/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/ca/LC_MESSAGES/django.mo` & `puput-2.0.0/puput/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/ca/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/de/LC_MESSAGES/django.mo` & `puput-2.0.0/puput/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/de/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/en/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/es/LC_MESSAGES/django.mo` & `puput-2.0.0/puput/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/es/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/fr/LC_MESSAGES/django.mo` & `puput-2.0.0/puput/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/fr/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/it/LC_MESSAGES/django.mo` & `puput-2.0.0/puput/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/it/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/ja/LC_MESSAGES/django.mo` & `puput-2.0.0/puput/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/ja/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/nl/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/pl/LC_MESSAGES/django.mo` & `puput-2.0.0/puput/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/pl/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/pt_BR/LC_MESSAGES/django.mo` & `puput-2.0.0/puput/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/pt_BR/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/pt_PT/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/ru/LC_MESSAGES/django.mo` & `puput-2.0.0/puput/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/locale/ru/LC_MESSAGES/django.po` & `puput-2.0.0/puput/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/management/commands/puput_initial_data.py` & `puput-2.0.0/puput/management/commands/puput_initial_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django import VERSION as DJANGO_VERSION
 from django.contrib.contenttypes.models import ContentType
 from django.core.management import BaseCommand
 
 from puput.models import BlogPage
-from wagtail.core.models import Page, Site
+from wagtail.models import Page, Site
 
 
 class Command(BaseCommand):
     help = "Load Puput initial dummy data"
 
     def handle(self, *args, **options):
         # Get blogpage content type
```

### Comparing `puput-1.2.1/puput/managers.py` & `puput-2.0.0/puput/managers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.db import models
 from django.db.models import Count
-from wagtail.core.models import PageManager
+from wagtail.models import PageManager
 
 from .utils import strip_prefix_and_ending_slash
 
 
 class TagManager(models.Manager):
     def most_common(self, blog_page):
         entries = blog_page.get_entries()
```

### Comparing `puput-1.2.1/puput/migrations/0001_initial.py` & `puput-2.0.0/puput/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import unicode_literals
 
 from django.db import models, migrations
-import wagtail.core.fields
+import wagtail.fields
 import puput.routes
 import datetime
 import django.db.models.deletion
 import modelcluster.contrib.taggit
 import modelcluster.fields
 
 
@@ -67,17 +67,17 @@
             },
             bases=(models.Model,),
         ),
         migrations.CreateModel(
             name='EntryPage',
             fields=[
                 ('page_ptr', models.OneToOneField(parent_link=True, auto_created=True, primary_key=True, serialize=False, to='wagtailcore.Page', on_delete=models.CASCADE)),
-                ('body', wagtail.core.fields.RichTextField(verbose_name='body')),
+                ('body', wagtail.fields.RichTextField(verbose_name='body')),
                 ('date', models.DateTimeField(default=datetime.datetime.today, verbose_name='Post date')),
-                ('excerpt', wagtail.core.fields.RichTextField(help_text='Used to display on puput pages list. If this field is not filled, a truncate version of body text will be used.', verbose_name='excerpt', blank=True)),
+                ('excerpt', wagtail.fields.RichTextField(help_text='Used to display on puput pages list. If this field is not filled, a truncate version of body text will be used.', verbose_name='excerpt', blank=True)),
                 ('num_comments', models.IntegerField(default=0, editable=False)),
                 ('categories', models.ManyToManyField(to='puput.Category', through='puput.CategoryEntryPage', blank=True)),
                 ('header_image', models.ForeignKey(related_name='+', on_delete=django.db.models.deletion.SET_NULL, verbose_name='Header image', blank=True, to='wagtailimages.Image', null=True)),
             ],
             options={
                 'verbose_name': 'Entry',
                 'verbose_name_plural': 'Entries',
```

### Comparing `puput-1.2.1/puput/migrations/0002_auto_20150919_0925.py` & `puput-2.0.0/puput/migrations/0002_auto_20150919_0925.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import unicode_literals
 
 from django.db import models, migrations
-import wagtail.core.fields
+import wagtail.fields
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('puput', '0001_initial'),
     ]
@@ -30,10 +30,10 @@
             model_name='category',
             name='parent',
             field=models.ForeignKey(to='puput.Category', related_name='children', null=True, verbose_name='Parent category', blank=True, on_delete=models.SET_NULL),
         ),
         migrations.AlterField(
             model_name='entrypage',
             name='excerpt',
-            field=wagtail.core.fields.RichTextField(help_text='Entry excerpt to be displayed on entries list. If this field is not filled, a truncate version of body text will be used.', verbose_name='excerpt', blank=True),
+            field=wagtail.fields.RichTextField(help_text='Entry excerpt to be displayed on entries list. If this field is not filled, a truncate version of body text will be used.', verbose_name='excerpt', blank=True),
         ),
     ]
```

### Comparing `puput-1.2.1/puput/migrations/0004_auto_20170912_0928.py` & `puput-2.0.0/puput/migrations/0004_auto_20170912_0928.py`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/migrations/0005_blogpage_main_color.py` & `puput-2.0.0/puput/migrations/0005_blogpage_main_color.py`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/models.py` & `puput-2.0.0/puput/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import markdown
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.template.defaultfilters import slugify
 from django.utils.translation import gettext_lazy as _
 
-from wagtail.core.models import Page
-from wagtail.admin.edit_handlers import FieldPanel
+from wagtail.models import Page
+from wagtail.admin.panels import FieldPanel
 from wagtail.snippets.models import register_snippet
 from wagtail.search import index
 from taggit.models import TaggedItemBase, Tag as TaggitTag
 from modelcluster.fields import ParentalKey
 
 from .abstracts import EntryAbstract, BlogAbstract
 from .utils import import_model
```

### Comparing `puput-1.2.1/puput/routes.py` & `puput-2.0.0/puput/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.contrib.auth import get_user_model
 from django.utils.dateformat import DateFormat
 from django.utils.formats import date_format
 from django.utils.translation import gettext_lazy as _
 from django.conf import settings
 
 from wagtail.contrib.routable_page.models import RoutablePageMixin, route
-from wagtail.core.models import Page
+from wagtail.models import Page
 from wagtail.search.models import Query
 
 from .utils import get_object_or_None
 
 USERNAME_REGEX = getattr(settings, "PUPUT_USERNAME_REGEX", "\\w+")
 USERNAME_FIELD = getattr(settings, "PUPUT_USERNAME_FIELD", "username")
```

### Comparing `puput-1.2.1/puput/signals.py` & `puput-2.0.0/puput/signals.py`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/static/colorful/colorPicker.css` & `puput-2.0.0/puput/static/colorful/colorPicker.css`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/static/puput/css/bootstrap.min.css` & `puput-2.0.0/puput/static/puput/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/static/puput/css/font-awesome.min.css` & `puput-2.0.0/puput/static/puput/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/static/puput/css/puput.css` & `puput-2.0.0/puput/static/puput/css/puput.css`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/static/puput/fonts/FontAwesome.otf` & `puput-2.0.0/puput/static/puput/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/static/puput/fonts/fontawesome-webfont.eot` & `puput-2.0.0/puput/static/puput/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/static/puput/fonts/fontawesome-webfont.svg` & `puput-2.0.0/puput/static/puput/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/static/puput/fonts/fontawesome-webfont.ttf` & `puput-2.0.0/puput/static/puput/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/static/puput/fonts/fontawesome-webfont.woff` & `puput-2.0.0/puput/static/puput/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/static/puput/js/jquery.min.js` & `puput-2.0.0/puput/static/puput/js/jquery.min.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,3726 +1,3133 @@
-/*! jQuery v1.7.1 jquery.com | jquery.org/license */
-(function(a, b) {
-    function cy(a) {
-        return f.isWindow(a) ? a : a.nodeType === 9 ? a.defaultView || a.parentWindow : !1
-    }
-
-    function cv(a) {
-        if (!ck[a]) {
-            var b = c.body,
-                d = f("<" + a + ">").appendTo(b),
-                e = d.css("display");
-            d.remove();
-            if (e === "none" || e === "") {
-                cl || (cl = c.createElement("iframe"), cl.frameBorder = cl.width = cl.height = 0), b.appendChild(cl);
-                if (!cm || !cl.createElement) cm = (cl.contentWindow || cl.contentDocument).document, cm.write((c.compatMode === "CSS1Compat" ? "<!doctype html>" : "") + "<html><body>"), cm.close();
-                d = cm.createElement(a), cm.body.appendChild(d), e = f.css(d, "display"), b.removeChild(cl)
-            }
-            ck[a] = e
-        }
-        return ck[a]
-    }
-
-    function cu(a, b) {
-        var c = {};
-        f.each(cq.concat.apply([], cq.slice(0, b)), function() {
-            c[this] = a
-        });
-        return c
-    }
-
-    function ct() {
-        cr = b
-    }
-
-    function cs() {
-        setTimeout(ct, 0);
-        return cr = f.now()
-    }
-
-    function cj() {
-        try {
-            return new a.ActiveXObject("Microsoft.XMLHTTP")
-        } catch (b) {}
-    }
+/*! jQuery v2.2.4 | (c) jQuery Foundation | jquery.org/license */ ! function(a, b) {
+    "object" == typeof module && "object" == typeof module.exports ? module.exports = a.document ? b(a, !0) : function(a) {
+        if (!a.document) throw new Error("jQuery requires a window with a document");
+        return b(a)
+    } : b(a)
+}("undefined" != typeof window ? window : this, function(a, b) {
+    var c = [],
+        d = a.document,
+        e = c.slice,
+        f = c.concat,
+        g = c.push,
+        h = c.indexOf,
+        i = {},
+        j = i.toString,
+        k = i.hasOwnProperty,
+        l = {},
+        m = "2.2.4",
+        n = function(a, b) {
+            return new n.fn.init(a, b)
+        },
+        o = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g,
+        p = /^-ms-/,
+        q = /-([\da-z])/gi,
+        r = function(a, b) {
+            return b.toUpperCase()
+        };
+    n.fn = n.prototype = {
+        jquery: m,
+        constructor: n,
+        selector: "",
+        length: 0,
+        toArray: function() {
+            return e.call(this)
+        },
+        get: function(a) {
+            return null != a ? 0 > a ? this[a + this.length] : this[a] : e.call(this)
+        },
+        pushStack: function(a) {
+            var b = n.merge(this.constructor(), a);
+            return b.prevObject = this, b.context = this.context, b
+        },
+        each: function(a) {
+            return n.each(this, a)
+        },
+        map: function(a) {
+            return this.pushStack(n.map(this, function(b, c) {
+                return a.call(b, c, b)
+            }))
+        },
+        slice: function() {
+            return this.pushStack(e.apply(this, arguments))
+        },
+        first: function() {
+            return this.eq(0)
+        },
+        last: function() {
+            return this.eq(-1)
+        },
+        eq: function(a) {
+            var b = this.length,
+                c = +a + (0 > a ? b : 0);
+            return this.pushStack(c >= 0 && b > c ? [this[c]] : [])
+        },
+        end: function() {
+            return this.prevObject || this.constructor()
+        },
+        push: g,
+        sort: c.sort,
+        splice: c.splice
+    }, n.extend = n.fn.extend = function() {
+        var a, b, c, d, e, f, g = arguments[0] || {},
+            h = 1,
+            i = arguments.length,
+            j = !1;
+        for ("boolean" == typeof g && (j = g, g = arguments[h] || {}, h++), "object" == typeof g || n.isFunction(g) || (g = {}), h === i && (g = this, h--); i > h; h++)
+            if (null != (a = arguments[h]))
+                for (b in a) c = g[b], d = a[b], g !== d && (j && d && (n.isPlainObject(d) || (e = n.isArray(d))) ? (e ? (e = !1, f = c && n.isArray(c) ? c : []) : f = c && n.isPlainObject(c) ? c : {}, g[b] = n.extend(j, f, d)) : void 0 !== d && (g[b] = d));
+        return g
+    }, n.extend({
+        expando: "jQuery" + (m + Math.random()).replace(/\D/g, ""),
+        isReady: !0,
+        error: function(a) {
+            throw new Error(a)
+        },
+        noop: function() {},
+        isFunction: function(a) {
+            return "function" === n.type(a)
+        },
+        isArray: Array.isArray,
+        isWindow: function(a) {
+            return null != a && a === a.window
+        },
+        isNumeric: function(a) {
+            var b = a && a.toString();
+            return !n.isArray(a) && b - parseFloat(b) + 1 >= 0
+        },
+        isPlainObject: function(a) {
+            var b;
+            if ("object" !== n.type(a) || a.nodeType || n.isWindow(a)) return !1;
+            if (a.constructor && !k.call(a, "constructor") && !k.call(a.constructor.prototype || {}, "isPrototypeOf")) return !1;
+            for (b in a);
+            return void 0 === b || k.call(a, b)
+        },
+        isEmptyObject: function(a) {
+            var b;
+            for (b in a) return !1;
+            return !0
+        },
+        type: function(a) {
+            return null == a ? a + "" : "object" == typeof a || "function" == typeof a ? i[j.call(a)] || "object" : typeof a
+        },
+        globalEval: function(a) {
+            var b, c = eval;
+            a = n.trim(a), a && (1 === a.indexOf("use strict") ? (b = d.createElement("script"), b.text = a, d.head.appendChild(b).parentNode.removeChild(b)) : c(a))
+        },
+        camelCase: function(a) {
+            return a.replace(p, "ms-").replace(q, r)
+        },
+        nodeName: function(a, b) {
+            return a.nodeName && a.nodeName.toLowerCase() === b.toLowerCase()
+        },
+        each: function(a, b) {
+            var c, d = 0;
+            if (s(a)) {
+                for (c = a.length; c > d; d++)
+                    if (b.call(a[d], d, a[d]) === !1) break
+            } else
+                for (d in a)
+                    if (b.call(a[d], d, a[d]) === !1) break;
+            return a
+        },
+        trim: function(a) {
+            return null == a ? "" : (a + "").replace(o, "")
+        },
+        makeArray: function(a, b) {
+            var c = b || [];
+            return null != a && (s(Object(a)) ? n.merge(c, "string" == typeof a ? [a] : a) : g.call(c, a)), c
+        },
+        inArray: function(a, b, c) {
+            return null == b ? -1 : h.call(b, a, c)
+        },
+        merge: function(a, b) {
+            for (var c = +b.length, d = 0, e = a.length; c > d; d++) a[e++] = b[d];
+            return a.length = e, a
+        },
+        grep: function(a, b, c) {
+            for (var d, e = [], f = 0, g = a.length, h = !c; g > f; f++) d = !b(a[f], f), d !== h && e.push(a[f]);
+            return e
+        },
+        map: function(a, b, c) {
+            var d, e, g = 0,
+                h = [];
+            if (s(a))
+                for (d = a.length; d > g; g++) e = b(a[g], g, c), null != e && h.push(e);
+            else
+                for (g in a) e = b(a[g], g, c), null != e && h.push(e);
+            return f.apply([], h)
+        },
+        guid: 1,
+        proxy: function(a, b) {
+            var c, d, f;
+            return "string" == typeof b && (c = a[b], b = a, a = c), n.isFunction(a) ? (d = e.call(arguments, 2), f = function() {
+                return a.apply(b || this, d.concat(e.call(arguments)))
+            }, f.guid = a.guid = a.guid || n.guid++, f) : void 0
+        },
+        now: Date.now,
+        support: l
+    }), "function" == typeof Symbol && (n.fn[Symbol.iterator] = c[Symbol.iterator]), n.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), function(a, b) {
+        i["[object " + b + "]"] = b.toLowerCase()
+    });
 
-    function ci() {
+    function s(a) {
+        var b = !!a && "length" in a && a.length,
+            c = n.type(a);
+        return "function" === c || n.isWindow(a) ? !1 : "array" === c || 0 === b || "number" == typeof b && b > 0 && b - 1 in a
+    }
+    var t = function(a) {
+        var b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u = "sizzle" + 1 * new Date,
+            v = a.document,
+            w = 0,
+            x = 0,
+            y = ga(),
+            z = ga(),
+            A = ga(),
+            B = function(a, b) {
+                return a === b && (l = !0), 0
+            },
+            C = 1 << 31,
+            D = {}.hasOwnProperty,
+            E = [],
+            F = E.pop,
+            G = E.push,
+            H = E.push,
+            I = E.slice,
+            J = function(a, b) {
+                for (var c = 0, d = a.length; d > c; c++)
+                    if (a[c] === b) return c;
+                return -1
+            },
+            K = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
+            L = "[\\x20\\t\\r\\n\\f]",
+            M = "(?:\\\\.|[\\w-]|[^\\x00-\\xa0])+",
+            N = "\\[" + L + "*(" + M + ")(?:" + L + "*([*^$|!~]?=)" + L + "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + M + "))|)" + L + "*\\]",
+            O = ":(" + M + ")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|" + N + ")*)|.*)\\)|)",
+            P = new RegExp(L + "+", "g"),
+            Q = new RegExp("^" + L + "+|((?:^|[^\\\\])(?:\\\\.)*)" + L + "+$", "g"),
+            R = new RegExp("^" + L + "*," + L + "*"),
+            S = new RegExp("^" + L + "*([>+~]|" + L + ")" + L + "*"),
+            T = new RegExp("=" + L + "*([^\\]'\"]*?)" + L + "*\\]", "g"),
+            U = new RegExp(O),
+            V = new RegExp("^" + M + "$"),
+            W = {
+                ID: new RegExp("^#(" + M + ")"),
+                CLASS: new RegExp("^\\.(" + M + ")"),
+                TAG: new RegExp("^(" + M + "|[*])"),
+                ATTR: new RegExp("^" + N),
+                PSEUDO: new RegExp("^" + O),
+                CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + L + "*(even|odd|(([+-]|)(\\d*)n|)" + L + "*(?:([+-]|)" + L + "*(\\d+)|))" + L + "*\\)|)", "i"),
+                bool: new RegExp("^(?:" + K + ")$", "i"),
+                needsContext: new RegExp("^" + L + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + L + "*((?:-\\d)?\\d*)" + L + "*\\)|)(?=[^-]|$)", "i")
+            },
+            X = /^(?:input|select|textarea|button)$/i,
+            Y = /^h\d$/i,
+            Z = /^[^{]+\{\s*\[native \w/,
+            $ = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
+            _ = /[+~]/,
+            aa = /'|\\/g,
+            ba = new RegExp("\\\\([\\da-f]{1,6}" + L + "?|(" + L + ")|.)", "ig"),
+            ca = function(a, b, c) {
+                var d = "0x" + b - 65536;
+                return d !== d || c ? b : 0 > d ? String.fromCharCode(d + 65536) : String.fromCharCode(d >> 10 | 55296, 1023 & d | 56320)
+            },
+            da = function() {
+                m()
+            };
         try {
-            return new a.XMLHttpRequest
-        } catch (b) {}
-    }
-
-    function cc(a, c) {
-        a.dataFilter && (c = a.dataFilter(c, a.dataType));
-        var d = a.dataTypes,
-            e = {},
-            g, h, i = d.length,
-            j, k = d[0],
-            l, m, n, o, p;
-        for (g = 1; g < i; g++) {
-            if (g === 1)
-                for (h in a.converters) typeof h == "string" && (e[h.toLowerCase()] = a.converters[h]);
-            l = k, k = d[g];
-            if (k === "*") k = l;
-            else if (l !== "*" && l !== k) {
-                m = l + " " + k, n = e[m] || e["* " + k];
-                if (!n) {
-                    p = b;
-                    for (o in e) {
-                        j = o.split(" ");
-                        if (j[0] === l || j[0] === "*") {
-                            p = e[j[1] + " " + k];
-                            if (p) {
-                                o = e[o], o === !0 ? n = p : p === !0 && (n = o);
-                                break
-                            }
-                        }
-                    }
-                }!n && !p && f.error("No conversion from " + m.replace(" ", " to ")), n !== !0 && (c = n ? n(c) : p(o(c)))
+            H.apply(E = I.call(v.childNodes), v.childNodes), E[v.childNodes.length].nodeType
+        } catch (ea) {
+            H = {
+                apply: E.length ? function(a, b) {
+                    G.apply(a, I.call(b))
+                } : function(a, b) {
+                    var c = a.length,
+                        d = 0;
+                    while (a[c++] = b[d++]);
+                    a.length = c - 1
+                }
             }
         }
-        return c
-    }
 
-    function cb(a, c, d) {
-        var e = a.contents,
-            f = a.dataTypes,
-            g = a.responseFields,
-            h, i, j, k;
-        for (i in g) i in d && (c[g[i]] = d[i]);
-        while (f[0] === "*") f.shift(), h === b && (h = a.mimeType || c.getResponseHeader("content-type"));
-        if (h)
-            for (i in e)
-                if (e[i] && e[i].test(h)) {
-                    f.unshift(i);
-                    break
-                } if (f[0] in d) j = f[0];
-        else {
-            for (i in d) {
-                if (!f[0] || a.converters[i + " " + f[0]]) {
-                    j = i;
-                    break
+        function fa(a, b, d, e) {
+            var f, h, j, k, l, o, r, s, w = b && b.ownerDocument,
+                x = b ? b.nodeType : 9;
+            if (d = d || [], "string" != typeof a || !a || 1 !== x && 9 !== x && 11 !== x) return d;
+            if (!e && ((b ? b.ownerDocument || b : v) !== n && m(b), b = b || n, p)) {
+                if (11 !== x && (o = $.exec(a)))
+                    if (f = o[1]) {
+                        if (9 === x) {
+                            if (!(j = b.getElementById(f))) return d;
+                            if (j.id === f) return d.push(j), d
+                        } else if (w && (j = w.getElementById(f)) && t(b, j) && j.id === f) return d.push(j), d
+                    } else {
+                        if (o[2]) return H.apply(d, b.getElementsByTagName(a)), d;
+                        if ((f = o[3]) && c.getElementsByClassName && b.getElementsByClassName) return H.apply(d, b.getElementsByClassName(f)), d
+                    } if (c.qsa && !A[a + " "] && (!q || !q.test(a))) {
+                    if (1 !== x) w = b, s = a;
+                    else if ("object" !== b.nodeName.toLowerCase()) {
+                        (k = b.getAttribute("id")) ? k = k.replace(aa, "\\$&"): b.setAttribute("id", k = u), r = g(a), h = r.length, l = V.test(k) ? "#" + k : "[id='" + k + "']";
+                        while (h--) r[h] = l + " " + qa(r[h]);
+                        s = r.join(","), w = _.test(a) && oa(b.parentNode) || b
+                    }
+                    if (s) try {
+                        return H.apply(d, w.querySelectorAll(s)), d
+                    } catch (y) {} finally {
+                        k === u && b.removeAttribute("id")
+                    }
                 }
-                k || (k = i)
             }
-            j = j || k
+            return i(a.replace(Q, "$1"), b, d, e)
         }
-        if (j) {
-            j !== f[0] && f.unshift(j);
-            return d[j]
-        }
-    }
 
-    function ca(a, b, c, d) {
-        if (f.isArray(b)) f.each(b, function(b, e) {
-            c || bE.test(a) ? d(a, e) : ca(a + "[" + (typeof e == "object" || f.isArray(e) ? b : "") + "]", e, c, d)
-        });
-        else if (!c && b != null && typeof b == "object")
-            for (var e in b) ca(a + "[" + e + "]", b[e], c, d);
-        else d(a, b)
-    }
-
-    function b_(a, c) {
-        var d, e, g = f.ajaxSettings.flatOptions || {};
-        for (d in c) c[d] !== b && ((g[d] ? a : e || (e = {}))[d] = c[d]);
-        e && f.extend(!0, a, e)
-    }
-
-    function b$(a, c, d, e, f, g) {
-        f = f || c.dataTypes[0], g = g || {}, g[f] = !0;
-        var h = a[f],
-            i = 0,
-            j = h ? h.length : 0,
-            k = a === bT,
-            l;
-        for (; i < j && (k || !l); i++) l = h[i](c, d, e), typeof l == "string" && (!k || g[l] ? l = b : (c.dataTypes.unshift(l), l = b$(a, c, d, e, l, g)));
-        (k || !l) && !g["*"] && (l = b$(a, c, d, e, "*", g));
-        return l
-    }
+        function ga() {
+            var a = [];
 
-    function bZ(a) {
-        return function(b, c) {
-            typeof b != "string" && (c = b, b = "*");
-            if (f.isFunction(c)) {
-                var d = b.toLowerCase().split(bP),
-                    e = 0,
-                    g = d.length,
-                    h, i, j;
-                for (; e < g; e++) h = d[e], j = /^\+/.test(h), j && (h = h.substr(1) || "*"), i = a[h] = a[h] || [], i[j ? "unshift" : "push"](c)
+            function b(c, e) {
+                return a.push(c + " ") > d.cacheLength && delete b[a.shift()], b[c + " "] = e
             }
+            return b
         }
-    }
-
-    function bC(a, b, c) {
-        var d = b === "width" ? a.offsetWidth : a.offsetHeight,
-            e = b === "width" ? bx : by,
-            g = 0,
-            h = e.length;
-        if (d > 0) {
-            if (c !== "border")
-                for (; g < h; g++) c || (d -= parseFloat(f.css(a, "padding" + e[g])) || 0), c === "margin" ? d += parseFloat(f.css(a, c + e[g])) || 0 : d -= parseFloat(f.css(a, "border" + e[g] + "Width")) || 0;
-            return d + "px"
-        }
-        d = bz(a, b, b);
-        if (d < 0 || d == null) d = a.style[b] || 0;
-        d = parseFloat(d) || 0;
-        if (c)
-            for (; g < h; g++) d += parseFloat(f.css(a, "padding" + e[g])) || 0, c !== "padding" && (d += parseFloat(f.css(a, "border" + e[g] + "Width")) || 0), c === "margin" && (d += parseFloat(f.css(a, c + e[g])) || 0);
-        return d + "px"
-    }
-
-    function bp(a, b) {
-        b.src ? f.ajax({
-            url: b.src,
-            async: !1,
-            dataType: "script"
-        }) : f.globalEval((b.text || b.textContent || b.innerHTML || "").replace(bf, "/*$0*/")), b.parentNode && b.parentNode.removeChild(b)
-    }
-
-    function bo(a) {
-        var b = c.createElement("div");
-        bh.appendChild(b), b.innerHTML = a.outerHTML;
-        return b.firstChild
-    }
-
-    function bn(a) {
-        var b = (a.nodeName || "").toLowerCase();
-        b === "input" ? bm(a) : b !== "script" && typeof a.getElementsByTagName != "undefined" && f.grep(a.getElementsByTagName("input"), bm)
-    }
 
-    function bm(a) {
-        if (a.type === "checkbox" || a.type === "radio") a.defaultChecked = a.checked
-    }
-
-    function bl(a) {
-        return typeof a.getElementsByTagName != "undefined" ? a.getElementsByTagName("*") : typeof a.querySelectorAll != "undefined" ? a.querySelectorAll("*") : []
-    }
-
-    function bk(a, b) {
-        var c;
-        if (b.nodeType === 1) {
-            b.clearAttributes && b.clearAttributes(), b.mergeAttributes && b.mergeAttributes(a), c = b.nodeName.toLowerCase();
-            if (c === "object") b.outerHTML = a.outerHTML;
-            else if (c !== "input" || a.type !== "checkbox" && a.type !== "radio") {
-                if (c === "option") b.selected = a.defaultSelected;
-                else if (c === "input" || c === "textarea") b.defaultValue = a.defaultValue
-            } else a.checked && (b.defaultChecked = b.checked = a.checked), b.value !== a.value && (b.value = a.value);
-            b.removeAttribute(f.expando)
+        function ha(a) {
+            return a[u] = !0, a
         }
-    }
 
-    function bj(a, b) {
-        if (b.nodeType === 1 && !!f.hasData(a)) {
-            var c, d, e, g = f._data(a),
-                h = f._data(b, g),
-                i = g.events;
-            if (i) {
-                delete h.handle, h.events = {};
-                for (c in i)
-                    for (d = 0, e = i[c].length; d < e; d++) f.event.add(b, c + (i[c][d].namespace ? "." : "") + i[c][d].namespace, i[c][d], i[c][d].data)
+        function ia(a) {
+            var b = n.createElement("div");
+            try {
+                return !!a(b)
+            } catch (c) {
+                return !1
+            } finally {
+                b.parentNode && b.parentNode.removeChild(b), b = null
             }
-            h.data && (h.data = f.extend({}, h.data))
         }
-    }
-
-    function bi(a, b) {
-        return f.nodeName(a, "table") ? a.getElementsByTagName("tbody")[0] || a.appendChild(a.ownerDocument.createElement("tbody")) : a
-    }
-
-    function U(a) {
-        var b = V.split("|"),
-            c = a.createDocumentFragment();
-        if (c.createElement)
-            while (b.length) c.createElement(b.pop());
-        return c
-    }
 
-    function T(a, b, c) {
-        b = b || 0;
-        if (f.isFunction(b)) return f.grep(a, function(a, d) {
-            var e = !!b.call(a, d, a);
-            return e === c
-        });
-        if (b.nodeType) return f.grep(a, function(a, d) {
-            return a === b === c
-        });
-        if (typeof b == "string") {
-            var d = f.grep(a, function(a) {
-                return a.nodeType === 1
-            });
-            if (O.test(b)) return f.filter(b, d, !c);
-            b = f.filter(b, d)
+        function ja(a, b) {
+            var c = a.split("|"),
+                e = c.length;
+            while (e--) d.attrHandle[c[e]] = b
         }
-        return f.grep(a, function(a, d) {
-            return f.inArray(a, b) >= 0 === c
-        })
-    }
 
-    function S(a) {
-        return !a || !a.parentNode || a.parentNode.nodeType === 11
-    }
-
-    function K() {
-        return !0
-    }
+        function ka(a, b) {
+            var c = b && a,
+                d = c && 1 === a.nodeType && 1 === b.nodeType && (~b.sourceIndex || C) - (~a.sourceIndex || C);
+            if (d) return d;
+            if (c)
+                while (c = c.nextSibling)
+                    if (c === b) return -1;
+            return a ? 1 : -1
+        }
 
-    function J() {
-        return !1
-    }
+        function la(a) {
+            return function(b) {
+                var c = b.nodeName.toLowerCase();
+                return "input" === c && b.type === a
+            }
+        }
 
-    function n(a, b, c) {
-        var d = b + "defer",
-            e = b + "queue",
-            g = b + "mark",
-            h = f._data(a, d);
-        h && (c === "queue" || !f._data(a, e)) && (c === "mark" || !f._data(a, g)) && setTimeout(function() {
-            !f._data(a, e) && !f._data(a, g) && (f.removeData(a, d, !0), h.fire())
-        }, 0)
-    }
+        function ma(a) {
+            return function(b) {
+                var c = b.nodeName.toLowerCase();
+                return ("input" === c || "button" === c) && b.type === a
+            }
+        }
 
-    function m(a) {
-        for (var b in a) {
-            if (b === "data" && f.isEmptyObject(a[b])) continue;
-            if (b !== "toJSON") return !1
+        function na(a) {
+            return ha(function(b) {
+                return b = +b, ha(function(c, d) {
+                    var e, f = a([], c.length, b),
+                        g = f.length;
+                    while (g--) c[e = f[g]] && (c[e] = !(d[e] = c[e]))
+                })
+            })
         }
-        return !0
-    }
 
-    function l(a, c, d) {
-        if (d === b && a.nodeType === 1) {
-            var e = "data-" + c.replace(k, "-$1").toLowerCase();
-            d = a.getAttribute(e);
-            if (typeof d == "string") {
-                try {
-                    d = d === "true" ? !0 : d === "false" ? !1 : d === "null" ? null : f.isNumeric(d) ? parseFloat(d) : j.test(d) ? f.parseJSON(d) : d
-                } catch (g) {}
-                f.data(a, c, d)
-            } else d = b
-        }
-        return d
-    }
-
-    function h(a) {
-        var b = g[a] = {},
-            c, d;
-        a = a.split(/\s+/);
-        for (c = 0, d = a.length; c < d; c++) b[a[c]] = !0;
-        return b
-    }
-    var c = a.document,
-        d = a.navigator,
-        e = a.location,
-        f = function() {
-            function J() {
-                if (!e.isReady) {
-                    try {
-                        c.documentElement.doScroll("left")
-                    } catch (a) {
-                        setTimeout(J, 1);
-                        return
-                    }
-                    e.ready()
-                }
-            }
-            var e = function(a, b) {
-                    return new e.fn.init(a, b, h)
-                },
-                f = a.jQuery,
-                g = a.$,
-                h, i = /^(?:[^#<]*(<[\w\W]+>)[^>]*$|#([\w\-]*)$)/,
-                j = /\S/,
-                k = /^\s+/,
-                l = /\s+$/,
-                m = /^<(\w+)\s*\/?>(?:<\/\1>)?$/,
-                n = /^[\],:{}\s]*$/,
-                o = /\\(?:["\\\/bfnrt]|u[0-9a-fA-F]{4})/g,
-                p = /"[^"\\\n\r]*"|true|false|null|-?\d+(?:\.\d*)?(?:[eE][+\-]?\d+)?/g,
-                q = /(?:^|:|,)(?:\s*\[)+/g,
-                r = /(webkit)[ \/]([\w.]+)/,
-                s = /(opera)(?:.*version)?[ \/]([\w.]+)/,
-                t = /(msie) ([\w.]+)/,
-                u = /(mozilla)(?:.*? rv:([\w.]+))?/,
-                v = /-([a-z]|[0-9])/ig,
-                w = /^-ms-/,
-                x = function(a, b) {
-                    return (b + "").toUpperCase()
-                },
-                y = d.userAgent,
-                z, A, B, C = Object.prototype.toString,
-                D = Object.prototype.hasOwnProperty,
-                E = Array.prototype.push,
-                F = Array.prototype.slice,
-                G = String.prototype.trim,
-                H = Array.prototype.indexOf,
-                I = {};
-            e.fn = e.prototype = {
-                constructor: e,
-                init: function(a, d, f) {
-                    var g, h, j, k;
-                    if (!a) return this;
-                    if (a.nodeType) {
-                        this.context = this[0] = a, this.length = 1;
-                        return this
-                    }
-                    if (a === "body" && !d && c.body) {
-                        this.context = c, this[0] = c.body, this.selector = a, this.length = 1;
-                        return this
-                    }
-                    if (typeof a == "string") {
-                        a.charAt(0) !== "<" || a.charAt(a.length - 1) !== ">" || a.length < 3 ? g = i.exec(a) : g = [null, a, null];
-                        if (g && (g[1] || !d)) {
-                            if (g[1]) {
-                                d = d instanceof e ? d[0] : d, k = d ? d.ownerDocument || d : c, j = m.exec(a), j ? e.isPlainObject(d) ? (a = [c.createElement(j[1])], e.fn.attr.call(a, d, !0)) : a = [k.createElement(j[1])] : (j = e.buildFragment([g[1]], [k]), a = (j.cacheable ? e.clone(j.fragment) : j.fragment).childNodes);
-                                return e.merge(this, a)
-                            }
-                            h = c.getElementById(g[2]);
-                            if (h && h.parentNode) {
-                                if (h.id !== g[2]) return f.find(a);
-                                this.length = 1, this[0] = h
+        function oa(a) {
+            return a && "undefined" != typeof a.getElementsByTagName && a
+        }
+        c = fa.support = {}, f = fa.isXML = function(a) {
+            var b = a && (a.ownerDocument || a).documentElement;
+            return b ? "HTML" !== b.nodeName : !1
+        }, m = fa.setDocument = function(a) {
+            var b, e, g = a ? a.ownerDocument || a : v;
+            return g !== n && 9 === g.nodeType && g.documentElement ? (n = g, o = n.documentElement, p = !f(n), (e = n.defaultView) && e.top !== e && (e.addEventListener ? e.addEventListener("unload", da, !1) : e.attachEvent && e.attachEvent("onunload", da)), c.attributes = ia(function(a) {
+                return a.className = "i", !a.getAttribute("className")
+            }), c.getElementsByTagName = ia(function(a) {
+                return a.appendChild(n.createComment("")), !a.getElementsByTagName("*").length
+            }), c.getElementsByClassName = Z.test(n.getElementsByClassName), c.getById = ia(function(a) {
+                return o.appendChild(a).id = u, !n.getElementsByName || !n.getElementsByName(u).length
+            }), c.getById ? (d.find.ID = function(a, b) {
+                if ("undefined" != typeof b.getElementById && p) {
+                    var c = b.getElementById(a);
+                    return c ? [c] : []
+                }
+            }, d.filter.ID = function(a) {
+                var b = a.replace(ba, ca);
+                return function(a) {
+                    return a.getAttribute("id") === b
+                }
+            }) : (delete d.find.ID, d.filter.ID = function(a) {
+                var b = a.replace(ba, ca);
+                return function(a) {
+                    var c = "undefined" != typeof a.getAttributeNode && a.getAttributeNode("id");
+                    return c && c.value === b
+                }
+            }), d.find.TAG = c.getElementsByTagName ? function(a, b) {
+                return "undefined" != typeof b.getElementsByTagName ? b.getElementsByTagName(a) : c.qsa ? b.querySelectorAll(a) : void 0
+            } : function(a, b) {
+                var c, d = [],
+                    e = 0,
+                    f = b.getElementsByTagName(a);
+                if ("*" === a) {
+                    while (c = f[e++]) 1 === c.nodeType && d.push(c);
+                    return d
+                }
+                return f
+            }, d.find.CLASS = c.getElementsByClassName && function(a, b) {
+                return "undefined" != typeof b.getElementsByClassName && p ? b.getElementsByClassName(a) : void 0
+            }, r = [], q = [], (c.qsa = Z.test(n.querySelectorAll)) && (ia(function(a) {
+                o.appendChild(a).innerHTML = "<a id='" + u + "'></a><select id='" + u + "-\r\\' msallowcapture=''><option selected=''></option></select>", a.querySelectorAll("[msallowcapture^='']").length && q.push("[*^$]=" + L + "*(?:''|\"\")"), a.querySelectorAll("[selected]").length || q.push("\\[" + L + "*(?:value|" + K + ")"), a.querySelectorAll("[id~=" + u + "-]").length || q.push("~="), a.querySelectorAll(":checked").length || q.push(":checked"), a.querySelectorAll("a#" + u + "+*").length || q.push(".#.+[+~]")
+            }), ia(function(a) {
+                var b = n.createElement("input");
+                b.setAttribute("type", "hidden"), a.appendChild(b).setAttribute("name", "D"), a.querySelectorAll("[name=d]").length && q.push("name" + L + "*[*^$|!~]?="), a.querySelectorAll(":enabled").length || q.push(":enabled", ":disabled"), a.querySelectorAll("*,:x"), q.push(",.*:")
+            })), (c.matchesSelector = Z.test(s = o.matches || o.webkitMatchesSelector || o.mozMatchesSelector || o.oMatchesSelector || o.msMatchesSelector)) && ia(function(a) {
+                c.disconnectedMatch = s.call(a, "div"), s.call(a, "[s!='']:x"), r.push("!=", O)
+            }), q = q.length && new RegExp(q.join("|")), r = r.length && new RegExp(r.join("|")), b = Z.test(o.compareDocumentPosition), t = b || Z.test(o.contains) ? function(a, b) {
+                var c = 9 === a.nodeType ? a.documentElement : a,
+                    d = b && b.parentNode;
+                return a === d || !(!d || 1 !== d.nodeType || !(c.contains ? c.contains(d) : a.compareDocumentPosition && 16 & a.compareDocumentPosition(d)))
+            } : function(a, b) {
+                if (b)
+                    while (b = b.parentNode)
+                        if (b === a) return !0;
+                return !1
+            }, B = b ? function(a, b) {
+                if (a === b) return l = !0, 0;
+                var d = !a.compareDocumentPosition - !b.compareDocumentPosition;
+                return d ? d : (d = (a.ownerDocument || a) === (b.ownerDocument || b) ? a.compareDocumentPosition(b) : 1, 1 & d || !c.sortDetached && b.compareDocumentPosition(a) === d ? a === n || a.ownerDocument === v && t(v, a) ? -1 : b === n || b.ownerDocument === v && t(v, b) ? 1 : k ? J(k, a) - J(k, b) : 0 : 4 & d ? -1 : 1)
+            } : function(a, b) {
+                if (a === b) return l = !0, 0;
+                var c, d = 0,
+                    e = a.parentNode,
+                    f = b.parentNode,
+                    g = [a],
+                    h = [b];
+                if (!e || !f) return a === n ? -1 : b === n ? 1 : e ? -1 : f ? 1 : k ? J(k, a) - J(k, b) : 0;
+                if (e === f) return ka(a, b);
+                c = a;
+                while (c = c.parentNode) g.unshift(c);
+                c = b;
+                while (c = c.parentNode) h.unshift(c);
+                while (g[d] === h[d]) d++;
+                return d ? ka(g[d], h[d]) : g[d] === v ? -1 : h[d] === v ? 1 : 0
+            }, n) : n
+        }, fa.matches = function(a, b) {
+            return fa(a, null, null, b)
+        }, fa.matchesSelector = function(a, b) {
+            if ((a.ownerDocument || a) !== n && m(a), b = b.replace(T, "='$1']"), c.matchesSelector && p && !A[b + " "] && (!r || !r.test(b)) && (!q || !q.test(b))) try {
+                var d = s.call(a, b);
+                if (d || c.disconnectedMatch || a.document && 11 !== a.document.nodeType) return d
+            } catch (e) {}
+            return fa(b, n, null, [a]).length > 0
+        }, fa.contains = function(a, b) {
+            return (a.ownerDocument || a) !== n && m(a), t(a, b)
+        }, fa.attr = function(a, b) {
+            (a.ownerDocument || a) !== n && m(a);
+            var e = d.attrHandle[b.toLowerCase()],
+                f = e && D.call(d.attrHandle, b.toLowerCase()) ? e(a, b, !p) : void 0;
+            return void 0 !== f ? f : c.attributes || !p ? a.getAttribute(b) : (f = a.getAttributeNode(b)) && f.specified ? f.value : null
+        }, fa.error = function(a) {
+            throw new Error("Syntax error, unrecognized expression: " + a)
+        }, fa.uniqueSort = function(a) {
+            var b, d = [],
+                e = 0,
+                f = 0;
+            if (l = !c.detectDuplicates, k = !c.sortStable && a.slice(0), a.sort(B), l) {
+                while (b = a[f++]) b === a[f] && (e = d.push(f));
+                while (e--) a.splice(d[e], 1)
+            }
+            return k = null, a
+        }, e = fa.getText = function(a) {
+            var b, c = "",
+                d = 0,
+                f = a.nodeType;
+            if (f) {
+                if (1 === f || 9 === f || 11 === f) {
+                    if ("string" == typeof a.textContent) return a.textContent;
+                    for (a = a.firstChild; a; a = a.nextSibling) c += e(a)
+                } else if (3 === f || 4 === f) return a.nodeValue
+            } else
+                while (b = a[d++]) c += e(b);
+            return c
+        }, d = fa.selectors = {
+            cacheLength: 50,
+            createPseudo: ha,
+            match: W,
+            attrHandle: {},
+            find: {},
+            relative: {
+                ">": {
+                    dir: "parentNode",
+                    first: !0
+                },
+                " ": {
+                    dir: "parentNode"
+                },
+                "+": {
+                    dir: "previousSibling",
+                    first: !0
+                },
+                "~": {
+                    dir: "previousSibling"
+                }
+            },
+            preFilter: {
+                ATTR: function(a) {
+                    return a[1] = a[1].replace(ba, ca), a[3] = (a[3] || a[4] || a[5] || "").replace(ba, ca), "~=" === a[2] && (a[3] = " " + a[3] + " "), a.slice(0, 4)
+                },
+                CHILD: function(a) {
+                    return a[1] = a[1].toLowerCase(), "nth" === a[1].slice(0, 3) ? (a[3] || fa.error(a[0]), a[4] = +(a[4] ? a[5] + (a[6] || 1) : 2 * ("even" === a[3] || "odd" === a[3])), a[5] = +(a[7] + a[8] || "odd" === a[3])) : a[3] && fa.error(a[0]), a
+                },
+                PSEUDO: function(a) {
+                    var b, c = !a[6] && a[2];
+                    return W.CHILD.test(a[0]) ? null : (a[3] ? a[2] = a[4] || a[5] || "" : c && U.test(c) && (b = g(c, !0)) && (b = c.indexOf(")", c.length - b) - c.length) && (a[0] = a[0].slice(0, b), a[2] = c.slice(0, b)), a.slice(0, 3))
+                }
+            },
+            filter: {
+                TAG: function(a) {
+                    var b = a.replace(ba, ca).toLowerCase();
+                    return "*" === a ? function() {
+                        return !0
+                    } : function(a) {
+                        return a.nodeName && a.nodeName.toLowerCase() === b
+                    }
+                },
+                CLASS: function(a) {
+                    var b = y[a + " "];
+                    return b || (b = new RegExp("(^|" + L + ")" + a + "(" + L + "|$)")) && y(a, function(a) {
+                        return b.test("string" == typeof a.className && a.className || "undefined" != typeof a.getAttribute && a.getAttribute("class") || "")
+                    })
+                },
+                ATTR: function(a, b, c) {
+                    return function(d) {
+                        var e = fa.attr(d, a);
+                        return null == e ? "!=" === b : b ? (e += "", "=" === b ? e === c : "!=" === b ? e !== c : "^=" === b ? c && 0 === e.indexOf(c) : "*=" === b ? c && e.indexOf(c) > -1 : "$=" === b ? c && e.slice(-c.length) === c : "~=" === b ? (" " + e.replace(P, " ") + " ").indexOf(c) > -1 : "|=" === b ? e === c || e.slice(0, c.length + 1) === c + "-" : !1) : !0
+                    }
+                },
+                CHILD: function(a, b, c, d, e) {
+                    var f = "nth" !== a.slice(0, 3),
+                        g = "last" !== a.slice(-4),
+                        h = "of-type" === b;
+                    return 1 === d && 0 === e ? function(a) {
+                        return !!a.parentNode
+                    } : function(b, c, i) {
+                        var j, k, l, m, n, o, p = f !== g ? "nextSibling" : "previousSibling",
+                            q = b.parentNode,
+                            r = h && b.nodeName.toLowerCase(),
+                            s = !i && !h,
+                            t = !1;
+                        if (q) {
+                            if (f) {
+                                while (p) {
+                                    m = b;
+                                    while (m = m[p])
+                                        if (h ? m.nodeName.toLowerCase() === r : 1 === m.nodeType) return !1;
+                                    o = p = "only" === a && !o && "nextSibling"
+                                }
+                                return !0
                             }
-                            this.context = c, this.selector = a;
-                            return this
+                            if (o = [g ? q.firstChild : q.lastChild], g && s) {
+                                m = q, l = m[u] || (m[u] = {}), k = l[m.uniqueID] || (l[m.uniqueID] = {}), j = k[a] || [], n = j[0] === w && j[1], t = n && j[2], m = n && q.childNodes[n];
+                                while (m = ++n && m && m[p] || (t = n = 0) || o.pop())
+                                    if (1 === m.nodeType && ++t && m === b) {
+                                        k[a] = [w, n, t];
+                                        break
+                                    }
+                            } else if (s && (m = b, l = m[u] || (m[u] = {}), k = l[m.uniqueID] || (l[m.uniqueID] = {}), j = k[a] || [], n = j[0] === w && j[1], t = n), t === !1)
+                                while (m = ++n && m && m[p] || (t = n = 0) || o.pop())
+                                    if ((h ? m.nodeName.toLowerCase() === r : 1 === m.nodeType) && ++t && (s && (l = m[u] || (m[u] = {}), k = l[m.uniqueID] || (l[m.uniqueID] = {}), k[a] = [w, t]), m === b)) break;
+                            return t -= e, t === d || t % d === 0 && t / d >= 0
                         }
-                        return !d || d.jquery ? (d || f).find(a) : this.constructor(d).find(a)
                     }
-                    if (e.isFunction(a)) return f.ready(a);
-                    a.selector !== b && (this.selector = a.selector, this.context = a.context);
-                    return e.makeArray(a, this)
-                },
-                selector: "",
-                jquery: "1.7.1",
-                length: 0,
-                size: function() {
-                    return this.length
-                },
-                toArray: function() {
-                    return F.call(this, 0)
-                },
-                get: function(a) {
-                    return a == null ? this.toArray() : a < 0 ? this[this.length + a] : this[a]
-                },
-                pushStack: function(a, b, c) {
-                    var d = this.constructor();
-                    e.isArray(a) ? E.apply(d, a) : e.merge(d, a), d.prevObject = this, d.context = this.context, b === "find" ? d.selector = this.selector + (this.selector ? " " : "") + c : b && (d.selector = this.selector + "." + b + "(" + c + ")");
-                    return d
-                },
-                each: function(a, b) {
-                    return e.each(this, a, b)
                 },
-                ready: function(a) {
-                    e.bindReady(), A.add(a);
-                    return this
-                },
-                eq: function(a) {
-                    a = +a;
-                    return a === -1 ? this.slice(a) : this.slice(a, a + 1)
-                },
-                first: function() {
-                    return this.eq(0)
-                },
-                last: function() {
-                    return this.eq(-1)
-                },
-                slice: function() {
-                    return this.pushStack(F.apply(this, arguments), "slice", F.call(arguments).join(","))
-                },
-                map: function(a) {
-                    return this.pushStack(e.map(this, function(b, c) {
-                        return a.call(b, c, b)
-                    }))
-                },
-                end: function() {
-                    return this.prevObject || this.constructor(null)
-                },
-                push: E,
-                sort: [].sort,
-                splice: [].splice
-            }, e.fn.init.prototype = e.fn, e.extend = e.fn.extend = function() {
-                var a, c, d, f, g, h, i = arguments[0] || {},
-                    j = 1,
-                    k = arguments.length,
-                    l = !1;
-                typeof i == "boolean" && (l = i, i = arguments[1] || {}, j = 2), typeof i != "object" && !e.isFunction(i) && (i = {}), k === j && (i = this, --j);
-                for (; j < k; j++)
-                    if ((a = arguments[j]) != null)
-                        for (c in a) {
-                            d = i[c], f = a[c];
-                            if (i === f) continue;
-                            l && f && (e.isPlainObject(f) || (g = e.isArray(f))) ? (g ? (g = !1, h = d && e.isArray(d) ? d : []) : h = d && e.isPlainObject(d) ? d : {}, i[c] = e.extend(l, h, f)) : f !== b && (i[c] = f)
+                PSEUDO: function(a, b) {
+                    var c, e = d.pseudos[a] || d.setFilters[a.toLowerCase()] || fa.error("unsupported pseudo: " + a);
+                    return e[u] ? e(b) : e.length > 1 ? (c = [a, a, "", b], d.setFilters.hasOwnProperty(a.toLowerCase()) ? ha(function(a, c) {
+                        var d, f = e(a, b),
+                            g = f.length;
+                        while (g--) d = J(a, f[g]), a[d] = !(c[d] = f[g])
+                    }) : function(a) {
+                        return e(a, 0, c)
+                    }) : e
+                }
+            },
+            pseudos: {
+                not: ha(function(a) {
+                    var b = [],
+                        c = [],
+                        d = h(a.replace(Q, "$1"));
+                    return d[u] ? ha(function(a, b, c, e) {
+                        var f, g = d(a, null, e, []),
+                            h = a.length;
+                        while (h--)(f = g[h]) && (a[h] = !(b[h] = f))
+                    }) : function(a, e, f) {
+                        return b[0] = a, d(b, null, f, c), b[0] = null, !c.pop()
+                    }
+                }),
+                has: ha(function(a) {
+                    return function(b) {
+                        return fa(a, b).length > 0
+                    }
+                }),
+                contains: ha(function(a) {
+                    return a = a.replace(ba, ca),
+                        function(b) {
+                            return (b.textContent || b.innerText || e(b)).indexOf(a) > -1
                         }
-                return i
-            }, e.extend({
-                noConflict: function(b) {
-                    a.$ === e && (a.$ = g), b && a.jQuery === e && (a.jQuery = f);
-                    return e
-                },
-                isReady: !1,
-                readyWait: 1,
-                holdReady: function(a) {
-                    a ? e.readyWait++ : e.ready(!0)
-                },
-                ready: function(a) {
-                    if (a === !0 && !--e.readyWait || a !== !0 && !e.isReady) {
-                        if (!c.body) return setTimeout(e.ready, 1);
-                        e.isReady = !0;
-                        if (a !== !0 && --e.readyWait > 0) return;
-                        A.fireWith(c, [e]), e.fn.trigger && e(c).trigger("ready").off("ready")
-                    }
-                },
-                bindReady: function() {
-                    if (!A) {
-                        A = e.Callbacks("once memory");
-                        if (c.readyState === "complete") return setTimeout(e.ready, 1);
-                        if (c.addEventListener) c.addEventListener("DOMContentLoaded", B, !1), a.addEventListener("load", e.ready, !1);
-                        else if (c.attachEvent) {
-                            c.attachEvent("onreadystatechange", B), a.attachEvent("onload", e.ready);
-                            var b = !1;
-                            try {
-                                b = a.frameElement == null
-                            } catch (d) {}
-                            c.documentElement.doScroll && b && J()
+                }),
+                lang: ha(function(a) {
+                    return V.test(a || "") || fa.error("unsupported lang: " + a), a = a.replace(ba, ca).toLowerCase(),
+                        function(b) {
+                            var c;
+                            do
+                                if (c = p ? b.lang : b.getAttribute("xml:lang") || b.getAttribute("lang")) return c = c.toLowerCase(), c === a || 0 === c.indexOf(a + "-"); while ((b = b.parentNode) && 1 === b.nodeType);
+                            return !1
                         }
-                    }
+                }),
+                target: function(b) {
+                    var c = a.location && a.location.hash;
+                    return c && c.slice(1) === b.id
                 },
-                isFunction: function(a) {
-                    return e.type(a) === "function"
+                root: function(a) {
+                    return a === o
                 },
-                isArray: Array.isArray || function(a) {
-                    return e.type(a) === "array"
+                focus: function(a) {
+                    return a === n.activeElement && (!n.hasFocus || n.hasFocus()) && !!(a.type || a.href || ~a.tabIndex)
                 },
-                isWindow: function(a) {
-                    return a && typeof a == "object" && "setInterval" in a
+                enabled: function(a) {
+                    return a.disabled === !1
                 },
-                isNumeric: function(a) {
-                    return !isNaN(parseFloat(a)) && isFinite(a)
+                disabled: function(a) {
+                    return a.disabled === !0
                 },
-                type: function(a) {
-                    return a == null ? String(a) : I[C.call(a)] || "object"
+                checked: function(a) {
+                    var b = a.nodeName.toLowerCase();
+                    return "input" === b && !!a.checked || "option" === b && !!a.selected
                 },
-                isPlainObject: function(a) {
-                    if (!a || e.type(a) !== "object" || a.nodeType || e.isWindow(a)) return !1;
-                    try {
-                        if (a.constructor && !D.call(a, "constructor") && !D.call(a.constructor.prototype, "isPrototypeOf")) return !1
-                    } catch (c) {
-                        return !1
-                    }
-                    var d;
-                    for (d in a);
-                    return d === b || D.call(a, d)
+                selected: function(a) {
+                    return a.parentNode && a.parentNode.selectedIndex, a.selected === !0
                 },
-                isEmptyObject: function(a) {
-                    for (var b in a) return !1;
+                empty: function(a) {
+                    for (a = a.firstChild; a; a = a.nextSibling)
+                        if (a.nodeType < 6) return !1;
                     return !0
                 },
-                error: function(a) {
-                    throw new Error(a)
+                parent: function(a) {
+                    return !d.pseudos.empty(a)
                 },
-                parseJSON: function(b) {
-                    if (typeof b != "string" || !b) return null;
-                    b = e.trim(b);
-                    if (a.JSON && a.JSON.parse) return a.JSON.parse(b);
-                    if (n.test(b.replace(o, "@").replace(p, "]").replace(q, ""))) return (new Function("return " + b))();
-                    e.error("Invalid JSON: " + b)
+                header: function(a) {
+                    return Y.test(a.nodeName)
                 },
-                parseXML: function(c) {
-                    var d, f;
-                    try {
-                        a.DOMParser ? (f = new DOMParser, d = f.parseFromString(c, "text/xml")) : (d = new ActiveXObject("Microsoft.XMLDOM"), d.async = "false", d.loadXML(c))
-                    } catch (g) {
-                        d = b
-                    }(!d || !d.documentElement || d.getElementsByTagName("parsererror").length) && e.error("Invalid XML: " + c);
-                    return d
+                input: function(a) {
+                    return X.test(a.nodeName)
                 },
-                noop: function() {},
-                globalEval: function(b) {
-                    b && j.test(b) && (a.execScript || function(b) {
-                        a.eval.call(a, b)
-                    })(b)
-                },
-                camelCase: function(a) {
-                    return a.replace(w, "ms-").replace(v, x)
-                },
-                nodeName: function(a, b) {
-                    return a.nodeName && a.nodeName.toUpperCase() === b.toUpperCase()
-                },
-                each: function(a, c, d) {
-                    var f, g = 0,
-                        h = a.length,
-                        i = h === b || e.isFunction(a);
-                    if (d) {
-                        if (i) {
-                            for (f in a)
-                                if (c.apply(a[f], d) === !1) break
-                        } else
-                            for (; g < h;)
-                                if (c.apply(a[g++], d) === !1) break
-                    } else if (i) {
-                        for (f in a)
-                            if (c.call(a[f], f, a[f]) === !1) break
-                    } else
-                        for (; g < h;)
-                            if (c.call(a[g], g, a[g++]) === !1) break;
-                    return a
+                button: function(a) {
+                    var b = a.nodeName.toLowerCase();
+                    return "input" === b && "button" === a.type || "button" === b
                 },
-                trim: G ? function(a) {
-                    return a == null ? "" : G.call(a)
-                } : function(a) {
-                    return a == null ? "" : (a + "").replace(k, "").replace(l, "")
-                },
-                makeArray: function(a, b) {
-                    var c = b || [];
-                    if (a != null) {
-                        var d = e.type(a);
-                        a.length == null || d === "string" || d === "function" || d === "regexp" || e.isWindow(a) ? E.call(c, a) : e.merge(c, a)
-                    }
-                    return c
+                text: function(a) {
+                    var b;
+                    return "input" === a.nodeName.toLowerCase() && "text" === a.type && (null == (b = a.getAttribute("type")) || "text" === b.toLowerCase())
                 },
-                inArray: function(a, b, c) {
-                    var d;
-                    if (b) {
-                        if (H) return H.call(b, a, c);
-                        d = b.length, c = c ? c < 0 ? Math.max(0, d + c) : c : 0;
-                        for (; c < d; c++)
-                            if (c in b && b[c] === a) return c
-                    }
-                    return -1
-                },
-                merge: function(a, c) {
-                    var d = a.length,
-                        e = 0;
-                    if (typeof c.length == "number")
-                        for (var f = c.length; e < f; e++) a[d++] = c[e];
-                    else
-                        while (c[e] !== b) a[d++] = c[e++];
-                    a.length = d;
+                first: na(function() {
+                    return [0]
+                }),
+                last: na(function(a, b) {
+                    return [b - 1]
+                }),
+                eq: na(function(a, b, c) {
+                    return [0 > c ? c + b : c]
+                }),
+                even: na(function(a, b) {
+                    for (var c = 0; b > c; c += 2) a.push(c);
                     return a
-                },
-                grep: function(a, b, c) {
-                    var d = [],
-                        e;
-                    c = !!c;
-                    for (var f = 0, g = a.length; f < g; f++) e = !!b(a[f], f), c !== e && d.push(a[f]);
-                    return d
-                },
-                map: function(a, c, d) {
-                    var f, g, h = [],
-                        i = 0,
-                        j = a.length,
-                        k = a instanceof e || j !== b && typeof j == "number" && (j > 0 && a[0] && a[j - 1] || j === 0 || e.isArray(a));
-                    if (k)
-                        for (; i < j; i++) f = c(a[i], i, d), f != null && (h[h.length] = f);
-                    else
-                        for (g in a) f = c(a[g], g, d), f != null && (h[h.length] = f);
-                    return h.concat.apply([], h)
-                },
-                guid: 1,
-                proxy: function(a, c) {
-                    if (typeof c == "string") {
-                        var d = a[c];
-                        c = a, a = d
-                    }
-                    if (!e.isFunction(a)) return b;
-                    var f = F.call(arguments, 2),
-                        g = function() {
-                            return a.apply(c, f.concat(F.call(arguments)))
-                        };
-                    g.guid = a.guid = a.guid || g.guid || e.guid++;
-                    return g
-                },
-                access: function(a, c, d, f, g, h) {
-                    var i = a.length;
-                    if (typeof c == "object") {
-                        for (var j in c) e.access(a, j, c[j], f, g, d);
-                        return a
-                    }
-                    if (d !== b) {
-                        f = !h && f && e.isFunction(d);
-                        for (var k = 0; k < i; k++) g(a[k], c, f ? d.call(a[k], k, g(a[k], c)) : d, h);
-                        return a
-                    }
-                    return i ? g(a[0], c) : b
-                },
-                now: function() {
-                    return (new Date).getTime()
-                },
-                uaMatch: function(a) {
-                    a = a.toLowerCase();
-                    var b = r.exec(a) || s.exec(a) || t.exec(a) || a.indexOf("compatible") < 0 && u.exec(a) || [];
-                    return {
-                        browser: b[1] || "",
-                        version: b[2] || "0"
-                    }
-                },
-                sub: function() {
-                    function a(b, c) {
-                        return new a.fn.init(b, c)
-                    }
-                    e.extend(!0, a, this), a.superclass = this, a.fn = a.prototype = this(), a.fn.constructor = a, a.sub = this.sub, a.fn.init = function(d, f) {
-                        f && f instanceof e && !(f instanceof a) && (f = a(f));
-                        return e.fn.init.call(this, d, f, b)
-                    }, a.fn.init.prototype = a.fn;
-                    var b = a(c);
+                }),
+                odd: na(function(a, b) {
+                    for (var c = 1; b > c; c += 2) a.push(c);
                     return a
-                },
-                browser: {}
-            }), e.each("Boolean Number String Function Array Date RegExp Object".split(" "), function(a, b) {
-                I["[object " + b + "]"] = b.toLowerCase()
-            }), z = e.uaMatch(y), z.browser && (e.browser[z.browser] = !0, e.browser.version = z.version), e.browser.webkit && (e.browser.safari = !0), j.test(" ") && (k = /^[\s\xA0]+/, l = /[\s\xA0]+$/), h = e(c), c.addEventListener ? B = function() {
-                c.removeEventListener("DOMContentLoaded", B, !1), e.ready()
-            } : c.attachEvent && (B = function() {
-                c.readyState === "complete" && (c.detachEvent("onreadystatechange", B), e.ready())
-            });
-            return e
-        }(),
-        g = {};
-    f.Callbacks = function(a) {
-        a = a ? g[a] || h(a) : {};
-        var c = [],
-            d = [],
-            e, i, j, k, l, m = function(b) {
-                var d, e, g, h, i;
-                for (d = 0, e = b.length; d < e; d++) g = b[d], h = f.type(g), h === "array" ? m(g) : h === "function" && (!a.unique || !o.has(g)) && c.push(g)
-            },
-            n = function(b, f) {
-                f = f || [], e = !a.memory || [b, f], i = !0, l = j || 0, j = 0, k = c.length;
-                for (; c && l < k; l++)
-                    if (c[l].apply(b, f) === !1 && a.stopOnFalse) {
-                        e = !0;
+                }),
+                lt: na(function(a, b, c) {
+                    for (var d = 0 > c ? c + b : c; --d >= 0;) a.push(d);
+                    return a
+                }),
+                gt: na(function(a, b, c) {
+                    for (var d = 0 > c ? c + b : c; ++d < b;) a.push(d);
+                    return a
+                })
+            }
+        }, d.pseudos.nth = d.pseudos.eq;
+        for (b in {
+                radio: !0,
+                checkbox: !0,
+                file: !0,
+                password: !0,
+                image: !0
+            }) d.pseudos[b] = la(b);
+        for (b in {
+                submit: !0,
+                reset: !0
+            }) d.pseudos[b] = ma(b);
+
+        function pa() {}
+        pa.prototype = d.filters = d.pseudos, d.setFilters = new pa, g = fa.tokenize = function(a, b) {
+            var c, e, f, g, h, i, j, k = z[a + " "];
+            if (k) return b ? 0 : k.slice(0);
+            h = a, i = [], j = d.preFilter;
+            while (h) {
+                c && !(e = R.exec(h)) || (e && (h = h.slice(e[0].length) || h), i.push(f = [])), c = !1, (e = S.exec(h)) && (c = e.shift(), f.push({
+                    value: c,
+                    type: e[0].replace(Q, " ")
+                }), h = h.slice(c.length));
+                for (g in d.filter) !(e = W[g].exec(h)) || j[g] && !(e = j[g](e)) || (c = e.shift(), f.push({
+                    value: c,
+                    type: g,
+                    matches: e
+                }), h = h.slice(c.length));
+                if (!c) break
+            }
+            return b ? h.length : h ? fa.error(a) : z(a, i).slice(0)
+        };
+
+        function qa(a) {
+            for (var b = 0, c = a.length, d = ""; c > b; b++) d += a[b].value;
+            return d
+        }
+
+        function ra(a, b, c) {
+            var d = b.dir,
+                e = c && "parentNode" === d,
+                f = x++;
+            return b.first ? function(b, c, f) {
+                while (b = b[d])
+                    if (1 === b.nodeType || e) return a(b, c, f)
+            } : function(b, c, g) {
+                var h, i, j, k = [w, f];
+                if (g) {
+                    while (b = b[d])
+                        if ((1 === b.nodeType || e) && a(b, c, g)) return !0
+                } else
+                    while (b = b[d])
+                        if (1 === b.nodeType || e) {
+                            if (j = b[u] || (b[u] = {}), i = j[b.uniqueID] || (j[b.uniqueID] = {}), (h = i[d]) && h[0] === w && h[1] === f) return k[2] = h[2];
+                            if (i[d] = k, k[2] = a(b, c, g)) return !0
+                        }
+            }
+        }
+
+        function sa(a) {
+            return a.length > 1 ? function(b, c, d) {
+                var e = a.length;
+                while (e--)
+                    if (!a[e](b, c, d)) return !1;
+                return !0
+            } : a[0]
+        }
+
+        function ta(a, b, c) {
+            for (var d = 0, e = b.length; e > d; d++) fa(a, b[d], c);
+            return c
+        }
+
+        function ua(a, b, c, d, e) {
+            for (var f, g = [], h = 0, i = a.length, j = null != b; i > h; h++)(f = a[h]) && (c && !c(f, d, e) || (g.push(f), j && b.push(h)));
+            return g
+        }
+
+        function va(a, b, c, d, e, f) {
+            return d && !d[u] && (d = va(d)), e && !e[u] && (e = va(e, f)), ha(function(f, g, h, i) {
+                var j, k, l, m = [],
+                    n = [],
+                    o = g.length,
+                    p = f || ta(b || "*", h.nodeType ? [h] : h, []),
+                    q = !a || !f && b ? p : ua(p, m, a, h, i),
+                    r = c ? e || (f ? a : o || d) ? [] : g : q;
+                if (c && c(q, r, h, i), d) {
+                    j = ua(r, n), d(j, [], h, i), k = j.length;
+                    while (k--)(l = j[k]) && (r[n[k]] = !(q[n[k]] = l))
+                }
+                if (f) {
+                    if (e || a) {
+                        if (e) {
+                            j = [], k = r.length;
+                            while (k--)(l = r[k]) && j.push(q[k] = l);
+                            e(null, r = [], j, i)
+                        }
+                        k = r.length;
+                        while (k--)(l = r[k]) && (j = e ? J(f, l) : m[k]) > -1 && (f[j] = !(g[j] = l))
+                    }
+                } else r = ua(r === g ? r.splice(o, r.length) : r), e ? e(null, g, r, i) : H.apply(g, r)
+            })
+        }
+
+        function wa(a) {
+            for (var b, c, e, f = a.length, g = d.relative[a[0].type], h = g || d.relative[" "], i = g ? 1 : 0, k = ra(function(a) {
+                    return a === b
+                }, h, !0), l = ra(function(a) {
+                    return J(b, a) > -1
+                }, h, !0), m = [function(a, c, d) {
+                    var e = !g && (d || c !== j) || ((b = c).nodeType ? k(a, c, d) : l(a, c, d));
+                    return b = null, e
+                }]; f > i; i++)
+                if (c = d.relative[a[i].type]) m = [ra(sa(m), c)];
+                else {
+                    if (c = d.filter[a[i].type].apply(null, a[i].matches), c[u]) {
+                        for (e = ++i; f > e; e++)
+                            if (d.relative[a[e].type]) break;
+                        return va(i > 1 && sa(m), i > 1 && qa(a.slice(0, i - 1).concat({
+                            value: " " === a[i - 2].type ? "*" : ""
+                        })).replace(Q, "$1"), c, e > i && wa(a.slice(i, e)), f > e && wa(a = a.slice(e)), f > e && qa(a))
+                    }
+                    m.push(c)
+                } return sa(m)
+        }
+
+        function xa(a, b) {
+            var c = b.length > 0,
+                e = a.length > 0,
+                f = function(f, g, h, i, k) {
+                    var l, o, q, r = 0,
+                        s = "0",
+                        t = f && [],
+                        u = [],
+                        v = j,
+                        x = f || e && d.find.TAG("*", k),
+                        y = w += null == v ? 1 : Math.random() || .1,
+                        z = x.length;
+                    for (k && (j = g === n || g || k); s !== z && null != (l = x[s]); s++) {
+                        if (e && l) {
+                            o = 0, g || l.ownerDocument === n || (m(l), h = !p);
+                            while (q = a[o++])
+                                if (q(l, g || n, h)) {
+                                    i.push(l);
+                                    break
+                                } k && (w = y)
+                        }
+                        c && ((l = !q && l) && r--, f && t.push(l))
+                    }
+                    if (r += s, c && s !== r) {
+                        o = 0;
+                        while (q = b[o++]) q(t, u, g, h);
+                        if (f) {
+                            if (r > 0)
+                                while (s--) t[s] || u[s] || (u[s] = F.call(i));
+                            u = ua(u)
+                        }
+                        H.apply(i, u), k && !f && u.length > 0 && r + b.length > 1 && fa.uniqueSort(i)
+                    }
+                    return k && (w = y, j = v), t
+                };
+            return c ? ha(f) : f
+        }
+        return h = fa.compile = function(a, b) {
+            var c, d = [],
+                e = [],
+                f = A[a + " "];
+            if (!f) {
+                b || (b = g(a)), c = b.length;
+                while (c--) f = wa(b[c]), f[u] ? d.push(f) : e.push(f);
+                f = A(a, xa(e, d)), f.selector = a
+            }
+            return f
+        }, i = fa.select = function(a, b, e, f) {
+            var i, j, k, l, m, n = "function" == typeof a && a,
+                o = !f && g(a = n.selector || a);
+            if (e = e || [], 1 === o.length) {
+                if (j = o[0] = o[0].slice(0), j.length > 2 && "ID" === (k = j[0]).type && c.getById && 9 === b.nodeType && p && d.relative[j[1].type]) {
+                    if (b = (d.find.ID(k.matches[0].replace(ba, ca), b) || [])[0], !b) return e;
+                    n && (b = b.parentNode), a = a.slice(j.shift().value.length)
+                }
+                i = W.needsContext.test(a) ? 0 : j.length;
+                while (i--) {
+                    if (k = j[i], d.relative[l = k.type]) break;
+                    if ((m = d.find[l]) && (f = m(k.matches[0].replace(ba, ca), _.test(j[0].type) && oa(b.parentNode) || b))) {
+                        if (j.splice(i, 1), a = f.length && qa(j), !a) return H.apply(e, f), e;
                         break
-                    } i = !1, c && (a.once ? e === !0 ? o.disable() : c = [] : d && d.length && (e = d.shift(), o.fireWith(e[0], e[1])))
-            },
-            o = {
-                add: function() {
-                    if (c) {
-                        var a = c.length;
-                        m(arguments), i ? k = c.length : e && e !== !0 && (j = a, n(e[0], e[1]))
                     }
+                }
+            }
+            return (n || h(a, o))(f, b, !p, e, !b || _.test(a) && oa(b.parentNode) || b), e
+        }, c.sortStable = u.split("").sort(B).join("") === u, c.detectDuplicates = !!l, m(), c.sortDetached = ia(function(a) {
+            return 1 & a.compareDocumentPosition(n.createElement("div"))
+        }), ia(function(a) {
+            return a.innerHTML = "<a href='#'></a>", "#" === a.firstChild.getAttribute("href")
+        }) || ja("type|href|height|width", function(a, b, c) {
+            return c ? void 0 : a.getAttribute(b, "type" === b.toLowerCase() ? 1 : 2)
+        }), c.attributes && ia(function(a) {
+            return a.innerHTML = "<input/>", a.firstChild.setAttribute("value", ""), "" === a.firstChild.getAttribute("value")
+        }) || ja("value", function(a, b, c) {
+            return c || "input" !== a.nodeName.toLowerCase() ? void 0 : a.defaultValue
+        }), ia(function(a) {
+            return null == a.getAttribute("disabled")
+        }) || ja(K, function(a, b, c) {
+            var d;
+            return c ? void 0 : a[b] === !0 ? b.toLowerCase() : (d = a.getAttributeNode(b)) && d.specified ? d.value : null
+        }), fa
+    }(a);
+    n.find = t, n.expr = t.selectors, n.expr[":"] = n.expr.pseudos, n.uniqueSort = n.unique = t.uniqueSort, n.text = t.getText, n.isXMLDoc = t.isXML, n.contains = t.contains;
+    var u = function(a, b, c) {
+            var d = [],
+                e = void 0 !== c;
+            while ((a = a[b]) && 9 !== a.nodeType)
+                if (1 === a.nodeType) {
+                    if (e && n(a).is(c)) break;
+                    d.push(a)
+                } return d
+        },
+        v = function(a, b) {
+            for (var c = []; a; a = a.nextSibling) 1 === a.nodeType && a !== b && c.push(a);
+            return c
+        },
+        w = n.expr.match.needsContext,
+        x = /^<([\w-]+)\s*\/?>(?:<\/\1>|)$/,
+        y = /^.[^:#\[\.,]*$/;
+
+    function z(a, b, c) {
+        if (n.isFunction(b)) return n.grep(a, function(a, d) {
+            return !!b.call(a, d, a) !== c
+        });
+        if (b.nodeType) return n.grep(a, function(a) {
+            return a === b !== c
+        });
+        if ("string" == typeof b) {
+            if (y.test(b)) return n.filter(b, a, c);
+            b = n.filter(b, a)
+        }
+        return n.grep(a, function(a) {
+            return h.call(b, a) > -1 !== c
+        })
+    }
+    n.filter = function(a, b, c) {
+        var d = b[0];
+        return c && (a = ":not(" + a + ")"), 1 === b.length && 1 === d.nodeType ? n.find.matchesSelector(d, a) ? [d] : [] : n.find.matches(a, n.grep(b, function(a) {
+            return 1 === a.nodeType
+        }))
+    }, n.fn.extend({
+        find: function(a) {
+            var b, c = this.length,
+                d = [],
+                e = this;
+            if ("string" != typeof a) return this.pushStack(n(a).filter(function() {
+                for (b = 0; c > b; b++)
+                    if (n.contains(e[b], this)) return !0
+            }));
+            for (b = 0; c > b; b++) n.find(a, e[b], d);
+            return d = this.pushStack(c > 1 ? n.unique(d) : d), d.selector = this.selector ? this.selector + " " + a : a, d
+        },
+        filter: function(a) {
+            return this.pushStack(z(this, a || [], !1))
+        },
+        not: function(a) {
+            return this.pushStack(z(this, a || [], !0))
+        },
+        is: function(a) {
+            return !!z(this, "string" == typeof a && w.test(a) ? n(a) : a || [], !1).length
+        }
+    });
+    var A, B = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]*))$/,
+        C = n.fn.init = function(a, b, c) {
+            var e, f;
+            if (!a) return this;
+            if (c = c || A, "string" == typeof a) {
+                if (e = "<" === a[0] && ">" === a[a.length - 1] && a.length >= 3 ? [null, a, null] : B.exec(a), !e || !e[1] && b) return !b || b.jquery ? (b || c).find(a) : this.constructor(b).find(a);
+                if (e[1]) {
+                    if (b = b instanceof n ? b[0] : b, n.merge(this, n.parseHTML(e[1], b && b.nodeType ? b.ownerDocument || b : d, !0)), x.test(e[1]) && n.isPlainObject(b))
+                        for (e in b) n.isFunction(this[e]) ? this[e](b[e]) : this.attr(e, b[e]);
                     return this
+                }
+                return f = d.getElementById(e[2]), f && f.parentNode && (this.length = 1, this[0] = f), this.context = d, this.selector = a, this
+            }
+            return a.nodeType ? (this.context = this[0] = a, this.length = 1, this) : n.isFunction(a) ? void 0 !== c.ready ? c.ready(a) : a(n) : (void 0 !== a.selector && (this.selector = a.selector, this.context = a.context), n.makeArray(a, this))
+        };
+    C.prototype = n.fn, A = n(d);
+    var D = /^(?:parents|prev(?:Until|All))/,
+        E = {
+            children: !0,
+            contents: !0,
+            next: !0,
+            prev: !0
+        };
+    n.fn.extend({
+        has: function(a) {
+            var b = n(a, this),
+                c = b.length;
+            return this.filter(function() {
+                for (var a = 0; c > a; a++)
+                    if (n.contains(this, b[a])) return !0
+            })
+        },
+        closest: function(a, b) {
+            for (var c, d = 0, e = this.length, f = [], g = w.test(a) || "string" != typeof a ? n(a, b || this.context) : 0; e > d; d++)
+                for (c = this[d]; c && c !== b; c = c.parentNode)
+                    if (c.nodeType < 11 && (g ? g.index(c) > -1 : 1 === c.nodeType && n.find.matchesSelector(c, a))) {
+                        f.push(c);
+                        break
+                    } return this.pushStack(f.length > 1 ? n.uniqueSort(f) : f)
+        },
+        index: function(a) {
+            return a ? "string" == typeof a ? h.call(n(a), this[0]) : h.call(this, a.jquery ? a[0] : a) : this[0] && this[0].parentNode ? this.first().prevAll().length : -1
+        },
+        add: function(a, b) {
+            return this.pushStack(n.uniqueSort(n.merge(this.get(), n(a, b))))
+        },
+        addBack: function(a) {
+            return this.add(null == a ? this.prevObject : this.prevObject.filter(a))
+        }
+    });
+
+    function F(a, b) {
+        while ((a = a[b]) && 1 !== a.nodeType);
+        return a
+    }
+    n.each({
+        parent: function(a) {
+            var b = a.parentNode;
+            return b && 11 !== b.nodeType ? b : null
+        },
+        parents: function(a) {
+            return u(a, "parentNode")
+        },
+        parentsUntil: function(a, b, c) {
+            return u(a, "parentNode", c)
+        },
+        next: function(a) {
+            return F(a, "nextSibling")
+        },
+        prev: function(a) {
+            return F(a, "previousSibling")
+        },
+        nextAll: function(a) {
+            return u(a, "nextSibling")
+        },
+        prevAll: function(a) {
+            return u(a, "previousSibling")
+        },
+        nextUntil: function(a, b, c) {
+            return u(a, "nextSibling", c)
+        },
+        prevUntil: function(a, b, c) {
+            return u(a, "previousSibling", c)
+        },
+        siblings: function(a) {
+            return v((a.parentNode || {}).firstChild, a)
+        },
+        children: function(a) {
+            return v(a.firstChild)
+        },
+        contents: function(a) {
+            return a.contentDocument || n.merge([], a.childNodes)
+        }
+    }, function(a, b) {
+        n.fn[a] = function(c, d) {
+            var e = n.map(this, b, c);
+            return "Until" !== a.slice(-5) && (d = c), d && "string" == typeof d && (e = n.filter(d, e)), this.length > 1 && (E[a] || n.uniqueSort(e), D.test(a) && e.reverse()), this.pushStack(e)
+        }
+    });
+    var G = /\S+/g;
+
+    function H(a) {
+        var b = {};
+        return n.each(a.match(G) || [], function(a, c) {
+            b[c] = !0
+        }), b
+    }
+    n.Callbacks = function(a) {
+        a = "string" == typeof a ? H(a) : n.extend({}, a);
+        var b, c, d, e, f = [],
+            g = [],
+            h = -1,
+            i = function() {
+                for (e = a.once, d = b = !0; g.length; h = -1) {
+                    c = g.shift();
+                    while (++h < f.length) f[h].apply(c[0], c[1]) === !1 && a.stopOnFalse && (h = f.length, c = !1)
+                }
+                a.memory || (c = !1), b = !1, e && (f = c ? [] : "")
+            },
+            j = {
+                add: function() {
+                    return f && (c && !b && (h = f.length - 1, g.push(c)), function d(b) {
+                        n.each(b, function(b, c) {
+                            n.isFunction(c) ? a.unique && j.has(c) || f.push(c) : c && c.length && "string" !== n.type(c) && d(c)
+                        })
+                    }(arguments), c && !b && i()), this
                 },
                 remove: function() {
-                    if (c) {
-                        var b = arguments,
-                            d = 0,
-                            e = b.length;
-                        for (; d < e; d++)
-                            for (var f = 0; f < c.length; f++)
-                                if (b[d] === c[f]) {
-                                    i && f <= k && (k--, f <= l && l--), c.splice(f--, 1);
-                                    if (a.unique) break
-                                }
-                    }
-                    return this
+                    return n.each(arguments, function(a, b) {
+                        var c;
+                        while ((c = n.inArray(b, f, c)) > -1) f.splice(c, 1), h >= c && h--
+                    }), this
                 },
                 has: function(a) {
-                    if (c) {
-                        var b = 0,
-                            d = c.length;
-                        for (; b < d; b++)
-                            if (a === c[b]) return !0
-                    }
-                    return !1
+                    return a ? n.inArray(a, f) > -1 : f.length > 0
                 },
                 empty: function() {
-                    c = [];
-                    return this
+                    return f && (f = []), this
                 },
                 disable: function() {
-                    c = d = e = b;
-                    return this
+                    return e = g = [], f = c = "", this
                 },
                 disabled: function() {
-                    return !c
+                    return !f
                 },
                 lock: function() {
-                    d = b, (!e || e === !0) && o.disable();
-                    return this
+                    return e = g = [], c || (f = c = ""), this
                 },
                 locked: function() {
-                    return !d
+                    return !!e
                 },
-                fireWith: function(b, c) {
-                    d && (i ? a.once || d.push([b, c]) : (!a.once || !e) && n(b, c));
-                    return this
+                fireWith: function(a, c) {
+                    return e || (c = c || [], c = [a, c.slice ? c.slice() : c], g.push(c), b || i()), this
                 },
                 fire: function() {
-                    o.fireWith(this, arguments);
-                    return this
+                    return j.fireWith(this, arguments), this
                 },
                 fired: function() {
-                    return !!e
+                    return !!d
                 }
             };
-        return o
-    };
-    var i = [].slice;
-    f.extend({
+        return j
+    }, n.extend({
         Deferred: function(a) {
-            var b = f.Callbacks("once memory"),
-                c = f.Callbacks("once memory"),
-                d = f.Callbacks("memory"),
-                e = "pending",
-                g = {
-                    resolve: b,
-                    reject: c,
-                    notify: d
-                },
-                h = {
-                    done: b.add,
-                    fail: c.add,
-                    progress: d.add,
+            var b = [
+                    ["resolve", "done", n.Callbacks("once memory"), "resolved"],
+                    ["reject", "fail", n.Callbacks("once memory"), "rejected"],
+                    ["notify", "progress", n.Callbacks("memory")]
+                ],
+                c = "pending",
+                d = {
                     state: function() {
-                        return e
-                    },
-                    isResolved: b.fired,
-                    isRejected: c.fired,
-                    then: function(a, b, c) {
-                        i.done(a).fail(b).progress(c);
-                        return this
+                        return c
                     },
                     always: function() {
-                        i.done.apply(i, arguments).fail.apply(i, arguments);
-                        return this
+                        return e.done(arguments).fail(arguments), this
                     },
-                    pipe: function(a, b, c) {
-                        return f.Deferred(function(d) {
-                            f.each({
-                                done: [a, "resolve"],
-                                fail: [b, "reject"],
-                                progress: [c, "notify"]
-                            }, function(a, b) {
-                                var c = b[0],
-                                    e = b[1],
-                                    g;
-                                f.isFunction(c) ? i[a](function() {
-                                    g = c.apply(this, arguments), g && f.isFunction(g.promise) ? g.promise().then(d.resolve, d.reject, d.notify) : d[e + "With"](this === i ? d : this, [g])
-                                }) : i[a](d[e])
-                            })
+                    then: function() {
+                        var a = arguments;
+                        return n.Deferred(function(c) {
+                            n.each(b, function(b, f) {
+                                var g = n.isFunction(a[b]) && a[b];
+                                e[f[1]](function() {
+                                    var a = g && g.apply(this, arguments);
+                                    a && n.isFunction(a.promise) ? a.promise().progress(c.notify).done(c.resolve).fail(c.reject) : c[f[0] + "With"](this === d ? c.promise() : this, g ? [a] : arguments)
+                                })
+                            }), a = null
                         }).promise()
                     },
                     promise: function(a) {
-                        if (a == null) a = h;
-                        else
-                            for (var b in h) a[b] = h[b];
-                        return a
+                        return null != a ? n.extend(a, d) : d
                     }
                 },
-                i = h.promise({}),
-                j;
-            for (j in g) i[j] = g[j].fire, i[j + "With"] = g[j].fireWith;
-            i.done(function() {
-                e = "resolved"
-            }, c.disable, d.lock).fail(function() {
-                e = "rejected"
-            }, b.disable, d.lock), a && a.call(i, i);
-            return i
+                e = {};
+            return d.pipe = d.then, n.each(b, function(a, f) {
+                var g = f[2],
+                    h = f[3];
+                d[f[1]] = g.add, h && g.add(function() {
+                    c = h
+                }, b[1 ^ a][2].disable, b[2][2].lock), e[f[0]] = function() {
+                    return e[f[0] + "With"](this === e ? d : this, arguments), this
+                }, e[f[0] + "With"] = g.fireWith
+            }), d.promise(e), a && a.call(e, e), e
         },
         when: function(a) {
-            function m(a) {
-                return function(b) {
-                    e[a] = arguments.length > 1 ? i.call(arguments, 0) : b, j.notifyWith(k, e)
-                }
-            }
+            var b = 0,
+                c = e.call(arguments),
+                d = c.length,
+                f = 1 !== d || a && n.isFunction(a.promise) ? d : 0,
+                g = 1 === f ? a : n.Deferred(),
+                h = function(a, b, c) {
+                    return function(d) {
+                        b[a] = this, c[a] = arguments.length > 1 ? e.call(arguments) : d, c === i ? g.notifyWith(b, c) : --f || g.resolveWith(b, c)
+                    }
+                },
+                i, j, k;
+            if (d > 1)
+                for (i = new Array(d), j = new Array(d), k = new Array(d); d > b; b++) c[b] && n.isFunction(c[b].promise) ? c[b].promise().progress(h(b, j, i)).done(h(b, k, c)).fail(g.reject) : --f;
+            return f || g.resolveWith(k, c), g.promise()
+        }
+    });
+    var I;
+    n.fn.ready = function(a) {
+        return n.ready.promise().done(a), this
+    }, n.extend({
+        isReady: !1,
+        readyWait: 1,
+        holdReady: function(a) {
+            a ? n.readyWait++ : n.ready(!0)
+        },
+        ready: function(a) {
+            (a === !0 ? --n.readyWait : n.isReady) || (n.isReady = !0, a !== !0 && --n.readyWait > 0 || (I.resolveWith(d, [n]), n.fn.triggerHandler && (n(d).triggerHandler("ready"), n(d).off("ready"))))
+        }
+    });
 
-            function l(a) {
-                return function(c) {
-                    b[a] = arguments.length > 1 ? i.call(arguments, 0) : c, --g || j.resolveWith(j, b)
-                }
-            }
-            var b = i.call(arguments, 0),
-                c = 0,
-                d = b.length,
-                e = Array(d),
-                g = d,
-                h = d,
-                j = d <= 1 && a && f.isFunction(a.promise) ? a : f.Deferred(),
-                k = j.promise();
-            if (d > 1) {
-                for (; c < d; c++) b[c] && b[c].promise && f.isFunction(b[c].promise) ? b[c].promise().then(l(c), j.reject, m(c)) : --g;
-                g || j.resolveWith(j, b)
-            } else j !== a && j.resolveWith(j, d ? [a] : []);
-            return k
-        }
-    }), f.support = function() {
-        var b, d, e, g, h, i, j, k, l, m, n, o, p, q = c.createElement("div"),
-            r = c.documentElement;
-        q.setAttribute("className", "t"), q.innerHTML = "   <link/><table></table><a href='/a' style='top:1px;float:left;opacity:.55;'>a</a><input type='checkbox'/>", d = q.getElementsByTagName("*"), e = q.getElementsByTagName("a")[0];
-        if (!d || !d.length || !e) return {};
-        g = c.createElement("select"), h = g.appendChild(c.createElement("option")), i = q.getElementsByTagName("input")[0], b = {
-            leadingWhitespace: q.firstChild.nodeType === 3,
-            tbody: !q.getElementsByTagName("tbody").length,
-            htmlSerialize: !!q.getElementsByTagName("link").length,
-            style: /top/.test(e.getAttribute("style")),
-            hrefNormalized: e.getAttribute("href") === "/a",
-            opacity: /^0.55/.test(e.style.opacity),
-            cssFloat: !!e.style.cssFloat,
-            checkOn: i.value === "on",
-            optSelected: h.selected,
-            getSetAttribute: q.className !== "t",
-            enctype: !!c.createElement("form").enctype,
-            html5Clone: c.createElement("nav").cloneNode(!0).outerHTML !== "<:nav></:nav>",
-            submitBubbles: !0,
-            changeBubbles: !0,
-            focusinBubbles: !1,
-            deleteExpando: !0,
-            noCloneEvent: !0,
-            inlineBlockNeedsLayout: !1,
-            shrinkWrapBlocks: !1,
-            reliableMarginRight: !0
-        }, i.checked = !0, b.noCloneChecked = i.cloneNode(!0).checked, g.disabled = !0, b.optDisabled = !h.disabled;
-        try {
-            delete q.test
-        } catch (s) {
-            b.deleteExpando = !1
-        }!q.addEventListener && q.attachEvent && q.fireEvent && (q.attachEvent("onclick", function() {
-            b.noCloneEvent = !1
-        }), q.cloneNode(!0).fireEvent("onclick")), i = c.createElement("input"), i.value = "t", i.setAttribute("type", "radio"), b.radioValue = i.value === "t", i.setAttribute("checked", "checked"), q.appendChild(i), k = c.createDocumentFragment(), k.appendChild(q.lastChild), b.checkClone = k.cloneNode(!0).cloneNode(!0).lastChild.checked, b.appendChecked = i.checked, k.removeChild(i), k.appendChild(q), q.innerHTML = "", a.getComputedStyle && (j = c.createElement("div"), j.style.width = "0", j.style.marginRight = "0", q.style.width = "2px", q.appendChild(j), b.reliableMarginRight = (parseInt((a.getComputedStyle(j, null) || {
-            marginRight: 0
-        }).marginRight, 10) || 0) === 0);
-        if (q.attachEvent)
-            for (o in {
-                    submit: 1,
-                    change: 1,
-                    focusin: 1
-                }) n = "on" + o, p = n in q, p || (q.setAttribute(n, "return;"), p = typeof q[n] == "function"), b[o + "Bubbles"] = p;
-        k.removeChild(q), k = g = h = j = q = i = null, f(function() {
-            var a, d, e, g, h, i, j, k, m, n, o, r = c.getElementsByTagName("body")[0];
-            !r || (j = 1, k = "position:absolute;top:0;left:0;width:1px;height:1px;margin:0;", m = "visibility:hidden;border:0;", n = "style='" + k + "border:5px solid #000;padding:0;'", o = "<div " + n + "><div></div></div>" + "<table " + n + " cellpadding='0' cellspacing='0'>" + "<tr><td></td></tr></table>", a = c.createElement("div"), a.style.cssText = m + "width:0;height:0;position:static;top:0;margin-top:" + j + "px", r.insertBefore(a, r.firstChild), q = c.createElement("div"), a.appendChild(q), q.innerHTML = "<table><tr><td style='padding:0;border:0;display:none'></td><td>t</td></tr></table>", l = q.getElementsByTagName("td"), p = l[0].offsetHeight === 0, l[0].style.display = "", l[1].style.display = "none", b.reliableHiddenOffsets = p && l[0].offsetHeight === 0, q.innerHTML = "", q.style.width = q.style.paddingLeft = "1px", f.boxModel = b.boxModel = q.offsetWidth === 2, typeof q.style.zoom != "undefined" && (q.style.display = "inline", q.style.zoom = 1, b.inlineBlockNeedsLayout = q.offsetWidth === 2, q.style.display = "", q.innerHTML = "<div style='width:4px;'></div>", b.shrinkWrapBlocks = q.offsetWidth !== 2), q.style.cssText = k + m, q.innerHTML = o, d = q.firstChild, e = d.firstChild, h = d.nextSibling.firstChild.firstChild, i = {
-                doesNotAddBorder: e.offsetTop !== 5,
-                doesAddBorderForTableAndCells: h.offsetTop === 5
-            }, e.style.position = "fixed", e.style.top = "20px", i.fixedPosition = e.offsetTop === 20 || e.offsetTop === 15, e.style.position = e.style.top = "", d.style.overflow = "hidden", d.style.position = "relative", i.subtractsBorderForOverflowNotVisible = e.offsetTop === -5, i.doesNotIncludeMarginInBodyOffset = r.offsetTop !== j, r.removeChild(a), q = a = null, f.extend(b, i))
-        });
-        return b
-    }();
-    var j = /^(?:\{.*\}|\[.*\])$/,
-        k = /([A-Z])/g;
-    f.extend({
-        cache: {},
-        uuid: 0,
-        expando: "jQuery" + (f.fn.jquery + Math.random()).replace(/\D/g, ""),
-        noData: {
-            embed: !0,
-            object: "clsid:D27CDB6E-AE6D-11cf-96B8-444553540000",
-            applet: !0
+    function J() {
+        d.removeEventListener("DOMContentLoaded", J), a.removeEventListener("load", J), n.ready()
+    }
+    n.ready.promise = function(b) {
+        return I || (I = n.Deferred(), "complete" === d.readyState || "loading" !== d.readyState && !d.documentElement.doScroll ? a.setTimeout(n.ready) : (d.addEventListener("DOMContentLoaded", J), a.addEventListener("load", J))), I.promise(b)
+    }, n.ready.promise();
+    var K = function(a, b, c, d, e, f, g) {
+            var h = 0,
+                i = a.length,
+                j = null == c;
+            if ("object" === n.type(c)) {
+                e = !0;
+                for (h in c) K(a, b, h, c[h], !0, f, g)
+            } else if (void 0 !== d && (e = !0, n.isFunction(d) || (g = !0), j && (g ? (b.call(a, d), b = null) : (j = b, b = function(a, b, c) {
+                    return j.call(n(a), c)
+                })), b))
+                for (; i > h; h++) b(a[h], c, g ? d : d.call(a[h], h, b(a[h], c)));
+            return e ? a : j ? b.call(a) : i ? b(a[0], c) : f
         },
-        hasData: function(a) {
-            a = a.nodeType ? f.cache[a[f.expando]] : a[f.expando];
-            return !!a && !m(a)
+        L = function(a) {
+            return 1 === a.nodeType || 9 === a.nodeType || !+a.nodeType
+        };
+
+    function M() {
+        this.expando = n.expando + M.uid++
+    }
+    M.uid = 1, M.prototype = {
+        register: function(a, b) {
+            var c = b || {};
+            return a.nodeType ? a[this.expando] = c : Object.defineProperty(a, this.expando, {
+                value: c,
+                writable: !0,
+                configurable: !0
+            }), a[this.expando]
+        },
+        cache: function(a) {
+            if (!L(a)) return {};
+            var b = a[this.expando];
+            return b || (b = {}, L(a) && (a.nodeType ? a[this.expando] = b : Object.defineProperty(a, this.expando, {
+                value: b,
+                configurable: !0
+            }))), b
         },
-        data: function(a, c, d, e) {
-            if (!!f.acceptData(a)) {
-                var g, h, i, j = f.expando,
-                    k = typeof c == "string",
-                    l = a.nodeType,
-                    m = l ? f.cache : a,
-                    n = l ? a[j] : a[j] && j,
-                    o = c === "events";
-                if ((!n || !m[n] || !o && !e && !m[n].data) && k && d === b) return;
-                n || (l ? a[j] = n = ++f.uuid : n = j), m[n] || (m[n] = {}, l || (m[n].toJSON = f.noop));
-                if (typeof c == "object" || typeof c == "function") e ? m[n] = f.extend(m[n], c) : m[n].data = f.extend(m[n].data, c);
-                g = h = m[n], e || (h.data || (h.data = {}), h = h.data), d !== b && (h[f.camelCase(c)] = d);
-                if (o && !h[c]) return g.events;
-                k ? (i = h[c], i == null && (i = h[f.camelCase(c)])) : i = h;
-                return i
-            }
-        },
-        removeData: function(a, b, c) {
-            if (!!f.acceptData(a)) {
-                var d, e, g, h = f.expando,
-                    i = a.nodeType,
-                    j = i ? f.cache : a,
-                    k = i ? a[h] : h;
-                if (!j[k]) return;
-                if (b) {
-                    d = c ? j[k] : j[k].data;
-                    if (d) {
-                        f.isArray(b) || (b in d ? b = [b] : (b = f.camelCase(b), b in d ? b = [b] : b = b.split(" ")));
-                        for (e = 0, g = b.length; e < g; e++) delete d[b[e]];
-                        if (!(c ? m : f.isEmptyObject)(d)) return
-                    }
-                }
-                if (!c) {
-                    delete j[k].data;
-                    if (!m(j[k])) return
-                }
-                f.support.deleteExpando || !j.setInterval ? delete j[k] : j[k] = null, i && (f.support.deleteExpando ? delete a[h] : a.removeAttribute ? a.removeAttribute(h) : a[h] = null)
+        set: function(a, b, c) {
+            var d, e = this.cache(a);
+            if ("string" == typeof b) e[b] = c;
+            else
+                for (d in b) e[d] = b[d];
+            return e
+        },
+        get: function(a, b) {
+            return void 0 === b ? this.cache(a) : a[this.expando] && a[this.expando][b]
+        },
+        access: function(a, b, c) {
+            var d;
+            return void 0 === b || b && "string" == typeof b && void 0 === c ? (d = this.get(a, b), void 0 !== d ? d : this.get(a, n.camelCase(b))) : (this.set(a, b, c), void 0 !== c ? c : b)
+        },
+        remove: function(a, b) {
+            var c, d, e, f = a[this.expando];
+            if (void 0 !== f) {
+                if (void 0 === b) this.register(a);
+                else {
+                    n.isArray(b) ? d = b.concat(b.map(n.camelCase)) : (e = n.camelCase(b), b in f ? d = [b, e] : (d = e, d = d in f ? [d] : d.match(G) || [])), c = d.length;
+                    while (c--) delete f[d[c]]
+                }(void 0 === b || n.isEmptyObject(f)) && (a.nodeType ? a[this.expando] = void 0 : delete a[this.expando])
             }
         },
+        hasData: function(a) {
+            var b = a[this.expando];
+            return void 0 !== b && !n.isEmptyObject(b)
+        }
+    };
+    var N = new M,
+        O = new M,
+        P = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
+        Q = /[A-Z]/g;
+
+    function R(a, b, c) {
+        var d;
+        if (void 0 === c && 1 === a.nodeType)
+            if (d = "data-" + b.replace(Q, "-$&").toLowerCase(), c = a.getAttribute(d), "string" == typeof c) {
+                try {
+                    c = "true" === c ? !0 : "false" === c ? !1 : "null" === c ? null : +c + "" === c ? +c : P.test(c) ? n.parseJSON(c) : c;
+                } catch (e) {}
+                O.set(a, b, c)
+            } else c = void 0;
+        return c
+    }
+    n.extend({
+        hasData: function(a) {
+            return O.hasData(a) || N.hasData(a)
+        },
+        data: function(a, b, c) {
+            return O.access(a, b, c)
+        },
+        removeData: function(a, b) {
+            O.remove(a, b)
+        },
         _data: function(a, b, c) {
-            return f.data(a, b, c, !0)
+            return N.access(a, b, c)
         },
-        acceptData: function(a) {
-            if (a.nodeName) {
-                var b = f.noData[a.nodeName.toLowerCase()];
-                if (b) return b !== !0 && a.getAttribute("classid") === b
-            }
-            return !0
+        _removeData: function(a, b) {
+            N.remove(a, b)
         }
-    }), f.fn.extend({
-        data: function(a, c) {
-            var d, e, g, h = null;
-            if (typeof a == "undefined") {
-                if (this.length) {
-                    h = f.data(this[0]);
-                    if (this[0].nodeType === 1 && !f._data(this[0], "parsedAttrs")) {
-                        e = this[0].attributes;
-                        for (var i = 0, j = e.length; i < j; i++) g = e[i].name, g.indexOf("data-") === 0 && (g = f.camelCase(g.substring(5)), l(this[0], g, h[g]));
-                        f._data(this[0], "parsedAttrs", !0)
-                    }
+    }), n.fn.extend({
+        data: function(a, b) {
+            var c, d, e, f = this[0],
+                g = f && f.attributes;
+            if (void 0 === a) {
+                if (this.length && (e = O.get(f), 1 === f.nodeType && !N.get(f, "hasDataAttrs"))) {
+                    c = g.length;
+                    while (c--) g[c] && (d = g[c].name, 0 === d.indexOf("data-") && (d = n.camelCase(d.slice(5)), R(f, d, e[d])));
+                    N.set(f, "hasDataAttrs", !0)
                 }
-                return h
-            }
-            if (typeof a == "object") return this.each(function() {
-                f.data(this, a)
-            });
-            d = a.split("."), d[1] = d[1] ? "." + d[1] : "";
-            if (c === b) {
-                h = this.triggerHandler("getData" + d[1] + "!", [d[0]]), h === b && this.length && (h = f.data(this[0], a), h = l(this[0], a, h));
-                return h === b && d[1] ? this.data(d[0]) : h
+                return e
             }
-            return this.each(function() {
-                var b = f(this),
-                    e = [d[0], c];
-                b.triggerHandler("setData" + d[1] + "!", e), f.data(this, a, c), b.triggerHandler("changeData" + d[1] + "!", e)
-            })
+            return "object" == typeof a ? this.each(function() {
+                O.set(this, a)
+            }) : K(this, function(b) {
+                var c, d;
+                if (f && void 0 === b) {
+                    if (c = O.get(f, a) || O.get(f, a.replace(Q, "-$&").toLowerCase()), void 0 !== c) return c;
+                    if (d = n.camelCase(a), c = O.get(f, d), void 0 !== c) return c;
+                    if (c = R(f, d, void 0), void 0 !== c) return c
+                } else d = n.camelCase(a), this.each(function() {
+                    var c = O.get(this, d);
+                    O.set(this, d, b), a.indexOf("-") > -1 && void 0 !== c && O.set(this, a, b)
+                })
+            }, null, b, arguments.length > 1, null, !0)
         },
         removeData: function(a) {
             return this.each(function() {
-                f.removeData(this, a)
+                O.remove(this, a)
             })
         }
-    }), f.extend({
-        _mark: function(a, b) {
-            a && (b = (b || "fx") + "mark", f._data(a, b, (f._data(a, b) || 0) + 1))
-        },
-        _unmark: function(a, b, c) {
-            a !== !0 && (c = b, b = a, a = !1);
-            if (b) {
-                c = c || "fx";
-                var d = c + "mark",
-                    e = a ? 0 : (f._data(b, d) || 1) - 1;
-                e ? f._data(b, d, e) : (f.removeData(b, d, !0), n(b, c, "mark"))
-            }
-        },
+    }), n.extend({
         queue: function(a, b, c) {
             var d;
-            if (a) {
-                b = (b || "fx") + "queue", d = f._data(a, b), c && (!d || f.isArray(c) ? d = f._data(a, b, f.makeArray(c)) : d.push(c));
-                return d || []
-            }
+            return a ? (b = (b || "fx") + "queue", d = N.get(a, b), c && (!d || n.isArray(c) ? d = N.access(a, b, n.makeArray(c)) : d.push(c)), d || []) : void 0
         },
         dequeue: function(a, b) {
             b = b || "fx";
-            var c = f.queue(a, b),
-                d = c.shift(),
-                e = {};
-            d === "inprogress" && (d = c.shift()), d && (b === "fx" && c.unshift("inprogress"), f._data(a, b + ".run", e), d.call(a, function() {
-                f.dequeue(a, b)
-            }, e)), c.length || (f.removeData(a, b + "queue " + b + ".run", !0), n(a, b, "queue"))
-        }
-    }), f.fn.extend({
-        queue: function(a, c) {
-            typeof a != "string" && (c = a, a = "fx");
-            if (c === b) return f.queue(this[0], a);
-            return this.each(function() {
-                var b = f.queue(this, a, c);
-                a === "fx" && b[0] !== "inprogress" && f.dequeue(this, a)
+            var c = n.queue(a, b),
+                d = c.length,
+                e = c.shift(),
+                f = n._queueHooks(a, b),
+                g = function() {
+                    n.dequeue(a, b)
+                };
+            "inprogress" === e && (e = c.shift(), d--), e && ("fx" === b && c.unshift("inprogress"), delete f.stop, e.call(a, g, f)), !d && f && f.empty.fire()
+        },
+        _queueHooks: function(a, b) {
+            var c = b + "queueHooks";
+            return N.get(a, c) || N.access(a, c, {
+                empty: n.Callbacks("once memory").add(function() {
+                    N.remove(a, [b + "queue", c])
+                })
+            })
+        }
+    }), n.fn.extend({
+        queue: function(a, b) {
+            var c = 2;
+            return "string" != typeof a && (b = a, a = "fx", c--), arguments.length < c ? n.queue(this[0], a) : void 0 === b ? this : this.each(function() {
+                var c = n.queue(this, a, b);
+                n._queueHooks(this, a), "fx" === a && "inprogress" !== c[0] && n.dequeue(this, a)
             })
         },
         dequeue: function(a) {
             return this.each(function() {
-                f.dequeue(this, a)
-            })
-        },
-        delay: function(a, b) {
-            a = f.fx ? f.fx.speeds[a] || a : a, b = b || "fx";
-            return this.queue(b, function(b, c) {
-                var d = setTimeout(b, a);
-                c.stop = function() {
-                    clearTimeout(d)
-                }
+                n.dequeue(this, a)
             })
         },
         clearQueue: function(a) {
             return this.queue(a || "fx", [])
         },
-        promise: function(a, c) {
-            function m() {
-                --h || d.resolveWith(e, [e])
-            }
-            typeof a != "string" && (c = a, a = b), a = a || "fx";
-            var d = f.Deferred(),
-                e = this,
-                g = e.length,
-                h = 1,
-                i = a + "defer",
-                j = a + "queue",
-                k = a + "mark",
-                l;
-            while (g--)
-                if (l = f.data(e[g], i, b, !0) || (f.data(e[g], j, b, !0) || f.data(e[g], k, b, !0)) && f.data(e[g], i, f.Callbacks("once memory"), !0)) h++, l.add(m);
-            m();
-            return d.promise()
+        promise: function(a, b) {
+            var c, d = 1,
+                e = n.Deferred(),
+                f = this,
+                g = this.length,
+                h = function() {
+                    --d || e.resolveWith(f, [f])
+                };
+            "string" != typeof a && (b = a, a = void 0), a = a || "fx";
+            while (g--) c = N.get(f[g], a + "queueHooks"), c && c.empty && (d++, c.empty.add(h));
+            return h(), e.promise(b)
         }
     });
-    var o = /[\n\t\r]/g,
-        p = /\s+/,
-        q = /\r/g,
-        r = /^(?:button|input)$/i,
-        s = /^(?:button|input|object|select|textarea)$/i,
-        t = /^a(?:rea)?$/i,
-        u = /^(?:autofocus|autoplay|async|checked|controls|defer|disabled|hidden|loop|multiple|open|readonly|required|scoped|selected)$/i,
-        v = f.support.getSetAttribute,
-        w, x, y;
-    f.fn.extend({
-        attr: function(a, b) {
-            return f.access(this, a, b, !0, f.attr)
-        },
-        removeAttr: function(a) {
-            return this.each(function() {
-                f.removeAttr(this, a)
-            })
-        },
-        prop: function(a, b) {
-            return f.access(this, a, b, !0, f.prop)
-        },
-        removeProp: function(a) {
-            a = f.propFix[a] || a;
-            return this.each(function() {
-                try {
-                    this[a] = b, delete this[a]
-                } catch (c) {}
-            })
-        },
-        addClass: function(a) {
-            var b, c, d, e, g, h, i;
-            if (f.isFunction(a)) return this.each(function(b) {
-                f(this).addClass(a.call(this, b, this.className))
-            });
-            if (a && typeof a == "string") {
-                b = a.split(p);
-                for (c = 0, d = this.length; c < d; c++) {
-                    e = this[c];
-                    if (e.nodeType === 1)
-                        if (!e.className && b.length === 1) e.className = a;
-                        else {
-                            g = " " + e.className + " ";
-                            for (h = 0, i = b.length; h < i; h++) ~g.indexOf(" " + b[h] + " ") || (g += b[h] + " ");
-                            e.className = f.trim(g)
-                        }
-                }
-            }
-            return this
-        },
-        removeClass: function(a) {
-            var c, d, e, g, h, i, j;
-            if (f.isFunction(a)) return this.each(function(b) {
-                f(this).removeClass(a.call(this, b, this.className))
-            });
-            if (a && typeof a == "string" || a === b) {
-                c = (a || "").split(p);
-                for (d = 0, e = this.length; d < e; d++) {
-                    g = this[d];
-                    if (g.nodeType === 1 && g.className)
-                        if (a) {
-                            h = (" " + g.className + " ").replace(o, " ");
-                            for (i = 0, j = c.length; i < j; i++) h = h.replace(" " + c[i] + " ", " ");
-                            g.className = f.trim(h)
-                        } else g.className = ""
-                }
-            }
-            return this
-        },
-        toggleClass: function(a, b) {
-            var c = typeof a,
-                d = typeof b == "boolean";
-            if (f.isFunction(a)) return this.each(function(c) {
-                f(this).toggleClass(a.call(this, c, this.className, b), b)
-            });
-            return this.each(function() {
-                if (c === "string") {
-                    var e, g = 0,
-                        h = f(this),
-                        i = b,
-                        j = a.split(p);
-                    while (e = j[g++]) i = d ? i : !h.hasClass(e), h[i ? "addClass" : "removeClass"](e)
-                } else if (c === "undefined" || c === "boolean") this.className && f._data(this, "__className__", this.className), this.className = this.className || a === !1 ? "" : f._data(this, "__className__") || ""
-            })
-        },
-        hasClass: function(a) {
-            var b = " " + a + " ",
-                c = 0,
-                d = this.length;
-            for (; c < d; c++)
-                if (this[c].nodeType === 1 && (" " + this[c].className + " ").replace(o, " ").indexOf(b) > -1) return !0;
-            return !1
-        },
-        val: function(a) {
-            var c, d, e, g = this[0]; {
-                if (!!arguments.length) {
-                    e = f.isFunction(a);
-                    return this.each(function(d) {
-                        var g = f(this),
-                            h;
-                        if (this.nodeType === 1) {
-                            e ? h = a.call(this, d, g.val()) : h = a, h == null ? h = "" : typeof h == "number" ? h += "" : f.isArray(h) && (h = f.map(h, function(a) {
-                                return a == null ? "" : a + ""
-                            })), c = f.valHooks[this.nodeName.toLowerCase()] || f.valHooks[this.type];
-                            if (!c || !("set" in c) || c.set(this, h, "value") === b) this.value = h
-                        }
-                    })
-                }
-                if (g) {
-                    c = f.valHooks[g.nodeName.toLowerCase()] || f.valHooks[g.type];
-                    if (c && "get" in c && (d = c.get(g, "value")) !== b) return d;
-                    d = g.value;
-                    return typeof d == "string" ? d.replace(q, "") : d == null ? "" : d
-                }
-            }
-        }
-    }), f.extend({
-        valHooks: {
-            option: {
-                get: function(a) {
-                    var b = a.attributes.value;
-                    return !b || b.specified ? a.value : a.text
-                }
-            },
-            select: {
-                get: function(a) {
-                    var b, c, d, e, g = a.selectedIndex,
-                        h = [],
-                        i = a.options,
-                        j = a.type === "select-one";
-                    if (g < 0) return null;
-                    c = j ? g : 0, d = j ? g + 1 : i.length;
-                    for (; c < d; c++) {
-                        e = i[c];
-                        if (e.selected && (f.support.optDisabled ? !e.disabled : e.getAttribute("disabled") === null) && (!e.parentNode.disabled || !f.nodeName(e.parentNode, "optgroup"))) {
-                            b = f(e).val();
-                            if (j) return b;
-                            h.push(b)
-                        }
-                    }
-                    if (j && !h.length && i.length) return f(i[g]).val();
-                    return h
-                },
-                set: function(a, b) {
-                    var c = f.makeArray(b);
-                    f(a).find("option").each(function() {
-                        this.selected = f.inArray(f(this).val(), c) >= 0
-                    }), c.length || (a.selectedIndex = -1);
-                    return c
-                }
-            }
-        },
-        attrFn: {
-            val: !0,
-            css: !0,
-            html: !0,
-            text: !0,
-            data: !0,
-            width: !0,
-            height: !0,
-            offset: !0
-        },
-        attr: function(a, c, d, e) {
-            var g, h, i, j = a.nodeType;
-            if (!!a && j !== 3 && j !== 8 && j !== 2) {
-                if (e && c in f.attrFn) return f(a)[c](d);
-                if (typeof a.getAttribute == "undefined") return f.prop(a, c, d);
-                i = j !== 1 || !f.isXMLDoc(a), i && (c = c.toLowerCase(), h = f.attrHooks[c] || (u.test(c) ? x : w));
-                if (d !== b) {
-                    if (d === null) {
-                        f.removeAttr(a, c);
-                        return
-                    }
-                    if (h && "set" in h && i && (g = h.set(a, d, c)) !== b) return g;
-                    a.setAttribute(c, "" + d);
-                    return d
-                }
-                if (h && "get" in h && i && (g = h.get(a, c)) !== null) return g;
-                g = a.getAttribute(c);
-                return g === null ? b : g
-            }
-        },
-        removeAttr: function(a, b) {
-            var c, d, e, g, h = 0;
-            if (b && a.nodeType === 1) {
-                d = b.toLowerCase().split(p), g = d.length;
-                for (; h < g; h++) e = d[h], e && (c = f.propFix[e] || e, f.attr(a, e, ""), a.removeAttribute(v ? e : c), u.test(e) && c in a && (a[c] = !1))
-            }
-        },
-        attrHooks: {
-            type: {
-                set: function(a, b) {
-                    if (r.test(a.nodeName) && a.parentNode) f.error("type property can't be changed");
-                    else if (!f.support.radioValue && b === "radio" && f.nodeName(a, "input")) {
-                        var c = a.value;
-                        a.setAttribute("type", b), c && (a.value = c);
-                        return b
-                    }
-                }
-            },
-            value: {
-                get: function(a, b) {
-                    if (w && f.nodeName(a, "button")) return w.get(a, b);
-                    return b in a ? a.value : null
-                },
-                set: function(a, b, c) {
-                    if (w && f.nodeName(a, "button")) return w.set(a, b, c);
-                    a.value = b
-                }
-            }
-        },
-        propFix: {
-            tabindex: "tabIndex",
-            readonly: "readOnly",
-            "for": "htmlFor",
-            "class": "className",
-            maxlength: "maxLength",
-            cellspacing: "cellSpacing",
-            cellpadding: "cellPadding",
-            rowspan: "rowSpan",
-            colspan: "colSpan",
-            usemap: "useMap",
-            frameborder: "frameBorder",
-            contenteditable: "contentEditable"
-        },
-        prop: function(a, c, d) {
-            var e, g, h, i = a.nodeType;
-            if (!!a && i !== 3 && i !== 8 && i !== 2) {
-                h = i !== 1 || !f.isXMLDoc(a), h && (c = f.propFix[c] || c, g = f.propHooks[c]);
-                return d !== b ? g && "set" in g && (e = g.set(a, d, c)) !== b ? e : a[c] = d : g && "get" in g && (e = g.get(a, c)) !== null ? e : a[c]
-            }
-        },
-        propHooks: {
-            tabIndex: {
-                get: function(a) {
-                    var c = a.getAttributeNode("tabindex");
-                    return c && c.specified ? parseInt(c.value, 10) : s.test(a.nodeName) || t.test(a.nodeName) && a.href ? 0 : b
-                }
-            }
+    var S = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
+        T = new RegExp("^(?:([+-])=|)(" + S + ")([a-z%]*)$", "i"),
+        U = ["Top", "Right", "Bottom", "Left"],
+        V = function(a, b) {
+            return a = b || a, "none" === n.css(a, "display") || !n.contains(a.ownerDocument, a)
+        };
+
+    function W(a, b, c, d) {
+        var e, f = 1,
+            g = 20,
+            h = d ? function() {
+                return d.cur()
+            } : function() {
+                return n.css(a, b, "")
+            },
+            i = h(),
+            j = c && c[3] || (n.cssNumber[b] ? "" : "px"),
+            k = (n.cssNumber[b] || "px" !== j && +i) && T.exec(n.css(a, b));
+        if (k && k[3] !== j) {
+            j = j || k[3], c = c || [], k = +i || 1;
+            do f = f || ".5", k /= f, n.style(a, b, k + j); while (f !== (f = h() / i) && 1 !== f && --g)
+        }
+        return c && (k = +k || +i || 0, e = c[1] ? k + (c[1] + 1) * c[2] : +c[2], d && (d.unit = j, d.start = k, d.end = e)), e
+    }
+    var X = /^(?:checkbox|radio)$/i,
+        Y = /<([\w:-]+)/,
+        Z = /^$|\/(?:java|ecma)script/i,
+        $ = {
+            option: [1, "<select multiple='multiple'>", "</select>"],
+            thead: [1, "<table>", "</table>"],
+            col: [2, "<table><colgroup>", "</colgroup></table>"],
+            tr: [2, "<table><tbody>", "</tbody></table>"],
+            td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
+            _default: [0, "", ""]
+        };
+    $.optgroup = $.option, $.tbody = $.tfoot = $.colgroup = $.caption = $.thead, $.th = $.td;
+
+    function _(a, b) {
+        var c = "undefined" != typeof a.getElementsByTagName ? a.getElementsByTagName(b || "*") : "undefined" != typeof a.querySelectorAll ? a.querySelectorAll(b || "*") : [];
+        return void 0 === b || b && n.nodeName(a, b) ? n.merge([a], c) : c
+    }
+
+    function aa(a, b) {
+        for (var c = 0, d = a.length; d > c; c++) N.set(a[c], "globalEval", !b || N.get(b[c], "globalEval"))
+    }
+    var ba = /<|&#?\w+;/;
+
+    function ca(a, b, c, d, e) {
+        for (var f, g, h, i, j, k, l = b.createDocumentFragment(), m = [], o = 0, p = a.length; p > o; o++)
+            if (f = a[o], f || 0 === f)
+                if ("object" === n.type(f)) n.merge(m, f.nodeType ? [f] : f);
+                else if (ba.test(f)) {
+            g = g || l.appendChild(b.createElement("div")), h = (Y.exec(f) || ["", ""])[1].toLowerCase(), i = $[h] || $._default, g.innerHTML = i[1] + n.htmlPrefilter(f) + i[2], k = i[0];
+            while (k--) g = g.lastChild;
+            n.merge(m, g.childNodes), g = l.firstChild, g.textContent = ""
+        } else m.push(b.createTextNode(f));
+        l.textContent = "", o = 0;
+        while (f = m[o++])
+            if (d && n.inArray(f, d) > -1) e && e.push(f);
+            else if (j = n.contains(f.ownerDocument, f), g = _(l.appendChild(f), "script"), j && aa(g), c) {
+            k = 0;
+            while (f = g[k++]) Z.test(f.type || "") && c.push(f)
         }
-    }), f.attrHooks.tabindex = f.propHooks.tabIndex, x = {
-        get: function(a, c) {
-            var d, e = f.prop(a, c);
-            return e === !0 || typeof e != "boolean" && (d = a.getAttributeNode(c)) && d.nodeValue !== !1 ? c.toLowerCase() : b
-        },
-        set: function(a, b, c) {
-            var d;
-            b === !1 ? f.removeAttr(a, c) : (d = f.propFix[c] || c, d in a && (a[d] = !0), a.setAttribute(c, c.toLowerCase()));
-            return c
+        return l
+    }! function() {
+        var a = d.createDocumentFragment(),
+            b = a.appendChild(d.createElement("div")),
+            c = d.createElement("input");
+        c.setAttribute("type", "radio"), c.setAttribute("checked", "checked"), c.setAttribute("name", "t"), b.appendChild(c), l.checkClone = b.cloneNode(!0).cloneNode(!0).lastChild.checked, b.innerHTML = "<textarea>x</textarea>", l.noCloneChecked = !!b.cloneNode(!0).lastChild.defaultValue
+    }();
+    var da = /^key/,
+        ea = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
+        fa = /^([^.]*)(?:\.(.+)|)/;
+
+    function ga() {
+        return !0
+    }
+
+    function ha() {
+        return !1
+    }
+
+    function ia() {
+        try {
+            return d.activeElement
+        } catch (a) {}
+    }
+
+    function ja(a, b, c, d, e, f) {
+        var g, h;
+        if ("object" == typeof b) {
+            "string" != typeof c && (d = d || c, c = void 0);
+            for (h in b) ja(a, h, c, d, b[h], f);
+            return a
         }
-    }, v || (y = {
-        name: !0,
-        id: !0
-    }, w = f.valHooks.button = {
-        get: function(a, c) {
-            var d;
-            d = a.getAttributeNode(c);
-            return d && (y[c] ? d.nodeValue !== "" : d.specified) ? d.nodeValue : b
-        },
-        set: function(a, b, d) {
-            var e = a.getAttributeNode(d);
-            e || (e = c.createAttribute(d), a.setAttributeNode(e));
-            return e.nodeValue = b + ""
-        }
-    }, f.attrHooks.tabindex.set = w.set, f.each(["width", "height"], function(a, b) {
-        f.attrHooks[b] = f.extend(f.attrHooks[b], {
-            set: function(a, c) {
-                if (c === "") {
-                    a.setAttribute(b, "auto");
-                    return c
-                }
-            }
+        if (null == d && null == e ? (e = c, d = c = void 0) : null == e && ("string" == typeof c ? (e = d, d = void 0) : (e = d, d = c, c = void 0)), e === !1) e = ha;
+        else if (!e) return a;
+        return 1 === f && (g = e, e = function(a) {
+            return n().off(a), g.apply(this, arguments)
+        }, e.guid = g.guid || (g.guid = n.guid++)), a.each(function() {
+            n.event.add(this, b, e, d, c)
         })
-    }), f.attrHooks.contenteditable = {
-        get: w.get,
-        set: function(a, b, c) {
-            b === "" && (b = "false"), w.set(a, b, c)
-        }
-    }), f.support.hrefNormalized || f.each(["href", "src", "width", "height"], function(a, c) {
-        f.attrHooks[c] = f.extend(f.attrHooks[c], {
-            get: function(a) {
-                var d = a.getAttribute(c, 2);
-                return d === null ? b : d
+    }
+    n.event = {
+        global: {},
+        add: function(a, b, c, d, e) {
+            var f, g, h, i, j, k, l, m, o, p, q, r = N.get(a);
+            if (r) {
+                c.handler && (f = c, c = f.handler, e = f.selector), c.guid || (c.guid = n.guid++), (i = r.events) || (i = r.events = {}), (g = r.handle) || (g = r.handle = function(b) {
+                    return "undefined" != typeof n && n.event.triggered !== b.type ? n.event.dispatch.apply(a, arguments) : void 0
+                }), b = (b || "").match(G) || [""], j = b.length;
+                while (j--) h = fa.exec(b[j]) || [], o = q = h[1], p = (h[2] || "").split(".").sort(), o && (l = n.event.special[o] || {}, o = (e ? l.delegateType : l.bindType) || o, l = n.event.special[o] || {}, k = n.extend({
+                    type: o,
+                    origType: q,
+                    data: d,
+                    handler: c,
+                    guid: c.guid,
+                    selector: e,
+                    needsContext: e && n.expr.match.needsContext.test(e),
+                    namespace: p.join(".")
+                }, f), (m = i[o]) || (m = i[o] = [], m.delegateCount = 0, l.setup && l.setup.call(a, d, p, g) !== !1 || a.addEventListener && a.addEventListener(o, g)), l.add && (l.add.call(a, k), k.handler.guid || (k.handler.guid = c.guid)), e ? m.splice(m.delegateCount++, 0, k) : m.push(k), n.event.global[o] = !0)
+            }
+        },
+        remove: function(a, b, c, d, e) {
+            var f, g, h, i, j, k, l, m, o, p, q, r = N.hasData(a) && N.get(a);
+            if (r && (i = r.events)) {
+                b = (b || "").match(G) || [""], j = b.length;
+                while (j--)
+                    if (h = fa.exec(b[j]) || [], o = q = h[1], p = (h[2] || "").split(".").sort(), o) {
+                        l = n.event.special[o] || {}, o = (d ? l.delegateType : l.bindType) || o, m = i[o] || [], h = h[2] && new RegExp("(^|\\.)" + p.join("\\.(?:.*\\.|)") + "(\\.|$)"), g = f = m.length;
+                        while (f--) k = m[f], !e && q !== k.origType || c && c.guid !== k.guid || h && !h.test(k.namespace) || d && d !== k.selector && ("**" !== d || !k.selector) || (m.splice(f, 1), k.selector && m.delegateCount--, l.remove && l.remove.call(a, k));
+                        g && !m.length && (l.teardown && l.teardown.call(a, p, r.handle) !== !1 || n.removeEvent(a, o, r.handle), delete i[o])
+                    } else
+                        for (o in i) n.event.remove(a, o + b[j], c, d, !0);
+                n.isEmptyObject(i) && N.remove(a, "handle events")
             }
-        })
-    }), f.support.style || (f.attrHooks.style = {
-        get: function(a) {
-            return a.style.cssText.toLowerCase() || b
         },
-        set: function(a, b) {
-            return a.style.cssText = "" + b
-        }
-    }), f.support.optSelected || (f.propHooks.selected = f.extend(f.propHooks.selected, {
-        get: function(a) {
-            var b = a.parentNode;
-            b && (b.selectedIndex, b.parentNode && b.parentNode.selectedIndex);
-            return null
-        }
-    })), f.support.enctype || (f.propFix.enctype = "encoding"), f.support.checkOn || f.each(["radio", "checkbox"], function() {
-        f.valHooks[this] = {
-            get: function(a) {
-                return a.getAttribute("value") === null ? "on" : a.value
+        dispatch: function(a) {
+            a = n.event.fix(a);
+            var b, c, d, f, g, h = [],
+                i = e.call(arguments),
+                j = (N.get(this, "events") || {})[a.type] || [],
+                k = n.event.special[a.type] || {};
+            if (i[0] = a, a.delegateTarget = this, !k.preDispatch || k.preDispatch.call(this, a) !== !1) {
+                h = n.event.handlers.call(this, a, j), b = 0;
+                while ((f = h[b++]) && !a.isPropagationStopped()) {
+                    a.currentTarget = f.elem, c = 0;
+                    while ((g = f.handlers[c++]) && !a.isImmediatePropagationStopped()) a.rnamespace && !a.rnamespace.test(g.namespace) || (a.handleObj = g, a.data = g.data, d = ((n.event.special[g.origType] || {}).handle || g.handler).apply(f.elem, i), void 0 !== d && (a.result = d) === !1 && (a.preventDefault(), a.stopPropagation()))
+                }
+                return k.postDispatch && k.postDispatch.call(this, a), a.result
+            }
+        },
+        handlers: function(a, b) {
+            var c, d, e, f, g = [],
+                h = b.delegateCount,
+                i = a.target;
+            if (h && i.nodeType && ("click" !== a.type || isNaN(a.button) || a.button < 1))
+                for (; i !== this; i = i.parentNode || this)
+                    if (1 === i.nodeType && (i.disabled !== !0 || "click" !== a.type)) {
+                        for (d = [], c = 0; h > c; c++) f = b[c], e = f.selector + " ", void 0 === d[e] && (d[e] = f.needsContext ? n(e, this).index(i) > -1 : n.find(e, this, null, [i]).length), d[e] && d.push(f);
+                        d.length && g.push({
+                            elem: i,
+                            handlers: d
+                        })
+                    } return h < b.length && g.push({
+                elem: this,
+                handlers: b.slice(h)
+            }), g
+        },
+        props: "altKey bubbles cancelable ctrlKey currentTarget detail eventPhase metaKey relatedTarget shiftKey target timeStamp view which".split(" "),
+        fixHooks: {},
+        keyHooks: {
+            props: "char charCode key keyCode".split(" "),
+            filter: function(a, b) {
+                return null == a.which && (a.which = null != b.charCode ? b.charCode : b.keyCode), a
+            }
+        },
+        mouseHooks: {
+            props: "button buttons clientX clientY offsetX offsetY pageX pageY screenX screenY toElement".split(" "),
+            filter: function(a, b) {
+                var c, e, f, g = b.button;
+                return null == a.pageX && null != b.clientX && (c = a.target.ownerDocument || d, e = c.documentElement, f = c.body, a.pageX = b.clientX + (e && e.scrollLeft || f && f.scrollLeft || 0) - (e && e.clientLeft || f && f.clientLeft || 0), a.pageY = b.clientY + (e && e.scrollTop || f && f.scrollTop || 0) - (e && e.clientTop || f && f.clientTop || 0)), a.which || void 0 === g || (a.which = 1 & g ? 1 : 2 & g ? 3 : 4 & g ? 2 : 0), a
+            }
+        },
+        fix: function(a) {
+            if (a[n.expando]) return a;
+            var b, c, e, f = a.type,
+                g = a,
+                h = this.fixHooks[f];
+            h || (this.fixHooks[f] = h = ea.test(f) ? this.mouseHooks : da.test(f) ? this.keyHooks : {}), e = h.props ? this.props.concat(h.props) : this.props, a = new n.Event(g), b = e.length;
+            while (b--) c = e[b], a[c] = g[c];
+            return a.target || (a.target = d), 3 === a.target.nodeType && (a.target = a.target.parentNode), h.filter ? h.filter(a, g) : a
+        },
+        special: {
+            load: {
+                noBubble: !0
+            },
+            focus: {
+                trigger: function() {
+                    return this !== ia() && this.focus ? (this.focus(), !1) : void 0
+                },
+                delegateType: "focusin"
+            },
+            blur: {
+                trigger: function() {
+                    return this === ia() && this.blur ? (this.blur(), !1) : void 0
+                },
+                delegateType: "focusout"
+            },
+            click: {
+                trigger: function() {
+                    return "checkbox" === this.type && this.click && n.nodeName(this, "input") ? (this.click(), !1) : void 0
+                },
+                _default: function(a) {
+                    return n.nodeName(a.target, "a")
+                }
+            },
+            beforeunload: {
+                postDispatch: function(a) {
+                    void 0 !== a.result && a.originalEvent && (a.originalEvent.returnValue = a.result)
+                }
+            }
+        }
+    }, n.removeEvent = function(a, b, c) {
+        a.removeEventListener && a.removeEventListener(b, c)
+    }, n.Event = function(a, b) {
+        return this instanceof n.Event ? (a && a.type ? (this.originalEvent = a, this.type = a.type, this.isDefaultPrevented = a.defaultPrevented || void 0 === a.defaultPrevented && a.returnValue === !1 ? ga : ha) : this.type = a, b && n.extend(this, b), this.timeStamp = a && a.timeStamp || n.now(), void(this[n.expando] = !0)) : new n.Event(a, b)
+    }, n.Event.prototype = {
+        constructor: n.Event,
+        isDefaultPrevented: ha,
+        isPropagationStopped: ha,
+        isImmediatePropagationStopped: ha,
+        isSimulated: !1,
+        preventDefault: function() {
+            var a = this.originalEvent;
+            this.isDefaultPrevented = ga, a && !this.isSimulated && a.preventDefault()
+        },
+        stopPropagation: function() {
+            var a = this.originalEvent;
+            this.isPropagationStopped = ga, a && !this.isSimulated && a.stopPropagation()
+        },
+        stopImmediatePropagation: function() {
+            var a = this.originalEvent;
+            this.isImmediatePropagationStopped = ga, a && !this.isSimulated && a.stopImmediatePropagation(), this.stopPropagation()
+        }
+    }, n.each({
+        mouseenter: "mouseover",
+        mouseleave: "mouseout",
+        pointerenter: "pointerover",
+        pointerleave: "pointerout"
+    }, function(a, b) {
+        n.event.special[a] = {
+            delegateType: b,
+            bindType: b,
+            handle: function(a) {
+                var c, d = this,
+                    e = a.relatedTarget,
+                    f = a.handleObj;
+                return e && (e === d || n.contains(d, e)) || (a.type = f.origType, c = f.handler.apply(this, arguments), a.type = b), c
             }
         }
-    }), f.each(["radio", "checkbox"], function() {
-        f.valHooks[this] = f.extend(f.valHooks[this], {
-            set: function(a, b) {
-                if (f.isArray(b)) return a.checked = f.inArray(f(a).val(), b) >= 0
-            }
-        })
-    });
-    var z = /^(?:textarea|input|select)$/i,
-        A = /^([^\.]*)?(?:\.(.+))?$/,
-        B = /\bhover(\.\S+)?\b/,
-        C = /^key/,
-        D = /^(?:mouse|contextmenu)|click/,
-        E = /^(?:focusinfocus|focusoutblur)$/,
-        F = /^(\w*)(?:#([\w\-]+))?(?:\.([\w\-]+))?$/,
-        G = function(a) {
-            var b = F.exec(a);
-            b && (b[1] = (b[1] || "").toLowerCase(), b[3] = b[3] && new RegExp("(?:^|\\s)" + b[3] + "(?:\\s|$)"));
-            return b
+    }), n.fn.extend({
+        on: function(a, b, c, d) {
+            return ja(this, a, b, c, d)
         },
-        H = function(a, b) {
-            var c = a.attributes || {};
-            return (!b[1] || a.nodeName.toLowerCase() === b[1]) && (!b[2] || (c.id || {}).value === b[2]) && (!b[3] || b[3].test((c["class"] || {}).value))
+        one: function(a, b, c, d) {
+            return ja(this, a, b, c, d, 1)
         },
-        I = function(a) {
-            return f.event.special.hover ? a : a.replace(B, "mouseenter$1 mouseleave$1")
-        };
-    f.event = {
-            add: function(a, c, d, e, g) {
-                var h, i, j, k, l, m, n, o, p, q, r, s;
-                if (!(a.nodeType === 3 || a.nodeType === 8 || !c || !d || !(h = f._data(a)))) {
-                    d.handler && (p = d, d = p.handler), d.guid || (d.guid = f.guid++), j = h.events, j || (h.events = j = {}), i = h.handle, i || (h.handle = i = function(a) {
-                        return typeof f != "undefined" && (!a || f.event.triggered !== a.type) ? f.event.dispatch.apply(i.elem, arguments) : b
-                    }, i.elem = a), c = f.trim(I(c)).split(" ");
-                    for (k = 0; k < c.length; k++) {
-                        l = A.exec(c[k]) || [], m = l[1], n = (l[2] || "").split(".").sort(), s = f.event.special[m] || {}, m = (g ? s.delegateType : s.bindType) || m, s = f.event.special[m] || {}, o = f.extend({
-                            type: m,
-                            origType: l[1],
-                            data: e,
-                            handler: d,
-                            guid: d.guid,
-                            selector: g,
-                            quick: G(g),
-                            namespace: n.join(".")
-                        }, p), r = j[m];
-                        if (!r) {
-                            r = j[m] = [], r.delegateCount = 0;
-                            if (!s.setup || s.setup.call(a, e, n, i) === !1) a.addEventListener ? a.addEventListener(m, i, !1) : a.attachEvent && a.attachEvent("on" + m, i)
-                        }
-                        s.add && (s.add.call(a, o), o.handler.guid || (o.handler.guid = d.guid)), g ? r.splice(r.delegateCount++, 0, o) : r.push(o), f.event.global[m] = !0
-                    }
-                    a = null
-                }
-            },
-            global: {},
-            remove: function(a, b, c, d, e) {
-                var g = f.hasData(a) && f._data(a),
-                    h, i, j, k, l, m, n, o, p, q, r, s;
-                if (!!g && !!(o = g.events)) {
-                    b = f.trim(I(b || "")).split(" ");
-                    for (h = 0; h < b.length; h++) {
-                        i = A.exec(b[h]) || [], j = k = i[1], l = i[2];
-                        if (!j) {
-                            for (j in o) f.event.remove(a, j + b[h], c, d, !0);
-                            continue
-                        }
-                        p = f.event.special[j] || {}, j = (d ? p.delegateType : p.bindType) || j, r = o[j] || [], m = r.length, l = l ? new RegExp("(^|\\.)" + l.split(".").sort().join("\\.(?:.*\\.)?") + "(\\.|$)") : null;
-                        for (n = 0; n < r.length; n++) s = r[n], (e || k === s.origType) && (!c || c.guid === s.guid) && (!l || l.test(s.namespace)) && (!d || d === s.selector || d === "**" && s.selector) && (r.splice(n--, 1), s.selector && r.delegateCount--, p.remove && p.remove.call(a, s));
-                        r.length === 0 && m !== r.length && ((!p.teardown || p.teardown.call(a, l) === !1) && f.removeEvent(a, j, g.handle), delete o[j])
-                    }
-                    f.isEmptyObject(o) && (q = g.handle, q && (q.elem = null), f.removeData(a, ["events", "handle"], !0))
-                }
-            },
-            customEvent: {
-                getData: !0,
-                setData: !0,
-                changeData: !0
-            },
-            trigger: function(c, d, e, g) {
-                if (!e || e.nodeType !== 3 && e.nodeType !== 8) {
-                    var h = c.type || c,
-                        i = [],
-                        j, k, l, m, n, o, p, q, r, s;
-                    if (E.test(h + f.event.triggered)) return;
-                    h.indexOf("!") >= 0 && (h = h.slice(0, -1), k = !0), h.indexOf(".") >= 0 && (i = h.split("."), h = i.shift(), i.sort());
-                    if ((!e || f.event.customEvent[h]) && !f.event.global[h]) return;
-                    c = typeof c == "object" ? c[f.expando] ? c : new f.Event(h, c) : new f.Event(h), c.type = h, c.isTrigger = !0, c.exclusive = k, c.namespace = i.join("."), c.namespace_re = c.namespace ? new RegExp("(^|\\.)" + i.join("\\.(?:.*\\.)?") + "(\\.|$)") : null, o = h.indexOf(":") < 0 ? "on" + h : "";
-                    if (!e) {
-                        j = f.cache;
-                        for (l in j) j[l].events && j[l].events[h] && f.event.trigger(c, d, j[l].handle.elem, !0);
-                        return
-                    }
-                    c.result = b, c.target || (c.target = e), d = d != null ? f.makeArray(d) : [], d.unshift(c), p = f.event.special[h] || {};
-                    if (p.trigger && p.trigger.apply(e, d) === !1) return;
-                    r = [
-                        [e, p.bindType || h]
-                    ];
-                    if (!g && !p.noBubble && !f.isWindow(e)) {
-                        s = p.delegateType || h, m = E.test(s + h) ? e : e.parentNode, n = null;
-                        for (; m; m = m.parentNode) r.push([m, s]), n = m;
-                        n && n === e.ownerDocument && r.push([n.defaultView || n.parentWindow || a, s])
-                    }
-                    for (l = 0; l < r.length && !c.isPropagationStopped(); l++) m = r[l][0], c.type = r[l][1], q = (f._data(m, "events") || {})[c.type] && f._data(m, "handle"), q && q.apply(m, d), q = o && m[o], q && f.acceptData(m) && q.apply(m, d) === !1 && c.preventDefault();
-                    c.type = h, !g && !c.isDefaultPrevented() && (!p._default || p._default.apply(e.ownerDocument, d) === !1) && (h !== "click" || !f.nodeName(e, "a")) && f.acceptData(e) && o && e[h] && (h !== "focus" && h !== "blur" || c.target.offsetWidth !== 0) && !f.isWindow(e) && (n = e[o], n && (e[o] = null), f.event.triggered = h, e[h](), f.event.triggered = b, n && (e[o] = n));
-                    return c.result
-                }
-            },
-            dispatch: function(c) {
-                c = f.event.fix(c || a.event);
-                var d = (f._data(this, "events") || {})[c.type] || [],
-                    e = d.delegateCount,
-                    g = [].slice.call(arguments, 0),
-                    h = !c.exclusive && !c.namespace,
-                    i = [],
-                    j, k, l, m, n, o, p, q, r, s, t;
-                g[0] = c, c.delegateTarget = this;
-                if (e && !c.target.disabled && (!c.button || c.type !== "click")) {
-                    m = f(this), m.context = this.ownerDocument || this;
-                    for (l = c.target; l != this; l = l.parentNode || this) {
-                        o = {}, q = [], m[0] = l;
-                        for (j = 0; j < e; j++) r = d[j], s = r.selector, o[s] === b && (o[s] = r.quick ? H(l, r.quick) : m.is(s)), o[s] && q.push(r);
-                        q.length && i.push({
-                            elem: l,
-                            matches: q
-                        })
-                    }
-                }
-                d.length > e && i.push({
-                    elem: this,
-                    matches: d.slice(e)
-                });
-                for (j = 0; j < i.length && !c.isPropagationStopped(); j++) {
-                    p = i[j], c.currentTarget = p.elem;
-                    for (k = 0; k < p.matches.length && !c.isImmediatePropagationStopped(); k++) {
-                        r = p.matches[k];
-                        if (h || !c.namespace && !r.namespace || c.namespace_re && c.namespace_re.test(r.namespace)) c.data = r.data, c.handleObj = r, n = ((f.event.special[r.origType] || {}).handle || r.handler).apply(p.elem, g), n !== b && (c.result = n, n === !1 && (c.preventDefault(), c.stopPropagation()))
-                    }
-                }
-                return c.result
-            },
-            props: "attrChange attrName relatedNode srcElement altKey bubbles cancelable ctrlKey currentTarget eventPhase metaKey relatedTarget shiftKey target timeStamp view which".split(" "),
-            fixHooks: {},
-            keyHooks: {
-                props: "char charCode key keyCode".split(" "),
-                filter: function(a, b) {
-                    a.which == null && (a.which = b.charCode != null ? b.charCode : b.keyCode);
-                    return a
-                }
-            },
-            mouseHooks: {
-                props: "button buttons clientX clientY fromElement offsetX offsetY pageX pageY screenX screenY toElement".split(" "),
-                filter: function(a, d) {
-                    var e, f, g, h = d.button,
-                        i = d.fromElement;
-                    a.pageX == null && d.clientX != null && (e = a.target.ownerDocument || c, f = e.documentElement, g = e.body, a.pageX = d.clientX + (f && f.scrollLeft || g && g.scrollLeft || 0) - (f && f.clientLeft || g && g.clientLeft || 0), a.pageY = d.clientY + (f && f.scrollTop || g && g.scrollTop || 0) - (f && f.clientTop || g && g.clientTop || 0)), !a.relatedTarget && i && (a.relatedTarget = i === a.target ? d.toElement : i), !a.which && h !== b && (a.which = h & 1 ? 1 : h & 2 ? 3 : h & 4 ? 2 : 0);
-                    return a
-                }
-            },
-            fix: function(a) {
-                if (a[f.expando]) return a;
-                var d, e, g = a,
-                    h = f.event.fixHooks[a.type] || {},
-                    i = h.props ? this.props.concat(h.props) : this.props;
-                a = f.Event(g);
-                for (d = i.length; d;) e = i[--d], a[e] = g[e];
-                a.target || (a.target = g.srcElement || c), a.target.nodeType === 3 && (a.target = a.target.parentNode), a.metaKey === b && (a.metaKey = a.ctrlKey);
-                return h.filter ? h.filter(a, g) : a
-            },
-            special: {
-                ready: {
-                    setup: f.bindReady
-                },
-                load: {
-                    noBubble: !0
-                },
-                focus: {
-                    delegateType: "focusin"
-                },
-                blur: {
-                    delegateType: "focusout"
-                },
-                beforeunload: {
-                    setup: function(a, b, c) {
-                        f.isWindow(this) && (this.onbeforeunload = c)
-                    },
-                    teardown: function(a, b) {
-                        this.onbeforeunload === b && (this.onbeforeunload = null)
-                    }
-                }
-            },
-            simulate: function(a, b, c, d) {
-                var e = f.extend(new f.Event, c, {
-                    type: a,
-                    isSimulated: !0,
-                    originalEvent: {}
-                });
-                d ? f.event.trigger(e, null, b) : f.event.dispatch.call(b, e), e.isDefaultPrevented() && c.preventDefault()
-            }
-        }, f.event.handle = f.event.dispatch, f.removeEvent = c.removeEventListener ? function(a, b, c) {
-            a.removeEventListener && a.removeEventListener(b, c, !1)
-        } : function(a, b, c) {
-            a.detachEvent && a.detachEvent("on" + b, c)
-        }, f.Event = function(a, b) {
-            if (!(this instanceof f.Event)) return new f.Event(a, b);
-            a && a.type ? (this.originalEvent = a, this.type = a.type, this.isDefaultPrevented = a.defaultPrevented || a.returnValue === !1 || a.getPreventDefault && a.getPreventDefault() ? K : J) : this.type = a, b && f.extend(this, b), this.timeStamp = a && a.timeStamp || f.now(), this[f.expando] = !0
-        }, f.Event.prototype = {
-            preventDefault: function() {
-                this.isDefaultPrevented = K;
-                var a = this.originalEvent;
-                !a || (a.preventDefault ? a.preventDefault() : a.returnValue = !1)
-            },
-            stopPropagation: function() {
-                this.isPropagationStopped = K;
-                var a = this.originalEvent;
-                !a || (a.stopPropagation && a.stopPropagation(), a.cancelBubble = !0)
-            },
-            stopImmediatePropagation: function() {
-                this.isImmediatePropagationStopped = K, this.stopPropagation()
-            },
-            isDefaultPrevented: J,
-            isPropagationStopped: J,
-            isImmediatePropagationStopped: J
-        }, f.each({
-            mouseenter: "mouseover",
-            mouseleave: "mouseout"
-        }, function(a, b) {
-            f.event.special[a] = {
-                delegateType: b,
-                bindType: b,
-                handle: function(a) {
-                    var c = this,
-                        d = a.relatedTarget,
-                        e = a.handleObj,
-                        g = e.selector,
-                        h;
-                    if (!d || d !== c && !f.contains(c, d)) a.type = e.origType, h = e.handler.apply(this, arguments), a.type = b;
-                    return h
-                }
-            }
-        }), f.support.submitBubbles || (f.event.special.submit = {
-            setup: function() {
-                if (f.nodeName(this, "form")) return !1;
-                f.event.add(this, "click._submit keypress._submit", function(a) {
-                    var c = a.target,
-                        d = f.nodeName(c, "input") || f.nodeName(c, "button") ? c.form : b;
-                    d && !d._submit_attached && (f.event.add(d, "submit._submit", function(a) {
-                        this.parentNode && !a.isTrigger && f.event.simulate("submit", this.parentNode, a, !0)
-                    }), d._submit_attached = !0)
-                })
-            },
-            teardown: function() {
-                if (f.nodeName(this, "form")) return !1;
-                f.event.remove(this, "._submit")
-            }
-        }), f.support.changeBubbles || (f.event.special.change = {
-            setup: function() {
-                if (z.test(this.nodeName)) {
-                    if (this.type === "checkbox" || this.type === "radio") f.event.add(this, "propertychange._change", function(a) {
-                        a.originalEvent.propertyName === "checked" && (this._just_changed = !0)
-                    }), f.event.add(this, "click._change", function(a) {
-                        this._just_changed && !a.isTrigger && (this._just_changed = !1, f.event.simulate("change", this, a, !0))
-                    });
-                    return !1
-                }
-                f.event.add(this, "beforeactivate._change", function(a) {
-                    var b = a.target;
-                    z.test(b.nodeName) && !b._change_attached && (f.event.add(b, "change._change", function(a) {
-                        this.parentNode && !a.isSimulated && !a.isTrigger && f.event.simulate("change", this.parentNode, a, !0)
-                    }), b._change_attached = !0)
-                })
-            },
-            handle: function(a) {
-                var b = a.target;
-                if (this !== b || a.isSimulated || a.isTrigger || b.type !== "radio" && b.type !== "checkbox") return a.handleObj.handler.apply(this, arguments)
-            },
-            teardown: function() {
-                f.event.remove(this, "._change");
-                return z.test(this.nodeName)
-            }
-        }), f.support.focusinBubbles || f.each({
-            focus: "focusin",
-            blur: "focusout"
-        }, function(a, b) {
-            var d = 0,
-                e = function(a) {
-                    f.event.simulate(b, a.target, f.event.fix(a), !0)
-                };
-            f.event.special[b] = {
-                setup: function() {
-                    d++ === 0 && c.addEventListener(a, e, !0)
-                },
-                teardown: function() {
-                    --d === 0 && c.removeEventListener(a, e, !0)
-                }
-            }
-        }), f.fn.extend({
-            on: function(a, c, d, e, g) {
-                var h, i;
-                if (typeof a == "object") {
-                    typeof c != "string" && (d = c, c = b);
-                    for (i in a) this.on(i, c, d, a[i], g);
-                    return this
-                }
-                d == null && e == null ? (e = c, d = c = b) : e == null && (typeof c == "string" ? (e = d, d = b) : (e = d, d = c, c = b));
-                if (e === !1) e = J;
-                else if (!e) return this;
-                g === 1 && (h = e, e = function(a) {
-                    f().off(a);
-                    return h.apply(this, arguments)
-                }, e.guid = h.guid || (h.guid = f.guid++));
-                return this.each(function() {
-                    f.event.add(this, a, e, d, c)
-                })
-            },
-            one: function(a, b, c, d) {
-                return this.on.call(this, a, b, c, d, 1)
-            },
-            off: function(a, c, d) {
-                if (a && a.preventDefault && a.handleObj) {
-                    var e = a.handleObj;
-                    f(a.delegateTarget).off(e.namespace ? e.type + "." + e.namespace : e.type, e.selector, e.handler);
-                    return this
-                }
-                if (typeof a == "object") {
-                    for (var g in a) this.off(g, c, a[g]);
-                    return this
-                }
-                if (c === !1 || typeof c == "function") d = c, c = b;
-                d === !1 && (d = J);
-                return this.each(function() {
-                    f.event.remove(this, a, d, c)
-                })
-            },
-            bind: function(a, b, c) {
-                return this.on(a, null, b, c)
-            },
-            unbind: function(a, b) {
-                return this.off(a, null, b)
-            },
-            live: function(a, b, c) {
-                f(this.context).on(a, this.selector, b, c);
-                return this
-            },
-            die: function(a, b) {
-                f(this.context).off(a, this.selector || "**", b);
+        off: function(a, b, c) {
+            var d, e;
+            if (a && a.preventDefault && a.handleObj) return d = a.handleObj, n(a.delegateTarget).off(d.namespace ? d.origType + "." + d.namespace : d.origType, d.selector, d.handler), this;
+            if ("object" == typeof a) {
+                for (e in a) this.off(e, b, a[e]);
                 return this
-            },
-            delegate: function(a, b, c, d) {
-                return this.on(b, a, c, d)
-            },
-            undelegate: function(a, b, c) {
-                return arguments.length == 1 ? this.off(a, "**") : this.off(b, a, c)
-            },
-            trigger: function(a, b) {
-                return this.each(function() {
-                    f.event.trigger(a, b, this)
-                })
-            },
-            triggerHandler: function(a, b) {
-                if (this[0]) return f.event.trigger(a, b, this[0], !0)
-            },
-            toggle: function(a) {
-                var b = arguments,
-                    c = a.guid || f.guid++,
-                    d = 0,
-                    e = function(c) {
-                        var e = (f._data(this, "lastToggle" + a.guid) || 0) % d;
-                        f._data(this, "lastToggle" + a.guid, e + 1), c.preventDefault();
-                        return b[e].apply(this, arguments) || !1
-                    };
-                e.guid = c;
-                while (d < b.length) b[d++].guid = c;
-                return this.click(e)
-            },
-            hover: function(a, b) {
-                return this.mouseenter(a).mouseleave(b || a)
-            }
-        }), f.each("blur focus focusin focusout load resize scroll unload click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup error contextmenu".split(" "), function(a, b) {
-            f.fn[b] = function(a, c) {
-                c == null && (c = a, a = null);
-                return arguments.length > 0 ? this.on(b, null, a, c) : this.trigger(b)
-            }, f.attrFn && (f.attrFn[b] = !0), C.test(b) && (f.event.fixHooks[b] = f.event.keyHooks), D.test(b) && (f.event.fixHooks[b] = f.event.mouseHooks)
-        }),
-        function() {
-            function x(a, b, c, e, f, g) {
-                for (var h = 0, i = e.length; h < i; h++) {
-                    var j = e[h];
-                    if (j) {
-                        var k = !1;
-                        j = j[a];
-                        while (j) {
-                            if (j[d] === c) {
-                                k = e[j.sizset];
-                                break
-                            }
-                            if (j.nodeType === 1) {
-                                g || (j[d] = c, j.sizset = h);
-                                if (typeof b != "string") {
-                                    if (j === b) {
-                                        k = !0;
-                                        break
-                                    }
-                                } else if (m.filter(b, [j]).length > 0) {
-                                    k = j;
-                                    break
-                                }
-                            }
-                            j = j[a]
-                        }
-                        e[h] = k
-                    }
-                }
             }
+            return b !== !1 && "function" != typeof b || (c = b, b = void 0), c === !1 && (c = ha), this.each(function() {
+                n.event.remove(this, a, c, b)
+            })
+        }
+    });
+    var ka = /<(?!area|br|col|embed|hr|img|input|link|meta|param)(([\w:-]+)[^>]*)\/>/gi,
+        la = /<script|<style|<link/i,
+        ma = /checked\s*(?:[^=]|=\s*.checked.)/i,
+        na = /^true\/(.*)/,
+        oa = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
 
-            function w(a, b, c, e, f, g) {
-                for (var h = 0, i = e.length; h < i; h++) {
-                    var j = e[h];
-                    if (j) {
-                        var k = !1;
-                        j = j[a];
-                        while (j) {
-                            if (j[d] === c) {
-                                k = e[j.sizset];
-                                break
-                            }
-                            j.nodeType === 1 && !g && (j[d] = c, j.sizset = h);
-                            if (j.nodeName.toLowerCase() === b) {
-                                k = j;
-                                break
-                            }
-                            j = j[a]
-                        }
-                        e[h] = k
-                    }
-                }
-            }
-            var a = /((?:\((?:\([^()]+\)|[^()]+)+\)|\[(?:\[[^\[\]]*\]|['"][^'"]*['"]|[^\[\]'"]+)+\]|\\.|[^ >+~,(\[\\]+)+|[>+~])(\s*,\s*)?((?:.|\r|\n)*)/g,
-                d = "sizcache" + (Math.random() + "").replace(".", ""),
-                e = 0,
-                g = Object.prototype.toString,
-                h = !1,
-                i = !0,
-                j = /\\/g,
-                k = /\r\n/g,
-                l = /\W/;
-            [0, 0].sort(function() {
-                i = !1;
-                return 0
-            });
-            var m = function(b, d, e, f) {
-                e = e || [], d = d || c;
-                var h = d;
-                if (d.nodeType !== 1 && d.nodeType !== 9) return [];
-                if (!b || typeof b != "string") return e;
-                var i, j, k, l, n, q, r, t, u = !0,
-                    v = m.isXML(d),
-                    w = [],
-                    x = b;
-                do {
-                    a.exec(""), i = a.exec(x);
-                    if (i) {
-                        x = i[3], w.push(i[1]);
-                        if (i[2]) {
-                            l = i[3];
-                            break
-                        }
-                    }
-                } while (i);
-                if (w.length > 1 && p.exec(b))
-                    if (w.length === 2 && o.relative[w[0]]) j = y(w[0] + w[1], d, f);
-                    else {
-                        j = o.relative[w[0]] ? [d] : m(w.shift(), d);
-                        while (w.length) b = w.shift(), o.relative[b] && (b += w.shift()), j = y(b, j, f)
-                    }
-                else {
-                    !f && w.length > 1 && d.nodeType === 9 && !v && o.match.ID.test(w[0]) && !o.match.ID.test(w[w.length - 1]) && (n = m.find(w.shift(), d, v), d = n.expr ? m.filter(n.expr, n.set)[0] : n.set[0]);
-                    if (d) {
-                        n = f ? {
-                            expr: w.pop(),
-                            set: s(f)
-                        } : m.find(w.pop(), w.length === 1 && (w[0] === "~" || w[0] === "+") && d.parentNode ? d.parentNode : d, v), j = n.expr ? m.filter(n.expr, n.set) : n.set, w.length > 0 ? k = s(j) : u = !1;
-                        while (w.length) q = w.pop(), r = q, o.relative[q] ? r = w.pop() : q = "", r == null && (r = d), o.relative[q](k, r, v)
-                    } else k = w = []
-                }
-                k || (k = j), k || m.error(q || b);
-                if (g.call(k) === "[object Array]")
-                    if (!u) e.push.apply(e, k);
-                    else if (d && d.nodeType === 1)
-                    for (t = 0; k[t] != null; t++) k[t] && (k[t] === !0 || k[t].nodeType === 1 && m.contains(d, k[t])) && e.push(j[t]);
-                else
-                    for (t = 0; k[t] != null; t++) k[t] && k[t].nodeType === 1 && e.push(j[t]);
-                else s(k, e);
-                l && (m(l, h, e, f), m.uniqueSort(e));
-                return e
-            };
-            m.uniqueSort = function(a) {
-                if (u) {
-                    h = i, a.sort(u);
-                    if (h)
-                        for (var b = 1; b < a.length; b++) a[b] === a[b - 1] && a.splice(b--, 1)
-                }
-                return a
-            }, m.matches = function(a, b) {
-                return m(a, null, null, b)
-            }, m.matchesSelector = function(a, b) {
-                return m(b, null, null, [a]).length > 0
-            }, m.find = function(a, b, c) {
-                var d, e, f, g, h, i;
-                if (!a) return [];
-                for (e = 0, f = o.order.length; e < f; e++) {
-                    h = o.order[e];
-                    if (g = o.leftMatch[h].exec(a)) {
-                        i = g[1], g.splice(1, 1);
-                        if (i.substr(i.length - 1) !== "\\") {
-                            g[1] = (g[1] || "").replace(j, ""), d = o.find[h](g, b, c);
-                            if (d != null) {
-                                a = a.replace(o.match[h], "");
-                                break
-                            }
-                        }
-                    }
-                }
-                d || (d = typeof b.getElementsByTagName != "undefined" ? b.getElementsByTagName("*") : []);
-                return {
-                    set: d,
-                    expr: a
-                }
-            }, m.filter = function(a, c, d, e) {
-                var f, g, h, i, j, k, l, n, p, q = a,
-                    r = [],
-                    s = c,
-                    t = c && c[0] && m.isXML(c[0]);
-                while (a && c.length) {
-                    for (h in o.filter)
-                        if ((f = o.leftMatch[h].exec(a)) != null && f[2]) {
-                            k = o.filter[h], l = f[1], g = !1, f.splice(1, 1);
-                            if (l.substr(l.length - 1) === "\\") continue;
-                            s === r && (r = []);
-                            if (o.preFilter[h]) {
-                                f = o.preFilter[h](f, s, d, r, e, t);
-                                if (!f) g = i = !0;
-                                else if (f === !0) continue
-                            }
-                            if (f)
-                                for (n = 0;
-                                    (j = s[n]) != null; n++) j && (i = k(j, f, n, s), p = e ^ i, d && i != null ? p ? g = !0 : s[n] = !1 : p && (r.push(j), g = !0));
-                            if (i !== b) {
-                                d || (s = r), a = a.replace(o.match[h], "");
-                                if (!g) return [];
-                                break
-                            }
-                        } if (a === q)
-                        if (g == null) m.error(a);
-                        else break;
-                    q = a
-                }
-                return s
-            }, m.error = function(a) {
-                throw new Error("Syntax error, unrecognized expression: " + a)
-            };
-            var n = m.getText = function(a) {
-                    var b, c, d = a.nodeType,
-                        e = "";
-                    if (d) {
-                        if (d === 1 || d === 9) {
-                            if (typeof a.textContent == "string") return a.textContent;
-                            if (typeof a.innerText == "string") return a.innerText.replace(k, "");
-                            for (a = a.firstChild; a; a = a.nextSibling) e += n(a)
-                        } else if (d === 3 || d === 4) return a.nodeValue
-                    } else
-                        for (b = 0; c = a[b]; b++) c.nodeType !== 8 && (e += n(c));
-                    return e
-                },
-                o = m.selectors = {
-                    order: ["ID", "NAME", "TAG"],
-                    match: {
-                        ID: /#((?:[\w\u00c0-\uFFFF\-]|\\.)+)/,
-                        CLASS: /\.((?:[\w\u00c0-\uFFFF\-]|\\.)+)/,
-                        NAME: /\[name=['"]*((?:[\w\u00c0-\uFFFF\-]|\\.)+)['"]*\]/,
-                        ATTR: /\[\s*((?:[\w\u00c0-\uFFFF\-]|\\.)+)\s*(?:(\S?=)\s*(?:(['"])(.*?)\3|(#?(?:[\w\u00c0-\uFFFF\-]|\\.)*)|)|)\s*\]/,
-                        TAG: /^((?:[\w\u00c0-\uFFFF\*\-]|\\.)+)/,
-                        CHILD: /:(only|nth|last|first)-child(?:\(\s*(even|odd|(?:[+\-]?\d+|(?:[+\-]?\d*)?n\s*(?:[+\-]\s*\d+)?))\s*\))?/,
-                        POS: /:(nth|eq|gt|lt|first|last|even|odd)(?:\((\d*)\))?(?=[^\-]|$)/,
-                        PSEUDO: /:((?:[\w\u00c0-\uFFFF\-]|\\.)+)(?:\((['"]?)((?:\([^\)]+\)|[^\(\)]*)+)\2\))?/
-                    },
-                    leftMatch: {},
-                    attrMap: {
-                        "class": "className",
-                        "for": "htmlFor"
-                    },
-                    attrHandle: {
-                        href: function(a) {
-                            return a.getAttribute("href")
-                        },
-                        type: function(a) {
-                            return a.getAttribute("type")
-                        }
-                    },
-                    relative: {
-                        "+": function(a, b) {
-                            var c = typeof b == "string",
-                                d = c && !l.test(b),
-                                e = c && !d;
-                            d && (b = b.toLowerCase());
-                            for (var f = 0, g = a.length, h; f < g; f++)
-                                if (h = a[f]) {
-                                    while ((h = h.previousSibling) && h.nodeType !== 1);
-                                    a[f] = e || h && h.nodeName.toLowerCase() === b ? h || !1 : h === b
-                                } e && m.filter(b, a, !0)
-                        },
-                        ">": function(a, b) {
-                            var c, d = typeof b == "string",
-                                e = 0,
-                                f = a.length;
-                            if (d && !l.test(b)) {
-                                b = b.toLowerCase();
-                                for (; e < f; e++) {
-                                    c = a[e];
-                                    if (c) {
-                                        var g = c.parentNode;
-                                        a[e] = g.nodeName.toLowerCase() === b ? g : !1
-                                    }
-                                }
-                            } else {
-                                for (; e < f; e++) c = a[e], c && (a[e] = d ? c.parentNode : c.parentNode === b);
-                                d && m.filter(b, a, !0)
-                            }
-                        },
-                        "": function(a, b, c) {
-                            var d, f = e++,
-                                g = x;
-                            typeof b == "string" && !l.test(b) && (b = b.toLowerCase(), d = b, g = w), g("parentNode", b, f, a, d, c)
-                        },
-                        "~": function(a, b, c) {
-                            var d, f = e++,
-                                g = x;
-                            typeof b == "string" && !l.test(b) && (b = b.toLowerCase(), d = b, g = w), g("previousSibling", b, f, a, d, c)
-                        }
-                    },
-                    find: {
-                        ID: function(a, b, c) {
-                            if (typeof b.getElementById != "undefined" && !c) {
-                                var d = b.getElementById(a[1]);
-                                return d && d.parentNode ? [d] : []
-                            }
-                        },
-                        NAME: function(a, b) {
-                            if (typeof b.getElementsByName != "undefined") {
-                                var c = [],
-                                    d = b.getElementsByName(a[1]);
-                                for (var e = 0, f = d.length; e < f; e++) d[e].getAttribute("name") === a[1] && c.push(d[e]);
-                                return c.length === 0 ? null : c
-                            }
-                        },
-                        TAG: function(a, b) {
-                            if (typeof b.getElementsByTagName != "undefined") return b.getElementsByTagName(a[1])
-                        }
-                    },
-                    preFilter: {
-                        CLASS: function(a, b, c, d, e, f) {
-                            a = " " + a[1].replace(j, "") + " ";
-                            if (f) return a;
-                            for (var g = 0, h;
-                                (h = b[g]) != null; g++) h && (e ^ (h.className && (" " + h.className + " ").replace(/[\t\n\r]/g, " ").indexOf(a) >= 0) ? c || d.push(h) : c && (b[g] = !1));
-                            return !1
-                        },
-                        ID: function(a) {
-                            return a[1].replace(j, "")
-                        },
-                        TAG: function(a, b) {
-                            return a[1].replace(j, "").toLowerCase()
-                        },
-                        CHILD: function(a) {
-                            if (a[1] === "nth") {
-                                a[2] || m.error(a[0]), a[2] = a[2].replace(/^\+|\s*/g, "");
-                                var b = /(-?)(\d*)(?:n([+\-]?\d*))?/.exec(a[2] === "even" && "2n" || a[2] === "odd" && "2n+1" || !/\D/.test(a[2]) && "0n+" + a[2] || a[2]);
-                                a[2] = b[1] + (b[2] || 1) - 0, a[3] = b[3] - 0
-                            } else a[2] && m.error(a[0]);
-                            a[0] = e++;
-                            return a
-                        },
-                        ATTR: function(a, b, c, d, e, f) {
-                            var g = a[1] = a[1].replace(j, "");
-                            !f && o.attrMap[g] && (a[1] = o.attrMap[g]), a[4] = (a[4] || a[5] || "").replace(j, ""), a[2] === "~=" && (a[4] = " " + a[4] + " ");
-                            return a
-                        },
-                        PSEUDO: function(b, c, d, e, f) {
-                            if (b[1] === "not")
-                                if ((a.exec(b[3]) || "").length > 1 || /^\w/.test(b[3])) b[3] = m(b[3], null, null, c);
-                                else {
-                                    var g = m.filter(b[3], c, d, !0 ^ f);
-                                    d || e.push.apply(e, g);
-                                    return !1
-                                }
-                            else if (o.match.POS.test(b[0]) || o.match.CHILD.test(b[0])) return !0;
-                            return b
-                        },
-                        POS: function(a) {
-                            a.unshift(!0);
-                            return a
-                        }
-                    },
-                    filters: {
-                        enabled: function(a) {
-                            return a.disabled === !1 && a.type !== "hidden"
-                        },
-                        disabled: function(a) {
-                            return a.disabled === !0
-                        },
-                        checked: function(a) {
-                            return a.checked === !0
-                        },
-                        selected: function(a) {
-                            a.parentNode && a.parentNode.selectedIndex;
-                            return a.selected === !0
-                        },
-                        parent: function(a) {
-                            return !!a.firstChild
-                        },
-                        empty: function(a) {
-                            return !a.firstChild
-                        },
-                        has: function(a, b, c) {
-                            return !!m(c[3], a).length
-                        },
-                        header: function(a) {
-                            return /h\d/i.test(a.nodeName)
-                        },
-                        text: function(a) {
-                            var b = a.getAttribute("type"),
-                                c = a.type;
-                            return a.nodeName.toLowerCase() === "input" && "text" === c && (b === c || b === null)
-                        },
-                        radio: function(a) {
-                            return a.nodeName.toLowerCase() === "input" && "radio" === a.type
-                        },
-                        checkbox: function(a) {
-                            return a.nodeName.toLowerCase() === "input" && "checkbox" === a.type
-                        },
-                        file: function(a) {
-                            return a.nodeName.toLowerCase() === "input" && "file" === a.type
-                        },
-                        password: function(a) {
-                            return a.nodeName.toLowerCase() === "input" && "password" === a.type
-                        },
-                        submit: function(a) {
-                            var b = a.nodeName.toLowerCase();
-                            return (b === "input" || b === "button") && "submit" === a.type
-                        },
-                        image: function(a) {
-                            return a.nodeName.toLowerCase() === "input" && "image" === a.type
-                        },
-                        reset: function(a) {
-                            var b = a.nodeName.toLowerCase();
-                            return (b === "input" || b === "button") && "reset" === a.type
-                        },
-                        button: function(a) {
-                            var b = a.nodeName.toLowerCase();
-                            return b === "input" && "button" === a.type || b === "button"
-                        },
-                        input: function(a) {
-                            return /input|select|textarea|button/i.test(a.nodeName)
-                        },
-                        focus: function(a) {
-                            return a === a.ownerDocument.activeElement
-                        }
-                    },
-                    setFilters: {
-                        first: function(a, b) {
-                            return b === 0
-                        },
-                        last: function(a, b, c, d) {
-                            return b === d.length - 1
-                        },
-                        even: function(a, b) {
-                            return b % 2 === 0
-                        },
-                        odd: function(a, b) {
-                            return b % 2 === 1
-                        },
-                        lt: function(a, b, c) {
-                            return b < c[3] - 0
-                        },
-                        gt: function(a, b, c) {
-                            return b > c[3] - 0
-                        },
-                        nth: function(a, b, c) {
-                            return c[3] - 0 === b
-                        },
-                        eq: function(a, b, c) {
-                            return c[3] - 0 === b
-                        }
-                    },
-                    filter: {
-                        PSEUDO: function(a, b, c, d) {
-                            var e = b[1],
-                                f = o.filters[e];
-                            if (f) return f(a, c, b, d);
-                            if (e === "contains") return (a.textContent || a.innerText || n([a]) || "").indexOf(b[3]) >= 0;
-                            if (e === "not") {
-                                var g = b[3];
-                                for (var h = 0, i = g.length; h < i; h++)
-                                    if (g[h] === a) return !1;
-                                return !0
-                            }
-                            m.error(e)
-                        },
-                        CHILD: function(a, b) {
-                            var c, e, f, g, h, i, j, k = b[1],
-                                l = a;
-                            switch (k) {
-                                case "only":
-                                case "first":
-                                    while (l = l.previousSibling)
-                                        if (l.nodeType === 1) return !1;
-                                    if (k === "first") return !0;
-                                    l = a;
-                                case "last":
-                                    while (l = l.nextSibling)
-                                        if (l.nodeType === 1) return !1;
-                                    return !0;
-                                case "nth":
-                                    c = b[2], e = b[3];
-                                    if (c === 1 && e === 0) return !0;
-                                    f = b[0], g = a.parentNode;
-                                    if (g && (g[d] !== f || !a.nodeIndex)) {
-                                        i = 0;
-                                        for (l = g.firstChild; l; l = l.nextSibling) l.nodeType === 1 && (l.nodeIndex = ++i);
-                                        g[d] = f
-                                    }
-                                    j = a.nodeIndex - e;
-                                    return c === 0 ? j === 0 : j % c === 0 && j / c >= 0
-                            }
-                        },
-                        ID: function(a, b) {
-                            return a.nodeType === 1 && a.getAttribute("id") === b
-                        },
-                        TAG: function(a, b) {
-                            return b === "*" && a.nodeType === 1 || !!a.nodeName && a.nodeName.toLowerCase() === b
-                        },
-                        CLASS: function(a, b) {
-                            return (" " + (a.className || a.getAttribute("class")) + " ").indexOf(b) > -1
-                        },
-                        ATTR: function(a, b) {
-                            var c = b[1],
-                                d = m.attr ? m.attr(a, c) : o.attrHandle[c] ? o.attrHandle[c](a) : a[c] != null ? a[c] : a.getAttribute(c),
-                                e = d + "",
-                                f = b[2],
-                                g = b[4];
-                            return d == null ? f === "!=" : !f && m.attr ? d != null : f === "=" ? e === g : f === "*=" ? e.indexOf(g) >= 0 : f === "~=" ? (" " + e + " ").indexOf(g) >= 0 : g ? f === "!=" ? e !== g : f === "^=" ? e.indexOf(g) === 0 : f === "$=" ? e.substr(e.length - g.length) === g : f === "|=" ? e === g || e.substr(0, g.length + 1) === g + "-" : !1 : e && d !== !1
-                        },
-                        POS: function(a, b, c, d) {
-                            var e = b[2],
-                                f = o.setFilters[e];
-                            if (f) return f(a, c, b, d)
-                        }
-                    }
-                },
-                p = o.match.POS,
-                q = function(a, b) {
-                    return "\\" + (b - 0 + 1)
-                };
-            for (var r in o.match) o.match[r] = new RegExp(o.match[r].source + /(?![^\[]*\])(?![^\(]*\))/.source), o.leftMatch[r] = new RegExp(/(^(?:.|\r|\n)*?)/.source + o.match[r].source.replace(/\\(\d+)/g, q));
-            var s = function(a, b) {
-                a = Array.prototype.slice.call(a, 0);
-                if (b) {
-                    b.push.apply(b, a);
-                    return b
-                }
-                return a
-            };
-            try {
-                Array.prototype.slice.call(c.documentElement.childNodes, 0)[0].nodeType
-            } catch (t) {
-                s = function(a, b) {
-                    var c = 0,
-                        d = b || [];
-                    if (g.call(a) === "[object Array]") Array.prototype.push.apply(d, a);
-                    else if (typeof a.length == "number")
-                        for (var e = a.length; c < e; c++) d.push(a[c]);
-                    else
-                        for (; a[c]; c++) d.push(a[c]);
-                    return d
-                }
-            }
-            var u, v;
-            c.documentElement.compareDocumentPosition ? u = function(a, b) {
-                    if (a === b) {
-                        h = !0;
-                        return 0
-                    }
-                    if (!a.compareDocumentPosition || !b.compareDocumentPosition) return a.compareDocumentPosition ? -1 : 1;
-                    return a.compareDocumentPosition(b) & 4 ? -1 : 1
-                } : (u = function(a, b) {
-                    if (a === b) {
-                        h = !0;
-                        return 0
-                    }
-                    if (a.sourceIndex && b.sourceIndex) return a.sourceIndex - b.sourceIndex;
-                    var c, d, e = [],
-                        f = [],
-                        g = a.parentNode,
-                        i = b.parentNode,
-                        j = g;
-                    if (g === i) return v(a, b);
-                    if (!g) return -1;
-                    if (!i) return 1;
-                    while (j) e.unshift(j), j = j.parentNode;
-                    j = i;
-                    while (j) f.unshift(j), j = j.parentNode;
-                    c = e.length, d = f.length;
-                    for (var k = 0; k < c && k < d; k++)
-                        if (e[k] !== f[k]) return v(e[k], f[k]);
-                    return k === c ? v(a, f[k], -1) : v(e[k], b, 1)
-                }, v = function(a, b, c) {
-                    if (a === b) return c;
-                    var d = a.nextSibling;
-                    while (d) {
-                        if (d === b) return -1;
-                        d = d.nextSibling
-                    }
-                    return 1
-                }),
-                function() {
-                    var a = c.createElement("div"),
-                        d = "script" + (new Date).getTime(),
-                        e = c.documentElement;
-                    a.innerHTML = "<a name='" + d + "'/>", e.insertBefore(a, e.firstChild), c.getElementById(d) && (o.find.ID = function(a, c, d) {
-                        if (typeof c.getElementById != "undefined" && !d) {
-                            var e = c.getElementById(a[1]);
-                            return e ? e.id === a[1] || typeof e.getAttributeNode != "undefined" && e.getAttributeNode("id").nodeValue === a[1] ? [e] : b : []
-                        }
-                    }, o.filter.ID = function(a, b) {
-                        var c = typeof a.getAttributeNode != "undefined" && a.getAttributeNode("id");
-                        return a.nodeType === 1 && c && c.nodeValue === b
-                    }), e.removeChild(a), e = a = null
-                }(),
-                function() {
-                    var a = c.createElement("div");
-                    a.appendChild(c.createComment("")), a.getElementsByTagName("*").length > 0 && (o.find.TAG = function(a, b) {
-                        var c = b.getElementsByTagName(a[1]);
-                        if (a[1] === "*") {
-                            var d = [];
-                            for (var e = 0; c[e]; e++) c[e].nodeType === 1 && d.push(c[e]);
-                            c = d
-                        }
-                        return c
-                    }), a.innerHTML = "<a href='#'></a>", a.firstChild && typeof a.firstChild.getAttribute != "undefined" && a.firstChild.getAttribute("href") !== "#" && (o.attrHandle.href = function(a) {
-                        return a.getAttribute("href", 2)
-                    }), a = null
-                }(), c.querySelectorAll && function() {
-                    var a = m,
-                        b = c.createElement("div"),
-                        d = "__sizzle__";
-                    b.innerHTML = "<p class='TEST'></p>";
-                    if (!b.querySelectorAll || b.querySelectorAll(".TEST").length !== 0) {
-                        m = function(b, e, f, g) {
-                            e = e || c;
-                            if (!g && !m.isXML(e)) {
-                                var h = /^(\w+$)|^\.([\w\-]+$)|^#([\w\-]+$)/.exec(b);
-                                if (h && (e.nodeType === 1 || e.nodeType === 9)) {
-                                    if (h[1]) return s(e.getElementsByTagName(b), f);
-                                    if (h[2] && o.find.CLASS && e.getElementsByClassName) return s(e.getElementsByClassName(h[2]), f)
-                                }
-                                if (e.nodeType === 9) {
-                                    if (b === "body" && e.body) return s([e.body], f);
-                                    if (h && h[3]) {
-                                        var i = e.getElementById(h[3]);
-                                        if (!i || !i.parentNode) return s([], f);
-                                        if (i.id === h[3]) return s([i], f)
-                                    }
-                                    try {
-                                        return s(e.querySelectorAll(b), f)
-                                    } catch (j) {}
-                                } else if (e.nodeType === 1 && e.nodeName.toLowerCase() !== "object") {
-                                    var k = e,
-                                        l = e.getAttribute("id"),
-                                        n = l || d,
-                                        p = e.parentNode,
-                                        q = /^\s*[+~]/.test(b);
-                                    l ? n = n.replace(/'/g, "\\$&") : e.setAttribute("id", n), q && p && (e = e.parentNode);
-                                    try {
-                                        if (!q || p) return s(e.querySelectorAll("[id='" + n + "'] " + b), f)
-                                    } catch (r) {} finally {
-                                        l || k.removeAttribute("id")
-                                    }
-                                }
-                            }
-                            return a(b, e, f, g)
-                        };
-                        for (var e in a) m[e] = a[e];
-                        b = null
-                    }
-                }(),
-                function() {
-                    var a = c.documentElement,
-                        b = a.matchesSelector || a.mozMatchesSelector || a.webkitMatchesSelector || a.msMatchesSelector;
-                    if (b) {
-                        var d = !b.call(c.createElement("div"), "div"),
-                            e = !1;
-                        try {
-                            b.call(c.documentElement, "[test!='']:sizzle")
-                        } catch (f) {
-                            e = !0
-                        }
-                        m.matchesSelector = function(a, c) {
-                            c = c.replace(/\=\s*([^'"\]]*)\s*\]/g, "='$1']");
-                            if (!m.isXML(a)) try {
-                                if (e || !o.match.PSEUDO.test(c) && !/!=/.test(c)) {
-                                    var f = b.call(a, c);
-                                    if (f || !d || a.document && a.document.nodeType !== 11) return f
-                                }
-                            } catch (g) {}
-                            return m(c, null, null, [a]).length > 0
-                        }
-                    }
-                }(),
-                function() {
-                    var a = c.createElement("div");
-                    a.innerHTML = "<div class='test e'></div><div class='test'></div>";
-                    if (!!a.getElementsByClassName && a.getElementsByClassName("e").length !== 0) {
-                        a.lastChild.className = "e";
-                        if (a.getElementsByClassName("e").length === 1) return;
-                        o.order.splice(1, 0, "CLASS"), o.find.CLASS = function(a, b, c) {
-                            if (typeof b.getElementsByClassName != "undefined" && !c) return b.getElementsByClassName(a[1])
-                        }, a = null
-                    }
-                }(), c.documentElement.contains ? m.contains = function(a, b) {
-                    return a !== b && (a.contains ? a.contains(b) : !0)
-                } : c.documentElement.compareDocumentPosition ? m.contains = function(a, b) {
-                    return !!(a.compareDocumentPosition(b) & 16)
-                } : m.contains = function() {
-                    return !1
-                }, m.isXML = function(a) {
-                    var b = (a ? a.ownerDocument || a : 0).documentElement;
-                    return b ? b.nodeName !== "HTML" : !1
-                };
-            var y = function(a, b, c) {
-                var d, e = [],
-                    f = "",
-                    g = b.nodeType ? [b] : b;
-                while (d = o.match.PSEUDO.exec(a)) f += d[0], a = a.replace(o.match.PSEUDO, "");
-                a = o.relative[a] ? a + "*" : a;
-                for (var h = 0, i = g.length; h < i; h++) m(a, g[h], e, c);
-                return m.filter(f, e)
-            };
-            m.attr = f.attr, m.selectors.attrMap = {}, f.find = m, f.expr = m.selectors, f.expr[":"] = f.expr.filters, f.unique = m.uniqueSort, f.text = m.getText, f.isXMLDoc = m.isXML, f.contains = m.contains
-        }();
-    var L = /Until$/,
-        M = /^(?:parents|prevUntil|prevAll)/,
-        N = /,/,
-        O = /^.[^:#\[\.,]*$/,
-        P = Array.prototype.slice,
-        Q = f.expr.match.POS,
-        R = {
-            children: !0,
-            contents: !0,
-            next: !0,
-            prev: !0
-        };
-    f.fn.extend({
-        find: function(a) {
-            var b = this,
-                c, d;
-            if (typeof a != "string") return f(a).filter(function() {
-                for (c = 0, d = b.length; c < d; c++)
-                    if (f.contains(b[c], this)) return !0
-            });
-            var e = this.pushStack("", "find", a),
-                g, h, i;
-            for (c = 0, d = this.length; c < d; c++) {
-                g = e.length, f.find(a, this[c], e);
-                if (c > 0)
-                    for (h = g; h < e.length; h++)
-                        for (i = 0; i < g; i++)
-                            if (e[i] === e[h]) {
-                                e.splice(h--, 1);
-                                break
-                            }
+    function pa(a, b) {
+        return n.nodeName(a, "table") && n.nodeName(11 !== b.nodeType ? b : b.firstChild, "tr") ? a.getElementsByTagName("tbody")[0] || a.appendChild(a.ownerDocument.createElement("tbody")) : a
+    }
+
+    function qa(a) {
+        return a.type = (null !== a.getAttribute("type")) + "/" + a.type, a
+    }
+
+    function ra(a) {
+        var b = na.exec(a.type);
+        return b ? a.type = b[1] : a.removeAttribute("type"), a
+    }
+
+    function sa(a, b) {
+        var c, d, e, f, g, h, i, j;
+        if (1 === b.nodeType) {
+            if (N.hasData(a) && (f = N.access(a), g = N.set(b, f), j = f.events)) {
+                delete g.handle, g.events = {};
+                for (e in j)
+                    for (c = 0, d = j[e].length; d > c; c++) n.event.add(b, e, j[e][c])
             }
-            return e
-        },
-        has: function(a) {
-            var b = f(a);
-            return this.filter(function() {
-                for (var a = 0, c = b.length; a < c; a++)
-                    if (f.contains(this, b[a])) return !0
-            })
-        },
-        not: function(a) {
-            return this.pushStack(T(this, a, !1), "not", a)
-        },
-        filter: function(a) {
-            return this.pushStack(T(this, a, !0), "filter", a)
+            O.hasData(a) && (h = O.access(a), i = n.extend({}, h), O.set(b, i))
+        }
+    }
+
+    function ta(a, b) {
+        var c = b.nodeName.toLowerCase();
+        "input" === c && X.test(a.type) ? b.checked = a.checked : "input" !== c && "textarea" !== c || (b.defaultValue = a.defaultValue)
+    }
+
+    function ua(a, b, c, d) {
+        b = f.apply([], b);
+        var e, g, h, i, j, k, m = 0,
+            o = a.length,
+            p = o - 1,
+            q = b[0],
+            r = n.isFunction(q);
+        if (r || o > 1 && "string" == typeof q && !l.checkClone && ma.test(q)) return a.each(function(e) {
+            var f = a.eq(e);
+            r && (b[0] = q.call(this, e, f.html())), ua(f, b, c, d)
+        });
+        if (o && (e = ca(b, a[0].ownerDocument, !1, a, d), g = e.firstChild, 1 === e.childNodes.length && (e = g), g || d)) {
+            for (h = n.map(_(e, "script"), qa), i = h.length; o > m; m++) j = e, m !== p && (j = n.clone(j, !0, !0), i && n.merge(h, _(j, "script"))), c.call(a[m], j, m);
+            if (i)
+                for (k = h[h.length - 1].ownerDocument, n.map(h, ra), m = 0; i > m; m++) j = h[m], Z.test(j.type || "") && !N.access(j, "globalEval") && n.contains(k, j) && (j.src ? n._evalUrl && n._evalUrl(j.src) : n.globalEval(j.textContent.replace(oa, "")))
+        }
+        return a
+    }
+
+    function va(a, b, c) {
+        for (var d, e = b ? n.filter(b, a) : a, f = 0; null != (d = e[f]); f++) c || 1 !== d.nodeType || n.cleanData(_(d)), d.parentNode && (c && n.contains(d.ownerDocument, d) && aa(_(d, "script")), d.parentNode.removeChild(d));
+        return a
+    }
+    n.extend({
+        htmlPrefilter: function(a) {
+            return a.replace(ka, "<$1></$2>")
         },
-        is: function(a) {
-            return !!a && (typeof a == "string" ? Q.test(a) ? f(a, this.context).index(this[0]) >= 0 : f.filter(a, this).length > 0 : this.filter(a).length > 0)
+        clone: function(a, b, c) {
+            var d, e, f, g, h = a.cloneNode(!0),
+                i = n.contains(a.ownerDocument, a);
+            if (!(l.noCloneChecked || 1 !== a.nodeType && 11 !== a.nodeType || n.isXMLDoc(a)))
+                for (g = _(h), f = _(a), d = 0, e = f.length; e > d; d++) ta(f[d], g[d]);
+            if (b)
+                if (c)
+                    for (f = f || _(a), g = g || _(h), d = 0, e = f.length; e > d; d++) sa(f[d], g[d]);
+                else sa(a, h);
+            return g = _(h, "script"), g.length > 0 && aa(g, !i && _(a, "script")), h
         },
-        closest: function(a, b) {
-            var c = [],
-                d, e, g = this[0];
-            if (f.isArray(a)) {
-                var h = 1;
-                while (g && g.ownerDocument && g !== b) {
-                    for (d = 0; d < a.length; d++) f(g).is(a[d]) && c.push({
-                        selector: a[d],
-                        elem: g,
-                        level: h
-                    });
-                    g = g.parentNode, h++
-                }
-                return c
-            }
-            var i = Q.test(a) || typeof a != "string" ? f(a, b || this.context) : 0;
-            for (d = 0, e = this.length; d < e; d++) {
-                g = this[d];
-                while (g) {
-                    if (i ? i.index(g) > -1 : f.find.matchesSelector(g, a)) {
-                        c.push(g);
-                        break
+        cleanData: function(a) {
+            for (var b, c, d, e = n.event.special, f = 0; void 0 !== (c = a[f]); f++)
+                if (L(c)) {
+                    if (b = c[N.expando]) {
+                        if (b.events)
+                            for (d in b.events) e[d] ? n.event.remove(c, d) : n.removeEvent(c, d, b.handle);
+                        c[N.expando] = void 0
                     }
-                    g = g.parentNode;
-                    if (!g || !g.ownerDocument || g === b || g.nodeType === 11) break
+                    c[O.expando] && (c[O.expando] = void 0)
                 }
-            }
-            c = c.length > 1 ? f.unique(c) : c;
-            return this.pushStack(c, "closest", a)
-        },
-        index: function(a) {
-            if (!a) return this[0] && this[0].parentNode ? this.prevAll().length : -1;
-            if (typeof a == "string") return f.inArray(this[0], f(a));
-            return f.inArray(a.jquery ? a[0] : a, this)
-        },
-        add: function(a, b) {
-            var c = typeof a == "string" ? f(a, b) : f.makeArray(a && a.nodeType ? [a] : a),
-                d = f.merge(this.get(), c);
-            return this.pushStack(S(c[0]) || S(d[0]) ? d : f.unique(d))
-        },
-        andSelf: function() {
-            return this.add(this.prevObject)
-        }
-    }), f.each({
-        parent: function(a) {
-            var b = a.parentNode;
-            return b && b.nodeType !== 11 ? b : null
-        },
-        parents: function(a) {
-            return f.dir(a, "parentNode")
-        },
-        parentsUntil: function(a, b, c) {
-            return f.dir(a, "parentNode", c)
-        },
-        next: function(a) {
-            return f.nth(a, 2, "nextSibling")
-        },
-        prev: function(a) {
-            return f.nth(a, 2, "previousSibling")
-        },
-        nextAll: function(a) {
-            return f.dir(a, "nextSibling")
-        },
-        prevAll: function(a) {
-            return f.dir(a, "previousSibling")
-        },
-        nextUntil: function(a, b, c) {
-            return f.dir(a, "nextSibling", c)
-        },
-        prevUntil: function(a, b, c) {
-            return f.dir(a, "previousSibling", c)
-        },
-        siblings: function(a) {
-            return f.sibling(a.parentNode.firstChild, a)
-        },
-        children: function(a) {
-            return f.sibling(a.firstChild)
-        },
-        contents: function(a) {
-            return f.nodeName(a, "iframe") ? a.contentDocument || a.contentWindow.document : f.makeArray(a.childNodes)
         }
-    }, function(a, b) {
-        f.fn[a] = function(c, d) {
-            var e = f.map(this, b, c);
-            L.test(a) || (d = c), d && typeof d == "string" && (e = f.filter(d, e)), e = this.length > 1 && !R[a] ? f.unique(e) : e, (this.length > 1 || N.test(d)) && M.test(a) && (e = e.reverse());
-            return this.pushStack(e, a, P.call(arguments).join(","))
-        }
-    }), f.extend({
-        filter: function(a, b, c) {
-            c && (a = ":not(" + a + ")");
-            return b.length === 1 ? f.find.matchesSelector(b[0], a) ? [b[0]] : [] : f.find.matches(a, b)
-        },
-        dir: function(a, c, d) {
-            var e = [],
-                g = a[c];
-            while (g && g.nodeType !== 9 && (d === b || g.nodeType !== 1 || !f(g).is(d))) g.nodeType === 1 && e.push(g), g = g[c];
-            return e
+    }), n.fn.extend({
+        domManip: ua,
+        detach: function(a) {
+            return va(this, a, !0)
         },
-        nth: function(a, b, c, d) {
-            b = b || 1;
-            var e = 0;
-            for (; a; a = a[c])
-                if (a.nodeType === 1 && ++e === b) break;
-            return a
+        remove: function(a) {
+            return va(this, a)
         },
-        sibling: function(a, b) {
-            var c = [];
-            for (; a; a = a.nextSibling) a.nodeType === 1 && a !== b && c.push(a);
-            return c
-        }
-    });
-    var V = "abbr|article|aside|audio|canvas|datalist|details|figcaption|figure|footer|header|hgroup|mark|meter|nav|output|progress|section|summary|time|video",
-        W = / jQuery\d+="(?:\d+|null)"/g,
-        X = /^\s+/,
-        Y = /<(?!area|br|col|embed|hr|img|input|link|meta|param)(([\w:]+)[^>]*)\/>/ig,
-        Z = /<([\w:]+)/,
-        $ = /<tbody/i,
-        _ = /<|&#?\w+;/,
-        ba = /<(?:script|style)/i,
-        bb = /<(?:script|object|embed|option|style)/i,
-        bc = new RegExp("<(?:" + V + ")", "i"),
-        bd = /checked\s*(?:[^=]|=\s*.checked.)/i,
-        be = /\/(java|ecma)script/i,
-        bf = /^\s*<!(?:\[CDATA\[|\-\-)/,
-        bg = {
-            option: [1, "<select multiple='multiple'>", "</select>"],
-            legend: [1, "<fieldset>", "</fieldset>"],
-            thead: [1, "<table>", "</table>"],
-            tr: [2, "<table><tbody>", "</tbody></table>"],
-            td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
-            col: [2, "<table><tbody></tbody><colgroup>", "</colgroup></table>"],
-            area: [1, "<map>", "</map>"],
-            _default: [0, "", ""]
-        },
-        bh = U(c);
-    bg.optgroup = bg.option, bg.tbody = bg.tfoot = bg.colgroup = bg.caption = bg.thead, bg.th = bg.td, f.support.htmlSerialize || (bg._default = [1, "div<div>", "</div>"]), f.fn.extend({
         text: function(a) {
-            if (f.isFunction(a)) return this.each(function(b) {
-                var c = f(this);
-                c.text(a.call(this, b, c.text()))
-            });
-            if (typeof a != "object" && a !== b) return this.empty().append((this[0] && this[0].ownerDocument || c).createTextNode(a));
-            return f.text(this)
-        },
-        wrapAll: function(a) {
-            if (f.isFunction(a)) return this.each(function(b) {
-                f(this).wrapAll(a.call(this, b))
-            });
-            if (this[0]) {
-                var b = f(a, this[0].ownerDocument).eq(0).clone(!0);
-                this[0].parentNode && b.insertBefore(this[0]), b.map(function() {
-                    var a = this;
-                    while (a.firstChild && a.firstChild.nodeType === 1) a = a.firstChild;
-                    return a
-                }).append(this)
-            }
-            return this
-        },
-        wrapInner: function(a) {
-            if (f.isFunction(a)) return this.each(function(b) {
-                f(this).wrapInner(a.call(this, b))
-            });
-            return this.each(function() {
-                var b = f(this),
-                    c = b.contents();
-                c.length ? c.wrapAll(a) : b.append(a)
-            })
-        },
-        wrap: function(a) {
-            var b = f.isFunction(a);
-            return this.each(function(c) {
-                f(this).wrapAll(b ? a.call(this, c) : a)
-            })
-        },
-        unwrap: function() {
-            return this.parent().each(function() {
-                f.nodeName(this, "body") || f(this).replaceWith(this.childNodes)
-            }).end()
+            return K(this, function(a) {
+                return void 0 === a ? n.text(this) : this.empty().each(function() {
+                    1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || (this.textContent = a)
+                })
+            }, null, a, arguments.length)
         },
         append: function() {
-            return this.domManip(arguments, !0, function(a) {
-                this.nodeType === 1 && this.appendChild(a)
+            return ua(this, arguments, function(a) {
+                if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
+                    var b = pa(this, a);
+                    b.appendChild(a)
+                }
             })
         },
         prepend: function() {
-            return this.domManip(arguments, !0, function(a) {
-                this.nodeType === 1 && this.insertBefore(a, this.firstChild)
+            return ua(this, arguments, function(a) {
+                if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
+                    var b = pa(this, a);
+                    b.insertBefore(a, b.firstChild)
+                }
             })
         },
         before: function() {
-            if (this[0] && this[0].parentNode) return this.domManip(arguments, !1, function(a) {
-                this.parentNode.insertBefore(a, this)
-            });
-            if (arguments.length) {
-                var a = f.clean(arguments);
-                a.push.apply(a, this.toArray());
-                return this.pushStack(a, "before", arguments)
-            }
+            return ua(this, arguments, function(a) {
+                this.parentNode && this.parentNode.insertBefore(a, this)
+            })
         },
         after: function() {
-            if (this[0] && this[0].parentNode) return this.domManip(arguments, !1, function(a) {
-                this.parentNode.insertBefore(a, this.nextSibling)
-            });
-            if (arguments.length) {
-                var a = this.pushStack(this, "after", arguments);
-                a.push.apply(a, f.clean(arguments));
-                return a
-            }
-        },
-        remove: function(a, b) {
-            for (var c = 0, d;
-                (d = this[c]) != null; c++)
-                if (!a || f.filter(a, [d]).length) !b && d.nodeType === 1 && (f.cleanData(d.getElementsByTagName("*")), f.cleanData([d])), d.parentNode && d.parentNode.removeChild(d);
-            return this
+            return ua(this, arguments, function(a) {
+                this.parentNode && this.parentNode.insertBefore(a, this.nextSibling)
+            })
         },
         empty: function() {
-            for (var a = 0, b;
-                (b = this[a]) != null; a++) {
-                b.nodeType === 1 && f.cleanData(b.getElementsByTagName("*"));
-                while (b.firstChild) b.removeChild(b.firstChild)
-            }
+            for (var a, b = 0; null != (a = this[b]); b++) 1 === a.nodeType && (n.cleanData(_(a, !1)), a.textContent = "");
             return this
         },
         clone: function(a, b) {
-            a = a == null ? !1 : a, b = b == null ? a : b;
-            return this.map(function() {
-                return f.clone(this, a, b)
+            return a = null == a ? !1 : a, b = null == b ? a : b, this.map(function() {
+                return n.clone(this, a, b)
             })
         },
         html: function(a) {
-            if (a === b) return this[0] && this[0].nodeType === 1 ? this[0].innerHTML.replace(W, "") : null;
-            if (typeof a == "string" && !ba.test(a) && (f.support.leadingWhitespace || !X.test(a)) && !bg[(Z.exec(a) || ["", ""])[1].toLowerCase()]) {
-                a = a.replace(Y, "<$1></$2>");
-                try {
-                    for (var c = 0, d = this.length; c < d; c++) this[c].nodeType === 1 && (f.cleanData(this[c].getElementsByTagName("*")), this[c].innerHTML = a)
-                } catch (e) {
-                    this.empty().append(a)
-                }
-            } else f.isFunction(a) ? this.each(function(b) {
-                var c = f(this);
-                c.html(a.call(this, b, c.html()))
-            }) : this.empty().append(a);
-            return this
-        },
-        replaceWith: function(a) {
-            if (this[0] && this[0].parentNode) {
-                if (f.isFunction(a)) return this.each(function(b) {
-                    var c = f(this),
-                        d = c.html();
-                    c.replaceWith(a.call(this, b, d))
-                });
-                typeof a != "string" && (a = f(a).detach());
-                return this.each(function() {
-                    var b = this.nextSibling,
-                        c = this.parentNode;
-                    f(this).remove(), b ? f(b).before(a) : f(c).append(a)
-                })
-            }
-            return this.length ? this.pushStack(f(f.isFunction(a) ? a() : a), "replaceWith", a) : this
-        },
-        detach: function(a) {
-            return this.remove(a, !0)
-        },
-        domManip: function(a, c, d) {
-            var e, g, h, i, j = a[0],
-                k = [];
-            if (!f.support.checkClone && arguments.length === 3 && typeof j == "string" && bd.test(j)) return this.each(function() {
-                f(this).domManip(a, c, d, !0)
-            });
-            if (f.isFunction(j)) return this.each(function(e) {
-                var g = f(this);
-                a[0] = j.call(this, e, c ? g.html() : b), g.domManip(a, c, d)
-            });
-            if (this[0]) {
-                i = j && j.parentNode, f.support.parentNode && i && i.nodeType === 11 && i.childNodes.length === this.length ? e = {
-                    fragment: i
-                } : e = f.buildFragment(a, this, k), h = e.fragment, h.childNodes.length === 1 ? g = h = h.firstChild : g = h.firstChild;
-                if (g) {
-                    c = c && f.nodeName(g, "tr");
-                    for (var l = 0, m = this.length, n = m - 1; l < m; l++) d.call(c ? bi(this[l], g) : this[l], e.cacheable || m > 1 && l < n ? f.clone(h, !0, !0) : h)
-                }
-                k.length && f.each(k, bp)
-            }
-            return this
-        }
-    }), f.buildFragment = function(a, b, d) {
-        var e, g, h, i, j = a[0];
-        b && b[0] && (i = b[0].ownerDocument || b[0]), i.createDocumentFragment || (i = c), a.length === 1 && typeof j == "string" && j.length < 512 && i === c && j.charAt(0) === "<" && !bb.test(j) && (f.support.checkClone || !bd.test(j)) && (f.support.html5Clone || !bc.test(j)) && (g = !0, h = f.fragments[j], h && h !== 1 && (e = h)), e || (e = i.createDocumentFragment(), f.clean(a, i, e, d)), g && (f.fragments[j] = h ? e : 1);
-        return {
-            fragment: e,
-            cacheable: g
+            return K(this, function(a) {
+                var b = this[0] || {},
+                    c = 0,
+                    d = this.length;
+                if (void 0 === a && 1 === b.nodeType) return b.innerHTML;
+                if ("string" == typeof a && !la.test(a) && !$[(Y.exec(a) || ["", ""])[1].toLowerCase()]) {
+                    a = n.htmlPrefilter(a);
+                    try {
+                        for (; d > c; c++) b = this[c] || {}, 1 === b.nodeType && (n.cleanData(_(b, !1)), b.innerHTML = a);
+                        b = 0
+                    } catch (e) {}
+                }
+                b && this.empty().append(a)
+            }, null, a, arguments.length)
+        },
+        replaceWith: function() {
+            var a = [];
+            return ua(this, arguments, function(b) {
+                var c = this.parentNode;
+                n.inArray(this, a) < 0 && (n.cleanData(_(this)), c && c.replaceChild(b, this))
+            }, a)
         }
-    }, f.fragments = {}, f.each({
+    }), n.each({
         appendTo: "append",
         prependTo: "prepend",
         insertBefore: "before",
         insertAfter: "after",
         replaceAll: "replaceWith"
     }, function(a, b) {
-        f.fn[a] = function(c) {
-            var d = [],
-                e = f(c),
-                g = this.length === 1 && this[0].parentNode;
-            if (g && g.nodeType === 11 && g.childNodes.length === 1 && e.length === 1) {
-                e[b](this[0]);
-                return this
-            }
-            for (var h = 0, i = e.length; h < i; h++) {
-                var j = (h > 0 ? this.clone(!0) : this).get();
-                f(e[h])[b](j), d = d.concat(j)
-            }
-            return this.pushStack(d, a, e.selector)
+        n.fn[a] = function(a) {
+            for (var c, d = [], e = n(a), f = e.length - 1, h = 0; f >= h; h++) c = h === f ? this : this.clone(!0), n(e[h])[b](c), g.apply(d, c.get());
+            return this.pushStack(d)
         }
-    }), f.extend({
-        clone: function(a, b, c) {
-            var d, e, g, h = f.support.html5Clone || !bc.test("<" + a.nodeName) ? a.cloneNode(!0) : bo(a);
-            if ((!f.support.noCloneEvent || !f.support.noCloneChecked) && (a.nodeType === 1 || a.nodeType === 11) && !f.isXMLDoc(a)) {
-                bk(a, h), d = bl(a), e = bl(h);
-                for (g = 0; d[g]; ++g) e[g] && bk(d[g], e[g])
-            }
-            if (b) {
-                bj(a, h);
-                if (c) {
-                    d = bl(a), e = bl(h);
-                    for (g = 0; d[g]; ++g) bj(d[g], e[g])
-                }
-            }
-            d = e = null;
-            return h
-        },
-        clean: function(a, b, d, e) {
-            var g;
-            b = b || c, typeof b.createElement == "undefined" && (b = b.ownerDocument || b[0] && b[0].ownerDocument || c);
-            var h = [],
-                i;
-            for (var j = 0, k;
-                (k = a[j]) != null; j++) {
-                typeof k == "number" && (k += "");
-                if (!k) continue;
-                if (typeof k == "string")
-                    if (!_.test(k)) k = b.createTextNode(k);
-                    else {
-                        k = k.replace(Y, "<$1></$2>");
-                        var l = (Z.exec(k) || ["", ""])[1].toLowerCase(),
-                            m = bg[l] || bg._default,
-                            n = m[0],
-                            o = b.createElement("div");
-                        b === c ? bh.appendChild(o) : U(b).appendChild(o), o.innerHTML = m[1] + k + m[2];
-                        while (n--) o = o.lastChild;
-                        if (!f.support.tbody) {
-                            var p = $.test(k),
-                                q = l === "table" && !p ? o.firstChild && o.firstChild.childNodes : m[1] === "<table>" && !p ? o.childNodes : [];
-                            for (i = q.length - 1; i >= 0; --i) f.nodeName(q[i], "tbody") && !q[i].childNodes.length && q[i].parentNode.removeChild(q[i])
-                        }!f.support.leadingWhitespace && X.test(k) && o.insertBefore(b.createTextNode(X.exec(k)[0]), o.firstChild), k = o.childNodes
-                    } var r;
-                if (!f.support.appendChecked)
-                    if (k[0] && typeof(r = k.length) == "number")
-                        for (i = 0; i < r; i++) bn(k[i]);
-                    else bn(k);
-                k.nodeType ? h.push(k) : h = f.merge(h, k)
-            }
-            if (d) {
-                g = function(a) {
-                    return !a.type || be.test(a.type)
-                };
-                for (j = 0; h[j]; j++)
-                    if (e && f.nodeName(h[j], "script") && (!h[j].type || h[j].type.toLowerCase() === "text/javascript")) e.push(h[j].parentNode ? h[j].parentNode.removeChild(h[j]) : h[j]);
-                    else {
-                        if (h[j].nodeType === 1) {
-                            var s = f.grep(h[j].getElementsByTagName("script"), g);
-                            h.splice.apply(h, [j + 1, 0].concat(s))
-                        }
-                        d.appendChild(h[j])
-                    }
-            }
-            return h
+    });
+    var wa, xa = {
+        HTML: "block",
+        BODY: "block"
+    };
+
+    function ya(a, b) {
+        var c = n(b.createElement(a)).appendTo(b.body),
+            d = n.css(c[0], "display");
+        return c.detach(), d
+    }
+
+    function za(a) {
+        var b = d,
+            c = xa[a];
+        return c || (c = ya(a, b), "none" !== c && c || (wa = (wa || n("<iframe frameborder='0' width='0' height='0'/>")).appendTo(b.documentElement), b = wa[0].contentDocument, b.write(), b.close(), c = ya(a, b), wa.detach()), xa[a] = c), c
+    }
+    var Aa = /^margin/,
+        Ba = new RegExp("^(" + S + ")(?!px)[a-z%]+$", "i"),
+        Ca = function(b) {
+            var c = b.ownerDocument.defaultView;
+            return c && c.opener || (c = a), c.getComputedStyle(b)
+        },
+        Da = function(a, b, c, d) {
+            var e, f, g = {};
+            for (f in b) g[f] = a.style[f], a.style[f] = b[f];
+            e = c.apply(a, d || []);
+            for (f in b) a.style[f] = g[f];
+            return e
         },
-        cleanData: function(a) {
-            var b, c, d = f.cache,
-                e = f.event.special,
-                g = f.support.deleteExpando;
-            for (var h = 0, i;
-                (i = a[h]) != null; h++) {
-                if (i.nodeName && f.noData[i.nodeName.toLowerCase()]) continue;
-                c = i[f.expando];
-                if (c) {
-                    b = d[c];
-                    if (b && b.events) {
-                        for (var j in b.events) e[j] ? f.event.remove(i, j) : f.removeEvent(i, j, b.handle);
-                        b.handle && (b.handle.elem = null)
-                    }
-                    g ? delete i[f.expando] : i.removeAttribute && i.removeAttribute(f.expando), delete d[c]
+        Ea = d.documentElement;
+    ! function() {
+        var b, c, e, f, g = d.createElement("div"),
+            h = d.createElement("div");
+        if (h.style) {
+            h.style.backgroundClip = "content-box", h.cloneNode(!0).style.backgroundClip = "", l.clearCloneStyle = "content-box" === h.style.backgroundClip, g.style.cssText = "border:0;width:8px;height:0;top:0;left:-9999px;padding:0;margin-top:1px;position:absolute", g.appendChild(h);
+
+            function i() {
+                h.style.cssText = "-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;position:relative;display:block;margin:auto;border:1px;padding:1px;top:1%;width:50%", h.innerHTML = "", Ea.appendChild(g);
+                var d = a.getComputedStyle(h);
+                b = "1%" !== d.top, f = "2px" === d.marginLeft, c = "4px" === d.width, h.style.marginRight = "50%", e = "4px" === d.marginRight, Ea.removeChild(g)
+            }
+            n.extend(l, {
+                pixelPosition: function() {
+                    return i(), b
+                },
+                boxSizingReliable: function() {
+                    return null == c && i(), c
+                },
+                pixelMarginRight: function() {
+                    return null == c && i(), e
+                },
+                reliableMarginLeft: function() {
+                    return null == c && i(), f
+                },
+                reliableMarginRight: function() {
+                    var b, c = h.appendChild(d.createElement("div"));
+                    return c.style.cssText = h.style.cssText = "-webkit-box-sizing:content-box;box-sizing:content-box;display:block;margin:0;border:0;padding:0", c.style.marginRight = c.style.width = "0", h.style.width = "1px", Ea.appendChild(g), b = !parseFloat(a.getComputedStyle(c).marginRight), Ea.removeChild(g), h.removeChild(c), b
                 }
+            })
+        }
+    }();
+
+    function Fa(a, b, c) {
+        var d, e, f, g, h = a.style;
+        return c = c || Ca(a), g = c ? c.getPropertyValue(b) || c[b] : void 0, "" !== g && void 0 !== g || n.contains(a.ownerDocument, a) || (g = n.style(a, b)), c && !l.pixelMarginRight() && Ba.test(g) && Aa.test(b) && (d = h.width, e = h.minWidth, f = h.maxWidth, h.minWidth = h.maxWidth = h.width = g, g = c.width, h.width = d, h.minWidth = e, h.maxWidth = f), void 0 !== g ? g + "" : g
+    }
+
+    function Ga(a, b) {
+        return {
+            get: function() {
+                return a() ? void delete this.get : (this.get = b).apply(this, arguments)
             }
         }
-    });
-    var bq = /alpha\([^)]*\)/i,
-        br = /opacity=([^)]*)/,
-        bs = /([A-Z]|^ms)/g,
-        bt = /^-?\d+(?:px)?$/i,
-        bu = /^-?\d/,
-        bv = /^([\-+])=([\-+.\de]+)/,
-        bw = {
+    }
+    var Ha = /^(none|table(?!-c[ea]).+)/,
+        Ia = {
             position: "absolute",
             visibility: "hidden",
             display: "block"
         },
-        bx = ["Left", "Right"],
-        by = ["Top", "Bottom"],
-        bz, bA, bB;
-    f.fn.css = function(a, c) {
-        if (arguments.length === 2 && c === b) return this;
-        return f.access(this, a, c, !0, function(a, c, d) {
-            return d !== b ? f.style(a, c, d) : f.css(a, c)
-        })
-    }, f.extend({
+        Ja = {
+            letterSpacing: "0",
+            fontWeight: "400"
+        },
+        Ka = ["Webkit", "O", "Moz", "ms"],
+        La = d.createElement("div").style;
+
+    function Ma(a) {
+        if (a in La) return a;
+        var b = a[0].toUpperCase() + a.slice(1),
+            c = Ka.length;
+        while (c--)
+            if (a = Ka[c] + b, a in La) return a
+    }
+
+    function Na(a, b, c) {
+        var d = T.exec(b);
+        return d ? Math.max(0, d[2] - (c || 0)) + (d[3] || "px") : b
+    }
+
+    function Oa(a, b, c, d, e) {
+        for (var f = c === (d ? "border" : "content") ? 4 : "width" === b ? 1 : 0, g = 0; 4 > f; f += 2) "margin" === c && (g += n.css(a, c + U[f], !0, e)), d ? ("content" === c && (g -= n.css(a, "padding" + U[f], !0, e)), "margin" !== c && (g -= n.css(a, "border" + U[f] + "Width", !0, e))) : (g += n.css(a, "padding" + U[f], !0, e), "padding" !== c && (g += n.css(a, "border" + U[f] + "Width", !0, e)));
+        return g
+    }
+
+    function Pa(a, b, c) {
+        var d = !0,
+            e = "width" === b ? a.offsetWidth : a.offsetHeight,
+            f = Ca(a),
+            g = "border-box" === n.css(a, "boxSizing", !1, f);
+        if (0 >= e || null == e) {
+            if (e = Fa(a, b, f), (0 > e || null == e) && (e = a.style[b]), Ba.test(e)) return e;
+            d = g && (l.boxSizingReliable() || e === a.style[b]), e = parseFloat(e) || 0
+        }
+        return e + Oa(a, b, c || (g ? "border" : "content"), d, f) + "px"
+    }
+
+    function Qa(a, b) {
+        for (var c, d, e, f = [], g = 0, h = a.length; h > g; g++) d = a[g], d.style && (f[g] = N.get(d, "olddisplay"), c = d.style.display, b ? (f[g] || "none" !== c || (d.style.display = ""), "" === d.style.display && V(d) && (f[g] = N.access(d, "olddisplay", za(d.nodeName)))) : (e = V(d), "none" === c && e || N.set(d, "olddisplay", e ? c : n.css(d, "display"))));
+        for (g = 0; h > g; g++) d = a[g], d.style && (b && "none" !== d.style.display && "" !== d.style.display || (d.style.display = b ? f[g] || "" : "none"));
+        return a
+    }
+    n.extend({
         cssHooks: {
             opacity: {
                 get: function(a, b) {
                     if (b) {
-                        var c = bz(a, "opacity", "opacity");
-                        return c === "" ? "1" : c
+                        var c = Fa(a, "opacity");
+                        return "" === c ? "1" : c
                     }
-                    return a.style.opacity
                 }
             }
         },
         cssNumber: {
+            animationIterationCount: !0,
+            columnCount: !0,
             fillOpacity: !0,
+            flexGrow: !0,
+            flexShrink: !0,
             fontWeight: !0,
             lineHeight: !0,
             opacity: !0,
+            order: !0,
             orphans: !0,
             widows: !0,
             zIndex: !0,
             zoom: !0
         },
         cssProps: {
-            "float": f.support.cssFloat ? "cssFloat" : "styleFloat"
+            "float": "cssFloat"
         },
-        style: function(a, c, d, e) {
-            if (!!a && a.nodeType !== 3 && a.nodeType !== 8 && !!a.style) {
-                var g, h, i = f.camelCase(c),
-                    j = a.style,
-                    k = f.cssHooks[i];
-                c = f.cssProps[i] || i;
-                if (d === b) {
-                    if (k && "get" in k && (g = k.get(a, !1, e)) !== b) return g;
-                    return j[c]
-                }
-                h = typeof d, h === "string" && (g = bv.exec(d)) && (d = +(g[1] + 1) * +g[2] + parseFloat(f.css(a, c)), h = "number");
-                if (d == null || h === "number" && isNaN(d)) return;
-                h === "number" && !f.cssNumber[i] && (d += "px");
-                if (!k || !("set" in k) || (d = k.set(a, d)) !== b) try {
-                    j[c] = d
-                } catch (l) {}
-            }
-        },
-        css: function(a, c, d) {
-            var e, g;
-            c = f.camelCase(c), g = f.cssHooks[c], c = f.cssProps[c] || c, c === "cssFloat" && (c = "float");
-            if (g && "get" in g && (e = g.get(a, !0, d)) !== b) return e;
-            if (bz) return bz(a, c)
-        },
-        swap: function(a, b, c) {
-            var d = {};
-            for (var e in b) d[e] = a.style[e], a.style[e] = b[e];
-            c.call(a);
-            for (e in b) a.style[e] = d[e]
+        style: function(a, b, c, d) {
+            if (a && 3 !== a.nodeType && 8 !== a.nodeType && a.style) {
+                var e, f, g, h = n.camelCase(b),
+                    i = a.style;
+                return b = n.cssProps[h] || (n.cssProps[h] = Ma(h) || h), g = n.cssHooks[b] || n.cssHooks[h], void 0 === c ? g && "get" in g && void 0 !== (e = g.get(a, !1, d)) ? e : i[b] : (f = typeof c, "string" === f && (e = T.exec(c)) && e[1] && (c = W(a, b, e), f = "number"), null != c && c === c && ("number" === f && (c += e && e[3] || (n.cssNumber[h] ? "" : "px")), l.clearCloneStyle || "" !== c || 0 !== b.indexOf("background") || (i[b] = "inherit"), g && "set" in g && void 0 === (c = g.set(a, c, d)) || (i[b] = c)), void 0)
+            }
+        },
+        css: function(a, b, c, d) {
+            var e, f, g, h = n.camelCase(b);
+            return b = n.cssProps[h] || (n.cssProps[h] = Ma(h) || h), g = n.cssHooks[b] || n.cssHooks[h], g && "get" in g && (e = g.get(a, !0, c)), void 0 === e && (e = Fa(a, b, d)), "normal" === e && b in Ja && (e = Ja[b]), "" === c || c ? (f = parseFloat(e), c === !0 || isFinite(f) ? f || 0 : e) : e
         }
-    }), f.curCSS = f.css, f.each(["height", "width"], function(a, b) {
-        f.cssHooks[b] = {
+    }), n.each(["height", "width"], function(a, b) {
+        n.cssHooks[b] = {
             get: function(a, c, d) {
-                var e;
-                if (c) {
-                    if (a.offsetWidth !== 0) return bC(a, b, d);
-                    f.swap(a, bw, function() {
-                        e = bC(a, b, d)
-                    });
-                    return e
+                return c ? Ha.test(n.css(a, "display")) && 0 === a.offsetWidth ? Da(a, Ia, function() {
+                    return Pa(a, b, d)
+                }) : Pa(a, b, d) : void 0
+            },
+            set: function(a, c, d) {
+                var e, f = d && Ca(a),
+                    g = d && Oa(a, b, d, "border-box" === n.css(a, "boxSizing", !1, f), f);
+                return g && (e = T.exec(c)) && "px" !== (e[3] || "px") && (a.style[b] = c, c = n.css(a, b)), Na(a, c, g)
+            }
+        }
+    }), n.cssHooks.marginLeft = Ga(l.reliableMarginLeft, function(a, b) {
+        return b ? (parseFloat(Fa(a, "marginLeft")) || a.getBoundingClientRect().left - Da(a, {
+            marginLeft: 0
+        }, function() {
+            return a.getBoundingClientRect().left
+        })) + "px" : void 0
+    }), n.cssHooks.marginRight = Ga(l.reliableMarginRight, function(a, b) {
+        return b ? Da(a, {
+            display: "inline-block"
+        }, Fa, [a, "marginRight"]) : void 0
+    }), n.each({
+        margin: "",
+        padding: "",
+        border: "Width"
+    }, function(a, b) {
+        n.cssHooks[a + b] = {
+            expand: function(c) {
+                for (var d = 0, e = {}, f = "string" == typeof c ? c.split(" ") : [c]; 4 > d; d++) e[a + U[d] + b] = f[d] || f[d - 2] || f[0];
+                return e
+            }
+        }, Aa.test(a) || (n.cssHooks[a + b].set = Na)
+    }), n.fn.extend({
+        css: function(a, b) {
+            return K(this, function(a, b, c) {
+                var d, e, f = {},
+                    g = 0;
+                if (n.isArray(b)) {
+                    for (d = Ca(a), e = b.length; e > g; g++) f[b[g]] = n.css(a, b[g], !1, d);
+                    return f
                 }
+                return void 0 !== c ? n.style(a, b, c) : n.css(a, b)
+            }, a, b, arguments.length > 1)
+        },
+        show: function() {
+            return Qa(this, !0)
+        },
+        hide: function() {
+            return Qa(this)
+        },
+        toggle: function(a) {
+            return "boolean" == typeof a ? a ? this.show() : this.hide() : this.each(function() {
+                V(this) ? n(this).show() : n(this).hide()
+            })
+        }
+    });
+
+    function Ra(a, b, c, d, e) {
+        return new Ra.prototype.init(a, b, c, d, e)
+    }
+    n.Tween = Ra, Ra.prototype = {
+        constructor: Ra,
+        init: function(a, b, c, d, e, f) {
+            this.elem = a, this.prop = c, this.easing = e || n.easing._default, this.options = b, this.start = this.now = this.cur(), this.end = d, this.unit = f || (n.cssNumber[c] ? "" : "px")
+        },
+        cur: function() {
+            var a = Ra.propHooks[this.prop];
+            return a && a.get ? a.get(this) : Ra.propHooks._default.get(this)
+        },
+        run: function(a) {
+            var b, c = Ra.propHooks[this.prop];
+            return this.options.duration ? this.pos = b = n.easing[this.easing](a, this.options.duration * a, 0, 1, this.options.duration) : this.pos = b = a, this.now = (this.end - this.start) * b + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), c && c.set ? c.set(this) : Ra.propHooks._default.set(this), this
+        }
+    }, Ra.prototype.init.prototype = Ra.prototype, Ra.propHooks = {
+        _default: {
+            get: function(a) {
+                var b;
+                return 1 !== a.elem.nodeType || null != a.elem[a.prop] && null == a.elem.style[a.prop] ? a.elem[a.prop] : (b = n.css(a.elem, a.prop, ""), b && "auto" !== b ? b : 0)
             },
-            set: function(a, b) {
-                if (!bt.test(b)) return b;
-                b = parseFloat(b);
-                if (b >= 0) return b + "px"
+            set: function(a) {
+                n.fx.step[a.prop] ? n.fx.step[a.prop](a) : 1 !== a.elem.nodeType || null == a.elem.style[n.cssProps[a.prop]] && !n.cssHooks[a.prop] ? a.elem[a.prop] = a.now : n.style(a.elem, a.prop, a.now + a.unit)
             }
         }
-    }), f.support.opacity || (f.cssHooks.opacity = {
-        get: function(a, b) {
-            return br.test((b && a.currentStyle ? a.currentStyle.filter : a.style.filter) || "") ? parseFloat(RegExp.$1) / 100 + "" : b ? "1" : ""
+    }, Ra.propHooks.scrollTop = Ra.propHooks.scrollLeft = {
+        set: function(a) {
+            a.elem.nodeType && a.elem.parentNode && (a.elem[a.prop] = a.now)
+        }
+    }, n.easing = {
+        linear: function(a) {
+            return a
         },
-        set: function(a, b) {
-            var c = a.style,
-                d = a.currentStyle,
-                e = f.isNumeric(b) ? "alpha(opacity=" + b * 100 + ")" : "",
-                g = d && d.filter || c.filter || "";
-            c.zoom = 1;
-            if (b >= 1 && f.trim(g.replace(bq, "")) === "") {
-                c.removeAttribute("filter");
-                if (d && !d.filter) return
-            }
-            c.filter = bq.test(g) ? g.replace(bq, e) : g + " " + e
-        }
-    }), f(function() {
-        f.support.reliableMarginRight || (f.cssHooks.marginRight = {
-            get: function(a, b) {
-                var c;
-                f.swap(a, {
-                    display: "inline-block"
-                }, function() {
-                    b ? c = bz(a, "margin-right", "marginRight") : c = a.style.marginRight
-                });
-                return c
+        swing: function(a) {
+            return .5 - Math.cos(a * Math.PI) / 2
+        },
+        _default: "swing"
+    }, n.fx = Ra.prototype.init, n.fx.step = {};
+    var Sa, Ta, Ua = /^(?:toggle|show|hide)$/,
+        Va = /queueHooks$/;
+
+    function Wa() {
+        return a.setTimeout(function() {
+            Sa = void 0
+        }), Sa = n.now()
+    }
+
+    function Xa(a, b) {
+        var c, d = 0,
+            e = {
+                height: a
+            };
+        for (b = b ? 1 : 0; 4 > d; d += 2 - b) c = U[d], e["margin" + c] = e["padding" + c] = a;
+        return b && (e.opacity = e.width = a), e
+    }
+
+    function Ya(a, b, c) {
+        for (var d, e = (_a.tweeners[b] || []).concat(_a.tweeners["*"]), f = 0, g = e.length; g > f; f++)
+            if (d = e[f].call(c, b, a)) return d
+    }
+
+    function Za(a, b, c) {
+        var d, e, f, g, h, i, j, k, l = this,
+            m = {},
+            o = a.style,
+            p = a.nodeType && V(a),
+            q = N.get(a, "fxshow");
+        c.queue || (h = n._queueHooks(a, "fx"), null == h.unqueued && (h.unqueued = 0, i = h.empty.fire, h.empty.fire = function() {
+            h.unqueued || i()
+        }), h.unqueued++, l.always(function() {
+            l.always(function() {
+                h.unqueued--, n.queue(a, "fx").length || h.empty.fire()
+            })
+        })), 1 === a.nodeType && ("height" in b || "width" in b) && (c.overflow = [o.overflow, o.overflowX, o.overflowY], j = n.css(a, "display"), k = "none" === j ? N.get(a, "olddisplay") || za(a.nodeName) : j, "inline" === k && "none" === n.css(a, "float") && (o.display = "inline-block")), c.overflow && (o.overflow = "hidden", l.always(function() {
+            o.overflow = c.overflow[0], o.overflowX = c.overflow[1], o.overflowY = c.overflow[2]
+        }));
+        for (d in b)
+            if (e = b[d], Ua.exec(e)) {
+                if (delete b[d], f = f || "toggle" === e, e === (p ? "hide" : "show")) {
+                    if ("show" !== e || !q || void 0 === q[d]) continue;
+                    p = !0
+                }
+                m[d] = q && q[d] || n.style(a, d)
+            } else j = void 0;
+        if (n.isEmptyObject(m)) "inline" === ("none" === j ? za(a.nodeName) : j) && (o.display = j);
+        else {
+            q ? "hidden" in q && (p = q.hidden) : q = N.access(a, "fxshow", {}), f && (q.hidden = !p), p ? n(a).show() : l.done(function() {
+                n(a).hide()
+            }), l.done(function() {
+                var b;
+                N.remove(a, "fxshow");
+                for (b in m) n.style(a, b, m[b])
+            });
+            for (d in m) g = Ya(p ? q[d] : 0, d, l), d in q || (q[d] = g.start, p && (g.end = g.start, g.start = "width" === d || "height" === d ? 1 : 0))
+        }
+    }
+
+    function $a(a, b) {
+        var c, d, e, f, g;
+        for (c in a)
+            if (d = n.camelCase(c), e = b[d], f = a[c], n.isArray(f) && (e = f[1], f = a[c] = f[0]), c !== d && (a[d] = f, delete a[c]), g = n.cssHooks[d], g && "expand" in g) {
+                f = g.expand(f), delete a[d];
+                for (c in f) c in a || (a[c] = f[c], b[c] = e)
+            } else b[d] = e
+    }
+
+    function _a(a, b, c) {
+        var d, e, f = 0,
+            g = _a.prefilters.length,
+            h = n.Deferred().always(function() {
+                delete i.elem
+            }),
+            i = function() {
+                if (e) return !1;
+                for (var b = Sa || Wa(), c = Math.max(0, j.startTime + j.duration - b), d = c / j.duration || 0, f = 1 - d, g = 0, i = j.tweens.length; i > g; g++) j.tweens[g].run(f);
+                return h.notifyWith(a, [j, f, c]), 1 > f && i ? c : (h.resolveWith(a, [j]), !1)
+            },
+            j = h.promise({
+                elem: a,
+                props: n.extend({}, b),
+                opts: n.extend(!0, {
+                    specialEasing: {},
+                    easing: n.easing._default
+                }, c),
+                originalProperties: b,
+                originalOptions: c,
+                startTime: Sa || Wa(),
+                duration: c.duration,
+                tweens: [],
+                createTween: function(b, c) {
+                    var d = n.Tween(a, j.opts, b, c, j.opts.specialEasing[b] || j.opts.easing);
+                    return j.tweens.push(d), d
+                },
+                stop: function(b) {
+                    var c = 0,
+                        d = b ? j.tweens.length : 0;
+                    if (e) return this;
+                    for (e = !0; d > c; c++) j.tweens[c].run(1);
+                    return b ? (h.notifyWith(a, [j, 1, 0]), h.resolveWith(a, [j, b])) : h.rejectWith(a, [j, b]), this
+                }
+            }),
+            k = j.props;
+        for ($a(k, j.opts.specialEasing); g > f; f++)
+            if (d = _a.prefilters[f].call(j, a, k, j.opts)) return n.isFunction(d.stop) && (n._queueHooks(j.elem, j.opts.queue).stop = n.proxy(d.stop, d)), d;
+        return n.map(k, Ya, j), n.isFunction(j.opts.start) && j.opts.start.call(a, j), n.fx.timer(n.extend(i, {
+            elem: a,
+            anim: j,
+            queue: j.opts.queue
+        })), j.progress(j.opts.progress).done(j.opts.done, j.opts.complete).fail(j.opts.fail).always(j.opts.always)
+    }
+    n.Animation = n.extend(_a, {
+            tweeners: {
+                "*": [function(a, b) {
+                    var c = this.createTween(a, b);
+                    return W(c.elem, a, T.exec(b), c), c
+                }]
+            },
+            tweener: function(a, b) {
+                n.isFunction(a) ? (b = a, a = ["*"]) : a = a.match(G);
+                for (var c, d = 0, e = a.length; e > d; d++) c = a[d], _a.tweeners[c] = _a.tweeners[c] || [], _a.tweeners[c].unshift(b)
+            },
+            prefilters: [Za],
+            prefilter: function(a, b) {
+                b ? _a.prefilters.unshift(a) : _a.prefilters.push(a)
+            }
+        }), n.speed = function(a, b, c) {
+            var d = a && "object" == typeof a ? n.extend({}, a) : {
+                complete: c || !c && b || n.isFunction(a) && a,
+                duration: a,
+                easing: c && b || b && !n.isFunction(b) && b
+            };
+            return d.duration = n.fx.off ? 0 : "number" == typeof d.duration ? d.duration : d.duration in n.fx.speeds ? n.fx.speeds[d.duration] : n.fx.speeds._default, null != d.queue && d.queue !== !0 || (d.queue = "fx"), d.old = d.complete, d.complete = function() {
+                n.isFunction(d.old) && d.old.call(this), d.queue && n.dequeue(this, d.queue)
+            }, d
+        }, n.fn.extend({
+            fadeTo: function(a, b, c, d) {
+                return this.filter(V).css("opacity", 0).show().end().animate({
+                    opacity: b
+                }, a, c, d)
+            },
+            animate: function(a, b, c, d) {
+                var e = n.isEmptyObject(a),
+                    f = n.speed(b, c, d),
+                    g = function() {
+                        var b = _a(this, n.extend({}, a), f);
+                        (e || N.get(this, "finish")) && b.stop(!0)
+                    };
+                return g.finish = g, e || f.queue === !1 ? this.each(g) : this.queue(f.queue, g)
+            },
+            stop: function(a, b, c) {
+                var d = function(a) {
+                    var b = a.stop;
+                    delete a.stop, b(c)
+                };
+                return "string" != typeof a && (c = b, b = a, a = void 0), b && a !== !1 && this.queue(a || "fx", []), this.each(function() {
+                    var b = !0,
+                        e = null != a && a + "queueHooks",
+                        f = n.timers,
+                        g = N.get(this);
+                    if (e) g[e] && g[e].stop && d(g[e]);
+                    else
+                        for (e in g) g[e] && g[e].stop && Va.test(e) && d(g[e]);
+                    for (e = f.length; e--;) f[e].elem !== this || null != a && f[e].queue !== a || (f[e].anim.stop(c), b = !1, f.splice(e, 1));
+                    !b && c || n.dequeue(this, a)
+                })
+            },
+            finish: function(a) {
+                return a !== !1 && (a = a || "fx"), this.each(function() {
+                    var b, c = N.get(this),
+                        d = c[a + "queue"],
+                        e = c[a + "queueHooks"],
+                        f = n.timers,
+                        g = d ? d.length : 0;
+                    for (c.finish = !0, n.queue(this, a, []), e && e.stop && e.stop.call(this, !0), b = f.length; b--;) f[b].elem === this && f[b].queue === a && (f[b].anim.stop(!0), f.splice(b, 1));
+                    for (b = 0; g > b; b++) d[b] && d[b].finish && d[b].finish.call(this);
+                    delete c.finish
+                })
             }
-        })
-    }), c.defaultView && c.defaultView.getComputedStyle && (bA = function(a, b) {
-        var c, d, e;
-        b = b.replace(bs, "-$1").toLowerCase(), (d = a.ownerDocument.defaultView) && (e = d.getComputedStyle(a, null)) && (c = e.getPropertyValue(b), c === "" && !f.contains(a.ownerDocument.documentElement, a) && (c = f.style(a, b)));
-        return c
-    }), c.documentElement.currentStyle && (bB = function(a, b) {
-        var c, d, e, f = a.currentStyle && a.currentStyle[b],
-            g = a.style;
-        f === null && g && (e = g[b]) && (f = e), !bt.test(f) && bu.test(f) && (c = g.left, d = a.runtimeStyle && a.runtimeStyle.left, d && (a.runtimeStyle.left = a.currentStyle.left), g.left = b === "fontSize" ? "1em" : f || 0, f = g.pixelLeft + "px", g.left = c, d && (a.runtimeStyle.left = d));
-        return f === "" ? "auto" : f
-    }), bz = bA || bB, f.expr && f.expr.filters && (f.expr.filters.hidden = function(a) {
-        var b = a.offsetWidth,
-            c = a.offsetHeight;
-        return b === 0 && c === 0 || !f.support.reliableHiddenOffsets && (a.style && a.style.display || f.css(a, "display")) === "none"
-    }, f.expr.filters.visible = function(a) {
-        return !f.expr.filters.hidden(a)
-    });
-    var bD = /%20/g,
-        bE = /\[\]$/,
-        bF = /\r?\n/g,
-        bG = /#.*$/,
-        bH = /^(.*?):[ \t]*([^\r\n]*)\r?$/mg,
-        bI = /^(?:color|date|datetime|datetime-local|email|hidden|month|number|password|range|search|tel|text|time|url|week)$/i,
-        bJ = /^(?:about|app|app\-storage|.+\-extension|file|res|widget):$/,
-        bK = /^(?:GET|HEAD)$/,
-        bL = /^\/\//,
-        bM = /\?/,
-        bN = /<script\b[^<]*(?:(?!<\/script>)<[^<]*)*<\/script>/gi,
-        bO = /^(?:select|textarea)/i,
-        bP = /\s+/,
-        bQ = /([?&])_=[^&]*/,
-        bR = /^([\w\+\.\-]+:)(?:\/\/([^\/?#:]*)(?::(\d+))?)?/,
-        bS = f.fn.load,
-        bT = {},
-        bU = {},
-        bV, bW, bX = ["*/"] + ["*"];
-    try {
-        bV = e.href
-    } catch (bY) {
-        bV = c.createElement("a"), bV.href = "", bV = bV.href
-    }
-    bW = bR.exec(bV.toLowerCase()) || [], f.fn.extend({
-        load: function(a, c, d) {
-            if (typeof a != "string" && bS) return bS.apply(this, arguments);
-            if (!this.length) return this;
-            var e = a.indexOf(" ");
-            if (e >= 0) {
-                var g = a.slice(e, a.length);
-                a = a.slice(0, e)
-            }
-            var h = "GET";
-            c && (f.isFunction(c) ? (d = c, c = b) : typeof c == "object" && (c = f.param(c, f.ajaxSettings.traditional), h = "POST"));
-            var i = this;
-            f.ajax({
-                url: a,
-                type: h,
-                dataType: "html",
-                data: c,
-                complete: function(a, b, c) {
-                    c = a.responseText, a.isResolved() && (a.done(function(a) {
-                        c = a
-                    }), i.html(g ? f("<div>").append(c.replace(bN, "")).find(g) : c)), d && i.each(d, [c, b, a])
+        }), n.each(["toggle", "show", "hide"], function(a, b) {
+            var c = n.fn[b];
+            n.fn[b] = function(a, d, e) {
+                return null == a || "boolean" == typeof a ? c.apply(this, arguments) : this.animate(Xa(b, !0), a, d, e)
+            }
+        }), n.each({
+            slideDown: Xa("show"),
+            slideUp: Xa("hide"),
+            slideToggle: Xa("toggle"),
+            fadeIn: {
+                opacity: "show"
+            },
+            fadeOut: {
+                opacity: "hide"
+            },
+            fadeToggle: {
+                opacity: "toggle"
+            }
+        }, function(a, b) {
+            n.fn[a] = function(a, c, d) {
+                return this.animate(b, a, c, d)
+            }
+        }), n.timers = [], n.fx.tick = function() {
+            var a, b = 0,
+                c = n.timers;
+            for (Sa = n.now(); b < c.length; b++) a = c[b], a() || c[b] !== a || c.splice(b--, 1);
+            c.length || n.fx.stop(), Sa = void 0
+        }, n.fx.timer = function(a) {
+            n.timers.push(a), a() ? n.fx.start() : n.timers.pop()
+        }, n.fx.interval = 13, n.fx.start = function() {
+            Ta || (Ta = a.setInterval(n.fx.tick, n.fx.interval))
+        }, n.fx.stop = function() {
+            a.clearInterval(Ta), Ta = null
+        }, n.fx.speeds = {
+            slow: 600,
+            fast: 200,
+            _default: 400
+        }, n.fn.delay = function(b, c) {
+            return b = n.fx ? n.fx.speeds[b] || b : b, c = c || "fx", this.queue(c, function(c, d) {
+                var e = a.setTimeout(c, b);
+                d.stop = function() {
+                    a.clearTimeout(e)
                 }
-            });
-            return this
+            })
         },
-        serialize: function() {
-            return f.param(this.serializeArray())
+        function() {
+            var a = d.createElement("input"),
+                b = d.createElement("select"),
+                c = b.appendChild(d.createElement("option"));
+            a.type = "checkbox", l.checkOn = "" !== a.value, l.optSelected = c.selected, b.disabled = !0, l.optDisabled = !c.disabled, a = d.createElement("input"), a.value = "t", a.type = "radio", l.radioValue = "t" === a.value
+        }();
+    var ab, bb = n.expr.attrHandle;
+    n.fn.extend({
+        attr: function(a, b) {
+            return K(this, n.attr, a, b, arguments.length > 1)
         },
-        serializeArray: function() {
-            return this.map(function() {
-                return this.elements ? f.makeArray(this.elements) : this
-            }).filter(function() {
-                return this.name && !this.disabled && (this.checked || bO.test(this.nodeName) || bI.test(this.type))
-            }).map(function(a, b) {
-                var c = f(this).val();
-                return c == null ? null : f.isArray(c) ? f.map(c, function(a, c) {
-                    return {
-                        name: b.name,
-                        value: a.replace(bF, "\r\n")
+        removeAttr: function(a) {
+            return this.each(function() {
+                n.removeAttr(this, a)
+            })
+        }
+    }), n.extend({
+        attr: function(a, b, c) {
+            var d, e, f = a.nodeType;
+            if (3 !== f && 8 !== f && 2 !== f) return "undefined" == typeof a.getAttribute ? n.prop(a, b, c) : (1 === f && n.isXMLDoc(a) || (b = b.toLowerCase(), e = n.attrHooks[b] || (n.expr.match.bool.test(b) ? ab : void 0)), void 0 !== c ? null === c ? void n.removeAttr(a, b) : e && "set" in e && void 0 !== (d = e.set(a, c, b)) ? d : (a.setAttribute(b, c + ""), c) : e && "get" in e && null !== (d = e.get(a, b)) ? d : (d = n.find.attr(a, b), null == d ? void 0 : d))
+        },
+        attrHooks: {
+            type: {
+                set: function(a, b) {
+                    if (!l.radioValue && "radio" === b && n.nodeName(a, "input")) {
+                        var c = a.value;
+                        return a.setAttribute("type", b), c && (a.value = c), b
                     }
-                }) : {
-                    name: b.name,
-                    value: c.replace(bF, "\r\n")
                 }
-            }).get()
+            }
+        },
+        removeAttr: function(a, b) {
+            var c, d, e = 0,
+                f = b && b.match(G);
+            if (f && 1 === a.nodeType)
+                while (c = f[e++]) d = n.propFix[c] || c, n.expr.match.bool.test(c) && (a[d] = !1), a.removeAttribute(c)
         }
-    }), f.each("ajaxStart ajaxStop ajaxComplete ajaxError ajaxSuccess ajaxSend".split(" "), function(a, b) {
-        f.fn[b] = function(a) {
-            return this.on(b, a)
+    }), ab = {
+        set: function(a, b, c) {
+            return b === !1 ? n.removeAttr(a, c) : a.setAttribute(c, c), c
         }
-    }), f.each(["get", "post"], function(a, c) {
-        f[c] = function(a, d, e, g) {
-            f.isFunction(d) && (g = g || e, e = d, d = b);
-            return f.ajax({
-                type: c,
-                url: a,
-                data: d,
-                success: e,
-                dataType: g
+    }, n.each(n.expr.match.bool.source.match(/\w+/g), function(a, b) {
+        var c = bb[b] || n.find.attr;
+        bb[b] = function(a, b, d) {
+            var e, f;
+            return d || (f = bb[b], bb[b] = e, e = null != c(a, b, d) ? b.toLowerCase() : null, bb[b] = f), e
+        }
+    });
+    var cb = /^(?:input|select|textarea|button)$/i,
+        db = /^(?:a|area)$/i;
+    n.fn.extend({
+        prop: function(a, b) {
+            return K(this, n.prop, a, b, arguments.length > 1)
+        },
+        removeProp: function(a) {
+            return this.each(function() {
+                delete this[n.propFix[a] || a]
             })
         }
-    }), f.extend({
-        getScript: function(a, c) {
-            return f.get(a, b, c, "script")
+    }), n.extend({
+        prop: function(a, b, c) {
+            var d, e, f = a.nodeType;
+            if (3 !== f && 8 !== f && 2 !== f) return 1 === f && n.isXMLDoc(a) || (b = n.propFix[b] || b, e = n.propHooks[b]),
+                void 0 !== c ? e && "set" in e && void 0 !== (d = e.set(a, c, b)) ? d : a[b] = c : e && "get" in e && null !== (d = e.get(a, b)) ? d : a[b]
         },
-        getJSON: function(a, b, c) {
-            return f.get(a, b, c, "json")
+        propHooks: {
+            tabIndex: {
+                get: function(a) {
+                    var b = n.find.attr(a, "tabindex");
+                    return b ? parseInt(b, 10) : cb.test(a.nodeName) || db.test(a.nodeName) && a.href ? 0 : -1
+                }
+            }
         },
-        ajaxSetup: function(a, b) {
-            b ? b_(a, f.ajaxSettings) : (b = a, a = f.ajaxSettings), b_(a, b);
-            return a
+        propFix: {
+            "for": "htmlFor",
+            "class": "className"
+        }
+    }), l.optSelected || (n.propHooks.selected = {
+        get: function(a) {
+            var b = a.parentNode;
+            return b && b.parentNode && b.parentNode.selectedIndex, null
+        },
+        set: function(a) {
+            var b = a.parentNode;
+            b && (b.selectedIndex, b.parentNode && b.parentNode.selectedIndex)
+        }
+    }), n.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
+        n.propFix[this.toLowerCase()] = this
+    });
+    var eb = /[\t\r\n\f]/g;
+
+    function fb(a) {
+        return a.getAttribute && a.getAttribute("class") || ""
+    }
+    n.fn.extend({
+        addClass: function(a) {
+            var b, c, d, e, f, g, h, i = 0;
+            if (n.isFunction(a)) return this.each(function(b) {
+                n(this).addClass(a.call(this, b, fb(this)))
+            });
+            if ("string" == typeof a && a) {
+                b = a.match(G) || [];
+                while (c = this[i++])
+                    if (e = fb(c), d = 1 === c.nodeType && (" " + e + " ").replace(eb, " ")) {
+                        g = 0;
+                        while (f = b[g++]) d.indexOf(" " + f + " ") < 0 && (d += f + " ");
+                        h = n.trim(d), e !== h && c.setAttribute("class", h)
+                    }
+            }
+            return this
+        },
+        removeClass: function(a) {
+            var b, c, d, e, f, g, h, i = 0;
+            if (n.isFunction(a)) return this.each(function(b) {
+                n(this).removeClass(a.call(this, b, fb(this)))
+            });
+            if (!arguments.length) return this.attr("class", "");
+            if ("string" == typeof a && a) {
+                b = a.match(G) || [];
+                while (c = this[i++])
+                    if (e = fb(c), d = 1 === c.nodeType && (" " + e + " ").replace(eb, " ")) {
+                        g = 0;
+                        while (f = b[g++])
+                            while (d.indexOf(" " + f + " ") > -1) d = d.replace(" " + f + " ", " ");
+                        h = n.trim(d), e !== h && c.setAttribute("class", h)
+                    }
+            }
+            return this
+        },
+        toggleClass: function(a, b) {
+            var c = typeof a;
+            return "boolean" == typeof b && "string" === c ? b ? this.addClass(a) : this.removeClass(a) : n.isFunction(a) ? this.each(function(c) {
+                n(this).toggleClass(a.call(this, c, fb(this), b), b)
+            }) : this.each(function() {
+                var b, d, e, f;
+                if ("string" === c) {
+                    d = 0, e = n(this), f = a.match(G) || [];
+                    while (b = f[d++]) e.hasClass(b) ? e.removeClass(b) : e.addClass(b)
+                } else void 0 !== a && "boolean" !== c || (b = fb(this), b && N.set(this, "__className__", b), this.setAttribute && this.setAttribute("class", b || a === !1 ? "" : N.get(this, "__className__") || ""))
+            })
+        },
+        hasClass: function(a) {
+            var b, c, d = 0;
+            b = " " + a + " ";
+            while (c = this[d++])
+                if (1 === c.nodeType && (" " + fb(c) + " ").replace(eb, " ").indexOf(b) > -1) return !0;
+            return !1
+        }
+    });
+    var gb = /\r/g,
+        hb = /[\x20\t\r\n\f]+/g;
+    n.fn.extend({
+        val: function(a) {
+            var b, c, d, e = this[0]; {
+                if (arguments.length) return d = n.isFunction(a), this.each(function(c) {
+                    var e;
+                    1 === this.nodeType && (e = d ? a.call(this, c, n(this).val()) : a, null == e ? e = "" : "number" == typeof e ? e += "" : n.isArray(e) && (e = n.map(e, function(a) {
+                        return null == a ? "" : a + ""
+                    })), b = n.valHooks[this.type] || n.valHooks[this.nodeName.toLowerCase()], b && "set" in b && void 0 !== b.set(this, e, "value") || (this.value = e))
+                });
+                if (e) return b = n.valHooks[e.type] || n.valHooks[e.nodeName.toLowerCase()], b && "get" in b && void 0 !== (c = b.get(e, "value")) ? c : (c = e.value, "string" == typeof c ? c.replace(gb, "") : null == c ? "" : c)
+            }
+        }
+    }), n.extend({
+        valHooks: {
+            option: {
+                get: function(a) {
+                    var b = n.find.attr(a, "value");
+                    return null != b ? b : n.trim(n.text(a)).replace(hb, " ")
+                }
+            },
+            select: {
+                get: function(a) {
+                    for (var b, c, d = a.options, e = a.selectedIndex, f = "select-one" === a.type || 0 > e, g = f ? null : [], h = f ? e + 1 : d.length, i = 0 > e ? h : f ? e : 0; h > i; i++)
+                        if (c = d[i], (c.selected || i === e) && (l.optDisabled ? !c.disabled : null === c.getAttribute("disabled")) && (!c.parentNode.disabled || !n.nodeName(c.parentNode, "optgroup"))) {
+                            if (b = n(c).val(), f) return b;
+                            g.push(b)
+                        } return g
+                },
+                set: function(a, b) {
+                    var c, d, e = a.options,
+                        f = n.makeArray(b),
+                        g = e.length;
+                    while (g--) d = e[g], (d.selected = n.inArray(n.valHooks.option.get(d), f) > -1) && (c = !0);
+                    return c || (a.selectedIndex = -1), f
+                }
+            }
+        }
+    }), n.each(["radio", "checkbox"], function() {
+        n.valHooks[this] = {
+            set: function(a, b) {
+                return n.isArray(b) ? a.checked = n.inArray(n(a).val(), b) > -1 : void 0
+            }
+        }, l.checkOn || (n.valHooks[this].get = function(a) {
+            return null === a.getAttribute("value") ? "on" : a.value
+        })
+    });
+    var ib = /^(?:focusinfocus|focusoutblur)$/;
+    n.extend(n.event, {
+        trigger: function(b, c, e, f) {
+            var g, h, i, j, l, m, o, p = [e || d],
+                q = k.call(b, "type") ? b.type : b,
+                r = k.call(b, "namespace") ? b.namespace.split(".") : [];
+            if (h = i = e = e || d, 3 !== e.nodeType && 8 !== e.nodeType && !ib.test(q + n.event.triggered) && (q.indexOf(".") > -1 && (r = q.split("."), q = r.shift(), r.sort()), l = q.indexOf(":") < 0 && "on" + q, b = b[n.expando] ? b : new n.Event(q, "object" == typeof b && b), b.isTrigger = f ? 2 : 3, b.namespace = r.join("."), b.rnamespace = b.namespace ? new RegExp("(^|\\.)" + r.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, b.result = void 0, b.target || (b.target = e), c = null == c ? [b] : n.makeArray(c, [b]), o = n.event.special[q] || {}, f || !o.trigger || o.trigger.apply(e, c) !== !1)) {
+                if (!f && !o.noBubble && !n.isWindow(e)) {
+                    for (j = o.delegateType || q, ib.test(j + q) || (h = h.parentNode); h; h = h.parentNode) p.push(h), i = h;
+                    i === (e.ownerDocument || d) && p.push(i.defaultView || i.parentWindow || a)
+                }
+                g = 0;
+                while ((h = p[g++]) && !b.isPropagationStopped()) b.type = g > 1 ? j : o.bindType || q, m = (N.get(h, "events") || {})[b.type] && N.get(h, "handle"), m && m.apply(h, c), m = l && h[l], m && m.apply && L(h) && (b.result = m.apply(h, c), b.result === !1 && b.preventDefault());
+                return b.type = q, f || b.isDefaultPrevented() || o._default && o._default.apply(p.pop(), c) !== !1 || !L(e) || l && n.isFunction(e[q]) && !n.isWindow(e) && (i = e[l], i && (e[l] = null), n.event.triggered = q, e[q](), n.event.triggered = void 0, i && (e[l] = i)), b.result
+            }
+        },
+        simulate: function(a, b, c) {
+            var d = n.extend(new n.Event, c, {
+                type: a,
+                isSimulated: !0
+            });
+            n.event.trigger(d, null, b)
+        }
+    }), n.fn.extend({
+        trigger: function(a, b) {
+            return this.each(function() {
+                n.event.trigger(a, b, this)
+            })
         },
+        triggerHandler: function(a, b) {
+            var c = this[0];
+            return c ? n.event.trigger(a, b, c, !0) : void 0
+        }
+    }), n.each("blur focus focusin focusout load resize scroll unload click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup error contextmenu".split(" "), function(a, b) {
+        n.fn[b] = function(a, c) {
+            return arguments.length > 0 ? this.on(b, null, a, c) : this.trigger(b)
+        }
+    }), n.fn.extend({
+        hover: function(a, b) {
+            return this.mouseenter(a).mouseleave(b || a)
+        }
+    }), l.focusin = "onfocusin" in a, l.focusin || n.each({
+        focus: "focusin",
+        blur: "focusout"
+    }, function(a, b) {
+        var c = function(a) {
+            n.event.simulate(b, a.target, n.event.fix(a))
+        };
+        n.event.special[b] = {
+            setup: function() {
+                var d = this.ownerDocument || this,
+                    e = N.access(d, b);
+                e || d.addEventListener(a, c, !0), N.access(d, b, (e || 0) + 1)
+            },
+            teardown: function() {
+                var d = this.ownerDocument || this,
+                    e = N.access(d, b) - 1;
+                e ? N.access(d, b, e) : (d.removeEventListener(a, c, !0), N.remove(d, b))
+            }
+        }
+    });
+    var jb = a.location,
+        kb = n.now(),
+        lb = /\?/;
+    n.parseJSON = function(a) {
+        return JSON.parse(a + "")
+    }, n.parseXML = function(b) {
+        var c;
+        if (!b || "string" != typeof b) return null;
+        try {
+            c = (new a.DOMParser).parseFromString(b, "text/xml")
+        } catch (d) {
+            c = void 0
+        }
+        return c && !c.getElementsByTagName("parsererror").length || n.error("Invalid XML: " + b), c
+    };
+    var mb = /#.*$/,
+        nb = /([?&])_=[^&]*/,
+        ob = /^(.*?):[ \t]*([^\r\n]*)$/gm,
+        pb = /^(?:about|app|app-storage|.+-extension|file|res|widget):$/,
+        qb = /^(?:GET|HEAD)$/,
+        rb = /^\/\//,
+        sb = {},
+        tb = {},
+        ub = "*/".concat("*"),
+        vb = d.createElement("a");
+    vb.href = jb.href;
+
+    function wb(a) {
+        return function(b, c) {
+            "string" != typeof b && (c = b, b = "*");
+            var d, e = 0,
+                f = b.toLowerCase().match(G) || [];
+            if (n.isFunction(c))
+                while (d = f[e++]) "+" === d[0] ? (d = d.slice(1) || "*", (a[d] = a[d] || []).unshift(c)) : (a[d] = a[d] || []).push(c)
+        }
+    }
+
+    function xb(a, b, c, d) {
+        var e = {},
+            f = a === tb;
+
+        function g(h) {
+            var i;
+            return e[h] = !0, n.each(a[h] || [], function(a, h) {
+                var j = h(b, c, d);
+                return "string" != typeof j || f || e[j] ? f ? !(i = j) : void 0 : (b.dataTypes.unshift(j), g(j), !1)
+            }), i
+        }
+        return g(b.dataTypes[0]) || !e["*"] && g("*")
+    }
+
+    function yb(a, b) {
+        var c, d, e = n.ajaxSettings.flatOptions || {};
+        for (c in b) void 0 !== b[c] && ((e[c] ? a : d || (d = {}))[c] = b[c]);
+        return d && n.extend(!0, a, d), a
+    }
+
+    function zb(a, b, c) {
+        var d, e, f, g, h = a.contents,
+            i = a.dataTypes;
+        while ("*" === i[0]) i.shift(), void 0 === d && (d = a.mimeType || b.getResponseHeader("Content-Type"));
+        if (d)
+            for (e in h)
+                if (h[e] && h[e].test(d)) {
+                    i.unshift(e);
+                    break
+                } if (i[0] in c) f = i[0];
+        else {
+            for (e in c) {
+                if (!i[0] || a.converters[e + " " + i[0]]) {
+                    f = e;
+                    break
+                }
+                g || (g = e)
+            }
+            f = f || g
+        }
+        return f ? (f !== i[0] && i.unshift(f), c[f]) : void 0
+    }
+
+    function Ab(a, b, c, d) {
+        var e, f, g, h, i, j = {},
+            k = a.dataTypes.slice();
+        if (k[1])
+            for (g in a.converters) j[g.toLowerCase()] = a.converters[g];
+        f = k.shift();
+        while (f)
+            if (a.responseFields[f] && (c[a.responseFields[f]] = b), !i && d && a.dataFilter && (b = a.dataFilter(b, a.dataType)), i = f, f = k.shift())
+                if ("*" === f) f = i;
+                else if ("*" !== i && i !== f) {
+            if (g = j[i + " " + f] || j["* " + f], !g)
+                for (e in j)
+                    if (h = e.split(" "), h[1] === f && (g = j[i + " " + h[0]] || j["* " + h[0]])) {
+                        g === !0 ? g = j[e] : j[e] !== !0 && (f = h[0], k.unshift(h[1]));
+                        break
+                    } if (g !== !0)
+                if (g && a["throws"]) b = g(b);
+                else try {
+                    b = g(b)
+                } catch (l) {
+                    return {
+                        state: "parsererror",
+                        error: g ? l : "No conversion from " + i + " to " + f
+                    }
+                }
+        }
+        return {
+            state: "success",
+            data: b
+        }
+    }
+    n.extend({
+        active: 0,
+        lastModified: {},
+        etag: {},
         ajaxSettings: {
-            url: bV,
-            isLocal: bJ.test(bW[1]),
-            global: !0,
+            url: jb.href,
             type: "GET",
-            contentType: "application/x-www-form-urlencoded",
+            isLocal: pb.test(jb.protocol),
+            global: !0,
             processData: !0,
             async: !0,
+            contentType: "application/x-www-form-urlencoded; charset=UTF-8",
             accepts: {
-                xml: "application/xml, text/xml",
-                html: "text/html",
+                "*": ub,
                 text: "text/plain",
-                json: "application/json, text/javascript",
-                "*": bX
+                html: "text/html",
+                xml: "application/xml, text/xml",
+                json: "application/json, text/javascript"
             },
             contents: {
-                xml: /xml/,
-                html: /html/,
-                json: /json/
+                xml: /\bxml\b/,
+                html: /\bhtml/,
+                json: /\bjson\b/
             },
             responseFields: {
                 xml: "responseXML",
-                text: "responseText"
+                text: "responseText",
+                json: "responseJSON"
             },
             converters: {
-                "* text": a.String,
+                "* text": String,
                 "text html": !0,
-                "text json": f.parseJSON,
-                "text xml": f.parseXML
+                "text json": n.parseJSON,
+                "text xml": n.parseXML
             },
             flatOptions: {
-                context: !0,
-                url: !0
+                url: !0,
+                context: !0
             }
         },
-        ajaxPrefilter: bZ(bT),
-        ajaxTransport: bZ(bU),
-        ajax: function(a, c) {
-            function w(a, c, l, m) {
-                if (s !== 2) {
-                    s = 2, q && clearTimeout(q), p = b, n = m || "", v.readyState = a > 0 ? 4 : 0;
-                    var o, r, u, w = c,
-                        x = l ? cb(d, v, l) : b,
-                        y, z;
-                    if (a >= 200 && a < 300 || a === 304) {
-                        if (d.ifModified) {
-                            if (y = v.getResponseHeader("Last-Modified")) f.lastModified[k] = y;
-                            if (z = v.getResponseHeader("Etag")) f.etag[k] = z
-                        }
-                        if (a === 304) w = "notmodified", o = !0;
-                        else try {
-                            r = cc(d, x), w = "success", o = !0
-                        } catch (A) {
-                            w = "parsererror", u = A
-                        }
-                    } else {
-                        u = w;
-                        if (!w || a) w = "error", a < 0 && (a = 0)
-                    }
-                    v.status = a, v.statusText = "" + (c || w), o ? h.resolveWith(e, [r, w, v]) : h.rejectWith(e, [v, w, u]), v.statusCode(j), j = b, t && g.trigger("ajax" + (o ? "Success" : "Error"), [v, d, o ? r : u]), i.fireWith(e, [v, w]), t && (g.trigger("ajaxComplete", [v, d]), --f.active || f.event.trigger("ajaxStop"))
-                }
-            }
-            typeof a == "object" && (c = a, a = b), c = c || {};
-            var d = f.ajaxSetup({}, c),
-                e = d.context || d,
-                g = e !== d && (e.nodeType || e instanceof f) ? f(e) : f.event,
-                h = f.Deferred(),
-                i = f.Callbacks("once memory"),
-                j = d.statusCode || {},
-                k, l = {},
-                m = {},
-                n, o, p, q, r, s = 0,
-                t, u, v = {
+        ajaxSetup: function(a, b) {
+            return b ? yb(yb(a, n.ajaxSettings), b) : yb(n.ajaxSettings, a)
+        },
+        ajaxPrefilter: wb(sb),
+        ajaxTransport: wb(tb),
+        ajax: function(b, c) {
+            "object" == typeof b && (c = b, b = void 0), c = c || {};
+            var e, f, g, h, i, j, k, l, m = n.ajaxSetup({}, c),
+                o = m.context || m,
+                p = m.context && (o.nodeType || o.jquery) ? n(o) : n.event,
+                q = n.Deferred(),
+                r = n.Callbacks("once memory"),
+                s = m.statusCode || {},
+                t = {},
+                u = {},
+                v = 0,
+                w = "canceled",
+                x = {
                     readyState: 0,
-                    setRequestHeader: function(a, b) {
-                        if (!s) {
-                            var c = a.toLowerCase();
-                            a = m[c] = m[c] || a, l[a] = b
+                    getResponseHeader: function(a) {
+                        var b;
+                        if (2 === v) {
+                            if (!h) {
+                                h = {};
+                                while (b = ob.exec(g)) h[b[1].toLowerCase()] = b[2]
+                            }
+                            b = h[a.toLowerCase()]
                         }
-                        return this
+                        return null == b ? null : b
                     },
                     getAllResponseHeaders: function() {
-                        return s === 2 ? n : null
+                        return 2 === v ? g : null
                     },
-                    getResponseHeader: function(a) {
-                        var c;
-                        if (s === 2) {
-                            if (!o) {
-                                o = {};
-                                while (c = bH.exec(n)) o[c[1].toLowerCase()] = c[2]
-                            }
-                            c = o[a.toLowerCase()]
-                        }
-                        return c === b ? null : c
+                    setRequestHeader: function(a, b) {
+                        var c = a.toLowerCase();
+                        return v || (a = u[c] = u[c] || a, t[a] = b), this
                     },
                     overrideMimeType: function(a) {
-                        s || (d.mimeType = a);
+                        return v || (m.mimeType = a), this
+                    },
+                    statusCode: function(a) {
+                        var b;
+                        if (a)
+                            if (2 > v)
+                                for (b in a) s[b] = [s[b], a[b]];
+                            else x.always(a[x.status]);
                         return this
                     },
                     abort: function(a) {
-                        a = a || "abort", p && p.abort(a), w(0, a);
-                        return this
+                        var b = a || w;
+                        return e && e.abort(b), z(0, b), this
                     }
                 };
-            h.promise(v), v.success = v.done, v.error = v.fail, v.complete = i.add, v.statusCode = function(a) {
-                if (a) {
-                    var b;
-                    if (s < 2)
-                        for (b in a) j[b] = [j[b], a[b]];
-                    else b = a[v.status], v.then(b, b)
+            if (q.promise(x).complete = r.add, x.success = x.done, x.error = x.fail, m.url = ((b || m.url || jb.href) + "").replace(mb, "").replace(rb, jb.protocol + "//"), m.type = c.method || c.type || m.method || m.type, m.dataTypes = n.trim(m.dataType || "*").toLowerCase().match(G) || [""], null == m.crossDomain) {
+                j = d.createElement("a");
+                try {
+                    j.href = m.url, j.href = j.href, m.crossDomain = vb.protocol + "//" + vb.host != j.protocol + "//" + j.host
+                } catch (y) {
+                    m.crossDomain = !0
                 }
-                return this
-            }, d.url = ((a || d.url) + "").replace(bG, "").replace(bL, bW[1] + "//"), d.dataTypes = f.trim(d.dataType || "*").toLowerCase().split(bP), d.crossDomain == null && (r = bR.exec(d.url.toLowerCase()), d.crossDomain = !(!r || r[1] == bW[1] && r[2] == bW[2] && (r[3] || (r[1] === "http:" ? 80 : 443)) == (bW[3] || (bW[1] === "http:" ? 80 : 443)))), d.data && d.processData && typeof d.data != "string" && (d.data = f.param(d.data, d.traditional)), b$(bT, d, c, v);
-            if (s === 2) return !1;
-            t = d.global, d.type = d.type.toUpperCase(), d.hasContent = !bK.test(d.type), t && f.active++ === 0 && f.event.trigger("ajaxStart");
-            if (!d.hasContent) {
-                d.data && (d.url += (bM.test(d.url) ? "&" : "?") + d.data, delete d.data), k = d.url;
-                if (d.cache === !1) {
-                    var x = f.now(),
-                        y = d.url.replace(bQ, "$1_=" + x);
-                    d.url = y + (y === d.url ? (bM.test(d.url) ? "&" : "?") + "_=" + x : "")
-                }
-            }(d.data && d.hasContent && d.contentType !== !1 || c.contentType) && v.setRequestHeader("Content-Type", d.contentType), d.ifModified && (k = k || d.url, f.lastModified[k] && v.setRequestHeader("If-Modified-Since", f.lastModified[k]), f.etag[k] && v.setRequestHeader("If-None-Match", f.etag[k])), v.setRequestHeader("Accept", d.dataTypes[0] && d.accepts[d.dataTypes[0]] ? d.accepts[d.dataTypes[0]] + (d.dataTypes[0] !== "*" ? ", " + bX + "; q=0.01" : "") : d.accepts["*"]);
-            for (u in d.headers) v.setRequestHeader(u, d.headers[u]);
-            if (d.beforeSend && (d.beforeSend.call(e, v, d) === !1 || s === 2)) {
-                v.abort();
-                return !1
             }
-            for (u in {
+            if (m.data && m.processData && "string" != typeof m.data && (m.data = n.param(m.data, m.traditional)), xb(sb, m, c, x), 2 === v) return x;
+            k = n.event && m.global, k && 0 === n.active++ && n.event.trigger("ajaxStart"), m.type = m.type.toUpperCase(), m.hasContent = !qb.test(m.type), f = m.url, m.hasContent || (m.data && (f = m.url += (lb.test(f) ? "&" : "?") + m.data, delete m.data), m.cache === !1 && (m.url = nb.test(f) ? f.replace(nb, "$1_=" + kb++) : f + (lb.test(f) ? "&" : "?") + "_=" + kb++)), m.ifModified && (n.lastModified[f] && x.setRequestHeader("If-Modified-Since", n.lastModified[f]), n.etag[f] && x.setRequestHeader("If-None-Match", n.etag[f])), (m.data && m.hasContent && m.contentType !== !1 || c.contentType) && x.setRequestHeader("Content-Type", m.contentType), x.setRequestHeader("Accept", m.dataTypes[0] && m.accepts[m.dataTypes[0]] ? m.accepts[m.dataTypes[0]] + ("*" !== m.dataTypes[0] ? ", " + ub + "; q=0.01" : "") : m.accepts["*"]);
+            for (l in m.headers) x.setRequestHeader(l, m.headers[l]);
+            if (m.beforeSend && (m.beforeSend.call(o, x, m) === !1 || 2 === v)) return x.abort();
+            w = "abort";
+            for (l in {
                     success: 1,
                     error: 1,
                     complete: 1
-                }) v[u](d[u]);
-            p = b$(bU, d, c, v);
-            if (!p) w(-1, "No Transport");
-            else {
-                v.readyState = 1, t && g.trigger("ajaxSend", [v, d]), d.async && d.timeout > 0 && (q = setTimeout(function() {
-                    v.abort("timeout")
-                }, d.timeout));
+                }) x[l](m[l]);
+            if (e = xb(tb, m, c, x)) {
+                if (x.readyState = 1, k && p.trigger("ajaxSend", [x, m]), 2 === v) return x;
+                m.async && m.timeout > 0 && (i = a.setTimeout(function() {
+                    x.abort("timeout")
+                }, m.timeout));
                 try {
-                    s = 1, p.send(l, w)
-                } catch (z) {
-                    if (s < 2) w(-1, z);
-                    else throw z
-                }
+                    v = 1, e.send(t, z)
+                } catch (y) {
+                    if (!(2 > v)) throw y;
+                    z(-1, y)
+                }
+            } else z(-1, "No Transport");
+
+            function z(b, c, d, h) {
+                var j, l, t, u, w, y = c;
+                2 !== v && (v = 2, i && a.clearTimeout(i), e = void 0, g = h || "", x.readyState = b > 0 ? 4 : 0, j = b >= 200 && 300 > b || 304 === b, d && (u = zb(m, x, d)), u = Ab(m, u, x, j), j ? (m.ifModified && (w = x.getResponseHeader("Last-Modified"), w && (n.lastModified[f] = w), w = x.getResponseHeader("etag"), w && (n.etag[f] = w)), 204 === b || "HEAD" === m.type ? y = "nocontent" : 304 === b ? y = "notmodified" : (y = u.state, l = u.data, t = u.error, j = !t)) : (t = y, !b && y || (y = "error", 0 > b && (b = 0))), x.status = b, x.statusText = (c || y) + "", j ? q.resolveWith(o, [l, y, x]) : q.rejectWith(o, [x, y, t]), x.statusCode(s), s = void 0, k && p.trigger(j ? "ajaxSuccess" : "ajaxError", [x, m, j ? l : t]), r.fireWith(o, [x, y]), k && (p.trigger("ajaxComplete", [x, m]), --n.active || n.event.trigger("ajaxStop")))
             }
-            return v
+            return x
         },
-        param: function(a, c) {
-            var d = [],
-                e = function(a, b) {
-                    b = f.isFunction(b) ? b() : b, d[d.length] = encodeURIComponent(a) + "=" + encodeURIComponent(b)
-                };
-            c === b && (c = f.ajaxSettings.traditional);
-            if (f.isArray(a) || a.jquery && !f.isPlainObject(a)) f.each(a, function() {
-                e(this.name, this.value)
-            });
-            else
-                for (var g in a) ca(g, a[g], c, e);
-            return d.join("&").replace(bD, "+")
+        getJSON: function(a, b, c) {
+            return n.get(a, b, c, "json")
+        },
+        getScript: function(a, b) {
+            return n.get(a, void 0, b, "script")
         }
-    }), f.extend({
-        active: 0,
-        lastModified: {},
-        etag: {}
-    });
-    var cd = f.now(),
-        ce = /(\=)\?(&|$)|\?\?/i;
-    f.ajaxSetup({
-        jsonp: "callback",
-        jsonpCallback: function() {
-            return f.expando + "_" + cd++
+    }), n.each(["get", "post"], function(a, b) {
+        n[b] = function(a, c, d, e) {
+            return n.isFunction(c) && (e = e || d, d = c, c = void 0), n.ajax(n.extend({
+                url: a,
+                type: b,
+                dataType: e,
+                data: c,
+                success: d
+            }, n.isPlainObject(a) && a))
         }
-    }), f.ajaxPrefilter("json jsonp", function(b, c, d) {
-        var e = b.contentType === "application/x-www-form-urlencoded" && typeof b.data == "string";
-        if (b.dataTypes[0] === "jsonp" || b.jsonp !== !1 && (ce.test(b.url) || e && ce.test(b.data))) {
-            var g, h = b.jsonpCallback = f.isFunction(b.jsonpCallback) ? b.jsonpCallback() : b.jsonpCallback,
-                i = a[h],
-                j = b.url,
-                k = b.data,
-                l = "$1" + h + "$2";
-            b.jsonp !== !1 && (j = j.replace(ce, l), b.url === j && (e && (k = k.replace(ce, l)), b.data === k && (j += (/\?/.test(j) ? "&" : "?") + b.jsonp + "=" + h))), b.url = j, b.data = k, a[h] = function(a) {
-                g = [a]
-            }, d.always(function() {
-                a[h] = i, g && f.isFunction(i) && a[h](g[0])
-            }), b.converters["script json"] = function() {
-                g || f.error(h + " was not called");
-                return g[0]
-            }, b.dataTypes[0] = "json";
-            return "script"
+    }), n._evalUrl = function(a) {
+        return n.ajax({
+            url: a,
+            type: "GET",
+            dataType: "script",
+            async: !1,
+            global: !1,
+            "throws": !0
+        })
+    }, n.fn.extend({
+        wrapAll: function(a) {
+            var b;
+            return n.isFunction(a) ? this.each(function(b) {
+                n(this).wrapAll(a.call(this, b))
+            }) : (this[0] && (b = n(a, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && b.insertBefore(this[0]), b.map(function() {
+                var a = this;
+                while (a.firstElementChild) a = a.firstElementChild;
+                return a
+            }).append(this)), this)
+        },
+        wrapInner: function(a) {
+            return n.isFunction(a) ? this.each(function(b) {
+                n(this).wrapInner(a.call(this, b))
+            }) : this.each(function() {
+                var b = n(this),
+                    c = b.contents();
+                c.length ? c.wrapAll(a) : b.append(a)
+            })
+        },
+        wrap: function(a) {
+            var b = n.isFunction(a);
+            return this.each(function(c) {
+                n(this).wrapAll(b ? a.call(this, c) : a)
+            })
+        },
+        unwrap: function() {
+            return this.parent().each(function() {
+                n.nodeName(this, "body") || n(this).replaceWith(this.childNodes)
+            }).end()
         }
-    }), f.ajaxSetup({
+    }), n.expr.filters.hidden = function(a) {
+        return !n.expr.filters.visible(a)
+    }, n.expr.filters.visible = function(a) {
+        return a.offsetWidth > 0 || a.offsetHeight > 0 || a.getClientRects().length > 0
+    };
+    var Bb = /%20/g,
+        Cb = /\[\]$/,
+        Db = /\r?\n/g,
+        Eb = /^(?:submit|button|image|reset|file)$/i,
+        Fb = /^(?:input|select|textarea|keygen)/i;
+
+    function Gb(a, b, c, d) {
+        var e;
+        if (n.isArray(b)) n.each(b, function(b, e) {
+            c || Cb.test(a) ? d(a, e) : Gb(a + "[" + ("object" == typeof e && null != e ? b : "") + "]", e, c, d)
+        });
+        else if (c || "object" !== n.type(b)) d(a, b);
+        else
+            for (e in b) Gb(a + "[" + e + "]", b[e], c, d)
+    }
+    n.param = function(a, b) {
+        var c, d = [],
+            e = function(a, b) {
+                b = n.isFunction(b) ? b() : null == b ? "" : b, d[d.length] = encodeURIComponent(a) + "=" + encodeURIComponent(b)
+            };
+        if (void 0 === b && (b = n.ajaxSettings && n.ajaxSettings.traditional), n.isArray(a) || a.jquery && !n.isPlainObject(a)) n.each(a, function() {
+            e(this.name, this.value)
+        });
+        else
+            for (c in a) Gb(c, a[c], b, e);
+        return d.join("&").replace(Bb, "+")
+    }, n.fn.extend({
+        serialize: function() {
+            return n.param(this.serializeArray())
+        },
+        serializeArray: function() {
+            return this.map(function() {
+                var a = n.prop(this, "elements");
+                return a ? n.makeArray(a) : this
+            }).filter(function() {
+                var a = this.type;
+                return this.name && !n(this).is(":disabled") && Fb.test(this.nodeName) && !Eb.test(a) && (this.checked || !X.test(a))
+            }).map(function(a, b) {
+                var c = n(this).val();
+                return null == c ? null : n.isArray(c) ? n.map(c, function(a) {
+                    return {
+                        name: b.name,
+                        value: a.replace(Db, "\r\n")
+                    }
+                }) : {
+                    name: b.name,
+                    value: c.replace(Db, "\r\n")
+                }
+            }).get()
+        }
+    }), n.ajaxSettings.xhr = function() {
+        try {
+            return new a.XMLHttpRequest
+        } catch (b) {}
+    };
+    var Hb = {
+            0: 200,
+            1223: 204
+        },
+        Ib = n.ajaxSettings.xhr();
+    l.cors = !!Ib && "withCredentials" in Ib, l.ajax = Ib = !!Ib, n.ajaxTransport(function(b) {
+        var c, d;
+        return l.cors || Ib && !b.crossDomain ? {
+            send: function(e, f) {
+                var g, h = b.xhr();
+                if (h.open(b.type, b.url, b.async, b.username, b.password), b.xhrFields)
+                    for (g in b.xhrFields) h[g] = b.xhrFields[g];
+                b.mimeType && h.overrideMimeType && h.overrideMimeType(b.mimeType), b.crossDomain || e["X-Requested-With"] || (e["X-Requested-With"] = "XMLHttpRequest");
+                for (g in e) h.setRequestHeader(g, e[g]);
+                c = function(a) {
+                    return function() {
+                        c && (c = d = h.onload = h.onerror = h.onabort = h.onreadystatechange = null, "abort" === a ? h.abort() : "error" === a ? "number" != typeof h.status ? f(0, "error") : f(h.status, h.statusText) : f(Hb[h.status] || h.status, h.statusText, "text" !== (h.responseType || "text") || "string" != typeof h.responseText ? {
+                            binary: h.response
+                        } : {
+                            text: h.responseText
+                        }, h.getAllResponseHeaders()))
+                    }
+                }, h.onload = c(), d = h.onerror = c("error"), void 0 !== h.onabort ? h.onabort = d : h.onreadystatechange = function() {
+                    4 === h.readyState && a.setTimeout(function() {
+                        c && d()
+                    })
+                }, c = c("abort");
+                try {
+                    h.send(b.hasContent && b.data || null)
+                } catch (i) {
+                    if (c) throw i
+                }
+            },
+            abort: function() {
+                c && c()
+            }
+        } : void 0
+    }), n.ajaxSetup({
         accepts: {
             script: "text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"
         },
         contents: {
-            script: /javascript|ecmascript/
+            script: /\b(?:java|ecma)script\b/
         },
         converters: {
             "text script": function(a) {
-                f.globalEval(a);
-                return a
+                return n.globalEval(a), a
             }
         }
-    }), f.ajaxPrefilter("script", function(a) {
-        a.cache === b && (a.cache = !1), a.crossDomain && (a.type = "GET", a.global = !1)
-    }), f.ajaxTransport("script", function(a) {
+    }), n.ajaxPrefilter("script", function(a) {
+        void 0 === a.cache && (a.cache = !1), a.crossDomain && (a.type = "GET")
+    }), n.ajaxTransport("script", function(a) {
         if (a.crossDomain) {
-            var d, e = c.head || c.getElementsByTagName("head")[0] || c.documentElement;
+            var b, c;
             return {
-                send: function(f, g) {
-                    d = c.createElement("script"), d.async = "async", a.scriptCharset && (d.charset = a.scriptCharset), d.src = a.url, d.onload = d.onreadystatechange = function(a, c) {
-                        if (c || !d.readyState || /loaded|complete/.test(d.readyState)) d.onload = d.onreadystatechange = null, e && d.parentNode && e.removeChild(d), d = b, c || g(200, "success")
-                    }, e.insertBefore(d, e.firstChild)
+                send: function(e, f) {
+                    b = n("<script>").prop({
+                        charset: a.scriptCharset,
+                        src: a.url
+                    }).on("load error", c = function(a) {
+                        b.remove(), c = null, a && f("error" === a.type ? 404 : 200, a.type)
+                    }), d.head.appendChild(b[0])
                 },
                 abort: function() {
-                    d && d.onload(0, 1)
+                    c && c()
                 }
             }
         }
     });
-    var cf = a.ActiveXObject ? function() {
-            for (var a in ch) ch[a](0, 1)
-        } : !1,
-        cg = 0,
-        ch;
-    f.ajaxSettings.xhr = a.ActiveXObject ? function() {
-            return !this.isLocal && ci() || cj()
-        } : ci,
-        function(a) {
-            f.extend(f.support, {
-                ajax: !!a,
-                cors: !!a && "withCredentials" in a
-            })
-        }(f.ajaxSettings.xhr()), f.support.ajax && f.ajaxTransport(function(c) {
-            if (!c.crossDomain || f.support.cors) {
-                var d;
-                return {
-                    send: function(e, g) {
-                        var h = c.xhr(),
-                            i, j;
-                        c.username ? h.open(c.type, c.url, c.async, c.username, c.password) : h.open(c.type, c.url, c.async);
-                        if (c.xhrFields)
-                            for (j in c.xhrFields) h[j] = c.xhrFields[j];
-                        c.mimeType && h.overrideMimeType && h.overrideMimeType(c.mimeType), !c.crossDomain && !e["X-Requested-With"] && (e["X-Requested-With"] = "XMLHttpRequest");
-                        try {
-                            for (j in e) h.setRequestHeader(j, e[j])
-                        } catch (k) {}
-                        h.send(c.hasContent && c.data || null), d = function(a, e) {
-                            var j, k, l, m, n;
-                            try {
-                                if (d && (e || h.readyState === 4)) {
-                                    d = b, i && (h.onreadystatechange = f.noop, cf && delete ch[i]);
-                                    if (e) h.readyState !== 4 && h.abort();
-                                    else {
-                                        j = h.status, l = h.getAllResponseHeaders(), m = {}, n = h.responseXML, n && n.documentElement && (m.xml = n), m.text = h.responseText;
-                                        try {
-                                            k = h.statusText
-                                        } catch (o) {
-                                            k = ""
-                                        }!j && c.isLocal && !c.crossDomain ? j = m.text ? 200 : 404 : j === 1223 && (j = 204)
-                                    }
-                                }
-                            } catch (p) {
-                                e || g(-1, p)
-                            }
-                            m && g(j, k, m, l)
-                        }, !c.async || h.readyState === 4 ? d() : (i = ++cg, cf && (ch || (ch = {}, f(a).unload(cf)), ch[i] = d), h.onreadystatechange = d)
-                    },
-                    abort: function() {
-                        d && d(0, 1)
-                    }
-                }
-            }
-        });
-    var ck = {},
-        cl, cm, cn = /^(?:toggle|show|hide)$/,
-        co = /^([+\-]=)?([\d+.\-]+)([a-z%]*)$/i,
-        cp, cq = [
-            ["height", "marginTop", "marginBottom", "paddingTop", "paddingBottom"],
-            ["width", "marginLeft", "marginRight", "paddingLeft", "paddingRight"],
-            ["opacity"]
-        ],
-        cr;
-    f.fn.extend({
-        show: function(a, b, c) {
-            var d, e;
-            if (a || a === 0) return this.animate(cu("show", 3), a, b, c);
-            for (var g = 0, h = this.length; g < h; g++) d = this[g], d.style && (e = d.style.display, !f._data(d, "olddisplay") && e === "none" && (e = d.style.display = ""), e === "" && f.css(d, "display") === "none" && f._data(d, "olddisplay", cv(d.nodeName)));
-            for (g = 0; g < h; g++) {
-                d = this[g];
-                if (d.style) {
-                    e = d.style.display;
-                    if (e === "" || e === "none") d.style.display = f._data(d, "olddisplay") || ""
-                }
-            }
-            return this
-        },
-        hide: function(a, b, c) {
-            if (a || a === 0) return this.animate(cu("hide", 3), a, b, c);
-            var d, e, g = 0,
-                h = this.length;
-            for (; g < h; g++) d = this[g], d.style && (e = f.css(d, "display"), e !== "none" && !f._data(d, "olddisplay") && f._data(d, "olddisplay", e));
-            for (g = 0; g < h; g++) this[g].style && (this[g].style.display = "none");
-            return this
-        },
-        _toggle: f.fn.toggle,
-        toggle: function(a, b, c) {
-            var d = typeof a == "boolean";
-            f.isFunction(a) && f.isFunction(b) ? this._toggle.apply(this, arguments) : a == null || d ? this.each(function() {
-                var b = d ? a : f(this).is(":hidden");
-                f(this)[b ? "show" : "hide"]()
-            }) : this.animate(cu("toggle", 3), a, b, c);
-            return this
-        },
-        fadeTo: function(a, b, c, d) {
-            return this.filter(":hidden").css("opacity", 0).show().end().animate({
-                opacity: b
-            }, a, c, d)
-        },
-        animate: function(a, b, c, d) {
-            function g() {
-                e.queue === !1 && f._mark(this);
-                var b = f.extend({}, e),
-                    c = this.nodeType === 1,
-                    d = c && f(this).is(":hidden"),
-                    g, h, i, j, k, l, m, n, o;
-                b.animatedProperties = {};
-                for (i in a) {
-                    g = f.camelCase(i), i !== g && (a[g] = a[i], delete a[i]), h = a[g], f.isArray(h) ? (b.animatedProperties[g] = h[1], h = a[g] = h[0]) : b.animatedProperties[g] = b.specialEasing && b.specialEasing[g] || b.easing || "swing";
-                    if (h === "hide" && d || h === "show" && !d) return b.complete.call(this);
-                    c && (g === "height" || g === "width") && (b.overflow = [this.style.overflow, this.style.overflowX, this.style.overflowY], f.css(this, "display") === "inline" && f.css(this, "float") === "none" && (!f.support.inlineBlockNeedsLayout || cv(this.nodeName) === "inline" ? this.style.display = "inline-block" : this.style.zoom = 1))
-                }
-                b.overflow != null && (this.style.overflow = "hidden");
-                for (i in a) j = new f.fx(this, b, i), h = a[i], cn.test(h) ? (o = f._data(this, "toggle" + i) || (h === "toggle" ? d ? "show" : "hide" : 0), o ? (f._data(this, "toggle" + i, o === "show" ? "hide" : "show"), j[o]()) : j[h]()) : (k = co.exec(h), l = j.cur(), k ? (m = parseFloat(k[2]), n = k[3] || (f.cssNumber[i] ? "" : "px"), n !== "px" && (f.style(this, i, (m || 1) + n), l = (m || 1) / j.cur() * l, f.style(this, i, l + n)), k[1] && (m = (k[1] === "-=" ? -1 : 1) * m + l), j.custom(l, m, n)) : j.custom(l, h, ""));
-                return !0
-            }
-            var e = f.speed(b, c, d);
-            if (f.isEmptyObject(a)) return this.each(e.complete, [!1]);
-            a = f.extend({}, a);
-            return e.queue === !1 ? this.each(g) : this.queue(e.queue, g)
-        },
-        stop: function(a, c, d) {
-            typeof a != "string" && (d = c, c = a, a = b), c && a !== !1 && this.queue(a || "fx", []);
-            return this.each(function() {
-                function h(a, b, c) {
-                    var e = b[c];
-                    f.removeData(a, c, !0), e.stop(d)
-                }
-                var b, c = !1,
-                    e = f.timers,
-                    g = f._data(this);
-                d || f._unmark(!0, this);
-                if (a == null)
-                    for (b in g) g[b] && g[b].stop && b.indexOf(".run") === b.length - 4 && h(this, g, b);
-                else g[b = a + ".run"] && g[b].stop && h(this, g, b);
-                for (b = e.length; b--;) e[b].elem === this && (a == null || e[b].queue === a) && (d ? e[b](!0) : e[b].saveState(), c = !0, e.splice(b, 1));
-                (!d || !c) && f.dequeue(this, a)
-            })
-        }
-    }), f.each({
-        slideDown: cu("show", 1),
-        slideUp: cu("hide", 1),
-        slideToggle: cu("toggle", 1),
-        fadeIn: {
-            opacity: "show"
-        },
-        fadeOut: {
-            opacity: "hide"
-        },
-        fadeToggle: {
-            opacity: "toggle"
-        }
-    }, function(a, b) {
-        f.fn[a] = function(a, c, d) {
-            return this.animate(b, a, c, d)
-        }
-    }), f.extend({
-        speed: function(a, b, c) {
-            var d = a && typeof a == "object" ? f.extend({}, a) : {
-                complete: c || !c && b || f.isFunction(a) && a,
-                duration: a,
-                easing: c && b || b && !f.isFunction(b) && b
-            };
-            d.duration = f.fx.off ? 0 : typeof d.duration == "number" ? d.duration : d.duration in f.fx.speeds ? f.fx.speeds[d.duration] : f.fx.speeds._default;
-            if (d.queue == null || d.queue === !0) d.queue = "fx";
-            d.old = d.complete, d.complete = function(a) {
-                f.isFunction(d.old) && d.old.call(this), d.queue ? f.dequeue(this, d.queue) : a !== !1 && f._unmark(this)
-            };
-            return d
-        },
-        easing: {
-            linear: function(a, b, c, d) {
-                return c + d * a
-            },
-            swing: function(a, b, c, d) {
-                return (-Math.cos(a * Math.PI) / 2 + .5) * d + c
-            }
-        },
-        timers: [],
-        fx: function(a, b, c) {
-            this.options = b, this.elem = a, this.prop = c, b.orig = b.orig || {}
-        }
-    }), f.fx.prototype = {
-        update: function() {
-            this.options.step && this.options.step.call(this.elem, this.now, this), (f.fx.step[this.prop] || f.fx.step._default)(this)
-        },
-        cur: function() {
-            if (this.elem[this.prop] != null && (!this.elem.style || this.elem.style[this.prop] == null)) return this.elem[this.prop];
-            var a, b = f.css(this.elem, this.prop);
-            return isNaN(a = parseFloat(b)) ? !b || b === "auto" ? 0 : b : a
-        },
-        custom: function(a, c, d) {
-            function h(a) {
-                return e.step(a)
-            }
-            var e = this,
-                g = f.fx;
-            this.startTime = cr || cs(), this.end = c, this.now = this.start = a, this.pos = this.state = 0, this.unit = d || this.unit || (f.cssNumber[this.prop] ? "" : "px"), h.queue = this.options.queue, h.elem = this.elem, h.saveState = function() {
-                e.options.hide && f._data(e.elem, "fxshow" + e.prop) === b && f._data(e.elem, "fxshow" + e.prop, e.start)
-            }, h() && f.timers.push(h) && !cp && (cp = setInterval(g.tick, g.interval))
-        },
-        show: function() {
-            var a = f._data(this.elem, "fxshow" + this.prop);
-            this.options.orig[this.prop] = a || f.style(this.elem, this.prop), this.options.show = !0, a !== b ? this.custom(this.cur(), a) : this.custom(this.prop === "width" || this.prop === "height" ? 1 : 0, this.cur()), f(this.elem).show()
-        },
-        hide: function() {
-            this.options.orig[this.prop] = f._data(this.elem, "fxshow" + this.prop) || f.style(this.elem, this.prop), this.options.hide = !0, this.custom(this.cur(), 0)
-        },
-        step: function(a) {
-            var b, c, d, e = cr || cs(),
-                g = !0,
-                h = this.elem,
-                i = this.options;
-            if (a || e >= i.duration + this.startTime) {
-                this.now = this.end, this.pos = this.state = 1, this.update(), i.animatedProperties[this.prop] = !0;
-                for (b in i.animatedProperties) i.animatedProperties[b] !== !0 && (g = !1);
-                if (g) {
-                    i.overflow != null && !f.support.shrinkWrapBlocks && f.each(["", "X", "Y"], function(a, b) {
-                        h.style["overflow" + b] = i.overflow[a]
-                    }), i.hide && f(h).hide();
-                    if (i.hide || i.show)
-                        for (b in i.animatedProperties) f.style(h, b, i.orig[b]), f.removeData(h, "fxshow" + b, !0), f.removeData(h, "toggle" + b, !0);
-                    d = i.complete, d && (i.complete = !1, d.call(h))
-                }
-                return !1
-            }
-            i.duration == Infinity ? this.now = e : (c = e - this.startTime, this.state = c / i.duration, this.pos = f.easing[i.animatedProperties[this.prop]](this.state, c, 0, 1, i.duration), this.now = this.start + (this.end - this.start) * this.pos), this.update();
-            return !0
-        }
-    }, f.extend(f.fx, {
-        tick: function() {
-            var a, b = f.timers,
-                c = 0;
-            for (; c < b.length; c++) a = b[c], !a() && b[c] === a && b.splice(c--, 1);
-            b.length || f.fx.stop()
-        },
-        interval: 13,
-        stop: function() {
-            clearInterval(cp), cp = null
-        },
-        speeds: {
-            slow: 600,
-            fast: 200,
-            _default: 400
-        },
-        step: {
-            opacity: function(a) {
-                f.style(a.elem, "opacity", a.now)
-            },
-            _default: function(a) {
-                a.elem.style && a.elem.style[a.prop] != null ? a.elem.style[a.prop] = a.now + a.unit : a.elem[a.prop] = a.now
-            }
+    var Jb = [],
+        Kb = /(=)\?(?=&|$)|\?\?/;
+    n.ajaxSetup({
+        jsonp: "callback",
+        jsonpCallback: function() {
+            var a = Jb.pop() || n.expando + "_" + kb++;
+            return this[a] = !0, a
         }
-    }), f.each(["width", "height"], function(a, b) {
-        f.fx.step[b] = function(a) {
-            f.style(a.elem, b, Math.max(0, a.now) + a.unit)
+    }), n.ajaxPrefilter("json jsonp", function(b, c, d) {
+        var e, f, g, h = b.jsonp !== !1 && (Kb.test(b.url) ? "url" : "string" == typeof b.data && 0 === (b.contentType || "").indexOf("application/x-www-form-urlencoded") && Kb.test(b.data) && "data");
+        return h || "jsonp" === b.dataTypes[0] ? (e = b.jsonpCallback = n.isFunction(b.jsonpCallback) ? b.jsonpCallback() : b.jsonpCallback, h ? b[h] = b[h].replace(Kb, "$1" + e) : b.jsonp !== !1 && (b.url += (lb.test(b.url) ? "&" : "?") + b.jsonp + "=" + e), b.converters["script json"] = function() {
+            return g || n.error(e + " was not called"), g[0]
+        }, b.dataTypes[0] = "json", f = a[e], a[e] = function() {
+            g = arguments
+        }, d.always(function() {
+            void 0 === f ? n(a).removeProp(e) : a[e] = f, b[e] && (b.jsonpCallback = c.jsonpCallback, Jb.push(e)), g && n.isFunction(f) && f(g[0]), g = f = void 0
+        }), "script") : void 0
+    }), n.parseHTML = function(a, b, c) {
+        if (!a || "string" != typeof a) return null;
+        "boolean" == typeof b && (c = b, b = !1), b = b || d;
+        var e = x.exec(a),
+            f = !c && [];
+        return e ? [b.createElement(e[1])] : (e = ca([a], b, f), f && f.length && n(f).remove(), n.merge([], e.childNodes))
+    };
+    var Lb = n.fn.load;
+    n.fn.load = function(a, b, c) {
+        if ("string" != typeof a && Lb) return Lb.apply(this, arguments);
+        var d, e, f, g = this,
+            h = a.indexOf(" ");
+        return h > -1 && (d = n.trim(a.slice(h)), a = a.slice(0, h)), n.isFunction(b) ? (c = b, b = void 0) : b && "object" == typeof b && (e = "POST"), g.length > 0 && n.ajax({
+            url: a,
+            type: e || "GET",
+            dataType: "html",
+            data: b
+        }).done(function(a) {
+            f = arguments, g.html(d ? n("<div>").append(n.parseHTML(a)).find(d) : a)
+        }).always(c && function(a, b) {
+            g.each(function() {
+                c.apply(this, f || [a.responseText, b, a])
+            })
+        }), this
+    }, n.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(a, b) {
+        n.fn[b] = function(a) {
+            return this.on(b, a)
         }
-    }), f.expr && f.expr.filters && (f.expr.filters.animated = function(a) {
-        return f.grep(f.timers, function(b) {
+    }), n.expr.filters.animated = function(a) {
+        return n.grep(n.timers, function(b) {
             return a === b.elem
         }).length
-    });
-    var cw = /^t(?:able|d|h)$/i,
-        cx = /^(?:body|html)$/i;
-    "getBoundingClientRect" in c.documentElement ? f.fn.offset = function(a) {
-        var b = this[0],
-            c;
-        if (a) return this.each(function(b) {
-            f.offset.setOffset(this, a, b)
-        });
-        if (!b || !b.ownerDocument) return null;
-        if (b === b.ownerDocument.body) return f.offset.bodyOffset(b);
-        try {
-            c = b.getBoundingClientRect()
-        } catch (d) {}
-        var e = b.ownerDocument,
-            g = e.documentElement;
-        if (!c || !f.contains(g, b)) return c ? {
-            top: c.top,
-            left: c.left
-        } : {
-            top: 0,
-            left: 0
-        };
-        var h = e.body,
-            i = cy(e),
-            j = g.clientTop || h.clientTop || 0,
-            k = g.clientLeft || h.clientLeft || 0,
-            l = i.pageYOffset || f.support.boxModel && g.scrollTop || h.scrollTop,
-            m = i.pageXOffset || f.support.boxModel && g.scrollLeft || h.scrollLeft,
-            n = c.top + l - j,
-            o = c.left + m - k;
-        return {
-            top: n,
-            left: o
-        }
-    } : f.fn.offset = function(a) {
-        var b = this[0];
-        if (a) return this.each(function(b) {
-            f.offset.setOffset(this, a, b)
-        });
-        if (!b || !b.ownerDocument) return null;
-        if (b === b.ownerDocument.body) return f.offset.bodyOffset(b);
-        var c, d = b.offsetParent,
-            e = b,
-            g = b.ownerDocument,
-            h = g.documentElement,
-            i = g.body,
-            j = g.defaultView,
-            k = j ? j.getComputedStyle(b, null) : b.currentStyle,
-            l = b.offsetTop,
-            m = b.offsetLeft;
-        while ((b = b.parentNode) && b !== i && b !== h) {
-            if (f.support.fixedPosition && k.position === "fixed") break;
-            c = j ? j.getComputedStyle(b, null) : b.currentStyle, l -= b.scrollTop, m -= b.scrollLeft, b === d && (l += b.offsetTop, m += b.offsetLeft, f.support.doesNotAddBorder && (!f.support.doesAddBorderForTableAndCells || !cw.test(b.nodeName)) && (l += parseFloat(c.borderTopWidth) || 0, m += parseFloat(c.borderLeftWidth) || 0), e = d, d = b.offsetParent), f.support.subtractsBorderForOverflowNotVisible && c.overflow !== "visible" && (l += parseFloat(c.borderTopWidth) || 0, m += parseFloat(c.borderLeftWidth) || 0), k = c
-        }
-        if (k.position === "relative" || k.position === "static") l += i.offsetTop, m += i.offsetLeft;
-        f.support.fixedPosition && k.position === "fixed" && (l += Math.max(h.scrollTop, i.scrollTop), m += Math.max(h.scrollLeft, i.scrollLeft));
-        return {
-            top: l,
-            left: m
-        }
-    }, f.offset = {
-        bodyOffset: function(a) {
-            var b = a.offsetTop,
-                c = a.offsetLeft;
-            f.support.doesNotIncludeMarginInBodyOffset && (b += parseFloat(f.css(a, "marginTop")) || 0, c += parseFloat(f.css(a, "marginLeft")) || 0);
-            return {
-                top: b,
-                left: c
-            }
-        },
+    };
+
+    function Mb(a) {
+        return n.isWindow(a) ? a : 9 === a.nodeType && a.defaultView
+    }
+    n.offset = {
         setOffset: function(a, b, c) {
-            var d = f.css(a, "position");
-            d === "static" && (a.style.position = "relative");
-            var e = f(a),
-                g = e.offset(),
-                h = f.css(a, "top"),
-                i = f.css(a, "left"),
-                j = (d === "absolute" || d === "fixed") && f.inArray("auto", [h, i]) > -1,
-                k = {},
-                l = {},
-                m, n;
-            j ? (l = e.position(), m = l.top, n = l.left) : (m = parseFloat(h) || 0, n = parseFloat(i) || 0), f.isFunction(b) && (b = b.call(a, c, g)), b.top != null && (k.top = b.top - g.top + m), b.left != null && (k.left = b.left - g.left + n), "using" in b ? b.using.call(a, k) : e.css(k)
-        }
-    }, f.fn.extend({
-        position: function() {
-            if (!this[0]) return null;
-            var a = this[0],
-                b = this.offsetParent(),
-                c = this.offset(),
-                d = cx.test(b[0].nodeName) ? {
+            var d, e, f, g, h, i, j, k = n.css(a, "position"),
+                l = n(a),
+                m = {};
+            "static" === k && (a.style.position = "relative"), h = l.offset(), f = n.css(a, "top"), i = n.css(a, "left"), j = ("absolute" === k || "fixed" === k) && (f + i).indexOf("auto") > -1, j ? (d = l.position(), g = d.top, e = d.left) : (g = parseFloat(f) || 0, e = parseFloat(i) || 0), n.isFunction(b) && (b = b.call(a, c, n.extend({}, h))), null != b.top && (m.top = b.top - h.top + g), null != b.left && (m.left = b.left - h.left + e), "using" in b ? b.using.call(a, m) : l.css(m)
+        }
+    }, n.fn.extend({
+        offset: function(a) {
+            if (arguments.length) return void 0 === a ? this : this.each(function(b) {
+                n.offset.setOffset(this, a, b)
+            });
+            var b, c, d = this[0],
+                e = {
                     top: 0,
                     left: 0
-                } : b.offset();
-            c.top -= parseFloat(f.css(a, "marginTop")) || 0, c.left -= parseFloat(f.css(a, "marginLeft")) || 0, d.top += parseFloat(f.css(b[0], "borderTopWidth")) || 0, d.left += parseFloat(f.css(b[0], "borderLeftWidth")) || 0;
-            return {
-                top: c.top - d.top,
-                left: c.left - d.left
+                },
+                f = d && d.ownerDocument;
+            if (f) return b = f.documentElement, n.contains(b, d) ? (e = d.getBoundingClientRect(), c = Mb(f), {
+                top: e.top + c.pageYOffset - b.clientTop,
+                left: e.left + c.pageXOffset - b.clientLeft
+            }) : e
+        },
+        position: function() {
+            if (this[0]) {
+                var a, b, c = this[0],
+                    d = {
+                        top: 0,
+                        left: 0
+                    };
+                return "fixed" === n.css(c, "position") ? b = c.getBoundingClientRect() : (a = this.offsetParent(), b = this.offset(), n.nodeName(a[0], "html") || (d = a.offset()), d.top += n.css(a[0], "borderTopWidth", !0), d.left += n.css(a[0], "borderLeftWidth", !0)), {
+                    top: b.top - d.top - n.css(c, "marginTop", !0),
+                    left: b.left - d.left - n.css(c, "marginLeft", !0)
+                }
             }
         },
         offsetParent: function() {
             return this.map(function() {
-                var a = this.offsetParent || c.body;
-                while (a && !cx.test(a.nodeName) && f.css(a, "position") === "static") a = a.offsetParent;
-                return a
+                var a = this.offsetParent;
+                while (a && "static" === n.css(a, "position")) a = a.offsetParent;
+                return a || Ea
             })
         }
-    }), f.each(["Left", "Top"], function(a, c) {
-        var d = "scroll" + c;
-        f.fn[d] = function(c) {
-            var e, g;
-            if (c === b) {
-                e = this[0];
-                if (!e) return null;
-                g = cy(e);
-                return g ? "pageXOffset" in g ? g[a ? "pageYOffset" : "pageXOffset"] : f.support.boxModel && g.document.documentElement[d] || g.document.body[d] : e[d]
+    }), n.each({
+        scrollLeft: "pageXOffset",
+        scrollTop: "pageYOffset"
+    }, function(a, b) {
+        var c = "pageYOffset" === b;
+        n.fn[a] = function(d) {
+            return K(this, function(a, d, e) {
+                var f = Mb(a);
+                return void 0 === e ? f ? f[b] : a[d] : void(f ? f.scrollTo(c ? f.pageXOffset : e, c ? e : f.pageYOffset) : a[d] = e)
+            }, a, d, arguments.length)
+        }
+    }), n.each(["top", "left"], function(a, b) {
+        n.cssHooks[b] = Ga(l.pixelPosition, function(a, c) {
+            return c ? (c = Fa(a, b), Ba.test(c) ? n(a).position()[b] + "px" : c) : void 0
+        })
+    }), n.each({
+        Height: "height",
+        Width: "width"
+    }, function(a, b) {
+        n.each({
+            padding: "inner" + a,
+            content: b,
+            "": "outer" + a
+        }, function(c, d) {
+            n.fn[d] = function(d, e) {
+                var f = arguments.length && (c || "boolean" != typeof d),
+                    g = c || (d === !0 || e === !0 ? "margin" : "border");
+                return K(this, function(b, c, d) {
+                    var e;
+                    return n.isWindow(b) ? b.document.documentElement["client" + a] : 9 === b.nodeType ? (e = b.documentElement, Math.max(b.body["scroll" + a], e["scroll" + a], b.body["offset" + a], e["offset" + a], e["client" + a])) : void 0 === d ? n.css(b, c, g) : n.style(b, c, d, g)
+                }, b, f ? d : void 0, f, null)
             }
-            return this.each(function() {
-                g = cy(this), g ? g.scrollTo(a ? f(g).scrollLeft() : c, a ? c : f(g).scrollTop()) : this[d] = c
-            })
+        })
+    }), n.fn.extend({
+        bind: function(a, b, c) {
+            return this.on(a, null, b, c)
+        },
+        unbind: function(a, b) {
+            return this.off(a, null, b)
+        },
+        delegate: function(a, b, c, d) {
+            return this.on(b, a, c, d)
+        },
+        undelegate: function(a, b, c) {
+            return 1 === arguments.length ? this.off(a, "**") : this.off(b, a || "**", c)
+        },
+        size: function() {
+            return this.length
         }
-    }), f.each(["Height", "Width"], function(a, c) {
-        var d = c.toLowerCase();
-        f.fn["inner" + c] = function() {
-            var a = this[0];
-            return a ? a.style ? parseFloat(f.css(a, d, "padding")) : this[d]() : null
-        }, f.fn["outer" + c] = function(a) {
-            var b = this[0];
-            return b ? b.style ? parseFloat(f.css(b, d, a ? "margin" : "border")) : this[d]() : null
-        }, f.fn[d] = function(a) {
-            var e = this[0];
-            if (!e) return a == null ? null : this;
-            if (f.isFunction(a)) return this.each(function(b) {
-                var c = f(this);
-                c[d](a.call(this, b, c[d]()))
-            });
-            if (f.isWindow(e)) {
-                var g = e.document.documentElement["client" + c],
-                    h = e.document.body;
-                return e.document.compatMode === "CSS1Compat" && g || h && h["client" + c] || g
-            }
-            if (e.nodeType === 9) return Math.max(e.documentElement["client" + c], e.body["scroll" + c], e.documentElement["scroll" + c], e.body["offset" + c], e.documentElement["offset" + c]);
-            if (a === b) {
-                var i = f.css(e, d),
-                    j = parseFloat(i);
-                return f.isNumeric(j) ? j : i
-            }
-            return this.css(d, typeof a == "string" ? a : a + "px")
-        }
-    }), a.jQuery = a.$ = f, typeof define == "function" && define.amd && define.amd.jQuery && define("jquery", [], function() {
-        return f
-    })
-})(window);
+    }), n.fn.andSelf = n.fn.addBack, "function" == typeof define && define.amd && define("jquery", [], function() {
+        return n
+    });
+    var Nb = a.jQuery,
+        Ob = a.$;
+    return n.noConflict = function(b) {
+        return a.$ === n && (a.$ = Ob), b && a.jQuery === n && (a.jQuery = Nb), n
+    }, b || (a.jQuery = a.$ = n), n
+});
```

### Comparing `puput-1.2.1/puput/static/puput/js/js.cookie.js` & `puput-2.0.0/puput/static/puput/js/js.cookie.js`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/static/puput/js/puput.js` & `puput-2.0.0/puput/static/puput/js/puput.js`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/templates/puput/base.html` & `puput-2.0.0/puput/templates/puput/base.html`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/templates/puput/blog_page.html` & `puput-2.0.0/puput/templates/puput/blog_page.html`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/templates/puput/comments/disqus.html` & `puput-2.0.0/puput/templates/puput/comments/disqus.html`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/templates/puput/entry_links.html` & `puput-2.0.0/puput/templates/puput/entry_links.html`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/templates/puput/entry_page.html` & `puput-2.0.0/puput/templates/puput/entry_page.html`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/templates/puput/related_entries.html` & `puput-2.0.0/puput/templates/puput/related_entries.html`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/templates/puput/tags/archives_list.html` & `puput-2.0.0/puput/templates/puput/tags/archives_list.html`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/templates/puput/tags/entries_list.html` & `puput-2.0.0/puput/templates/puput/tags/entries_list.html`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/templates/wagtailadmin/pages/_editor_css.html` & `puput-2.0.0/puput/templates/wagtailadmin/pages/_editor_css.html`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/templatetags/puput_tags.py` & `puput-2.0.0/puput/templatetags/puput_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django_social_share.templatetags.social_share import _build_url
 from el_pagination.templatetags.el_pagination_tags import show_pages, paginate
 
 from ..conf import settings
 from ..utils import import_model
 from ..models import Category, Tag
 
-from wagtail.core.models import Site
+from wagtail.models import Site
 
 register = Library()
 
 
 @register.inclusion_tag("puput/tags/entries_list.html", takes_context=True)
 def recent_entries(context, limit=None):
     blog_page = context["blog_page"]
```

### Comparing `puput-1.2.1/puput/urls.py` & `puput-2.0.0/puput/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     ),
     path(route="<int:year>/<int:month>/<int:day>/<str:slug>/", view=EntryPageServe.as_view(), name="entry_page_serve"),
     path(route="<path:blog_path>/feed/", view=BlogPageFeed(), name="blog_page_feed_slug"),
     path(route="feed/", view=BlogPageFeed(), name="blog_page_feed"),
 ]
 
 if not getattr(settings, "PUPUT_AS_PLUGIN", False):
-    from wagtail.core import urls as wagtail_urls
+    from wagtail import urls as wagtail_urls
     from wagtail.admin import urls as wagtailadmin_urls
     from wagtail.documents import urls as wagtaildocs_urls
     from wagtail.contrib.sitemaps.views import sitemap
 
     urlpatterns.extend(
         [
             path(route="blog_admin/", view=include(wagtailadmin_urls)),
```

### Comparing `puput-1.2.1/puput/utils.py` & `puput-2.0.0/puput/utils.py`

 * *Files identical despite different names*

### Comparing `puput-1.2.1/puput/views.py` & `puput-2.0.0/puput/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.conf import settings
 from django.http import Http404, HttpResponse
 from django.views.generic import View
 from django.views.decorators.csrf import ensure_csrf_cookie
 from django.utils.decorators import method_decorator
 
-from wagtail.core import hooks
-from wagtail.core.models import Site
+from wagtail import hooks
+from wagtail.models import Site
 
 from .models import EntryPage
 from .utils import strip_prefix_and_ending_slash, import_model
 
 
 class EntryPageServe(View):
     """
```

### Comparing `puput-1.2.1/puput/wagtail_hooks.py` & `puput-2.0.0/puput/wagtail_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import wagtail.admin.rich_text.editors.draftail.features as draftail_features
 from wagtail.admin.rich_text.converters.html_to_contentstate import InlineStyleElementHandler, BlockElementHandler
-from wagtail.core import hooks
+from wagtail import hooks
 
 
 @hooks.register("register_rich_text_features")
 def register_blockquote_feature(features):
     """
     Registering the `blockquote` feature, which uses the `blockquote` Draft.js block type,
     and is stored as HTML with a `<blockquote>` tag.
```

### Comparing `puput-1.2.1/puput.egg-info/PKG-INFO` & `puput-2.0.0/puput.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: puput
-Version: 1.2.1
+Version: 2.0.0
 Summary: A Django blog app implemented in Wagtail.
 Home-page: http://github.com/APSL/puput
 Author: Marc Tudurí
 Author-email: marctc@gmail.com
 Keywords: django wagtail puput blog cms app
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -68,22 +69,19 @@
 
 .. image:: http://i.imgur.com/d13sGI3.png
 
 Examples of blog sites made with Puput
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * `Open Study Room <https://openstudyroom.org/blog/>`_
-* `Ncora Blog <https://www.ncora.com/blog/>`_
-* `Ncora TV <https://www.ncora.com/tv/>`_
 * `APSL <https://www.apsl.net/blog/>`_
 * `Nautic Advisor <https://www.nauticadvisor.com/blog/>`_
 * `Trespams <http://trespams.com/blog/>`_
 * `Body Therapy <http://bodytherapy.ru/blog/>`_
 * `Astro <http://www.mallorcasoft.es/blog/>`_
-* `Kontrabando Film Festival <https://www.kontrabandofilmfestival.org/blog/>`_
 * `IP/DE <https://ipde.com/>`_
 
 Setup
 ~~~~~
 
 The setup process is explained `here <http://puput.readthedocs.io/en/latest/setup.html>`_.
```

### Comparing `puput-1.2.1/puput.egg-info/SOURCES.txt` & `puput-2.0.0/puput.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 puput/migrations/0001_initial.py
 puput/migrations/0002_auto_20150919_0925.py
 puput/migrations/0003_add_short_feed_description_to_blog_page.py
 puput/migrations/0004_auto_20170912_0928.py
 puput/migrations/0005_blogpage_main_color.py
 puput/migrations/0006_entrypage_markdown_body.py
 puput/migrations/0007_alter_entrypage_body.py
+puput/migrations/0008_alter_tagentrypage_tag.py
 puput/migrations/__init__.py
 puput/static/colorful/arrow.gif
 puput/static/colorful/colorPicker.css
 puput/static/puput/css/bootstrap.min.css
 puput/static/puput/css/font-awesome.min.css
 puput/static/puput/css/puput.css
 puput/static/puput/fonts/FontAwesome.otf
```

### Comparing `puput-1.2.1/setup.py` & `puput-2.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,31 +21,33 @@
     version=get_metadata('puput', 'version'),
     packages=find_packages(exclude=("example*", "tests*")),
     include_package_data=True,
     keywords="django wagtail puput blog cms app",
     description='A Django blog app implemented in Wagtail.',
     long_description=codecs.open(os.path.join(os.path.dirname(__file__), 'README.rst'), encoding='utf-8').read(),
     install_requires=[
-        'Django>=3.2,<4.2',
-        'wagtail>=3.0,<4.2',
+        'Django>=3.2,<4.3',
+        'wagtail>=4.0,<5.1',
         'django-el-pagination==4.0.0',
         'django-social-share>=1.3.0',
         'django-colorful>=1.3',
+        'django-taggit>=3.1.0,<4.1',
         'wagtail-markdown==0.11.0'
     ],
     url='http://github.com/APSL/puput',
     author=get_metadata('puput', 'author'),
     author_email=get_metadata('puput', 'email'),
     long_description_content_type='text/x-rst',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

