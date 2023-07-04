# Comparing `tmp/nonebot_plugin_blive_danmaku-0.3.22.tar.gz` & `tmp/nonebot_plugin_blive_danmaku-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blive_danmaku-0.3.22.tar", max compression
+gzip compressed data, was "nonebot_plugin_blive_danmaku-0.3.3.tar", max compression
```

## Comparing `nonebot_plugin_blive_danmaku-0.3.22.tar` & `nonebot_plugin_blive_danmaku-0.3.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.3.22/LICENSE
--rw-r--r--   0        0        0     1027 2023-06-30 08:42:41.437287 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/__init__.py
--rw-r--r--   0        0        0     1610 2023-04-28 07:50:38.274424 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/__init__.py
--rw-r--r--   0        0        0       91 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/_plugin-vue_export-helper-1b428a4d.js
--rw-r--r--   0        0        0   533008 2023-06-26 02:58:12.791659 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/echarts-400b5edd.js
--rw-r--r--   0        0        0   285956 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-2bbb65c2.js
--rw-r--r--   0        0        0   324265 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-5cfbb218.css
--rw-r--r--   0        0        0     9045 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-1-k-823c4f26.png
--rw-r--r--   0        0        0     8799 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-2-k-a0b7be7c.png
--rw-r--r--   0        0        0     7006 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-3-k-3c7bacae.png
--rw-r--r--   0        0        0      902 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/helpDialog-a1deb50e.js
--rw-r--r--   0        0        0     6723 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-10fe5420.js
--rw-r--r--   0        0        0     2787 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-1f52d48f.js
--rw-r--r--   0        0        0    20588 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-3b039937.js
--rw-r--r--   0        0        0     9107 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-4d7b4401.css
--rw-r--r--   0        0        0      703 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-54bfb553.css
--rw-r--r--   0        0        0     3061 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6803b0c6.js
--rw-r--r--   0        0        0      815 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-7bb2b86c.css
--rw-r--r--   0        0        0     5128 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-c1b5ef2f.js
--rw-r--r--   0        0        0      167 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-cd2e8127.css
--rw-r--r--   0        0        0      699 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e7323967.css
--rw-r--r--   0        0        0     3593 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f24fc95e.js
--rw-r--r--   0        0        0     1239 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f9e2a7e5.js
--rw-r--r--   0        0        0       51 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-fe1a4f18.css
--rw-r--r--   0        0        0    20126 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-520df23f.js
--rw-r--r--   0        0        0     6259 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-1-f98dcdbf.png
--rw-r--r--   0        0        0     5886 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-2-abaf3760.png
--rw-r--r--   0        0        0    20334 2023-06-26 02:58:12.784659 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/SC-bg-img-0e2aa755.png
--rw-r--r--   0        0        0      330 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-8f8a299b.css
--rw-r--r--   0        0        0    18870 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-fcb4d4cd.js
--rw-r--r--   0        0        0     1757 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b57f6aba.css
--rw-r--r--   0        0        0   447924 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-fa374c7f.js
--rw-r--r--   0        0        0    12014 2023-04-15 02:38:23.791948 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico
--rw-r--r--   0        0        0      908 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/index.html
--rw-r--r--   0        0        0      200 2023-06-04 10:26:16.056985 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/models.py
--rw-r--r--   0        0        0     4864 2023-06-24 03:21:58.563784 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/router.py
--rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/.git
--rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
--rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/.gitignore
--rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
--rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
--rw-r--r--   0        0        0     7552 2023-06-22 11:19:57.567827 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
--rw-r--r--   0        0        0    13206 2023-06-22 11:29:10.027052 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
--rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/LICENSE
--rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/README.md
--rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
--rw-r--r--   0        0        0     2928 2023-04-24 05:16:11.948995 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/sample.py
--rw-r--r--   0        0        0      136 2023-06-07 09:20:41.977052 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/__init__.py
--rw-r--r--   0        0        0        4 2023-06-07 09:03:03.288555 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/listener/__init__.py
--rw-r--r--   0        0        0      991 2023-06-07 16:56:34.852077 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/listener/kick.py
--rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/__init__.py
--rw-r--r--   0        0        0     1654 2023-06-24 08:58:25.069731 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
--rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
--rw-r--r--   0        0        0     1198 2023-06-24 09:05:18.581398 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
--rw-r--r--   0        0        0     1719 2023-06-24 05:42:04.607908 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
--rw-r--r--   0        0        0     1704 2023-06-24 05:39:55.256327 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
--rw-r--r--   0        0        0      728 2023-06-04 03:13:56.120283 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/sub_open.py
--rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
--rw-r--r--   0        0        0     7816 2023-06-30 02:55:31.194002 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
--rw-r--r--   0        0        0     2057 2023-04-24 02:36:16.771789 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/subscribe/live.py
--rw-r--r--   0        0        0      450 2023-06-22 16:58:52.849473 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/config.py
--rw-r--r--   0        0        0       20 2023-05-26 14:35:08.837033 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/database/__init__.py
--rw-r--r--   0        0        0     9884 2023-06-30 02:57:46.146679 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/database/db.py
--rw-r--r--   0        0        0     2750 2023-06-24 02:54:45.822615 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/database/model.py
--rw-r--r--   0        0        0     4011 2023-06-22 17:11:16.482488 nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/utils/__init__.py
--rw-r--r--   0        0        0     1000 2023-06-30 08:34:45.660052 nonebot_plugin_blive_danmaku-0.3.22/pyproject.toml
--rw-r--r--   0        0        0     5599 2023-06-24 09:07:18.310064 nonebot_plugin_blive_danmaku-0.3.22/README.md
--rw-r--r--   0        0        0     6554 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.3.22/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1027 2023-06-30 08:42:41.437287 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/__init__.py
+-rw-r--r--   0        0        0     1610 2023-04-28 07:50:38.274424 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/_plugin-vue_export-helper-1b428a4d.js
+-rw-r--r--   0        0        0   533008 2023-06-26 02:58:12.791659 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/echarts-400b5edd.js
+-rw-r--r--   0        0        0   285956 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-2bbb65c2.js
+-rw-r--r--   0        0        0   324265 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-5cfbb218.css
+-rw-r--r--   0        0        0     9045 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-1-k-823c4f26.png
+-rw-r--r--   0        0        0     8799 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-2-k-a0b7be7c.png
+-rw-r--r--   0        0        0     7006 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-3-k-3c7bacae.png
+-rw-r--r--   0        0        0      902 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/helpDialog-a1deb50e.js
+-rw-r--r--   0        0        0     6723 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-10fe5420.js
+-rw-r--r--   0        0        0     2787 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-1f52d48f.js
+-rw-r--r--   0        0        0    20588 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-3b039937.js
+-rw-r--r--   0        0        0     9107 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-4d7b4401.css
+-rw-r--r--   0        0        0      703 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-54bfb553.css
+-rw-r--r--   0        0        0     3061 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6803b0c6.js
+-rw-r--r--   0        0        0      815 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-7bb2b86c.css
+-rw-r--r--   0        0        0     5128 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-c1b5ef2f.js
+-rw-r--r--   0        0        0      167 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-cd2e8127.css
+-rw-r--r--   0        0        0      699 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e7323967.css
+-rw-r--r--   0        0        0     3593 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f24fc95e.js
+-rw-r--r--   0        0        0     1239 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f9e2a7e5.js
+-rw-r--r--   0        0        0       51 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-fe1a4f18.css
+-rw-r--r--   0        0        0    20126 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-520df23f.js
+-rw-r--r--   0        0        0     6259 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-1-f98dcdbf.png
+-rw-r--r--   0        0        0     5886 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-2-abaf3760.png
+-rw-r--r--   0        0        0    20334 2023-06-26 02:58:12.784659 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/SC-bg-img-0e2aa755.png
+-rw-r--r--   0        0        0      330 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-8f8a299b.css
+-rw-r--r--   0        0        0    18870 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-fcb4d4cd.js
+-rw-r--r--   0        0        0     1757 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b57f6aba.css
+-rw-r--r--   0        0        0   447924 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-fa374c7f.js
+-rw-r--r--   0        0        0    12014 2023-04-15 02:38:23.791948 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico
+-rw-r--r--   0        0        0      908 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/index.html
+-rw-r--r--   0        0        0      200 2023-06-04 10:26:16.056985 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/models.py
+-rw-r--r--   0        0        0     4864 2023-06-24 03:21:58.563784 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/router.py
+-rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/.git
+-rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
+-rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/.gitignore
+-rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
+-rw-r--r--   0        0        0    21948 2023-07-04 01:36:55.332967 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
+-rw-r--r--   0        0        0     7802 2023-07-04 17:30:44.363774 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
+-rw-r--r--   0        0        0    13206 2023-06-22 11:29:10.027052 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
+-rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/LICENSE
+-rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/README.md
+-rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
+-rw-r--r--   0        0        0     2928 2023-04-24 05:16:11.948995 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/sample.py
+-rw-r--r--   0        0        0      136 2023-06-07 09:20:41.977052 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/__init__.py
+-rw-r--r--   0        0        0        4 2023-06-07 09:03:03.288555 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/listener/__init__.py
+-rw-r--r--   0        0        0      991 2023-06-07 16:56:34.852077 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/listener/kick.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/__init__.py
+-rw-r--r--   0        0        0     1654 2023-06-24 08:58:25.069731 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
+-rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
+-rw-r--r--   0        0        0     1198 2023-06-24 09:05:18.581398 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
+-rw-r--r--   0        0        0     1719 2023-06-24 05:42:04.607908 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
+-rw-r--r--   0        0        0     1704 2023-06-24 05:39:55.256327 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
+-rw-r--r--   0        0        0      728 2023-06-04 03:13:56.120283 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/sub_open.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
+-rw-r--r--   0        0        0     7812 2023-07-04 17:10:18.909444 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
+-rw-r--r--   0        0        0     2057 2023-04-24 02:36:16.771789 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/subscribe/live.py
+-rw-r--r--   0        0        0      450 2023-06-22 16:58:52.849473 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/config.py
+-rw-r--r--   0        0        0       20 2023-05-26 14:35:08.837033 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/database/__init__.py
+-rw-r--r--   0        0        0     9884 2023-06-30 02:57:46.146679 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/database/db.py
+-rw-r--r--   0        0        0     2750 2023-07-04 17:05:11.717173 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/database/model.py
+-rw-r--r--   0        0        0     4011 2023-06-22 17:11:16.482488 nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/utils/__init__.py
+-rw-r--r--   0        0        0      999 2023-07-04 17:00:07.767248 nonebot_plugin_blive_danmaku-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5729 2023-07-04 17:01:06.493769 nonebot_plugin_blive_danmaku-0.3.3/README.md
+-rw-r--r--   0        0        0     6680 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.3.3/PKG-INFO
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/LICENSE` & `nonebot_plugin_blive_danmaku-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/__init__.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/__init__.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/echarts-400b5edd.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/echarts-400b5edd.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-2bbb65c2.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-2bbb65c2.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-5cfbb218.css` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-5cfbb218.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-1-k-823c4f26.png` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-1-k-823c4f26.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-2-k-a0b7be7c.png` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-2-k-a0b7be7c.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-3-k-3c7bacae.png` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-3-k-3c7bacae.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/helpDialog-a1deb50e.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/helpDialog-a1deb50e.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-10fe5420.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-10fe5420.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-1f52d48f.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-1f52d48f.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-3b039937.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-3b039937.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-4d7b4401.css` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-4d7b4401.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-54bfb553.css` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-54bfb553.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6803b0c6.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6803b0c6.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-7bb2b86c.css` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-7bb2b86c.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-c1b5ef2f.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-c1b5ef2f.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e7323967.css` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e7323967.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f24fc95e.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f24fc95e.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f9e2a7e5.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f9e2a7e5.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-520df23f.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-520df23f.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-1-f98dcdbf.png` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-1-f98dcdbf.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-2-abaf3760.png` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-2-abaf3760.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/SC-bg-img-0e2aa755.png` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/SC-bg-img-0e2aa755.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-fcb4d4cd.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-fcb4d4cd.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b57f6aba.css` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b57f6aba.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-fa374c7f.js` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-fa374c7f.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/frontend/index.html` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/frontend/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/app/router.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/app/router.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/.gitignore` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,15 @@
             self._heartbeat_timer_handle = None
 
     async def _send_auth(self):
         """
         发送认证包
         """
         auth_params = {
-            'uid': self._uid,
+            'uid': self._uid or self.room_owner_uid or 0,
             'roomid': self._room_id,
             'protover': 3,
             'platform': 'web',
             'type': 2
         }
         if self._host_server_token is not None:
             auth_params['key'] = self._host_server_token
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,30 +15,34 @@
 # 常见可忽略的cmd
 IGNORED_CMDS = (
     'AREA_RANK_CHANGED',
     'ANCHOR_LOT_CHECKSTATUS', # 天选时刻检查状态
     'ANCHOR_LOT_START', # 天选时刻抽奖开始
     'ANCHOR_LOT_END', # 天选时刻抽奖结束
     'ANCHOR_LOT_AWARD', # 天选时刻中奖名单
+    'ANCHOR_HELPER_DANMU',
     'COMBO_SEND', # 礼物连击
     'COMMON_NOTICE_DANMAKU', # 通用通知，含红包礼物涨粉、直播活动信息等
     'DANMU_AGGREGATION', # 抽奖弹幕，包含天选抽奖弹幕、红包抽奖弹幕等
     'ENTRY_EFFECT', # 入场特效
     'FULL_SCREEN_SPECIAL_EFFECT',
     'GIFT_PANEL_PLAN',
     'GIFT_STAR_PROCESS',
     'GUARD_ACHIEVEMENT_ROOM',
+    'GUARD_HONOR_THOUSAND',
     'HOT_RANK_CHANGED',
     'HOT_RANK_CHANGED_V2',
     'LIVE', # 直播开始
     'LIVE_INTERACTIVE_GAME',
     'LIVE_OPEN_PLATFORM_GAME',
     'LIVE_PANEL_CHANGE_CONTENT',
     'LIKE_INFO_V3_CLICK', # 用户点赞
     'LIKE_INFO_V3_UPDATE', # 点赞总数量更新
+    'LIKE_INFO_V3_NOTICE', # 双击点赞提示
+    'MESSAGEBOX_USER_GAIN_MEDAL', # 加入粉丝团？
     'NOTICE_MSG', # 通知横幅
     'ONLINE_RANK_COUNT', # 高能用户总数量
     'ONLINE_RANK_TOP3', # 高能榜前三变化
     'ONLINE_RANK_V2', # 高能榜前七名单
     'PK_BATTLE_START',
     'PK_BATTLE_START_NEW',
     'PK_BATTLE_PRE_NEW',
@@ -55,14 +59,16 @@
     'POPULARITY_RED_POCKET_NEW', # 红包礼物
     'POPULARITY_RED_POCKET_START', # 红包开抢
     'POPULARITY_RED_POCKET_WINNER_LIST', # 红包中奖
     'ROOM_REAL_TIME_MESSAGE_UPDATE', # 粉丝数等更新
     'ROOM_BLOCK_MSG',
     'ROOM_CHANGE',
     'ROOM_SKIN_MSG',
+    'SPREAD_SHOW_FEET', # 流量包推广
+    'SPRED_SHOW_FEET_V2', # 流量包推广
     'STOP_LIVE_ROOM_LIST', # 停播房间列表
     'SUPER_CHAT_MESSAGE_JPN', # 醒目留言(日)
     'SUPER_CHAT_ENTRANCE',
     'TRADING_SCORE',
     'USER_TOAST_MSG',
     'WIDGET_BANNER', # 小部件横幅
     'WIDGET_GIFT_STAR_PROCESS',
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/LICENSE` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/blivedm/sample.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/blivedm/sample.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/listener/kick.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/listener/kick.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/sub_add.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/sub_add.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/sub_list.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/sub_list.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/sub_off.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/sub_off.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/sub_on.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/sub_on.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/sub/sub_open.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/sub/sub_open.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self, room_id):
         self.uid=""
         self.name=""
         self.live_time=0
         self.client=blivedm.BLiveClient(room_id)
 
 
