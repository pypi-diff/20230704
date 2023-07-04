# Comparing `tmp/BAC0-22.9.21.tar.gz` & `tmp/BAC0-23.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BAC0-22.9.21.tar", last modified: Thu Sep 22 02:09:49 2022, max compression
+gzip compressed data, was "BAC0-23.7.3.tar", last modified: Tue Jul  4 01:58:24 2023, max compression
```

## Comparing `BAC0-22.9.21.tar` & `BAC0-23.7.3.tar`

### file list

```diff
@@ -1,185 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.264424 BAC0-22.9.21/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.236423 BAC0-22.9.21/BAC0/
--rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.236423 BAC0-22.9.21/BAC0/core/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.236423 BAC0-22.9.21/BAC0/core/app/
--rw-r--r--   0 runner    (1001) docker     (121)    14683 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/app/ScriptApplication.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.236423 BAC0-22.9.21/BAC0/core/devices/
--rwxr-xr-x   0 runner    (1001) docker     (121)    39200 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/Device.py
--rw-r--r--   0 runner    (1001) docker     (121)    41754 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/Points.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8550 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/Trends.py
--rw-r--r--   0 runner    (1001) docker     (121)     8216 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/Virtuals.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6317 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/create_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.236423 BAC0-22.9.21/BAC0/core/devices/local/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7583 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/local/decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7606 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/local/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     9110 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/local/object.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.236423 BAC0-22.9.21/BAC0/core/devices/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)    16340 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/mixins/CommandableMixin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/mixins/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    28027 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/devices/mixins/read_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.240423 BAC0-22.9.21/BAC0/core/functions/
--rw-r--r--   0 runner    (1001) docker     (121)     6914 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/functions/Calendar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3000 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/functions/DeviceCommunicationControl.py
--rw-r--r--   0 runner    (1001) docker     (121)    14297 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/functions/Discover.py
--rw-r--r--   0 runner    (1001) docker     (121)     3982 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/functions/GetIPAddr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/functions/Reinitialize.py
--rw-r--r--   0 runner    (1001) docker     (121)    11140 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/functions/Schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)     2220 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/functions/Text.py
--rw-r--r--   0 runner    (1001) docker     (121)     5037 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/functions/TimeSync.py
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5711 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/functions/cov.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.240423 BAC0-22.9.21/BAC0/core/io/
--rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/io/IOExceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    33614 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/io/Read.py
--rw-r--r--   0 runner    (1001) docker     (121)     4172 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/io/Simulate.py
--rw-r--r--   0 runner    (1001) docker     (121)    12642 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/io/Write.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.240423 BAC0-22.9.21/BAC0/core/proprietary_objects/
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/proprietary_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13310 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/proprietary_objects/jci.py
--rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/proprietary_objects/object.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.240423 BAC0-22.9.21/BAC0/core/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9441 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/core/utils/notes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.240423 BAC0-22.9.21/BAC0/db/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8503 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/db/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (121)    10737 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/db/sql.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/infos.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.240423 BAC0-22.9.21/BAC0/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)    12378 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/scripts/Base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8901 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/scripts/Complete.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16594 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/scripts/Lite.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.244423 BAC0-22.9.21/BAC0/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)     2990 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/tasks/Devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/tasks/DoOnce.py
--rw-r--r--   0 runner    (1001) docker     (121)     3267 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/tasks/Match.py
--rw-r--r--   0 runner    (1001) docker     (121)     7139 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/tasks/Poll.py
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/tasks/RecurringTask.py
--rw-r--r--   0 runner    (1001) docker     (121)     7288 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/tasks/TaskManager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/tasks/UpdateCOV.py
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.244423 BAC0-22.9.21/BAC0/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/tools/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     3022 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/tools/tad_display.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.244423 BAC0-22.9.21/BAC0/web/
--rw-r--r--   0 runner    (1001) docker     (121)    27183 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/BokehRenderer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/BokehServer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6410 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/FlaskServer.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.232422 BAC0-22.9.21/BAC0/web/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.232422 BAC0-22.9.21/BAC0/web/static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.248423 BAC0-22.9.21/BAC0/web/static/assets/css/
--rw-r--r--   0 runner    (1001) docker     (121)     6148 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/css/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (121)    55523 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/css/animate.min.css
--rw-r--r--   0 runner    (1001) docker     (121)   122540 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/css/demo.css
--rw-r--r--   0 runner    (1001) docker     (121)    96563 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/css/paper-dashboard.css
--rw-r--r--   0 runner    (1001) docker     (121)    16454 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/css/themify-icons.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.248423 BAC0-22.9.21/BAC0/web/static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)     6148 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/fonts/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (121)    78748 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/fonts/themify.eot
--rw-r--r--   0 runner    (1001) docker     (121)   234269 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/fonts/themify.svg
--rw-r--r--   0 runner    (1001) docker     (121)    78584 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/fonts/themify.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    56108 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/fonts/themify.woff
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.252423 BAC0-22.9.21/BAC0/web/static/assets/img/
--rw-r--r--   0 runner    (1001) docker     (121)     8196 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (121)   796044 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/31554.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     7157 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/GitHub-Mark.png
--rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/apple-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.252423 BAC0-22.9.21/BAC0/web/static/assets/img/background/
--rw-r--r--   0 runner    (1001) docker     (121)     6148 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/background/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (121)    39026 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/background.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   395363 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/bg.png
--rw-r--r--   0 runner    (1001) docker     (121)  1360901 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/bg.xcf
--rw-r--r--   0 runner    (1001) docker     (121)     4907 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/devices2.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.256423 BAC0-22.9.21/BAC0/web/static/assets/img/faces/
--rw-r--r--   0 runner    (1001) docker     (121)     6148 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/faces/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (121)    17964 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/faces/face-0.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    20568 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/faces/face-1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    55860 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/faces/face-2.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    41590 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/faces/face-3.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     2871 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/favicon.png
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/gitter2.png
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/histories2.png
--rw-r--r--   0 runner    (1001) docker     (121)     3557 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/new_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/notes.png
--rw-r--r--   0 runner    (1001) docker     (121)     7413 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/readthedocs.png
--rw-r--r--   0 runner    (1001) docker     (121)     8686 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/search.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.256423 BAC0-22.9.21/BAC0/web/static/assets/img/tables/
--rw-r--r--   0 runner    (1001) docker     (121)     6148 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/tables/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (121)     4821 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/tim_80x80.png
--rw-r--r--   0 runner    (1001) docker     (121)    16745 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/img/wordpress.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.256423 BAC0-22.9.21/BAC0/web/static/assets/js/
--rw-r--r--   0 runner    (1001) docker     (121)     6148 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/js/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/js/BAC0_script.js
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/js/bac0.js
--rw-r--r--   0 runner    (1001) docker     (121)     6978 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/js/bootstrap-checkbox-radio.js
--rw-r--r--   0 runner    (1001) docker     (121)    13213 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/js/bootstrap-notify.js
--rw-r--r--   0 runner    (1001) docker     (121)    36816 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    36026 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/js/chartist.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     9745 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/js/demo.js
--rw-r--r--   0 runner    (1001) docker     (121)   273198 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/js/jquery-1.10.2.js
--rw-r--r--   0 runner    (1001) docker     (121)     5427 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/js/paper-dashboard.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.256423 BAC0-22.9.21/BAC0/web/static/assets/sass/
--rw-r--r--   0 runner    (1001) docker     (121)     6148 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.260424 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_alerts.scss
--rw-r--r--   0 runner    (1001) docker     (121)     3063 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (121)     4571 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (121)     6817 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_chartist.scss
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_checkbox-radio.scss
--rw-r--r--   0 runner    (1001) docker     (121)     2948 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_footers.scss
--rw-r--r--   0 runner    (1001) docker     (121)     4151 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_inputs.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (121)     5541 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_navbars.scss
--rw-r--r--   0 runner    (1001) docker     (121)    10457 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_responsive.scss
--rw-r--r--   0 runner    (1001) docker     (121)     4566 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_sidebar-and-main-panel.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (121)     8872 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.260424 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (121)     3585 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_chartist.scss
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_inputs.scss
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_labels.scss
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_navbars.scss
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_sidebar.scss
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_tabs.scss
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_transparency.scss
--rw-r--r--   0 runner    (1001) docker     (121)     6728 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_vendor-prefixes.scss
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/static/assets/sass/paper-dashboard.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.260424 BAC0-22.9.21/BAC0/web/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/templates/device_table.html
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/templates/embed_bck.html
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (121)    13636 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/templates/notifications.html
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/templates/theme.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/templates/trends.html
--rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-09-22 02:09:38.000000 BAC0-22.9.21/BAC0/web/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 02:09:49.236423 BAC0-22.9.21/BAC0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4970 2022-09-22 02:09:49.000000 BAC0-22.9.21/BAC0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5516 2022-09-22 02:09:49.000000 BAC0-22.9.21/BAC0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 02:09:49.000000 BAC0-22.9.21/BAC0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-22 02:09:49.000000 BAC0-22.9.21/BAC0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-22 02:09:49.000000 BAC0-22.9.21/BAC0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-09-22 02:09:38.000000 BAC0-22.9.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-22 02:09:38.000000 BAC0-22.9.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4970 2022-09-22 02:09:49.264424 BAC0-22.9.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4224 2022-09-22 02:09:38.000000 BAC0-22.9.21/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-22 02:09:49.264424 BAC0-22.9.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-09-22 02:09:38.000000 BAC0-22.9.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.697128 BAC0-23.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.665126 BAC0-23.7.3/BAC0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.669126 BAC0-23.7.3/BAC0/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.669126 BAC0-23.7.3/BAC0/core/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/app/ScriptApplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.669126 BAC0-23.7.3/BAC0/core/devices/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39670 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/Device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42382 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/Points.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9213 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/Trends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/Virtuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/create_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.669126 BAC0-23.7.3/BAC0/core/devices/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/local/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/local/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/local/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/local/trendLogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.669126 BAC0-23.7.3/BAC0/core/devices/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/mixins/CommandableMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/mixins/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28151 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/devices/mixins/read_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.673126 BAC0-23.7.3/BAC0/core/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/functions/Calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/functions/DeviceCommunicationControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/functions/Discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/functions/GetIPAddr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/functions/Reinitialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/functions/Schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/functions/Text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/functions/TimeSync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/functions/cov.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.673126 BAC0-23.7.3/BAC0/core/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/io/IOExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34599 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/io/Read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/io/Simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/io/Write.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.673126 BAC0-23.7.3/BAC0/core/proprietary_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/proprietary_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/proprietary_objects/jci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/proprietary_objects/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.673126 BAC0-23.7.3/BAC0/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/core/utils/notes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.673126 BAC0-23.7.3/BAC0/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/db/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/db/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/infos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.673126 BAC0-23.7.3/BAC0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/scripts/Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/scripts/Complete.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17545 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/scripts/Lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.677127 BAC0-23.7.3/BAC0/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/tasks/Devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/tasks/DoOnce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/tasks/Match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/tasks/Poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/tasks/RecurringTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/tasks/TaskManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/tasks/UpdateCOV.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.677127 BAC0-23.7.3/BAC0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/tools/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/tools/tad_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.677127 BAC0-23.7.3/BAC0/web/
+-rw-r--r--   0 runner    (1001) docker     (123)    26780 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/BokehRenderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/BokehServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/FlaskServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.665126 BAC0-23.7.3/BAC0/web/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.665126 BAC0-23.7.3/BAC0/web/static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.677127 BAC0-23.7.3/BAC0/web/static/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/css/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)    55523 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/css/animate.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   122540 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/css/demo.css
+-rw-r--r--   0 runner    (1001) docker     (123)    96563 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/css/paper-dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/css/themify-icons.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.677127 BAC0-23.7.3/BAC0/web/static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/fonts/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)    78748 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/fonts/themify.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   234269 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/fonts/themify.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    78584 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/fonts/themify.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    56108 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/fonts/themify.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.689127 BAC0-23.7.3/BAC0/web/static/assets/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)   796044 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/31554.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/GitHub-Mark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/apple-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.689127 BAC0-23.7.3/BAC0/web/static/assets/img/background/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/background/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)    39026 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/background.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   395363 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/bg.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1360901 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/bg.xcf
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/devices2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.689127 BAC0-23.7.3/BAC0/web/static/assets/img/faces/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/faces/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/faces/face-0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    20568 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/faces/face-1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    55860 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/faces/face-2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    41590 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/faces/face-3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/gitter2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/histories2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/new_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/notes.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/readthedocs.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/search.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.689127 BAC0-23.7.3/BAC0/web/static/assets/img/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/tables/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/tim_80x80.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/img/wordpress.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.689127 BAC0-23.7.3/BAC0/web/static/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/js/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/js/BAC0_script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/js/bac0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/js/bootstrap-checkbox-radio.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/js/bootstrap-notify.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36816 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36026 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/js/chartist.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/js/demo.js
+-rw-r--r--   0 runner    (1001) docker     (123)   273198 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/js/jquery-1.10.2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/js/paper-dashboard.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.693127 BAC0-23.7.3/BAC0/web/static/assets/sass/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.693127 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_alerts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_chartist.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_checkbox-radio.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_footers.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_inputs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_navbars.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_responsive.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_sidebar-and-main-panel.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.697128 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_chartist.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_inputs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_labels.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_navbars.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_sidebar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_tabs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_transparency.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_vendor-prefixes.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/static/assets/sass/paper-dashboard.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.697128 BAC0-23.7.3/BAC0/web/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/templates/device_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/templates/embed_bck.html
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/templates/notifications.html
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/templates/theme.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/templates/trends.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-04 01:58:13.000000 BAC0-23.7.3/BAC0/web/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.669126 BAC0-23.7.3/BAC0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-04 01:58:24.000000 BAC0-23.7.3/BAC0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-07-04 01:58:24.000000 BAC0-23.7.3/BAC0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:58:24.000000 BAC0-23.7.3/BAC0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 01:58:24.000000 BAC0-23.7.3/BAC0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-04 01:58:24.000000 BAC0-23.7.3/BAC0.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-04 01:58:13.000000 BAC0-23.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 01:58:13.000000 BAC0-23.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-04 01:58:24.697128 BAC0-23.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-04 01:58:13.000000 BAC0-23.7.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:58:24.697128 BAC0-23.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-04 01:58:13.000000 BAC0-23.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:58:24.697128 BAC0-23.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-04 01:58:13.000000 BAC0-23.7.3/tests/test_0BacpypesVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-04 01:58:13.000000 BAC0-23.7.3/tests/test_1AddressesTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-04 01:58:13.000000 BAC0-23.7.3/tests/test_BAC0_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-04 01:58:13.000000 BAC0-23.7.3/tests/test_BAC0_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-04 01:58:13.000000 BAC0-23.7.3/tests/test_Read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-04 01:58:13.000000 BAC0-23.7.3/tests/test_SaveToSQL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-04 01:58:13.000000 BAC0-23.7.3/tests/test_WhoHasIHave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-04 01:58:13.000000 BAC0-23.7.3/tests/test_Write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-04 01:58:13.000000 BAC0-23.7.3/tests/test_proprietaryobjects.py
```

### Comparing `BAC0-22.9.21/BAC0/__init__.py` & `BAC0-23.7.3/BAC0/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,32 +9,31 @@
     print(
         'bacpypes module missing, please install latest version using \n    $ "pip install bacpypes"'
     )
     print("\nDiscard this message if you are actually installing BAC0.")
     print("=" * 80)
 
 try:
-    from . import core
-    from . import tasks
-    from .scripts.Base import Base
+    from . import core, tasks
     from .core.devices.Device import Device as device
     from .core.devices.Device import DeviceLoad as load
     from .core.devices.Trends import TrendLog as TrendLog
-    from .tasks.Poll import SimplePoll as poll
-    from .tasks.Match import Match as match
-    from .tasks.Devices import AddDevice as add_device
     from .core.utils.notes import update_log_level as log_level
     from .infos import __version__ as version
+    from .scripts.Base import Base
+    from .tasks.Devices import AddDevice as add_device
+    from .tasks.Match import Match as match
+    from .tasks.Poll import SimplePoll as poll
 
     # To be able to use the complete version pandas, flask and bokeh must be installed.
     try:
-        import pandas
         import bokeh
         import flask
         import flask_bootstrap
+        import pandas
 
         _COMPLETE = True
     except ImportError:
         _COMPLETE = False
 
     try:
         #
@@ -50,15 +49,15 @@
     from .scripts.Lite import Lite as lite
 
     if _COMPLETE:
         from .scripts.Complete import Complete as gui
 
         connect = gui
     else:
-        connect = lite
+        connect = lite  # type: ignore[assignment, misc]
         web = lambda: print(
             "All features not available to run BAC0.web(). Some modules are missing (flask, flask-bootstrap, bokeh, pandas). See docs for details. To start BAC0, use BAC0.lite()"
         )
 
     # Import proprietary classes
     from .core.proprietary_objects import jci
```

### Comparing `BAC0-22.9.21/BAC0/core/app/ScriptApplication.py` & `BAC0-23.7.3/BAC0/core/app/ScriptApplication.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,69 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
-SimpleApplication 
+SimpleApplication
 =================
 
-A basic BACnet application (bacpypes BIPSimpleApplication) for interacting with 
-the bacpypes BACnet stack.  It enables the base-level BACnet functionality 
+A basic BACnet application (bacpypes BIPSimpleApplication) for interacting with
+the bacpypes BACnet stack.  It enables the base-level BACnet functionality
 (a.k.a. device discovery) - meaning it can send & receive WhoIs & IAm messages.
 
-Additional functionality is enabled by inheriting this application, and then 
+Additional functionality is enabled by inheriting this application, and then
 extending it with more functions. [See BAC0.scripts for more examples of this.]
 
 """
+import typing as t
+
 # --- standard Python modules ---
 from collections import defaultdict
+from typing import Any, Dict, Optional
+
+from bacpypes.apdu import IAmRequest, ReadRangeACK, SimpleAckPDU
 
 # --- 3rd party modules ---
 from bacpypes.app import ApplicationIOController
-from bacpypes.pdu import Address
-from bacpypes.service.object import ReadWritePropertyMultipleServices
-from bacpypes.service.cov import ChangeOfValueServices
-from bacpypes.netservice import NetworkServiceAccessPoint, NetworkServiceElement
+from bacpypes.appservice import ApplicationServiceAccessPoint, StateMachineAccessPoint
 from bacpypes.bvllservice import (
-    BIPSimple,
-    BIPForeign,
     BIPBBMD,
     AnnexJCodec,
+    BIPForeign,
+    BIPSimple,
     UDPMultiplexer,
 )
-from bacpypes.apdu import SubscribeCOVRequest, SimpleAckPDU, RejectPDU, AbortPDU
-
-from bacpypes.appservice import StateMachineAccessPoint, ApplicationServiceAccessPoint
-from bacpypes.comm import ApplicationServiceElement, bind, Client
-from bacpypes.iocb import IOCB
+from bacpypes.comm import Client, bind
+from bacpypes.constructeddata import (
+    Array,
+    List,
+    SequenceOfAny,
+)
 from bacpypes.core import deferred
+from bacpypes.errors import ExecutionError, RejectException
+from bacpypes.iocb import IOCB
+from bacpypes.local.device import LocalDeviceObject
+from bacpypes.netservice import NetworkServiceAccessPoint
+from bacpypes.object import PropertyError
+from bacpypes.pdu import Address
+from bacpypes.service.cov import ChangeOfValueServices
 
 # basic services
-from bacpypes.service.device import WhoIsIAmServices, WhoHasIHaveServices
-from bacpypes.service.object import ReadWritePropertyServices
+from bacpypes.service.device import WhoHasIHaveServices, WhoIsIAmServices
+from bacpypes.service.object import (
+    ReadWritePropertyMultipleServices,
+    ReadWritePropertyServices,
+)
+
+from ..functions.Discover import NetworkServiceElementWithRequests
 
 # --- this application's modules ---
 from ..utils.notes import note_and_log
-from ..functions.Discover import NetworkServiceElementWithRequests
 
 # ------------------------------------------------------------------------------
 
 
 class common_mixin:
     """
     They take message coming from the network that are not generated from
@@ -143,14 +157,90 @@
         self._log.debug("Unconfirmed COV Notification: {}".format(elements))
         self.subscription_contexts["context_callback"](elements)
 
         # execute callback
         if context.callback is not None:
             context.callback(elements=elements)
 