-clients = []
+clients:list[ClientModel] = []
 driver = get_driver()
 host = danmaku_config.danmaku_host if danmaku_config.danmaku_host else f"http://{driver.config.host}:{driver.config.port}"
 
 @scheduler.scheduled_job(
     "interval", seconds=15, id="street_lamp_sched"
 )
 async def danmaku():
@@ -40,34 +40,34 @@
     if not res:
         return
     logger.debug(f'爬取路灯列表')
     handler = MsgHandler()
     for uid, info in res.items():
         new_status = 0 if info["live_status"] == 2 else info["live_status"]
         index = [x for x in clients if x.uid == uid]
-        if not index:
-            if new_status:
-                logger.info(f'{info["uname"]}开播了，连接直播间')
-                room_id = info["short_id"] if info["short_id"] else info["room_id"]
-                room_info = await get_room_info_by_id(room_id, reqtype="web")
-                model = ClientModel(room_id)
-                model.client.add_handler(handler)
-                model.client.start()
-                model.uid=uid
-                model.name=info["uname"]
-                model.live_time=get_timespan(room_info["live_time"])
-                clients.append(model)
-
-                start_timespan = get_timespan(room_info["live_time"])
-                room = await db.get_room(room_id=room_id, uid=uid, start_time=start_timespan)
-                if not room:
-                    cover = (
-                        info["cover_from_user"] if info["cover_from_user"] else info["keyframe"]
-                    )
-                    await db.add_room(room_id=room_id, uid=uid, cover=cover, title=info["title"], name=info["uname"], start_time=start_timespan, end_time=0)
+        if not index and new_status:
+            logger.info(f'{info["uname"]}开播了，连接直播间')
+
+            room_id = info["short_id"] if info["short_id"] else info["room_id"]
+            room_info = await get_room_info_by_id(room_id, reqtype="web")
+            start_timespan = get_timespan(room_info["live_time"])
+            model = ClientModel(room_id)
+            model.client.add_handler(handler)
+            model.client.start()
+            model.uid=uid
+            model.name=info["uname"]
+            model.live_time=start_timespan
+            clients.append(model)
+
+            room = await db.get_room(room_id=room_id, uid=uid, start_time=start_timespan)
+            if room is None:
+                cover = (
+                    info["cover_from_user"] if info["cover_from_user"] else info["keyframe"]
+                )
+                await db.add_room(room_id=room_id, uid=uid, cover=cover, title=info["title"], name=info["uname"], start_time=start_timespan, end_time=0, watch_person=0)
     
 
 class MsgHandler(blivedm.BaseHandler):
     async def _on_danmaku(self, client: blivedm.BLiveClient, message: blivedm.DanmakuMessage):
         if(message.msg.startswith("#路灯")):
             logger.info(f'{client.room_owner_uid}的直播间收到路灯：{message.uname} -> {message.msg}')
         await save_danmaku(client.room_id, client.room_owner_uid, message.uname, int(message.timestamp / 1000), message.msg)
@@ -89,75 +89,76 @@
         logger.debug(f"[{client.room_id}] 当前人气值：{message.popularity}")
 
     async def _on_preparing(self, client: blivedm.BLiveClient, message: blivedm.PreparingMessage):
         index = [x for x in clients if x.uid == str(client.room_owner_uid)]
         model = index[0]
         if not model:
             return
+        await disconnect_room(model)
         now = int(time.time())
-        room_list = await db.get_rooms(room_id=client.room_id, end_time=0)
-        room_list.sort(key=lambda x:x.start_time, reverse=True)
-        room = room_list[0]
+        room = await db.get_room(room_id=client.room_id, start_time=model.live_time)
+        if room is None:
+            return
         await db.update_room("end_time", now, id=room.id)
         subs = await db.get_subs(uid=client.room_owner_uid,street_lamp=True)
         for sub in subs:
             msg = f'{model.name}下播了，可前往面板查看本次直播的路灯记录：{host}/danmaku/#/room?roomid={room.id}&type={sub.type}&type_id={sub.type_id}&uid={sub.uid}'
             await send_msg(bot_id=sub.bot_id,send_type=sub.type,type_id=sub.type_id,message=msg)
-        await disconnect_room(model)
     
     async def _on_watched(self, client: blivedm.BLiveClient, message: blivedm.WatchedMessage):
         room_list = await db.get_rooms(room_id=client.room_id, end_time=0)
         room_list.sort(key=lambda x:x.start_time, reverse=True)
         room = room_list[0]