+    def do_ReadRangeRequest(self, apdu):
+        self._log.debug("do_ReadRangeRequest %r", apdu)
+
+        # extract the object identifier
+        objId = apdu.objectIdentifier
+
+        # get the object
+        obj = self.get_object_id(objId)
+        self._log.debug("    - object: %r", obj)
+
+        if not obj:
+            raise ExecutionError(errorClass="object", errorCode="unknownObject")
+
+        # get the datatype
+        datatype = obj.get_datatype(apdu.propertyIdentifier)
+        self._log.debug("    - datatype: %r", datatype)
+
+        # must be a list, or an array of lists
+        if issubclass(datatype, List):
+            pass
+        elif (
+            (apdu.propertyArrayIndex is not None)
+            and issubclass(datatype, Array)
+            and issubclass(datatype.subtype, List)
+        ):
+            pass
+        else:
+            raise ExecutionError(errorClass="property", errorCode="propertyIsNotAList")
+
+        # get the value
+        self._log.debug(apdu.__dict__)
+        value = obj.ReadProperty(apdu.propertyIdentifier, apdu.propertyArrayIndex)
+        self._log.debug(f"    - value: {value.__repr__()} | of type {type(value)}")
+        if value is None:
+            raise PropertyError(apdu.propertyIdentifier)
+        if isinstance(value, List):
+            self._log.debug("    - value is a list of: %r", datatype.subtype)
+            # datatype = datatype.subtype
+
+        if apdu.range.byPosition:
+            range_by_position = apdu.range.byPosition
+            self._log.debug("    - range_by_position: %r", range_by_position)
+
+        elif apdu.range.bySequenceNumber:
+            range_by_sequence_number = apdu.range.bySequenceNumber
+            self._log.debug(
+                "    - range_by_sequence_number: %r", range_by_sequence_number
+            )
+
+        elif apdu.range.byTime:
+            range_by_time = apdu.range.byTime
+            self._log.debug("    - range_by_time: %r", range_by_time)
+
+        else:
+            raise RejectException("missingRequiredParameter")
+
+        # this is an ack
+        resp = ReadRangeACK(context=apdu)
+        resp.objectIdentifier = objId
+        resp.propertyIdentifier = apdu.propertyIdentifier
+        resp.propertyArrayIndex = apdu.propertyArrayIndex
+
+        resp.resultFlags = [1, 1, 0]
+        resp.itemCount = len(value)
+
+        # save the result in the item data
+        item_data = SequenceOfAny()
+        item_data.cast_in(value)
+        resp.itemData = item_data
+        self._log.debug("    - itemData : %r", resp.itemData)
+        self._log.debug("    - resp: %r", resp)
+        self.response(resp)
+        # return the result
+        # iocb = IOCB(resp)  # make an IOCB
+        # deferred(self.request_io, iocb)
+
 
 @note_and_log
 class BAC0Application(
     common_mixin,
     ApplicationIOController,
     WhoIsIAmServices,
     WhoHasIHaveServices,
@@ -164,35 +254,36 @@
     :param *args: local object device, local IP address
         See BAC0.scripts.BasicScript for more details.
 
     """
 
     def __init__(
         self,
-        localDevice,
-        localAddress,
+        localDevice: LocalDeviceObject,
+        localAddress: Address,
+        networkNumber: int = None,
         bbmdAddress=None,
-        bbmdTTL=0,
+        bbmdTTL: int = 0,
         deviceInfoCache=None,
         aseID=None,
-        iam_req=None,
-        subscription_contexts=None,
-    ):
+        iam_req: Optional[IAmRequest] = None,
+        subscription_contexts: Optional[Dict[Any, Any]] = None,
+    ) -> None:
 
         ApplicationIOController.__init__(
             self, localDevice, deviceInfoCache, aseID=aseID
         )
 
         self.iam_req = iam_req
         # local address might be useful for subclasses
         if isinstance(localAddress, Address):
             self.localAddress = localAddress
         else:
             self.localAddress = Address(localAddress)
-
+        self.networkNumber = networkNumber
         # include a application decoder
         self.asap = ApplicationServiceAccessPoint()
 
         # pass the device object to the state machine access point so it
         # can know if it should support segmentation
         self.smap = StateMachineAccessPoint(localDevice)
 
@@ -216,17 +307,17 @@
         self.annexj = AnnexJCodec()
         self.mux = UDPMultiplexer(self.localAddress)
 
         # bind the bottom layers
         bind(self.bip, self.annexj, self.mux.annexJ)
 
         # bind the BIP stack to the network, no network number
-        self.nsap.bind(self.bip, address=self.localAddress)
+        self.nsap.bind(self.bip, net=self.networkNumber, address=self.localAddress)
 
-        self.i_am_counter = defaultdict(int)
+        self.i_am_counter: t.Dict[t.Tuple[str, int], int] = defaultdict(int)
         self.i_have_counter = defaultdict(int)
         self.who_is_counter = defaultdict(int)
 
         # keep track of requests to line up responses
         self._request = None
         self._last_i_am_received = []
         self._last_i_have_received = []
@@ -264,14 +355,15 @@
 
     """
 
     def __init__(
         self,
         localDevice,
         localAddress,
+        networkNumber: int = None,
         bbmdAddress=None,
         bbmdTTL=0,
         deviceInfoCache=None,
         aseID=None,
         iam_req=None,
         subscription_contexts=None,
     ):
@@ -364,14 +456,15 @@
 
     bdt = []
 
     def __init__(
         self,
         localDevice,
         localAddress,
+        networkNumber: int = None,
         bdtable=[],
         deviceInfoCache=None,
         aseID=None,
         iam_req=None,
         subscription_contexts=None,
     ):
 
@@ -423,14 +516,15 @@
 
         if self.bdtable:
             for bdtentry in self.bdtable:
                 self.add_peer(bdtentry)
 
         # bind the NSAP to the stack, no network number
         self.nsap.bind(self.bip)
+        # self.nsap.bind(self.bip, net=self.networkNumber)
 
         self.i_am_counter = defaultdict(int)
         self.i_have_counter = defaultdict(int)
         self.who_is_counter = defaultdict(int)
         # keep track of requests to line up responses
         self._request = None
         self._last_i_am_received = []
```

### Comparing `BAC0-22.9.21/BAC0/core/devices/Device.py` & `BAC0-23.7.3/BAC0/core/devices/Device.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,59 +4,53 @@
 # Copyright (C) 2015-2017 by Christian Tremblay, P.Eng <christian.tremblay@servisysDeviceObject.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
 Device.py - describe a BACnet Device
 
 """
+import os.path
+
 # --- standard Python modules ---
 from collections import namedtuple
-from datetime import datetime
-import weakref
-
-import os.path
 
 try:
     import pandas as pd
 
     _PANDAS = True
 except ImportError:
     _PANDAS = False
-import logging
 
 try:
-    from xlwings import Workbook, Sheet, Range, Chart
+    from xlwings import Chart, Range, Sheet, Workbook  # noqa E401
 
     _XLWINGS = True
 except ImportError:
     _XLWINGS = False
 
 
 # --- this application's modules ---
 from bacpypes.basetypes import ServicesSupported
 
-from .Points import NumericPoint, BooleanPoint, EnumPoint, OfflinePoint
+# from ...bokeh.BokehRenderer import BokehPlot
+from ...db.sql import SQLMixin
+from ...tasks.DoOnce import DoOnce
 from ..io.IOExceptions import (
-    NoResponseFromController,
-    SegmentationNotSupported,
     BadDeviceDefinition,
+    DeviceNotConnected,
+    NoResponseFromController,
     RemovedPointException,
+    SegmentationNotSupported,
     WritePropertyException,
     WrongParameter,
-    DeviceNotConnected,
 )
-
-# from ...bokeh.BokehRenderer import BokehPlot
-from ...db.sql import SQLMixin
-from ...tasks.DoOnce import DoOnce
-from .mixins.read_mixin import ReadPropertyMultiple, ReadProperty
-from .Virtuals import VirtualPoint
-
 from ..utils.notes import note_and_log
-
+from .mixins.read_mixin import ReadProperty, ReadPropertyMultiple
+from .Points import BooleanPoint, EnumPoint, NumericPoint, OfflinePoint
+from .Virtuals import VirtualPoint
 
 # ------------------------------------------------------------------------------
 
 
 class DeviceProperties(object):
     """
     This serves as a container for device properties
@@ -130,15 +124,15 @@
     def __init__(
         self,
         address=None,
         device_id=None,
         network=None,
         *,
         poll=10,
-        from_backup=None,
+        from_backup=None,  # filename of backup
         segmentation_supported=True,
         object_list=None,
         auto_save=False,
         save_resampling="1s",
         clear_history_on_save=False,
         history_size=None,
         reconnect_on_failure=True
@@ -163,24 +157,26 @@
         self._reconnect_on_failure = reconnect_on_failure
 
         self.segmentation_supported = segmentation_supported
         self.custom_object_list = object_list
 
         # self.db = None
         # Todo : find a way to normalize the name of the db
-        self.properties.db_name = ""
+        self.properties.db_name = None
 
         self.points = []
         self._list_of_trendlogs = {}
 
         self._polling_task = namedtuple("_polling_task", ["task", "running"])
         self._polling_task.task = None
         self._polling_task.running = False
 
+        self._find_overrides_progress = 0.0
         self._find_overrides_running = False
+        self._release_overrides_progress = 0.0
         self._release_overrides_running = False
 
         self.note("Controller initialized")
 
         if from_backup:
             filename = from_backup
             db_name = filename.split(".")[0]
@@ -246,15 +242,15 @@
         """
         iterate over simulated points
 
         :returns: points if simulated (out_of_service == True)
         :rtype: BAC0.core.devices.Points.Point
         """
         for each in self.points:
-            if each.properties.simulated:
+            if each.properties.simulated[0]:
                 yield each
 
     def _buildPointList(self):
         """
         Read all points from a device into a (Pandas) dataframe (Pandas).  Items are
         accessible by point name.
         """
@@ -379,15 +375,15 @@
             self._log.warning(
                 "Already running ({:.1%})... please wait.".format(
                     self._find_overrides_progress
                 )
             )
             return
         lst = []
-        self._find_overrides_progress = 0
+        self._find_overrides_progress = 0.0
         self._find_overrides_running = True
         total = len(self.points)
 
         def _find_overrides():
             self._log.warning(
                 "Overrides are being checked, wait for completion message."
             )
@@ -396,31 +392,31 @@
                     lst.append(point)
                 self._find_overrides_progress = idx / total
             self._log.warning(
                 "Override check ready, results available in device.properties.points_overridden"
             )
             self.properties.points_overridden = lst
             self._find_overrides_running = False
-            self._find_overrides_progress = 1
+            self._find_overrides_progress = 1.0
 
         self.do(_find_overrides)
 
-    def find_overrides_progress(self):
+    def find_overrides_progress(self) -> float:
         return self._find_overrides_progress
 
     def release_all_overrides(self, force=False):
         if self._release_overrides_running and not force:
             self._log.warning(
                 "Already running ({:.1%})... please wait.".format(
                     self._release_overrides_progress
                 )
             )
             return
         self._release_overrides_running = True
-        self._release_overrides_progress = 0
+        self._release_overrides_progress = 0.0
 
         def _release_all_overrides():
             self.find_overrides()
             while self._find_overrides_running:
                 self._release_overrides_progress = self._find_overrides_progress * 0.5
 
             if self.properties.points_overridden:
@@ -457,19 +453,23 @@
     def _init_state(self):
         self._buildPointList()
         self.properties.network.register_device(self)
 
     def disconnect(self, save_on_disconnect=True, unregister=True):
         self._log.info("Wait while stopping polling")
         self.poll(command="stop")
-        if save_on_disconnect:
-            self.save()
         if unregister:
             self.properties.network.unregister_device(self)
-        self.new_state(DeviceFromDB)
+            self.properties.network = None
+        if save_on_disconnect:
+            self.save()
+        if self.properties.db_name:
+            self.new_state(DeviceFromDB)
+        else:
+            self.new_state(DeviceDisconnected)
 
     def connect(self, *, db=None):
         """
         A connected device can be switched to 'database mode' where the device will
         not use the BACnet network but instead obtain its contents from a previously
         stored database.
         """
@@ -509,15 +509,15 @@
                 )
             )
 
         except NoResponseFromController as error:
             self._log.error("Controller not found, aborting. ({})".format(error))
             return ("Not Found", "", [], [])
 