+        if room is None:
+            return
+
         await db.update_room("watch_person", message.num, id=room.id)
 
 
-async def disconnect_room(model):
+async def disconnect_room(model: ClientModel):
     client = model.client
     try:
         asyncio.gather(client.join())
     finally:
         await asyncio.gather(client.stop_and_close())
         clients.remove(model)
         logger.info(f'{model.name} 断开直播间连接')
 
 
 async def save_danmaku(room_id, uid, send_name: str, timestamp: int, raw_msg: str):
     datetime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(timestamp))
-    subs = await db.get_subs(uid=uid)
-    if not subs:
+    index = [x for x in clients if x.uid == str(uid)]
+    if not index:
         return
-    for sub in subs:
-        index = [x for x in clients if x.uid == str(sub.uid)]
-        if not index:
-            continue
-        model = index[0]
-
-        dt = get_time_difference(model.live_time, timestamp)
-        room_list = await db.get_rooms(room_id=room_id, end_time=0)
-        room_list.sort(key=lambda x:x.start_time, reverse=True)
-        room = room_list[0]
-
-        danmaku_type = "danamku"
-        if raw_msg.startswith("#路灯"):
-            blive_danmaku = raw_msg.replace("#路灯","", 1).strip()
-            street_lamp = f'【{model.name}】 在 {datetime}({dt}) 收到了 {send_name} 发来的路灯【{blive_danmaku}】'
+    model = index[0]
+    dt = get_time_difference(model.live_time, timestamp)
+    room = await db.get_room(room_id=room_id, start_time=model.live_time)
+    if room is None:
+        return
+    danmaku_type = "danamku"
+    statistics_list = await db.get_subs(uid=uid,statistics=True)
+    if raw_msg.startswith("#路灯"):
+        blive_danmaku = raw_msg.replace("#路灯","", 1).strip()
+        street_lamp = f'【{model.name}】 在 {datetime}({dt}) 收到了 {send_name} 发来的路灯【{blive_danmaku}】'
+        danmaku_type = "street_lamp"
+        subs = await db.get_subs(uid=uid, street_lamp=True)
+        for sub in subs:
             await send_msg(bot_id=sub.bot_id, send_type=sub.type, type_id=sub.type_id, message=street_lamp)
-            danmaku_type = "street_lamp"
-        if(sub.statistics is False and danmaku_type == "danamku"):
-            continue
+        await db.add_danmaku(room_id=room.id, uname=send_name, message=raw_msg, create_time=datetime, live_duration=dt, type=danmaku_type)
+    if danmaku_type == "danamku" and len(statistics_list) > 0:
         await db.add_danmaku(room_id=room.id, uname=send_name, message=raw_msg, create_time=datetime, live_duration=dt, type=danmaku_type)
 
 
 async def save_gift(room_id, uid, send_name: str, send_uid: int, name: str, price: int, num: int, type: str, guard_level: int):
     datetime = int(time.time())
     index = [x for x in clients if x.uid == str(uid)]
     if not index:
         return
     model = index[0]
     dt = get_time_difference(model.live_time, datetime)
-    room_list = await db.get_rooms(room_id=room_id, end_time=0)
-    room_list.sort(key=lambda x:x.start_time, reverse=True)
-    room = room_list[0]
+    room = await db.get_room(room_id=room_id, start_time=model.live_time)
+    if room is None:
+        return
+
     coin = price if type == 'sc' else price / 1000
     await db.add_gift(rid=room.id, name=name, price=coin, num=num, uname=send_name, uid=send_uid, type=type, create_time=datetime, live_duration=dt, guard=guard_level)
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/command/subscribe/live.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/command/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/database/db.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/database/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/database/model.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/database/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/nonebot_plugin_blive_danmaku/utils/__init__.py` & `nonebot_plugin_blive_danmaku-0.3.3/nonebot_plugin_blive_danmaku/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/pyproject.toml` & `nonebot_plugin_blive_danmaku-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-blive-danmaku"
-version = "0.3.22"
+version = "0.3.3"
 description = "A danmaku plugin for Nonebot2"
 authors = ["ricardo <thespirit@vip.qq.com>"]
 documentation = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku#readme"
 license = "MIT"
 homepage = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "bilibili", "danmaku"]
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/README.md` & `nonebot_plugin_blive_danmaku-0.3.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -100,14 +100,17 @@
     ProxyRequests Off
     ProxyPass "/danmaku/" http://127.0.0.1:8080/danmaku/
     ProxyPassReverse "/danmaku/" http://127.0.0.1:8080/danmaku/
 </VirtualHost>
 ```
 
 ## 更新日志 
+- v0.3.3
+    - 修复弹幕用户名打码
+    - fix [#12](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/12)
 - v0.3.0
     - 适配nonebot2 2.0.0
     - 增加弹幕统计
     - 新增记录SuperChat内容，可在面板生成SuperChat图片
     - 更新依赖 [#11](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/11)
 - v0.2.9
     - 面板查询开播历史列表，标题旁展示该场直播的路灯数量
```