-        except SegmentationNotSupported as error:
+        except SegmentationNotSupported:
             self._log.warning("Segmentation not supported")
             self.segmentation_supported = False
             self.new_state(DeviceDisconnected)
 
         self.properties.name = self.properties.network.read(
             "{} device {} objectName".format(
                 self.properties.address, self.properties.device_id
@@ -535,23 +535,23 @@
         )
         try:
             (
                 self.properties.objects_list,
                 self.points,
                 self._list_of_trendlogs,
             ) = self._discoverPoints(self.custom_object_list)
-            if self.properties.pollDelay > 0:
+            if self.properties.pollDelay is not None and self.properties.pollDelay > 0:
                 self.poll(delay=self.properties.pollDelay)
             self.update_history_size(size=self.properties.history_size)
             # self.clear_histories()
-        except NoResponseFromController as error:
+        except NoResponseFromController:
             self._log.error("Cannot retrieve object list, disconnecting...")
             self.segmentation_supported = False
             self.new_state(DeviceDisconnected)
-        except IndexError as error:
+        except IndexError:
             if self._reconnect_on_failure:
                 self._log.error("Device creation failed... re-connecting")
                 self.new_state(DeviceDisconnected)
             else:
                 self._log.error("Device creation failed... disconnecting")
 
     def __getitem__(self, point_name):
@@ -583,15 +583,15 @@
                             if "@prop_" in point_name:
                                 point_name = point_name.split("prop_")[1]
                                 return self.read_property(
                                     ("device", self.properties.device_id, point_name)
                                 )
                             else:
                                 raise ValueError()
-                        except ValueError as ve:
+                        except ValueError:
                             raise ValueError()
         except ValueError as ve:
             self._log.error("{}".format(ve))
 
     def __iter__(self):
         yield from self.points
 
@@ -852,25 +852,32 @@
     """
     [Device state] Initial state of a device. Disconnected from BACnet.
     """
 
     def _init_state(self):
         self.connect()
 
-    def connect(self, *, db=None):
+    def connect(self, *, db=None, network=None):
         """
         Attempt to connect to device.  If unable, attempt to connect to a controller database
         (so the user can use previously saved data).
         """
+        if network:
+            self.properties.network = network
         if not self.properties.network:
             self._log.debug("No network...calling DeviceFromDB")
-            self.new_state(DeviceFromDB)
+            if db:
+                self.new_state(DeviceFromDB)
+            self._log.info(
+                'You can reconnect to network using : "device.connect(network=bacnet)"'
+            )
+
         else:
             try:
-                name = self.properties.network.read(
+                self.properties.network.read(
                     "{} device {} objectName".format(
                         self.properties.address, self.properties.device_id
                     )
                 )
 
                 segmentation = self.properties.network.read(
                     "{} device {} segmentationSupported".format(
```

### Comparing `BAC0-22.9.21/BAC0/core/devices/Points.py` & `BAC0-23.7.3/BAC0/core/devices/Points.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,72 +4,65 @@
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
 Points.py - Definition of points so operations on Read results are more convenient.
 """
 
-# --- standard Python modules ---
-from datetime import datetime, timedelta, timezone
-import pytz
-from collections import namedtuple
 import time
+import typing as t
+from collections import namedtuple
 
-from bacpypes.primitivedata import (
-    CharacterString,
-    Null,
-    Atomic,
-    Integer,
-    Unsigned,
-    Real,
-    Enumerated,
-)
+# --- standard Python modules ---
+from datetime import datetime, timedelta
 
 # --- 3rd party modules ---
+from bacpypes.primitivedata import CharacterString
+
 try:
     import pandas as pd
-    from pandas.io import sql
+    from pandas.io import sql  # noqa E401
 
     try:
         from pandas import Timestamp
     except ImportError:
         from pandas.lib import Timestamp
     _PANDAS = True
 except ImportError:
     _PANDAS = False
 
+from ...tasks.Match import Match, Match_Value
+
 # --- this application's modules ---
 from ...tasks.Poll import SimplePoll as Poll
-from ...tasks.Match import Match, Match_Value
 from ..io.IOExceptions import (
     NoResponseFromController,
-    UnknownPropertyError,
     RemovedPointException,
+    UnknownPropertyError,
     WritePropertyException,
 )
 from ..utils.notes import note_and_log
 
-
 # ------------------------------------------------------------------------------
 
 
 class PointProperties(object):
     """
     A container for point properties.
     """
 
     def __init__(self):
         self.device = None
         self.name = None
-        self.type = None
-        self.address = None
+        self.type = ""
+        self.address = -1
         self.description = None
         self.units_state = None
-        self.simulated = (False, None)
-        self.overridden = (False, None)
+        self.simulated: t.Tuple[bool, t.Optional[int]] = (False, None)
+        self.overridden: t.Tuple[bool, t.Optional[int]] = (False, None)
         self.priority_array = None
         self.history_size = None
         self.bacnet_properties = {}
 
     def __repr__(self):
         return "{}".format(self.asdict)
 
@@ -132,15 +125,17 @@
         self.properties.simulated = (False, 0)
         self.properties.overridden = (False, 0)
 
         self.cov_registered = False
 
         self.tags = tags
 
-        self._cache = {"_previous_read": (None, None)}
+        self._cache: t.Dict[str, t.Tuple[t.Optional[datetime], t.Any]] = {
+            "_previous_read": (None, None)
+        }
 
     @property
     def value(self):
         """
         Retrieve value of the point
         """
         if (
@@ -156,24 +151,24 @@
                     self.properties.device.properties.address,
                     self.properties.type,
                     str(self.properties.address),
                 ),
                 vendor_id=self.properties.device.properties.vendor_id,
             )
             # self._trend(res)
-        except Exception as e:
+        except Exception:
             raise
         self._cache["_previous_read"] = (datetime.now().astimezone(), res)
         return res
 
     def read_priority_array(self):
         """
         Retrieve priority array of the point
         """
-        if self.properties.priority_array != False:
+        if self.properties.priority_array is not False:
             try:
                 res = self.properties.device.properties.network.read(
                     "{} {} {} priorityArray".format(
                         self.properties.device.properties.address,
                         self.properties.type,
                         str(self.properties.address),
                     ),
@@ -230,24 +225,24 @@
         if not self.properties.bacnet_properties:
             self.update_bacnet_properties()
         return self.properties.bacnet_properties
 
     @property
     def is_overridden(self):
         self.read_priority_array()
-        if self.properties.priority_array == False:
+        if self.properties.priority_array is False:
             return False
         if self.priority(8) or self.priority(1):
             self.properties.overridden = (True, self.value)
             return True
         else:
             return False
 
     def priority(self, priority=None):
-        if self.properties.priority_array == False:
+        if self.properties.priority_array is False:
             return None
 
         self.read_priority_array()
         if not priority:
             return self.properties.priority_array.debug_contents()
         if priority < 1 or priority > 16:
             raise IndexError("Please provide priority to read (1-16)")
@@ -259,16 +254,15 @@
                 if key[0] == "null":
                     return None
                 else:
                     return (key[0], value[0])
             except ValueError:
                 return None
 
-    def _trend(self, res):
-        # now = datetime.now(tz=pytz.UTC)
+    def _trend(self, res: float) -> None:
         now = datetime.now().astimezone()
         self._history.timestamp.append(now)
         self._history.value.append(res)
         if self.properties.device.properties.network.database:
             self.properties.device.properties.network.database.write_points_lastvalue_to_db(
                 [self]
             )
@@ -276,22 +270,22 @@
             return
         else:
             if self.properties.history_size < 1:
                 self.properties.history_size = 1
             if len(self._history.timestamp) >= self.properties.history_size:
                 try:
                     self._history.timestamp = self._history.timestamp[
-                        -self.properties.history_size :
+                        -self.properties.history_size :  # noqa E203
                     ]
                     self._history.value = self._history.value[
-                        -self.properties.history_size :
+                        -self.properties.history_size :  # noqa E203
                     ]
                     assert len(self._history.timestamp) == len(self._history.value)
 
-                except Exception as e:
+                except Exception:
                     self._log.exception("Can't append to history")
 
     @property
     def units(self):
         """
         Should return units
         """
@@ -299,30 +293,34 @@
 
     @property
     def lastValue(self):
         """
         returns: last value read
         """
         if _PANDAS:
-            return self.history.dropna().iloc[-1]
+            last_val = self.history.dropna()
+            last_val_clean = None if len(last_val) == 0 else last_val.iloc[-1]
+            return last_val_clean
         else:
             return self._history.value[-1]
 
     @property
     def lastTimestamp(self):
         """
-        returns: last value read
+        returns: last timestamp read
         """
         if _PANDAS:
-            return self.history.dropna().index[-1]
+            last_val = self.history.dropna()
+            last_val_clean = None if len(last_val) == 0 else last_val.index[-1]
+            return last_val_clean
         else:
             return self._history.timestamp[-1]
 
     @property
-    def history(self):
+    def history(self) -> t.Dict[datetime, t.Union[int, float, str]]:
         """
         returns : (pd.Series) containing timestamp and value of all readings
         """
         if not _PANDAS:
             return dict(zip(self._history.timestamp, self._history.value))
         idx = self._history.timestamp.copy()
         his_table = pd.Series(index=idx, data=self._history.value[: len(idx)])
@@ -424,15 +422,15 @@
         The point name is added to the list of simulated points (self.simPoints)
 
         :param value: (float) value to simulate
         """
         if (
             not self.properties.simulated[0]
             or self.properties.simulated[1] != value
-            or force != False
+            or force is not False
         ):
             self.properties.device.properties.network.sim(
                 "{} {} {} presentValue {}".format(
                     self.properties.device.properties.address,
                     self.properties.type,
                     str(self.properties.address),
                     str(value),
@@ -514,23 +512,23 @@
     def _set(self, value):
         """
         Allows the syntax:
             device['point'] = value
         """
         raise NotImplementedError("Must be overridden")
 
-    def poll(self, command="start", *, delay=10):
+    def poll(self, command="start", *, delay: int = 10) -> None:
         """
         Poll a point every x seconds (delay=x sec)
         Stopped by using point.poll('stop') or .poll(0) or .poll(False)
         or by setting a delay = 0
         """
         if (
             str(command).lower() == "stop"
-            or command == False
+            or command is False
             or command == 0
             or delay == 0
         ):
 
             if isinstance(self._polling_task.task, Poll):
                 self._polling_task.task.stop()
                 self._polling_task.task = None
@@ -730,15 +728,20 @@
         except ValueError:
             self._log.error(
                 "Cannot convert value {}. Device probably disconnected or the response is inconsistent".format(
                     self.value
                 )
             )
             # Probably disconnected
-            val = None
+            return "{}/{} : (n/a) {}".format(
+                self.properties.device.properties.name,
+                self.properties.name,
+                self.properties.units_state,
+            )
+
         return "{}/{} : {:.2f} {}".format(
             self.properties.device.properties.name,
             self.properties.name,
             val,
             self.properties.units_state,
         )
 
@@ -854,17 +857,17 @@
         """
         Boolean points don't have units
         """
         return None
 
     def _set(self, value):
         try:
-            if value == True:
+            if value is True:
                 self._setitem("active")
-            elif value == False:
+            elif value is False:
                 self._setitem("inactive")
             elif str(value) in ["inactive", "active"] or str(value).lower() == "auto":
                 self._setitem(value)
             else:
                 raise ValueError(
                     'Value must be boolean True, False or "active"/"inactive"'
                 )
@@ -935,15 +938,16 @@
         # self._log.info("Value : {}".format(res))
         # self._log.info("EnumValue : {}".format(self.get_state(res)))
         self._trend(res)
         return res
 
     def get_state(self, v):
         try:
-            return self.properties.units_state[v - 1]
+            # errors caught below
+            return self.properties.units_state[v - 1]  # type: ignore[index]
         except (TypeError, IndexError):
             return "n/a"
 
     @property
     def enumValue(self):
         """
         returns: (str) Enum state value
@@ -968,15 +972,15 @@
         """
         return None
 
     def _set(self, value):
         try:
             if isinstance(value, int):
                 self._setitem(value)
-            elif str(value) in self.properties.units_state:
+            elif str(value) in self.properties.units_state:  # type: ignore[operator]
                 self._setitem(self.properties.units_state.index(value) + 1)
             elif str(value).lower() == "auto":
                 self._setitem("auto")
             else:
                 raise ValueError(
                     "Value must be integer or correct enum state : {}".format(
                         self.properties.units_state
@@ -1183,16 +1187,16 @@
 
         self.properties.name = props["name"]
         self.properties.type = props["type"]
         self.properties.address = props["address"]
 
         self.properties.description = props["description"]
         self.properties.units_state = props["units_state"]
-        self.properties.simulated = "Offline"
-        self.properties.overridden = "Offline"
+        self.properties.simulated = (True, None)
+        self.properties.overridden = (False, None)
 
         if "analog" in self.properties.type:
             self.new_state(NumericPointOffline)
         elif "multi" in self.properties.type:
             self.new_state(EnumPointOffline)
         elif "binary" in self.properties.type:
             self.new_state(BooleanPointOffline)
@@ -1307,15 +1311,15 @@
 
     @property
     def enumValue(self):
         """
         returns: (str) Enum state value
         """
         try:
-            value = self.properties.units_state[int(self.lastValue) - 1]
+            value = self.properties.units_state[int(self.lastValue) - 1]  # type: ignore[index]
         except IndexError:
             value = "unknown"
         except ValueError:
             value = "NaN"
         return value
 
     def _set(self, value):
```

### Comparing `BAC0-22.9.21/BAC0/core/devices/Trends.py` & `BAC0-23.7.3/BAC0/core/devices/Trends.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,33 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
-"""
-Points.py - Definition of points so operations on Read results are more convenient.
-"""
 
 # --- standard Python modules ---
-from datetime import datetime
-from collections import namedtuple
-import time
-from itertools import islice
-
-
 # --- 3rd party modules ---
 try:
     import pandas as pd
-    from pandas.io import sql
 
-    try:
-        from pandas import Timestamp
-    except ImportError:
-        from pandas.lib import Timestamp
     _PANDAS = True
 except ImportError:
     _PANDAS = False
 
-from bacpypes.object import TrendLogObject
 from bacpypes.primitivedata import Date, Time
+from collections import namedtuple
 
 # --- this application's modules ---
-from ...tasks.Poll import SimplePoll as Poll
-from ...tasks.Match import Match, Match_Value
-from ..io.IOExceptions import NoResponseFromController, UnknownPropertyError
 from ..utils.notes import note_and_log
 
-
 # ------------------------------------------------------------------------------
 
+HistoryComponent = namedtuple("HistoryComponent", "index logdatum status choice")
+
 
 class TrendLogProperties(object):
     """
     A container for trend properties
     """
 
     def __init__(self):
@@ -52,23 +36,22 @@
         self.object_name = None
         self.description = ""
         self.log_device_object_property = None
         self.buffer_size = 0
         self.record_count = 0
         self.total_record_count = 0
         self.log_interval = 0
-        self.description = None
         self.statusFlags = None
         self.status_flags = {
             "in_alarm": False,
             "fault": False,
             "overridden": False,
             "out_of_service": False,
         }
-        self._history_components = {"index": [], "logdatum": [], "status": []}
+        self._history_components = []
         self._df = None
         self.type = "TrendLog"
         self.units_state = "None"
 
     def __repr__(self):
         return "{} | Descr : {} | Record count : {}".format(
             self.object_name, self.description, self.record_count
@@ -93,27 +76,34 @@
         self.properties.oid = OID
         self.update_properties()
 
         if read_log_on_creation:
             self.read_log_buffer()
         self._last_index = 0
 
+    @staticmethod
+    def read_logDatum(logDatum):
+        for k, v in logDatum.__dict__.items():
+            if v is None:
+                continue
+            else:
+                return (k, v)
+
     def update_properties(self):
         try:
             (
                 self.properties.object_name,
                 self.properties.description,
                 self.properties.record_count,
                 self.properties.buffer_size,
                 self.properties.total_record_count,
-                self.properties.log_device_object_property,
                 self.properties.statusFlags,
                 self.properties.log_interval,
             ) = self.properties.device.properties.network.readMultiple(
-                "{addr} trendLog {oid} objectName description recordCount bufferSize totalRecordCount logDeviceObjectProperty statusFlags logInterval".format(
+                "{addr} trendLog {oid} objectName description recordCount bufferSize totalRecordCount statusFlags logInterval".format(
                     addr=self.properties.device.properties.address,
                     oid=str(self.properties.oid),
                 )
             )
         except Exception as error:
             raise Exception("Problem reading trendLog informations: {}".format(error))
 
@@ -128,17 +118,17 @@
         )
         return self.properties.total_record_count
 
     def read_log_buffer(self):
         RECORDS = 10
         log_buffer = set()
         _actual_index = self._total_record_count()
-        start = max(_actual_index - self.properties.record_count, self._last_index) + 1
-        _count = _actual_index - start
-        steps = int(_count / 10) + int(_count % 10)
+        start = max(_actual_index - self.properties.record_count, self._last_index)
+        _count = max(_actual_index - start, 0)
+        steps = int(_count / RECORDS) + int(1 if (_count % RECORDS) > 0 else 0)
 
         self._log.debug("Reading log : {} {} {}".format(start, _count, steps))
 
         _from = start
         for each in range(steps):
             range_params = ("s", _from, Date("1979-01-01"), Time("00:00"), RECORDS)
             _chunk = self.properties.device.properties.network.readRange(
@@ -155,82 +145,105 @@
         self.create_dataframe(log_buffer)
 
     def create_dataframe(self, log_buffer):
         for each in log_buffer:
             year, month, day, dow = each.timestamp.date
             year = year + 1900
             hours, minutes, seconds, ms = each.timestamp.time
-            self.properties._history_components["index"].append(
-                pd.to_datetime(
-                    "{}-{}-{} {}:{}:{}.{}".format(
-                        year, month, day, hours, minutes, seconds, ms
-                    ),
-                    format="%Y-%m-%d %H:%M:%S.%f",
-                )
-            )
-            self.properties._history_components["logdatum"].append(
-                each.logDatum.dict_contents()
+            seconds = 0 if seconds == 255 else seconds
+            ms = 0 if ms == 255 else ms
+            _index = pd.to_datetime(
+                "{}-{}-{} {}:{}:{}.{}".format(
+                    year, month, day, hours, minutes, seconds, ms
+                ),
+                format="%Y-%m-%d %H:%M:%S.%f",
             )
-            self.properties._history_components["status"].append(each.statusFlags)
+            _choice, _logDatum = self.read_logDatum(each.logDatum)
+            _status = each.statusFlags
+            print(_index, _logDatum, _status, _choice)
+            his_component = HistoryComponent(_index, _logDatum, _status, _choice)
+            if his_component not in self.properties._history_components:
+                self.properties._history_components.append(his_component)
 
         if _PANDAS:
             df = pd.DataFrame(
                 {
-                    "index": self.properties._history_components["index"],
-                    "logdatum": self.properties._history_components["logdatum"],
-                    "status": self.properties._history_components["status"],
+                    "index": [
+                        each.index for each in self.properties._history_components
+                    ],
+                    self.properties.object_name: [
+                        each.logdatum for each in self.properties._history_components
+                    ],
+                    "status": [
+                        each.status for each in self.properties._history_components
+                    ],
+                    "choice": [
+                        each.choice for each in self.properties._history_components
+                    ],
                 }
             )
             df = df.set_index("index")
-            df["choice"] = df["logdatum"].apply(lambda x: list(x.keys())[0])
-            df[self.properties.object_name] = df["logdatum"].apply(
-                lambda x: list(x.values())[0]
-            )
+            # df["choice"] = _choice
+            # df[self.properties.object_name] = df['logDatum']
 
             self.properties._df = df
         else:
             # self.properties._history_components = (self.index, self.logdatum, self.status)
             self._log.warning(
                 "Pandas not installed. Treating histories as simple list."
             )
 
     @property
     def history(self):
         self.read_log_buffer()
-        if not _PANDAS:
+
+        if not _PANDAS or self.properties._df is None:
             return dict(
                 zip(
-                    self.properties._history_components["index"],
-                    self.properties._history_components["logdatum"],
+                    [each.index for each in self.properties._history_components],
+                    [each.logDatum for each in self.properties._history_components],
                 )
             )
-        (
-            objectType,
-            objectAddress,
-        ) = self.properties.log_device_object_property.objectIdentifier
+
         try:
+            if not self.properties.log_device_object_property:
+                self.properties.log_device_object_property = (
+                    self.properties.device.properties.network.read(
+                        "{addr} trendLog {oid} logDeviceObjectProperty".format(
+                            addr=self.properties.device.properties.address,
+                            oid=str(self.properties.oid),
+                        )
+                    )
+                )
+            (
+                objectType,
+                objectAddress,
+            ) = self.properties.log_device_object_property.objectIdentifier
             logged_point = self.properties.device.find_point(objectType, objectAddress)
-        except ValueError:
+        except (Exception, ValueError):
             logged_point = None
+
         serie = self.properties._df[self.properties.object_name].copy()
         serie.units = logged_point.properties.units_state if logged_point else "n/a"
         serie.name = ("{}/{}").format(
             self.properties.device.properties.name, self.properties.object_name
         )
         if not logged_point:
             serie.states = "unknown"
+            serie.datatype = None
         else:
             if logged_point.properties.name in self.properties.device.binary_states:
                 serie.states = "binary"
             elif logged_point.properties.name in self.properties.device.multi_states:
                 serie.states = "multistates"
             else:
                 serie.states = "analog"
+            serie.datatype = objectType
         serie.description = self.properties.description
-        serie.datatype = objectType
+
         return serie.sort_index()
 
     def chart(self, remove=False):
         """
         Add point to the bacnet trending list
         """
         if not _PANDAS:
```

### Comparing `BAC0-22.9.21/BAC0/core/devices/Virtuals.py` & `BAC0-23.7.3/BAC0/core/devices/Virtuals.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,41 +4,39 @@
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
 Points.py - Definition of points so operations on Read results are more convenient.
 """
 
+import time
+from collections import namedtuple
+
 # --- standard Python modules ---
 from datetime import datetime
-from collections import namedtuple
-import time
 
 # --- 3rd party modules ---
 try:
     import pandas as pd
     from pandas.io import sql
 
     try:
         from pandas import Timestamp
     except ImportError:
         from pandas.lib import Timestamp
     _PANDAS = True
 except ImportError:
     _PANDAS = False
 
-from bacpypes.object import TrendLogObject
+
+from ...tasks.Match import Match_Value
 
 # --- this application's modules ---
-from ...tasks.Poll import SimplePoll as Poll
-from ...tasks.Match import Match, Match_Value
-from ..io.IOExceptions import NoResponseFromController, UnknownPropertyError
 from ..utils.notes import note_and_log
 
-
 # ------------------------------------------------------------------------------
 
 
 class VirtualDeviceProperties(object):
     """
     This serves as a container for device properties
     """
@@ -156,15 +154,15 @@
                     self._history.timestamp = self._history.timestamp[
                         -self.properties.history_size :
                     ]
                     self._history.value = self._history.value[
                         -self.properties.history_size :
                     ]
                     assert len(self._history.timestamp) == len(self._history.value)
-                except Exception as e:
+                except Exception:
                     self._log.exception("Can't append to history")
 
     @property
     def value(self):
         """
         Retrieve value of the point
         """
```

### Comparing `BAC0-22.9.21/BAC0/core/devices/create_objects.py` & `BAC0-23.7.3/BAC0/core/devices/create_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,24 @@
+from bacpypes.basetypes import DateTime, PriorityArray, StatusFlags
+from bacpypes.constructeddata import ArrayOf
 from bacpypes.object import (
-    MultiStateValueObject,
-    AnalogValueObject,
-    BinaryValueObject,
     AnalogInputObject,
-    BinaryInputObject,
     AnalogOutputObject,
-    BinaryOutputObject,
+    AnalogValueObject,
+    BinaryInputObject,
+    BinaryValueObject,
     CharacterStringValueObject,
     DateTimeValueObject,
-    Property,
-    register_object_type,
-)
-
-from bacpypes.local.object import (
-    AnalogOutputCmdObject,
-    AnalogValueCmdObject,
-    BinaryOutputCmdObject,
-    BinaryValueCmdObject,
+    MultiStateValueObject,
 )
-
-from bacpypes.primitivedata import CharacterString, Date, Time, Real, Boolean
-from bacpypes.constructeddata import ArrayOf
-from bacpypes.basetypes import EngineeringUnits, DateTime, PriorityArray, StatusFlags
+from bacpypes.primitivedata import Boolean, CharacterString, Date, Time
 
 from .mixins.CommandableMixin import LocalBinaryOutputObjectCmd
 
-
+# THIS IS DEPRECATED
 def _make_mutable(obj, identifier="presentValue", mutable=True):
     """
     This function is not the way to go as it changes the class
     property...As bacpypes issue #224, it will need a lot of work
     """
     for prop in obj.properties:
         if prop.identifier == identifier:
```

### Comparing `BAC0-22.9.21/BAC0/core/devices/local/decorator.py` & `BAC0-23.7.3/BAC0/core/devices/local/decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-from functools import wraps, partial
+from functools import wraps
 
+from bacpypes.basetypes import EngineeringUnits
+from bacpypes.local.object import Commandable
 from bacpypes.object import (
-    AnalogInputObject,
-    AnalogValueObject,
-    BinaryValueObject,
     Property,
+    TrendLogObject,
     register_object_type,
-    registered_object_types,
-    DatePatternValueObject,
 )
-from bacpypes.primitivedata import CharacterString, Date, Time, Real, Boolean, Integer
-from bacpypes.basetypes import EngineeringUnits, BinaryPV, Polarity
-from bacpypes.local.object import AnalogValueCmdObject, Commandable, MinOnOff
+from bacpypes.primitivedata import CharacterString
 
 _SHOULD_BE_COMMANDABLE = ["relinquishDefault", "outOfService", "lowLimit", "highLimit"]
 
 """
 Template
 
 Decorators is an effort to handle object creation without explicitly declare a new class
@@ -220,15 +216,23 @@
             return obj
 
         return wrapper
 
     return decorate
 
 
-def create(object_type, instance, objectName, presentValue, description):
-    new_object = object_type(
-        objectIdentifier=(object_type.objectType, instance),
-        objectName="{}".format(objectName),
-        presentValue=presentValue,
-        description=CharacterString("{}".format(description)),
-    )
+def create(object_type, instance, objectName, value, description):
+    if object_type is TrendLogObject:
+        new_object = object_type(
+            objectIdentifier=(object_type.objectType, instance),
+            objectName="{}".format(objectName),
+            logBuffer=value,
+            description=CharacterString("{}".format(description)),
+        )
+    else:
+        new_object = object_type(
+            objectIdentifier=(object_type.objectType, instance),
+            objectName="{}".format(objectName),
+            presentValue=value,
+            description=CharacterString("{}".format(description)),
+        )
     return new_object
```

### Comparing `BAC0-22.9.21/BAC0/core/devices/local/models.py` & `BAC0-23.7.3/BAC0/core/devices/local/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from bacpypes.basetypes import (
+    Boolean,
+    Date,
+    DateTime,
+    EventState,
+    LogRecord,
+    Polarity,
+    Time,
+    Unsigned,
+)
+from bacpypes.constructeddata import ArrayOf, ListOf
 from bacpypes.object import (
-    AnalogValueObject,
-    CharacterStringValueObject,
     AnalogInputObject,
     AnalogOutputObject,
+    AnalogValueObject,
     BinaryInputObject,
     BinaryOutputObject,
     BinaryValueObject,
-    DateValueObject,
+    CharacterStringValueObject,
     DateTimeValueObject,
+    DateValueObject,
     MultiStateInputObject,
     MultiStateOutputObject,
     MultiStateValueObject,
+    TrendLogObject,
 )
-from bacpypes.basetypes import (
-    EngineeringUnits,
-    BinaryPV,
-    Polarity,
-    Boolean,
-    EventState,
-    Date,
-    Time,
-    DateTime,
-    Unsigned,
-)
-from bacpypes.constructeddata import ArrayOf
-from bacpypes.primitivedata import CharacterString, Real
+from bacpypes.primitivedata import CharacterString
+
 from .object import ObjectFactory
 
 """
 Those models are opiniated versions of BACnet objects.
 They are meant to supply an easy mechanism to build BACnet objects
 that will be served by the local device of BAC0.
 
@@ -47,16 +48,17 @@
         "is_commandable": False,
         "relinquish_default": None,
     }
     _definition.update(definition)
     for k, v in kwargs.items():
         if k == "properties":
             for _k, _v in v.items():
-                _definition[k][_k] = _v
-        _definition[k] = v
+                _definition["properties"][_k] = _v  # type: ignore[index]
+        else:
+            _definition[k] = v
     return ObjectFactory.from_dict(_definition)
 
 
 def make_state_text(list_of_string):
     _arr = ArrayOf(CharacterString)
     _lst = [CharacterString(each) for each in list_of_string]
     return _arr(_lst)
@@ -259,7 +261,25 @@
         "description": "No description",
         "presentValue": DateTime(date=Date().now().value, time=Time().now().value),
         "properties": {},
         "is_commandable": False,
         "relinquish_default": "inactive",
     }
     return _create(definition, **kwargs)
+
+
+def trendlog(**kwargs):
+    definition = {
+        "name": "TREND_LOG",
+        "objectType": TrendLogObject,
+        "instance": 0,
+        "description": "No description",
+        "properties": {
+            "enable": True,
+            "logBuffer": ListOf(LogRecord),
+            # "logDeviceObjectProperty": DeviceObjectPropertyReference(
+            #    objectIdentifier=ObjectIdentifier("trendLog", 0),
+            # ),
+            "trendLog_datatype": "realValue",
+        },
+    }
+    return _create(definition, **kwargs)
```

### Comparing `BAC0-22.9.21/BAC0/core/devices/local/object.py` & `BAC0-23.7.3/BAC0/core/devices/local/object.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,24 @@
-from .decorator import bacnet_properties, make_commandable, create
+import typing as t
+from collections import namedtuple
+
+from bacpypes.basetypes import PriorityArray, Reliability
+from bacpypes.object import TrendLogObject
+from colorama import Fore
+
+from BAC0.core.devices.local.trendLogs import LocalTrendLog
 
-from ...utils.notes import note_and_log
 from ....scripts.Base import Base
 from ...app.ScriptApplication import (
     BAC0Application,
     BAC0BBMDDeviceApplication,
     BAC0ForeignDeviceApplication,
 )
-
-from bacpypes.object import (
-    AnalogInputObject,
-    AnalogValueObject,
-    BinaryValueObject,
-    Property,
-    register_object_type,
-    registered_object_types,
-    DatePatternValueObject,
-    ReadableProperty,
-    WritableProperty,
-    OptionalProperty,
-)
-from bacpypes.basetypes import (
-    EngineeringUnits,
-    DateTime,
-    PriorityArray,
-    StatusFlags,
-    Reliability,
-    Polarity,
-)
-
-from collections import namedtuple
-from colorama import Fore, Back, Style
+from ...utils.notes import note_and_log
+from .decorator import bacnet_properties, create, make_commandable
 
 
 @note_and_log
 class ObjectFactory(object):
     """
     This is an exploration of a method to create local objects in BAC0 instance.
 
@@ -51,46 +35,51 @@
     Then you can use the factory to create your object
     ex. :
 
         av0 = ObjectFactory(AnalogValueObject, 1, 'av0', )
 
     """
 
-    instances = {}
+    instances: t.Dict[str, t.Set] = {}
 
-    definition = namedtuple(
+    definition = namedtuple(  # type: ignore[name-match]
         "Definition",
         "name, objectType, instance, properties, description, presentValue, is_commandable, relinquish_default",
     )
 
-    objects = {}
+    objects: t.Dict[str, t.Any] = {}
     # In the future... should think about a way to store relinquish default values because on a restart
     # those should be restored.
 
     def __init__(
         self,
         objectType,
         instance,
         objectName,
         properties=None,
         description="",
         presentValue=None,
         is_commandable=False,
         relinquish_default=None,
     ):
+        _localTrendLogDataType = properties.pop("trendLog_datatype", None)
         self._properties = ObjectFactory.default_properties(
             objectType, properties, is_commandable, relinquish_default
         )
-        pv_datatype = ObjectFactory.get_pv_datatype(objectType)
-
-        if not isinstance(presentValue, pv_datatype):
-            try:
-                presentValue = pv_datatype(presentValue)
-            except:
-                raise ValueError("Wrong datatype provided for presentValue")
+        print(f"Obj {objectType} of type {type(objectType)}")
+        if objectType is not TrendLogObject:
+            pv_datatype = ObjectFactory.get_pv_datatype(objectType)
+
+            if not isinstance(presentValue, pv_datatype):
+                try:
+                    presentValue = pv_datatype(presentValue)
+                except:
+                    raise ValueError(
+                        f"Wrong datatype provided for presentValue for {objectType} of type {type(objectType)}"
+                    )
 
         @bacnet_properties(self._properties)
         @make_commandable()
         def _create_commandable(
             objectType, instance, objectName, presentValue, description
         ):
             return create(objectType, instance, objectName, presentValue, description)
@@ -107,14 +96,18 @@
             self.objects[objectName] = _create_commandable(
                 objectType, instance, objectName, presentValue, description
             )
         else:
             self.objects[objectName] = _create(
                 objectType, instance, objectName, presentValue, description
             )
+        if objectType is TrendLogObject:
+            self.objects[objectName]._local = LocalTrendLog(
+                self.objects[objectName], datatype=_localTrendLogDataType
+            )  # this will need to be fed by another process.
 
     def validate_instance(self, objectType, instance):
         _warning = True
         try:
             _set = self.instances[objectType.__name__]
         except KeyError:
             _set = set()
```

### Comparing `BAC0-22.9.21/BAC0/core/devices/mixins/CommandableMixin.py` & `BAC0-23.7.3/BAC0/core/devices/mixins/CommandableMixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,71 +1,65 @@
 #!/usr/bin/env python
+# type: ignore
 
 """
 Rebuilt Commandable
 """
 
-from bacpypes.debugging import bacpypes_debugging, ModuleLogger
-from bacpypes.consolelogging import ConfigArgumentParser
-
-from bacpypes.core import run
-from bacpypes.task import OneShotTask
-from bacpypes.errors import ExecutionError
-
-from bacpypes.primitivedata import (
-    BitString,
-    CharacterString,
-    Date,
-    Integer,
-    Double,
-    Enumerated,
-    OctetString,
-    Real,
-    Time,
-    Unsigned,
-)
 from bacpypes.basetypes import (
     BinaryPV,
     ChannelValue,
     DateTime,
     DoorValue,
-    PriorityValue,
     PriorityArray,
+    PriorityValue,
 )
+from bacpypes.debugging import ModuleLogger, bacpypes_debugging
+from bacpypes.errors import ExecutionError
+from bacpypes.local.object import CurrentPropertyListMixIn
 from bacpypes.object import (
-    Property,
-    ReadableProperty,
-    WritableProperty,
-    register_object_type,
     AccessDoorObject,
     AnalogOutputObject,
     AnalogValueObject,
     BinaryOutputObject,
     BinaryValueObject,
     BitStringValueObject,
+    ChannelObject,
     CharacterStringValueObject,
-    DateValueObject,
     DatePatternValueObject,
     DateTimePatternValueObject,
     DateTimeValueObject,
+    DateValueObject,
     IntegerValueObject,
     LargeAnalogValueObject,
     LightingOutputObject,
     MultiStateOutputObject,
     MultiStateValueObject,
     OctetStringValueObject,
     PositiveIntegerValueObject,
-    TimeValueObject,
+    Property,
+    ReadableProperty,
     TimePatternValueObject,
-    ChannelObject,
+    TimeValueObject,
+    WritableProperty,
+    register_object_type,
 )
-
-from bacpypes.app import BIPSimpleApplication
-from bacpypes.local.object import CurrentPropertyListMixIn
-from bacpypes.local.device import LocalDeviceObject
+from bacpypes.primitivedata import (
+    BitString,
+    CharacterString,
+    Date,
+    Double,
+    Enumerated,
+    Integer,
+    OctetString,
+    Real,
+    Time,
+    Unsigned,
+)
+from bacpypes.task import OneShotTask
 
 # some debugging
 _debug = 0
 _log = ModuleLogger(globals())
 
 
 #
```

### Comparing `BAC0-22.9.21/BAC0/core/devices/mixins/read_mixin.py` & `BAC0-23.7.3/BAC0/core/devices/mixins/read_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,35 +4,29 @@
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
 read_mixin.py - Add ReadProperty and ReadPropertyMultiple to a device
 """
 # --- standard Python modules ---
-
-# --- 3rd party modules ---
+import typing as t
 
 # --- this application's modules ---
-from ....tasks.Poll import DeviceNormalPoll, DeviceFastPoll
+from ....tasks.Poll import DeviceFastPoll, DeviceNormalPoll
 from ...io.IOExceptions import (
-    ReadPropertyMultipleException,
+    BufferOverflow,
     NoResponseFromController,
     SegmentationNotSupported,
-    BufferOverflow,
-)
-from ..Points import (
-    NumericPoint,
-    BooleanPoint,
-    EnumPoint,
-    StringPoint,
-    OfflinePoint,
-    DateTimePoint,
 )
+from ..Points import BooleanPoint, DateTimePoint, EnumPoint, NumericPoint, StringPoint
 from ..Trends import TrendLog
 
+# --- 3rd party modules ---
+
+
 # from ...functions.Schedule import Schedule
 
 # ------------------------------------------------------------------------------
 
 # Requests processing
 def retrieve_type(obj_list, point_type_key):
     for point_type, point_address in obj_list:
@@ -66,20 +60,23 @@
 def create_trendlogs(objList, device):
     trendlogs = {}
     for each in retrieve_type(objList, "trendLog"):
         point_address = str(each[1])
         try:
             tl = TrendLog(point_address, device, read_log_on_creation=False)
             if tl.properties.log_device_object_property is None:
-                raise TrendLogCreationException
-            (
-                ldop_type,
-                ldop_addr,
-            ) = tl.properties.log_device_object_property.objectIdentifier
-            ldop_prop = tl.properties.log_device_object_property.propertyIdentifier
+                ldop_type = "trendLog"
+                ldop_addr = point_address
+                ldop_prop = "log"
+            else:
+                (
+                    ldop_type,
+                    ldop_addr,
+                ) = tl.properties.log_device_object_property.objectIdentifier
+                ldop_prop = tl.properties.log_device_object_property.propertyIdentifier
             trendlogs["{}_{}_{}".format(ldop_type, ldop_addr, ldop_prop)] = (
                 tl.properties.object_name,
                 tl,
             )
         except TrendLogCreationException:
             device._log.error("Problem creating {}".format(each))
             continue
@@ -247,15 +244,15 @@
                 values.append(points_info)
 
         return values
 
 
 class RPMObjectsProcessing:
     def _process_new_objects(
-        self, obj_cls=None, obj_type=None, objList=None, points_per_request=5
+        self, obj_cls=None, obj_type: str = "", objList=None, points_per_request=5
     ):
         """
         Template to generate BAC0 points instances from information coming from the network.
         """
         request = []
         new_points = []
         if obj_type == "analog":
@@ -298,15 +295,15 @@
             point_type = str(each[0])
             point_address = str(each[1])
             point_infos = points_info[i]
             i += 1
 
             pointName = point_infos[_find_propid_index("objectName")]
             presentValue = point_infos[_find_propid_index("presentValue")]
-            if presentValue != None:
+            if presentValue is not None:
                 if obj_type == "analog" or obj_type == "loop":
                     presentValue = float(presentValue)
                 elif obj_type == "multi":
                     presentValue = int(presentValue)
             try:
                 point_description = point_infos[_find_propid_index("description")]
             except KeyError:
@@ -350,15 +347,15 @@
                 )
                 raise
         return new_points
 
 
 class RPObjectsProcessing:
     def _process_new_objects(
-        self, obj_cls=NumericPoint, obj_type="analog", objList=None
+        self, obj_cls=NumericPoint, obj_type: str = "analog", objList=None
     ):
         _newpoints = []
         for each in retrieve_type(objList, obj_type):
             point_type = str(each[0])
             point_address = str(each[1])
 
             if obj_type == "analog":
@@ -463,22 +460,22 @@
                             val = self.properties.network.readMultiple(
                                 request, vendor_id=self.properties.vendor_id
                             )
                         except SegmentationNotSupported:
                             raise
 
                         # print('val : ', val, len(val), type(val))
-                        if val == None:
+                        if val is None:
                             self.properties.segmentation_supported = False
                             raise SegmentationNotSupported
 
                     except KeyError as error:
                         raise Exception("Unknown point name : {}".format(error))
 
-                    except SegmentationNotSupported as error:
+                    except SegmentationNotSupported:
                         self.properties.segmentation_supported = False
                         # self.read_multiple(points_list,points_per_request=1, discover_request=discover_request)
                         self._log.warning("Segmentation not supported")
                         self._log.warning("Request too big...will reduce it")
                         if points_per_request == 1:
                             raise
                         self.read_multiple(
@@ -502,15 +499,15 @@
                             self.properties.address, "".join(request)
                         )
                         self._log.debug(request)
                         val = self.properties.network.readMultiple(
                             request, vendor_id=self.properties.vendor_id
                         )
 
-                    except SegmentationNotSupported as error:
+                    except SegmentationNotSupported:
                         self.properties.segmentation_supported = False
                         self.read_multiple(
                             points_list,
                             points_per_request=1,
                             discover_request=discover_request,
                         )
 
@@ -561,14 +558,15 @@
 
         :Example:
 
         device.poll()
         device.poll('stop')
         device.poll(delay = 5)
         """
+        _poll_cls: t.Union[t.Type[DeviceFastPoll], t.Type[DeviceNormalPoll]]
         if delay < 10:
             self.properties.fast_polling = True
             _poll_cls = DeviceFastPoll
         else:
             self.properties.fast_polling = False
             _poll_cls = DeviceNormalPoll
 
@@ -576,15 +574,15 @@
             self._log.error(
                 'Bad argument for function. Needs "stop", "start", "0" or "False" or provide keyword arg (command or delay)'
             )
             return
 
         if (
             str(command).lower() == "stop"
-            or command == False
+            or command == False  # noqa E712
             or command == 0
             or delay == 0
         ):
 
             if isinstance(self._polling_task.task, DeviceNormalPoll) or isinstance(
                 self._polling_task.task, DeviceFastPoll
             ):
@@ -662,15 +660,15 @@
             self._log.debug("RP_Request: %s " % request)
             return self.properties.network.read(
                 request, vendor_id=self.properties.vendor_id
             )
         except KeyError as error:
             raise Exception("Unknown point name: {}".format(error))
 
-        except NoResponseFromController as error:
+        except NoResponseFromController:
             return ""
 
     def poll(self, command="start", *, delay=120):
         """
         Poll a point every x seconds (delay=x sec)
         Can be stopped by using point.poll('stop') or .poll(0) or .poll(False)
         or by setting a delay = 0
@@ -691,15 +689,15 @@
                 "Device do not support RPM, fast polling not available, limiting delay to 10sec."
             )
             self.properties.fast_polling = False
             delay = 10
 
         if (
             str(command).lower() == "stop"
-            or command == False
+            or command is False
             or command == 0
             or delay == 0
         ):
 
             if isinstance(self._polling_task.task, DeviceNormalPoll):
                 self._polling_task.task.stop()
                 while self._polling_task.task.is_alive():
```

### Comparing `BAC0-22.9.21/BAC0/core/functions/Calendar.py` & `BAC0-23.7.3/BAC0/core/functions/Calendar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,29 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
-"""
-ScheduleWrite.py - creation of ReinitializeDeviceRequest
-
-"""
-from ..io.Read import find_reason
-from ..io.IOExceptions import NoResponseFromController
-from ...core.utils.notes import note_and_log
-
 # --- standard Python modules ---
-import datetime as dt
+import datetime
+import typing as t
 
-# --- 3rd party modules ---
-from bacpypes.pdu import Address, GlobalBroadcast
-from bacpypes.primitivedata import Integer, Date, Time, CharacterString
-from bacpypes.basetypes import DateTime
-from bacpypes.apdu import WritePropertyRequest, SimpleAckPDU
-from bacpypes.iocb import IOCB
+from bacpypes.apdu import SimpleAckPDU, WritePropertyRequest
+from bacpypes.basetypes import CalendarEntry, DateRange
+from bacpypes.constructeddata import Any, ArrayOf
 from bacpypes.core import deferred
-from bacpypes.basetypes import (
-    DateTime,
-    DailySchedule,
-    TimeValue,
-    Time,
-    CalendarEntry,
-    DateRange,
-)
-from bacpypes.constructeddata import ArrayOf, Any
-from BAC0.core.io.IOExceptions import NoResponseFromController, WritePropertyException
+from bacpypes.iocb import IOCB
 
-from bacpypes.primitivedata import Null, Atomic, Integer, Unsigned, Real, Enumerated
+# --- 3rd party modules ---
+from bacpypes.pdu import Address
 
-from datetime import time as dt_time
-from datetime import datetime as dt
+from ...core.utils.notes import note_and_log
+from ..io.IOExceptions import NoResponseFromController
+from ..io.Read import find_reason
 
 
 @note_and_log
 class Calendar:
     """
     Everything you need to write dates and date ranges to a calendar object.
     """
@@ -66,34 +49,34 @@
         entries = []
         if "dates" in dict_calendar.keys():
             for date_entry in dict_calendar["dates"]:
                 year, month, day = (int(x) for x in date_entry["date"].split("/"))
                 if date_entry["recurring"]:
                     weekday = 255
                 else:
-                    weekday = dt.date(year, month, day).weekday() + 1
+                    weekday = datetime.date(year, month, day).weekday() + 1
                     if weekday > 7:
                         weekday = 1
                 _date = (year - 1900, month, day, weekday)
                 entries.append(CalendarEntry(date=_date))
 
         if "dateRanges" in dict_calendar.keys():
             for date_range_entry in dict_calendar["dateRanges"]:
                 year, month, day = (
                     int(x) for x in date_range_entry["startDate"].split("/")
                 )
-                weekday = dt.date(year, month, day).weekday() + 1
+                weekday = datetime.date(year, month, day).weekday() + 1
                 if weekday > 7:
                     weekday = 1
                 start_date = (year - 1900, month, day, weekday)
 
                 year, month, day = (
                     int(x) for x in date_range_entry["endDate"].split("/")
                 )
-                weekday = dt.date(year, month, day).weekday() + 1
+                weekday = datetime.date(year, month, day).weekday() + 1
                 if weekday > 7:
                     weekday = 1
                 end_date = (year - 1900, month, day, weekday)
 
                 date_range = DateRange(startDate=start_date, endDate=end_date)
                 entries.append(CalendarEntry(dateRange=date_range))
 
@@ -120,17 +103,15 @@
         iocb.wait()  # Wait for BACnet response
 
         if iocb.ioResponse:  # successful response
             apdu = iocb.ioResponse
 
             if not isinstance(apdu, SimpleAckPDU):  # expect an ACK
                 self._log.warning("Not an ack, see debug for more infos.")
-                self._log.debug(
-                    "Not an ack. | APDU : {} / {}".format((apdu, type(apdu)))
-                )
+                self._log.debug("Not an ack. | APDU : {} / {}".format(apdu, type(apdu)))
                 return
 
         if iocb.ioError:  # unsuccessful: error/reject/abort
             apdu = iocb.ioError
             reason = find_reason(apdu)
             raise NoResponseFromController("APDU Abort Reason : {}".format(reason))
 
@@ -160,18 +141,18 @@
             dict_calendar = self.decode_dateList(dateList_object)
         except Exception as error:
             self._log.error("exception: {!r}".format(error))
             return {}
 
         return dict_calendar
 
-    def decode_dateList(self, dateList_object):
+    def decode_dateList(self, dateList_object) -> t.Dict[str, t.List[t.Dict]]:
         dict_calendar = {"dates": [], "dateRanges": []}
         for entry in dateList_object:
-            entry_dict = {}
+            entry_dict: t.Dict[str, t.Union[str, bool]] = {}
             if entry.date:
                 if entry.date[3] == 255:
                     recurring = True
                 else:
                     recurring = False
                 entry_dict["date"] = "{}/{}/{}".format(
                     entry.date[0] + 1900, entry.date[1], entry.date[2]
```

### Comparing `BAC0-22.9.21/BAC0/core/functions/DeviceCommunicationControl.py` & `BAC0-23.7.3/BAC0/core/functions/DeviceCommunicationControl.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,38 +5,30 @@
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
 Reinitialize.py - creation of ReinitializeDeviceRequest
 
 """
 # --- standard Python modules ---
-import datetime as dt
 
-# --- 3rd party modules ---
-from bacpypes.pdu import Address, GlobalBroadcast
-from bacpypes.primitivedata import Date, Time, CharacterString, Unsigned16
-from bacpypes.basetypes import DateTime
 from bacpypes.apdu import (
     DeviceCommunicationControlRequest,
     DeviceCommunicationControlRequestEnableDisable,
     SimpleAckPDU,
 )
-from bacpypes.iocb import IOCB
 from bacpypes.core import deferred
+from bacpypes.iocb import IOCB
 
-from ...core.io.Read import find_reason
-from ..io.IOExceptions import (
-    SegmentationNotSupported,
-    ReadPropertyException,
-    ReadPropertyMultipleException,
-    NoResponseFromController,
-    ApplicationNotStarted,
-)
+# --- 3rd party modules ---
+from bacpypes.pdu import Address
+from bacpypes.primitivedata import CharacterString, Unsigned16
 
+from ...core.io.Read import find_reason
 from ...core.utils.notes import note_and_log
+from ..io.IOExceptions import ApplicationNotStarted, NoResponseFromController
 
 
 @note_and_log
 class DeviceCommunicationControl:
     """
     Mixin to support DeviceCommunicationControl from BAC0 to other devices
     """
@@ -76,17 +68,15 @@
         iocb.wait()  # Wait for BACnet response
 
         if iocb.ioResponse:  # successful response
             apdu = iocb.ioResponse
 
             if not isinstance(apdu, SimpleAckPDU):  # expect an ACK
                 self._log.warning("Not an ack, see debug for more infos.")
-                self._log.debug(
-                    "Not an ack. | APDU : {} / {}".format((apdu, type(apdu)))
-                )
+                self._log.debug("Not an ack. | APDU : {} / {}".format(apdu, type(apdu)))
                 return
 
         if iocb.ioError:  # unsuccessful: error/reject/abort
             apdu = iocb.ioError
             reason = find_reason(apdu)
             raise NoResponseFromController("APDU Abort Reason : {}".format(reason))
```

### Comparing `BAC0-22.9.21/BAC0/core/functions/Discover.py` & `BAC0-23.7.3/BAC0/core/functions/Discover.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,48 +11,41 @@
 
 """
 # --- standard Python modules ---
 import time
 
 # --- 3rd party modules ---
 from bacpypes.apdu import (
-    WhoIsRequest,
     IAmRequest,
-    WhoHasRequest,
     WhoHasLimits,
     WhoHasObject,
+    WhoHasRequest,
+    WhoIsRequest,
 )
 from bacpypes.core import deferred
-from bacpypes.pdu import Address, GlobalBroadcast, LocalBroadcast
-from bacpypes.primitivedata import Unsigned, ObjectIdentifier, CharacterString
-from bacpypes.constructeddata import Array
-from bacpypes.object import get_object_class, get_datatype
-from bacpypes.iocb import IOCB, SieveQueue, IOController
-
-from bacpypes.netservice import NetworkServiceAccessPoint, NetworkServiceElement
+from bacpypes.iocb import IOCB, IOController, SieveQueue
+from bacpypes.netservice import NetworkServiceElement
 from bacpypes.npdu import (
-    WhoIsRouterToNetwork,
     IAmRouterToNetwork,
     InitializeRoutingTable,
     InitializeRoutingTableAck,
-    WhatIsNetworkNumber,
     NetworkNumberIs,
     RejectMessageToNetwork,
+    WhatIsNetworkNumber,
+    WhoIsRouterToNetwork,
 )
+from bacpypes.pdu import Address, GlobalBroadcast, LocalBroadcast
+from bacpypes.primitivedata import CharacterString, ObjectIdentifier
 
-# --- this application's modules ---
-from ..io.IOExceptions import (
-    SegmentationNotSupported,
-    ReadPropertyException,
-    ReadPropertyMultipleException,
-    NoResponseFromController,
-    ApplicationNotStarted,
-)
 from ...core.utils.notes import note_and_log
 
+# --- this application's modules ---
+from ..io.IOExceptions import ApplicationNotStarted
+
+
 # ------------------------------------------------------------------------------
 @note_and_log
 class NetworkServiceElementWithRequests(IOController, NetworkServiceElement):
     """
     This class will add the capability to send requests at network level
     And capability to read responses for NPDU
     Deals with IOCB so the request can be deferred to task manager
@@ -80,15 +73,14 @@
         if not queue:
             queue = SieveQueue(self.request, address=destination_address)
             self.queue_by_address[destination_address] = queue
         # ask the queue to process the request
         queue.request_io(iocb)
 
     def _net_complete(self, npdu):
-
         # look up the queue
         queue = self.queue_by_address.get(npdu.pduDestination, None)
         if not queue:
             return
 
         # make sure it has an active iocb
         if not queue.active_iocb:
@@ -193,14 +185,15 @@
         msg = args if args else "any"
 
         self._log.debug("do_whois {!r}".format(msg))
 
         # build a request
         request = WhoIsRequest()
         if (len(args) == 1) or (len(args) == 3):
+            self._log.info("{:>12} {}".format("- discovered addr:", args))
             request.pduDestination = Address(args[0])
             del args[0]
         else:
             if global_broadcast:
                 request.pduDestination = GlobalBroadcast()
             else:
                 request.pduDestination = LocalBroadcast()
@@ -219,20 +212,21 @@
         self.this_application._last_i_am_received = []
         # pass to the BACnet stack
         deferred(self.this_application.request_io, iocb)
 
         iocb.wait()  # Wait for BACnet response
 
         if iocb.ioResponse:  # successful response
-            apdu = iocb.ioResponse
+            pass
 
         if iocb.ioError:  # unsuccessful: error/reject/abort
             pass
 
-        time.sleep(3)
+        for each in range(100):
+            time.sleep(1 / 1000)
         self.discoveredDevices = self.this_application.i_am_counter
         return self.this_application._last_i_am_received
 
     def _iam_request(self, destination=None):
         """
         Build the IOCB request for a I Am
         """
@@ -368,14 +362,15 @@
         obj_id = ObjectIdentifier(object_id)
         if object_name and not object_id:
             obj_name = CharacterString(object_name)
             obj = WhoHasObject(objectName=obj_name)
         elif object_id and not object_name:
             obj = WhoHasObject(objectIdentifier=obj_id)
         else:
+            obj_name = CharacterString(object_name)
             obj = WhoHasObject(objectIdentifier=obj_id, objectName=obj_name)
         limits = WhoHasLimits(
             deviceInstanceRangeLowLimit=instance_range_low_limit,
             deviceInstanceRangeHighLimit=instance_range_high_limit,
         )
         request = WhoHasRequest(object=obj, limits=limits)
         if destination:
@@ -390,15 +385,15 @@
         deferred(self.this_application.request_io, iocb)
         iocb.wait()
 
         iocb = IOCB(request)  # make an IOCB
         self.this_application._last_i_have_received = []
 
         if iocb.ioResponse:  # successful response
-            apdu = iocb.ioResponse
+            pass
 
         if iocb.ioError:  # unsuccessful: error/reject/abort
             pass
 
         time.sleep(3)
         # self.discoveredObjects = self.this_application.i_am_counter
         return self.this_application._last_i_have_received
```

### Comparing `BAC0-22.9.21/BAC0/core/functions/GetIPAddr.py` & `BAC0-23.7.3/BAC0/core/functions/GetIPAddr.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,36 +7,39 @@
 """
 Utility function to retrieve a functionnal IP and a correct broadcast IP
 address.
 Goal : not use 255.255.255.255 as a broadcast IP address as it is not
 accepted by every devices (>3.8.38.1 bacnet.jar of Tridium Jace for example)
 
 """
+import ipaddress
+import socket
+import typing as t
+
 from bacpypes.pdu import Address
 
+from ...core.utils.notes import note_and_log
 from ..io.IOExceptions import NetworkInterfaceException
 
-import socket
-import subprocess
-import ipaddress
-import sys
-import re
-from ...core.utils.notes import note_and_log
+DEFAULT_PORT = 47808
 
 
 @note_and_log
 class HostIP:
     """
     Special class to identify host IP informations
     """
 
-    def __init__(self, port=47808):
+    def __init__(self, port: t.Optional[int] = None) -> None:
         ip = self._findIPAddr()
         mask = self._findSubnetMask(ip)
-        self._port = port
+        if port is not None:
+            self._port = port
+        else:
+            self._port = DEFAULT_PORT
         self.interface = ipaddress.IPv4Interface("{}/{}".format(ip, mask))
 
     @property
     def ip_address_subnet(self):
         """
         IP Address/subnet
         """
@@ -48,15 +51,15 @@
     def ip_address(self):
         """
         IP Address/subnet
         """
         return "{}".format(self.interface.ip.compressed)
 
     @property
-    def address(self):
+    def address(self) -> Address:
         """
         IP Address using bacpypes Address format
         """
         port = ""
         if self._port:
             port = ":{}".format(self._port)
         return Address(
@@ -77,33 +80,33 @@
     @property
     def port(self):
         """
         IP Port used
         """
         return self._port
 
-    def _findIPAddr(self):
+    def _findIPAddr(self) -> str:
         """
         Retrieve the IP address connected to internet... used as
         a default IP address when defining Script
 
         :returns: IP Adress as String
         """
         s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         try:
-            s.connect(("google.com", 0))
+            s.connect(("google.com", 443))
             addr = s.getsockname()[0]
             s.close()
         except socket.error:
             raise NetworkInterfaceException(
                 "Impossible to retrieve IP, please provide one manually"
             )
         return addr
 
-    def _findSubnetMask(self, ip):
+    def _findSubnetMask(self, ip: str) -> str:
         """
         Retrieve the broadcast IP address connected to internet... used as
         a default IP address when defining Script
 
         :param ip: (str) optionnal IP address. If not provided, default to getIPAddr()
 
         :returns: broadcast IP Adress as String
@@ -120,24 +123,25 @@
                             return address["netmask"]
                 except KeyError:
                     pass
 
             return "255.255.255.255"
         except ImportError:
             self._log.warning(
-                "Netifaces not installed on your system. BAC0 can't detect the subnet.\nPlease provide subnet for now, we'll consider 255.255.255.0 (/24).\nYou can install netifaces using 'pip install netifaces'."
+                "Netifaces not installed on your system. BAC0 can't detect the subnet.\nPlease provide subnet for now, "
+                "we'll consider 255.255.255.0 (/24).\nYou can install netifaces using 'pip install netifaces'."
             )
             return "255.255.255.0"
 
 
-def validate_ip_address(ip):
+def validate_ip_address(ip: Address) -> bool:
     result = True
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
         if not isinstance(ip, Address):
             raise ValueError("Provide Address as bacpypes.Address object")
         s.bind(ip.addrTuple)
-    except OSError as error:
+    except OSError:
         result = False
     finally:
         s.close()
     return result
```

### Comparing `BAC0-22.9.21/BAC0/core/functions/Reinitialize.py` & `BAC0-23.7.3/BAC0/core/functions/Reinitialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,38 +4,31 @@
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
 Reinitialize.py - creation of ReinitializeDeviceRequest
 
 """
-from ...core.io.Read import find_reason
-from ..io.IOExceptions import (
-    SegmentationNotSupported,
-    ReadPropertyException,
-    ReadPropertyMultipleException,
-    NoResponseFromController,
-    ApplicationNotStarted,
-)
-from ...core.utils.notes import note_and_log
-
-# --- standard Python modules ---
-import datetime as dt
-
-# --- 3rd party modules ---
-from bacpypes.pdu import Address, GlobalBroadcast
-from bacpypes.primitivedata import Date, Time, CharacterString
-from bacpypes.basetypes import DateTime
 from bacpypes.apdu import (
     ReinitializeDeviceRequest,
     ReinitializeDeviceRequestReinitializedStateOfDevice,
     SimpleAckPDU,
 )
-from bacpypes.iocb import IOCB
 from bacpypes.core import deferred
+from bacpypes.iocb import IOCB
+
+# --- 3rd party modules ---
+from bacpypes.pdu import Address
+from bacpypes.primitivedata import CharacterString
+
+from ...core.io.Read import find_reason
+from ...core.utils.notes import note_and_log
+from ..io.IOExceptions import ApplicationNotStarted, NoResponseFromController
+
+# --- standard Python modules ---
 
 
 @note_and_log
 class Reinitialize:
     """
     Mixin to support Reinitialize from BAC0 to other devices
     """
@@ -69,17 +62,15 @@
         iocb.wait()  # Wait for BACnet response
 
         if iocb.ioResponse:  # successful response
             apdu = iocb.ioResponse
 
             if not isinstance(apdu, SimpleAckPDU):  # expect an ACK
                 self._log.warning("Not an ack, see debug for more infos.")
-                self._log.debug(
-                    "Not an ack. | APDU : {} / {}".format((apdu, type(apdu)))
-                )
+                self._log.debug("Not an ack. | APDU : {} / {}".format(apdu, type(apdu)))
                 return
 
         if iocb.ioError:  # unsuccessful: error/reject/abort
             apdu = iocb.ioError
             reason = find_reason(apdu)
             raise NoResponseFromController("APDU Abort Reason : {}".format(reason))
```

### Comparing `BAC0-22.9.21/BAC0/core/functions/Schedule.py` & `BAC0-23.7.3/BAC0/core/functions/Schedule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,31 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
-"""
-ScheduleWrite.py - creation of ReinitializeDeviceRequest
-
-"""
-from ..io.Read import find_reason
-from ..io.IOExceptions import (
-    SegmentationNotSupported,
-    ReadPropertyException,
-    ReadPropertyMultipleException,
-    NoResponseFromController,
-    ApplicationNotStarted,
-)
-from ...core.utils.notes import note_and_log
+import typing as t
 
 # --- standard Python modules ---
-import datetime as dt
+from datetime import time as dt_time
 
-# --- 3rd party modules ---
-from bacpypes.pdu import Address, GlobalBroadcast
-from bacpypes.primitivedata import Integer, Date, Time, CharacterString
-from bacpypes.basetypes import DateTime
-from bacpypes.apdu import WritePropertyRequest, SimpleAckPDU
-from bacpypes.iocb import IOCB
+from bacpypes.apdu import SimpleAckPDU, WritePropertyRequest
+from bacpypes.basetypes import DailySchedule, TimeValue
+from bacpypes.constructeddata import Any, ArrayOf
 from bacpypes.core import deferred
-from bacpypes.basetypes import DateTime, DailySchedule, TimeValue, Time
-from bacpypes.constructeddata import ArrayOf, Any
+from bacpypes.iocb import IOCB
 
-from bacpypes.primitivedata import Null, Atomic, Integer, Unsigned, Real, Enumerated
+# --- 3rd party modules ---
+from bacpypes.pdu import Address
+from bacpypes.primitivedata import Enumerated, Integer, Real
 
-from datetime import time as dt_time
-from datetime import datetime as dt
+from ...core.utils.notes import note_and_log
+from ..io.IOExceptions import NoResponseFromController
+from ..io.Read import find_reason
 
 
 @note_and_log
 class Schedule:
     """
     Everything you need to write to a schedule
     """
@@ -102,15 +89,15 @@
             self.schedules[object_reference] = ds
 
         def _set_value(v):
             try:
                 if dict_schedule["states"].lower() == "analog":
                     return Real(v)
             except AttributeError:
-                if dict_schedule["states"] == ["inactive", "active"]:
+                if dict_schedule["states"] == {"inactive": 0, "active": 1}:
                     return Integer(dict_schedule["states"][v])
                 else:
                     return Enumerated(dict_schedule["states"][v] - 1)
 
         daily_schedules = []
         for day in Schedule.days:
             list_of_events = dict_schedule["week"][day]
@@ -142,17 +129,15 @@
         iocb.wait()
 
         if iocb.ioResponse:  # successful response
             apdu = iocb.ioResponse
 
             if not isinstance(apdu, SimpleAckPDU):  # expect an ACK
                 self._log.warning("Not an ack, see debug for more infos.")
-                self._log.debug(
-                    "Not an ack. | APDU : {} / {}".format((apdu, type(apdu)))
-                )
+                self._log.debug("Not an ack. | APDU : {} / {}".format(apdu, type(apdu)))
                 return
         if iocb.ioError:  # unsuccessful: error/reject/abort
             apdu = iocb.ioError
             reason = find_reason(apdu)
             raise NoResponseFromController("APDU Abort Reason : {}".format(reason))
 
         self._log.info(
@@ -201,16 +186,16 @@
                 reliability = _read("reliability")
                 priority = _read("priorityForWriting")
                 presentValue = _read("presentValue")
 
             except Exception:
                 raise ()
 
-        schedule = {}
-        _state_text = None
+        schedule: t.Dict[str, t.Union[t.Dict, t.List]] = {}
+        _state_text: t.Union[str, range, t.List[str], None] = None
         offset_MV = 0 if len(object_references) == 0 else 1
 
         try:
             first_obj_id = object_references[0]
             obj_type, obj_instance = first_obj_id.objectIdentifier
             if obj_type == "binaryValue":
                 _state_text = ["inactive", "active"]
@@ -235,38 +220,41 @@
         except Exception as error:
             self._log.error("Error {}".format(error))
             # Not used in device, not linked...
             _state_text = range(255)
             schedule["object_references"] = []
             schedule["references_names"] = []
 
-        schedule["states"] = {}
+        # re-ordered to make type inference possible, but not sure the logic here
+        # is 100% sound (ignored type warnings both look like actual problems).
+        # keeping logic intact and ignoring warnings for now
+        sched_states = {}
         if _state_text == ["inactive", "active"]:
             for i, each in enumerate(_state_text):
-                schedule["states"][each] = i
+                sched_states[each] = i
             presentValue = "{} ({})".format(
-                list(schedule["states"].keys())[int(presentValue.value)],
+                list(sched_states.keys())[int(presentValue.value)],
                 presentValue.value,
             )
-        elif _state_text != "analog":
-            for i, each in enumerate(_state_text):
-                schedule["states"][each] = i + offset_MV
+        elif _state_text == "analog":
+            sched_states = _state_text  # type: ignore[assignment]
+            if presentValue is not None:
+                presentValue = "{}".format(presentValue.value)
+        else:
             try:
+                for i, each in enumerate(_state_text):  # type: ignore[arg-type]
+                    sched_states[each] = i + offset_MV
                 presentValue = "{} ({})".format(
-                    list(schedule["states"].keys())[
-                        int(presentValue.value) - offset_MV
-                    ],
+                    list(sched_states.keys())[int(presentValue.value) - offset_MV],
                     presentValue.value,
                 )
             except TypeError:
                 presentValue = presentValue.value
-        else:
-            schedule["states"] = _state_text
-            if presentValue is not None:
-                presentValue = "{}".format(presentValue.value)
+
+        schedule["states"] = sched_states
         schedule["reliability"] = reliability
         schedule["priority"] = priority
         schedule["presentValue"] = presentValue
         schedule["week"] = self.decode_weeklySchedule(_schedule, _state_text, offset_MV)
 
         return schedule
```

### Comparing `BAC0-22.9.21/BAC0/core/functions/Text.py` & `BAC0-23.7.3/BAC0/core/functions/Text.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from bacpypes.iocb import IOCB
-from bacpypes.core import deferred
-from bacpypes.apdu import WritePropertyRequest, SimpleAckPDU
-from bacpypes.primitivedata import CharacterString
+from bacpypes.apdu import SimpleAckPDU, WritePropertyRequest
 from bacpypes.constructeddata import Any
+from bacpypes.core import deferred
+from bacpypes.iocb import IOCB
 from bacpypes.pdu import Address
+from bacpypes.primitivedata import CharacterString
+
 from BAC0.core.io.IOExceptions import NoResponseFromController, WritePropertyException
 from BAC0.core.io.Read import find_reason
 
 
 class TextMixin:
     """
     Mixin with functions to deal with text properties.
```

### Comparing `BAC0-22.9.21/BAC0/core/functions/TimeSync.py` & `BAC0-23.7.3/BAC0/core/functions/TimeSync.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,35 +4,32 @@
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
 TimeSync.py - creation of time synch requests
 
 """
-from ...core.io.Read import find_reason
-from ..io.IOExceptions import (
-    SegmentationNotSupported,
-    ReadPropertyException,
-    ReadPropertyMultipleException,
-    NoResponseFromController,
-    ApplicationNotStarted,
-)
-from ...core.utils.notes import note_and_log
-
 # --- standard Python modules ---
 import datetime as dt
+from datetime import datetime
+
+import pytz
+from bacpypes.apdu import TimeSynchronizationRequest, UTCTimeSynchronizationRequest
+from bacpypes.basetypes import DateTime
+from bacpypes.core import deferred
+from bacpypes.iocb import IOCB
 
 # --- 3rd party modules ---
 from bacpypes.pdu import Address, GlobalBroadcast, LocalBroadcast
 from bacpypes.primitivedata import Date, Time
-from bacpypes.basetypes import DateTime
-from bacpypes.apdu import TimeSynchronizationRequest, UTCTimeSynchronizationRequest
-from bacpypes.iocb import IOCB
-from bacpypes.core import deferred
-import pytz
+
+from ...core.utils.notes import note_and_log
+from ..io.IOExceptions import (
+    ApplicationNotStarted,
+)
 
 
 def _build_datetime(UTC=False):
     if UTC:
         _d = dt.datetime.utcnow().date()
         _t = dt.datetime.utcnow().time()
         _date = Date(
@@ -134,32 +131,32 @@
 class TimeHandler(object):
     """
     This class will deal with Time / Timezone related features
     To deal with DateTime Value correctly we need to be aware
     of timezone.
     """
 
-    def __init__(self, tz="America/Montreal"):
+    def __init__(self, tz: str = "America/Montreal") -> None:
         self.set_timezone(tz)
 
-    def set_timezone(self, tz):
+    def set_timezone(self, tz: str) -> None:
         self.timezone = pytz.timezone(tz)
 
     @property
-    def now(self):
+    def now(self) -> datetime:
         return dt.datetime.now()
 
     def local_time(self):
         return self.now.time()
 
     def local_date(self):
         return self.now.date()
 
-    def utcOffset(self):
+    def utcOffset(self) -> float:
         "Returns UTC offset in minutes"
-        return round(self.now.astimezone().utcoffset().total_seconds() / 60)
+        return round(self.now.astimezone().utcoffset().total_seconds() / 60)  # type: ignore[union-attr]
 
-    def is_dst(self):
+    def is_dst(self) -> bool:
         return self.timezone.dst(self.now) != dt.timedelta(0)
 
     def __repr__(self):
         return "{}".format(self.__dict__)
```

### Comparing `BAC0-22.9.21/BAC0/core/functions/cov.py` & `BAC0-23.7.3/BAC0/core/functions/cov.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from bacpypes.apdu import SubscribeCOVRequest, SimpleAckPDU, RejectPDU, AbortPDU
-from bacpypes.iocb import IOCB
+from bacpypes.apdu import SubscribeCOVRequest
+from bacpypes.constructeddata import Array
 from bacpypes.core import deferred
+from bacpypes.iocb import IOCB
+from bacpypes.object import get_datatype
 from bacpypes.pdu import Address
-from bacpypes.object import get_object_class, get_datatype
-from bacpypes.constructeddata import Array
-from bacpypes.primitivedata import Tag, ObjectIdentifier, Unsigned
+from bacpypes.primitivedata import Unsigned
 
 from BAC0.core.io.Read import cast_datatype_from_tag
 
 """
 
 using cov, we build a "context" which is turned into a subscription being sent to 
 the destination.
```

### Comparing `BAC0-22.9.21/BAC0/core/io/IOExceptions.py` & `BAC0-23.7.3/BAC0/core/io/IOExceptions.py`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/core/io/Read.py` & `BAC0-23.7.3/BAC0/core/io/Read.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,84 +17,82 @@
         ReadProperty()
             def read()
             def readMultiple()
 
 """
 
 # --- standard Python modules ---
+import typing as t
 
-# --- 3rd party modules ---
-from bacpypes.debugging import bacpypes_debugging
-
-from bacpypes.pdu import Address
-from bacpypes.object import get_object_class, get_datatype
 from bacpypes.apdu import (
-    PropertyReference,
-    ReadAccessSpecification,
-    ReadPropertyRequest,
-    ReadPropertyMultipleRequest,
-    RejectReason,
-    AbortReason,
-    RejectPDU,
     AbortPDU,
-)
-
-from bacpypes.basetypes import PropertyIdentifier, DateTime
-from bacpypes.apdu import (
-    ReadPropertyMultipleACK,
-    ReadPropertyACK,
-    ReadRangeRequest,
-    ReadRangeACK,
+    AbortReason,
+    PropertyReference,
     Range,
     RangeByPosition,
     RangeBySequenceNumber,
     RangeByTime,
+    ReadAccessSpecification,
+    ReadPropertyACK,
+    ReadPropertyMultipleACK,
+    ReadPropertyMultipleRequest,
+    ReadPropertyRequest,
+    ReadRangeACK,
+    ReadRangeRequest,
+    RejectPDU,
+    RejectReason,
 )
-from bacpypes.primitivedata import Tag, ObjectIdentifier, Unsigned, Date, Time
+from bacpypes.basetypes import DateTime, PropertyIdentifier
 from bacpypes.constructeddata import Array
-from bacpypes.iocb import IOCB, TimeoutError
 from bacpypes.core import deferred
+from bacpypes.iocb import IOCB, TimeoutError
+from bacpypes.object import get_datatype, get_object_class, registered_object_types
+
+# --- 3rd party modules ---
+from bacpypes.pdu import Address
+from bacpypes.primitivedata import Date, Tag, Time, Unsigned
+
+from ..utils.notes import note_and_log
 
 # --- this application's modules ---
 from .IOExceptions import (
+    ApplicationNotStarted,
+    NoResponseFromController,
     ReadPropertyException,
     ReadPropertyMultipleException,
     ReadRangeException,
-    NoResponseFromController,
-    ApplicationNotStarted,
-    UnrecognizedService,
     SegmentationNotSupported,
-    UnknownPropertyError,
     UnknownObjectError,
-    BufferOverflow,
+    UnknownPropertyError,
+    UnrecognizedService,
 )
-from bacpypes.object import registered_object_types
-
-from ..utils.notes import note_and_log
 
 # ------------------------------------------------------------------------------
 
 
+ReadValue = t.Union[float, str, t.List]
+
+
 @note_and_log
 class ReadProperty:
     """
     Defines BACnet Read functions: readProperty and readPropertyMultiple.
     Data exchange is made via a Queue object
     A timeout of 10 seconds allows detection of invalid device or communciation errors.
     """
 
     def read(
         self,
-        args,
-        arr_index=None,
-        vendor_id=0,
+        args: str,
+        arr_index: t.Optional[int] = None,
+        vendor_id: int = 0,
         bacoid=None,
-        timeout=10,
-        show_property_name=False,
-    ):
+        timeout: int = 10,
+        show_property_name: bool = False,
+    ) -> t.Union[ReadValue, t.Tuple[ReadValue, str], None]:
         """
         Build a ReadProperty request, wait for the answer and return the value
 
         :param args: String with <addr> <type> <inst> <prop> [ <indx> ]
         :returns: data read from device (str representing data like 10 or True)
 
         *Example*::
@@ -110,17 +108,14 @@
         if not self._started:
             raise ApplicationNotStarted("BACnet stack not running - use startApp()")
 
         args_split = args.split()
 
         self.log_title("Read property", args_split)
 
-        vendor_id = vendor_id
-        bacoid = bacoid
-
         try:
             # build ReadProperty request
             iocb = IOCB(
                 self.build_rp_request(
                     args_split, arr_index=arr_index, vendor_id=vendor_id, bacoid=bacoid
                 )
             )
@@ -137,15 +132,15 @@
 
         if iocb.ioResponse:  # successful response
             apdu = iocb.ioResponse
 
             if not isinstance(apdu, ReadPropertyACK):  # expecting an ACK
                 self._log.warning("Not an ack, see debug for more infos.")
                 self._log.debug("Not an ack. | APDU : {}".format(apdu))
-                return
+                return None
 
             # find the datatype
             datatype = get_datatype(
                 apdu.objectIdentifier[0], apdu.propertyIdentifier, vendor_id=vendor_id
             )
             if not datatype:
                 # raise TypeError("unknown datatype")
@@ -169,41 +164,44 @@
                 self._log.debug("{:<20} {:<20}".format("value", "datatype"))
                 self._log.debug("{!r:<20} {!r:<20}".format(value, datatype))
             if not show_property_name:
                 return value
 
             try:
                 int(apdu.propertyIdentifier)
-                objid = apdu.objectIdentifier
                 prop_id = "@prop_{}".format(apdu.propertyIdentifier)
                 value = list(value.items())[0][1]
             except ValueError:
                 prop_id = apdu.propertyIdentifier
             return (value, prop_id)
+
         if iocb.ioError:  # unsuccessful: error/reject/abort
             apdu = iocb.ioError
             reason = find_reason(apdu)
             if reason == "segmentationNotSupported":
                 value = self._split_the_read_request(args, arr_index)
                 return value
             else:
                 if reason == "unknownProperty":
                     if "description" in args:
                         self._log.warning(
-                            "The description property is not implemented in the device. Using a default value for internal needs."
+                            "The description property is not implemented in the device. "
+                            "Using a default value for internal needs."
                         )
                         return "Property Not Implemented"
                     elif "inactiveText" in args:
                         self._log.warning(
-                            "The inactiveText property is not implemented in the device. Using a default value of Off for internal needs."
+                            "The inactiveText property is not implemented in the device. "
+                            "Using a default value of Off for internal needs."
                         )
                         return "Off"
                     elif "activeText" in args:
                         self._log.warning(
-                            "The activeText property is not implemented in the device. Using a default value of On for internal needs."
+                            "The activeText property is not implemented in the device. "
+                            "Using a default value of On for internal needs."
                         )
                         return "On"
                     else:
                         raise UnknownPropertyError("Unknown property {}".format(args))
                 elif reason == "unknownObject":
                     self._log.warning("Unknown object {}".format(args))
                     raise UnknownObjectError("Unknown object {}".format(args))
@@ -214,32 +212,39 @@
                     return self._split_the_read_request(args, arr_index)
                 else:
                     # Other error... consider NoResponseFromController (65)
                     # even if the real reason is another one
                     raise NoResponseFromController(
                         "APDU Abort Reason : {}".format(reason)
                     )
+        return None
 
     def _split_the_read_request(self, args, arr_index):
         """
         When a device doesn't support segmentation, this function
         will split the request according to the length of the
         predicted result which can be known when reading the array_index
         number 0.
 
         This can be a very long process as some devices count a large
         number of properties without supporting segmentation
         (FieldServers are a good example)
         """
+        # parameter arr_index appears to be unused in this function?
         nmbr_obj = self.read(args, arr_index=0)
-        return [self.read(args, arr_index=i) for i in range(1, nmbr_obj + 1)]
+        return [self.read(args, arr_index=i) for i in range(1, nmbr_obj + 1)]  # type: ignore
 
     def readMultiple(
-        self, args, request_dict=None, vendor_id=0, timeout=10, show_property_name=False
-    ):
+        self,
+        args: str,
+        request_dict=None,
+        vendor_id: int = 0,
+        timeout: int = 10,
+        show_property_name: bool = False,
+    ) -> t.Union[t.Dict, t.List[t.Tuple[t.Any, str]]]:
         """Build a ReadPropertyMultiple request, wait for the answer and return the values
 
         :param args: String with <addr> ( <type> <inst> ( <prop> [ <indx> ] )... )...
         :returns: data read from device (str representing data like 10 or True)
 
         *Example*::
 
@@ -253,17 +258,17 @@
         """
         if not self._started:
             raise ApplicationNotStarted("BACnet stack not running - use startApp()")
 
         if request_dict is not None:
             request = self.build_rpm_request_from_dict(request_dict, vendor_id)
         else:
-            args = args.split()
-            request = self.build_rpm_request(args, vendor_id=vendor_id)
-            self.log_title("Read Multiple", args)
+            args_list = args.split()
+            request = self.build_rpm_request(args_list, vendor_id=vendor_id)
+            self.log_title("Read Multiple", args_list)
 
         values = []
         dict_values = {}
 
         try:
             # build an ReadPropertyMultiple request
             iocb = IOCB(request)
@@ -277,20 +282,22 @@
             self._log.exception("exception: {!r}".format(error))
 
         iocb.wait()  # Wait for BACnet response
 
         if iocb.ioResponse:  # successful response
             apdu = iocb.ioResponse
 
+            # note: the return types along this pass don't appear to be consistent
+            # not sure if this is a real problem or not, leaving as-is and ignoring errors
             if not isinstance(apdu, ReadPropertyMultipleACK):  # expecting an ACK
                 self._log.debug("{:<20}".format("not an ack"))
                 self._log.warning(
-                    "Not an Ack. | APDU : {} / {}".format((apdu, type(apdu)))
+                    "Not an Ack. | APDU : {} / {}".format(apdu, type(apdu))
                 )
-                return
+                return  # type: ignore[return-value]
 
             # loop through the results
             for result in apdu.listOfReadAccessResults:
                 # here is the object identifier
                 objectIdentifier = result.objectIdentifier
 
                 self.log_subtitle(
@@ -374,15 +381,15 @@
                                 _key = (str(_obj), vendor_id)
                                 if _key in registered_object_types.keys():
                                     _classname = registered_object_types[_key].__name__
                                     for k, v in registered_object_types["BAC0"][
                                         _classname
                                     ].items():
                                         if v["obj_id"] == propertyIdentifier:
-                                            prop_id = (k, propertyIdentifier)
+                                            prop_id = (k, propertyIdentifier)  # type: ignore
                                 if isinstance(value, dict):
                                     value = list(value.items())[0][1]
 
                             except ValueError:
                                 prop_id = propertyIdentifier
                             values.append((value, prop_id))
                             dict_values[objectIdentifier].append(
@@ -393,14 +400,16 @@
                             dict_values[objectIdentifier].append((_prop_id, value))
 
             if request_dict is not None:
                 return dict_values
             else:
                 return values
 
+        # note: the return types along this pass don't appear to be consistent
+        # not sure if this is a real problem or not, leaving as-is and ignoring errors
         if iocb.ioError:  # unsuccessful: error/reject/abort
             apdu = iocb.ioError
             reason = find_reason(apdu)
             self._log.warning("APDU Abort Reject Reason : {}".format(reason))
             self._log.debug("The Request was : {}".format(args))
             if reason == "unrecognizedService":
                 raise UnrecognizedService()
@@ -410,40 +419,46 @@
                 self.segmentation_supported = False
                 raise SegmentationNotSupported()
             elif reason == "unknownObject":
                 self._log.warning("Unknown object {}".format(args))
                 raise UnknownObjectError("Unknown object {}".format(args))
             elif reason == "unknownProperty":
                 self._log.warning("Unknown property {}".format(args))
-
-                values.append("")
+                values.append("")  # type: ignore[arg-type]
                 return values
             else:
                 self._log.warning("No response from controller {}".format(reason))
-                values.append("")
+                values.append("")  # type: ignore[arg-type]
                 return values
 
-    def build_rp_request(self, args, arr_index=None, vendor_id=0, bacoid=None):
-        addr, obj_type, obj_inst, prop_id = args[:4]
-        vendor_id = vendor_id
-        bacoid = bacoid
+        return values
 
+    def __get_obj_type(self, obj_type: str, vendor_id) -> int:
         if obj_type.isdigit():
-            obj_type = int(obj_type)
+            return int(obj_type)
         elif "@obj_" in obj_type:
-            obj_type = int(obj_type.split("_")[1])
+            return int(obj_type.split("_")[1])
         elif not get_object_class(obj_type, vendor_id=vendor_id):
             raise ValueError("Unknown object type : {}".format(obj_type))
+        return obj_type  # type: ignore
 
-        obj_inst = int(obj_inst)
-
-        if prop_id.isdigit():
-            prop_id = int(prop_id)
-        elif "@prop_" in prop_id:
-            prop_id = int(prop_id.split("_")[1])
+    def build_rp_request(
+        self, args: t.List[str], arr_index=None, vendor_id: int = 0, bacoid=None
+    ) -> ReadPropertyRequest:
+        addr, obj_type_str, obj_inst_str, prop_id_str = args[:4]
+
+        obj_type = self.__get_obj_type(obj_type_str, vendor_id)
+        obj_inst = int(obj_inst_str)
+
+        if prop_id_str.isdigit():
+            prop_id = int(prop_id_str)
+        elif "@prop_" in prop_id_str:
+            prop_id = int(prop_id_str.split("_")[1])
+        else:
+            prop_id = prop_id_str  # type: ignore
 
         # datatype = get_datatype(obj_type, prop_id, vendor_id=vendor_id)
 
         # build a request
         request = ReadPropertyRequest(
             objectIdentifier=(obj_type, obj_inst),
             propertyIdentifier=prop_id,
@@ -452,48 +467,44 @@
         request.pduDestination = Address(addr)
 
         if len(args) == 5:
             request.propertyArrayIndex = int(args[4])
         self._log.debug("{:<20} {!r}".format("REQUEST", request))
         return request
 
-    def build_rpm_request(self, args, vendor_id=0):
+    def build_rpm_request(
+        self, args: t.List[str], vendor_id: int = 0
+    ) -> ReadPropertyMultipleRequest:
         """
         Build request from args
         """
         self._log.debug(args)
         i = 0
         addr = args[i]
         i += 1
         vendor_id = vendor_id
 
         read_access_spec_list = []
         while i < len(args):
-            obj_type = args[i]
+            obj_type_str = args[i]
             i += 1
 
-            if obj_type.isdigit():
-                obj_type = int(obj_type)
-            elif "@obj_" in obj_type:
-                obj_type = int(obj_type.split("_")[1])
-            elif not get_object_class(obj_type, vendor_id=vendor_id):
-                raise ValueError("Unknown object type : {}".format(obj_type))
-
+            obj_type = self.__get_obj_type(obj_type_str, vendor_id)
             obj_inst = int(args[i])
             i += 1
 
             prop_reference_list = []
             while i < len(args):
                 prop_id = args[i]
                 if "@obj_" in prop_id:
                     break
                 if prop_id not in PropertyIdentifier.enumerations:
                     try:
                         if "@prop_" in prop_id:
-                            prop_id = int(prop_id.split("_")[1])
+                            prop_id = int(prop_id.split("_")[1])  # type: ignore[assignment]
                             self._log.debug(
                                 "Proprietary property : {} | {} -> Vendor : {}".format(
                                     obj_type, prop_id, vendor_id
                                 )
                             )
                         else:
                             break
@@ -708,17 +719,15 @@
         iocb.wait()  # Wait for BACnet response
 
         if iocb.ioResponse:  # successful response
             apdu = iocb.ioResponse
 
             if not isinstance(apdu, ReadRangeACK):  # expecting an ACK
                 self._log.warning("Not an ack, see debug for more infos.")
-                self._log.debug(
-                    "Not an ack. | APDU : {} / {}".format((apdu, type(apdu)))
-                )
+                self._log.debug("Not an ack. | APDU : {} / {}".format(apdu, type(apdu)))
                 return
 
             # find the datatype
             datatype = get_datatype(
                 apdu.objectIdentifier[0], apdu.propertyIdentifier, vendor_id=vendor_id
             )
             if not datatype:
@@ -773,45 +782,52 @@
                 else:
                     # Other error... consider NoResponseFromController (65)
                     # even if the realy reason is another one
                     raise NoResponseFromController(
                         "APDU Abort Reason : {}".format(reason)
                     )
 
-    def read_priority_array(self, addr, obj, obj_instance):
+    def read_priority_array(self, addr, obj, obj_instance) -> t.List:
         pa = self.read("{} {} {} priorityArray".format(addr, obj, obj_instance))
         res = [pa]
         for each in range(1, 17):
-            _pa = pa[each]
+            _pa = pa[each]  # type: ignore[index]
             for k, v in _pa.__dict__.items():
-                if v != None:
+                if v is not None:
                     res.append(v)
         return res
 
 
 def find_reason(apdu):
     try:
         if apdu == TimeoutError:
             return "Timeout"
         elif apdu.pduType == RejectPDU.pduType:
             reasons = RejectReason.enumerations
         elif apdu.pduType == AbortPDU.pduType:
             reasons = AbortReason.enumerations
         else:
-            if apdu.errorCode and apdu.errorClass:
-                return "{}".format(apdu.errorCode)
-            else:
-                raise ValueError("Cannot find reason...")
+            _code = None
+            try:
+                _code = apdu.errorCode
+            except AttributeError:
+                try:
+                    _code = apdu.errorType.errorCode
+                except AttributeError:
+                    raise ValueError("Cannot find reason...")
+
+            if _code:
+                return "{}".format(_code)
         code = apdu.apduAbortRejectReason
         try:
             return [k for k, v in reasons.items() if v == code][0]
         except IndexError:
             return code
     except KeyError as err:
-        return "KeyError: {} has no key {0!r}".format(type(apdu), err.args[0])
+        return "KeyError: {} has no key {!r}".format(type(apdu), err.args[0])
 
 
 def cast_datatype_from_tag(propertyValue, obj_id, prop_id):
     try:
         tag_list = propertyValue.tagList.tagList
         if tag_list[0].tagClass == 0:
             tag = tag_list[0].tagNumber
```

### Comparing `BAC0-22.9.21/BAC0/core/io/Simulate.py` & `BAC0-23.7.3/BAC0/core/io/Simulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/python
+# type: ignore
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
 Simulate.py - simulate the value of controller I/O values
 """
 
 # --- standard Python modules ---
 # --- 3rd party modules ---
 # --- this application's modules ---
 from .IOExceptions import (
+    ApplicationNotStarted,
+    NoResponseFromController,
     OutOfServiceNotSet,
     OutOfServiceSet,
-    NoResponseFromController,
-    ApplicationNotStarted,
 )
 
-
 # ------------------------------------------------------------------------------
 
 
 class Simulation:
     """
     Global informations regarding simulation
     """
```

### Comparing `BAC0-22.9.21/BAC0/core/io/Write.py` & `BAC0-23.7.3/BAC0/core/io/Write.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,42 +15,40 @@
     Class::
 
         WriteProperty()
             def write()
 
 
 """
-# --- 3rd party modules ---
-from bacpypes.debugging import bacpypes_debugging, ModuleLogger
-
-from bacpypes.pdu import Address
-from bacpypes.object import get_datatype
-
 from bacpypes.apdu import (
-    WritePropertyRequest,
-    WritePropertyMultipleRequest,
     SimpleAckPDU,
     WriteAccessSpecification,
+    WritePropertyMultipleRequest,
+    WritePropertyRequest,
 )
+from bacpypes.basetypes import PropertyValue
+from bacpypes.constructeddata import Any, Array
+from bacpypes.core import deferred
 
-from bacpypes.primitivedata import Null, Atomic, Integer, Unsigned, Real, Enumerated
-from bacpypes.constructeddata import Array, Any, SequenceOf
-from bacpypes.basetypes import PropertyValue, PropertyIdentifier
+# --- 3rd party modules ---
+from bacpypes.debugging import ModuleLogger
 from bacpypes.iocb import IOCB
-from bacpypes.core import deferred
+from bacpypes.object import get_datatype
+from bacpypes.pdu import Address
+from bacpypes.primitivedata import Atomic, Enumerated, Integer, Null, Real, Unsigned
+
+from ...core.utils.notes import note_and_log
 
 # --- this application's modules ---
 from .IOExceptions import (
-    WritePropertyCastError,
+    ApplicationNotStarted,
     NoResponseFromController,
+    WritePropertyCastError,
     WritePropertyException,
-    WriteAccessDenied,
-    ApplicationNotStarted,
 )
-from ...core.utils.notes import note_and_log
 from .Read import find_reason
 
 # ------------------------------------------------------------------------------
 
 # some debugging
 _debug = 0
 _LOG = ModuleLogger(globals())
@@ -98,17 +96,15 @@
         iocb.wait()  # Wait for BACnet response
 
         if iocb.ioResponse:  # successful response
             apdu = iocb.ioResponse
 
             if not isinstance(apdu, SimpleAckPDU):  # expect an ACK
                 self._log.warning("Not an ack, see debug for more infos.")
-                self._log.debug(
-                    "Not an ack. | APDU : {} / {}".format((apdu, type(apdu)))
-                )
+                self._log.debug("Not an ack. | APDU : {} / {}".format(apdu, type(apdu)))
                 return
 
         if iocb.ioError:  # unsuccessful: error/reject/abort
             apdu = iocb.ioError
             reason = find_reason(apdu)
             raise NoResponseFromController("APDU Abort Reason : {}".format(reason))
 
@@ -275,17 +271,15 @@
         iocb.wait()  # Wait for BACnet response
 
         if iocb.ioResponse:  # successful response
             apdu = iocb.ioResponse
 
             if not isinstance(apdu, SimpleAckPDU):  # expect an ACK
                 self._log.warning("Not an ack, see debug for more infos.")
-                self._log.debug(
-                    "Not an ack. | APDU : {} / {}".format((apdu, type(apdu)))
-                )
+                self._log.debug("Not an ack. | APDU : {} / {}".format(apdu, type(apdu)))
                 return
 
         if iocb.ioError:  # unsuccessful: error/reject/abort
             apdu = iocb.ioError
             reason = find_reason(apdu)
             raise NoResponseFromController("APDU Abort Reason : {}".format(reason))
 
@@ -323,15 +317,15 @@
             )
 
             existingObject = next(
                 (obj for obj in was if obj.objectIdentifier == (obj_type, obj_inst)),
                 None,
             )
 
-            if existingObject == None:
+            if existingObject is None:
                 property_values.append(
                     PropertyValue(
                         propertyIdentifier=prop_id,
                         propertyArrayIndex=indx,
                         value=value,
                         priority=priority,
                     )
```

### Comparing `BAC0-22.9.21/BAC0/core/proprietary_objects/jci.py` & `BAC0-23.7.3/BAC0/core/proprietary_objects/jci.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 #!/usr/bin/env python
 
 """
 Johnson Controls Proprietary Objects for FX/FEC Line
 """
+from bacpypes.object import (
+    AnalogInputObject,
+    AnalogOutputObject,
+    AnalogValueObject,
+    DeviceObject,
+)
 from bacpypes.primitivedata import (
-    Real,
-    Boolean,
-    CharacterString,
-    Enumerated,
-    Unsigned,
     Atomic,
+    Boolean,  # Signed,
+    CharacterString,
     Date,
+    Enumerated,
+    Real,
     Time,
-    #    Signed,
-)
-from bacpypes.object import (
-    Object,
-    DeviceObject,
-    AnalogValueObject,
-    AnalogInputObject,
-    AnalogOutputObject,
-    BinaryValueObject,
-    Property,
-    register_object_type,
+    Unsigned,
 )
 
 #
 #   Proprietary Objects and their attributes
 #   https://cgproducts.johnsoncontrols.com/MET_PDF/12013102.pdf
 #
 
@@ -38,15 +33,14 @@
     "properties": {
         "ALARM_STATE": {"obj_id": 1006, "datatype": Enumerated, "mutable": False},
         "ARCHIVE_DATE": {"obj_id": 849, "datatype": Date, "mutable": False},
         "ARCHIVE_STATUS": {"obj_id": 1187, "datatype": Unsigned, "mutable": False},
         "ARCHIVE_TIME": {"obj_id": 850, "datatype": Time, "mutable": False},
         "CPU_USAGE": {"obj_id": 2583, "datatype": Real, "mutable": False},
         "ENABLED": {"obj_id": 673, "datatype": Boolean, "mutable": True},
-        "ENABLED": {"obj_id": 673, "datatype": Boolean, "mutable": True},
         "EXECUTION_PRIORITY": {
             "obj_id": 2197,
             "datatype": Enumerated,
             "mutable": True,
         },  # 0-3
         "EXTENDED_PROTO_VERSION": {
             "obj_id": 2291,
@@ -303,18 +297,16 @@
     "name": "JCIAnalogOutputObject",
     "vendor_id": 5,
     "objectType": "analogOutput",
     "bacpypes_type": AnalogOutputObject,
     "properties": {
         "Offline": {"obj_id": 913, "datatype": Boolean, "mutable": False},
         "SABusAddr": {"obj_id": 3645, "datatype": Unsigned, "mutable": False},
-        "InputRangeLow": {"obj_id": 1293, "datatype": Real, "mutable": True},
-        "InputRangeHigh": {"obj_id": 1294, "datatype": Real, "mutable": True},
-        "OutputRangeLow": {"obj_id": 1295, "datatype": Real, "mutable": True},
-        "OutputRangeHigh": {"obj_id": 1296, "datatype": Real, "mutable": True},
+        "MIN_OUT_VALUE": {"obj_id": 652, "datatype": Real, "mutable": True},
+        "MAX_OUT_VALUE": {"obj_id": 653, "datatype": Real, "mutable": True},
         "polarity": {"obj_id": "polarity", "datatype": Enumerated, "mutable": True},
         "stroketime": {"obj_id": 3478, "datatype": Real, "mutable": True},
     },
 }
 
 
 def tec_short_point_list(unit_type="2-pipe"):
```

### Comparing `BAC0-22.9.21/BAC0/core/proprietary_objects/object.py` & `BAC0-23.7.3/BAC0/core/proprietary_objects/object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from typing import Any, Dict
+
 from bacpypes.object import (
     Object,
     Property,
     register_object_type,
     registered_object_types,
 )
 
+
 # Prochaine étape : créer une focntion qui va lire "all" et se redéfinir dynamiquement
-def create_proprietary_object(params):
+def create_proprietary_object(params: Dict[str, Any]) -> None:
 
     try:
         _validate_params(params)
     except:
         raise
     # Prevent breaking change for existing code, since issue #311
     try:
@@ -32,15 +35,15 @@
     register_object_type(new_class, vendor_id=params["vendor_id"])
     if "BAC0" not in registered_object_types.keys():
         registered_object_types["BAC0"] = {}
 
     registered_object_types["BAC0"][params["name"]] = params["properties"]
 
 
-def _validate_params(params):
+def _validate_params(params: Dict[str, Any]) -> bool:
     if not params["name"]:
         raise ValueError(
             "Proprietary definition dict must contains a name key with a custom class name"
         )
     if not params["vendor_id"]:
         raise ValueError("Vendor ID is mandatory")
     if not isinstance(params["properties"], dict):
```

### Comparing `BAC0-22.9.21/BAC0/core/utils/notes.py` & `BAC0-23.7.3/BAC0/core/utils/notes.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,35 +2,36 @@
 """
 Notes and logger decorator to be used on class
 This will add a "notes" object to the class and will allow
 logging feature at the same time.
 Goal is to be able to access quickly to important informations for
 the web interface.
 """
-# --- standard Python modules ---
-from collections import namedtuple
-from datetime import datetime
 import logging
-from logging import FileHandler
+import os
 import sys
+import typing as t
 
-import os
+# --- standard Python modules ---
+from collections import namedtuple
+from datetime import datetime
+from logging import FileHandler, Logger
 from os.path import expanduser, join
 
 # --- 3rd party modules ---
 try:
     import pandas as pd
 
     _PANDAS = True
 except ImportError:
     _PANDAS = False
 
 
 class LogList:
-    LOGGERS = []
+    LOGGERS: t.List[Logger] = []
 
 
 def convert_level(level):
     if not level:
         return None
     _valid_levels = [
         logging.DEBUG,
```

### Comparing `BAC0-22.9.21/BAC0/db/influxdb.py` & `BAC0-23.7.3/BAC0/db/influxdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 try:
     from influxdb_client import InfluxDBClient, Point, WriteOptions
-
+    from influxdb_client.client.write import WriteApi
 except ImportError:
     raise ImportError("Install influxdb to use this feature")
 
 import pytz
-from datetime import datetime
 
 
 class InfluxDB:
     """
     Connection to InfluxDB to write to DB or to read from it
     """
 
@@ -17,15 +16,16 @@
     port = 8086
     token = None
     org = None
     bucket = None
     tags_file = None
     username = None
     password = None
-    client = None
+    client: InfluxDBClient
+    write_api: WriteApi
 
     def __init__(self, params):
         # params should be a dict with name=InfluxDB and bucket=valid_bucket_to_use.
         # optional params : url, port, token and org may be provided
         # if they are not provided, BAC0 will try to get them from environment
         # variables that shoudl have been provided in a .env file, which is loaded
         # when BAC0 is imported.
@@ -173,15 +173,15 @@
                         "description",
                         "units_state",
                         "object",
                         "device",
                         "device_id",
                     ],
                 )
-            except Exception as error:
+            except Exception:
                 # print('Oups', _name, error)
                 continue
 
     def read_last_value_from_db(self, id=None):
         # example id : Device_5004/analogInput:1
         # maybe use device name and object name ?
         # This must be easy
```

### Comparing `BAC0-22.9.21/BAC0/db/sql.py` & `BAC0-23.7.3/BAC0/db/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
-sql.py - 
+sql.py -
 """
 
+import contextlib
+import os.path
+
 # --- standard Python modules ---
 import pickle
-import os.path
 
 # --- 3rd party modules ---
 import sqlite3
-import contextlib
 
 try:
     import pandas as pd
-    from pandas.io import sql
     from pandas.core.base import DataError
+    from pandas.io import sql
 
     try:
         from pandas import Timestamp
     except ImportError:
         from pandas.lib import Timestamp
     _PANDAS = True
 except ImportError:
     _PANDAS = False
 
-from ..core.io.IOExceptions import RemovedPointException, NoResponseFromController
+from ..core.io.IOExceptions import NoResponseFromController, RemovedPointException
 
 # --- this application's modules ---
 
 # ------------------------------------------------------------------------------
 
 
 class SQLMixin(object):
@@ -267,15 +268,15 @@
         points = self._read_from_sql("SELECT * FROM history;", db_name)
         return list(points.columns.values)[1:]
 
     def his_from_sql(self, db_name, point):
         """
         Retrive point histories from SQL database
         """
-        his = self._read_from_sql('select * from "{}"'.format("history", db_name))
+        his = self._read_from_sql('select * from "{}"'.format("history"), db_name)
         his.index = his["index"].apply(Timestamp)
         return his.set_index("index")[point]
 
     def value_from_sql(self, db_name, point):
         """
         Take last known value as the value
         """
```

### Comparing `BAC0-22.9.21/BAC0/scripts/Base.py` & `BAC0-23.7.3/BAC0/scripts/Base.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,28 +17,29 @@
 Class::
     BasicScript(WhoisIAm)
         def startApp()
         def stopApp()
 """
 import random
 import sys
+import typing as t
 
 # --- standard Python modules ---
 from threading import Thread
 
-from bacpypes.basetypes import DeviceStatus, ServicesSupported
+from bacpypes.basetypes import DeviceStatus
 from bacpypes.core import enable_sleeping
 from bacpypes.core import run as startBacnetIPApp
 from bacpypes.core import stop as stopBacnetIPApp
 from bacpypes.local.device import LocalDeviceObject
+from bacpypes.pdu import Address
 from bacpypes.primitivedata import CharacterString
 
-from .. import infos
-
 # --- this application's modules ---
+from .. import infos
 from ..core.app.ScriptApplication import (
     BAC0Application,
     BAC0BBMDDeviceApplication,
     BAC0ForeignDeviceApplication,
 )
 from ..core.functions.GetIPAddr import validate_ip_address
 from ..core.functions.TimeSync import TimeHandler
@@ -77,46 +78,52 @@
             item = self.device.this_application.get_object_name(name)
         if item is None:
             raise UnknownObjectError("Can't find {} in local device".format(obj))
         else:
             return item
 
 
+def charstring(val):
+    return CharacterString(val) if isinstance(val, str) else val
+
+
 @note_and_log
 class Base:
     """
     Build a running BACnet/IP device that accepts WhoIs and IAm requests
     Initialization requires some minimial information about the local device.
 
     :param localIPAddr='127.0.0.1':
     :param localObjName='BAC0':
     :param deviceId=None:
     :param maxAPDULengthAccepted='1024':
     :param maxSegmentsAccepted='1024':
     :param segmentationSupported='segmentedBoth':
     """
 
-    _used_ips = set()
+    _used_ips: t.Set[Address] = set()
 
     def __init__(
         self,
         localIPAddr="127.0.0.1",
+        networkNumber=None,
         localObjName="BAC0",
         deviceId=None,
         firmwareRevision="".join(sys.version.split("|")[:2]),
         maxAPDULengthAccepted="1024",
         maxSegmentsAccepted="1024",
         segmentationSupported="segmentedBoth",
         bbmdAddress=None,
         bbmdTTL=0,
         bdtable=None,
-        modelName=CharacterString("BAC0 Scripting Tool"),
+        modelName="BAC0 Scripting Tool",
         vendorId=842,
-        vendorName=CharacterString("SERVISYS inc."),
-        description=CharacterString("http://christiantremblay.github.io/BAC0/"),
+        vendorName="SERVISYS inc.",
+        description="http://christiantremblay.github.io/BAC0/",
+        location="Bromont, Québec",
         spin=None,
     ):
 
         self._log.debug("Configurating app")
 
         self.timehandler = TimeHandler()
 
@@ -145,31 +152,33 @@
             self.localIPAddr = localIPAddr
         else:
             raise InitializationError(
                 "IP Address provided ({}) invalid. Check if another software is using port 47808 on this network interface. If so, you can define multiple IP per interface. Or specify another IP using BAC0.lite(ip='IP/mask')".format(
                     localIPAddr
                 )
             )
+        self.networkNumber = networkNumber
 
         self.Boid = (
             int(deviceId) if deviceId else (3056177 + int(random.uniform(0, 1000)))
         )
 
         self.segmentationSupported = segmentationSupported
         self.maxSegmentsAccepted = maxSegmentsAccepted
         self.localObjName = localObjName
         self.local_objects = LocalObjects(device=self)
 
         self.maxAPDULengthAccepted = maxAPDULengthAccepted
         self.vendorId = vendorId
-        self.vendorName = vendorName
-        self.modelName = modelName
-        self.description = description
+        self.vendorName = charstring(vendorName)
+        self.modelName = charstring(modelName)
+        self.description = charstring(description)
+        self.location = charstring(location)
 
-        self.discoveredDevices = None
+        self.discoveredDevices: t.Optional[t.Dict[t.Tuple[str, int], int]] = None
         self.systemStatus = DeviceStatus(1)
 
         self.bbmdAddress = bbmdAddress
         self.bbmdTTL = bbmdTTL
         self.bdtable = bdtable
 
         self.firmwareRevision = firmwareRevision
@@ -191,54 +200,59 @@
         """
         self._log.debug("Create Local Device")
         try:
             # make a device object
             self.this_device = LocalDeviceObject(
                 objectName=self.localObjName,
                 objectIdentifier=self.Boid,
+                maxSegmentsAccepted=int(self.maxSegmentsAccepted),
                 maxApduLengthAccepted=int(self.maxAPDULengthAccepted),
                 segmentationSupported=self.segmentationSupported,
                 vendorIdentifier=self.vendorId,
                 vendorName=self.vendorName,
                 modelName=self.modelName,
                 systemStatus=self.systemStatus,
                 description=self.description,
+                location=self.location,
                 firmwareRevision=self.firmwareRevision,
                 applicationSoftwareVersion=infos.__version__,
                 protocolVersion=1,
                 protocolRevision=0,
                 utcOffset=self.timehandler.utcOffset(),
                 daylightSavingsStatus=self.timehandler.is_dst(),
             )
 
             # make an application
             if self.bdtable:
                 self.this_application = BAC0BBMDDeviceApplication(
                     self.this_device,
                     self.localIPAddr,
+                    networkNumber=self.networkNumber,
                     bdtable=self.bdtable,
                     iam_req=self._iam_request(),
                     subscription_contexts=self.subscription_contexts,
                 )
                 app_type = "BBMD Device"
             elif self.bbmdAddress and self.bbmdTTL > 0:
 
                 self.this_application = BAC0ForeignDeviceApplication(
                     self.this_device,
                     self.localIPAddr,
+                    networkNumber=self.networkNumber,
                     bbmdAddress=self.bbmdAddress,
                     bbmdTTL=self.bbmdTTL,
                     iam_req=self._iam_request(),
                     subscription_contexts=self.subscription_contexts,
                 )
                 app_type = "Foreign Device"
             else:
                 self.this_application = BAC0Application(
                     self.this_device,
                     self.localIPAddr,
+                    networkNumber=self.networkNumber,
                     iam_req=self._iam_request(),
                     subscription_contexts=self.subscription_contexts,
                 )
                 app_type = "Simple BACnet/IP App"
             self._log.debug("Starting")
             self._initialized = True
             try:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `BAC0-22.9.21/BAC0/scripts/Complete.py` & `BAC0-23.7.3/BAC0/scripts/Complete.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,34 +17,35 @@
 
 Once the class is created, create the local object and use it::
 
     bacnet = ReadWriteScript(localIPAddr = '192.168.1.10')
     bacnet.read('2:5 analogInput 1 presentValue)
 
 """
-# --- standard Python modules ---
-from datetime import datetime
 import logging
-import pandas as pd
 import time
+import typing as t
+
+# --- standard Python modules ---
+from datetime import datetime
 
+import pandas as pd
 
 # --- 3rd party modules ---
 from bokeh.application import Application
 
-# --- this application's modules ---
-from ..scripts.Lite import Lite
-
 from ..core.io.IOExceptions import (
     BokehServerCantStart,
     NoResponseFromController,
     UnrecognizedService,
 )
 from ..core.utils.notes import note_and_log, update_log_level
 
+# --- this application's modules ---
+from ..scripts.Lite import Lite
 from ..web.BokehRenderer import (
     DevicesTableHandler,
     DynamicPlotHandler,
     NotesTableHandler,
 )
 from ..web.BokehServer import Bokeh_Worker
 from ..web.FlaskServer import FlaskServer
@@ -57,17 +58,15 @@
     Statistics used by Flask App
     """
 
     @property
     def number_of_devices(self):
         if not self.discoveredDevices:
             return 0
-        s = []
-        [s.append(x) for x in self.discoveredDevices.items() if x[1] > 0]
-        return len(s)
+        return len([x for x in self.discoveredDevices.items() if x[1] > 0])
 
     @property
     def number_of_registered_trends(self):
         if self.trends:
             return len(self.trends)
         else:
             return 0
@@ -101,15 +100,15 @@
         return s
 
     @property
     def network_stats(self):
         """
         Used by Flask to show informations on the network
         """
-        statistics = {}
+        statistics: t.Dict[str, t.Any] = {}
         mstp_networks = []
         mstp_map = {}
         ip_devices = []
         bacoids = []
         mstp_devices = []
         if self.discoveredDevices:
             for address, bacoid in self.discoveredDevices.keys():
@@ -186,15 +185,15 @@
         else:
             self._log.warning("Bokeh server not started. Trend feature will not work")
         self.discover()
 
     @property
     def devices(self):
         lst = []
-        for device in list(self.discoveredDevices):
+        for device in list(self.discoveredDevices or {}):
             try:
                 deviceName, vendorName = self.readMultiple(
                     "{} device {} objectName vendorName".format(device[0], device[1])
                 )
             except UnrecognizedService:
                 deviceName = self.read(
                     "{} device {} objectName".format(device[0], device[1])
@@ -248,15 +247,15 @@
         except OSError as error:
             self.bokehserver = False
             self._log.error(
                 "[bokeh serve] required for trending (controller.chart) features"
             )
             self._log.error(error)
 
-        except RuntimeError as rterror:
+        except RuntimeError:
             self.bokehserver = False
             self._log.warning("Server already running")
 
         except BokehServerCantStart:
             self.bokehserver = False
             self._log.error("No Bokeh Server - controller.chart not available")
```

### Comparing `BAC0-22.9.21/BAC0/scripts/Lite.py` & `BAC0-23.7.3/BAC0/scripts/Lite.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,55 +17,52 @@
 
 Once the class is created, create the local object and use it::
 
     bacnet = ReadWriteScript(localIPAddr = '192.168.1.10')
     bacnet.read('2:5 analogInput 1 presentValue)
 
 """
+import typing as t
+
 # --- standard Python modules ---
-import time
-from datetime import datetime
 import weakref
 from collections import namedtuple
 
-
-# --- this application's modules ---
-from ..scripts.Base import Base
-
-from ..core.io.Read import ReadProperty
-from ..core.io.Write import WriteProperty
-from ..core.functions.GetIPAddr import HostIP
+from ..core.devices.Device import RPDeviceConnected, RPMDeviceConnected
+from ..core.devices.Points import Point
+from ..core.devices.Trends import TrendLog
+from ..core.devices.Virtuals import VirtualPoint
+from ..core.functions.Calendar import Calendar
+from ..core.functions.cov import CoV
+from ..core.functions.DeviceCommunicationControl import DeviceCommunicationControl
 from ..core.functions.Discover import Discover
-from ..core.functions.TimeSync import TimeSync
+from ..core.functions.GetIPAddr import HostIP
 from ..core.functions.Reinitialize import Reinitialize
-from ..core.functions.DeviceCommunicationControl import DeviceCommunicationControl
-from ..core.functions.cov import CoV
 from ..core.functions.Schedule import Schedule
-from ..core.functions.Calendar import Calendar
 from ..core.functions.Text import TextMixin
-from ..core.io.Simulate import Simulation
-from ..core.devices.Points import Point
-from ..core.devices.Device import RPDeviceConnected, RPMDeviceConnected
-from ..core.devices.Trends import TrendLog
-from ..core.devices.Virtuals import VirtualPoint
-from ..core.utils.notes import note_and_log
+from ..core.functions.TimeSync import TimeSync
 from ..core.io.IOExceptions import (
     NoResponseFromController,
-    UnrecognizedService,
-    Timeout,
     NumerousPingFailures,
+    Timeout,
+    UnrecognizedService,
 )
+from ..core.io.Read import ReadProperty
+from ..core.io.Simulate import Simulation
+from ..core.io.Write import WriteProperty
+from ..core.utils.notes import note_and_log
+from ..infos import __version__ as version
 
+# --- this application's modules ---
+from ..scripts.Base import Base
 from ..tasks.RecurringTask import RecurringTask
 from ..tasks.UpdateCOV import Update_local_COV
 
-from ..infos import __version__ as version
-
 try:
-    from ..db.influxdb import InfluxDB, ConnectionError
+    from ..db.influxdb import ConnectionError, InfluxDB
 
     INFLUXDB = True
 except ImportError:
     INFLUXDB = False
 
 from bacpypes.pdu import Address
 
@@ -96,25 +93,25 @@
     :param ip='127.0.0.1': Address must be in the same subnet as the BACnet network
         [BBMD and Foreign Device - not supported]
 
     """
 
     def __init__(
         self,
-        ip=None,
-        port=None,
-        mask=None,
+        ip: t.Optional[str] = None,
+        port: t.Optional[int] = None,
+        mask: t.Optional[int] = None,
         bbmdAddress=None,
-        bbmdTTL=0,
+        bbmdTTL: int = 0,
         bdtable=None,
-        ping=True,
-        ping_delay=300,
-        db_params=None,
-        **params
-    ):
+        ping: bool = True,
+        ping_delay: int = 300,
+        db_params: t.Optional[t.Dict[str, t.Any]] = None,
+        **params,
+    ) -> None:
         self._log.info(
             "Starting BAC0 version {} ({})".format(
                 version, self.__module__.split(".")[-1]
             )
         )
         self._log.info("Use BAC0.log_level to adjust verbosity of the app.")
         self._log.info("Ex. BAC0.log_level('silence') or BAC0.log_level('error')")
@@ -133,35 +130,40 @@
         if ip is None:
             host = HostIP(port)
             ip_addr = host.address
         else:
             try:
                 ip, subnet_mask_and_port = ip.split("/")
                 try:
-                    mask, port = subnet_mask_and_port.split(":")
+                    mask_s, port_s = subnet_mask_and_port.split(":")
+                    mask = int(mask_s)
+                    port = int(port_s)
                 except ValueError:
-                    mask = subnet_mask_and_port
+                    mask = int(subnet_mask_and_port)
             except ValueError:
                 ip = ip
 
             if not mask:
                 mask = 24
             if not port:
                 port = 47808
             ip_addr = Address("{}/{}:{}".format(ip, mask, port))
-        self._log.info("Using ip : {ip_addr}".format(ip_addr=ip_addr))
+        self._log.info(
+            f"Using ip : {ip_addr} on port {ip_addr.addrPort} | broadcast : {ip_addr.addrBroadcastTuple[0]}"
+        )
+
         Base.__init__(
             self,
             localIPAddr=ip_addr,
             bbmdAddress=bbmdAddress,
             bbmdTTL=bbmdTTL,
             bdtable=bdtable,
-            **params
+            **params,
         )
-
+        self._log.info("Device instance (id) : {boid}".format(boid=self.Boid))
         self.bokehserver = False
         self._points_to_trend = weakref.WeakValueDictionary()
 
         # Announce yourself
         self.iam()
 
         # Do what's needed to support COV
@@ -169,15 +171,15 @@
             "_update_local_cov_task", ["task", "running"]
         )
         self._update_local_cov_task.task = Update_local_COV(
             self, delay=1, name="Update Local COV Task"
         )
         self._update_local_cov_task.task.start()
         self._update_local_cov_task.running = True
-        self._log.info("Update Local COV Task started")
+        self._log.info("Update Local COV Task started (required to support COV)")
 
         # Activate InfluxDB if params are available
         if db_params and INFLUXDB:
             try:
                 self.database = (
                     InfluxDB(db_params)
                     if db_params["name"].lower() == "influxdb"
@@ -201,20 +203,27 @@
         and add any network number that would not be in the NSE table.
         """
         if self.discoveredDevices:
             for each in self.discoveredDevices:
                 addr, instance = each
                 net = addr.split(":")[0] if ":" in addr else None
                 if net:
-                    self.this_application.nse._learnedNetworks.add(int(net))
+                    try:
+                        self.this_application.nse._learnedNetworks.add(int(net))
+                    except ValueError:
+                        pass  # proabbly a IP address with a specified port other than 0xBAC0
 
         return self.this_application.nse._learnedNetworks
 
     def discover(
-        self, networks="known", limits=(0, 4194303), global_broadcast=False, reset=False
+        self,
+        networks: t.Union[str, t.List[int], int] = "known",
+        limits: t.Tuple[int, int] = (0, 4194303),
+        global_broadcast: bool = False,
+        reset: bool = False,
     ):
         """
         Discover is meant to be the function used to explore the network when we
         connect.
         It will trigger whois request using the different options provided with
         parameters.
 
@@ -237,15 +246,15 @@
         :param networks (list, integer) : A simple integer or a list of integer
             representing the network numbers used to issue whois request.
 
         :param limits (tuple) : tuple made of 2 integer, the low limit and the high
             limit. Those are the device instances used in the creation of the
             whois request. Min : 0 ; Max : 4194303
 
-        :param global_broadcast (boolean) : If set to true, a global braodcast
+        :param global_broadcast (boolean) : If set to true, a global broadcast
             will be used for the whois. Use with care.
         """
         if reset:
             self.discoveredDevices = None
         found = []
         _networks = []
         deviceInstanceRangeLowLimit, deviceInstanceRangeHighLimit = limits
@@ -260,15 +269,15 @@
                 # we'll make multiple whois...
                 for network in networks:
                     if network < 65535:
                         _networks.append(network)
             elif networks == "known":
                 _networks = self.known_network_numbers.copy()
             else:
-                if networks < 65535:
+                if isinstance(networks, int) and networks < 65535:
                     _networks.append(networks)
 
         if _networks:
             for network in _networks:
                 self._log.info("Discovering network {}".format(network))
                 _res = self.whois(
                     "{}:* {} {}".format(
@@ -293,19 +302,21 @@
                 ),
                 global_broadcast=global_broadcast,
             )
             for each in _res:
                 found.append(each)
         return found
 
-    def register_device(self, device):
+    def register_device(
+        self, device: t.Union[RPDeviceConnected, RPMDeviceConnected]
+    ) -> None:
         oid = id(device)
         self._registered_devices[oid] = device
 
-    def ping_registered_devices(self):
+    def ping_registered_devices(self) -> None:
         """
         Registered device on a network (self) are kept in a list (registered_devices).
         This function will allow pinging thoses device regularly to monitor them. In case
         of disconnected devices, we will disconnect the device (which will save it). Then
         we'll ping again until reconnection, where the device will be bring back online.
 
         To permanently disconnect a device, an explicit device.disconnect(unregister=True [default value])
@@ -361,32 +372,34 @@
         """
         oid = id(device)
         try:
             del self._registered_devices[oid]
         except KeyError:
             pass
 
-    def add_trend(self, point_to_trend):
+    def add_trend(self, point_to_trend: t.Union[Point, TrendLog, VirtualPoint]) -> None:
         """
         Add point to the list of histories that will be handled by Bokeh
 
         Argument provided must be of type Point or TrendLog
         ex. bacnet.add_trend(controller['point_name'])
         """
         if (
             isinstance(point_to_trend, Point)
             or isinstance(point_to_trend, TrendLog)
-            or (isinstance(point_to_trend, VirtualPoint))
+            or isinstance(point_to_trend, VirtualPoint)
         ):
             oid = id(point_to_trend)
             self._points_to_trend[oid] = point_to_trend
         else:
             raise TypeError("Please provide point containing history")
 
-    def remove_trend(self, point_to_remove):
+    def remove_trend(
+        self, point_to_remove: t.Union[Point, TrendLog, VirtualPoint]
+    ) -> None:
         """
         Remove point from the list of histories that will be handled by Bokeh
 
         Argument provided must be of type Point or TrendLog
         ex. bacnet.remove_trend(controller['point_name'])
         """
         if (
@@ -397,24 +410,24 @@
             oid = id(point_to_remove)
         else:
             raise TypeError("Please provide point or trendLog containing history")
         if oid in self._points_to_trend.keys():
             del self._points_to_trend[oid]
 
     @property
-    def devices(self):
+    def devices(self) -> t.List[t.Tuple[str, str, str, int]]:
         """
         This property will create a good looking table of all the discovered devices
         seen on the network.
 
         For that, some requests will be sent over the network to look for name,
         manufacturer, etc and in big network, this could be a long process.
         """
         lst = []
-        for device in list(self.discoveredDevices):
+        for device in list(self.discoveredDevices or {}):
             try:
                 deviceName, vendorName = self.readMultiple(
                     "{} device {} objectName vendorName".format(device[0], device[1])
                 )
             except (UnrecognizedService, ValueError):
                 self._log.warning(
                     "Unrecognized service for {} | {}".format(device[0], device[1])
@@ -429,30 +442,30 @@
                 except NoResponseFromController:
                     self._log.warning("No response from {}".format(device))
                     continue
             except (NoResponseFromController, Timeout):
                 self._log.warning("No response from {}".format(device))
                 continue
             lst.append((deviceName, vendorName, device[0], device[1]))
-        return lst
+        return lst  # type: ignore[return-value]
 
     @property
-    def trends(self):
+    def trends(self) -> t.List[t.Any]:
         """
         This will present a list of all registered trends used by Bokeh Server
         """
         return list(self._points_to_trend.values())
 
-    def disconnect(self):
+    def disconnect(self) -> None:
         self._log.debug("Disconnecting")
         for each in self.registered_devices:
             each.disconnect()
         super().disconnect()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "Bacnet Network using ip {} with device id {}".format(
             self.localIPAddr, self.Boid
         )
 
     def __getitem__(self, boid_or_localobject):
         item = self.this_application.objectName[boid_or_localobject]
         if item is None:
```

### Comparing `BAC0-22.9.21/BAC0/tasks/Devices.py` & `BAC0-23.7.3/BAC0/tasks/Devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
-"""
-Match.py - verify a point's status matches its commanded value.
-
-Example:
-    Is a fan commanded to 'On' actually 'running'?
-"""
 
 # --- standard Python modules ---
 # --- 3rd party modules ---
 
+from ..core.devices.Device import Device
+from ..core.io.IOExceptions import BadDeviceDefinition
+
 # --- this application's modules ---
 from .TaskManager import Task
-from ..core.io.IOExceptions import BadDeviceDefinition
-from ..core.devices.Device import Device
-from ..core.utils.notes import note_and_log
 
 """
 A way to define a BAC0.device using a task, so it won't block the Notebook or the REPL
 """
 
 
 class AddDevice(Task):
```

### Comparing `BAC0-22.9.21/BAC0/tasks/DoOnce.py` & `BAC0-23.7.3/BAC0/tasks/DoOnce.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
 DoOnce.py - execute a task once
 """
 
-from .TaskManager import OneShotTask
 from ..core.utils.notes import note_and_log
+from .TaskManager import OneShotTask
 
 
 @note_and_log
 class DoOnce(OneShotTask):
     """
     Start a polling task which is in fact a recurring read of the point.
     ex.
```

### Comparing `BAC0-22.9.21/BAC0/tasks/Match.py` & `BAC0-23.7.3/BAC0/tasks/Match.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 Example:
     Is a fan commanded to 'On' actually 'running'?
 """
 
 # --- standard Python modules ---
 # --- 3rd party modules ---
 
+from ..core.utils.notes import note_and_log
+
 # --- this application's modules ---
 from .TaskManager import Task
-from ..core.utils.notes import note_and_log
 
 # ------------------------------------------------------------------------------
 
 
 @note_and_log
 class Match(Task):
     """
```

### Comparing `BAC0-22.9.21/BAC0/tasks/Poll.py` & `BAC0-23.7.3/BAC0/tasks/Poll.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,38 +4,42 @@
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
 Poll.py - create a Polling task to repeatedly read a point.
 """
 
+import typing as t
+
 # --- standard Python modules ---
 import weakref
 
-# --- 3rd party modules ---
-from bacpypes.core import deferred
+from ..core.utils.notes import note_and_log
 
 # --- this application's modules ---
 from .TaskManager import Task
-from ..core.utils.notes import note_and_log
+
+if t.TYPE_CHECKING:
+    from ..core.devices.Device import RPDeviceConnected, RPMDeviceConnected
+
 
 # ------------------------------------------------------------------------------
 class MultiplePollingFailures(Exception):
     pass
 
 
 @note_and_log
 class SimplePoll(Task):
     """
     Start a polling task to repeatedly read a point's Present_Value.
     ex.
         device['point_name'].poll(delay=60)
     """
 
-    def __init__(self, point, *, delay=10):
+    def __init__(self, point, *, delay: int = 10) -> None:
         """
         :param point: (BAC0.core.device.Points.Point) name of the point to read
         :param delay: (int) Delay between reads in seconds, defaults = 10sec
 
         A delay cannot be < 1sec
         This task is meant for single points, so BAC0 will allow short delays.
         This way, a fast polling is available for some points in a device that
@@ -58,15 +62,21 @@
 @note_and_log
 class DevicePoll(Task):
     """
     Start a polling task to repeatedly read a list of points from a device using
     ReadPropertyMultiple requests.
     """
 
-    def __init__(self, device, delay=10, name="", prefix="basic_poll"):
+    def __init__(
+        self,
+        device: t.Union["RPMDeviceConnected", "RPDeviceConnected"],
+        delay: int = 10,
+        name: str = "",
+        prefix: str = "basic_poll",
+    ) -> None:
         """
         :param device: (BAC0.core.devices.Device.Device) device to poll
         :param delay: (int) Delay between polls in seconds, defaults = 10sec
 
         A delay cannot be < 10sec
         For delays under 10s, use DeviceFastPoll class.
 
@@ -75,18 +85,18 @@
         self.failures = 0
         self.MAX_FAILURES = 3
         self._device = weakref.ref(device)
         Task.__init__(self, name="{}_{}".format(prefix, name), delay=delay)
         self._counter = 0
 
     @property
-    def device(self):
+    def device(self) -> t.Union["RPMDeviceConnected", "RPDeviceConnected", None]:
         return self._device()
 
-    def task(self):
+    def task(self) -> None:
         if self.device.properties.ping_failures > 0:
             self.device._log.warning(
                 "{} ({}) | Ping failed, skipping polling for now. Resending a ping to speed up things".format(
                     self.device.properties.name, self.device.properties.address
                 )
             )
             self.device.ping()
```

### Comparing `BAC0-22.9.21/BAC0/tasks/RecurringTask.py` & `BAC0-23.7.3/BAC0/tasks/RecurringTask.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
-RecurringTask.py - execute a recurring task 
+RecurringTask.py - execute a recurring task
 """
 
-from .TaskManager import Task
+from typing import Any, Callable, Tuple, Union
+
 from ..core.utils.notes import note_and_log
+from .TaskManager import Task
 
 
 @note_and_log
 class RecurringTask(Task):
     """
     Start a recurring task (a function passed)
     """
 
-    def __init__(self, fnc, delay=60, name="recurring"):
+    def __init__(
+        self,
+        fnc: Union[Tuple[Callable, Any], Callable],
+        delay: int = 60,
+        name: str = "recurring",
+    ) -> None:
         """
         :param fnc: a function or a tuple (function, args)
         :param delay: (int) Delay between reads executions
 
         :returns: Nothing
         """
         self.fnc_args = None
@@ -32,12 +39,12 @@
             self.func = fnc
         else:
             raise ValueError(
                 "You must pass a function or a tuple (function,args) to this..."
             )
         Task.__init__(self, name=name, delay=delay)
 
-    def task(self):
+    def task(self) -> None:
         if self.fnc_args:
             self.func(self.fnc_args)
         else:
             self.func()
```

### Comparing `BAC0-22.9.21/BAC0/tasks/TaskManager.py` & `BAC0-23.7.3/BAC0/tasks/TaskManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 #
 """
-TaskManager.py - creation of threads used for repetitive tasks.  
+TaskManager.py - creation of threads used for repetitive tasks.
 
 A key building block for point simulation.
 """
-# --- standard Python modules ---
-from threading import Thread, Lock
 import time
-from collections import deque
 from random import random
 
+# --- standard Python modules ---
+from threading import Thread
+
+from ..core.io.IOExceptions import DeviceNotConnected
 
 # --- 3rd party modules ---
 # --- this application's modules ---
 from ..core.utils.notes import note_and_log
-from ..core.io.IOExceptions import DeviceNotConnected
 
 # ------------------------------------------------------------------------------
 
 
 @note_and_log
 class Manager:
     tasks = []
@@ -58,15 +58,17 @@
                         "Task {} | {} executed. {}".format(task.id, task.name, task)
                     )
             except IndexError:
                 cls._log.debug("Task Manager waiting for tasks...")
                 time.sleep(1)
             except DeviceNotConnected as error:
                 cls._log.warning(
-                    "Device disconnected. Removing task ({}).".format(error, task)
+                    "Device disconnected with error {}. Removing task ({}).".format(
+                        error, task
+                    )
                 )
                 cls.tasks.remove(task.id)
             except Exception as error:
                 if task.name == "Ping Task":
                     cls._log.warning(
                         "Ping failed with error {} ({}).".format(error, task)
                     )
@@ -146,15 +148,15 @@
             self.delay = delay if delay >= 5 else 5
         else:
             self.delay = 0
         self.previous_execution = None
         self.average_execution_delay = 0
         self.average_latency = 0
         self.next_execution = time.time() + delay + (random() * 10)
-        self.execution_time = 0
+        self.execution_time = 0.0
         self.count = 0
         self.id = id(self)
         self._kwargs = None
         Task._tasks.append(self)
 
     def task(self):
         raise NotImplementedError("Must be implemented")
@@ -167,15 +169,15 @@
         ) / 2
         if self.fn and self.args is not None:
             self.fn(self.args)
         elif self.fn:
             self.fn()
         else:
             if self._kwargs is not None:
-                self.task(self._kwargs)
+                self.task(**self._kwargs)
             else:
                 self.task()
         if self.previous_execution:
             _total = self.average_execution_delay + (
                 _start_time - self.previous_execution
             )
             self.average_execution_delay = _total / 2
```

### Comparing `BAC0-22.9.21/BAC0/tasks/UpdateCOV.py` & `BAC0-23.7.3/BAC0/tasks/UpdateCOV.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # --- standard Python modules ---
 import weakref
 
 # --- 3rd party modules ---
 from bacpypes.core import deferred
 
+from ..core.utils.notes import note_and_log
+
 # --- this application's modules ---
 from .TaskManager import Task
-from ..core.utils.notes import note_and_log
 
 
 @note_and_log
 class Update_local_COV(Task):
     """
     Start a task to validate each points inside local device and send
     cov notifications to subscribers.
```

### Comparing `BAC0-22.9.21/BAC0/tools/const.py` & `BAC0-23.7.3/BAC0/tools/const.py`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/tools/tad_display.py` & `BAC0-23.7.3/BAC0/tools/tad_display.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,18 @@
+import typing as t
+
 from . import const
 
 FILE_HEADER = const.FILE_HEADER
 FILE_FOOTER = const.FILE_FOOTER
 TAG = const.TAG
 
-template_example = {
-    "names": [("name", "dev_id")],
-}
-
 
-def convert(d, device_name=None, make_template=False):
-    """
-    Template : If true, will not populate name and device id so the file
-    can be reused to create a dictionnary in T3 Studio with multiple
-    devices. This will prevents us from switching dictionnary all the time.
-    """
+def convert(d, device_name=None):
     list_of_tags = []
-    device_id = None
     OBJECT_TYPE = {
         "analogValue": "AV",
         "analogInput": "AI",
         "analogOutput": "AO",
         "binaryInput": "BI",
         "binaryValue": "BV",
         "binaryOutput": "BO",
@@ -48,63 +40,37 @@
         "BO": 8,
         "BV": 10,
         "MI": 0,
         "MO": 8,
         "MV": 10,
     }
 
-    if make_template:
-        device_name = "$DEVICE_NAME"
-        device_id = "$DEVICE_ID"
-
-    data = {}
     for each in d.points:
+        data: t.Dict[str, t.Union[str, int]] = {}
         name = device_name if device_name else d.properties.name
+        obj_type = OBJECT_TYPE[each.properties.type]
         data["name"] = "{}/{}".format(name, each.properties.name)
         data["group"] = ""
-        data["object_type"] = OBJECT_TYPE[each.properties.type]
+        data["object_type"] = obj_type
         data["object_instance"] = each.properties.address
-        data["device_id"] = device_id if device_id else d.properties.device_id
-        data["data_type"] = DATATYPES[data["object_type"]]
+        data["device_id"] = d.properties.device_id
+        data["data_type"] = DATATYPES[obj_type]
         data["object_property"] = 85
-        data["write_priority"] = WRITE_PRIORITY[data["object_type"]]
+        data["write_priority"] = WRITE_PRIORITY[obj_type]
         data["cov"] = "false"
         data["refresh_time"] = 1000
         data["access_mode"] = "READ"
         data["active"] = "false"
         data["comment"] = each.properties.description
         data["array_index"] = -1
         list_of_tags.append(TAG.format(d=data))
 
-    return (name, list_of_tags)
+        file = FILE_HEADER
+        for tag in list_of_tags:
+            file += tag
+        file += FILE_FOOTER
+        write_tags_import_file(name, file)
 
 
-def build_from_templates(list_of_tags, config={}):
-    """
-    Config must be a list of tuple (name, device_id)
-    """
-    _lst_of_tags = []
-    for each in config:
-        name, device_id = each
-        for tag in list_of_tags:
-            if "$DEVICE_NAME" in tag:
-                tag.replace("$DEVICE_NAME", name)
-            if "$DEVICE_ID" in tag:
-                tag.replace("DEVICE_ID", device_id)
-            _lst_of_tags.append(tag)
-    return _lst_of_tags
-
-
-def merge_templates(lst=[]):
-    _lst = []
-    for each in lst:
-        _lst.extend(each)
-    return _lst
-
-
-def write_tags_import_file(name, list_of_tags):
-    _content = FILE_HEADER
-    for tag in list_of_tags:
-        _content += tag
-    _content += FILE_FOOTER
+def write_tags_import_file(name, file):
     with open("{}.xml".format(name), "w") as xml_file:
-        xml_file.write(_content)
+        xml_file.write(file)
```

### Comparing `BAC0-22.9.21/BAC0/web/BokehRenderer.py` & `BAC0-23.7.3/BAC0/web/BokehRenderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,49 +4,37 @@
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 #
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 """
 This module deals with Bokeh Session, Document and Plots
 A connection to the server is mandatory to use update_data
 """
-from bokeh.plotting import Figure
+import weakref
+from queue import Queue
+
+import pandas as pd
+from bokeh.application.handlers import Handler
+from bokeh.io import curdoc
+from bokeh.layouts import column, row
 from bokeh.models import (
     ColumnDataSource,
+    CustomJS,
     HoverTool,
-    Range1d,
-    Label,
-    LabelSet,
-    LinearAxis,
     Legend,
     LegendItem,
-    Dropdown,
+    LinearAxis,
     MultiChoice,
-    CustomJS,
+    Range1d,
 )
-from bokeh.models.widgets import DataTable, TableColumn, Div
-from bokeh.layouts import widgetbox, row, column, gridplot, widgetbox
-from bokeh.palettes import d3, viridis
-from bokeh.io import curdoc
-from bokeh.application.handlers import Handler
-from bokeh.models.tools import CustomJSHover
-
-from functools import partial
-
-from tornado import gen
-
-import math
-import pandas as pd
-import weakref
-from queue import Queue
-from collections import deque
+from bokeh.models.widgets import DataTable, TableColumn
+from bokeh.palettes import d3
+from bokeh.plotting import Figure
 
-from ..tasks.RecurringTask import RecurringTask
-from ..core.utils.notes import note_and_log
 from ..core.devices.Virtuals import VirtualPoint
-from ..core.devices.Trends import TrendLog
+from ..core.utils.notes import note_and_log
 
 
 @note_and_log
 class DynamicPlotHandler(Handler):
 
     analog_queue = Queue()
     binary_queue = Queue()
@@ -190,29 +178,27 @@
         for _, v in self.glyphs["multistates_labels"].items():
             v.visible = False
         for _, v in self.glyphs["virtual"].items():
             v.visible = False
 
     def update_glyphs(self):
         self._log.debug("Updating Glyphs")
-        enumerated_axis_needed = True
         for point in self.network.trends:
             name = "{}/{}".format(
                 point.properties.device.properties.name, point.properties.name
             )
             if "analog" in point.properties.type or "TrendLog" in point.properties.type:
                 self.analog_queue.put(
                     (name, point.properties.description, point.properties.units_state)
                 )
             elif "binary" in point.properties.type:
                 self.binary_queue.put(
                     (name, point.properties.description, point.properties.units_state)
                 )
             elif "multi" in point.properties.type:
-                enumerated_axis_needed = True
                 self.multistates_queue.put(
                     (name, point.properties.description, point.properties.units_state)
                 )
                 self.multistates_label_queue.put(
                     (
                         name + "_state",
                         point.properties.description,
```

### Comparing `BAC0-22.9.21/BAC0/web/BokehServer.py` & `BAC0-23.7.3/BAC0/web/BokehServer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 #
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 #
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 """
 This will start the Bokeh Server
 """
-from threading import Thread
 import weakref
+from threading import Thread
+
 from bokeh.server.server import Server
 from tornado.ioloop import IOLoop
 
 from ..core.utils.notes import note_and_log
 
 
 @note_and_log
```

### Comparing `BAC0-22.9.21/BAC0/web/FlaskServer.py` & `BAC0-23.7.3/BAC0/web/FlaskServer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 #
 # Copyright (C) 2015 by Christian Tremblay, P.Eng <christian.tremblay@servisys.com>
 #
 # Licensed under LGPLv3, see file LICENSE in this source tree.
 """
 This module will start the Flask server 
 """
-from threading import Thread
-import weakref
-import logging
-from flask import Flask, render_template, jsonify, request
-from flask_bootstrap import Bootstrap
 import json
-from bokeh.embed import server_document
+import weakref
+from threading import Thread
 
-from .templates import create_sidebar, create_card, update_notifications
+from bokeh.embed import server_document
+from flask import Flask, jsonify, render_template, request
 from flask.logging import default_handler
+from flask_bootstrap import Bootstrap
+
+from .templates import create_card, create_sidebar, update_notifications
 
 
 class FlaskServer(Thread):
 
     # Init thread running server
     def __init__(self, network, port=8111, ip="0.0.0.0", *, daemon=True):
         Thread.__init__(self, daemon=daemon)
```

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/css/.DS_Store` & `BAC0-23.7.3/BAC0/web/static/assets/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/css/animate.min.css` & `BAC0-23.7.3/BAC0/web/static/assets/css/animate.min.css`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/css/bootstrap.min.css` & `BAC0-23.7.3/BAC0/web/static/assets/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/css/demo.css` & `BAC0-23.7.3/BAC0/web/static/assets/css/demo.css`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/css/paper-dashboard.css` & `BAC0-23.7.3/BAC0/web/static/assets/css/paper-dashboard.css`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/css/themify-icons.css` & `BAC0-23.7.3/BAC0/web/static/assets/css/themify-icons.css`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/fonts/.DS_Store` & `BAC0-23.7.3/BAC0/web/static/assets/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/fonts/themify.eot` & `BAC0-23.7.3/BAC0/web/static/assets/fonts/themify.eot`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/fonts/themify.svg` & `BAC0-23.7.3/BAC0/web/static/assets/fonts/themify.svg`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/fonts/themify.ttf` & `BAC0-23.7.3/BAC0/web/static/assets/fonts/themify.ttf`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/fonts/themify.woff` & `BAC0-23.7.3/BAC0/web/static/assets/fonts/themify.woff`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/.DS_Store` & `BAC0-23.7.3/BAC0/web/static/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/31554.jpg` & `BAC0-23.7.3/BAC0/web/static/assets/img/31554.jpg`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/GitHub-Mark.png` & `BAC0-23.7.3/BAC0/web/static/assets/img/GitHub-Mark.png`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/apple-icon.png` & `BAC0-23.7.3/BAC0/web/static/assets/img/apple-icon.png`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/background/.DS_Store` & `BAC0-23.7.3/BAC0/web/static/assets/img/background/.DS_Store`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/background.jpg` & `BAC0-23.7.3/BAC0/web/static/assets/img/background.jpg`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/bg.png` & `BAC0-23.7.3/BAC0/web/static/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/bg.xcf` & `BAC0-23.7.3/BAC0/web/static/assets/img/bg.xcf`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/devices2.png` & `BAC0-23.7.3/BAC0/web/static/assets/img/devices2.png`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/faces/.DS_Store` & `BAC0-23.7.3/BAC0/web/static/assets/img/faces/.DS_Store`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/faces/face-0.jpg` & `BAC0-23.7.3/BAC0/web/static/assets/img/faces/face-0.jpg`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/faces/face-1.jpg` & `BAC0-23.7.3/BAC0/web/static/assets/img/faces/face-1.jpg`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/faces/face-2.jpg` & `BAC0-23.7.3/BAC0/web/static/assets/img/faces/face-2.jpg`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/faces/face-3.jpg` & `BAC0-23.7.3/BAC0/web/static/assets/img/faces/face-3.jpg`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/favicon.png` & `BAC0-23.7.3/BAC0/web/static/assets/img/favicon.png`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/histories2.png` & `BAC0-23.7.3/BAC0/web/static/assets/img/histories2.png`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/new_logo.png` & `BAC0-23.7.3/BAC0/web/static/assets/img/new_logo.png`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/notes.png` & `BAC0-23.7.3/BAC0/web/static/assets/img/notes.png`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/readthedocs.png` & `BAC0-23.7.3/BAC0/web/static/assets/img/readthedocs.png`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/search.png` & `BAC0-23.7.3/BAC0/web/static/assets/img/search.png`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/tables/.DS_Store` & `BAC0-23.7.3/BAC0/web/static/assets/img/tables/.DS_Store`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/tim_80x80.png` & `BAC0-23.7.3/BAC0/web/static/assets/img/tim_80x80.png`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/img/wordpress.png` & `BAC0-23.7.3/BAC0/web/static/assets/img/wordpress.png`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/js/.DS_Store` & `BAC0-23.7.3/BAC0/web/static/assets/js/.DS_Store`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/js/BAC0_script.js` & `BAC0-23.7.3/BAC0/web/static/assets/js/BAC0_script.js`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/js/bac0.js` & `BAC0-23.7.3/BAC0/web/static/assets/js/bac0.js`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/js/bootstrap-checkbox-radio.js` & `BAC0-23.7.3/BAC0/web/static/assets/js/bootstrap-checkbox-radio.js`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/js/bootstrap-notify.js` & `BAC0-23.7.3/BAC0/web/static/assets/js/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/js/bootstrap.min.js` & `BAC0-23.7.3/BAC0/web/static/assets/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/js/chartist.min.js` & `BAC0-23.7.3/BAC0/web/static/assets/js/chartist.min.js`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/js/demo.js` & `BAC0-23.7.3/BAC0/web/static/assets/js/demo.js`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/js/jquery-1.10.2.js` & `BAC0-23.7.3/BAC0/web/static/assets/js/jquery-1.10.2.js`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/js/paper-dashboard.js` & `BAC0-23.7.3/BAC0/web/static/assets/js/paper-dashboard.js`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/.DS_Store` & `BAC0-23.7.3/BAC0/web/static/assets/sass/.DS_Store`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_alerts.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_alerts.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_buttons.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_buttons.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_cards.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_cards.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_chartist.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_chartist.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_checkbox-radio.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_checkbox-radio.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_dropdown.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_footers.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_footers.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_inputs.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_inputs.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_misc.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_misc.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_navbars.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_navbars.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_responsive.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_responsive.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_sidebar-and-main-panel.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_sidebar-and-main-panel.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_tables.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_tables.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_typography.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_typography.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/_variables.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/_variables.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_buttons.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_chartist.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_chartist.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_labels.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_labels.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_sidebar.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper/mixins/_vendor-prefixes.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper/mixins/_vendor-prefixes.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/static/assets/sass/paper-dashboard.scss` & `BAC0-23.7.3/BAC0/web/static/assets/sass/paper-dashboard.scss`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/templates/base.html` & `BAC0-23.7.3/BAC0/web/templates/base.html`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/templates/dashboard.html` & `BAC0-23.7.3/BAC0/web/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/templates/footer.html` & `BAC0-23.7.3/BAC0/web/templates/footer.html`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/templates/navbar.html` & `BAC0-23.7.3/BAC0/web/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/templates/notifications.html` & `BAC0-23.7.3/BAC0/web/templates/notifications.html`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0/web/templates.py` & `BAC0-23.7.3/BAC0/web/templates.py`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/BAC0.egg-info/PKG-INFO` & `BAC0-23.7.3/BAC0.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BAC0
-Version: 22.9.21
+Version: 23.7.3
 Summary: BACnet Scripting Framework for testing DDC Controls
 Home-page: https://github.com/ChristianTremblay/BAC0
 Download-URL: https://github.com/ChristianTremblay/BAC0/archive/master.zip
 Author: Christian Tremblay, P.Eng.
 Author-email: christian.tremblay@servisys.com
 Keywords: bacnet,building,automation,test
 Classifier: Development Status :: 4 - Beta
```

### Comparing `BAC0-22.9.21/BAC0.egg-info/SOURCES.txt` & `BAC0-23.7.3/BAC0.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 BAC0/core/devices/Virtuals.py
 BAC0/core/devices/__init__.py
 BAC0/core/devices/create_objects.py
 BAC0/core/devices/local/__init__.py
 BAC0/core/devices/local/decorator.py
 BAC0/core/devices/local/models.py
 BAC0/core/devices/local/object.py
+BAC0/core/devices/local/trendLogs.py
 BAC0/core/devices/mixins/CommandableMixin.py
 BAC0/core/devices/mixins/__init__.py
 BAC0/core/devices/mixins/read_mixin.py
 BAC0/core/functions/Calendar.py
 BAC0/core/functions/DeviceCommunicationControl.py
 BAC0/core/functions/Discover.py
 BAC0/core/functions/GetIPAddr.py
@@ -146,8 +147,17 @@
 BAC0/web/templates/dashboard.html
 BAC0/web/templates/device_table.html
 BAC0/web/templates/embed_bck.html
 BAC0/web/templates/footer.html
 BAC0/web/templates/navbar.html
 BAC0/web/templates/notifications.html
 BAC0/web/templates/theme.yaml
-BAC0/web/templates/trends.html
+BAC0/web/templates/trends.html
+tests/test_0BacpypesVersion.py
+tests/test_1AddressesTypes.py
+tests/test_BAC0_lite.py
+tests/test_BAC0_web.py
+tests/test_Read.py
+tests/test_SaveToSQL.py
+tests/test_WhoHasIHave.py
+tests/test_Write.py
+tests/test_proprietaryobjects.py
```

### Comparing `BAC0-22.9.21/LICENSE` & `BAC0-23.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/PKG-INFO` & `BAC0-23.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BAC0
-Version: 22.9.21
+Version: 23.7.3
 Summary: BACnet Scripting Framework for testing DDC Controls
 Home-page: https://github.com/ChristianTremblay/BAC0
 Download-URL: https://github.com/ChristianTremblay/BAC0/archive/master.zip
 Author: Christian Tremblay, P.Eng.
 Author-email: christian.tremblay@servisys.com
 Keywords: bacnet,building,automation,test
 Classifier: Development Status :: 4 - Beta
```

### Comparing `BAC0-22.9.21/README.rst` & `BAC0-23.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `BAC0-22.9.21/setup.py` & `BAC0-23.7.3/setup.py`

 * *Files identical despite different names*