#### html2text {}

```diff
@@ -39,16 +39,17 @@
 { proxy_pass http://127.0.0.1:8080/danmaku/; proxy_http_version 1.1;
 proxy_set_header Upgrade $http_upgrade; proxy_set_header Connection keep-alive;
 proxy_set_header Host $host; proxy_set_header X-Real-IP $remote_addr;
 proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; proxy_cache_bypass
 $http_upgrade; } location /ws { deny all; } } ``` Apache ``` apache
 :80> ServerName www.your_domain.com ProxyRequests Off ProxyPass "/danmaku/
 " http://127.0.0.1:8080/danmaku/ ProxyPassReverse "/danmaku/" http://127.0.0.1:
-8080/danmaku/  ``` ## æ´æ°æ¥å¿ - v0.3.0 - éénonebot2 2.0.0 -
-å¢å å¼¹å¹ç»è®¡ -
+8080/danmaku/  ``` ## æ´æ°æ¥å¿ - v0.3.3 - ä¿®å¤å¼¹å¹ç¨æ·åæç  - fix
+[#12](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/12) -
+v0.3.0 - éénonebot2 2.0.0 - å¢å å¼¹å¹ç»è®¡ -
 æ°å¢è®°å½SuperChatåå®¹ï¼å¯å¨é¢æ¿çæSuperChatå¾ç - æ´æ°ä¾èµ
 [#11](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/11) -
 v0.2.9 -
 é¢æ¿æ¥è¯¢å¼æ­åå²åè¡¨ï¼æ é¢æå±ç¤ºè¯¥åºç´æ­çè·¯ç¯æ°é -
 Botè¢«è¸¢åºç¾¤åæ¸é¤è¯¥ç¾¤çè®¢é - fixè·¯ç¯åè¡¨æç´¢bug - Clean Up
 Code - v0.2.8 -
 å°é¢å°åä¸åç»å®urlï¼é¢æ¿å°ååæ´å¯¼è´å°é¢å¾çå¼å¸¸çå¯æå¨æ¸ç
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.22/PKG-INFO` & `nonebot_plugin_blive_danmaku-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blive-danmaku
-Version: 0.3.22
+Version: 0.3.3
 Summary: A danmaku plugin for Nonebot2
 Home-page: https://github.com/zangxx66/nonebot_plugin_blive_danmaku
 License: MIT
 Keywords: nonebot,nonebot2,bilibili,danmaku
 Author: ricardo
 Author-email: thespirit@vip.qq.com
 Requires-Python: >=3.10,<4.0
@@ -127,14 +127,17 @@
     ProxyRequests Off
     ProxyPass "/danmaku/" http://127.0.0.1:8080/danmaku/
     ProxyPassReverse "/danmaku/" http://127.0.0.1:8080/danmaku/
 </VirtualHost>
 ```
 
 ## 更新日志 
+- v0.3.3
+    - 修复弹幕用户名打码
+    - fix [#12](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/12)
 - v0.3.0
     - 适配nonebot2 2.0.0
     - 增加弹幕统计
     - 新增记录SuperChat内容，可在面板生成SuperChat图片
     - 更新依赖 [#11](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/11)
 - v0.2.9
     - 面板查询开播历史列表，标题旁展示该场直播的路灯数量
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.3.22
+Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.3.3
 Summary: A danmaku plugin for Nonebot2 Home-page: https://github.com/zangxx66/
 nonebot_plugin_blive_danmaku License: MIT Keywords:
 nonebot,nonebot2,bilibili,danmaku Author: ricardo Author-email:
 thespirit@vip.qq.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -55,16 +55,17 @@
 { proxy_pass http://127.0.0.1:8080/danmaku/; proxy_http_version 1.1;
 proxy_set_header Upgrade $http_upgrade; proxy_set_header Connection keep-alive;
 proxy_set_header Host $host; proxy_set_header X-Real-IP $remote_addr;
 proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; proxy_cache_bypass
 $http_upgrade; } location /ws { deny all; } } ``` Apache ``` apache
 :80> ServerName www.your_domain.com ProxyRequests Off ProxyPass "/danmaku/
 " http://127.0.0.1:8080/danmaku/ ProxyPassReverse "/danmaku/" http://127.0.0.1:
-8080/danmaku/  ``` ## æ´æ°æ¥å¿ - v0.3.0 - éénonebot2 2.0.0 -
-å¢å å¼¹å¹ç»è®¡ -
+8080/danmaku/  ``` ## æ´æ°æ¥å¿ - v0.3.3 - ä¿®å¤å¼¹å¹ç¨æ·åæç  - fix
+[#12](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/12) -
+v0.3.0 - éénonebot2 2.0.0 - å¢å å¼¹å¹ç»è®¡ -
 æ°å¢è®°å½SuperChatåå®¹ï¼å¯å¨é¢æ¿çæSuperChatå¾ç - æ´æ°ä¾èµ
 [#11](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/11) -
 v0.2.9 -
 é¢æ¿æ¥è¯¢å¼æ­åå²åè¡¨ï¼æ é¢æå±ç¤ºè¯¥åºç´æ­çè·¯ç¯æ°é -
 Botè¢«è¸¢åºç¾¤åæ¸é¤è¯¥ç¾¤çè®¢é - fixè·¯ç¯åè¡¨æç´¢bug - Clean Up
 Code - v0.2.8 -
 å°é¢å°åä¸åç»å®urlï¼é¢æ¿å°ååæ´å¯¼è´å°é¢å¾çå¼å¸¸çå¯æå¨æ¸ç
```

