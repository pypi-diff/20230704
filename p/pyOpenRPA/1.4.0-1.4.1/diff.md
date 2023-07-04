# Comparing `tmp/pyOpenRPA-1.4.0.tar.gz` & `tmp/pyOpenRPA-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyOpenRPA-1.4.0.tar", last modified: Tue Jul  4 08:42:58 2023, max compression
+gzip compressed data, was "dist\pyOpenRPA-1.4.1.tar", last modified: Tue Jul  4 08:44:30 2023, max compression
```

## Comparing `pyOpenRPA-1.4.0.tar` & `pyOpenRPA-1.4.1.tar`

### file list

```diff
@@ -1,367 +1,374 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/
--rw-rw-rw-   0        0        0       55 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4341 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Agent/
--rw-rw-rw-   0        0        0     1713 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Agent/A2O.py
--rw-rw-rw-   0        0        0     6305 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Agent/O2A.py
--rw-rw-rw-   0        0        0     6346 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Agent/Processor.py
--rw-rw-rw-   0        0        0    15338 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Agent/__Agent__.py
--rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Agent/__init__.py
--rw-rw-rw-   0        0        0       19 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Agent/readme.md
--rw-rw-rw-   0        0        0       85 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Info.md
--rw-rw-rw-   0        0        0  4322139 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/LICENSE.pdf
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/
--rw-rw-rw-   0        0        0    39641 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/BackwardCompatibility.py
--rw-rw-rw-   0        0        0      103 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/ControlPanel.py
--rw-rw-rw-   0        0        0      529 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Core.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Managers/
--rw-rw-rw-   0        0        0    17877 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Managers/ControlPanel.py
--rw-rw-rw-   0        0        0    12879 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Managers/Git.py
--rw-rw-rw-   0        0        0    42537 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Managers/Process.py
--rw-rw-rw-   0        0        0       71 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Managers/__init__.py
--rw-rw-rw-   0        0        0    10368 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Processor.py
--rw-rw-rw-   0        0        0    13749 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/ProcessorOld.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/
--rw-rw-rw-   0        0        0     1531 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/CMDStr.py
--rw-rw-rw-   0        0        0     1954 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Clipboard.py
--rw-rw-rw-   0        0        0    28437 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Connector.py
--rw-rw-rw-   0        0        0      657 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/ConnectorExceptions.py
--rw-rw-rw-   0        0        0    12405 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Processor.py
--rw-rw-rw-   0        0        0     2954 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Recovery.py
--rw-rw-rw-   0        0        0    13271 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/RobotRDPActive.py
--rw-rw-rw-   0        0        0     9144 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Scheduler.py
--rw-rw-rw-   0        0        0     2462 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Template.rdp
--rw-rw-rw-   0        0        0     1077 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Timer.py
--rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/__init__.py
--rw-rw-rw-   0        0        0     2508 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotScreenActive/
--rwxrwxrwx   0        0        0      114 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotScreenActive/ConsoleStart.bat
--rw-rw-rw-   0        0        0      603 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotScreenActive/Monitor.py
--rw-rw-rw-   0        0        0      606 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotScreenActive/Screen.py
--rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotScreenActive/__init__.py
--rw-rw-rw-   0        0        0      593 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotScreenActive/__main__.py
--rw-rw-rw-   0        0        0    17081 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Server.py
--rw-rw-rw-   0        0        0    23787 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/ServerBC.py
--rw-rw-rw-   0        0        0    35984 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/ServerSettings.py
--rw-rw-rw-   0        0        0    21612 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/SettingsTemplate.py
--rw-rw-rw-   0        0        0     2097 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Timer.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Utils/
--rw-rw-rw-   0        0        0      681 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Utils/LoggerHandlerDumpLogList.py
--rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Web/
--rw-rw-rw-   0        0        0     7757 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Web/Basic.py
--rw-rw-rw-   0        0        0   218024 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/__Orchestrator__.py
--rw-rw-rw-   0        0        0      207 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/__init__.py
--rw-rw-rw-   0        0        0      273 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/__main__.py
--rw-rw-rw-   0        0        0     2521 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Google/
--rw-rw-rw-   0        0        0     3112 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Google/LatoItalic.css
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Handlebars/
--rw-rw-rw-   0        0        0   171994 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Handlebars/handlebars-v4.1.2.js
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/JsRender/
--rw-rw-rw-   0        0        0    25927 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/JsRender/jsrender.min.js
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/
--rw-rw-rw-   0        0        0       72 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/.versions
--rw-rw-rw-   0        0        0     1102 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/LICENSE
--rw-rw-rw-   0        0        0      448 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/
--rw-rw-rw-   0        0        0     8971 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.css
--rw-rw-rw-   0        0        0    20790 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.js
--rw-rw-rw-   0        0        0     6955 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.min.css
--rw-rw-rw-   0        0        0     7100 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.min.js
--rw-rw-rw-   0        0        0     4176 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/ad.css
--rw-rw-rw-   0        0        0     2066 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/ad.min.css
--rw-rw-rw-   0        0        0    40952 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/api.js
--rw-rw-rw-   0        0        0    14594 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/api.min.js
--rw-rw-rw-   0        0        0     2166 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/breadcrumb.css
--rw-rw-rw-   0        0        0     1192 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/breadcrumb.min.css
--rw-rw-rw-   0        0        0   116361 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/button.css
--rw-rw-rw-   0        0        0    90207 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/button.min.css
--rw-rw-rw-   0        0        0    25330 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/card.css
--rw-rw-rw-   0        0        0    17410 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/card.min.css
--rw-rw-rw-   0        0        0    17473 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.css
--rw-rw-rw-   0        0        0    26912 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.js
--rw-rw-rw-   0        0        0    12727 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.min.css
--rw-rw-rw-   0        0        0    11369 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.min.js
--rw-rw-rw-   0        0        0     8710 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/colorize.js
--rw-rw-rw-   0        0        0     3270 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/colorize.min.js
--rw-rw-rw-   0        0        0     5120 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/comment.css
--rw-rw-rw-   0        0        0     2945 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/comment.min.css
--rw-rw-rw-   0        0        0     3099 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/container.css
--rw-rw-rw-   0        0        0     1925 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/container.min.css
--rw-rw-rw-   0        0        0     5559 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.css
--rw-rw-rw-   0        0        0    22303 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.js
--rw-rw-rw-   0        0        0     3517 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.min.css
--rw-rw-rw-   0        0        0     8071 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.min.js
--rw-rw-rw-   0        0        0     8034 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/divider.css
--rw-rw-rw-   0        0        0     6097 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/divider.min.css
--rw-rw-rw-   0        0        0    37420 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.css
--rw-rw-rw-   0        0        0   145962 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.js
--rw-rw-rw-   0        0        0    25679 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.min.css
--rw-rw-rw-   0        0        0    50895 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.min.js
--rw-rw-rw-   0        0        0     3169 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.css
--rw-rw-rw-   0        0        0    20926 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.js
--rw-rw-rw-   0        0        0     1836 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.min.css
--rw-rw-rw-   0        0        0     7728 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.min.js
--rw-rw-rw-   0        0        0     5845 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/feed.css
--rw-rw-rw-   0        0        0     3590 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/feed.min.css
--rw-rw-rw-   0        0        0    22423 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/flag.css
--rw-rw-rw-   0        0        0    18577 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/flag.min.css
--rw-rw-rw-   0        0        0    29092 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.css
--rw-rw-rw-   0        0        0    57618 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.js
--rw-rw-rw-   0        0        0    21568 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.min.css
--rw-rw-rw-   0        0        0    20458 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.min.js
--rw-rw-rw-   0        0        0    73036 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/grid.css
--rw-rw-rw-   0        0        0    57335 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/grid.min.css
--rw-rw-rw-   0        0        0    13499 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/header.css
--rw-rw-rw-   0        0        0     8872 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/header.min.css
--rw-rw-rw-   0        0        0    86945 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/icon.css
--rw-rw-rw-   0        0        0    67019 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/icon.min.css
--rw-rw-rw-   0        0        0     5676 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/image.css
--rw-rw-rw-   0        0        0     3727 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/image.min.css
--rw-rw-rw-   0        0        0    12699 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/input.css
--rw-rw-rw-   0        0        0     8692 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/input.min.css
--rw-rw-rw-   0        0        0     9753 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/item.css
--rw-rw-rw-   0        0        0     5985 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/item.min.css
--rw-rw-rw-   0        0        0    28382 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/label.css
--rw-rw-rw-   0        0        0    20005 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/label.min.css
--rw-rw-rw-   0        0        0    22486 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/list.css
--rw-rw-rw-   0        0        0    16094 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/list.min.css
--rw-rw-rw-   0        0        0     7128 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/loader.css
--rw-rw-rw-   0        0        0     4702 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/loader.min.css
--rw-rw-rw-   0        0        0    45279 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/menu.css
--rw-rw-rw-   0        0        0    31506 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/menu.min.css
--rw-rw-rw-   0        0        0    12466 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/message.css
--rw-rw-rw-   0        0        0     8354 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/message.min.css
--rw-rw-rw-   0        0        0    12800 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.css
--rw-rw-rw-   0        0        0    33442 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.js
--rw-rw-rw-   0        0        0     8012 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.min.css
--rw-rw-rw-   0        0        0    12701 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.min.js
--rw-rw-rw-   0        0        0     2727 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.css
--rw-rw-rw-   0        0        0    15553 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.js
--rw-rw-rw-   0        0        0     1483 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.min.css
--rw-rw-rw-   0        0        0     5696 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.min.js
--rw-rw-rw-   0        0        0     5938 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/placeholder.css
--rw-rw-rw-   0        0        0     4452 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/placeholder.min.css
--rw-rw-rw-   0        0        0    17407 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.css
--rw-rw-rw-   0        0        0    52273 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.js
--rw-rw-rw-   0        0        0    12032 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.min.css
--rw-rw-rw-   0        0        0    18630 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.min.js
--rw-rw-rw-   0        0        0    10669 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.css
--rw-rw-rw-   0        0        0    31204 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.js
--rw-rw-rw-   0        0        0     7422 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.min.css
--rw-rw-rw-   0        0        0    12331 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.min.js
--rw-rw-rw-   0        0        0     2646 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rail.css
--rw-rw-rw-   0        0        0     1453 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rail.min.css
--rw-rw-rw-   0        0        0    20696 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.css
--rw-rw-rw-   0        0        0    14869 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.js
--rw-rw-rw-   0        0        0    18393 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.min.css
--rw-rw-rw-   0        0        0     5354 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.min.js
--rw-rw-rw-   0        0        0     9123 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reset.css
--rw-rw-rw-   0        0        0     2822 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reset.min.css
--rw-rw-rw-   0        0        0     8177 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reveal.css
--rw-rw-rw-   0        0        0     5784 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reveal.min.css
--rw-rw-rw-   0        0        0    10377 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.css
--rw-rw-rw-   0        0        0    51211 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.js
--rw-rw-rw-   0        0        0     6891 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.min.css
--rw-rw-rw-   0        0        0    17622 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.min.js
--rw-rw-rw-   0        0        0    20063 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/segment.css
--rw-rw-rw-   0        0        0    13763 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/segment.min.css
--rw-rw-rw-   0        0        0     3865 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.css
--rw-rw-rw-   0        0        0    29873 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.js
--rw-rw-rw-   0        0        0     2521 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.min.css
--rw-rw-rw-   0        0        0    10803 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.min.js
--rw-rw-rw-   0        0        0    15757 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.css
--rw-rw-rw-   0        0        0    34488 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.js
--rw-rw-rw-   0        0        0    10726 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.min.css
--rw-rw-rw-   0        0        0    13466 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.min.js
--rw-rw-rw-   0        0        0     3918 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.css
--rw-rw-rw-   0        0        0    14604 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.js
--rw-rw-rw-   0        0        0     2452 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.min.css
--rw-rw-rw-   0        0        0     6066 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.min.js
--rw-rw-rw-   0        0        0    21498 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/state.js
--rw-rw-rw-   0        0        0     7804 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/state.min.js
--rw-rw-rw-   0        0        0    13221 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/statistic.css
--rw-rw-rw-   0        0        0     9594 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/statistic.min.css
--rw-rw-rw-   0        0        0    23555 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/step.css
--rw-rw-rw-   0        0        0    19188 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/step.min.css
--rw-rw-rw-   0        0        0     1288 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.css
--rw-rw-rw-   0        0        0    31814 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.js
--rw-rw-rw-   0        0        0      607 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.min.css
--rw-rw-rw-   0        0        0    11854 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.min.js
--rw-rw-rw-   0        0        0     1865 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.css
--rw-rw-rw-   0        0        0    33771 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.js
--rw-rw-rw-   0        0        0     1075 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.min.css
--rw-rw-rw-   0        0        0    11487 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.min.js
--rw-rw-rw-   0        0        0    25536 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/table.css
--rw-rw-rw-   0        0        0    18015 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/table.min.css
--rw-rw-rw-   0        0        0    49176 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.css
--rw-rw-rw-   0        0        0    36076 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.js
--rw-rw-rw-   0        0        0    33525 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.min.css
--rw-rw-rw-   0        0        0    13010 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.min.js
--rw-rw-rw-   0        0        0     2346 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.css
--rw-rw-rw-   0        0        0    16252 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.js
--rw-rw-rw-   0        0        0     1328 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.min.css
--rw-rw-rw-   0        0        0     6090 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.min.js
--rw-rw-rw-   0        0        0    44180 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visibility.js
--rw-rw-rw-   0        0        0    16294 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visibility.min.js
--rw-rw-rw-   0        0        0    16142 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visit.js
--rw-rw-rw-   0        0        0     5887 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visit.min.js
--rw-rw-rw-   0        0        0      774 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/package.js
--rw-rw-rw-   0        0        0      524 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/package.json
--rw-rw-rw-   0        0        0   869203 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.css
--rw-rw-rw-   0        0        0   759089 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.js
--rw-rw-rw-   0        0        0   628944 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.min.css
--rw-rw-rw-   0        0        0   275740 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.min.js
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/
--rw-rw-rw-   0        0        0    98640 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.eot
--rw-rw-rw-   0        0        0   508636 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.svg
--rw-rw-rw-   0        0        0    98404 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.ttf
--rw-rw-rw-   0        0        0    63728 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.woff
--rw-rw-rw-   0        0        0    54488 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.woff2
--rw-rw-rw-   0        0        0   106004 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.eot
--rw-rw-rw-   0        0        0    93888 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.otf
--rw-rw-rw-   0        0        0   392355 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.svg
--rw-rw-rw-   0        0        0   105784 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.ttf
--rw-rw-rw-   0        0        0    50524 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.woff
--rw-rw-rw-   0        0        0    40148 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.woff2
--rw-rw-rw-   0        0        0    31156 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.eot
--rw-rw-rw-   0        0        0   107567 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.svg
--rw-rw-rw-   0        0        0    30928 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.ttf
--rw-rw-rw-   0        0        0    14712 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.woff
--rw-rw-rw-   0        0        0    12240 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.woff2
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/images/
--rw-rw-rw-   0        0        0    28123 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/images/flags.png
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/jQuery/
--rw-rw-rw-   0        0        0    86713 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/jQuery/jquery-3.1.1.min.js
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/
--rw-rw-rw-   0        0        0     4916 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/auth.xhtml
--rw-rw-rw-   0        0        0     2339 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/badAuth.xhtml
--rw-rw-rw-   0        0        0   112922 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/favicon.ico
--rw-rw-rw-   0        0        0     4093 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/footer.xhtml
--rw-rw-rw-   0        0        0     3709 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/header.xhtml
--rw-rw-rw-   0        0        0    15975 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/logo.png
--rw-rw-rw-   0        0        0    44545 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/orc.js
--rw-rw-rw-   0        0        0    19223 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/orc.xhtml
--rw-rw-rw-   0        0        0     1913 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std.css
--rw-rw-rw-   0        0        0   110270 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std.js
--rw-rw-rw-   0        0        0    60979 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std.xhtml
--rw-rw-rw-   0        0        0    21304 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std_browser.js
--rw-rw-rw-   0        0        0      916 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std_floidd.css
--rw-rw-rw-   0        0        0    31527 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std_floidd.js
--rw-rw-rw-   0        0        0    16830 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std_helper.js
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/
--rw-rw-rw-   0        0        0   184912 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/Lato-Bold.woff2
--rw-rw-rw-   0        0        0   195704 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/Lato-Italic.woff2
--rw-rw-rw-   0        0        0   182708 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/Lato-Regular.woff2
--rw-rw-rw-   0        0        0   251041 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg1.jpg
--rw-rw-rw-   0        0        0   256648 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg10.jpg
--rw-rw-rw-   0        0        0   249670 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg2.jpg
--rw-rw-rw-   0        0        0   245168 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg3.jpg
--rw-rw-rw-   0        0        0   258568 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg4.jpg
--rw-rw-rw-   0        0        0   261562 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg5.jpg
--rw-rw-rw-   0        0        0   260686 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg6.jpg
--rw-rw-rw-   0        0        0   261376 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg7.jpg
--rw-rw-rw-   0        0        0   261288 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg8.jpg
--rw-rw-rw-   0        0        0   261559 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg9.jpg
--rw-rw-rw-   0        0        0    55821 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/docs.css
--rw-rw-rw-   0        0        0    55845 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/docs.css.bak
--rw-rw-rw-   0        0        0    44749 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/docs.js
--rw-rw-rw-   0        0        0    37642 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/dropdown.css
--rw-rw-rw-   0        0        0     3794 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/easing.min.js
--rw-rw-rw-   0        0        0    13723 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/header.css
--rw-rw-rw-   0        0        0    21964 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/highlight.min.js
--rw-rw-rw-   0        0        0    16245 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/home.css
--rw-rw-rw-   0        0        0     8926 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/home.js
--rw-rw-rw-   0        0        0    84349 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/jquery.min.js
--rw-rw-rw-   0        0        0   136781 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/less.min.js
--rw-rw-rw-   0        0        0        2 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/metadata.json
--rw-rw-rw-   0        0        0    23839 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/nan.jpg
--rw-rw-rw-   0        0        0   242713 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/ogImage.JPG
--rw-rw-rw-   0        0        0   131928 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/ogImage.PNG
--rw-rw-rw-   0        0        0     4899 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/pyOpenRPA_logo.png
--rw-rw-rw-   0        0        0    20287 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/segment.css
--rw-rw-rw-   0        0        0    34482 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/sidebar.js
--rw-rw-rw-   0        0        0    36070 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/transition.js
--rw-rw-rw-   0        0        0    44174 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/visibility.js
--rw-rw-rw-   0        0        0     5951 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/white-image.png
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/
--rw-rw-rw-   0        0        0    22176 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Audio.py
--rw-rw-rw-   0        0        0     1992 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Clipboard.py
--rw-rw-rw-   0        0        0    26619 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Keyboard.py
--rw-rw-rw-   0        0        0    16391 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Mouse.py
--rw-rw-rw-   0        0        0    20445 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/OrchestratorConnector.py
--rw-rw-rw-   0        0        0     1623 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/README.md
--rw-rw-rw-   0        0        0    57171 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Screen.py
--rw-rw-rw-   0        0        0     1453 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/SettingsTemplate.py
--rw-rw-rw-   0        0        0     2878 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Test.py
--rw-rw-rw-   0        0        0   194982 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/UIDesktop.py
--rw-rw-rw-   0        0        0    90412 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/UIWeb.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Utils/
--rw-rw-rw-   0        0        0     3884 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Utils/JSONNormalize.py
--rw-rw-rw-   0        0        0     4591 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Utils/ProcessBitness.py
--rw-rw-rw-   0        0        0     8039 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Utils/ProcessCommunicator.py
--rw-rw-rw-   0        0        0      961 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Utils/TimerRepeat.py
--rw-rw-rw-   0        0        0      777 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Utils/ValueVerify.py
--rw-rw-rw-   0        0        0       28 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Utils/__init__.py
--rw-rw-rw-   0        0        0      764 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/Window.py
--rw-rw-rw-   0        0        0      255 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/__init__.py
--rw-rw-rw-   0        0        0     2029 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Robot/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Studio/
--rw-rw-rw-   0        0        0     3341 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Studio/JSONNormalize.py
--rw-rw-rw-   0        0        0     7912 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Studio/ProcessCommunicator.py
--rw-rw-rw-   0        0        0     6571 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Studio/Processor.py
--rw-rw-rw-   0        0        0     5038 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Studio/RobotConnector.py
--rw-rw-rw-   0        0        0    27538 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Studio/Studio.py
--rw-rw-rw-   0        0        0      777 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Studio/ValueVerify.py
--rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Studio/__init__.py
--rw-rw-rw-   0        0        0      458 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Studio/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/
--rw-rw-rw-   0        0        0       29 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/CrossOS.py
--rw-rw-rw-   0        0        0       30 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/Debugger.py
--rw-rw-rw-   0        0        0       29 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/License.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotDB/
--rw-rw-rw-   0        0        0      343 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotDB/ExcelCom.py
--rw-rw-rw-   0        0        0     1473 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotDB/HowToUse
--rw-rw-rw-   0        0        0     1655 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotDB/RobotDB.py
--rw-rw-rw-   0        0        0    20087 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotDB/Server.py
--rw-rw-rw-   0        0        0     7406 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotDB/ServerSettings.py
--rw-rw-rw-   0        0        0      124 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotDB/__init__.py
--rw-rw-rw-   0        0        0      140 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotDB/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotScreenActive/
--rwxrwxrwx   0        0        0      114 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotScreenActive/ConsoleStart.bat
--rw-rw-rw-   0        0        0      492 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotScreenActive/Monitor.py
--rw-rw-rw-   0        0        0      606 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotScreenActive/Screen.py
--rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotScreenActive/__init__.py
--rw-rw-rw-   0        0        0      593 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotScreenActive/__main__.py
--rw-rw-rw-   0        0        0       30 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/StopSafe.py
--rw-rw-rw-   0        0        0     5507 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/Template.py
--rw-rw-rw-   0        0        0     2998 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/Usage.py
--rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.0/pyOpenRPA/Tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/Utils/
--rw-rw-rw-   0        0        0     3539 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Utils/CrossOS.py
--rw-rw-rw-   0        0        0      570 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Utils/Debugger.py
--rw-rw-rw-   0        0        0     2261 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Utils/Dictionary.py
--rw-rw-rw-   0        0        0     1848 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Utils/Disk.py
--rw-rw-rw-   0        0        0     9932 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Utils/License.py
--rw-rw-rw-   0        0        0      600 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Utils/Network.py
--rw-rw-rw-   0        0        0     6720 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Utils/Render.py
--rw-rw-rw-   0        0        0     2346 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Utils/StopSafe.py
--rw-rw-rw-   0        0        0      214 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.0/pyOpenRPA/Utils/Text.py
--rw-rw-rw-   0        0        0     6657 2023-07-04 08:33:29.000000 pyOpenRPA-1.4.0/pyOpenRPA/Utils/__define__.py
--rw-rw-rw-   0        0        0      154 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA.egg-info/
--rw-rw-rw-   0        0        0     4341 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18533 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-10 19:47:56.000000 pyOpenRPA-1.4.0/pyOpenRPA.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      350 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/pyOpenRPA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 08:42:58.000000 pyOpenRPA-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     3300 2023-07-04 08:42:48.000000 pyOpenRPA-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/
+-rw-rw-rw-   0        0        0       55 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4334 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Agent/
+-rw-rw-rw-   0        0        0     1713 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Agent/A2O.py
+-rw-rw-rw-   0        0        0     6305 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Agent/O2A.py
+-rw-rw-rw-   0        0        0     6346 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Agent/Processor.py
+-rw-rw-rw-   0        0        0    15338 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Agent/__Agent__.py
+-rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Agent/__init__.py
+-rw-rw-rw-   0        0        0       19 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Agent/readme.md
+-rw-rw-rw-   0        0        0       85 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Info.md
+-rw-rw-rw-   0        0        0  4322139 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/LICENSE.pdf
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/
+-rw-rw-rw-   0        0        0    39641 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/BackwardCompatibility.py
+-rw-rw-rw-   0        0        0      103 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/ControlPanel.py
+-rw-rw-rw-   0        0        0      529 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Core.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Managers/
+-rw-rw-rw-   0        0        0    17877 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Managers/ControlPanel.py
+-rw-rw-rw-   0        0        0    12879 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Managers/Git.py
+-rw-rw-rw-   0        0        0    42537 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Managers/Process.py
+-rw-rw-rw-   0        0        0       71 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Managers/__init__.py
+-rw-rw-rw-   0        0        0    10368 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Processor.py
+-rw-rw-rw-   0        0        0    13749 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/ProcessorOld.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/
+-rw-rw-rw-   0        0        0     1531 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/CMDStr.py
+-rw-rw-rw-   0        0        0     1954 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Clipboard.py
+-rw-rw-rw-   0        0        0    28437 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Connector.py
+-rw-rw-rw-   0        0        0      657 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/ConnectorExceptions.py
+-rw-rw-rw-   0        0        0    12405 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Processor.py
+-rw-rw-rw-   0        0        0     2954 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Recovery.py
+-rw-rw-rw-   0        0        0    13271 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/RobotRDPActive.py
+-rw-rw-rw-   0        0        0     9144 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Scheduler.py
+-rw-rw-rw-   0        0        0     2462 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Template.rdp
+-rw-rw-rw-   0        0        0     1077 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Timer.py
+-rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/__init__.py
+-rw-rw-rw-   0        0        0     2508 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotScreenActive/
+-rwxrwxrwx   0        0        0      114 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotScreenActive/ConsoleStart.bat
+-rw-rw-rw-   0        0        0      603 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotScreenActive/Monitor.py
+-rw-rw-rw-   0        0        0      606 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotScreenActive/Screen.py
+-rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotScreenActive/__init__.py
+-rw-rw-rw-   0        0        0      593 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotScreenActive/__main__.py
+-rw-rw-rw-   0        0        0    17081 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Server.py
+-rw-rw-rw-   0        0        0    23787 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/ServerBC.py
+-rw-rw-rw-   0        0        0    36012 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/ServerSettings.py
+-rw-rw-rw-   0        0        0    21612 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/SettingsTemplate.py
+-rw-rw-rw-   0        0        0     2097 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Timer.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Utils/
+-rw-rw-rw-   0        0        0      681 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Utils/LoggerHandlerDumpLogList.py
+-rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Web/
+-rw-rw-rw-   0        0        0     7757 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Web/Basic.py
+-rw-rw-rw-   0        0        0   219211 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/__Orchestrator__.py
+-rw-rw-rw-   0        0        0      207 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/__init__.py
+-rw-rw-rw-   0        0        0      273 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/__main__.py
+-rw-rw-rw-   0        0        0     2521 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Google/
+-rw-rw-rw-   0        0        0     3112 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Google/LatoItalic.css
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Handlebars/
+-rw-rw-rw-   0        0        0   171994 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Handlebars/handlebars-v4.1.2.js
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/JsRender/
+-rw-rw-rw-   0        0        0    25927 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/JsRender/jsrender.min.js
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/
+-rw-rw-rw-   0        0        0       72 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/.versions
+-rw-rw-rw-   0        0        0     1102 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/LICENSE
+-rw-rw-rw-   0        0        0      448 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/
+-rw-rw-rw-   0        0        0     8971 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.css
+-rw-rw-rw-   0        0        0    20790 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.js
+-rw-rw-rw-   0        0        0     6955 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.min.css
+-rw-rw-rw-   0        0        0     7100 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.min.js
+-rw-rw-rw-   0        0        0     4176 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/ad.css
+-rw-rw-rw-   0        0        0     2066 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/ad.min.css
+-rw-rw-rw-   0        0        0    40952 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/api.js
+-rw-rw-rw-   0        0        0    14594 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/api.min.js
+-rw-rw-rw-   0        0        0     2166 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/breadcrumb.css
+-rw-rw-rw-   0        0        0     1192 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/breadcrumb.min.css
+-rw-rw-rw-   0        0        0   116361 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/button.css
+-rw-rw-rw-   0        0        0    90207 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/button.min.css
+-rw-rw-rw-   0        0        0    25330 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/card.css
+-rw-rw-rw-   0        0        0    17410 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/card.min.css
+-rw-rw-rw-   0        0        0    17473 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.css
+-rw-rw-rw-   0        0        0    26912 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.js
+-rw-rw-rw-   0        0        0    12727 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.min.css
+-rw-rw-rw-   0        0        0    11369 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.min.js
+-rw-rw-rw-   0        0        0     8710 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/colorize.js
+-rw-rw-rw-   0        0        0     3270 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/colorize.min.js
+-rw-rw-rw-   0        0        0     5120 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/comment.css
+-rw-rw-rw-   0        0        0     2945 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/comment.min.css
+-rw-rw-rw-   0        0        0     3099 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/container.css
+-rw-rw-rw-   0        0        0     1925 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/container.min.css
+-rw-rw-rw-   0        0        0     5559 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.css
+-rw-rw-rw-   0        0        0    22303 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.js
+-rw-rw-rw-   0        0        0     3517 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.min.css
+-rw-rw-rw-   0        0        0     8071 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.min.js
+-rw-rw-rw-   0        0        0     8034 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/divider.css
+-rw-rw-rw-   0        0        0     6097 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/divider.min.css
+-rw-rw-rw-   0        0        0    37420 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.css
+-rw-rw-rw-   0        0        0   145962 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.js
+-rw-rw-rw-   0        0        0    25679 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.min.css
+-rw-rw-rw-   0        0        0    50895 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.min.js
+-rw-rw-rw-   0        0        0     3169 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.css
+-rw-rw-rw-   0        0        0    20926 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.js
+-rw-rw-rw-   0        0        0     1836 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.min.css
+-rw-rw-rw-   0        0        0     7728 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.min.js
+-rw-rw-rw-   0        0        0     5845 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/feed.css
+-rw-rw-rw-   0        0        0     3590 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/feed.min.css
+-rw-rw-rw-   0        0        0    22423 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/flag.css
+-rw-rw-rw-   0        0        0    18577 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/flag.min.css
+-rw-rw-rw-   0        0        0    29092 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.css
+-rw-rw-rw-   0        0        0    57618 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.js
+-rw-rw-rw-   0        0        0    21568 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.min.css
+-rw-rw-rw-   0        0        0    20458 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.min.js
+-rw-rw-rw-   0        0        0    73036 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/grid.css
+-rw-rw-rw-   0        0        0    57335 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/grid.min.css
+-rw-rw-rw-   0        0        0    13499 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/header.css
+-rw-rw-rw-   0        0        0     8872 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/header.min.css
+-rw-rw-rw-   0        0        0    86945 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/icon.css
+-rw-rw-rw-   0        0        0    67019 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/icon.min.css
+-rw-rw-rw-   0        0        0     5676 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/image.css
+-rw-rw-rw-   0        0        0     3727 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/image.min.css
+-rw-rw-rw-   0        0        0    12699 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/input.css
+-rw-rw-rw-   0        0        0     8692 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/input.min.css
+-rw-rw-rw-   0        0        0     9753 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/item.css
+-rw-rw-rw-   0        0        0     5985 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/item.min.css
+-rw-rw-rw-   0        0        0    28382 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/label.css
+-rw-rw-rw-   0        0        0    20005 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/label.min.css
+-rw-rw-rw-   0        0        0    22486 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/list.css
+-rw-rw-rw-   0        0        0    16094 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/list.min.css
+-rw-rw-rw-   0        0        0     7128 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/loader.css
+-rw-rw-rw-   0        0        0     4702 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/loader.min.css
+-rw-rw-rw-   0        0        0    45279 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/menu.css
+-rw-rw-rw-   0        0        0    31506 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/menu.min.css
+-rw-rw-rw-   0        0        0    12466 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/message.css
+-rw-rw-rw-   0        0        0     8354 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/message.min.css
+-rw-rw-rw-   0        0        0    12800 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.css
+-rw-rw-rw-   0        0        0    33442 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.js
+-rw-rw-rw-   0        0        0     8012 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.min.css
+-rw-rw-rw-   0        0        0    12701 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.min.js
+-rw-rw-rw-   0        0        0     2727 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.css
+-rw-rw-rw-   0        0        0    15553 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.js
+-rw-rw-rw-   0        0        0     1483 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.min.css
+-rw-rw-rw-   0        0        0     5696 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.min.js
+-rw-rw-rw-   0        0        0     5938 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/placeholder.css
+-rw-rw-rw-   0        0        0     4452 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/placeholder.min.css
+-rw-rw-rw-   0        0        0    17407 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.css
+-rw-rw-rw-   0        0        0    52273 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.js
+-rw-rw-rw-   0        0        0    12032 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.min.css
+-rw-rw-rw-   0        0        0    18630 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.min.js
+-rw-rw-rw-   0        0        0    10669 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.css
+-rw-rw-rw-   0        0        0    31204 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.js
+-rw-rw-rw-   0        0        0     7422 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.min.css
+-rw-rw-rw-   0        0        0    12331 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.min.js
+-rw-rw-rw-   0        0        0     2646 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rail.css
+-rw-rw-rw-   0        0        0     1453 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rail.min.css
+-rw-rw-rw-   0        0        0    20696 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.css
+-rw-rw-rw-   0        0        0    14869 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.js
+-rw-rw-rw-   0        0        0    18393 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.min.css
+-rw-rw-rw-   0        0        0     5354 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.min.js
+-rw-rw-rw-   0        0        0     9123 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reset.css
+-rw-rw-rw-   0        0        0     2822 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reset.min.css
+-rw-rw-rw-   0        0        0     8177 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reveal.css
+-rw-rw-rw-   0        0        0     5784 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reveal.min.css
+-rw-rw-rw-   0        0        0    10377 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.css
+-rw-rw-rw-   0        0        0    51211 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.js
+-rw-rw-rw-   0        0        0     6891 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.min.css
+-rw-rw-rw-   0        0        0    17622 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.min.js
+-rw-rw-rw-   0        0        0    20063 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/segment.css
+-rw-rw-rw-   0        0        0    13763 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/segment.min.css
+-rw-rw-rw-   0        0        0     3865 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.css
+-rw-rw-rw-   0        0        0    29873 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.js
+-rw-rw-rw-   0        0        0     2521 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.min.css
+-rw-rw-rw-   0        0        0    10803 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.min.js
+-rw-rw-rw-   0        0        0    15757 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.css
+-rw-rw-rw-   0        0        0    34488 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.js
+-rw-rw-rw-   0        0        0    10726 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.min.css
+-rw-rw-rw-   0        0        0    13466 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.min.js
+-rw-rw-rw-   0        0        0     3918 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.css
+-rw-rw-rw-   0        0        0    14604 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.js
+-rw-rw-rw-   0        0        0     2452 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.min.css
+-rw-rw-rw-   0        0        0     6066 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.min.js
+-rw-rw-rw-   0        0        0    21498 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/state.js
+-rw-rw-rw-   0        0        0     7804 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/state.min.js
+-rw-rw-rw-   0        0        0    13221 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/statistic.css
+-rw-rw-rw-   0        0        0     9594 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/statistic.min.css
+-rw-rw-rw-   0        0        0    23555 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/step.css
+-rw-rw-rw-   0        0        0    19188 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/step.min.css
+-rw-rw-rw-   0        0        0     1288 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.css
+-rw-rw-rw-   0        0        0    31814 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.js
+-rw-rw-rw-   0        0        0      607 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.min.css
+-rw-rw-rw-   0        0        0    11854 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.min.js
+-rw-rw-rw-   0        0        0     1865 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.css
+-rw-rw-rw-   0        0        0    33771 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.js
+-rw-rw-rw-   0        0        0     1075 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.min.css
+-rw-rw-rw-   0        0        0    11487 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.min.js
+-rw-rw-rw-   0        0        0    25536 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/table.css
+-rw-rw-rw-   0        0        0    18015 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/table.min.css
+-rw-rw-rw-   0        0        0    49176 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.css
+-rw-rw-rw-   0        0        0    36076 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.js
+-rw-rw-rw-   0        0        0    33525 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.min.css
+-rw-rw-rw-   0        0        0    13010 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.min.js
+-rw-rw-rw-   0        0        0     2346 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.css
+-rw-rw-rw-   0        0        0    16252 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.js
+-rw-rw-rw-   0        0        0     1328 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.min.css
+-rw-rw-rw-   0        0        0     6090 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.min.js
+-rw-rw-rw-   0        0        0    44180 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visibility.js
+-rw-rw-rw-   0        0        0    16294 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visibility.min.js
+-rw-rw-rw-   0        0        0    16142 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visit.js
+-rw-rw-rw-   0        0        0     5887 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visit.min.js
+-rw-rw-rw-   0        0        0      774 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/package.js
+-rw-rw-rw-   0        0        0      524 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/package.json
+-rw-rw-rw-   0        0        0   869203 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.css
+-rw-rw-rw-   0        0        0   759089 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.js
+-rw-rw-rw-   0        0        0   628944 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.min.css
+-rw-rw-rw-   0        0        0   275740 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.min.js
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/
+-rw-rw-rw-   0        0        0    98640 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.eot
+-rw-rw-rw-   0        0        0   508636 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.svg
+-rw-rw-rw-   0        0        0    98404 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.ttf
+-rw-rw-rw-   0        0        0    63728 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.woff
+-rw-rw-rw-   0        0        0    54488 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.woff2
+-rw-rw-rw-   0        0        0   106004 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.eot
+-rw-rw-rw-   0        0        0    93888 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.otf
+-rw-rw-rw-   0        0        0   392355 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.svg
+-rw-rw-rw-   0        0        0   105784 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.ttf
+-rw-rw-rw-   0        0        0    50524 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.woff
+-rw-rw-rw-   0        0        0    40148 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.woff2
+-rw-rw-rw-   0        0        0    31156 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.eot
+-rw-rw-rw-   0        0        0   107567 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.svg
+-rw-rw-rw-   0        0        0    30928 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.ttf
+-rw-rw-rw-   0        0        0    14712 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.woff
+-rw-rw-rw-   0        0        0    12240 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.woff2
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/images/
+-rw-rw-rw-   0        0        0    28123 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/images/flags.png
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/jQuery/
+-rw-rw-rw-   0        0        0    86713 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/jQuery/jquery-3.1.1.min.js
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/
+-rw-rw-rw-   0        0        0     4916 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/auth.xhtml
+-rw-rw-rw-   0        0        0     2339 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/badAuth.xhtml
+-rw-rw-rw-   0        0        0   112922 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/favicon.ico
+-rw-rw-rw-   0        0        0     4093 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/footer.xhtml
+-rw-rw-rw-   0        0        0     3709 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/header.xhtml
+-rw-rw-rw-   0        0        0    15975 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/logo.png
+-rw-rw-rw-   0        0        0    44545 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/orc.js
+-rw-rw-rw-   0        0        0    19223 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/orc.xhtml
+-rw-rw-rw-   0        0        0     1913 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std.css
+-rw-rw-rw-   0        0        0    86103 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std.js
+-rw-rw-rw-   0        0        0    67072 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std.xhtml
+-rw-rw-rw-   0        0        0    21304 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std_browser.js
+-rw-rw-rw-   0        0        0    25795 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std_desktop.js
+-rw-rw-rw-   0        0        0    26642 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std_desktop_linux.js
+-rw-rw-rw-   0        0        0      916 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std_floidd.css
+-rw-rw-rw-   0        0        0    40351 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std_floidd.js
+-rw-rw-rw-   0        0        0    18231 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std_helper.js
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/
+-rw-rw-rw-   0        0        0   184912 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/Lato-Bold.woff2
+-rw-rw-rw-   0        0        0   195704 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/Lato-Italic.woff2
+-rw-rw-rw-   0        0        0   182708 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/Lato-Regular.woff2
+-rw-rw-rw-   0        0        0   251041 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg1.jpg
+-rw-rw-rw-   0        0        0   256648 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg10.jpg
+-rw-rw-rw-   0        0        0   249670 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg2.jpg
+-rw-rw-rw-   0        0        0   245168 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg3.jpg
+-rw-rw-rw-   0        0        0   258568 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg4.jpg
+-rw-rw-rw-   0        0        0   261562 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg5.jpg
+-rw-rw-rw-   0        0        0   260686 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg6.jpg
+-rw-rw-rw-   0        0        0   261376 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg7.jpg
+-rw-rw-rw-   0        0        0   261288 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg8.jpg
+-rw-rw-rw-   0        0        0   261559 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg9.jpg
+-rw-rw-rw-   0        0        0    55821 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/docs.css
+-rw-rw-rw-   0        0        0    55845 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/docs.css.bak
+-rw-rw-rw-   0        0        0    44749 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/docs.js
+-rw-rw-rw-   0        0        0    37642 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/dropdown.css
+-rw-rw-rw-   0        0        0     3794 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/easing.min.js
+-rw-rw-rw-   0        0        0    13723 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/header.css
+-rw-rw-rw-   0        0        0    21964 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/highlight.min.js
+-rw-rw-rw-   0        0        0    16245 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/home.css
+-rw-rw-rw-   0        0        0     8926 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/home.js
+-rw-rw-rw-   0        0        0    84349 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/jquery.min.js
+-rw-rw-rw-   0        0        0   136781 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/less.min.js
+-rw-rw-rw-   0        0        0        2 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/metadata.json
+-rw-rw-rw-   0        0        0    23839 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/nan.jpg
+-rw-rw-rw-   0        0        0   242713 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/ogImage.JPG
+-rw-rw-rw-   0        0        0   131928 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/ogImage.PNG
+-rw-rw-rw-   0        0        0     4899 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/pyOpenRPA_logo.png
+-rw-rw-rw-   0        0        0    20287 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/segment.css
+-rw-rw-rw-   0        0        0    34482 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/sidebar.js
+-rw-rw-rw-   0        0        0    36070 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/transition.js
+-rw-rw-rw-   0        0        0    44174 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/visibility.js
+-rw-rw-rw-   0        0        0     5951 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/white-image.png
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/
+-rw-rw-rw-   0        0        0    22176 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Audio.py
+-rw-rw-rw-   0        0        0     1992 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Clipboard.py
+-rw-rw-rw-   0        0        0    44824 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Keyboard.py
+-rw-rw-rw-   0        0        0    16980 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Mouse.py
+-rw-rw-rw-   0        0        0    20445 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/OrchestratorConnector.py
+-rw-rw-rw-   0        0        0     1623 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/README.md
+-rw-rw-rw-   0        0        0    74562 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Screen.py
+-rw-rw-rw-   0        0        0     1453 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/SettingsTemplate.py
+-rw-rw-rw-   0        0        0     2878 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Test.py
+-rw-rw-rw-   0        0        0   218957 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/UIDesktop.py
+-rw-rw-rw-   0        0        0    91914 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/UIWeb.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/
+-rw-rw-rw-   0        0        0     3884 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/JSONNormalize.py
+-rw-rw-rw-   0        0        0    24149 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/LCompatibility.py
+-rw-rw-rw-   0        0        0     4810 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/ProcessBitness.py
+-rw-rw-rw-   0        0        0     8039 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/ProcessCommunicator.py
+-rw-rw-rw-   0        0        0      961 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/TimerRepeat.py
+-rw-rw-rw-   0        0        0      777 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/ValueVerify.py
+-rw-rw-rw-   0        0        0     2789 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/WCompatibility.py
+-rw-rw-rw-   0        0        0       28 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/__init__.py
+-rw-rw-rw-   0        0        0     1318 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/Window.py
+-rw-rw-rw-   0        0        0      255 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/__init__.py
+-rw-rw-rw-   0        0        0     2029 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Robot/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Studio/
+-rw-rw-rw-   0        0        0     3341 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Studio/JSONNormalize.py
+-rw-rw-rw-   0        0        0     7912 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Studio/ProcessCommunicator.py
+-rw-rw-rw-   0        0        0     6740 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Studio/Processor.py
+-rw-rw-rw-   0        0        0     5038 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Studio/RobotConnector.py
+-rw-rw-rw-   0        0        0    28581 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Studio/Studio.py
+-rw-rw-rw-   0        0        0      777 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Studio/ValueVerify.py
+-rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Studio/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Studio/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/
+-rw-rw-rw-   0        0        0       29 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/CrossOS.py
+-rw-rw-rw-   0        0        0       30 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/Debugger.py
+-rw-rw-rw-   0        0        0       29 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/License.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotDB/
+-rw-rw-rw-   0        0        0      343 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotDB/ExcelCom.py
+-rw-rw-rw-   0        0        0     1473 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotDB/HowToUse
+-rw-rw-rw-   0        0        0     1655 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotDB/RobotDB.py
+-rw-rw-rw-   0        0        0    20087 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotDB/Server.py
+-rw-rw-rw-   0        0        0     7406 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotDB/ServerSettings.py
+-rw-rw-rw-   0        0        0      124 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotDB/__init__.py
+-rw-rw-rw-   0        0        0      140 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotDB/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotScreenActive/
+-rwxrwxrwx   0        0        0      114 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotScreenActive/ConsoleStart.bat
+-rw-rw-rw-   0        0        0      492 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotScreenActive/Monitor.py
+-rw-rw-rw-   0        0        0      606 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotScreenActive/Screen.py
+-rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotScreenActive/__init__.py
+-rw-rw-rw-   0        0        0      593 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotScreenActive/__main__.py
+-rw-rw-rw-   0        0        0       30 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/StopSafe.py
+-rw-rw-rw-   0        0        0     5507 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/Template.py
+-rw-rw-rw-   0        0        0     2998 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/Usage.py
+-rw-rw-rw-   0        0        0        0 2022-10-12 17:40:40.000000 pyOpenRPA-1.4.1/pyOpenRPA/Tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/Administrator/
+-rw-rw-rw-   0        0        0     6941 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/Administrator/__main__.py
+-rw-rw-rw-   0        0        0     3539 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/CrossOS.py
+-rw-rw-rw-   0        0        0      570 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/Debugger.py
+-rw-rw-rw-   0        0        0     2261 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/Dictionary.py
+-rw-rw-rw-   0        0        0     1848 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/Disk.py
+-rw-rw-rw-   0        0        0     8647 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/License.py
+-rw-rw-rw-   0        0        0      600 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/Network.py
+-rw-rw-rw-   0        0        0     6720 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/Render.py
+-rw-rw-rw-   0        0        0     5930 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/SSH.py
+-rw-rw-rw-   0        0        0     2346 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/StopSafe.py
+-rw-rw-rw-   0        0        0      214 2023-07-04 08:32:07.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/Text.py
+-rw-rw-rw-   0        0        0     8630 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/pyOpenRPA/Utils/__define__.py
+-rw-rw-rw-   0        0        0      154 2023-07-04 08:44:29.000000 pyOpenRPA-1.4.1/pyOpenRPA/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA.egg-info/
+-rw-rw-rw-   0        0        0     4334 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18772 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-10 19:47:56.000000 pyOpenRPA-1.4.1/pyOpenRPA.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      393 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/pyOpenRPA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 08:44:30.000000 pyOpenRPA-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     3367 2023-07-04 08:44:21.000000 pyOpenRPA-1.4.1/setup.py
```

### Comparing `pyOpenRPA-1.4.0/PKG-INFO` & `pyOpenRPA-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyOpenRPA
-Version: 1.4.0
+Version: 1.4.1
 Summary: The powerful open source RPA platform for business
 Home-page: https://pyopenrpa.ru/
 Author: Ivan Maslov
 Author-email: Ivan.Maslov@pyopenrpa.ru
 License: Текст лицензии см. в файле: LICENSE.PDF (в корне) или по адресу: https://pyopenrpa.ru/license/oferta.pdf
 Description: <!-- pyOpenRPA documentation master file, created by
         sphinx-quickstart on Sat Dec 19 23:59:00 2020.
@@ -55,15 +55,15 @@
         Ivan Maslov contacts (CEO & FOUNDER): 
         
         - E-mail: Ivan.Maslov@pyOpenRPA.ru
         - Skype: MegaFinder
         - Web: https://pyopenrpa.ru/
         - Telegram: https://t.me/pyopenrpa
         - WhatsApp | Telegram: +7 906 722 39 25 | @IvanMaslov
-Keywords: pyOpenRPA OpenRPA RPA Robot Automation Robotization OpenSource IT4Business
+Keywords: pyOpenRPA ORPA OpenRPA RPA Robot Automation Robotization OpenSource
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Free For Educational Use
 Classifier: License :: Free For Home Use
 Classifier: License :: Free for non-commercial use
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Agent/A2O.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Agent/A2O.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Agent/O2A.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Agent/O2A.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Agent/Processor.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Agent/Processor.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Agent/__Agent__.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Agent/__Agent__.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/LICENSE.pdf` & `pyOpenRPA-1.4.1/pyOpenRPA/LICENSE.pdf`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/BackwardCompatibility.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/BackwardCompatibility.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Core.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Core.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Managers/ControlPanel.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Managers/ControlPanel.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Managers/Git.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Managers/Git.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Managers/Process.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Managers/Process.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Processor.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Processor.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/ProcessorOld.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/ProcessorOld.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/CMDStr.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/CMDStr.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Clipboard.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Clipboard.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Connector.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Connector.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/ConnectorExceptions.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/ConnectorExceptions.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Processor.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Processor.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Recovery.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Recovery.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/RobotRDPActive.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/RobotRDPActive.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Scheduler.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Scheduler.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Template.rdp` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Template.rdp`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/Timer.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/Timer.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotRDPActive/__main__.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotRDPActive/__main__.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotScreenActive/Monitor.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotScreenActive/Monitor.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotScreenActive/Screen.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotScreenActive/Screen.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/RobotScreenActive/__main__.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/RobotScreenActive/__main__.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Server.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Server.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/ServerBC.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/ServerBC.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/ServerSettings.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/ServerSettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from . import SettingsTemplate
 from fastapi import FastAPI, Form, Request, HTTPException, Depends, Header, Response, Body
 from fastapi.responses import PlainTextResponse, HTMLResponse, FileResponse
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 from pydantic import BaseModel
 import io
+import subprocess
 from starlette.responses import StreamingResponse
 from typing import Union
 from fastapi.responses import JSONResponse
 import asyncio
 
 # # # # # # # # # # # #
 # v 1.2.0 Functionallity
@@ -208,15 +209,15 @@
         SaveScreenshot("screenshot.png")
         lFileObject = open("screenshot.png", "rb")
         # Write content as utf-8 data
         lImage = lFileObject.read()
         # Закрыть файловый объект
         lFileObject.close()
     else: 
-        pyscreeze._screenshot_linux(imageFilename='screenshot.png')
+        result = subprocess.run(["scrot", "--file", "screenshot.png", "-o"])
         lFileObject = open("screenshot.png", "rb")
         # Write content as utf-8 data
         lImage = lFileObject.read()
         # Закрыть файловый объект
         lFileObject.close()
     return StreamingResponse(io.BytesIO(lImage), media_type="image/png")
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/SettingsTemplate.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/SettingsTemplate.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Timer.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Timer.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Utils/LoggerHandlerDumpLogList.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Utils/LoggerHandlerDumpLogList.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/Web/Basic.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/Web/Basic.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Orchestrator/__Orchestrator__.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Orchestrator/__Orchestrator__.py`

 * *Files 2% similar despite different names*

```diff
@@ -628,14 +628,22 @@
     """L+,W+: Проверить, активирована ли авторизация при переходе к Оркестратору. 
 
     :return: True - Активирована; False - Деактивирована
     """
     inGSettings = GSettingsGet()
     return inGSettings["ServerDict"]["AccessUsers"]["FlagCredentialsAsk"]
 
+def OrchestratorSetCredentialsAsk(inCredentialAskBool=True):
+    """L+,W+: Установить авторизацию при входе на Оркестратор. 
+
+    :param inCredentialAskBool: True - Активировать авторизацию; False - Деактивировать авторизацию
+    """
+    inGSettings = GSettingsGet()
+    inGSettings["ServerDict"]["AccessUsers"]["FlagCredentialsAsk"]=inCredentialAskBool
+
 def OrchestratorIsInited() -> bool:
     """L+,W+: Проверить, было ли проинициализировано ядро Оркестратора
 
     :return: True - Ядро Оркестратора было проинициализировано; False - Требуется время на инициализацию
     :rtype: bool
     """    
 
@@ -1726,15 +1734,15 @@
     for lModuleItemStr in lSysModulesSnapshot:
         lModuleItem = lSysModulesSnapshot[lModuleItemStr]
         for lDefItemStr in dir(lModuleItem):
             try:
                 lDefItem = getattr(lModuleItem,lDefItemStr)
                 if callable(lDefItem) and not lDefItemStr.startswith("_"):
                     ActivityItemDefAliasCreate(inDef=lDefItem, inAliasStr=f"{lModuleItemStr}.{lDefItemStr}")
-            except ModuleNotFoundError:
+            except Exception:
                 pass
     lL.info(f"Синонимы функций: окончание инициализации sys.modules")
 
 def ActivityItemDefAliasUpdate(inDef, inAliasStr, inGSettings = None):
     """L+,W+: Обновить синоним (текстовый ключ) для инициации выполнения функции в том случае, если запрос на выполнения пришел из вне (передача функций невозможна). 
     
     .. code-block:: python
@@ -2845,14 +2853,16 @@
     # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 from .. import __version__ # Get version from the package
 
 def Start(inDumpRestoreBool = True, inRunAsAdministratorBool = True):
     Orchestrator(inDumpRestoreBool = True, inRunAsAdministratorBool = True)
 
+from pyOpenRPA.Robot import Keyboard
+
 def Orchestrator(inGSettings=None, inDumpRestoreBool = True, inRunAsAdministratorBool = True):
     """L+,W+: Инициализация ядра Оркестратора (всех потоков)
 
     :param inGSettings: Глобальный словарь настроек Оркестратора (синглтон)
     :param inDumpRestoreBool: True - Восстановить информацию о RDP сессиях и StorageDict; False - не восстанавливать
     :param inRunAsAdministratorBool: True - Проверить права администратратора и обеспечить их; False - Не обеспечивать права администратора
     """
@@ -2917,18 +2927,29 @@
         # Init the RobotScreenActive in another thread
         lRobotScreenActiveThread = threading.Thread(target= Monitor.CheckScreen)
         lRobotScreenActiveThread.daemon = True # Run the thread in daemon mode.
         lRobotScreenActiveThread.setName("SCREEN_ACTIVE")
         lRobotScreenActiveThread.start() # Start the thread execution.
         if lL: lL.info("Модуль активного рабочего стола инициализирован")  #Logging
 
-        # Init hotkey to restart orchestrator (LEFT CTRL + LEFT ALT + X)
-        keyboard.add_hotkey("ctrl+alt+x", OrchestratorRestart)
-        if lL: lL.info("Хоткей для перезапуска --> CTRL + ALT + X")  #Logging
-
+        # Init hotkey to restart orchestrator (LEFT CTRL + LEFT ALT + X) 1.4.1 ONLY FOR WINDOWS BECAUSE FOR LINUX THE SUDO IS REQUIRED (NEED TEST)
+        if CrossOS.IS_WINDOWS_BOOL:
+            keyboard.add_hotkey("ctrl+alt+x", OrchestratorRestart)
+            if lL: lL.info("Хоткей для перезапуска --> CTRL + ALT + X")  #Logging
+        else:
+            def hook_restart():
+                while True:
+                    if Keyboard.IsDown("ctrl") and Keyboard.IsDown("alt") and Keyboard.IsDown("x"):
+                        OrchestratorRestart()
+                        break
+                    time.sleep(0.4)
+            lKBDHOOKRESTARTThread = threading.Thread(target= hook_restart)
+            lKBDHOOKRESTARTThread.daemon = True # Run the thread in daemon mode.
+            lKBDHOOKRESTARTThread.setName("KBD_HOOK_RESTART")
+            lKBDHOOKRESTARTThread.start() # Start the thread execution.
         # Init the RobotRDPActive in another thread
         lRobotRDPThreadControlDict = {"ThreadExecuteBool":True} # inThreadControlDict = {"ThreadExecuteBool":True}
         lRobotRDPActiveThread = threading.Thread(target= RobotRDPActive.RobotRDPActive, kwargs={"inGSettings":gSettingsDict, "inThreadControlDict":lRobotRDPThreadControlDict})
         lRobotRDPActiveThread.daemon = True # Run the thread in daemon mode.
         lRobotRDPActiveThread.setName("RDP_CONNECT")
         lRobotRDPActiveThread.start() # Start the thread execution.
         if lL: lL.info("Модуль подключения по РДП инициализированн")  #Logging
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/README.md` & `pyOpenRPA-1.4.1/pyOpenRPA/README.md`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Google/LatoItalic.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Google/LatoItalic.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Handlebars/handlebars-v4.1.2.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Handlebars/handlebars-v4.1.2.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/JsRender/jsrender.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/JsRender/jsrender.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/LICENSE` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/LICENSE`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/accordion.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/ad.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/ad.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/ad.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/ad.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/api.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/api.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/api.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/api.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/breadcrumb.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/breadcrumb.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/breadcrumb.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/breadcrumb.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/button.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/button.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/button.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/button.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/card.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/card.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/card.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/card.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/checkbox.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/colorize.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/colorize.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/colorize.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/colorize.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/comment.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/comment.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/comment.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/comment.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/container.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/container.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/container.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/container.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dimmer.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/divider.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/divider.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/divider.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/divider.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/dropdown.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/embed.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/feed.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/feed.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/feed.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/feed.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/flag.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/flag.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/flag.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/flag.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/form.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/grid.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/grid.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/grid.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/grid.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/header.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/header.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/header.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/header.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/icon.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/icon.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/icon.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/icon.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/image.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/image.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/image.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/image.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/input.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/input.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/input.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/input.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/item.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/item.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/item.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/item.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/label.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/label.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/label.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/label.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/list.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/list.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/list.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/list.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/loader.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/loader.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/loader.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/loader.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/menu.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/menu.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/menu.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/menu.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/message.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/message.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/message.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/message.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/modal.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/nag.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/placeholder.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/placeholder.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/placeholder.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/placeholder.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/popup.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/progress.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rail.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rail.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rail.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rail.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/rating.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reset.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reset.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reset.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reset.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reveal.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reveal.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reveal.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/reveal.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/search.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/segment.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/segment.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/segment.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/segment.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/shape.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sidebar.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/site.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/state.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/state.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/state.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/state.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/statistic.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/statistic.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/statistic.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/statistic.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/step.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/step.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/step.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/step.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/sticky.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/tab.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/table.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/table.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/table.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/table.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/transition.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/video.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visibility.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visibility.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visibility.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visibility.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visit.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visit.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visit.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/components/visit.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/package.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/package.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/package.json` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/package.json`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.min.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.min.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/semantic.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.eot` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.eot`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.svg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.svg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.ttf` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.ttf`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.woff` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.woff`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.woff2` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.eot` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.eot`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.otf` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.otf`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.svg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.svg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.ttf` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.ttf`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.woff` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.woff2` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/icons.woff2`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.eot` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.eot`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.svg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.svg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.ttf` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.ttf`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.woff` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.woff`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.woff2` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/fonts/outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/images/flags.png` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/Semantic-UI-CSS-master/themes/default/assets/images/flags.png`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/jQuery/jquery-3.1.1.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/jQuery/jquery-3.1.1.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/auth.xhtml` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/auth.xhtml`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/badAuth.xhtml` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/badAuth.xhtml`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/favicon.ico` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/footer.xhtml` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/footer.xhtml`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/header.xhtml` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/header.xhtml`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/logo.png` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/logo.png`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/orc.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/orc.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/orc.xhtml` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/orc.xhtml`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -156,41 +156,42 @@
     code_generate = () => {
         var selector_textarea = document.getElementById(this.html_id_str)
         var code_str = "'" + selector_textarea.value + "'"
         if (this.mode_str == "UIO") {
             code_str = selector_textarea.value
         }
         code_str = replaceAll(code_str, "\n", "")
+        code_str = orpa_utils_json_2_python(code_str)
         clipboard_set(code_str)
     }
 
     code_highlight_generate = () => {
         if (this.module_type_str == "DESKTOP") {
             var code_str = `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nUIDesktop.UIOSelector_FocusHighlight(uio_selector)`
-            code_str = replaceAll(code_str, "<SELECTOR>", JSON.stringify(this.uio_get()))
+            code_str = replaceAll(code_str, "<SELECTOR>", orpa_utils_json_2_python(JSON.stringify(this.uio_get())))
             clipboard_set(code_str)
         } else {
             var page_url_str = document.getElementById("orpa-browser-driver-tab-url").value
             var code_str = `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIWeb\nUIWeb.BrowserChromeStart() #!Удалить, если браузер уже открыт\nUIWeb.PageOpen("<PAGE_URL>")#!Удалить, если страница уже открыта\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nUIWeb.UIOSelectorFocusHighlight(uio_selector)`
-            code_str = replaceAll(code_str, "<SELECTOR>", JSON.stringify(this.uio_get()))
+            code_str = replaceAll(code_str, "<SELECTOR>", orpa_utils_json_2_python(JSON.stringify(this.uio_get())))
             code_str = replaceAll(code_str, "<PAGE_URL>", page_url_str)
             clipboard_set(code_str)
         }
     }
 
 
     code_locate_all_generate = () => {
         if (this.module_type_str == "DESKTOP") {
             var code_str = `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nUIDesktop.UIOSelector_Get_UIOList(uio_selector)`
-            code_str = replaceAll(code_str, "<SELECTOR>", JSON.stringify(this.uio_get()))
+            code_str = replaceAll(code_str, "<SELECTOR>", orpa_utils_json_2_python(JSON.stringify(this.uio_get())))
             clipboard_set(code_str)
         } else {
             var page_url_str = document.getElementById("orpa-browser-driver-tab-url").value
             var code_str = `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIWeb\nUIWeb.BrowserChromeStart() #!Удалить, если браузер уже открыт\nUIWeb.PageOpen("<PAGE_URL>")#!Удалить, если страница уже открыта\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nuio_list = UIWeb.UIOSelectorList(uio_selector)`
-            code_str = replaceAll(code_str, "<SELECTOR>", JSON.stringify(this.uio_get()))
+            code_str = replaceAll(code_str, "<SELECTOR>", orpa_utils_json_2_python(JSON.stringify(this.uio_get())))
             code_str = replaceAll(code_str, "<PAGE_URL>", page_url_str)
             clipboard_set(code_str)
         }
     }
 
     //Стрелочная функция для того, чтобы объект this не переопределялся из за html onchange объекта, а оставался экземпляром класса
     on_change = () => {
@@ -354,20 +355,27 @@
             }
         } catch (error) {
             return false
         }
     }
     ui_highlight = function() {
         var l_action_str = ""
-        if (this.module_type_str == "DESKTOP") {
-            l_action_str = "pyOpenRPA.Robot.UIDesktop.UIOSelector_FocusHighlight"
+        if (this.uio != null) {
+            if (this.module_type_str == "DESKTOP") {
+                l_action_str = "pyOpenRPA.Robot.UIDesktop.UIOSelector_FocusHighlight"
+            } else {
+                l_action_str = "pyOpenRPA.Robot.UIWeb.UIOSelectorFocusHighlight"
+            }
+            orpa_api_activity_list_execute_async(function() {}, l_action_str, [this.uio]);
+
         } else {
-            l_action_str = "pyOpenRPA.Robot.UIWeb.UIOSelectorFocusHighlight"
+
+            orpa_helper_info('orpa_desktop_selector_empty');
         }
-        orpa_api_activity_list_execute_async(function() {}, l_action_str, [this.uio]);
+
 
     }
     clear = function() {
         this.uio = null
         var selector_textarea = document.getElementById(this.html_id_str)
         selector_textarea.value = ""
     }
@@ -424,32 +432,40 @@
     }
     __ = function() {
         // IN CODE REPLACE THE <SELECTOR> STR to the selector
         if (this.data["is_tab_desktop_bool"]) {
             this.help_function_list = [
                 "Exists",
                 "Highlight",
+                "Focus",
                 "FocusHighlight",
                 "WaitAppear",
                 "WaitAppearList",
                 "WaitDisappear",
                 "WaitDisappearList",
+                "Click",
+                "ClickRight",
+                "ClickDouble",
                 "TryRestore",
                 "GetActivityList",
                 "GetLevelList"
             ]
             this.help_code_generator_dict = {
                 "Exists": {
                     "help_str": "Код Python скопирован в буфер обмена.\nФункция проверяет наличие UI объекта по UIO селектору.",
                     "code_str": `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nuio_exists_bool = UIDesktop.UIOSelector_Exist_Bool(uio_selector)`
                 },
                 "Highlight": {
                     "help_str": "Код Python скопирован в буфер обмена.\nФункция выполняет посвечивание обнаруженного UI объекта по UIO селектору",
                     "code_str": `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nUIDesktop.UIOSelector_Highlight(uio_selector)`
                 },
+                "Focus": {
+                    "help_str": "Код Python скопирован в буфер обмена.\nФункция выполняет фокусировку на объект по UIO селектору",
+                    "code_str": `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nUIDesktop.UIOSelector_Focus(uio_selector)`
+                },
                 "FocusHighlight": {
                     "help_str": "Код Python скопирован в буфер обмена.\nФункция выполняет фокусировку на объект и посвечивание обнаруженного UI объекта по UIO селектору",
                     "code_str": `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nUIDesktop.UIOSelector_FocusHighlight(uio_selector)`
                 },
                 "WaitAppear": {
                     "help_str": "Код Python скопирован в буфер обмена.\nФункция ожидает появления хотя бы обного UI объекта по UIO селектору.\n\n:параметр inWaitSecs: Количество секунд, которые отвести на ожидание UIO объекта. По умолчанию 24 часа (86400 секунд)\n:параметр inFlagRaiseException (опционально): True - формировать ошибку exception, если платформа не обнаружина ни одного UIO объекта по заданному UIO селектору. False - обратный случай (может привести к ошибочным результатам). По умолчанию True.",
                     "code_str": `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nUIDesktop.UIOSelectorSecs_WaitAppear_Bool (uio_selector,inWaitSecs=60, inFlagRaiseException=True)`
@@ -466,14 +482,26 @@
                     "help_str": "Код Python скопирован в буфер обмена.\nФункция ожидает момента, когда на экране не будет доступно ни одного UI объекта из списка UIO селекторов.\n\n:параметр inWaitSecs: Количество секунд, которые отвести на ожидание UIO объекта. По умолчанию 24 часа (86400 секунд)\n:параметр inFlagRaiseException (опционально): True - формировать ошибку exception, если платформа не обнаружина ни одного UIO объекта по заданному UIO селектору. False - обратный случай (может привести к ошибочным результатам). По умолчанию True.",
                     "code_str": `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nuio_selector_list = [uio_selector]\ndisappeared_index_list = UIDesktop.UIOSelectorsSecs_WaitDisappear_List(uio_selector_list,inWaitSecs=60,inFlagWaitAllInMoment=True, inFlagRaiseException=True)`
                 },
                 "TryRestore": {
                     "help_str": "Код Python скопирован в буфер обмена.\nФункция пытается восстановить окно приложения, если оно было свернуто. Окно идентифицируется по установленному UIO селектору",
                     "code_str": `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nUIDesktop.UIOSelector_TryRestore_Dict(uio_selector)`
                 },
+                "Click": {
+                    "help_str": "Код Python скопирован в буфер обмена.\nФункция пытается восстановить окно приложения, если оно было свернуто. Окно идентифицируется по установленному UIO селектору",
+                    "code_str": `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nUIDesktop.UIOSelector_Click(uio_selector, inRuleStr = "CC", inFocusBool = True)`
+                },
+                "ClickRight": {
+                    "help_str": "Код Python скопирован в буфер обмена.\nФункция пытается восстановить окно приложения, если оно было свернуто. Окно идентифицируется по установленному UIO селектору",
+                    "code_str": `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nUIDesktop.UIOSelector_ClickRight(uio_selector, inRuleStr = "CC", inFocusBool = True)`
+                },
+                "ClickDouble": {
+                    "help_str": "Код Python скопирован в буфер обмена.\nФункция пытается восстановить окно приложения, если оно было свернуто. Окно идентифицируется по установленному UIO селектору",
+                    "code_str": `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nUIDesktop.UIOSelector_ClickDouble(uio_selector, inRuleStr = "CC", inFocusBool = True)`
+                },
                 "GetActivityList": {
                     "help_str": "Код Python скопирован в буфер обмена.\nФункция возвращает список функций / свойств, доступных для UI объекта по установленному UIO селектору",
                     "code_str": `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nactivity_list = UIDesktop.UIOSelector_Get_UIOActivityList(uio_selector)\n#UIOSelectorUIOActivity_Run_Dict(uio_selector, inActionName="click_input")`
                 },
                 "GetLevelList": {
                     "help_str": "Код Python скопирован в буфер обмена.\nФункция возвращает список атрибутов, обнаруженных на всех родительских уровнях до UI объекта по UIO селектору",
                     "code_str": `#Импорт библиотеки\nfrom pyOpenRPA.Robot import UIDesktop\n#Установить селектор и вызвать функцию\nuio_selector = <SELECTOR>\nlevel_info_list = UIDesktop.UIOSelector_LevelInfo_List(uio_selector)`
@@ -578,30 +606,30 @@
     }
     code_run_generate = (is_focus_bool = false) => {
         if (this.data.is_tab_desktop_bool == true) {
             if (this.data.is_module_bool) {
                 var in_value = this.data.function_str
                 if (in_value != "") {
                     var code_str = this.help_code_generator_dict[in_value].code_str
-                    code_str = replaceAll(code_str, "<SELECTOR>", JSON.stringify(this.data["uio_selector"]))
+                    code_str = replaceAll(code_str, "<SELECTOR>", orpa_utils_json_2_python(JSON.stringify(this.data["uio_selector"])))
                     clipboard_set(code_str)
                 }
             } else {
                 `
         from pyOpenRPA.Robot import UIDesktop #Импорт (удалить, если импортировано ранее)
         # Установить селектор, получить UI объект, выполнить действие
         uio_selector = []
         uio = UIDesktop.UIOSelector_Get_UIO(uio_selector)
         uio.set_focus()
         result = uio.<FUNC>(*<JSON_LIST>)
         result = uio.<FUNC>(**<JSON_DICT>)
         `
                 var code_str = `from pyOpenRPA.Robot import UIDesktop #Импорт (удалить, если импортировано ранее)
 # Установить селектор, получить UI объект, выполнить действие`
-                code_str += `\nuio_selector = ` + JSON.stringify(this.data["uio_selector"])
+                code_str += `\nuio_selector = ` + orpa_utils_json_2_python(JSON.stringify(this.data["uio_selector"]))
                 code_str += `\nuio = UIDesktop.UIOSelector_Get_UIO(uio_selector)`
                 if (is_focus_bool == true) {
                     code_str += `\nuio.set_focus()`
                 }
                 if (this.data["is_function_bool"]) {
                     if (this.data["args_is_dict"] == true) {
                         code_str += `\nresult = uio.` + this.data["function_str"] + "(**" + orpa_utils_json_2_python(this.data["args_value_dict_str"]) + ")"
@@ -615,15 +643,15 @@
             }
         } else {
             if (this.data.is_module_bool) {
                 var in_value = this.data.function_str
                 if (in_value != "") {
                     var page_url_str = document.getElementById("orpa-browser-driver-tab-url").value
                     var code_str = this.help_code_generator_dict[in_value].code_str
-                    code_str = replaceAll(code_str, "<SELECTOR>", JSON.stringify(this.data["uio_selector"]))
+                    code_str = replaceAll(code_str, "<SELECTOR>", orpa_utils_json_2_python(JSON.stringify(this.data["uio_selector"])))
                     code_str = replaceAll(code_str, "<PAGE_URL>", page_url_str)
                     clipboard_set(code_str)
                 }
             } else {
                 `
         from pyOpenRPA.Robot import UIWeb #Импорт (удалить, если импортировано ранее)
         # Установить селектор, получить UI объект, выполнить действие
@@ -634,15 +662,15 @@
         result = uio.<FUNC>(**<JSON_DICT>)
         `
                 var page_url_str = document.getElementById("orpa-browser-driver-tab-url").value
                 var code_str = `from pyOpenRPA.Robot import UIWeb #Импорт (удалить, если импортировано ранее)
 UIWeb.BrowserChromeStart() #!Удалить, если браузер уже открыт
 UIWeb.PageOpen("<PAGE_URL>")#!Удалить, если страница уже открыта
 # Установить селектор, получить UI объект, выполнить действие`
-                code_str += `\nuio_selector = ` + JSON.stringify(this.data["uio_selector"])
+                code_str += `\nuio_selector = ` + orpa_utils_json_2_python(JSON.stringify(this.data["uio_selector"]))
                 code_str += `\nuio = UIWeb.UIOSelectorFirst(uio_selector)`
                 if (is_focus_bool == true) {
                     code_str += `\nUIWeb.BrowserFocus()`
                 }
                 if (this.data["is_function_bool"]) {
                     if (this.data["args_is_dict"] == true) {
                         code_str += `\nresult = uio.` + this.data["function_str"] + "(**" + orpa_utils_json_2_python(this.data["args_value_dict_str"]) + ")"
@@ -1139,15 +1167,15 @@
                 dataType: "text",
                 async: false
             });
             try {
 
                 data_json = JSON.parse(l_response_data)
                 if ("ErrorHeader" in data_json) {
-                    if (data_json["ErrorTraceback"].indexOf("pywinauto.findwindows.ElementNotFoundError") != -1) {
+                    if (data_json["ErrorTraceback"].indexOf("There are no UI elements by selector (UIO / XPATH / CSS)") != -1) {
                         orpa_utils_modal_uio_no_elements();
                     } else {
 
                         orpa_workspace_modal_show("GUI Error", data_json.ErrorHeader + " \nTraceback: " + data_json.ErrorTraceback);
                         throw new Error('Со стороны сервера поступила ошибка - прервать обработку JS');
                     }
 
@@ -1181,15 +1209,15 @@
                 url: '/api/activity-list-execute',
                 data: JSON.stringify(in_activity_list),
                 success: function(in_data) {
                     data_json = JSON.parse(in_data)
                     data_json.forEach(element => {
                         try {
                             if ("ErrorHeader" in element) {
-                                if (element["ErrorTraceback"].indexOf("pywinauto.findwindows.ElementNotFoundError") != -1) {
+                                if (element["ErrorTraceback"].indexOf("There are no UI elements by selector (UIO / XPATH / CSS)") != -1) {
                                     orpa_utils_modal_uio_no_elements();
                                 } else {
 
                                     orpa_workspace_modal_show("GUI Error", element.ErrorHeader + " \nTraceback: " + element.ErrorTraceback);
                                     throw new Error('Со стороны сервера поступила ошибка - прервать обработку JS');
                                 }
 
@@ -1223,15 +1251,15 @@
                 url: '/api/activity-list-execute',
                 data: JSON.stringify(l_data_dict),
                 success: function(in_data) {
                     try {
 
                         data_json = JSON.parse(in_data)
                         if ("ErrorHeader" in data_json) {
-                            if (data_json["ErrorTraceback"].indexOf("pywinauto.findwindows.ElementNotFoundError") != -1) {
+                            if (data_json["ErrorTraceback"].indexOf("There are no UI elements by selector (UIO / XPATH / CSS)") != -1) {
                                 orpa_utils_modal_uio_no_elements();
                             } else {
 
                                 orpa_workspace_modal_show("GUI Error", data_json.ErrorHeader + " \nTraceback: " + data_json.ErrorTraceback);
                                 throw new Error('Со стороны сервера поступила ошибка - прервать обработку JS');
                             }
 
@@ -1463,14 +1491,26 @@
             if (l_group.length > 0) {
                 return l_group[0].getAttribute("orpa-data-value")
             } else {
                 return in_default
             }
         }
 
+        orpa_range_value_set = function(in_orpa_data_key, in_orpa_data_value, in_default = null) {
+            //ПРОВЕРИТЬ НАЛИЧИЕ ОСТАЛЬНЫХ ЭЛЕМЕНТОВ ГРУППЫ
+            l_group = $("[orpa-data-key='" + in_orpa_data_key + "'][orpa-data-value='" + in_orpa_data_value + "']")
+            if (l_group.length > 0) {
+                orpa_range_select(l_group[0])
+                return l_group[0]
+            } else {
+                return in_default
+            }
+        }
+
+
         orpa_range_get = function(in_orpa_data_key, in_orpa_data_value) {
             //ПРОВЕРИТЬ НАЛИЧИЕ ОСТАЛЬНЫХ ЭЛЕМЕНТОВ ГРУППЫ
             l_group = $("[orpa-data-key='" + in_orpa_data_key + "'][orpa-data-value='" + in_orpa_data_value + "']")
             if (l_group.length > 0) {
                 return l_group[0]
             } else {
                 return null
@@ -1521,607 +1561,14 @@
                 type: "POST",
                 url: '/api/orpa-lab-open-path',
                 data: "",
                 dataType: "text"
             });
         }
 
-
-
-
-        // ORPA_DESKTOP_TREE
-
-
-
-
-        ////////////////////////////////////////////////////
-        ///////// ORPA DESKTOP SELECTOR НАЧАЛО /////////////////
-        ////////////////////////////////////////////////////  
-
-        orpa_desktop_selector_uio_clear = function(in_selector_uio) {
-            ///Создать урезанную версию селектора
-            lTextAreaSpecificationArray = mGlobal.iSysClone(in_selector_uio, true);
-            for (var i = 0; i < lTextAreaSpecificationArray.length; i++) {
-                ///Очистить ненужные ключи для выборки
-                delete lTextAreaSpecificationArray[i]['rich_text']
-                delete lTextAreaSpecificationArray[i]['process_id']
-                delete lTextAreaSpecificationArray[i]['rectangle']
-                delete lTextAreaSpecificationArray[i]['control_id']
-                delete lTextAreaSpecificationArray[i]['process']
-                delete lTextAreaSpecificationArray[i]['name']
-                delete lTextAreaSpecificationArray[i]['handle']
-                delete lTextAreaSpecificationArray[i]['control_type']
-                delete lTextAreaSpecificationArray[i]['runtime_id']
-                delete lTextAreaSpecificationArray[i]['selector']
-                delete lTextAreaSpecificationArray[i]['child_list']
-                if (i != 0) {
-                    delete lTextAreaSpecificationArray[i]['title']
-                    delete lTextAreaSpecificationArray[i]['class_name']
-                }
-            }
-            return lTextAreaSpecificationArray
-        }
-
-
-
-        orpa_desktop_selector_range_select = function(in_range) {
-            var l_callback = function(in_mode_str) {
-                l_range = orpa_range_get("orpa-desktop-selector-type", in_mode_str)
-                orpa_range_select(l_range)
-            }
-            orpa_desktop_selector.mode_set(in_range.getAttribute("orpa-data-value"), l_callback)
-        }
-
-
-
-
-        ////////////////////////////////////////////////////
-        ///////// ORPA DESKTOP TREE НАЧАЛО /////////////////
-        ////////////////////////////////////////////////////
-        orpa_desktop_tree = new orpa_utils_tree("orpa-desktop-tree");
-
-        orpa_desktop_tree_to_selector = function(in_item = null) {
-            if (in_item == null) {
-                // Достать выбранный объект
-                in_item = $("#orpa-desktop-tree .orpa-utils-list-item-selected")[0].js_dict["selector"]
-            } else {
-                in_item = in_item["selector"]
-            }
-            orpa_desktop_selector.uio_set(in_item)
-        }
-
-        orpa_desktop_tree_selected_item = null
-        orpa_desktop_tree_callback_api = function(in_data) {
-            orpa_utils_modal_uio_search_mouse_hide();
-            var recursive = function(in_data, parent_item = null) {
-                var l_data_list = []
-                in_data.forEach((item, index) => {
-                    //ФОРМИРУЕМ СЕЛЕКТОР
-                    if ("selector" in item) {
-                        selector_dict = mGlobal.iSysClone(item.selector, true);
-                    } else {
-                        selector_dict = orpa_desktop_selector_uio_clear([item])
-                        // ЕСЛИ ЕСТЬ РОДИТЕЛЬ
-                        if (parent_item != null) {
-                            selector_dict = mGlobal.iSysClone(parent_item.selector, true);
-                            if ("ctrl_index" in item) {
-                                selector_dict.push({
-                                    "ctrl_index": item.ctrl_index
-                                })
-                            } else {
-                                selector_dict.push({
-                                    "ctrl_index": index
-                                })
-                            }
-                        }
-                        item.selector = selector_dict
-                    }
-                    //selector_dict.ctrl_index = index // СФОРМИРОВАТЬ СЕЛЕКТОР ДЛЯ ДАЛЬНЕЙШЕЙ ОТРАБОТКИ
-
-                    //ОТПРАВЛЯЕМ В ДЕРЕВО
-                    l_title = item.title
-                    if (item.title == "") {
-                        l_title = "Нет заголовка"
-                    }
-                    var l_data_item = {
-                        "title_str": l_title,
-                        "description_str": `process_id: ${item.process_id}; handle: ${item.handle}; class_name: ${item.class_name}; RECT: L${item.rectangle.left} T${item.rectangle.top} R${item.rectangle.right} B${item.rectangle.bottom}`,
-                        "action_list": [{
-                            "_title_str": "ПОДСВЕТИТЬ",
-                            "icon_str": "lightbulb",
-                            "popup_str": "Выделить цветом UI объект",
-                            "callback_click": function(in_object, in_item, in_action) {
-                                orpa_api_activity_list_execute_async(function() {}, "pyOpenRPA.Robot.UIDesktop.UIOSelector_FocusHighlight", [in_item.selector]);
-                            }
-                        }, {
-                            "_title_str": "ПОИСК МЫШИ",
-                            "icon_str": "mouse pointer",
-                            "popup_str": "Выполнить поиск вложенного UI объекта с помощью мыши",
-                            "callback_click": function(in_object, in_item, in_action) {
-                                orpa_desktop_tree_selected_item = in_item;
-                                orpa_utils_modal_uio_search_mouse_show();
-                                orpa_api_activity_list_execute_async_json(orpa_desktop_tree_callback_api, "pyOpenRPA.Robot.UIDesktop.UIOSelector_SearchChildByMouse_UIOTree", [in_item.selector, 3.0], null)
-                            }
-                        }, {
-                            "_title_str": "СЕЛЕКТОР",
-                            "icon_str": "i cursor",
-                            "popup_str": "Сформировать селектор для обращения к UI объекту",
-                            "callback_click": function(in_object, in_item, in_action) {
-                                orpa_desktop_tree_to_selector(in_item);
-                            }
-                        }, {
-                            "_title_str": "РАСКРЫТЬ",
-                            "icon_str": "level down alternate",
-                            "visible_filter_str": "NO_CHILD",
-                            "popup_str": "Отобразить вложенные UI объекты",
-                            "callback_click": function(in_object, in_item, in_action) {
-                                orpa_desktop_tree_selected_item = in_item;
-                                orpa_api_activity_list_execute_async_json(orpa_desktop_tree_callback_api, "pyOpenRPA.Robot.UIDesktop.UIOSelector_GetChildList_UIOList", [in_item.selector], null)
-                            }
-                        }, {
-                            "_title_str": "СВЕРНУТЬ",
-                            "icon_str": "level up alternate",
-                            "visible_filter_str": "HAS_CHILD",
-                            "popup_str": "Свернуть вложенные UI объекты",
-                            "callback_click": function(in_object, in_item, in_action) {
-                                in_item.child_list = [];
-                                orpa_desktop_tree.render();
-                            }
-                        }, ],
-                        "callback_selected": function(in_object, in_item) {
-                            orpa_desktop_level_load_levels(in_object, in_item);
-                        },
-                        "is_unselect_block_bool": true,
-                        "selector": selector_dict
-                    }
-
-                    //ОБРАБОТКА ДЕТЕЙ
-                    if ("child_list" in item) {
-                        l_data_item["child_list"] = recursive(item.child_list, item)
-                    }
-                    l_data_list.push(l_data_item)
-                });
-                return l_data_list
-            }
-            l_data_list = recursive(in_data, orpa_desktop_tree_selected_item)
-            if (orpa_desktop_tree_selected_item != null) {
-                orpa_desktop_tree_selected_item['child_list'] = l_data_list
-                orpa_desktop_tree_selected_item = null
-            } else {
-                orpa_desktop_tree.load(l_data_list)
-            }
-            orpa_desktop_tree.render()
-            orpa_desktop_tree.loader_turn_off();
-        }
-        orpa_desktop_tree_refresh = function() {
-            backend_str = orpa_range_value_get("orpa-desktop-framework")
-            orpa_desktop_tree.loader_turn_on();
-            orpa_api_activity_list_execute_async_json(orpa_desktop_tree_callback_api, "pyOpenRPA.Robot.UIDesktop.UIOSelector_GetChildList_UIOList", null, {
-                inBackend: backend_str
-            })
-
-        }
-        orpa_desktop_tree_refresh()
-        orpa_desktop_tree_search = function() {
-            var search_value_str = document.getElementById("orpa-desktop-tree-search-value").value
-            var search_type_str = orpa_range_value_get("orpa-desktop-tree-search")
-            var backend_str = orpa_range_value_get("orpa-desktop-framework")
-            orpa_desktop_tree.loader_turn_on();
-            orpa_api_activity_list_execute_async_json(orpa_desktop_tree_callback_api, "pyOpenRPA.Robot.UIDesktop.UIO_Search_UIOTree", [search_value_str, search_type_str, null, null, backend_str], null)
-        }
-        ////////////////////////////////////////////////////
-        ///////// ORPA DESKTOP TREE КОНЕЦ /////////////////
-        ////////////////////////////////////////////////////
-
-        ////////////////////////////////////////////////////
-        ///////// ORPA DESKTOP LEVEL НАЧАЛО /////////////////
-        ////////////////////////////////////////////////////
-        orpa_desktop_level = new orpa_utils_tree("orpa-desktop-level");
-        orpa_desktop_level.mode_set("LIST")
-        orpa_desktop_level_load_levels = function(in_object, in_item) {
-            var callback = function(in_data) {
-                var l_data_list = []
-                in_data.forEach((item, index) => {
-                    //selector_dict.ctrl_index = index // СФОРМИРОВАТЬ СЕЛЕКТОР ДЛЯ ДАЛЬНЕЙШЕЙ ОТРАБОТКИ
-                    //ОТПРАВЛЯЕМ В ДЕРЕВО
-                    l_data_list.push({
-                        "icon_str": "dot circle",
-                        "title_str": "Уровень " + index + ": " + item.title,
-                        "description_str": `process_id: ${item.process_id}; handle: ${item.handle}; class_name: ${item.class_name}; RECT: L${item.rectangle.left} T${item.rectangle.top} R${item.rectangle.right} B${item.rectangle.bottom}`,
-                        "action_list": [],
-                        "callback_selected": function(in_object, in_item) {
-                            orpa_desktop_property_load(in_item);
-                        },
-                        "server_item": item,
-                        "level_int": index,
-                        "is_unselect_block_bool": true
-                    })
-                });
-                l_data_list.slice(-1)[0].is_selected_bool = true
-                orpa_desktop_level.load(l_data_list)
-                orpa_desktop_level.render()
-                orpa_desktop_level.loader_turn_off();
-                orpa_desktop_property_load(l_data_list.slice(-1)[0])
-            }
-
-            orpa_desktop_levels(in_item.selector, callback);
-        }
-
-        ////////////////////////////////////////////////////
-        ///////// ORPA DESKTOP LEVEL КОНЕЦ /////////////////
-        ////////////////////////////////////////////////////
-
-        ////////////////////////////////////////////////////
-        ///////// ORPA DESKTOP PROPERTY НАЧАЛО /////////////////
-        ////////////////////////////////////////////////////
-        var orpa_desktop_property_limit_len = 120
-        orpa_desktop_property = new orpa_utils_tree("orpa-desktop-property");
-        orpa_desktop_property.mode_set("LIST")
-
-        orpa_desktop_property_load = function(in_item) {
-            var l_data_list = []
-            var const_ignore = {
-                "rectangle": true
-            }
-            for (let key in in_item.server_item) {
-                if (key in const_ignore) {
-                    // В списке игнорирования
-                } else {
-                    let str = in_item.server_item[key];
-                    let str_render = str
-                    if (typeof str === "string") {
-                        if (str.length > orpa_desktop_property_limit_len) {
-                            str_render = str.slice(0, orpa_desktop_property_limit_len) + "...";
-                        }
-                    }
-                    if (str === "" || str == null) {
-                        str_render = "Отсутствует"
-                    }
-                    l_icon_str = "circle outline"
-                    if (orpa_desktop_selector.attribute_exists(in_item.level_int, key)) {
-                        l_icon_str = "circle"
-                    }
-                    l_data_list.push({
-                        "icon_str": l_icon_str,
-                        "title_str": key + ": ",
-                        "title_right_str": String(str_render),
-                        "description_str": "",
-                        "action_list": [],
-                        "callback_selected": function(in_object, in_item) {
-                            in_item.icon_str = "circle";
-                            orpa_desktop_selector.attribute_set(in_item.level_int, key, str);
-                            orpa_desktop_property.render();
-                        },
-                        "callback_unselected": function(in_object, in_item) {
-                            in_item.icon_str = "circle outline";
-                            orpa_desktop_selector.attribute_remove(in_item.level_int, key);
-                            orpa_desktop_property.render();
-                        },
-
-                        "level_int": in_item.level_int
-
-                    })
-                }
-
-            }
-            // ДОБАВИТЬ ИНФО ПРО МНОГОУРОВНЕВЫЙ ПОИСК DEPTH
-            l_icon_str = "circle outline"
-            if (orpa_desktop_selector.attribute_exists(in_item.level_int, "depth_end")) {
-                l_icon_str = "circle"
-            }
-            l_data_list.push({
-                "icon_str": l_icon_str,
-                "title_str": "depth: ",
-                "title_right_str": String("Многоуровневый поиск"),
-                "description_str": "",
-                "action_list": [],
-                "callback_selected": function(in_object, in_item) {
-                    in_item.icon_str = "circle";
-                    orpa_desktop_selector.attribute_set(in_item.level_int, "depth_start", 1);
-                    orpa_desktop_selector.attribute_set(in_item.level_int, "depth_end", 99);
-                    orpa_desktop_property.render();
-                },
-                "callback_unselected": function(in_object, in_item) {
-                    in_item.icon_str = "circle outline";
-                    orpa_desktop_selector.attribute_remove(in_item.level_int, "depth_start");
-                    orpa_desktop_selector.attribute_remove(in_item.level_int, "depth_end");
-                    orpa_desktop_property.render();
-                },
-
-                "level_int": in_item.level_int
-
-            })
-            orpa_desktop_property.load(l_data_list)
-            orpa_desktop_property.render()
-            orpa_desktop_property.loader_turn_off();
-        }
-
-        // ORPA DESKTOP ACTION
-
-
-
-        ///Выполнить действие
-        orpa_desktop_action_load_by_selector = function(in_selector_uio) {
-
-            var action_type_str = orpa_range_value_get("orpa-desktop-action-type")
-            if (action_type_str == "OBJECT") {
-                //Установить свойство disabled на textarea
-                document.getElementById("orpa-desktop-action-arg-textarea").removeAttribute("disabled")
-                document.getElementById("orpa-desktop-action-args-title").style.removeProperty('display');
-                document.getElementById("orpa-desktop-action-help-title").style.setProperty("display", "none")
-                document.getElementById("orpa-desktop-action-arg-textarea").style.setProperty("height", "93px")
-                document.getElementById("orpa-desktop-action-button-focus-run").style.removeProperty("display")
-                document.getElementById("orpa-desktop-action-button-run").style.removeProperty("display")
-                // КЕЙС, если идет прогрузка методов / свойств UI объекта
-                var callback = function(in_data) {
-                    var lDataKeyList = in_data
-                    var lValueList = []
-                    for (var i = 0; i < lDataKeyList.length; i++) {
-                        if (lDataKeyList[i].length > 0)
-                            if (lDataKeyList[i][0] != "_")
-                                lValueList.push({
-                                    'name': lDataKeyList[i],
-                                    'value': lDataKeyList[i]
-                                })
-                    }
-                    ///Установка значений в dropdown
-                    $('.ui.dropdown.gui-action')
-                        .dropdown({
-                            values: lValueList,
-                            onChange: orpa_desktop_action_helper_load
-                        });
-                }
-                orpa_api_activity_list_execute_async_json(callback, "pyOpenRPA.Robot.UIDesktop.UIOSelector_Get_UIOActivityList", [in_selector_uio])
-
-            } else {
-                // КЕЙС, если ВЫБРАН МОДУЛЬ UI Desktop
-
-                //Установить свойство disabled на textarea
-                document.getElementById("orpa-desktop-action-arg-textarea").setAttribute("disabled", "")
-                document.getElementById("orpa-desktop-action-help-title").style.removeProperty('display');
-                document.getElementById("orpa-desktop-action-args-title").style.setProperty("display", "none")
-                document.getElementById("orpa-desktop-action-arg-textarea").style.setProperty("height", "101px")
-                document.getElementById("orpa-desktop-action-button-focus-run").style.setProperty("display", "none")
-                document.getElementById("orpa-desktop-action-button-run").style.setProperty("display", "none")
-                var lValueList = []
-                for (let key in orpa_desktop_action_dict) {
-                    var item = orpa_desktop_action_dict[key]
-                    lValueList.push({
-                        'name': key,
-                        'value': key
-                    })
-                }
-                ///Установка значений в dropdown
-                $('.ui.dropdown.gui-action')
-                    .dropdown({
-                        values: lValueList,
-                        onChange: orpa_desktop_action_module_code_generator
-                    });
-            }
-        }
-
-        orpa_desktop_action_args_render = function() {
-            var arg_type_str = orpa_range_value_get("orpa-desktop-action-arg-type")
-            var arg_textarea = document.getElementById("orpa-desktop-action-arg-textarea")
-            if (arg_type_str == "LIST") {
-                arg_textarea.setAttribute("placeholder", "[\"Привет\", \"Мир\"]")
-                if (orpa_desktop_action_helper_list_str != null) {
-                    orpa_desktop_action_helper_render_function()
-                    arg_textarea.value = orpa_desktop_action_helper_list_str
-                } else {
-                    orpa_desktop_action_helper_render_property()
-                    arg_textarea.value = "Выбранное наименование является свойством. Нажмите 'Выполнить', чтобы просмотреть его содержимое"
-                }
-            } else {
-                arg_textarea.setAttribute("placeholder", "{\"key1\":\"Привет\", \"key2\":\"Мир\"}")
-                if (orpa_desktop_action_helper_dict_str != null) {
-                    orpa_desktop_action_helper_render_function()
-                    arg_textarea.value = orpa_desktop_action_helper_dict_str
-                } else {
-                    orpa_desktop_action_helper_render_property()
-                    arg_textarea.value = "Выбранное наименование является свойством. Нажмите 'Выполнить', чтобы просмотреть его содержимое"
-                }
-            }
-        }
-        orpa_desktop_action_helper_save = function() {
-            var arg_type_str = orpa_range_value_get("orpa-desktop-action-arg-type")
-            var arg_textarea = document.getElementById("orpa-desktop-action-arg-textarea")
-            if (arg_type_str == "LIST") {
-                orpa_desktop_action_helper_list_str = arg_textarea.value
-            } else {
-                orpa_desktop_action_helper_dict_str = arg_textarea.value
-            }
-        }
-        orpa_desktop_action_helper_render_function = function() {
-            orpa_desktop_action_helper_is_function = true
-            //Установить свойство disabled на textarea
-            document.getElementById("orpa-desktop-action-arg-textarea").removeAttribute("disabled")
-            document.getElementById("orpa-desktop-action-args-title").style.removeProperty('display');
-            document.getElementById("orpa-desktop-action-help-title").style.setProperty("display", "none")
-            document.getElementById("orpa-desktop-action-arg-textarea").style.setProperty("height", "93px")
-            document.getElementById("orpa-desktop-action-button-focus-run").style.removeProperty("display")
-        }
-
-        orpa_desktop_action_helper_render_property = function() {
-            orpa_desktop_action_helper_is_function = false
-            //Установить свойство disabled на textarea
-            document.getElementById("orpa-desktop-action-arg-textarea").setAttribute("disabled", "")
-            document.getElementById("orpa-desktop-action-help-title").style.removeProperty('display');
-            document.getElementById("orpa-desktop-action-args-title").style.setProperty("display", "none")
-            document.getElementById("orpa-desktop-action-arg-textarea").style.setProperty("height", "101px")
-            document.getElementById("orpa-desktop-action-button-focus-run").style.setProperty("display", "none")
-        }
-
-        orpa_desktop_action_helper_dict_str = null
-        orpa_desktop_action_helper_list_str = null
-        orpa_desktop_action_helper_is_function = null
-        orpa_desktop_action_helper_load = function(in_value) {
-            var callback = function(in_data) {
-                var arg_type_str = orpa_range_value_get("orpa-desktop-action-arg-type")
-                var arg_textarea = document.getElementById("orpa-desktop-action-arg-textarea")
-                if (arg_type_str == "LIST") {
-                    orpa_desktop_action_helper_dict_str = null
-                    if (in_data["ArgList"] == null) {
-                        orpa_desktop_action_helper_list_str = null
-                    } else {
-                        orpa_desktop_action_helper_list_str = JSON.stringify(in_data["ArgList"])
-                    }
-                } else {
-                    orpa_desktop_action_helper_list_str = null
-                    if (in_data["ArgDict"] == null) {
-                        orpa_desktop_action_helper_dict_str = null
-                    } else {
-                        orpa_desktop_action_helper_dict_str = JSON.stringify(in_data["ArgDict"])
-                    }
-                }
-                orpa_desktop_action_args_render()
-            }
-            orpa_api_activity_list_execute_async_json(callback, "pyOpenRPA.Robot.UIDesktop.UIOSelectorUIOActivity_Get_ArgDict", [orpa_desktop_selector.uio_get(), in_value])
-
-        }
-
-        orpa_desktop_action_module_code_generator = function(in_value) {
-            if (in_value != "") {
-                var code_str = orpa_desktop_action_dict[in_value].code_str
-                var help_str = orpa_desktop_action_dict[in_value].help_str
-                document.getElementById("orpa-desktop-action-arg-textarea").value = help_str
-                code_str = code_str.replace("<SELECTOR>", JSON.stringify(orpa_desktop_selector.uio_get()));
-                clipboard_set(code_str)
-            }
-
-        }
-
-        orpa_desktop_action_run = function(in_ui_focus_bool = true) {
-            var callback = function(in_data) {
-                var result_textarea = document.getElementById("orpa-desktop-action-result")
-                var data = in_data[in_data.length - 1]
-                if (data == null) {
-                    result_textarea.innerHTML = "Значение null / None"
-                } else {
-                    result_textarea.innerHTML = JSON.stringify(data)
-                }
-                result_textarea.classList.remove("orpa-placeholder");
-            }
-            var arg_type_str = orpa_range_value_get("orpa-desktop-action-arg-type")
-            var arg_textarea = document.getElementById("orpa-desktop-action-arg-textarea")
-            var uio = orpa_desktop_selector.uio_get()
-            var action_str = $("#orpa-desktop-action-def-input").dropdown("get value")
-            var activity_list = []
-            var textarea_value = arg_textarea.value
-            if (orpa_desktop_action_helper_is_function == true) {
-                if (textarea_value != "" && textarea_value != null) {
-                    textarea_value = JSON.parse(textarea_value)
-                } else {
-                    if (arg_type_str == "LIST") {
-                        textarea_value = []
-                    } else {
-                        textarea_value = {}
-                    }
-                }
-            } else {
-                textarea_value = ""
-            }
-            if (in_ui_focus_bool == true) {
-                activity_list.push({
-                    "Def": "pyOpenRPA.Robot.UIDesktop.UIOSelector_FocusHighlight",
-                    "ArgList": [uio],
-                    "ArgDict": {}
-                })
-            }
-            if (arg_type_str == "LIST") {
-                activity_list.push({
-                    "Def": "pyOpenRPA.Robot.UIDesktop.UIOSelectorUIOActivity_Run_Dict",
-                    "ArgList": [uio, action_str, true, textarea_value],
-                    "ArgDict": {}
-                })
-            } else {
-                activity_list.push({
-                    "Def": "pyOpenRPA.Robot.UIDesktop.UIOSelectorUIOActivity_Run_Dict",
-                    "ArgList": [uio, action_str, true, null, textarea_value],
-                    "ArgDict": {}
-                })
-            }
-
-            orpa_api_activity_list_execute_async_json_many(callback, activity_list)
-        }
-
-
-
-
-        ////////////////////////////////////////////////////
-        ///////// ORPA DESKTOP PROPERTY КОНЕЦ /////////////////
-        ////////////////////////////////////////////////////
-        // ORPA DESKTOP MEMORY
-        orpa_desktop_memory_slot_dict = {}
-
-        orpa_desktop_memory_switch = function(in_new_item) {
-            key_old_str = orpa_range_value_get("orpa-desktop-memory-slot")
-            orpa_desktop_memory_save(key_old_str)
-            orpa_range_select(in_new_item);
-            key_new_str = orpa_range_value_get("orpa-desktop-memory-slot")
-            orpa_desktop_memory_restore(key_new_str)
-        }
-
-        orpa_desktop_memory_save = function(in_slot_key) {
-            orpa_desktop_memory_slot_dict[in_slot_key] = {}
-            slot_dict = orpa_desktop_memory_slot_dict[in_slot_key]
-            slot_dict["tree"] = orpa_desktop_tree.data_list
-            slot_dict["tree_mode"] = orpa_desktop_tree.mode
-            slot_dict["level"] = orpa_desktop_level.data_list
-            slot_dict["property"] = orpa_desktop_property.data_list
-            slot_dict["selector"] = orpa_desktop_selector.uio_get()
-            slot_dict["action"] = orpa_desktop_action.data_get()
-            slot_dict["action-result"] = document.getElementById("orpa-desktop-action-result").innerHTML
-
-        }
-        orpa_desktop_memory_restore = function(in_slot_key) {
-            if (in_slot_key in orpa_desktop_memory_slot_dict) {
-                slot_dict = orpa_desktop_memory_slot_dict[in_slot_key]
-                orpa_desktop_tree.load(slot_dict.tree)
-                orpa_desktop_tree.mode_set(slot_dict.tree_mode)
-                orpa_desktop_level.load(slot_dict.level)
-                orpa_desktop_property.load(slot_dict.property)
-                orpa_desktop_selector.uio_set(slot_dict["selector"])
-                orpa_desktop_action.data_load(slot_dict["action"])
-                document.getElementById("orpa-desktop-action-result").innerHTML = slot_dict["action-result"]
-                if (slot_dict["action-result"] != "") {
-                    document.getElementById("orpa-desktop-action-result").classList.remove("orpa-placeholder");
-                } else {
-                    document.getElementById("orpa-desktop-action-result").classList.add("orpa-placeholder");
-                }
-
-            } else {
-                orpa_desktop_tree_refresh()
-                orpa_desktop_tree.mode_set("TREE")
-                orpa_desktop_level.clear()
-                orpa_desktop_property.clear()
-                orpa_desktop_selector.clear()
-                orpa_desktop_action.clear()
-                document.getElementById("orpa-desktop-action-result").innerHTML = ""
-                document.getElementById("orpa-desktop-action-result").classList.add("orpa-placeholder");
-            }
-        }
-        orpa_desktop_memory_clear = function(in_slot_key) {
-
-        }
-
-
-        ////////////////////////////////////////////////////
-        ///////// ORPA BROWSER НАЧАЛО /////////////////
-        ////////////////////////////////////////////////////
-        orpa_browser_tree = new orpa_utils_tree("orpa-browser-tree");
-        orpa_browser_level = new orpa_utils_tree("orpa-browser-level");
-        //orpa_browser_level.mode_set("LIST")
-        orpa_browser_property = new orpa_utils_tree("orpa-browser-property");
-        //orpa_browser_property.mode_set("LIST")
-
-        ////////////////////////////////////////////////////
-        ///////// ORPA BROWSER КОНЕЦ /////////////////
-        ////////////////////////////////////////////////////
-
         ////////////////////////////////////////////////////
         ///////// ORPA API НАЧАЛО /////////////////
         ////////////////////////////////////////////////////
         // UIO, CSS, XPATH
         orpa_api_uidesktop_selector_convert = function(in_selector, in_type_str, in_callback, in_type_from_str = null) {
             switch (true) {
                 case in_type_from_str == "XPATH" && in_type_str == "UIO":
@@ -2191,37 +1638,14 @@
 
 
         ////////////////////////////////////////////////////
         ///////// ORPA API КОНЕЦ /////////////////
         ////////////////////////////////////////////////////
 
 
-        orpa_desktop_selector_search_list = function() {
-            var uio_selector = orpa_desktop_selector.uio_get()
-            var in_callback = function(in_data) {
-                for (var i = 0; i < in_data.length; i++) {
-                    var item_selector = mGlobal.iSysClone(uio_selector, true)
-                    item_selector[item_selector.length - 1]["ctrl_index"] = i;
-                    in_data[i].selector = item_selector
-                }
-
-                orpa_desktop_tree_callback_api(in_data)
-            }
-            orpa_desktop_tree.loader_turn_on()
-            orpa_api_activity_list_execute_async_json(in_callback, "pyOpenRPA.Robot.UIDesktop.UIOSelector_Get_UIOInfoList", [uio_selector], null)
-        }
-
-        orpa_desktop_action = new orpa_utils_action("orpa-desktop-action", "orpa-desktop-action-result", true);
-        orpa_desktop_selector = new orpa_utils_selector('orpa-desktop-selector-textarea', 'UIO', orpa_desktop_action.on_change_uio_selector, "DESKTOP")
-
-        orpa_desktop_action.render();
-
-        // Загрузить список
-        // Сформировать подходящую структуру
-        //orpa_desktop_tree.load()
 
         // ОБНОВИТЬ СОСТОЯНИЕ ВКЛАДОК
         orpa_tabs_render = function() {
             l_group = $(".orpa-tab.ui.tag.label")
             for (var i = 0; i < l_group.length; i++) {
                 l_workspace_id = l_group[i].getAttribute("orpa-data-value")
                 l_workspace = $("#" + l_workspace_id)[0]
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std.xhtml` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std.xhtml`

 * *Files 2% similar despite different names*

```diff
@@ -97,19 +97,28 @@
 
 				</div>
 			</div>
 		</div>
 
 		<!-- РАЗДЕЛ ПРОЕКТ -- ORPA-PROJECT -- НАЧАЛО -->
 		<div class="ui aligned stackable grid container" id="orpa-project">
+
+
+
+
 			<div class="row">
+				
 				<div class="sixteen wide column " >
 					<div class="ui horizontal divider header" style="margin-bottom:5px;margin-top:0px; ">
 						<div ><i style="margin-left: 0.75rem;" class="angle double down icon" onclick="jump('#orpa-project-iframe');"></i></div>				
 					</div>
+					<div class="sixteen wide column " >
+						<i style="display:inline-block; cursor: pointer; margin-bottom:15px;margin-top:0px; " data="" class="exclamation triangle icon orange" onclick="orpa_utils_popup_show(this, 'Функциональность зависит от текущей раскладки клавиатуры (РУС, АНГ)');"></i>
+						<span>ПРИ НЕКОРРЕКТНОМ ОТОБРАЖЕНИИ ОКНА РЕДАКТОРА НАЖАТЬ КНОПКУ "ОБНОВИТЬ"</span>
+					</div>
 					<button style="margin-bottom: 10px;"  class="ui button grey labeled icon mini" onclick="orpa_project_jupyter_open_path();">
 						<i class="folder icon"></i>
 						Открыть в проводнике
 					</button> 
 					<button style="margin-bottom: 10px;"  class="ui button grey labeled icon mini" onclick="orpa_project_jupyter_set_path();">
 						<i class="folder icon"></i>
 						Открыть / создать проект
@@ -137,16 +146,24 @@
 		<!-- РАЗДЕЛ ПРИЛОЖЕНИЕ -- ORPA-DESKTOP -- НАЧАЛО -->
 		<div class="ui aligned stackable grid container" id="orpa-desktop">
 
 			<div class="row">
 				<div class="sixteen wide column " >
 					<div class="ui horizontal divider header" style="margin-bottom:30px;margin-top:0px; ">
 						<div ><i style="margin-left: 0.75rem;" class="angle double down icon" onclick="jump('#orpa-desktop-col-1');"></i>
+							{% if is_linux_bool==False %}
 							<span orpa-data-key="orpa-desktop-framework" orpa-data-value="uia" class="ui tag label teal  tiny noselect" onclick="orpa_range_select(this); orpa_desktop_tree_refresh();">UIA</span>
 							<span orpa-data-key="orpa-desktop-framework" orpa-data-value="win32" class="ui tag label  tiny noselect" onclick="orpa_range_select(this); orpa_desktop_tree_refresh();">WIN32</span>
+
+					  
+							 {% else %}
+							 <span orpa-data-key="orpa-desktop-framework" orpa-data-value="at-spi" class="ui tag label teal  tiny noselect" onclick="orpa_range_select(this); orpa_desktop_tree_refresh();">AT-SPI</span>
+							<span orpa-data-key="orpa-desktop-framework" orpa-data-value="wnck" class="ui tag label  tiny noselect" onclick="orpa_range_select(this); orpa_desktop_tree_refresh();">WNCK</span>
+
+							{% endif %}
 							<span style="color:teal; cursor: pointer;" onclick="orpa_desktop_workspace_proportion_set('eight', 'four', 'four');"><i class="expand icon"></i>:<i class="compress icon"></i>:<i class="compress icon"></i></span>
 							|
 							<span style="color:teal; cursor: pointer;" onclick="orpa_desktop_workspace_proportion_set('four', 'eight', 'four');"><i class="compress icon"></i>:<i class="expand icon"></i>:<i class="compress icon"></i></span>
 							|
 							<span style="color:teal; cursor: pointer;" onclick="orpa_desktop_workspace_proportion_set('four', 'four', 'eight');"><i class="compress icon"></i>:<i class="compress icon"></i>:<i class="expand icon"></i></span>
 							|
 							<span style="color:teal; cursor: pointer;" onclick="orpa_desktop_workspace_proportion_set('six', 'six', 'four');"><i class="redo icon"></i></span>
@@ -161,32 +178,52 @@
 					<div class="ui tiny header orpa">UI ОБЪЕКТЫ
 						
 						<span style="margin-left:20px;" orpa-data-key="orpa-desktop-tree-type" orpa-data-value="TREE" class="ui tag label teal  tiny noselect" onclick="orpa_range_select(this); orpa_desktop_tree.mode_set('TREE');">ДЕРЕВО</span>
 						<span orpa-data-key="orpa-desktop-tree-type" orpa-data-value="LIST" class="ui tag label  tiny noselect" onclick="orpa_range_select(this); orpa_desktop_tree.mode_set('LIST');">СПИСОК</span>
 						<i style="display:inline-block" class="question circle icon teal" onclick="orpa_helper_info('orpa_desktop_ui_object');"></i>
 
 					</div>
+
+
+
+					{% if is_linux_bool==False %}
+
 					<div class="ui input mini {% if is_ee_bool==False %}disabled{% endif %}" style="width:44%; margin-bottom:8px;">
 						<input id="orpa-desktop-tree-search-value" type="text" placeholder="Поиск" onkeydown="if (event.keyCode == 13) document.getElementById('orpa-desktop-tree-search-icon').click();">
 					</div>
 
 
 					<i id="orpa-desktop-tree-search-icon" style="margin-left:5px;display:inline-block; cursor: pointer;" class="search icon teal {% if is_ee_bool==False %}disabled{% endif %}" onclick="{% if is_ee_bool==True %}orpa_desktop_tree_search();{% endif %}"></i>
 					
 					<span style="margin-left:20px;" orpa-data-key="orpa-desktop-tree-search" orpa-data-value="STR" class="ui tag label  tiny noselect {% if is_ee_bool==False %}disabled{% endif %}" onclick="orpa_range_select(this);">STR</span>
 					<span orpa-data-key="orpa-desktop-tree-search" orpa-data-value="WC" class="ui tag label teal  tiny noselect {% if is_ee_bool==False %}disabled{% endif %}" onclick="orpa_range_select(this);">WC</span>
 					<span orpa-data-key="orpa-desktop-tree-search" orpa-data-value="RE" class="ui tag label  tiny noselect {% if is_ee_bool==False %}disabled{% endif %}" onclick="orpa_range_select(this);">RE</span>
 
 					
+			  
+					 {% else %}
+					 <div class="ui input mini disabled" style="width:44%; margin-bottom:8px;">
+						<input id="orpa-desktop-tree-search-value" type="text" placeholder="Поиск" onkeydown="">
+					</div>
+
+
+					<i id="orpa-desktop-tree-search-icon" style="margin-left:5px;display:inline-block; cursor: pointer;" class="search icon teal disabled" onclick=""></i>
+					
+					<span style="margin-left:20px;" orpa-data-key="orpa-desktop-tree-search" orpa-data-value="STR" class="ui tag label  tiny noselect disabled" onclick="">STR</span>
+					<span orpa-data-key="orpa-desktop-tree-search" orpa-data-value="WC" class="ui tag label teal  tiny noselect disabled" onclick="">WC</span>
+					<span orpa-data-key="orpa-desktop-tree-search" orpa-data-value="RE" class="ui tag label  tiny noselect disabled" onclick="">RE</span>
+
+					{% endif %}
+
 					<!-- ORPA TREE -- НАЧАЛО -->
 					<div id="orpa-desktop-tree" class="ui segment" style="-webkit-box-shadow:0 0 0 0 rgba(34,36,38,.15);box-shadow:0 0 0 0 rgba(34,36,38,.15);margin:0px;padding:0px; border-radius: 0px; border:0px;;">
 						<div class="ui  inverted dimmer">
 						  <div class="ui text loader">Загружаем...</div>
 						</div>
-						<div class="orpa-utils-tree-workspace" style="margin-top: 10px; height:385px;overflow-x:hidden; overflow-y:auto; margin-top:0px;"></div>
+						<div class="orpa-utils-tree-workspace" style="margin-top: 10px; height:385px;overflow-x:auto; overflow-y:auto; margin-top:0px;"></div>
 
 					</div>
 					<!-- ORPA TREE -- КОНЕЦ -->
 
 						<div class="ui tiny header orpa">СЕЛЕКТОР
 						<i style="margin-left:10px;display:inline-block" class="i cursor icon"></i>
 						<span style="margin-left:20px;"  orpa-data-key="orpa-desktop-selector-type" orpa-data-value="UIO" class="ui tag label  teal tiny noselect" onclick="orpa_desktop_selector_range_select(this)">UIO</span>
@@ -523,40 +560,55 @@
 					
 					<div style="margin-bottom:0px;margin-top:15px;">
 						<span orpa-data-key="orpa-keyboard-sleep" class="ui tag label  tiny noselect keyboard-wait-time" onclick="orpa_range_select(this); ">0.2 СЕК.</span>
 						<span orpa-data-key="orpa-keyboard-sleep" class="ui tag label  teal tiny noselect keyboard-wait-time" onclick="orpa_range_select(this); ">1.0 СЕК.</span>
 						<span orpa-data-key="orpa-keyboard-sleep" class="ui tag label  tiny noselect keyboard-wait-time" onclick="orpa_range_select(this); ">3.0 СЕК.</span>
 						<span orpa-data-key="orpa-keyboard-sleep" class="ui tag label  tiny noselect keyboard-wait-time" onclick="orpa_range_select(this); ">5.0 СЕК.</span>
 					</div>
+
+
+					<div style="margin-bottom: 10px;" class="ui tiny header orpa">СИМВОЛ
+						<i style="margin-left:10px;display:inline-block" onclick="orpa_keyboard_symbol_function_copy(); orpa_utils_popup_show(this, 'Код Python скопирован в буфер обмена! Для вставки используйте комбинацию клавиш Ctrl+V');"  class="code icon teal"></i>
+						<i style="display:inline-block" data="" class="question circle icon teal" onclick="orpa_helper_info('orpa_keyboard_symbol_detect');"></i>
+
+					</div>
+					<div class="" style="margin-bottom:5px;margin-top:10px;">
+						<div class="ui input" style="width:90%; margin-bottom: 10px;">
+							<input oninput="orpa_keyboard_do_variants_update();" class="" type="text" id="orpa-keyboard-hotkey-symbol" placeholder="">
+						</div>
+						<div id="orpa-keyboard-hotkey-symbol-variants" style="width:86%; display:grid">
+							
+						</div>
+					</div>
+
 				</div>
 
 				<div class="five wide column" id="orpa-keyboard-col-2">
 					<div class="ui tiny header orpa">ТЕКСТ
 
-						<i style="margin-left:10px;display:inline-block" onclick="orpa_keyboard_do_write_function_copy()" class="code icon teal"></i>
+						<i style="margin-left:10px;display:inline-block" onclick="orpa_keyboard_do_write_function_copy(); orpa_utils_popup_show(this, 'Код Python скопирован в буфер обмена! Для вставки используйте комбинацию клавиш Ctrl+V');" class="code icon teal"></i>
 						<i style="display:inline-block" data="" class="question circle icon teal" onclick="orpa_helper_info('orpa_keyboard_text');"></i>
 
 					</div>
-					<textarea style="width:100%; height: 115px;font-size:12pt; resize: none;" class="orpa-keyboard-write-data" cols="60"></textarea>
+					<textarea style="width:100%; height: 170px;font-size:12pt; resize: none;" class="orpa-keyboard-write-data" cols="60"></textarea>
 					<button style="margin-top: 10px;"  class="ui button grey labeled icon mini" onclick="orpa_keyboard_do_write_function()">
 						<i class="play icon"></i>
 						Выполнить
 					</button>
 
-					<div class="ui tiny header orpa">СИМВОЛ 
+					<div class="ui tiny header orpa">СИМВОЛ + ДЕЙСТВИЕ 
 						
 
-						<i style="margin-left:10px;display:inline-block" onclick="orpa_keyboard_do_function_copy()" class="code icon teal"></i>
-						<i style="display:inline-block" data="" class="question circle icon teal" onclick="orpa_helper_info('orpa_keyboard_symbol');"></i>
+						<i style="margin-left:10px;display:inline-block" onclick="orpa_keyboard_do_function_copy(); orpa_utils_popup_show(this, 'Код Python скопирован в буфер обмена! Для вставки используйте комбинацию клавиш Ctrl+V');" class="code icon teal"></i>
+						<i style="display:inline-block; cursor: pointer;" data="" class="question circle icon teal" onclick="orpa_helper_info('orpa_keyboard_symbol');"></i>
+						<i style="display:inline-block; cursor: pointer;" data="" class="exclamation triangle icon orange" onclick="orpa_utils_popup_show(this, 'Функциональность зависит от текущей раскладки клавиатуры (РУС, АНГ)');"></i>
+						
 					</div>
 					<div>
-						<div class="ui input" style="width:25%">
-							<input type="text" id="orpa-keyboard-function-symbol-select", placeholder="Символ">
-						</div>
-						<div class="ui selection dropdown" style="width:40%;" id="orpa-keyboard-function-select">
+						<div class="ui selection dropdown" style="width:86%;" id="orpa-keyboard-function-select">
 							<input type="hidden" name="orpa-keyboard-action">
 							<i class="dropdown icon"></i>
 							<div class="default text">Функция</div>
 							<div class="scrollhint menu">
 							<div class="item" data-value="Down">Down</div>
 							<div class="item" data-value="Up">Up</div>
 							<div class="item" data-value="Wait">Wait</div>
@@ -564,40 +616,39 @@
 							</div>
 						</div>
 						<button class="ui grey icon button" onclick="orpa_keyboard_do_function()" style="width:12%">
 							<i class="play icon"></i>
 						</button>
 					</div>
 
-					<div style="margin-bottom: 10px;" class="ui tiny header orpa">ГОРЯЧИЕ КЛАВИШИ 
-						<i style="margin-left:10px;display:inline-block" onclick="orpa_keyboard_do_function_hotkey_copy()" class="code icon teal"></i>
-						<i style="display:inline-block" data="" class="question circle icon teal" onclick="orpa_helper_info('orpa_keyboard_hotkey');"></i>
-
+					<div style="margin-bottom: 10px;" class="ui tiny header orpa">СИМВОЛ + ГОРЯЧИЕ КЛАВИШИ 
+						<i style="margin-left:10px;display:inline-block" onclick="orpa_keyboard_do_function_hotkey_copy();  orpa_utils_popup_show(this, 'Код Python скопирован в буфер обмена! Для вставки используйте комбинацию клавиш Ctrl+V');" class="code icon teal"></i>
+						<i style="display:inline-block; cursor: pointer;" data="" class="question circle icon teal" onclick="orpa_helper_info('orpa_keyboard_hotkey');"></i>
+						<i style="display:inline-block; cursor: pointer;" data="" class="exclamation triangle icon orange" onclick="orpa_utils_popup_show(this, 'Функциональность зависит от текущей раскладки клавиатуры (РУС, АНГ)');"></i>
 					</div>
 					<div class="" style="margin-bottom:5px;margin-top:10px;">
 						<span style="width:15%" orpa-data-key="orpa-keyboard-hotkey-first" class="ui tag label  tiny noselect keyboard-hotkey" onclick="orpa_range_toogle(this); ">CTRL</span>
 						<span style="width:13%" orpa-data-key="orpa-keyboard-hotkey-second" class="ui tag label teal tiny noselect keyboard-hotkey" onclick="orpa_range_toogle(this); ">ALT</span>
-						<span style="width:17%" orpa-data-key="orpa-keyboard-hotkey-third" class="ui tag label  tiny noselect keyboard-hotkey" onclick="orpa_range_toogle(this); ">SHIFT </span>
+						<span style="width:17%" orpa-data-key="orpa-keyboard-hotkey-third" class="ui tag label  tiny noselect keyboard-hotkey" onclick="orpa_range_toogle(this); ">SHIFT</span>
 						<span style="width:16%" orpa-data-key="orpa-keyboard-hotkey-fourth" class="ui tag label  tiny noselect keyboard-hotkey" onclick="orpa_range_toogle(this); ">WIN</span>
-						<b>+</b>
-						<div class="ui input" style="width:16%">
-							<input class="" type="text" id="orpa-keyboard-hotkey-common-symbol-select" placeholder="А">
+						<div id="orpa-keyboard-hotkey-symbol-variants" style="width:86%; display:grid">
+							
 						</div>
 					</div>
-					<button style="margin-top: 10px;"  class="ui button grey labeled icon mini" onclick="orpa_keyboard_do_function_hotkey()">
+					<button style="margin-top: 10px;"  class="ui button grey labeled icon mini" onclick="orpa_keyboard_do_function_hotkey();">
 						<i class="play icon"></i>
 						Выполнить
 					</button>
 
 					
 				</div>
 
 				<div class="five wide column" id="orpa-keyboard-col-3" >
 					<div class="ui tiny header orpa">БУФЕР ОБМЕНА</div>
-					<textarea style="width:100%; height: 355px;font-size:12pt; resize: none;" id="orpa-keyboard-clipboard-textarea" cols="60"></textarea>	
+					<textarea style="width:100%; height: 395px;font-size:12pt; resize: none;" id="orpa-keyboard-clipboard-textarea" cols="60"></textarea>	
 					<button style="margin-top: 10px;" class="ui button grey labeled icon mini" onclick="orpa_keyboard_clipboard_get()">
 						<i class="caret up icon"></i>
 						Прочитать
 					</button>
 					<i onclick="orpa_keyboard_clipboard_get_copy()" class="code icon teal"></i>
 					<button style="margin-top: 10px;"  class="ui button grey labeled icon mini" onclick="orpa_keyboard_clipboard_set()">
 						<i class="caret down icon"></i>
@@ -622,14 +673,21 @@
 		<div class="ui aligned stackable grid container" id="orpa-mouse">
 
 			<div class="row">
 				<div class="sixteen wide column "  >
 					<div class="ui horizontal divider header orpa" style="margin-bottom:30px;margin-top:0px; ">
 						<div >
 							<i style="margin-left: 0.75rem;" class="angle double down icon" onclick="jump('#orpa-mouse-col-1');"></i>
+							{% if is_linux_bool==True %}
+							<i style="display:inline-block; cursor: pointer;" data="" class="exclamation triangle icon orange" onclick="orpa_utils_popup_show(this, 'ВНИМАНИЕ! В LINUX УКАЗАТЕЛЬ ВАШЕГО УСТРОЙСТВА МЫШИ НЕ ПЕРЕМЕЩАЕТСЯ ПРИ ВЫПОЛНЕНИИ КОМАНДЫ (НО КОМАНДА ВЫПОЛНЯЕТСЯ).');"></i>
+			
+							 {% else %}
+							{% endif %}
+							<span orpa-data-key="orpa-mouse-source" orpa-data-value="file" class="ui tag label teal tiny noselect" onclick="orpa_range_select(this); orpa_desktop_tree_refresh();">ИЗ ФАЙЛА</span>
+							<span orpa-data-key="orpa-mouse-source" orpa-data-value="string" class="ui tag label  tiny noselect" onclick="orpa_range_select(this); orpa_desktop_tree_refresh();">ИЗ СТРОКИ</span>
 							<span style="color:teal; cursor: pointer;" onclick="orpa_mouse_workspace_proportion_set('six', 'five', 'five');"><i class="expand icon"></i>:<i class="compress icon"></i>:<i class="compress icon"></i></span>
 							|
 							<span style="color:teal; cursor: pointer;" onclick="orpa_mouse_workspace_proportion_set('five', 'six', 'five');"><i class="compress icon"></i>:<i class="expand icon"></i>:<i class="compress icon"></i></span>
 							|
 							<span style="color:teal; cursor: pointer;" onclick="orpa_mouse_workspace_proportion_set('five', 'five', 'six');"><i class="compress icon"></i>:<i class="compress icon"></i>:<i class="expand icon"></i></span>
 							<i style="margin-left: 0.35rem;" class="angle double down icon" onclick="jump('#orpa-mouse-col-1');"></i>
 						</div>				
@@ -658,15 +716,17 @@
 
 					</div>
 					<div class="orpa-placeholder-img-preview" style="height:258px; background-color: #e8e8e8;" ></div>
 				</div>
 
 				<div class="five wide column" id="orpa-mouse-col-2" >
 					<div class="ui tiny header orpa">ОБНАРУЖЕНО
-						<i style="margin-left:10px;display:inline-block" data="Точность: 1.0 - идентичное соответствие, 0.0 - полное несоответствие.&#10;СУТ - точка относительно которой выполнен поиск изображения" class="question circle icon teal" onclick="orpa_helper_info('orpa_mouse_location');"></i>
+						<i style="margin-left:10px;display:inline-block"class="code icon teal" onclick="orpa_mouse_detect_copy();orpa_utils_popup_show(this, 'Код Python скопирован в буфер обмена! Для вставки используйте комбинацию клавиш Ctrl+V');"></i>
+
+						<i style="margin-left:0px;display:inline-block" data="Точность: 1.0 - идентичное соответствие, 0.0 - полное несоответствие.&#10;СУТ - точка относительно которой выполнен поиск изображения" class="question circle icon teal" onclick="orpa_helper_info('orpa_mouse_location');"></i>
 
 					</div>
 					<div class="ui tiny header orpa" style="margin-top: 20px;">
 						Точность
 						<div class="ui input" style="width:30%;height: 24px;">
 							<input type="text" id="orpa-screen-accuracy-img-locate", value="0.9">
 						</div>
@@ -729,16 +789,18 @@
 					<button style="margin-top: 10px;"  class="ui button grey labeled icon mini" onclick="orpa_mouse_do_function()">
 						<i class="play icon"></i>
 						Выполнить
 					</button>
 					<i class="code icon teal" onclick="orpa_mouse_do_function_copy()"></i>
 
 					<div class="ui tiny header" style="margin-bottom: 6px;">РАСПОЗНАВАНИЕ 
-						<i style="margin-left:10px;display:inline-block" data="Для работы с модулем распознования необходим&#10;Tesseract-OCR v4.1.0 + языковой пакет rus.traineddata" class="question circle icon teal" onclick="orpa_helper_info('orpa_mouse_recognition');"></i>
+						<i style="margin-left:10px;display:inline-block"class="code icon teal" onclick="orpa_mouse_recognize_copy(); orpa_utils_popup_show(this, 'Код Python скопирован в буфер обмена! Для вставки используйте комбинацию клавиш Ctrl+V');"></i>
 
+						<i style="margin-left:0px;display:inline-block" data="Для работы с модулем распознования необходим&#10;Tesseract-OCR v4.1.0 + языковой пакет rus.traineddata" class="question circle icon teal" onclick="orpa_helper_info('orpa_mouse_recognition');"></i>
+						
 					</div>
 					<div>
 						<div class="ui input" style="width:86%; margin-bottom: 10px;">
 							<input type="text" id="orpa-screen-teseract-location" placeholder="Путь к изображению">
 						</div>
 						<button class="ui grey icon button" onclick="orpa_api_tesseract_render()" style="width:12%">
 							<i class="play icon"></i>
@@ -763,15 +825,21 @@
 		<!-- РАЗДЕЛ МЫШЬ & ЭКРАН -- ORPA-MOUSE -- КОНЕЦ -->
 
 		<script
 		src="/3rdParty/jQuery/jquery-3.1.1.min.js"
 		crossorigin="anonymous"></script>
 	  <script src="/3rdParty/Semantic-UI-CSS-master/semantic.min.js"></script>
 	  <script src="/orpa/resources/Web/orpa/std.js"></script>
-	  
+	  {% if is_linux_bool==False %}
+	  <script src="/orpa/resources/Web/orpa/std_desktop.js"></script>
+
+	   {% else %}
+	   <script src="/orpa/resources/Web/orpa/std_desktop_linux.js"></script>
+	  {% endif %}
+
 	  {% if is_ee_bool==True %}
 	  <script src="/orpa/resources/Web/orpa/std_browser.js"></script>
 	  <script src="/orpa/resources/Web/orpa/std_floidd.js"></script>
 	  {% endif %}
 	  <script src="/orpa/resources/Web/orpa/std_helper.js"></script>
 	  
 	  <script src="/orpa/resources/Web/Handlebars/handlebars-v4.1.2.js"></script>
@@ -832,21 +900,24 @@
 		<div id="orpa-utils-modal-uio-search-mouse" class="ui basic modal" style="text-align: center;">
 			<div class="ui icon header">
 				<i class="mouse pointer icon"></i>
 				Режим поиска UI объекта по курсору мыши
 				
 			</div>
 			<div class="content" style="text-align: left;">
+				<p>!ВНИМАНИЕ! НАЧИНАЯ С ВЕРСИИ ORPA 1.4.1 ПОМЕНЯЛИСЬ ФУНКЦИИ ГОРЯЧИХ КЛАВИШ, ОПИСАНИЕ СМ. НИЖЕ!</p>
+
 				<p>Уважаемый пользователь!</p>
 				<p>Инициирован режим поиска локального UI объекта по наведению курсора мыши.</p>
 				<p>Через несколько секунд ORPA перенесет вас в приложение для поиска объекта.</p>
 				<p>Ниже представлены доступные команды:</p>
 				<ul>
-					<li>Длительное нажатие <b>ctrl (левый или правый)</b>: Завершить поиск и вернуть UI объект, который был обнаружен по наведенному курсору мыши</li>
-					<li>Длительное нажатие <b>shift</b> или <b>alt</b>: Фиксация координат мыши на момент начала нажатия клавиши shift. Данная опция позволяет идентифицировать UI объект в том случае, когда он активен без наведенного курсора мыши. </li>
+					<li>Длительное нажатие <b>shift (левый или правый)</b>: Завершить поиск и вернуть UI объект, который был обнаружен по наведенному курсору мыши</li>
+					<li>Длительное нажатие <b>alt (левый или правый)</b>: Вывод всех Ui объектов, которые удовлетворяют условию нахождения под координатами мыши. Данная опция позволяет найти Ui объект, даже в том случае, если он перекрыт другим Ui слоем.</li>
+					<li>Длительное нажатие <b>ctrl (левый или правый)</b>: Фиксация координат мыши на момент начала нажатия клавиши shift. Данная опция позволяет идентифицировать UI объект в том случае, когда он активен без наведенного курсора мыши. </li>
 				</ul>
 				<p>Данное модальное окно будет открыто до момента завершения режима поиска.</p>
 			</div>
 		</div>
 		<!-- МОДАЛЬНОЕ ОКНО НЕ ОБНАРУЖЕНЫ ОБЪЕКТЫ ПО СЕЛЕКТОРУ -- КОНЕЦ -->
 
 	</body>
```

#### html2text {}

```diff
@@ -6,21 +6,27 @@
 {% if is_ee_bool==False %}
  {% endif %}  {% raw %}
  {% endraw %}  {% include 'header.xhtml' %}
 Ð Ð°Ð·Ð²ÐµÑÐ½ÑÑÑ Ð½Ð° Ð²ÐµÑÑ ÑÐºÑÐ°Ð½
 Ð¡Ð²ÐµÑÐ½ÑÑÑ Ð½Ð° ÑÐ°ÑÑÑ ÑÐºÑÐ°Ð½Ð°
 ÐÑÐ¾ÐµÐºÑ ÐÑÐ¸Ð»Ð¾Ð¶ÐµÐ½Ð¸Ðµ ÐÑÐ°ÑÐ·ÐµÑ ÐÐ»Ð°Ð²Ð¸Ð°ÑÑÑÐ° &
 ÐÑÑÐµÑ ÐÑÑÑ & Ð­ÐºÑÐ°Ð½
+ ÐÐ Ð ÐÐÐÐÐ Ð ÐÐÐ¢ÐÐÐ ÐÐ¢ÐÐÐ ÐÐÐÐÐÐ ÐÐÐÐ
+Ð ÐÐÐÐÐ¢ÐÐ Ð ÐÐÐÐÐ¢Ð¬ ÐÐÐÐÐÐ£ "ÐÐÐÐÐÐÐ¢Ð¬"
   ÐÑÐºÑÑÑÑ Ð² Ð¿ÑÐ¾Ð²Ð¾Ð´Ð½Ð¸ÐºÐµ    ÐÑÐºÑÑÑÑ / ÑÐ¾Ð·Ð´Ð°ÑÑ
 Ð¿ÑÐ¾ÐµÐºÑ    ÐÐ¾Ð»Ð½Ð¾ÑÐºÑÐ°Ð½Ð½ÑÐ¹ ÑÐµÐ¶Ð¸Ð¼    ÐÐ±Ð½Ð¾Ð²Ð¸ÑÑ
 
- UIA WIN32 :: | :: | :: |
+ {% if is_linux_bool==False %} UIA WIN32 {% else %} AT-SPI WNCK {% endif %} ::
+| :: | :: |
 UI ÐÐÐªÐÐÐ¢Ð« ÐÐÐ ÐÐÐ Ð¡ÐÐÐ¡ÐÐ
+{% if is_linux_bool==False %}
 [                    ]
- STR WC RE
+ STR WC RE {% else %}
+[                    ]
+ STR WC RE {% endif %}
 ÐÐ°Ð³ÑÑÐ¶Ð°ÐµÐ¼...
 Ð¡ÐÐÐÐÐ¢ÐÐ   UIO XPATH CSS
    ÐÐ¾Ð´ÑÐ²ÐµÑÐ¸ÑÑ     ÐÐ°Ð¹ÑÐ¸ Ð²ÑÐµ
 Ð£Ð ÐÐÐÐ ÐÐÐÐÐÐÐÐÐ¡Ð¢Ð
 Ð¡ÐÐÐ¢ 1 Ð¡ÐÐÐ¢ 2 Ð¡ÐÐÐ¢ 3 Ð¡ÐÐÐ¢ 4
 ÐÐ°Ð³ÑÑÐ¶Ð°ÐµÐ¼...
 ÐÐÐÐ¡Ð¢ÐÐÐ
@@ -59,33 +65,34 @@
 ÐÐ°Ð³ÑÑÐ¶Ð°ÐµÐ¼...
 Ð ÐÐÐ£ÐÐ¬Ð¢ÐÐ¢
 
  :: | :: | ::
 Ð¡ÐÐÐÐÐ¢ÐÐ   UIO XPATH CSS
 ÐÐÐÐÐÐÐÐ
 0.2 Ð¡ÐÐ. 1.0 Ð¡ÐÐ. 3.0 Ð¡ÐÐ. 5.0 Ð¡ÐÐ.
+Ð¡ÐÐÐÐÐ
+[                    ]
 Ð¢ÐÐÐ¡Ð¢
    ÐÑÐ¿Ð¾Ð»Ð½Ð¸ÑÑ
-Ð¡ÐÐÐÐÐ
- placeholder="Ð¡Ð¸Ð¼Ð²Ð¾Ð»">
+Ð¡ÐÐÐÐÐ + ÐÐÐÐ¡Ð¢ÐÐÐ
 
 Ð¤ÑÐ½ÐºÑÐ¸Ñ
 Down
 Up
 Wait
 Send
 
-ÐÐÐ Ð¯Ð§ÐÐ ÐÐÐÐÐÐ¨Ð
-CTRL ALT SHIFT  WIN +
-[                    ]
+Ð¡ÐÐÐÐÐ + ÐÐÐ Ð¯Ð§ÐÐ ÐÐÐÐÐÐ¨Ð
+CTRL ALT SHIFT WIN
   ÐÑÐ¿Ð¾Ð»Ð½Ð¸ÑÑ
 ÐÐ£Ð¤ÐÐ  ÐÐÐÐÐÐ
    ÐÑÐ¾ÑÐ¸ÑÐ°ÑÑ     Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ
 
- :: | :: | ::
+ {% if is_linux_bool==True %}  {% else %} {% endif %} ÐÐ Ð¤ÐÐÐÐ ÐÐ
+Ð¡Ð¢Ð ÐÐÐ :: | :: | ::
 ÐÐ ÐÐÐÐ¢
 [                    ]
 
 [                    ]
   ÐÑÑÐµÐ·Ð°ÑÑ
 ÐÐ ÐÐÐÐ ÐÐ¡ÐÐÐ¢Ð 
 ÐÐÐÐÐ Ð£ÐÐÐÐ
@@ -108,15 +115,17 @@
 Down
 Up
 ÐÑÐ³ÑÐ¼ÐµÐ½ÑÑ Ð¡ÐÐÐ¡ÐÐ Ð¡ÐÐÐÐÐ Ð¬
   ÐÑÐ¿Ð¾Ð»Ð½Ð¸ÑÑ
 Ð ÐÐ¡ÐÐÐÐÐÐÐÐÐÐ
 [                    ]
 
- {% if is_ee_bool==True %}
+ {% if is_linux_bool==False %}
+ {% else %}
+ {% endif %} {% if is_ee_bool==True %}
  {% endif %}
  {% include 'footer.xhtml' %}
 Here is the message text!
  ÐÐµ Ð¿Ð¾Ð½ÑÐ»
  ÐÐ¾Ð½ÑÐ»
  ÐÐµ ÑÐ´Ð°Ð»Ð¾ÑÑ Ð¾Ð±Ð½Ð°ÑÑÐ¶Ð¸ÑÑ UI Ð¾Ð±ÑÐµÐºÑÑ Ð¿Ð¾
 ÑÐµÐ»ÐµÐºÑÐ¾ÑÑ
@@ -138,25 +147,35 @@
       ÐÐ¾Ð¿ÑÐ¾Ð±ÑÐ¹ÑÐµ ÑÐµÐ¶Ð¸Ð¼ ÑÐ¸ÐºÑÐ°ÑÐ¸Ð¸ ÐºÐ¾Ð¾ÑÐ´Ð¸Ð½Ð°Ñ
       Ð¼ÑÑÐ¸.
     * ÐÐ·Ð¼ÐµÐ½Ð¸Ð»Ð°ÑÑ Ð²ÐµÑÑÑÐºÐ° UI ÑÐ»ÐµÐ¼ÐµÐ½ÑÐ¾Ð²
  ÐÐ°ÐºÑÑÑÑ
  ÐÐ¾Ð½ÑÑÐ½Ð¾
 
  Ð ÐµÐ¶Ð¸Ð¼ Ð¿Ð¾Ð¸ÑÐºÐ° UI Ð¾Ð±ÑÐµÐºÑÐ° Ð¿Ð¾ ÐºÑÑÑÐ¾ÑÑ Ð¼ÑÑÐ¸
+!ÐÐÐÐÐÐÐÐ! ÐÐÐ§ÐÐÐÐ¯ Ð¡ ÐÐÐ Ð¡ÐÐ ORPA 1.4.1
+ÐÐÐÐÐÐ¯ÐÐÐ¡Ð¬ Ð¤Ð£ÐÐÐ¦ÐÐ ÐÐÐ Ð¯Ð§ÐÐ¥ ÐÐÐÐÐÐ¨,
+ÐÐÐÐ¡ÐÐÐÐ Ð¡Ð. ÐÐÐÐ!
 Ð£Ð²Ð°Ð¶Ð°ÐµÐ¼ÑÐ¹ Ð¿Ð¾Ð»ÑÐ·Ð¾Ð²Ð°ÑÐµÐ»Ñ!
 ÐÐ½Ð¸ÑÐ¸Ð¸ÑÐ¾Ð²Ð°Ð½ ÑÐµÐ¶Ð¸Ð¼ Ð¿Ð¾Ð¸ÑÐºÐ° Ð»Ð¾ÐºÐ°Ð»ÑÐ½Ð¾Ð³Ð¾ UI
 Ð¾Ð±ÑÐµÐºÑÐ° Ð¿Ð¾ Ð½Ð°Ð²ÐµÐ´ÐµÐ½Ð¸Ñ ÐºÑÑÑÐ¾ÑÐ° Ð¼ÑÑÐ¸.
 Ð§ÐµÑÐµÐ· Ð½ÐµÑÐºÐ¾Ð»ÑÐºÐ¾ ÑÐµÐºÑÐ½Ð´ ORPA Ð¿ÐµÑÐµÐ½ÐµÑÐµÑ Ð²Ð°Ñ Ð²
 Ð¿ÑÐ¸Ð»Ð¾Ð¶ÐµÐ½Ð¸Ðµ Ð´Ð»Ñ Ð¿Ð¾Ð¸ÑÐºÐ° Ð¾Ð±ÑÐµÐºÑÐ°.
 ÐÐ¸Ð¶Ðµ Ð¿ÑÐµÐ´ÑÑÐ°Ð²Ð»ÐµÐ½Ñ Ð´Ð¾ÑÑÑÐ¿Ð½ÑÐµ ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ:
-    * ÐÐ»Ð¸ÑÐµÐ»ÑÐ½Ð¾Ðµ Ð½Ð°Ð¶Ð°ÑÐ¸Ðµ ctrl (Ð»ÐµÐ²ÑÐ¹ Ð¸Ð»Ð¸
+    * ÐÐ»Ð¸ÑÐµÐ»ÑÐ½Ð¾Ðµ Ð½Ð°Ð¶Ð°ÑÐ¸Ðµ shift (Ð»ÐµÐ²ÑÐ¹ Ð¸Ð»Ð¸
       Ð¿ÑÐ°Ð²ÑÐ¹): ÐÐ°Ð²ÐµÑÑÐ¸ÑÑ Ð¿Ð¾Ð¸ÑÐº Ð¸ Ð²ÐµÑÐ½ÑÑÑ UI
       Ð¾Ð±ÑÐµÐºÑ, ÐºÐ¾ÑÐ¾ÑÑÐ¹ Ð±ÑÐ» Ð¾Ð±Ð½Ð°ÑÑÐ¶ÐµÐ½ Ð¿Ð¾
       Ð½Ð°Ð²ÐµÐ´ÐµÐ½Ð½Ð¾Ð¼Ñ ÐºÑÑÑÐ¾ÑÑ Ð¼ÑÑÐ¸
-    * ÐÐ»Ð¸ÑÐµÐ»ÑÐ½Ð¾Ðµ Ð½Ð°Ð¶Ð°ÑÐ¸Ðµ shift Ð¸Ð»Ð¸ alt: Ð¤Ð¸ÐºÑÐ°ÑÐ¸Ñ
-      ÐºÐ¾Ð¾ÑÐ´Ð¸Ð½Ð°Ñ Ð¼ÑÑÐ¸ Ð½Ð° Ð¼Ð¾Ð¼ÐµÐ½Ñ Ð½Ð°ÑÐ°Ð»Ð° Ð½Ð°Ð¶Ð°ÑÐ¸Ñ
-      ÐºÐ»Ð°Ð²Ð¸ÑÐ¸ shift. ÐÐ°Ð½Ð½Ð°Ñ Ð¾Ð¿ÑÐ¸Ñ Ð¿Ð¾Ð·Ð²Ð¾Ð»ÑÐµÑ
+    * ÐÐ»Ð¸ÑÐµÐ»ÑÐ½Ð¾Ðµ Ð½Ð°Ð¶Ð°ÑÐ¸Ðµ alt (Ð»ÐµÐ²ÑÐ¹ Ð¸Ð»Ð¸ Ð¿ÑÐ°Ð²ÑÐ¹):
+      ÐÑÐ²Ð¾Ð´ Ð²ÑÐµÑ Ui Ð¾Ð±ÑÐµÐºÑÐ¾Ð², ÐºÐ¾ÑÐ¾ÑÑÐµ
+      ÑÐ´Ð¾Ð²Ð»ÐµÑÐ²Ð¾ÑÑÑÑ ÑÑÐ»Ð¾Ð²Ð¸Ñ Ð½Ð°ÑÐ¾Ð¶Ð´ÐµÐ½Ð¸Ñ Ð¿Ð¾Ð´
+      ÐºÐ¾Ð¾ÑÐ´Ð¸Ð½Ð°ÑÐ°Ð¼Ð¸ Ð¼ÑÑÐ¸. ÐÐ°Ð½Ð½Ð°Ñ Ð¾Ð¿ÑÐ¸Ñ
+      Ð¿Ð¾Ð·Ð²Ð¾Ð»ÑÐµÑ Ð½Ð°Ð¹ÑÐ¸ Ui Ð¾Ð±ÑÐµÐºÑ, Ð´Ð°Ð¶Ðµ Ð² ÑÐ¾Ð¼
+      ÑÐ»ÑÑÐ°Ðµ, ÐµÑÐ»Ð¸ Ð¾Ð½ Ð¿ÐµÑÐµÐºÑÑÑ Ð´ÑÑÐ³Ð¸Ð¼ Ui ÑÐ»Ð¾ÐµÐ¼.
+    * ÐÐ»Ð¸ÑÐµÐ»ÑÐ½Ð¾Ðµ Ð½Ð°Ð¶Ð°ÑÐ¸Ðµ ctrl (Ð»ÐµÐ²ÑÐ¹ Ð¸Ð»Ð¸
+      Ð¿ÑÐ°Ð²ÑÐ¹): Ð¤Ð¸ÐºÑÐ°ÑÐ¸Ñ ÐºÐ¾Ð¾ÑÐ´Ð¸Ð½Ð°Ñ Ð¼ÑÑÐ¸ Ð½Ð°
+      Ð¼Ð¾Ð¼ÐµÐ½Ñ Ð½Ð°ÑÐ°Ð»Ð° Ð½Ð°Ð¶Ð°ÑÐ¸Ñ ÐºÐ»Ð°Ð²Ð¸ÑÐ¸ shift.
+      ÐÐ°Ð½Ð½Ð°Ñ Ð¾Ð¿ÑÐ¸Ñ Ð¿Ð¾Ð·Ð²Ð¾Ð»ÑÐµÑ
       Ð¸Ð´ÐµÐ½ÑÐ¸ÑÐ¸ÑÐ¸ÑÐ¾Ð²Ð°ÑÑ UI Ð¾Ð±ÑÐµÐºÑ Ð² ÑÐ¾Ð¼ ÑÐ»ÑÑÐ°Ðµ,
       ÐºÐ¾Ð³Ð´Ð° Ð¾Ð½ Ð°ÐºÑÐ¸Ð²ÐµÐ½ Ð±ÐµÐ· Ð½Ð°Ð²ÐµÐ´ÐµÐ½Ð½Ð¾Ð³Ð¾
       ÐºÑÑÑÐ¾ÑÐ° Ð¼ÑÑÐ¸.
 ÐÐ°Ð½Ð½Ð¾Ðµ Ð¼Ð¾Ð´Ð°Ð»ÑÐ½Ð¾Ðµ Ð¾ÐºÐ½Ð¾ Ð±ÑÐ´ÐµÑ Ð¾ÑÐºÑÑÑÐ¾ Ð´Ð¾
 Ð¼Ð¾Ð¼ÐµÐ½ÑÐ° Ð·Ð°Ð²ÐµÑÑÐµÐ½Ð¸Ñ ÑÐµÐ¶Ð¸Ð¼Ð° Ð¿Ð¾Ð¸ÑÐºÐ°.
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std_browser.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std_browser.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std_floidd.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std_floidd.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/std_helper.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/std_helper.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,18 @@
         "title_str": "Подсказка по разделу действий",
         "description_str": "Окно активации действия / генерации Python кода. Доступны действия (функции) UI объектов, а также модуля pyOpenRPA.Robot.UIDesktop. В отношении всех выбранных действий доступна функция генерации Python кода (иконка </>). При нажатии, сгенерированный код Python помещается в буфер обмена. Далее этот код можно вставить в проект робота, например, на вкладке 'Проект'. Для функций поддерживается 2 формы ввода аргументов: в виде списка (кнопка СПИСОК) и в виде словаря (кнопка СЛОВАРЬ). Также панель действий поддерживает функциональность по просмотру свойств UI объектов. В случае выбора свойства поле Аргументы не будет доступно для ввода."
     },
     "orpa_desktop_selector": {
         "title_str": "Подсказка по разделу селектора",
         "description_str": "Окно формирования селектора (указателя на один или несколько UI объектов). Дополнительно (только в EE версии) поддерживается функциональность формирования селектора в форматах XPATH и CSS. Сформировать селектор автоматически можно с помощью соответсвующей кнопки в окне UI объекты."
     },
-
+    "orpa_desktop_selector_empty": {
+        "title_str": "Отсутствует селектор UIO / CSS / XPATH",
+        "description_str": "Невозможно выполнить запрашиваемое действие: требуется установить селектор в одном из форматов (UIO / CSS / XPATH). Установить селектор можно как в ручном режиме, так и с помощью средств автогенерации ORPA."
+    },
     "orpa_browser_ui_object": {
         "title_str": "Подсказка по разделу UI объектов",
         "description_str": "Одно из ключевых окон. Здесь можно исследовать структуру открытых приложений (их компонентов). Также здесь доступны такие опции как: Просмотр в виде дерева (кнопка 'Дерево') или в виде списка (кнопка 'Список'). В отношении каждого UI объекта доступны следующие действия: Подсветить UI объект, Поиск дочернего UI объекта с помощью мыши, Генерация UIO селектора, Развернуть дочерние UI объекты. Дополнительно (только в EE версии) можно воспользоваться универсальным поиском UI компонентов. Данный поиск ищет вхождение введенной текстовой строки в один или несколько атрибутов UI элемента. Допускается универсальный поиск в режимах STR (точное соответствие), WC (соответствие с использованием правил WildCard), RegExp (соответствие с использованием правил регулярных выражений)"
     },
     "orpa_browser_level_info": {
         "title_str": "Подсказка по разделу уровней вложенности",
         "description_str": "Окно по просмотру уровней вложенности до UI объекта. Выбрать UI объект можно в разделе UI объектов с помощью мыши. Дополнительно (только в EE версии) можно воспользоваться функцией сохранения контекста экрана в слоты 1 - 4. Данная функция позволяет работать над роботизацией нескольких UI объектов одновременно."
@@ -66,19 +69,23 @@
         "description_str": "Окно установки задержки перед инициализацией функции клавиатуры. Данная функциональность позволяет установить фокус там, где требуется перед выполнением действия."
     },
     "orpa_keyboard_text": {
         "title_str": "Подсказка по разделу текст",
         "description_str": "Печать произвольного текста по локации, где установлен фокус. ВНИМАНИЕ! В одной строке поддерживает символы разных языков! Не зависит от текущей раскладки клавиатуры."
     },
     "orpa_keyboard_symbol": {
-        "title_str": "Подсказка по разделу символа",
+        "title_str": "Подсказка по разделу символа + действия",
         "description_str": "Печать произвольного символа, где установлен фокус. ВНИМАНИЕ! Зависит от текущей раскладки клавиатуры."
     },
+    "orpa_keyboard_symbol_detect": {
+        "title_str": "Подсказка по разделу символа",
+        "description_str": "Идентификация символа, с которым произвести действия в разделах 'СИМВОЛ + ДЕЙСТВИЕ' или 'СИМВОЛ + ГОРЯЧИЕ КЛАВИШИ'. Данная функциональность позволяет выбрать допустимые варианты наименований клавиш. Также поле подсвечивается зеленым цветом в том случае, если автоматическое сопоставление выполнено успешно. Красный цвет, если выполнить автоматическое сопоставление не удалось."
+    },
     "orpa_keyboard_hotkey": {
-        "title_str": "Подсказка по разделу горячих клавиш",
+        "title_str": "Подсказка по разделу символа + горячих клавиш",
         "description_str": "Инициация нажатия комбинации горячих клавиш. ВНИМАНИЕ! Не зависит от текущей раскладки клавиатуры."
     },
 
     "orpa_mouse_project": {
         "title_str": "Подсказка по разделу проекта",
         "description_str": "Данное окно отображает перечень всех изображений, обнаруженных в папке. Выбранные изображения можно: распознать, найти на экране, переименовать, удалить. Для создания изображения необходимо нажать кнопку ВЫРЕЗАТЬ"
     },
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/Lato-Bold.woff2` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/Lato-Bold.woff2`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/Lato-Italic.woff2` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/Lato-Italic.woff2`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/Lato-Regular.woff2` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/Lato-Regular.woff2`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg1.jpg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg1.jpg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg10.jpg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg10.jpg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg2.jpg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg2.jpg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg3.jpg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg3.jpg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg4.jpg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg4.jpg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg5.jpg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg5.jpg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg6.jpg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg6.jpg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg7.jpg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg7.jpg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg8.jpg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg8.jpg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/bg9.jpg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/bg9.jpg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/docs.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/docs.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/docs.css.bak` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/docs.css.bak`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/docs.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/docs.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/dropdown.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/dropdown.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/easing.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/easing.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/header.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/header.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/highlight.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/highlight.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/home.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/home.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/home.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/home.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/jquery.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/less.min.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/less.min.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/nan.jpg` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/nan.jpg`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/ogImage.JPG` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/ogImage.JPG`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/ogImage.PNG` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/ogImage.PNG`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/pyOpenRPA_logo.png` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/pyOpenRPA_logo.png`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/segment.css` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/segment.css`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/sidebar.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/sidebar.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/transition.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/transition.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/visibility.js` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/visibility.js`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Resources/Web/orpa/styleset/white-image.png` & `pyOpenRPA-1.4.1/pyOpenRPA/Resources/Web/orpa/styleset/white-image.png`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/Audio.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/Audio.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/Clipboard.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/Clipboard.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/Mouse.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/Mouse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 from pyautogui import *
 import time
 
 WAIT_AFTER_SEC_FLOAT = 0.4 # Настройка модуля Mouse: Время, которое ожидать после выполнения любой операции модуля Mouse. Настройка является единой для всех участов кода, использующих модуль Mouse. Если для некоторой функции требуется изменить данное время ожидания, то в отношении этой функции можно применить соответсвующий аргумент.
 
+# "GetPosition" >pyautogui.Point (.x .y)
+def GetXY() -> Point:
+    """L+,W+: Получить координаты мыши
+    !ВНИМАНИЕ! Отсчет координат inXInt, inYInt начинается с левого верхнего края рабочей области (экрана).
+    
+    .. code-block:: python
+
+        # Mouse: Взаимодействие с мышью
+        from pyOpenRPA.Robot import Mouse
+        coord = Mouse.GetXY() #Получить координаты мыши
+        coord.x; coord.y;
+
+    """
+    return position()
+
 def Click(inXInt:int=None, inYInt:int=None, inClickCountInt:int=1, inIntervalSecFloat:float=0.0, inButtonStr:str='left', inMoveDurationSecFloat:float=0.0, inWaitAfterSecFloat:float=WAIT_AFTER_SEC_FLOAT):
     """L+,W+: Нажатие (вниз) кнопки мыши и затем немедленно выпуск (вверх) её. Допускается следующая параметризация. Если не указаны inXInt и inYInt - клик производится по месту нахождения указателя мыши.
 
     !ВНИМАНИЕ! Отсчет координат inXInt, inYInt начинается с левого верхнего края рабочей области (экрана).
     
     .. code-block:: python
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/OrchestratorConnector.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/OrchestratorConnector.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/README.md` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/README.md`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/Screen.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/Screen.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,42 +7,277 @@
 from pyOpenRPA.Tools import CrossOS
 from . import Mouse, Keyboard, UIDesktop
 if CrossOS.IS_WINDOWS_BOOL:
     from pywinauto import win32defines, win32structures, win32functions
     import win32api
 elif CrossOS.IS_LINUX_BOOL: 
     import tkinter as tk # Python 3
+    from Xlib import display
+    from PIL import Image
 from screeninfo import get_monitors
 import tkinter as tk
-from desktopmagic.screengrab_win32 import (
-getDisplayRects, saveScreenToBmp, saveRectToBmp, getScreenAsImage,
-getRectAsImage, getDisplaysAsImages)
-
+if CrossOS.IS_WINDOWS_BOOL:
+    from desktopmagic.screengrab_win32 import (
+    getDisplayRects, saveScreenToBmp, saveRectToBmp, getScreenAsImage,
+    getRectAsImage, getDisplaysAsImages)
 
+import subprocess
 import time
+import copy
 
 IMAGE_WAIT_SEC_FLOAT = 60
 IMAGE_WAIT_INTERVAL_SEC_FLOAT = 1.0
 
+class Box:
+    def __init__(self, left,top,width,height):
+        self.left = left
+        self.top = top
+        self.width = width
+        self.height = height
+    
+    left = 0
+    top = 0
+    width = 0
+    height = 0
+
+class Point:
+    def __init__(self, x,y):
+        self.x = x
+        self.y = y
+    
+    x = 0
+    y = 0
+
+def DisplayInfo():
+    """L+,W-: Получить информацию об экранах
+
+    .. code-block:: python
+
+        # Screen: Взаимодействие с экраном
+        from pyOpenRPA.Robot import Screen
+        Screen.DisplayInfo() # RESULT: [{'x': 0, 'y': 0, 'width': 1920, 'height': 1080, 'depth': 24}]
+
+    """
+    result_list = []
+    display_obj = display.Display()
+    screen_count = display_obj.screen_count()
+
+    for i in range(screen_count):
+        screen_obj = display_obj.screen(i)
+        root_window = screen_obj.root
+        geometry = root_window.get_geometry()
+        result_list.append({"x":geometry.x, "y":geometry.y, "width":geometry.width, "height": geometry.height, "depth": geometry.depth})
+    display_obj.close()
+    return result_list
+def DisplayBox(inBox):
+    """L+,W-: Скорректировать прямоугольную область Box под существующие экраны.
+
+    :param inBox: Прямоугольная область 
+    :type inBox: Box, list, dict
+    """
+    
+    inBox=BoxParse(inBox)
+    result_box = copy.copy(inBox)
+    display_list = DisplayInfo()
+    flag_display_overlay = False
+    for display in display_list:
+        display_box = BoxParse(display)
+        if BoxOverlay(inBox, display_box):
+            flag_display_overlay=True
+            if result_box.left<display_box.left: result_box.left = display_box.left
+            if result_box.top<display_box.top: result_box.top = display_box.top
+            if result_box.left+result_box.width>display_box.left+display_box.width: result_box.width = display_box.left+display_box.width
+            if result_box.top+result_box.height>display_box.top+display_box.height: result_box.height = display_box.top+display_box.height
+            break
+    if flag_display_overlay==False: return BoxParse([0,0,0,0])
+    return result_box
+
+def BoxToDict(inBox):
+    """L+,W+: Конвертировать объект Box в {"x":0, "y":0, "width":100, "height":100}
+
+    :param inBox: Прямоугольная область 
+    :type inBox: Box, list, dict
+    """
+    inBox=BoxParse(inBox)
+    return {"x":inBox.left, "y":inBox.top, "width":inBox.width, "height":inBox.height}
+
+def PointIsInBox(inPoint, inBox): 
+    """L+,W+: Проверить вхождение точки Point в прямоугольную область Box
+
+    .. code-block:: python
+
+        # Screen: Взаимодействие с экраном
+        from pyOpenRPA.Robot import Screen
+        # Поддерживает форматы
+        Screen.PointIsInBox([1,1], [10,10,200,200])
+        Screen.PointIsInBox((1,1), (1,1,200,200))
+        Screen.PointIsInBox({"x":1,"y":1}, {"x":1,"y":1, "w":200,"h":200})
+
+    """
+    lPoint = PointParse(inPoint)
+    lBox = BoxParse(inBox)
+    return (lPoint.x>=lBox.left and lPoint.x<=lBox.width+lBox.left and lPoint.y>=lBox.top and lPoint.y<=lBox.top+lBox.height)
 
-def BoxCreate(inTopInt:int, inLeftInt:int, inHeightInt:int, inWidthInt:int) -> pyscreeze.Box:
+def PointParse(*args, **kwargs):
+    """L+,W+: Создать экземпляр точки.
+
+    .. code-block:: python
+
+        # Screen: Взаимодействие с экраном
+        from pyOpenRPA.Robot import Screen
+        # Поддерживает форматы
+        Screen.PointParse(x=1,y=1)
+        Screen.PointParse(1,1)
+        Screen.PointParse(x=1,y=1)
+        Screen.PointParse(l=1,t=1)
+        Screen.PointParse([1,1])
+        Screen.PointParse((1,1))
+        Screen.PointParse({"x":1,"y":1})
+
+    """
+    lTopInt=0; lLeftInt=0;
+
+    if len(args)==2: # xywh
+        lLeftInt=args[0];lTopInt=args[1];
+    elif len(args)==1:
+        var = args[0]
+        if type(var) is pyscreeze.Point: return Point(x=var.x, y=var.y) #Передан корректный объект - конвертация не требуется
+        if (type(var) is tuple) or (type(var) is list):
+            lLeftInt=var[0];lTopInt=var[1];
+        elif (type(var) is dict):
+            for char in ["x","X","l","L","left","LEFT","Left"]: 
+                if char in var: lLeftInt=var[char]; break;
+            for char in ["y","Y","T","t","top","TOP","Top"]: 
+                if char in var: lTopInt=var[char]; break;
+            for char in ["w","W","width","WIDTH","Width"]: 
+                if char in var: lLeftInt=var[char]; break;
+            for char in ["h","H","height","HEIGHT","Height"]: 
+                if char in var: lTopInt=var[char]; break;
+            for char in ["r","R","right","RIGHT","Right"]: 
+                if char in var: lLeftInt=var[char]; break;
+            for char in ["b","B","bottom","BOTTOM","Bottom"]: 
+                if char in var: lTopInt=var[char]; break;
+        else:
+            attr_list = dir(var)
+            for char in ["x","X","l","L","left","LEFT","Left"]: 
+                if char in attr_list: lLeftInt=getattr(var,char); break;
+            for char in ["y","Y","T","t","top","TOP","Top"]: 
+                if char in attr_list: lTopInt=getattr(var,char); break;
+            for char in ["w","W","width","WIDTH","Width"]: 
+                if char in attr_list: lLeftInt=getattr(var,char); break;
+            for char in ["h","H","height","HEIGHT","Height"]: 
+                if char in attr_list: lTopInt=getattr(var,char); break;
+            for char in ["r","R","right","RIGHT","Right"]: 
+                if char in attr_list: lLeftInt=getattr(var,char); break;
+            for char in ["b","B","bottom","BOTTOM","Bottom"]: 
+                if char in attr_list: lTopInt=getattr(var,char); break;
+
+    if len(kwargs)>0:
+        for char in ["x","X","l","L","left","LEFT","Left"]: 
+            if char in kwargs: lLeftInt=kwargs[char]; break;
+        for char in ["y","Y","T","t","top","TOP","Top"]: 
+            if char in kwargs: lTopInt=kwargs[char]; break;
+        for char in ["w","W","width","WIDTH","Width"]: 
+            if char in kwargs: lLeftInt=kwargs[char]; break;
+        for char in ["h","H","height","HEIGHT","Height"]: 
+            if char in kwargs: lTopInt=kwargs[char]; break;
+        for char in ["r","R","right","RIGHT","Right"]: 
+            if char in kwargs: lLeftInt=kwargs[char]; break;
+        for char in ["b","B","bottom","BOTTOM","Bottom"]: 
+            if char in kwargs: lTopInt=kwargs[char]; break;
+    # СОЗДАТЬ ОБЪЕКТ BOX
+    return PointCreate(inXInt=lLeftInt, inYInt=lTopInt )
+
+def BoxParse(*args, **kwargs):
+    """L+,W+: Создать экземпляр прямоугольной области.
+
+    .. code-block:: python
+
+        # Screen: Взаимодействие с экраном
+        from pyOpenRPA.Robot import Screen
+        # Поддерживает форматы
+        Screen.BoxParse(x=1,y=1,w=900, h=90)
+        Screen.BoxParse(1,1,900, 90)
+        Screen.BoxParse(x=1,y=1,r=901, b=91)
+        Screen.BoxParse(x=1,y=1,r=901, bottom=91)
+        Screen.BoxParse([1,1,900, 90])
+        Screen.BoxParse((1,1,900, 90))
+        Screen.BoxParse({"x":1,"y":1,"w":900, "h":90})
+
+    """
+    lTopInt=0; lLeftInt=0; lHeightInt=0; lWidthInt=0
+
+    if len(args)==4: # xywh
+        lLeftInt=args[0];lTopInt=args[1];lWidthInt=args[2];lHeightInt=args[3]
+    elif len(args)==2: # wh == rb
+        lWidthInt=args[0];lHeightInt=args[1]
+    elif len(args)==1:
+        var = args[0]
+        if type(var) is pyscreeze.Box: return Box(left=var.left, top=var.top, width=var.width, height=var.height) #Передан корректный объект - конвертация не требуется
+        if (type(var) is tuple) or (type(var) is list):
+            lLeftInt=var[0];lTopInt=var[1];lWidthInt=var[2];lHeightInt=var[3]
+        elif (type(var) is dict):
+            for char in ["x","X","l","L","left","LEFT","Left"]: 
+                if char in var: lLeftInt=var[char]; break;
+            for char in ["y","Y","T","t","top","TOP","Top"]: 
+                if char in var: lTopInt=var[char]; break;
+            for char in ["w","W","width","WIDTH","Width"]: 
+                if char in var: lWidthInt=var[char]; break;
+            for char in ["h","H","height","HEIGHT","Height"]: 
+                if char in var: lHeightInt=var[char]; break;
+            for char in ["r","R","right","RIGHT","Right"]: 
+                if char in var: lWidthInt=var[char]-lLeftInt; break;
+            for char in ["b","B","bottom","BOTTOM","Bottom"]: 
+                if char in var: lHeightInt=var[char]-lTopInt; break;
+        else:
+            attr_list = dir(var)
+            for char in ["x","X","l","L","left","LEFT","Left"]: 
+                if char in attr_list: lLeftInt=getattr(var,char); break;
+            for char in ["y","Y","T","t","top","TOP","Top"]: 
+                if char in attr_list: lTopInt=getattr(var,char); break;
+            for char in ["w","W","width","WIDTH","Width"]: 
+                if char in attr_list: lWidthInt=getattr(var,char); break;
+            for char in ["h","H","height","HEIGHT","Height"]: 
+                if char in attr_list: lHeightInt=getattr(var,char); break;
+            for char in ["r","R","right","RIGHT","Right"]: 
+                if char in attr_list: lWidthInt=getattr(var,char)-lLeftInt; break;
+            for char in ["b","B","bottom","BOTTOM","Bottom"]: 
+                if char in attr_list: lHeightInt=getattr(var,char)-lTopInt; break;
+
+    if len(kwargs)>0:
+        for char in ["x","X","l","L","left","LEFT","Left"]: 
+            if char in kwargs: lLeftInt=kwargs[char]; break;
+        for char in ["y","Y","T","t","top","TOP","Top"]: 
+            if char in kwargs: lTopInt=kwargs[char]; break;
+        for char in ["w","W","width","WIDTH","Width"]: 
+            if char in kwargs: lWidthInt=kwargs[char]; break;
+        for char in ["h","H","height","HEIGHT","Height"]: 
+            if char in kwargs: lHeightInt=kwargs[char]; break;
+        for char in ["r","R","right","RIGHT","Right"]: 
+            if char in kwargs: lWidthInt=kwargs[char]-lLeftInt; break;
+        for char in ["b","B","bottom","BOTTOM","Bottom"]: 
+            if char in kwargs: lHeightInt=kwargs[char]-lTopInt; break;
+    # СОЗДАТЬ ОБЪЕКТ BOX
+    return BoxCreate(inTopInt=lTopInt, inLeftInt= lLeftInt, inHeightInt= lHeightInt, inWidthInt=lWidthInt)
+
+def BoxCreate(inTopInt:int, inLeftInt:int, inHeightInt:int, inWidthInt:int) -> Box:
     """L+,W+: Создать экземпляр прямоугольной области.
 
     !ВНИМАНИЕ! Координаты inTopInt, inLeftInt определяют верхний левый край прямоугольной области.
 
     :param inTopInt: Координата левой верхней точки в пикселях по оси X (горизонталь)
     :type inTopInt: int
     :param inLeftInt: Координата левой верхней точки в пикселях по оси Y (вертикаль)
     :type inLeftInt: int
     :param inHeightInt: Расстояние вниз от левой верхней точки в пикселях
     :type inHeightInt: int
     :param inWidthInt: Расстояние вправо от левой верхней точки в пикселях
     :type inWidthInt: int
     """
-    return pyscreeze.Box(top = inTopInt, left = inLeftInt, height = inHeightInt, width = inWidthInt)
+    return Box(top = inTopInt, left = inLeftInt, height = inHeightInt, width = inWidthInt)
 
 def BoxNormalize(*inArgList, **inAgrDict) -> list:
     pass
 
 def BoxMoveTo(inBox, inDXInt=None, inDYInt=None):
     """L+,W+: Переместить прямоугольную область (сохранить длину/ширину).
 
@@ -55,21 +290,21 @@
         # Вариант изменения 1-го элемента
         # Создать пробную прямоугольную область
         lBox = Screen.BoxCreate(inTopInt=10, inLeftInt=10, inHeightInt=10, inWidthInt=10)
         # Переместить пробную прямоугольную область
         lBox = Screen.BoxMoveTo(lBox, inDXInt=100, inDYInt=200)
         
     :param inBox: Экземпляр класса прямоугольной области Box
-    :type inBox: pyscreeze.Box
+    :type inBox: Box
     :param inDXInt: Смещение левой верхней координаты по оси X в пикселях (горизонтальная ось). 
     :type inDXInt: int, опциональный
     :param inDYInt: Смещение левой верхней координаты по оси Y в пикселях (вертикальная ось). 
     :type inDYInt: int, опциональный
     :return: Экземпляр класса прямоугольной области Box
-    :rtype: pyscreeze.Box
+    :rtype: Box
     """
     if type(inBox) is list:
         lResult = []
         for lBox in inBox:
             lResult.append(BoxMoveTo(lBox, inDXInt=inDXInt, inDYInt=inDYInt))
         return lResult
     else:
@@ -98,23 +333,23 @@
         lBox2 = Screen.BoxModify(lBox,10,10,"CC"); print(lBox2)
         lBox2 = Screen.BoxModify(lBox,10,10,"LU"); print(lBox2)
         lBox2 = Screen.BoxModify(lBox,10,10,"LD"); print(lBox2)
         lBox2 = Screen.BoxModify(lBox,10,10,"RU"); print(lBox2)
         lBox2 = Screen.BoxModify(lBox,10,10,"RD"); print(lBox2)
         
     :param inBox: Экземпляр класса прямоугольной области Box
-    :type inBox: pyscreeze.Box
+    :type inBox: Box
     :param inDXInt: Смещение левой верхней координаты по оси X в пикселях (горизонтальная ось). 
     :type inDXInt: int, опциональный
     :param inDYInt: Смещение левой верхней координаты по оси Y в пикселях (вертикальная ось). 
     :type inDYInt: int, опциональный
     :param inPointRuleStr: Символьное указание точки (подробнее см. выше), относительно которой выполнить изменение прямоугольной области. Допустимые значения: "CC" (по умолчанию), "LU", "LD", "RD", "RU"
     :type inPointRuleStr: str, опциональный
     :return: Экземпляр класса прямоугольной области Box
-    :rtype: pyscreeze.Box
+    :rtype: Box
     """
     if type(inBox) is list:
         lResult = []
         for lBox in inBox:
             lResult.append(BoxModify(lBox, inDWidthInt=inDWidthInt, inDHeightInt=inDHeightInt, inPointRuleStr=inPointRuleStr))
         return lResult
     else:
@@ -156,15 +391,15 @@
         # ВАРИАНТ ПАКЕТНОЙ ОТРИСОВКИ
         # Создать пробную прямоугольную область
         lBox = Screen.BoxCreate(inTopInt=10, inLeftInt=10, inHeightInt=100, inWidthInt=100)
         lBox2 = Screen.BoxCreate(inTopInt=60, inLeftInt=60, inHeightInt=100, inWidthInt=100)
         Screen.BoxDraw([lBox, lBox2])
 
     :param inBox: Экземпляр класса прямоугольной области Box
-    :type inBox: pyscreeze.Box
+    :type inBox: Box
     :param inColorStr: цвет подсветки прямоугольной области. Варианты: 'red', 'green', 'blue'. По умолчанию 'green'
     :type inColorStr: str, необязательный
     :param inThicknessInt: толщина подсветки прямоугольной области. По умолчанию 2
     :type inThicknessInt: int, необязательный
     """
     if type(inBox) is list:
         for lBox in inBox:
@@ -248,17 +483,17 @@
         lBox2 = Screen.BoxCreate(inTopInt=160, inLeftInt=160, inHeightInt=100, inWidthInt=100)
         lBox3 = Screen.BoxCreate(inTopInt=460, inLeftInt=60, inHeightInt=100, inWidthInt=100)
 
         l = Screen.BoxAnchorRuleCheck(inBox=lBox1, inAnchorBox=[lBox2,lBox3], inAnchorRuleStr=["LD","CUS"])
         Screen.BoxDraw([lBox1,lBox2,lBox3])
 
     :param inBox: Экземпляр класса прямоугольной области Box
-    :type inBox: pyscreeze.Box
+    :type inBox: Box
     :param inAnchorBox: Экземпляр класса прямоугольной области Box
-    :type inAnchorBox: pyscreeze.Box или list из pyscreeze.Box
+    :type inAnchorBox: Box или list из Box
     :param inAnchorRuleStr: Символьное указание области проверки соответствия. Может принимать единственное значение (единый формат для всех inAnchorBox), или список форматов для каждого inAnchorBox (если inAnchorBox является списком Box)
     :type inAnchorRuleStr: str или list из str
     :return: True - соответствует всем правилам
     :rtype: bool
     """
     # Формирование стартовых переменных
     if inAnchorBox is None: inAnchorBox = []
@@ -338,230 +573,314 @@
         from pyOpenRPA.Robot import Screen
         lBox1 = Screen.BoxCreate(inTopInt=10, inLeftInt=10, inHeightInt=100, inWidthInt=1000)
         lBox2 = Screen.BoxCreate(inTopInt=160, inLeftInt=160, inHeightInt=100, inWidthInt=100)
         Screen.BoxDraw([lBox1, lBox2])
         Screen.BoxOverlay(lBox1,lBox2)
 
     :param inBox1: Экземпляр класса прямоугольной области Box
-    :type inBox1: pyscreeze.Box
+    :type inBox1: Box
     :param inBox2: Экземпляр класса прямоугольной области Box
-    :type inBox2: pyscreeze.Box
+    :type inBox2: Box
     :return: True - inBox1 наложен на inBox2
     :rtype: bool
     """
     return not ((inBox1.left>inBox2.left + inBox2.width or inBox2.left>inBox1.left + inBox1.width) or (inBox1.top>inBox2.top + inBox2.height or inBox2.top>inBox1.top + inBox1.height))
 
 import re
-def BoxGetPoint(inBox, inPointRuleStr="CC") -> pyscreeze.Point:
-    """L+,W+:Получить точку pyscreeze.Point по заданной прямоугольной области pyscreeze.Box и строковому параметру расположения inPointRuleStr.
+def BoxGetPoint(inBox, inPointRuleStr="CC") -> Point:
+    """L+,W+:Получить точку Point по заданной прямоугольной области Box и строковому параметру расположения inPointRuleStr.
 
     .. code-block:: python
 
         # Screen: Взаимодействие с мышью объектами экрана
         from pyOpenRPA.Robot import Screen
         lBox1 = Screen.BoxCreate(inTopInt=10, inLeftInt=10, inHeightInt=100, inWidthInt=1000)
         lPoint = Screen.BoxGetPoint(inBox=lBox1, inPointRuleStr="LC")
 
     :param inBox: Прямоугольная область на экране
-    :type inBox: pyscreeze.Box, обязательный
+    :type inBox: Box, обязательный
     :param inPointRuleStr: Правило идентификации точки на прямоугольной области (правила формирования см. выше). Варианты: "LU","CU","RU","LC","CC","RC","LD","CD","RD".  По умолчанию "CC"
     :type inPointRuleStr: str, опциональный
     :return: Точка на экране
-    :rtype: pyscreeze.Point
+    :rtype: Screen.Point
     """
+    inBox= BoxParse(inBox) #Конвертация из разных типов (если необходимо)
     lPoint = None
     inPointRuleStr = inPointRuleStr.upper()
-    if "CC" in inPointRuleStr: lPoint = pyscreeze.Point(x=inBox.left + inBox.width/2,y=inBox.top + inBox.height/2)
-    elif "LU" in inPointRuleStr: lPoint = pyscreeze.Point(x=inBox.left,y=inBox.top)
-    elif "RU" in inPointRuleStr: lPoint = pyscreeze.Point(x=inBox.left + inBox.width,y=inBox.top)
-    elif "CU" in inPointRuleStr: lPoint = pyscreeze.Point(x=inBox.left + inBox.width/2,y=inBox.top)
-    elif "LC" in inPointRuleStr: lPoint = pyscreeze.Point(x=inBox.left,y=inBox.top + inBox.height/2)
-    elif "RC" in inPointRuleStr: lPoint = pyscreeze.Point(x=inBox.left + inBox.width,y=inBox.top + inBox.height/2)
-    elif "LD" in inPointRuleStr: lPoint = pyscreeze.Point(x=inBox.left,y=inBox.top + inBox.height)
-    elif "CD" in inPointRuleStr: lPoint = pyscreeze.Point(x=inBox.left + inBox.width/2,y=inBox.top + inBox.height)
-    elif "RD" in inPointRuleStr: lPoint = pyscreeze.Point(x=inBox.left + inBox.width,y=inBox.top + inBox.height)
+    if "CC" in inPointRuleStr: lPoint = Point(x=inBox.left + inBox.width/2,y=inBox.top + inBox.height/2)
+    elif "LU" in inPointRuleStr: lPoint = Point(x=inBox.left,y=inBox.top)
+    elif "RU" in inPointRuleStr: lPoint = Point(x=inBox.left + inBox.width,y=inBox.top)
+    elif "CU" in inPointRuleStr: lPoint = Point(x=inBox.left + inBox.width/2,y=inBox.top)
+    elif "LC" in inPointRuleStr: lPoint = Point(x=inBox.left,y=inBox.top + inBox.height/2)
+    elif "RC" in inPointRuleStr: lPoint = Point(x=inBox.left + inBox.width,y=inBox.top + inBox.height/2)
+    elif "LD" in inPointRuleStr: lPoint = Point(x=inBox.left,y=inBox.top + inBox.height)
+    elif "CD" in inPointRuleStr: lPoint = Point(x=inBox.left + inBox.width/2,y=inBox.top + inBox.height)
+    elif "RD" in inPointRuleStr: lPoint = Point(x=inBox.left + inBox.width,y=inBox.top + inBox.height)
     # Корректировка при необходимости
     lDXInt=0
     lDYInt=0
     lMatchY = re.search(r'.*Y([-+]?\d*).*', inPointRuleStr)
     if lMatchY is not None: lDYInt=int(lMatchY.group(1))
     lMatchX = re.search(r'.*X([-+]?\d*).*', inPointRuleStr)
     if lMatchX is not None: lDXInt=int(lMatchX.group(1))
     lPoint = PointModify(inPoint=lPoint,inDXInt=lDXInt,inDYInt=lDYInt)
     return lPoint
 
-def PointModify(inPoint, inDXInt, inDYInt) -> pyscreeze.Point:
-    """L+,W+:Скорректировать точку pyscreeze.Point.
+def PointModify(inPoint, inDXInt, inDYInt) -> Point:
+    """L+,W+:Скорректировать точку Point.
 
     .. code-block:: python
 
         # Screen: Взаимодействие с мышью объектами экрана
         from pyOpenRPA.Robot import Screen
         lPoint = Screen.PointCreate(inXInt=10, inYInt=10)
         lPoint = Screen.PointModify(inPoint=lPoint, inDXInt=90, inDYInt=10)
 
     :param inPoint: Точка на экране, по которой выполнить нажатие мыши
-    :type inPoint: pyscreeze.Point, обязательный
+    :type inPoint: Point, обязательный
     :param inDXInt: Смещение указателя мыши по оси X (горизонтальная ось). 
     :type inDXInt: int, опциональный
     :param inDYInt: Смещение указателя мыши по оси Y (вертикальная ось). 
     :type inDYInt: int, опциональный
     :return: Точка на экране
-    :rtype: pyscreeze.Point
+    :rtype: Screen.Point
     """
     return PointCreate(inXInt=inPoint.x+inDXInt, inYInt=inPoint.y+inDYInt)
 
+
+def PointFromBox(inBox, inRuleStr):
+    """L+,W+:Создать точку Point на основании прямоугольной области и символьного указания точки (см функцию BoxGetPoint).
+
+    .. code-block:: python
+
+        # Screen: Взаимодействие с мышью объектами экрана
+        from pyOpenRPA.Robot import Screen
+        lBox1 = Screen.PointFromBox(inTopInt=10, inLeftInt=10, inHeightInt=100, inWidthInt=1000)
+        lPoint = Screen.PointFromBox(inBox=lBox1, inPointRuleStr="LC")
+
+    :param inBox: Прямоугольная область на экране
+    :type inBox: Box, обязательный
+    :param inRuleStr: Правило идентификации точки на прямоугольной области (правила формирования см. выше). Варианты: "LU","CU","RU","LC","CC","RC","LD","CD","RD".  По умолчанию "CC"
+    :type inRuleStr: str, опциональный
+    :return: Точка на экране
+    :rtype: Screen.Point
+    """
+    return BoxGetPoint(inBox=inBox, inPointRuleStr=inRuleStr)
+
 def PointCreate(inXInt, inYInt):
-    """L+,W+:Создать точку pyscreeze.Point.
+    """L+,W+:Создать точку Point.
 
     .. code-block:: python
 
         # Screen: Взаимодействие с мышью объектами экрана
         from pyOpenRPA.Robot import Screen
         lPoint = Screen.PointCreate(inXInt=10, inYInt=10)
 
     :param inXInt: Смещение указателя мыши по оси X (горизонтальная ось). 
     :type inXInt: int, опциональный
     :param inYInt: Смещение указателя мыши по оси Y (вертикальная ось). 
     :type inYInt: int, опциональный
     :return: Точка на экране
-    :rtype: pyscreeze.Point
+    :rtype: Screen.Point
     """
-    return pyscreeze.Point(x=inXInt,y=inYInt)
+    return Point(x=inXInt,y=inYInt)
 
-def PointClick(inPoint:pyscreeze.Point, inClickCountInt:int=1, inIntervalSecFloat:float=0.0, inButtonStr:str='left', inMoveDurationSecFloat:float=0.0, inWaitAfterSecFloat:float=None):
+def PointClick(inPoint:Point, inClickCountInt:int=1, inIntervalSecFloat:float=0.0, inButtonStr:str='left', inMoveDurationSecFloat:float=0.0, inWaitAfterSecFloat:float=None):
     """L+,W+:Нажатие (вниз) кнопки мыши и затем немедленно выпуск (вверх) её. Допускается следующая параметризация.
 
     .. code-block:: python
 
         # Screen: Взаимодействие с мышью объектами экрана
         from pyOpenRPA.Robot import Screen
         lPoint = Screen.PointCreate(100,150)
         Screen.PointClick(lPoint) #Выполнить нажатие левой клавиши мыши
 
     :param inPoint: Точка на экране, по которой выполнить нажатие мыши
-    :type inPoint: pyscreeze.Point, обязательный
+    :type inPoint: Point, обязательный
     :param inClickCountInt: Количество нажатий (вниз и вверх) кнопкой мыши, По умолчанию 1
     :type inClickCountInt: int, опциональный
     :param inIntervalSecFloat: Интервал ожидания в секундах между нажатиями, По умолчанию 0.0
     :type inIntervalSecFloat: float, опциональный 
     :param inButtonStr: Номер кнопки, которую требуется нажать. Возможные варианты: 'left', 'middle', 'right' или 1, 2, 3. В остальных случаях инициирует исключение ValueError. По умолчанию 'left'
     :type inButtonStr: str, опциональный
     :param inMoveDurationSecFloat: Время перемещения указателя мыши, По умолчанию 0.0 (моментальное перемещение)
     :type inMoveDurationSecFloat: float, опциональный
     :param inWaitAfterSecFloat: Количество секунд, которые ожидать после выполнения операции. По умолчанию установлено в настройках модуля Mouse (базовое значение 0.4)
     :type inWaitAfterSecFloat: float, опциональный
     """
     Mouse.Click(inXInt=inPoint.x, inYInt=inPoint.y, inClickCountInt=inClickCountInt, inIntervalSecFloat=inIntervalSecFloat, inButtonStr=inButtonStr, inMoveDurationSecFloat=inMoveDurationSecFloat, inWaitAfterSecFloat=inWaitAfterSecFloat)
 
 
-def PointClickDouble(inPoint:pyscreeze.Point, inWaitAfterSecFloat:float=None):
+def PointClickDouble(inPoint:Point, inWaitAfterSecFloat:float=None):
     """L+,W+:Двойное нажатие левой клавиши мыши. Данное действие аналогично вызову функции (см. ниже).
 
     .. code-block:: python
 
         # Screen: Взаимодействие с мышью объектами экрана
         from pyOpenRPA.Robot import Screen
         lPoint = Screen.PointCreate(100,150)
         Screen.PointClickDouble(lPoint) #Выполнить двойное нажатие левой клавиши мыши
 
     :param inPoint: Точка на экране, по которой выполнить нажатие мыши
-    :type inPoint: pyscreeze.Point, обязательный
+    :type inPoint: Point, обязательный
     :param inWaitAfterSecFloat: Количество секунд, которые ожидать после выполнения операции. По умолчанию установлено в настройках модуля Mouse (базовое значение 0.4)
     :type inWaitAfterSecFloat: float, опциональный
     """
     Mouse.ClickDouble(inXInt=inPoint.x, inYInt=inPoint.y, inWaitAfterSecFloat=inWaitAfterSecFloat)
 
-def PointDown(inPoint:pyscreeze.Point, inButtonStr:str='left', inWaitAfterSecFloat:float=None):
+
+def PointDown(inPoint:Point, inButtonStr:str='left', inWaitAfterSecFloat:float=None):
     """L+,W+:Переместить указатель по координатам inPoint, после чего нажать (вниз) клавишу мыши и не отпускать до выполнения соответсвующей команды (см. Up). 
 
     .. code-block:: python
 
         # Screen: Взаимодействие с мышью объектами экрана
         from pyOpenRPA.Robot import Screen
         lPoint = Screen.PointCreate(100,150)
         Screen.PointDown(lPoint)
 
     :param inPoint: Точка на экране, по которой выполнить нажатие мыши
-    :type inPoint: pyscreeze.Point, обязательный
+    :type inPoint: Point, обязательный
     :param inButtonStr: Номер кнопки, которую требуется нажать. Возможные варианты: 'left', 'middle', 'right' или 1, 2, 3. В остальных случаях инициирует исключение ValueError. По умолчанию 'left'
     :type inButtonStr: str, опциональный
     :param inWaitAfterSecFloat: Количество секунд, которые ожидать после выполнения операции. По умолчанию установлено в настройках модуля Mouse (базовое значение 0.4)
     :type inWaitAfterSecFloat: float, опциональный
     """
     Mouse.Down(inXInt=inPoint.x, inYInt=inPoint.y,inButtonStr=inButtonStr, inWaitAfterSecFloat=inWaitAfterSecFloat)
 
-def PointUp(inPoint:pyscreeze.Point, inButtonStr:str='left', inWaitAfterSecFloat:float=None):
+def PointUp(inPoint:Point, inButtonStr:str='left', inWaitAfterSecFloat:float=None):
     """L+,W+:Отпустить (вверх) клавишу мыши.
 
     .. code-block:: python
 
         # Screen: Взаимодействие с мышью объектами экрана
         from pyOpenRPA.Robot import Screen
         lPoint = Screen.PointCreate(100,150)
         Screen.PointUp(lPoint)
 
     :param inPoint: Точка на экране, по которой выполнить нажатие мыши
-    :type inPoint: pyscreeze.Point, обязательный
+    :type inPoint: Point, обязательный
     :param inButtonStr: Номер кнопки, которую требуется поднять. Возможные варианты: 'left', 'middle', 'right' или 1, 2, 3. В остальных случаях инициирует исключение ValueError. По умолчанию 'left'
     :type inButtonStr: str, опциональный
     :param inWaitAfterSecFloat: Количество секунд, которые ожидать после выполнения операции. По умолчанию установлено в настройках модуля Mouse (базовое значение 0.4)
     :type inWaitAfterSecFloat: float, опциональный
     """
     Mouse.Up(inXInt=inPoint.x, inYInt=inPoint.y,inButtonStr=inButtonStr, inWaitAfterSecFloat=inWaitAfterSecFloat)
 
-def PointMoveTo(inPoint:pyscreeze.Point, inWaitAfterSecFloat:float=None):
+def PointMoveTo(inPoint:Point, inWaitAfterSecFloat:float=None):
     """L+,W+:Переместить указатель мыши на позицию inXInt, inYInt за время inMoveDurationSecFloat.
 
     !ВНИМАНИЕ! Отсчет координат inXInt, inYInt начинается с левого верхнего края рабочей области (экрана).
 
     .. code-block:: python
 
         # Screen: Взаимодействие с мышью объектами экрана
         from pyOpenRPA.Robot import Screen
         lPoint = Screen.PointCreate(100,150)
         Screen.PointMoveTo(inXInt=100, inYInt=200)
 
     :param inPoint: Точка на экране, по которой выполнить нажатие мыши
-    :type inPoint: pyscreeze.Point, обязательный
+    :type inPoint: Point, обязательный
     :param inWaitAfterSecFloat: Количество секунд, которые ожидать после выполнения операции. По умолчанию установлено в настройках модуля Mouse (базовое значение 0.4)
     :type inWaitAfterSecFloat: float, опциональный
     """
     Mouse.MoveTo(inXInt=inPoint.x, inYInt=inPoint.y, inWaitAfterSecFloat=inWaitAfterSecFloat)
 
+
+def is_base64(s):
+    if os.path.exists(s): return False
+    try:
+        # декодируем строку base64
+        base64.decodebytes(s.encode())
+        # если декодирование прошло успешно, то строка является форматом base64
+        return True
+    except:
+        # если декодирование не удалось, то строка не является форматом base64
+        return False
+from io import BytesIO
+from PIL import Image
+import pytesseract
+
+def ImageRecognize(inImgPathStr:str, inLangStr = "rus+eng"):
+    """L+,W+: Выполнить распознавание текста на изображении
+
+    .. code-block:: python
+
+        # Screen: Взаимодействие с объектами экрана
+        from pyOpenRPA.Robot import Screen
+        RecognizedStr = Screen.ImageRecognize(inImgPathStr="Button.png")
+
+    :param inImgPathStr: Путь к изображению / Строка Base64 / Список bytes, которое требуется искать на экране.
+    :type inImgPathStr: str, относительный или абсолютный
+    :param inLangStr: Языки, используемые для распознавания. По умолчанию rus+eng
+    :type inLangStr: str, опционально
+    :return: Список из Box
+    :rtype: list
+    """
+    # ЕСЛИ ПОСТУПИЛ BASE 64
+    if is_base64(inImgPathStr):
+        imgdata = base64.b64decode(inImgPathStr)
+        return pytesseract.image_to_string(Image.open(BytesIO(imgdata)), lang = inLangStr)
+    else:
+        inImgPathStr = CrossOS.PathStr(inImgPathStr)
+        return pytesseract.image_to_string(Image.open(inImgPathStr), lang = inLangStr)
+    
 def ImageLocateAll(inImgPathStr:str, inIsGrayModeBool:bool=False, inConfidenceFloat:float=None) -> list:
-    """L+W+: Искать на экране графические объекты, которые похожи на inImgPathStr. Вернуть список прямоугольных областей на экране (pyscreeze.Box)
+    """L+,W+: Искать на экране графические объекты, которые похожи на inImgPathStr. Вернуть список прямоугольных областей на экране (Box)
 
     !ВНИМАНИЕ! Для использования параметра точности inConfidenceFloat необходим пакет Python opencv-python (python -m pip install opencv-python)
 
     .. code-block:: python
 
         # Screen: Взаимодействие с объектами экрана
         from pyOpenRPA.Robot import Screen
         Screen.ImageLocateAll(inImgPathStr="Button.png",inConfidenceFloat=0.9)
 
-    :param inImgPathStr: Путь к изображению, которое требуется искать на экране
+    :param inImgPathStr: Путь к изображению / Строка Base64 / Список bytes, которое требуется искать на экране.
     :type inImgPathStr: str, относительный или абсолютный
     :param inIsGrayModeBool: True - выполнить поиск изображения в режиме серых оттенков (ускоряет производительность, если допускается искажение цвета). По умолчанию False
     :type inIsGrayModeBool: bool, опционально
     :param inConfidenceFloat: Показатель точности. 1.0 - идентичное соответствие, 0.0 - полное несоответствие. По умолчанию 1.0 (None)
     :type inConfidenceFloat: float, опционально
-    :return: Список из pyscreeze.Box
+    :return: Список из Box
     :rtype: list
     """
     lResult = []
-    if inConfidenceFloat is None or inConfidenceFloat==1: lLocateList = pyautogui.locateAllOnScreen(image = inImgPathStr, grayscale = inIsGrayModeBool)
-    else: lLocateList = pyautogui.locateAllOnScreen(image = inImgPathStr, grayscale = inIsGrayModeBool, confidence = inConfidenceFloat)
-    for lItem in lLocateList:
-        lResult.append(lItem)
-    if __define__.DEFINE_ACCEPTED==True: return lResult
-    else: []
+    # ЕСЛИ ПОСТУПИЛ BASE 64
+    if is_base64(inImgPathStr):
+            imgdata = base64.b64decode(inImgPathStr)
+            img = Image.open(BytesIO(imgdata))
+            if inConfidenceFloat is None or inConfidenceFloat==1: lLocateList = pyautogui.locateAllOnScreen(image = img, grayscale = inIsGrayModeBool)
+            else: lLocateList = pyautogui.locateAllOnScreen(image = img, grayscale = inIsGrayModeBool, confidence = inConfidenceFloat)
+            for lItem in lLocateList:
+                lResult.append(lItem)
+            img.close()
+            if __define__.DEFINE_ACCEPTED==True: return lResult
+            else: []
+    # ЕСЛИ ПОСТУПИЛ BYTES
+    elif type(inImgPathStr) is bytes:
+            img = Image.open(BytesIO(inImgPathStr))
+            if inConfidenceFloat is None or inConfidenceFloat==1: lLocateList = pyautogui.locateAllOnScreen(image = img, grayscale = inIsGrayModeBool)
+            else: lLocateList = pyautogui.locateAllOnScreen(image = img, grayscale = inIsGrayModeBool, confidence = inConfidenceFloat)
+            for lItem in lLocateList:
+                lResult.append(lItem)
+            img.close()
+            if __define__.DEFINE_ACCEPTED==True: return lResult
+            else: []
+    else:
+        inImgPathStr = CrossOS.PathStr(inImgPathStr)
+        if inConfidenceFloat is None or inConfidenceFloat==1: lLocateList = pyautogui.locateAllOnScreen(image = inImgPathStr, grayscale = inIsGrayModeBool)
+        else: lLocateList = pyautogui.locateAllOnScreen(image = inImgPathStr, grayscale = inIsGrayModeBool, confidence = inConfidenceFloat)
+        for lItem in lLocateList:
+            lResult.append(lItem)
+        if __define__.DEFINE_ACCEPTED==True: return lResult
+        else: []
 from ..Utils import __define__
 def ImageLocateAllInfo(inImgPathStr:str, inIsGrayModeBool:bool=False, inConfidenceFloat:float=None) -> list:
-    """L+W+: Искать на экране графические объекты, которые похожи на inImgPathStr. Вернуть список прямоугольных областей на экране (pyscreeze.Box)
+    """L+W+: Искать на экране графические объекты, которые похожи на inImgPathStr. Вернуть список прямоугольных областей на экране (Box)
 
     !ВНИМАНИЕ! Для использования параметра точности inConfidenceFloat необходим пакет Python opencv-python (python -m pip install opencv-python)
 
     .. code-block:: python
 
         # Screen: Взаимодействие с объектами экрана
         from pyOpenRPA.Robot import Screen
@@ -597,15 +916,15 @@
 
     :param inImgPathStr: Путь к изображению, которое требуется искать на экране
     :type inImgPathStr: str, относительный или абсолютный
     :param inIsGrayModeBool: True - выполнить поиск изображения в режиме серых оттенков (ускоряет производительность, если допускается искажение цвета). По умолчанию False
     :type inIsGrayModeBool: bool, опционально
     :param inConfidenceFloat: Показатель точности. 1.0 - идентичное соответствие, 0.0 - полное несоответствие. По умолчанию 1.0 (None)
     :type inConfidenceFloat: float, опционально
-    :return: Список из pyscreeze.Box
+    :return: Список из Box
     :rtype: list
     """
     lLocateList = ImageLocateAll(inImgPathStr=inImgPathStr,inIsGrayModeBool=inIsGrayModeBool, inConfidenceFloat=inConfidenceFloat)
     return len(lLocateList)>0
 
 
 def ImageWaitAppear(inImgPathStr:str, inWaitSecFloat:float=IMAGE_WAIT_SEC_FLOAT, inWaitIntervalSecFloat:float = IMAGE_WAIT_INTERVAL_SEC_FLOAT, inIsGrayModeBool:bool=False, inConfidenceFloat:float=None) -> list:
@@ -626,15 +945,15 @@
     :type inWaitSecFloat: float, опциональный
     :param inWaitIntervalSecFloat: Интервал повторной проверки наличия изображения. По умолчанию IMAGE_WAIT_INTERVAL_SEC_FLOAT (1)
     :type inWaitIntervalSecFloat: float, опциональный
     :param inIsGrayModeBool: True - выполнить поиск изображения в режиме серых оттенков (ускоряет производительность, если допускается искажение цвета). По умолчанию False
     :type inIsGrayModeBool: bool, опционально
     :param inConfidenceFloat: Показатель точности. 1.0 - идентичное соответствие, 0.0 - полное несоответствие. По умолчанию 1.0 (None)
     :type inConfidenceFloat: float, опционально
-    :return: Список из pyscreeze.Box или [] если прошло время ожидания.
+    :return: Список из Box или [] если прошло время ожидания.
     :rtype: list
     """
     lStartSecFloat = time.time()
     lResultList=[]
     while time.time() - lStartSecFloat < inWaitSecFloat:
         lResultList = ImageLocateAll(inImgPathStr=inImgPathStr,inIsGrayModeBool=inIsGrayModeBool, inConfidenceFloat=inConfidenceFloat)
         if len(lResultList)>0: break
@@ -668,14 +987,37 @@
     lStartSecFloat = time.time()
     lResultList=[]
     while time.time() - lStartSecFloat < inWaitSecFloat:
         lResultList = ImageLocateAll(inImgPathStr=inImgPathStr,inIsGrayModeBool=inIsGrayModeBool, inConfidenceFloat=inConfidenceFloat)
         if len(lResultList)==0: break
         time.sleep(inWaitIntervalSecFloat)
     return lResultList
+import os
+import base64
+def ImageToBase64(inImgPathStr:str, inLimitBytesInt:int=30000) -> str:
+    """L+,W+: Открыть файл и преобразовать содержимое изображения в формат base64 (в виде строки). Вернуть None, если файл не существует или превышает допустимый размер
+
+    .. code-block:: python
+
+        # Screen: Взаимодействие с объектами экрана
+        from pyOpenRPA.Robot import Screen
+        ImageBase64Str = Screen.ImageToBase64(inImgPathStr="Button.png")
+        ImageBytes = base64.b64decode(ImageBase64Str.encode())
+
+    """
+    inImgPathStr = CrossOS.PathStr(inImgPathStr)
+    str = None
+    if os.path.exists(inImgPathStr):
+        log = b""
+        with open(inImgPathStr, "rb") as f:
+            log = f.read()
+        if len(log) < inLimitBytesInt:
+            str = base64.b64encode(log).decode()
+    return str
+    
 
 def ImageClick(inImgPathStr:str,inBoxIndexInt:int = 0, inPointRuleStr:str="CC",  inIsGrayModeBool:bool=False, inConfidenceFloat:float=None, inWaitSecFloat:float=0, inWaitIntervalSecFloat:float = 0):
     """L+,W+:Выполнить поиск прямоугольной области по изображению.
 
     !ВНИМАНИЕ! Для использования параметра точности inConfidenceFloat необходим пакет Python opencv-python (python -m pip install opencv-python)
 
 
@@ -732,63 +1074,76 @@
         # Разрешение
         lResult.append([int((lMonitor[2][2]-lMonitor[2][0])*lScaleFactor.value/100),int((lMonitor[2][3]-lMonitor[2][1])*lScaleFactor.value/100)])
     return lResult
 
 
 class SnipingTool(tk.Frame):
     def __init__(self, parent, path):
-        """L-,W+: Инициализация экземпляра класса SnipingTool
+        """L+,W+: Инициализация экземпляра класса SnipingTool
+
+        ВНИМАНИЕ В LINUX ПРИ ВЫРЕЗАНИИ ЧАСТИ ЭКРАНА НЕ ПРОИСХОДИТ ЗАТЕМНЕНИЯ - СВЯЗАНО С ОСОБЕННОСТЯМИ ГРАФИЧЕСКИХ ОКОН В LINUX
 
         .. code-block:: python
             from pyOpenRPA.Robot import Screen
             lRoot = tk.Tk()
             app = Screen.SnipingTool(parent=lRoot, path=inPath)
 
         :param parent: Верхнеуровневый виджет
         :type parent: экземпляр класса Tk
         :param path: Путь, по которому будет сохранена выделенная область
         :type path: str, относительный или абсолютный
         """
-        tk.Frame.__init__(self, parent)
-        self.root = parent
-        self.path = path
-        self.root.config(cursor="cross")#Изменение курсора
-        self.root.attributes('-alpha', 0.2) #Установить прозрачность
-        #Определить общее разрешение экрана/ов
-        self.width, self.height = self.getMonitorsResolution()
-        self.root.geometry( f"{self.width}x{self.height}" ) #Установить размеры окна snipingtool
-        #Установить безрамочный режим и верхний уровень
-        self.root.overrideredirect(1)
-        self.root.attributes('-topmost', True)
-        self._createVariables(parent)
-        self._createCanvas()
-        self._createCanvasBinding()
+        self.path = CrossOS.PathStr(path) 
+        if CrossOS.IS_WINDOWS_BOOL:
+            tk.Frame.__init__(self, parent)
+            self.root = parent
+            self.root.config(cursor="cross")#Изменение курсора
+            self.root.attributes('-alpha', 0.2) #Установить прозрачность
+            #Определить общее разрешение экрана/ов
+            self.width, self.height = self.getMonitorsResolution()
+            self.root.geometry( f"{self.width}x{self.height}" ) #Установить размеры окна snipingtool
+            
+            #Установить безрамочный режим и верхний уровень
+            self.root.overrideredirect(1)
+            self.root.attributes('-topmost', True)
+            self._createVariables(parent)
+            self._createCanvas()
+            self._createCanvasBinding()
 
     def getMonitorsResolution(self):
-        """L-,W+: Определение разрешения всей области экрана (охватывает все подключенные мониторы)
+        """L+,W+: Определение разрешения всей области экрана (охватывает все подключенные мониторы)
 
         .. code-block:: python
             from pyOpenRPA.Robot import Screen
             lRoot = tk.Tk()
             app = Screen.SnipingTool(parent=lRoot, path=inPath)
             lResolution = app.getMonitorsResolution()
         """
         mHeight = 0
         mWidth = 0
-        for mMonitor in win32api.EnumDisplayMonitors():
-            # Определение hadle у монитора
-            mHandle = mMonitor[0].Detach()
-            # Подгрузка shcore
-            shcore = ctypes.WinDLL('shcore')
-            # Множитель мастшабирования монитора
-            mScaleFactor = ctypes.c_uint()
-            shcore.GetScaleFactorForMonitor(mHandle, ctypes.byref(mScaleFactor))
-            # Разрешение
-            if mHeight < (mMonitor[2][3] - mMonitor[2][1])*(mScaleFactor.value/100): mHeight = int((mMonitor[2][3] - mMonitor[2][1])*(mScaleFactor.value/100))
-            mWidth += int((mMonitor[2][2] - mMonitor[2][0])*(mScaleFactor.value/100))
+        if CrossOS.IS_WINDOWS_BOOL:
+            for mMonitor in win32api.EnumDisplayMonitors():
+                # Определение hadle у монитора
+                mHandle = mMonitor[0].Detach()
+                # Подгрузка shcore
+                shcore = ctypes.WinDLL('shcore')
+                # Множитель мастшабирования монитора
+                mScaleFactor = ctypes.c_uint()
+                shcore.GetScaleFactorForMonitor(mHandle, ctypes.byref(mScaleFactor))
+                # Разрешение
+                if mHeight < (mMonitor[2][3] - mMonitor[2][1])*(mScaleFactor.value/100): mHeight = int((mMonitor[2][3] - mMonitor[2][1])*(mScaleFactor.value/100))
+                mWidth += int((mMonitor[2][2] - mMonitor[2][0])*(mScaleFactor.value/100))
+        else:
+            for i in range(display.Display().screen_count()):
+                screen = display.Display().screen(i)
+                loc_width = screen.root.get_geometry().width
+                loc_height = screen.root.get_geometry().height
+                # Разрешение
+                if mHeight < (loc_height): mHeight = int(loc_height)
+                mWidth += int(loc_width)
         return mWidth, mHeight
 
     def _createVariables(self, parent):
         self.parent = parent
         self.rectx0 = 0
         self.recty0 = 0
         self.rectx1 = 0
@@ -837,24 +1192,30 @@
         #Определение конечных координат выделяемой области
         self.rectx1 = self.canvas.canvasx(event.x)
         self.recty1 = self.canvas.canvasy(event.y)
         self.canvas.delete("all")
         self.parent.attributes('-alpha', 0.0)
         self.root.destroy()
         #Сохранение прямоугольной области как изображение  
-        mImg = getRectAsImage(
-            (
-                int(self.rectx0 if self.rectx0 <= self.rectx1 else self.rectx1), 
-                int(self.recty0 if self.recty0 <= self.recty1 else self.recty1), 
-                int(self.rectx1 if self.rectx0 <= self.rectx1 else self.rectx0), 
-                int(self.recty1 if self.recty0 <= self.recty1 else self.recty0)
+        if CrossOS.IS_WINDOWS_BOOL:
+            mImg = getRectAsImage(
+                (
+                    int(self.rectx0 if self.rectx0 <= self.rectx1 else self.rectx1), 
+                    int(self.recty0 if self.recty0 <= self.recty1 else self.recty1), 
+                    int(self.rectx1 if self.rectx0 <= self.rectx1 else self.rectx0), 
+                    int(self.recty1 if self.recty0 <= self.recty1 else self.recty0)
+                )
             )
-        )
-        mImg.save(self.path)
-
+            mImg.save(self.path)
+        else:
+            #print(" ".join(['scrot', '-s', f'{self.rectx0},{self.rectx1},{self.recty0},{self.recty1}', self.path]))
+            subprocess.run(['scrot', self.path], capture_output=True, text=True)
+            mImg = Image.open(self.path)
+            mImg = mImg.crop((self.rectx0,self.recty0,self.rectx1,self.recty1))
+            mImg.save(self.path)
 
 gThreadStopFlag = False
 # Функция для minimize/maximize окна tkintera
 def WindowMinimize(inRoot):
     lSelector = [{"title":"tk","class_name":"TkTopLevel","backend":"win32"}]
     lFlag = False
     global gThreadStopFlag
@@ -880,20 +1241,23 @@
         # Screen: Взаимодействие с объектами экрана
         from pyOpenRPA.Robot import Screen
         Screen.InitSnipingTool(inPath="Screenshot.png")
 
     :param inPath: Путь, по которому будет сохранена выделенная область
     :type inPath: str, относительный или абсолютный
     """
-    global gThreadStopFlag
-    lRoot = tk.Tk()
-    def quit(l) -> None:
-        lRoot.destroy()  
-    lRoot.bind("<Escape>",quit) #Установить esc как кнопку выхода
-    app = SnipingTool(lRoot,inPath)
-    #Инициализация потока для сворачивания окна (Зажать кнопку CTRL)
-    lThread = threading.Thread(target=WindowMinimize, args=(lRoot,), daemon=True)
-    lThread.start()
-    lRoot.mainloop()
-    gThreadStopFlag = True #Посылаем сигнал для остановки потока
-    lThread.join()
-
+    if CrossOS.IS_WINDOWS_BOOL:
+        global gThreadStopFlag
+        lRoot = tk.Tk()
+        def quit(l) -> None:
+            lRoot.destroy()  
+        lRoot.bind("<Escape>",quit) #Установить esc как кнопку выхода
+        app = SnipingTool(lRoot,inPath)
+        #Инициализация потока для сворачивания окна (Зажать кнопку CTRL)
+        lThread = threading.Thread(target=WindowMinimize, args=(lRoot,), daemon=True)
+        lThread.start()
+        lRoot.mainloop()
+        gThreadStopFlag = True #Посылаем сигнал для остановки потока
+        lThread.join()
+    else:
+        inPath = CrossOS.PathStr(inPath)
+        subprocess.run(['scrot', '-s',inPath], capture_output=True, text=True)
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/SettingsTemplate.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/SettingsTemplate.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/Test.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/Test.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/UIDesktop.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/UIDesktop.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
 #   },
 #   { ... }
 #
 #]
 from ..Utils import __define__
 #Default parameters
 mDefaultPywinautoBackend="win32"
+if CrossOS.IS_WINDOWS_BOOL == False:
+    mDefaultPywinautoBackend="at-spi"
 
 ############################
 #Новая версия
 ############################
 #Получить список элементов, который удовлетворяет условиям через расширенный движок поиска
 #[
 #   {
@@ -102,15 +104,15 @@
 #       "rich_text" - наименование rich_text
 #   }
 #]
 
 
 #old:PywinautoExtElementsGet
 def UIOSelector_Get_UIOList (inSpecificationList,inElement=None,inFlagRaiseException=True):
-    '''L-,W+: Получить список UIO объектов по UIO селектору
+    '''L+,W+: Получить список UIO объектов по UIO селектору
     
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
         # 1С: UIO Селектор выбора базы
         lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"},{"title":"DEMO", "depth_start": 5, "depth_end": 5}]		
@@ -342,15 +344,15 @@
 
     except Exception as e:
         if inFlagRaiseException: raise e
         else: return []
 
 #old:PywinautoExtElementGet
 def UIOSelector_Get_UIO (inSpecificationList,inElement=None,inFlagRaiseException=True):
-    '''L-,W+: Получить список UIO объект по UIO селектору. Если критериям UIO селектора удовлетворяет несколько UIO объектов - вернуть первый из списка
+    '''L+,W+: Получить список UIO объект по UIO селектору. Если критериям UIO селектора удовлетворяет несколько UIO объектов - вернуть первый из списка
     
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
         # 1С: UIO Селектор выбора базы
         lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"},{"title":"DEMO", "depth_start": 5, "depth_end": 5}]		
@@ -371,15 +373,15 @@
     lResultList=UIOSelector_Get_UIOList(inSpecificationList,inElement,inFlagRaiseException)
     if len(lResultList)>0:
         lResult=lResultList[0]
     return lResult
     
 #old:-
 def UIOSelector_Exist_Bool (inUIOSelector, inFlagRaiseException=True):
-    '''L-,W+: Проверить существование хотя бы 1-го UIO объекта по заданному UIO селектору
+    '''L+,W+: Проверить существование хотя бы 1-го UIO объекта по заданному UIO селектору
     
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
     
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -419,15 +421,15 @@
                 f"Exception was occured in child process (message): {lPIPEResponseDict['ErrorMessage']}, (traceback): {lPIPEResponseDict['ErrorTraceback']}")
         else:
             lResult = lPIPEResponseDict["Result"]
     return lResult
 
 #old: -
 def UIOSelectorsSecs_WaitAppear_List (inSpecificationListList,inWaitSecs=86400.0,inFlagWaitAllInMoment=False, inFlagRaiseException=True):
-    '''L-,W+: Ожидать появление хотя бы 1-го / всех UIO объектов по заданным UIO селекторам
+    '''L+,W+: Ожидать появление хотя бы 1-го / всех UIO объектов по заданным UIO селекторам
     
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
     
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -480,15 +482,15 @@
         if lResultFlag == False:
             lSecsDone=lSecsDone+lSecsSleep
             time.sleep(lSecsSleep)
     return lResultList
 
 #old: -
 def UIOSelectorsSecs_WaitDisappear_List (inSpecificationListList,inWaitSecs=86400.0,inFlagWaitAllInMoment=False, inFlagRaiseException=True):
-    '''L-,W+:  Ожидать исчезновение хотя бы 1-го / всех UIO объектов по заданным UIO селекторам
+    '''L+,W+:  Ожидать исчезновение хотя бы 1-го / всех UIO объектов по заданным UIO селекторам
     
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
     
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -541,15 +543,15 @@
         if lResultFlag == False:
             lSecsDone=lSecsDone+lSecsSleep
             time.sleep(lSecsSleep)
     return lResultList
 
 #old: -
 def UIOSelectorSecs_WaitAppear_Bool (inSpecificationList,inWaitSecs, inFlagRaiseException=True):
-    '''L-,W+: Ожидать появление 1-го UIO объекта по заданному UIO селектору
+    '''L+,W+: Ожидать появление 1-го UIO объекта по заданному UIO селектору
     
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
     
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -571,15 +573,15 @@
     lResult=False
     if len(lWaitAppearList)>0:
         lResult=True
     return lResult
 
 #old name - -
 def UIOSelectorSecs_WaitDisappear_Bool (inSpecificationList,inWaitSecs,inFlagRaiseException=True):
-    '''L-,W+: Ожидать исчезновение 1-го UIO объекта по заданному UIO селектору
+    '''L+,W+: Ожидать исчезновение 1-го UIO объекта по заданному UIO селектору
     
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
     
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -601,86 +603,94 @@
     lResult=False
     if len(lWaitDisappearList)>0:
         lResult=True
     return lResult
 
 #old: -
 def UIOSelector_Get_BitnessInt (inSpecificationList):
-    '''L-,W+: Определить разрядность приложения по UIO селектору. Вернуть результат в формате целого числа (64 или 32)
+    '''L+,W+: Определить разрядность приложения по UIO селектору. Вернуть результат в формате целого числа (64 или 32)
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
         # 1С: UIO Селектор выбора базы
         lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"},{"title":"DEMO", "depth_start": 5, "depth_end": 5}]		
         lDemoBaseBitInt = UIDesktop.UIOSelector_Get_BitnessInt(lDemoBaseUIOSelector) # Определить разрядность приложения, в котором обнаружен UIO объект по селектору
 
     :param inSpecificationList: UIO селектор, который определяет критерии поиска UIO объекта
     :type inSpecificationList: list, обязательный
     :return: None - UIO объект не обнаружен; 64 (int) - разрядность приложения равна 64 битам; 32 (int) - разрядность приложения равна 32 битам
     '''
     #Конвертация селектора в формат UIO
-    inSpecificationList = Selector_Convert_Selector(inSelector=inSpecificationList, inToTypeStr="UIO")
-    lResult=None
-    #Получить объект Application (Для проверки разрядности)
-    lRootElement=PWASpecification_Get_PWAApplication(inSpecificationList)
-    if lRootElement is not None:
-        if lRootElement.is64bit():
-            lResult=64
-        else:
-            lResult=32
-    return lResult
+    if CrossOS.IS_WINDOWS_BOOL==True:
+        inSpecificationList = Selector_Convert_Selector(inSelector=inSpecificationList, inToTypeStr="UIO")
+        lResult=None
+        #Получить объект Application (Для проверки разрядности)
+        lRootElement=PWASpecification_Get_PWAApplication(inSpecificationList)
+        if lRootElement is not None:
+            if lRootElement.is64bit():
+                lResult=64
+            else:
+                lResult=32
+        return lResult
+    else: return 64
+
 
 #old: -
 def UIOSelector_Get_BitnessStr (inSpecificationList):
-    """L-,W+: Определить разрядность приложения по UIO селектору. Вернуть результат в формате строки ("64" или "32")
+    """L+,W+: Определить разрядность приложения по UIO селектору. Вернуть результат в формате строки ("64" или "32")
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
         # 1С: UIO Селектор выбора базы
         lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"},{"title":"DEMO", "depth_start": 5, "depth_end": 5}]		
         lDemoBaseBitStr = UIDesktop.UIOSelector_Get_BitnessStr(lDemoBaseUIOSelector) # Определить разрядность приложения, в котором обнаружен UIO объект по селектору
 
     :param inSpecificationList: UIO селектор, который определяет критерии поиска UIO объекта
     :type inSpecificationList: list, обязательный
     :return: None - UIO объект не обнаружен; "64" (str) - разрядность приложения равна 64 битам; "32" (str) - разрядность приложения равна 32 битам
     """
-    #Конвертация селектора в формат UIO
-    inSpecificationList = Selector_Convert_Selector(inSelector=inSpecificationList, inToTypeStr="UIO")
-    lResult=None
-    #Получить объект Application (Для проверки разрядности)
-    lRootElement=PWASpecification_Get_PWAApplication(inSpecificationList)
-    if lRootElement is not None:
-        if lRootElement.is64bit():
-            lResult="64"
-        else:
-            lResult="32"
-    return lResult
+    if CrossOS.IS_WINDOWS_BOOL==True:
+        #Конвертация селектора в формат UIO
+        inSpecificationList = Selector_Convert_Selector(inSelector=inSpecificationList, inToTypeStr="UIO")
+        lResult=None
+        #Получить объект Application (Для проверки разрядности)
+        lRootElement=PWASpecification_Get_PWAApplication(inSpecificationList)
+        if lRootElement is not None:
+            if lRootElement.is64bit():
+                lResult="64"
+            else:
+                lResult="32"
+        return lResult
+    else:
+        return "64"
 
 #old: -
 def Get_OSBitnessInt ():
-    '''L-,W+: Определить разрядность робота, в котором запускается данная функция
+    '''L+,W+: Определить разрядность робота, в котором запускается данная функция
 
     .. code-block:: python
 
         from pyOpenRPA.Robot import UIDesktop
         lRobotBitInt = UIDesktop.Get_OSBitnessInt() # Определить разрядность робота, в котором была вызвана это функция
     
     :return: 64 (int) - разрядность приложения равна 64 битам; 32 (int) - разрядность приложения равна 32 битам
     '''
-    lResult=32
-    if pywinauto.sysinfo.is_x64_OS():
-        lResult=64
-    return lResult
+    if CrossOS.IS_WINDOWS_BOOL==True:
+        lResult=32
+        if pywinauto.sysinfo.is_x64_OS():
+            lResult=64
+        return lResult
+    else: return 64
 #old: -
 def UIOSelector_SafeOtherGet_Process(inUIOSelector):
-    """L-,W+: Получить процесс робота другой разрядности (если приложение UIO объекта выполняется в другой разрядности). Функция возвращает None, если разрядность робота совпадает с разрядностью приложения UIO объекта, либо если при инициализации робота не устанавливался интерпретатор другой разрядности.
+    """L+,W+: Получить процесс робота другой разрядности (если приложение UIO объекта выполняется в другой разрядности). Функция возвращает None, если разрядность робота совпадает с разрядностью приложения UIO объекта, либо если при инициализации робота не устанавливался интерпретатор другой разрядности.
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
         # 1С: UIO Селектор выбора базы
         lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"},{"title":"DEMO", "depth_start": 5, "depth_end": 5}]		
@@ -848,79 +858,112 @@
             except Exception as e:
                 lRPAApplication = None
         if lRPAApplication is not None:
             #lTempObject=lRPAApplication.window(**inControlSpecificationArray[0])
             #Скорректировано из-за недопонимания структуры
             lTempObject=lRPAApplication
     return lTempObject
+
+from . import Keyboard,Mouse
+
+SEARCH_CHILD_BY_MOUSE_POINT_X = None
+SEARCH_CHILD_BY_MOUSE_POINT_Y = None
+SEARCH_CHILD_BY_MOUSE_ACTIVE = False
+def __SEARCH_CHILD_BY_MOUSE_POINT_X_Y_LISTEN():
+    global SEARCH_CHILD_BY_MOUSE_POINT_X, SEARCH_CHILD_BY_MOUSE_ACTIVE, SEARCH_CHILD_BY_MOUSE_POINT_Y
+    SEARCH_CHILD_BY_MOUSE_ACTIVE = True
+    while SEARCH_CHILD_BY_MOUSE_ACTIVE == True:
+        lSavePositionBool=Keyboard.IsDown("ctrl") or Keyboard.IsDown("ctrl r")
+        #Получить координаты мыши
+        if lSavePositionBool == True and SEARCH_CHILD_BY_MOUSE_POINT_X is None: # ЗАПОМНИТЬ КООРДИНАТЫ ТАК КАК НАЖАТА SHIFT ИЛИ ALT L
+            lMousePoint = Mouse.GetXY()
+            (SEARCH_CHILD_BY_MOUSE_POINT_X,SEARCH_CHILD_BY_MOUSE_POINT_Y) = (lMousePoint.x, lMousePoint.y)
+        elif lSavePositionBool==False: (SEARCH_CHILD_BY_MOUSE_POINT_X,SEARCH_CHILD_BY_MOUSE_POINT_Y)  = (None,None)
+        time.sleep(0.3)
+import threading
 #old: AutomationSearchMouseElement
 def UIOSelector_SearchChildByMouse_UIO(inElementSpecification):
-    """L-,W+: Инициировать визуальный поиск UIO объекта с помощью указателя мыши. При наведении указателя мыши UIO объект выделяется зеленой рамкой. Остановить режим поиска можно с помощью зажима клавиши ctrl left на протяжении нескольких секунд. После этого в веб окне студии будет отображено дерево расположения искомого UIO объекта.
+    """L+,W+: Инициировать визуальный поиск UIO объекта с помощью указателя мыши. При наведении указателя мыши UIO объект выделяется зеленой рамкой. Остановить режим поиска можно с помощью зажима клавиши ctrl left на протяжении нескольких секунд. После этого в веб окне студии будет отображено дерево расположения искомого UIO объекта.
 
+    !ВНИМАНИЕ! НАЧИНАЯ С ВЕРСИИ 1.4.1 ПОМЕНЯЛСЯ ВЫВОД ФУНКЦИИ С [{index, element}, {index, element}, {index, element}] на [ [{index, element}, {index, element}, {index, element}], [{index, element}, {index, element}, {index, element}]]. Данная мера позволила добавить функциональность по поиску множества Ui объектов по курсору мыши 
+    
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
         # 1С: UIO Селектор выбора базы
         lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
         lUIO = UIDesktop.UIOSelector_SearchChildByMouse_UIO(lDemoBaseUIOSelector) # Инициировать поиск дочернего UIO объекта, который расположен внутри lDemoBaseUIOSelector.
 
     :param inElementSpecification: UIO селектор, который определяет критерии поиска родительского UIO объекта, в котором будет производиться поиск дочернего UIO объекта
     :type inElementSpecification: list, обязательный
     :return: UIO объект или None (если UIO не был обнаружен)
     """
+    global SEARCH_CHILD_BY_MOUSE_POINT_X, SEARCH_CHILD_BY_MOUSE_ACTIVE, SEARCH_CHILD_BY_MOUSE_POINT_Y
     #Конвертация селектора в формат UIO
     inElementSpecification = Selector_Convert_Selector(inSelector=inElementSpecification, inToTypeStr="UIO")
     lGUISearchElementSelected=None
     #Настройка - частота обновления подсвечивания
     lTimeSleepSeconds=0.3
     lElementFoundedList=[]
     #Ветка поиска в режиме реального времени
     #Сбросить нажатие Ctrl, если оно было
-    win32api.GetAsyncKeyState(16)
-    win32api.GetAsyncKeyState(17)
-    win32api.GetAsyncKeyState(18)
+    if CrossOS.IS_WINDOWS_BOOL:
+        win32api.GetAsyncKeyState(16)
+        win32api.GetAsyncKeyState(17)
+        win32api.GetAsyncKeyState(18)
     #Оптимизация - получить объект для опроса единажды
     lUIORoot=UIOSelector_Get_UIO(inElementSpecification)
     lFlagLoop = True
-    (lX,lY) = win32api.GetCursorPos()
+    LISTEN_THREAD = threading.Thread(target=__SEARCH_CHILD_BY_MOUSE_POINT_X_Y_LISTEN)
+    LISTEN_THREAD.start()
     while lFlagLoop:
         #Проверить, нажата ли клавиша Ctrl (код 17)
-        lFlagKeyPressedCtrl=bool(win32api.GetAsyncKeyState(17))
-        lAltBool=bool(win32api.GetAsyncKeyState(18)) or bool(win32api.GetAsyncKeyState(16))
-        #Подсветить объект, если мышка наведена над тем объектом, который не подсвечивался в прошлый раз
-        if not lFlagKeyPressedCtrl:
-            #Получить координаты мыши
-            if lAltBool == False: # СВЕТИТЬ, НО НЕ ВЫБИРАТЬ
-                (lX,lY) = win32api.GetCursorPos()
-            lElementFounded={}
-            #Создать карту пикселей и элементов
-            #####Внимание! Функция UIOXY_SearchChild_ListDict не написана
-            lElementFoundedList=UIOXY_SearchChild_ListDict(lUIORoot,lX,lY)
-            lElementFounded=lElementFoundedList[-1]["element"]
-            #Подсветить объект, если он мышь раньше стояла на другом объекте
-            if lGUISearchElementSelected != lElementFounded:
-                lGUISearchElementSelected = lElementFounded
-            #Доработанная функция отрисовки
-            if lElementFounded is not None:
-                UIO_Highlight(lElementFounded)
+        lFlagKeyPressedExit=None
+        #Получить координаты мыши
+        (lX,lY) = (None, None)
+        if SEARCH_CHILD_BY_MOUSE_POINT_X is None: # СВЕТИТЬ, НО НЕ ВЫБИРАТЬ
+            lMousePoint = Mouse.GetXY()
+            (lX,lY) = (lMousePoint.x, lMousePoint.y)
         else:
+            (lX,lY) = (SEARCH_CHILD_BY_MOUSE_POINT_X,SEARCH_CHILD_BY_MOUSE_POINT_Y)
+        lElementFounded=None
+        #Создать карту пикселей и элементов
+        #####Внимание! Функция UIOXY_SearchChild_ListDict не написана
+        inFlagSearchAll = Keyboard.IsDown("alt r") or Keyboard.IsDown("alt l") 
+        lElementFoundedList=UIOXY_SearchChild_ListDict(lUIORoot,lX,lY, inFlagSearchAll=inFlagSearchAll)
+        lElementFounded=set()
+        for item in lElementFoundedList:
+            lElementFounded.add(item[-1]["element"])
+        #Подсветить объект, если он мышь раньше стояла на другом объекте
+        if lGUISearchElementSelected != lElementFounded:
+            lGUISearchElementSelected = lElementFounded
+        else: time.sleep(1)
+        #Доработанная функция отрисовки
+        if lElementFounded is not None:
+            for item in lElementFounded:
+                UIO_Highlight(item, inHighlightCountInt=1)
+        FlagKeyPressedExit=Keyboard.IsDown("shift") or Keyboard.IsDown("shift r") or Keyboard.IsDown("shift l")
+        #Подсветить объект, если мышка наведена над тем объектом, который не подсвечивался в прошлый раз
+        if FlagKeyPressedExit:
             #Была нажата клавиша Ctrl - выйти из цикла
             lFlagLoop=False
-        #Заснуть до следующего цикла
-        time.sleep(lTimeSleepSeconds)
+        else:
+            #Заснуть до следующего цикла
+            time.sleep(lTimeSleepSeconds)
+    SEARCH_CHILD_BY_MOUSE_ACTIVE = False
+    LISTEN_THREAD.join()
     #Вернуть результат поиска
     return lElementFoundedList
 
 #old: - AutomationSearchMouseElementHierarchy
 def UIOSelector_SearchChildByMouse_UIOTree(inUIOSelector, inWaitBeforeSec=0.0):
-    """L-,W+: Получить список уровней UIO объекта с указнием всех имеющихся атрибутов по входящему UIO селектору.
+    """L+,W+: Получить список уровней UIO объекта с указнием всех имеющихся атрибутов по входящему UIO селектору.
 
     ОБНОВЛЕНИЕ 1.4.0: Функция обновлена под использование в новой версии студии
-    
     ОБНОВЛЕНИЕ 1.4.0: ПОСЛЕ ОТРАБОТКИ ВОЗВРАЩАЕТ ФОКУС НА ТО ОКНО, КОТОРОЕ БЫЛО ПРИ ИНИЦИАЛИЗАЦИИ ФУНКЦИИ
 
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
@@ -929,70 +972,79 @@
         lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
         lBackendStr = UIDesktop.UIOSelector_SearchChildByMouse_UIOTree(lDemoBaseUIOSelector) # Получить список атрибутов всех родительских элементов lDemoBaseUIOSelector.
 
     :param inUIOSelector: UIO селектор, который определяет UIO объект, для которого будет произведено извлечение всех атрибутов на всех уровнях.
     :type inUIOSelector: list, обязательный
     :param inWaitBeforeSec: Время ожидания перед началом поиска и перефокусировки. Данный аргумент может быть полезен для отображения полезной информации перед инициализацией режима поиска
     :type inWaitBeforeSec: float, необязательный
+    :param inFlagSearchAll: True - Поиск всех подходящих UI объектов нижних уровней. False - Только до первого подходящего. По умолчанию False
+    :type inFlagSearchAll: bool, необязательный
     :return: list, список атрибутов на каждом уровне UIO объекта
     """
     time.sleep(inWaitBeforeSec)
     #Конвертация селектора в формат UIO
     inUIOSelector = Selector_Convert_Selector(inSelector=inUIOSelector, inToTypeStr="UIO")
     lItemInfo = []
     #Check the bitness
     lSafeOtherProcess = UIOSelector_SafeOtherGet_Process(inUIOSelector)
     if lSafeOtherProcess is None:
         #Получить UI объект, на котором сейчас установлен фокус
         lUIOInitFocused = GetFocused_UIO()
         # Установить фокус по родительскому элементу
         UIOSelector_FocusHighlight(inUIOSelector)
         #Запустить функцию поиска элемента по мыши
-        lElementList = UIOSelector_SearchChildByMouse_UIO(inUIOSelector)
-        lElement = lElementList[-1]['element']
-        #Detect backend of the elements
-        lFlagIsBackendWin32 = True
-        #Если объект имеется (не None), то выполнить построение иерархии
-        if lElement is not None:
-            if lElement.backend.name == 'uia':
-                lFlagIsBackendWin32 = False
-            #Циклическое создание дерева
-            #while lElement is not None:
-            lListIterator=0
-            lItemInfo2=lItemInfo
-            index = 0
-            length = len(lElementList)
-            for lListItem in lElementList:
-                lElement = lListItem["element"]
-                #Продолжать построение иерархии во всех случаях кроме бэк uia & parent() is None
-                #if not lFlagIsBackendWin32 and lElement.parent() is None:
-                #    lElement = None
-                #else:
-                #Получить информацию про объект
-                lItemInfo2.append(UIOEI_Convert_UIOInfo(lElement.element_info))
-                if index==length-1: lItemInfo2[-1]["is_selected_bool"]=True
-                #Дообогатить информацией об индексе ребенка в родительском объекте
-                if "index" in lListItem:
-                    if lListItem["index"] is not None:
-                        lItemInfo2[-1]['ctrl_index']=lListItem["index"]
+        lElementListList = UIOSelector_SearchChildByMouse_UIO(inUIOSelector)
+        for lElementList in lElementListList: # 2023 06 НОВАЯ ФУНКЦИОНАЛЬНО ПО ОТОБРАЖЕНИЮ НЕСКОЛЬКИХ ВЕТОК UI
+            lElement = lElementList[-1]['element']
+            #Detect backend of the elements
+            lFlagIsBackendWin32 = True
+            #Если объект имеется (не None), то выполнить построение иерархии
+            if lElement is not None:
+                if CrossOS.IS_WINDOWS_BOOL and lElement.backend.name == 'uia':
+                    lFlagIsBackendWin32 = False
+                #Циклическое создание дерева
+                #while lElement is not None:
+                lListIterator=0
+                lItemInfo2=lItemInfo
+                index = 0
+                length = len(lElementList)
+                for lListItem in lElementList:
+                    lElement = lListItem["element"]
+                    #Продолжать построение иерархии во всех случаях кроме бэк uia & parent() is None
+                    #if not lFlagIsBackendWin32 and lElement.parent() is None:
+                    #    lElement = None
+                    #else:
+                    #Получить информацию про объект
+                    if CrossOS.IS_WINDOWS_BOOL:
+                        lItemInfo2.append(UIOEI_Convert_UIOInfo(lElement.element_info))
+                        if index==length-1: lItemInfo2[-1]["is_selected_bool"]=True
+                        #Дообогатить информацией об индексе ребенка в родительском объекте
+                        if "index" in lListItem:
+                            if lListItem["index"] is not None:
+                                lItemInfo2[-1]['ctrl_index']=lListItem["index"]
+                            else:
+                                if "ctrl_index" in lListItem:
+                                    lItemInfo2[-1]['ctrl_index']=lListItem["ctrl_index"]
+                        else:
+                            if "ctrl_index" in lListItem:
+                                lItemInfo2[-1]['ctrl_index']=lListItem["ctrl_index"]
                     else:
-                        if "ctrl_index" in lListItem:
-                            lItemInfo2[-1]['ctrl_index']=lListItem["ctrl_index"]
-                else:
-                    if "ctrl_index" in lListItem:
-                        lItemInfo2[-1]['ctrl_index']=lListItem["ctrl_index"]
-                #Оборачиваем потомка в массив, потому что у родителя по структуре интерфейса может быть больше одного наследников
-                lItemInfo2[-1]['child_list']=[]
-                lItemInfo2=lItemInfo2[-1]['child_list']
-                #Переход на родительский объект
-                #lElement = lElement.parent()
-                lListIterator=lListIterator+1
-                index+=1
-            #Добавить информацию о Backend в первый объект
-            lItemInfo[0]["backend"]=lElement.backend.name
+                        info = LCompatibility.get_attr_dict(lElement)
+                        info["ctrl_index"]=lListItem["index"]
+                        lItemInfo2.append(info)
+                    #Оборачиваем потомка в массив, потому что у родителя по структуре интерфейса может быть больше одного наследников
+                    lItemInfo2[-1]['child_list']=[]
+                    lItemInfo2=lItemInfo2[-1]['child_list']
+                    #Переход на родительский объект
+                    #lElement = lElement.parent()
+                    lListIterator=lListIterator+1
+                    index+=1
+                #Добавить информацию о Backend в первый объект
+                if CrossOS.IS_WINDOWS_BOOL:
+                    lItemInfo[0]["backend"]=lElement.backend.name
         #Вернуть фокус исходному окну по итогу отработки
         if lUIOInitFocused!=None: 
             try:
                 lUIOInitFocused.set_focus()
             except Exception as e:
                 pass
     else:
@@ -1238,15 +1290,15 @@
     except RuntimeError:#Обработка истечения таймаута
         return lResultList
     except Exception as e:#Общая обработка исключений
         if inFlagRaiseException: raise e
         else: return []
 
 def UIO_GetValue_Str(inUIO):
-    """Получить значение UI объекта по методу get_value. Если нет такого метода или ошибка выполнения - вернуть None
+    """L-,W+: Получить значение UI объекта по методу get_value. Если нет такого метода или ошибка выполнения - вернуть None
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
         lFilterStr = "1С*"
         lFilterType = "WC"
@@ -1481,15 +1533,15 @@
             lIndexInt+=1
     # ДЛЯ КАЖДОГО ЭЛЕМЕНТА ФОРМИРУЕМ СЕЛЕКТОР
     #Вернуть результат
     return lResultList
 
 #old: - PywinautoExtElementsGetInfo
 def UIOSelector_Get_UIOInfoList (inUIOSelector, inElement=None, inFlagRaiseException=True):
-    """L-,W+: Техническая функция: Получить список параметров последних уровней UIO селектора по UIO объектам, которые удовлетворяют входящим inUIOSelector, поиск по которым будет производится от уровня inElement.
+    """L+,W+: Техническая функция: Получить список параметров последних уровней UIO селектора по UIO объектам, которые удовлетворяют входящим inUIOSelector, поиск по которым будет производится от уровня inElement.
 
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -1564,15 +1616,15 @@
         lRPAApplication.top_window().restore()
     except Exception:
         True==False
     return lResult
 
 #old: - ElementActionGetList
 def UIOSelector_Get_UIOActivityList (inUIOSelector,inFlagRaiseException=True):
-    """L-,W+: Получить список доступных действий/функций по UIO селектору inUIOSelector. Описание возможных активностей см. ниже.
+    """L+,W+: Получить список доступных действий/функций по UIO селектору inUIOSelector. Описание возможных активностей см. ниже.
 
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -1622,25 +1674,30 @@
         lResult=dir(lObject)
         #Выполнить чистку списка от неактуальных методов
         for lActionItem in lActionList:
             #Удалить те, которые начинаются на _
             if lActionItem[0]=='_':
                 lResult.remove(lActionItem)
             #Удалить те, которые начинаются с символа верхнего регистра
-            if lActionItem[0].isupper():
+            elif lActionItem[0].isupper():
                 lResult.remove(lActionItem)
             #Удалить те, которые начинаются с iface - extended режим
-            if lActionItem.startswith("iface"):
+            elif lActionItem.startswith("iface"):
                 lResult.remove(lActionItem)
             #Удалить те, которые начинаются с iter - extended режим
-            if lActionItem.startswith("iter"):
+            elif lActionItem.startswith("iter"):
                 lResult.remove(lActionItem)
             # Удалить те, которые в ignore списке
-            if lActionItem in ignore_list:
+            elif lActionItem in ignore_list:
                 lResult.remove(lActionItem)
+            # Удалить те, которые не начинаются с get / set (для AT-SPI LINUX)
+            elif inUIOSelector[0].get("backend", "at-spi")=="at-spi":
+                if lActionItem.startswith("get_") or lActionItem.startswith("set_"): pass
+                else: lResult.remove(lActionItem)
+            
     else:
         # Run function from other process with help of PIPE
         lPIPEResuestDict = {"ModuleName": "UIDesktop", "ActivityName": "UIOSelector_Get_UIOActivityList",
                             "ArgumentList": [inUIOSelector],
                             "ArgumentDict": {}}
         # Отправить запрос в дочерний процесс, который отвечает за работу с Windows окнами
         ProcessCommunicator.ProcessChildSendObject(lSafeOtherProcess, lPIPEResuestDict)
@@ -1651,15 +1708,15 @@
                 f"Exception was occured in child process (message): {lPIPEResponseDict['ErrorMessage']}, (traceback): {lPIPEResponseDict['ErrorTraceback']}")
         else:
             lResult = lPIPEResponseDict["Result"]
     return lResult
 
 
 def UIOSelectorUIOActivity_Get_ArgDict(inUIOSelector, inActionStr):
-    """L-,W+: Сформировать преднастроенный список/словарь аргументов, передаваемый в функцию inActionStr, которая будет вызываться у объекта UIO, полученного по inUIOSelector
+    """L+,W+: Сформировать преднастроенный список/словарь аргументов, передаваемый в функцию inActionStr, которая будет вызываться у объекта UIO, полученного по inUIOSelector
 
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -1699,29 +1756,32 @@
     if inActionStr in lModuleDefList:
         lItemDef = getattr(l_uio,inActionStr)
         if callable(lItemDef): lDef=lItemDef
         else: 
             lResultDict["ArgDict"] = None
             lResultDict["ArgList"] = None
             return lResultDict
-        lDefSignature = inspect.signature(lDef)
-        for lItemKeyStr in lDefSignature.parameters:
-            lItemValue = lDefSignature.parameters[lItemKeyStr]
-            if lItemValue.default is inspect._empty:
-                lResultDict["ArgDict"][lItemKeyStr] = None
-                lResultDict["ArgList"].append(f"{lItemValue.name}{':'+lItemValue.annotation if lItemValue.annotation!=inspect._empty else ''}")
-            else:
-                lResultDict["ArgDict"][lItemKeyStr] = lItemValue.default
-                lResultDict["ArgList"].append(lItemValue.default)
+        try:
+            lDefSignature = inspect.signature(lDef)
+            for lItemKeyStr in lDefSignature.parameters:
+                lItemValue = lDefSignature.parameters[lItemKeyStr]
+                if lItemValue.default is inspect._empty:
+                    lResultDict["ArgDict"][lItemKeyStr] = None
+                    lResultDict["ArgList"].append(f"{lItemValue.name}{':'+lItemValue.annotation if lItemValue.annotation!=inspect._empty else ''}")
+                else:
+                    lResultDict["ArgDict"][lItemKeyStr] = lItemValue.default
+                    lResultDict["ArgList"].append(lItemValue.default)
+        except ValueError:
+            pass
 
     return lResultDict
 
 #old: - ElementRunAction
 def UIOSelectorUIOActivity_Run_Dict(inUIOSelector, inActionName, inFlagRaiseException=True, inArgumentList=None, inkwArgumentObject=None):
-    """L-,W+: Выполнить активность inActionName над UIO объектом, полученным с помощью UIO селектора inUIOSelector. Описание возможных активностей см. ниже.
+    """L+,W+: Выполнить активность inActionName над UIO объектом, полученным с помощью UIO селектора inUIOSelector. Описание возможных активностей см. ниже.
 
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -1788,16 +1848,17 @@
             raise Exception(f"Exception was occured in child process (message): {lPIPEResponseDict['ErrorMessage']}, (traceback): {lPIPEResponseDict['ErrorTraceback']}")
         else:
             lResult = lPIPEResponseDict["Result"]
     return lResult
 
 #old name - ElementGetInfo
 def UIOSelector_Get_UIOInfo(inUIOSelector):
-    """L-,W+: Получить свойства UIO объекта (element_info), по заданному UIO селектору. Ниже представлен перечень возвращаемых свойств.
+    """L+,W+: Получить свойства UIO объекта (element_info), по заданному UIO селектору. Ниже представлен перечень возвращаемых свойств.
 
+    WINDOWS
     Для backend = win32:
     
     - automation_id (int)
     - class_name (str)
     - control_id (int)
     - control_type (str)
     - full_control_type (str)
@@ -1823,14 +1884,33 @@
     - parent (object/UIO)
     - process_id (int)
     - rectangle (object/rect)
     - rich_text (str)
     - runtime_id (int)
     - visible (bool)
 
+    LINUX:
+    Для backend = at-spi
+
+    "id":
+    "name": 
+    "caption": 
+    "current_value":
+    "description": 
+    "role_name": 
+    "localized_role_name": 
+    "child_count":
+    "toolkit_name":
+    "toolkit_version":
+    "path": 
+    "alpha":
+    "process_id":
+    "rectangle":
+    "attributes":
+
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
         # 1С: UIO Селектор выбора базы
@@ -1977,15 +2057,15 @@
                         lResultHierarchyList = lChildFoundedHierarchyList
                 lChildIterator=lChildIterator+1
     except Exception as e:
         False == False
     return lResultHierarchyList
 
 def UIOSelector_LevelInfo_List(inUIOSelector, inBackend=mDefaultPywinautoBackend):
-    """L-,W+: Получить список свойств всех уровней до UI объекта, обнаруженного с помощью селектора inUIOSelector.
+    """L+,W+: Получить список свойств всех уровней до UI объекта, обнаруженного с помощью селектора inUIOSelector.
     
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -2009,44 +2089,80 @@
         inUIOSelector=UIOSelector_SearchUIONormalize_UIOSelector(inUIOSelector)
         #Выполнить идентификацию объектов, если передан массив
         lResultList=[]
         if len(inUIOSelector) > 0:
             #Получить объект
             lTempObject = UIOSelector_Get_UIO(inUIOSelector)
             def recursive(item, backend):
-                result_list = [UIOEI_Convert_UIOInfo(item.element_info)]
+                result_list = []
+                if CrossOS.IS_WINDOWS_BOOL==True:
+                    result_list =[UIOEI_Convert_UIOInfo(item.element_info)]
+                else: 
+                    result_list = [UIOEI_Convert_UIOInfo(item)]
                 if backend=="uia":
                     # Идентифицировать ctrl_index
-                    parent = item.parent()
+                    parent = None
+                    if CrossOS.IS_WINDOWS_BOOL==True: parent = item.parent()
+                    else: parent=item.parent
                     #while parent == None: parent = item.parent() # Фикс на плавующую ошибку , что иногда не возвращается parent
-                    parent_children_list = parent.children()
+                    parent_children_list = []
+                    if CrossOS.IS_WINDOWS_BOOL==True:
+                        parent_children_list = parent.children()
+                    else:
+                        parent_children_list=list(parent)
                     index = 0
                     for i in parent_children_list:
                         if i==item:
                             result_list[0]["ctrl_index"]=index
                         index+=1
-                    parent_parent = parent.parent()
+                    parent_parent = None
+                    if CrossOS.IS_WINDOWS_BOOL==True: parent_parent = parent.parent()
+                    else: parent_parent=parent.parent
+                    index = 0
                     #while parent_parent == None: parent_parent = parent.parent()
                     if parent_parent != None:
                         result_list=recursive(parent, backend)+result_list
                     else:
                         del result_list[0]["ctrl_index"]
                     return result_list
                 else:
                     # Идентифицировать ctrl_index
-                    parent = item.parent()
-                    #while parent == None: parent = item.parent() # Фикс на плавующую ошибку , что иногда не возвращается parent
-                    if parent != None:
-                        parent_children_list = parent.children()
-                        index = 0
-                        for i in parent_children_list:
-                            if i==item:
-                                result_list[0]["ctrl_index"]=index
-                            index+=1
-                        result_list=recursive(parent, backend)+result_list
+                    try:
+                        parent = None
+                        if CrossOS.IS_WINDOWS_BOOL==True: parent = item.parent()
+                        else: parent=item.parent
+                        #while parent == None: parent = item.parent() # Фикс на плавующую ошибку , что иногда не возвращается parent
+                        if parent != None:
+                            if CrossOS.IS_WINDOWS_BOOL==False:
+                                if (LCompatibility.is_backend_atspi(parent)!=True) or (LCompatibility.is_backend_atspi(parent) and parent.get_name()!="main" and parent.get_role_name()!="desktop frame"):
+                                    parent_children_list = []
+                                    if CrossOS.IS_WINDOWS_BOOL==True:
+                                        parent_children_list = parent.children()
+                                    else:
+                                        parent_children_list=list(parent)
+                                    index = 0
+                                    for i in parent_children_list:
+                                        if i==item:
+                                            result_list[0]["ctrl_index"]=index
+                                        index+=1
+                                    result_list=recursive(parent, backend)+result_list
+                            else:
+                                parent_children_list = []
+                                if CrossOS.IS_WINDOWS_BOOL==True:
+                                    parent_children_list = parent.children()
+                                else:
+                                    parent_children_list=list(parent)
+                                index = 0
+                                for i in parent_children_list:
+                                    if i==item:
+                                        result_list[0]["ctrl_index"]=index
+                                    index+=1
+                                result_list=recursive(parent, backend)+result_list
+                    except Exception as e:
+                        pass
                     return result_list
 
             return recursive(lTempObject, inBackend)
         else:
             lResultList=BackendStr_GetTopLevelList_UIOInfo(inBackend)
             #Установка бэк-енда на первый элемент
             for lItem in lResultList:
@@ -2066,15 +2182,15 @@
         else:
             lResultList = lPIPEResponseDict["Result"]
     return lResultList
 
 
 #old: - ElementGetChildElementList
 def UIOSelector_GetChildList_UIOList(inUIOSelector=None, inBackend=mDefaultPywinautoBackend):
-    """L-,W+: Получить список дочерних UIO объектов по входящему UIO селектору inUIOSelector.
+    """L+,W+: Получить список дочерних UIO объектов по входящему UIO селектору inUIOSelector.
     
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -2097,19 +2213,27 @@
         inUIOSelector=UIOSelector_SearchUIONormalize_UIOSelector(inUIOSelector)
         #Выполнить идентификацию объектов, если передан массив
         lResultList=[]
         if len(inUIOSelector) > 0:
             #Получить объект
             lTempObject = UIOSelector_Get_UIO(inUIOSelector)
             #Получить список дочерних объектов
-            lTempChildList = lTempObject.children()
+            lTempChildList = []
+            if CrossOS.IS_WINDOWS_BOOL==True:
+                lTempChildList = lTempObject.children()
+            elif LCompatibility.is_backend_atspi(lTempObject): # UI ОБЪЕКТЫ WNCK НЕ ИТЕРИРУЮТСЯ
+                lTempChildList = list(lTempObject)
             lIterator=0
             #Подготовить результирующий объект
             for lChild in lTempChildList:
-                lTempObjectInfo=lChild.element_info
+                lTempObjectInfo={}
+                if CrossOS.IS_WINDOWS_BOOL==True:
+                    lTempObjectInfo=lChild.element_info
+                else:
+                    lTempObjectInfo=lChild
                 #Добавить информацию об обнаруженом объекте
                 lObjectInfoItem=UIOEI_Convert_UIOInfo(lTempObjectInfo)
                 #Итератор внутри объекта (для точной идентификации)
                 lObjectInfoItem['ctrl_index']=lIterator
                 lResultList.append(lObjectInfoItem)
                 #Инкремент счетчика
                 lIterator=lIterator+1
@@ -2133,15 +2257,15 @@
         else:
             lResultList = lPIPEResponseDict["Result"]
     return lResultList
 
 #old1: - ElementSpecificationArraySearchPrepare
 #old2: - ElementSpecificationListNormalize
 def UIOSelector_SearchUIONormalize_UIOSelector (inControlSpecificationArray):
-    """L-,W+: Нормализовать UIO селектор для дальнейшего использования в функциях поиск UIO объекта. Если недопустимых атрибутов не присутствует, то оставить как есть.
+    """L+,W+: Нормализовать UIO селектор для дальнейшего использования в функциях поиск UIO объекта. Если недопустимых атрибутов не присутствует, то оставить как есть.
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
         # 1С: UIO Селектор выбора базы
         lDemoBaseUIOSelectorDitry = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
@@ -2149,81 +2273,84 @@
 
     :param inControlSpecificationArray: UIO селектор, который определяет UIO объект, для которого будет представлен перечень доступных активностей.
     :type inControlSpecificationArray: list, обязательный
     :return: нормализованный UIO селектор
     """
     #Конвертация селектора в формат UIO
     inControlSpecificationArray = Selector_Convert_Selector(inSelector=inControlSpecificationArray, inToTypeStr="UIO")
-    lResult=[]
-    #Циклический обход
-    for lSpecificationItem in inControlSpecificationArray:
-        lSpecificationItemNew=lSpecificationItem.copy()
-        #Перебор всех элементов
-        for lItemKey,lItemValue in lSpecificationItem.items():
-            #Флаг удаления атрибута
-            lFlagRemoveAttribute=False
-            #############################
-            #Если является вложенным словарем - удалить
-            if type(lItemValue) is dict:
-                lFlagRemoveAttribute=True
-            #Является типом None
-            if lItemValue is None:
-                lFlagRemoveAttribute=True
-            #Проверка допустимого ключевого слова
-            if (
-                lItemKey == "class_name" or
-                lItemKey == "class_name_re" or
-                lItemKey == "parent" or
-                lItemKey == "process" or
-                lItemKey == "title" or
-                lItemKey == "title_re" or
-                lItemKey == "top_level_only" or
-                lItemKey == "visible_only" or
-                lItemKey == "enabled_only" or
-                lItemKey == "best_match" or
-                lItemKey == "handle" or
-                lItemKey == "ctrl_index" or
-                lItemKey == "found_index" or
-                lItemKey == "predicate_func" or
-                lItemKey == "active_only" or
-                lItemKey == "control_id" or
-                lItemKey == "control_type" or
-                lItemKey == "auto_id" or
-                lItemKey == "framework_id" or
-                lItemKey == "backend"):
-                pass
-            else:
-                lFlagRemoveAttribute=True
+    if CrossOS.IS_WINDOWS_BOOL==True:
+        lResult=[]
+        #Циклический обход
+        for lSpecificationItem in inControlSpecificationArray:
+            lSpecificationItemNew=lSpecificationItem.copy()
+            #Перебор всех элементов
+            for lItemKey,lItemValue in lSpecificationItem.items():
+                #Флаг удаления атрибута
+                lFlagRemoveAttribute=False
+                #############################
+                #Если является вложенным словарем - удалить
+                if type(lItemValue) is dict:
+                    lFlagRemoveAttribute=True
+                #Является типом None
+                if lItemValue is None:
+                    lFlagRemoveAttribute=True
+                #Проверка допустимого ключевого слова
+                if (
+                    lItemKey == "class_name" or
+                    lItemKey == "class_name_re" or
+                    lItemKey == "parent" or
+                    lItemKey == "process" or
+                    lItemKey == "title" or
+                    lItemKey == "title_re" or
+                    lItemKey == "top_level_only" or
+                    lItemKey == "visible_only" or
+                    lItemKey == "enabled_only" or
+                    lItemKey == "best_match" or
+                    lItemKey == "handle" or
+                    lItemKey == "ctrl_index" or
+                    lItemKey == "found_index" or
+                    lItemKey == "predicate_func" or
+                    lItemKey == "active_only" or
+                    lItemKey == "control_id" or
+                    lItemKey == "control_type" or
+                    lItemKey == "auto_id" or
+                    lItemKey == "framework_id" or
+                    lItemKey == "backend"):
+                    pass
+                else:
+                    lFlagRemoveAttribute=True
 
-                
-            #############################
-            #Конструкция по удалению ключа из словаря
-            if lFlagRemoveAttribute:
-                lSpecificationItemNew.pop(lItemKey)
-        #Проверит наличие ctrl_index - если он есть, то удалить control_id и control_type из-за того, что они мешают друг другу
-        if 'ctrl_index' in lSpecificationItemNew:
-            if "control_id" in lSpecificationItemNew:
-                lSpecificationItemNew.pop("control_id")
-            if "control_type" in lSpecificationItemNew:
-                lSpecificationItemNew.pop("control_type")
-        #Проверить наличие handle - если он есть, то удалить process, control_id и control_type из-за того, что они мешают друг другу
-        if 'handle' in lSpecificationItemNew:
-            if "control_id" in lSpecificationItemNew:
-                lSpecificationItemNew.pop("control_id")
-            if "control_type" in lSpecificationItemNew:
-                lSpecificationItemNew.pop("control_type")
-            if "process" in lSpecificationItemNew:
+                    
+                #############################
+                #Конструкция по удалению ключа из словаря
+                if lFlagRemoveAttribute:
+                    lSpecificationItemNew.pop(lItemKey)
+            #Проверит наличие ctrl_index - если он есть, то удалить control_id и control_type из-за того, что они мешают друг другу
+            if 'ctrl_index' in lSpecificationItemNew:
+                if "control_id" in lSpecificationItemNew:
+                    lSpecificationItemNew.pop("control_id")
+                if "control_type" in lSpecificationItemNew:
+                    lSpecificationItemNew.pop("control_type")
+            #Проверить наличие handle - если он есть, то удалить process, control_id и control_type из-за того, что они мешают друг другу
+            if 'handle' in lSpecificationItemNew:
+                if "control_id" in lSpecificationItemNew:
+                    lSpecificationItemNew.pop("control_id")
+                if "control_type" in lSpecificationItemNew:
+                    lSpecificationItemNew.pop("control_type")
+                if "process" in lSpecificationItemNew:
+                    lSpecificationItemNew.pop("process")
+            #Иначе Проверить наличие process - если он есть, то удалить тк он нужен только при подключении к процессу
+            if 'process' in lSpecificationItemNew:
                 lSpecificationItemNew.pop("process")
-        #Иначе Проверить наличие process - если он есть, то удалить тк он нужен только при подключении к процессу
-        if 'process' in lSpecificationItemNew:
-            lSpecificationItemNew.pop("process")
-        #Добавить строку в результирующий массив
-        lResult.append(lSpecificationItemNew)
-    #Вернуть результат
-    return lResult
+            #Добавить строку в результирующий массив
+            lResult.append(lSpecificationItemNew)
+        #Вернуть результат
+        return lResult
+    else:
+        return inControlSpecificationArray
 
 #old name 1 - ElementSpecificationArraySearchPrepare
 #old name 2 - ElementSpecificationListNormalize
 def UIOSelector_SearchProcessNormalize_UIOSelector (inControlSpecificationArray):
     """L-,W+: Нормализовать UIO селектор для дальнейшего использования в функциях поиска процесса, в котором находится искомый UIO объект. Если недопустимых атрибутов не присутствует, то оставить как есть.
 
     .. code-block:: python
@@ -2395,15 +2522,15 @@
     except Exception as e:
         True == False
     #Вернуть результат
     return lResult
 
 #old: - GetRootElementList
 def BackendStr_GetTopLevelList_UIOInfo(inBackend=mDefaultPywinautoBackend):
-    """L-,W+: Получить список UIOInfo словарей - процессы, которые запущены в рабочей сессии и готовы для взаимодействия с роботом через backend inBackend
+    """L+,W+: Получить список UIOInfo словарей - процессы, которые запущены в рабочей сессии и готовы для взаимодействия с роботом через backend inBackend
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
         lAppList = UIDesktop.BackendStr_GetTopLevelList_UIOInfo() # Очистить UIO селектор от недопустимых ключей для дальнейшего использования
 
@@ -2417,15 +2544,15 @@
     for lI in lResultList:
         lTempObjectInfo=lI
         lResultList2.append(UIOEI_Convert_UIOInfo(lI))
     return lResultList2
 
 #old: - ElementDrawOutlineNew
 def UIOSelector_Highlight(inUIOSelector):
-    """L-,W+: Подсветить на несколько секунд на экране зеленой рамкой UIO объект, который соответствует входящему UIO селектору inUIOSelector
+    """L+,W+: Подсветить на несколько секунд на экране зеленой рамкой UIO объект, который соответствует входящему UIO селектору inUIOSelector
 
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -2455,15 +2582,15 @@
             raise Exception(
                 f"Exception was occured in child process (message): {lPIPEResponseDict['ErrorMessage']}, (traceback): {lPIPEResponseDict['ErrorTraceback']}")
         else:
             return lPIPEResponseDict["Result"]
     return True
 #old: - ElementDrawOutlineNewFocus
 def UIOSelector_FocusHighlight(inUIOSelector):
-    """L-,W+: Установить фокус и подсветить на несколько секунд на экране зеленой рамкой UIO объект, который соответствует входящему UIO селектору inUIOSelector
+    """L+,W+: Установить фокус и подсветить на несколько секунд на экране зеленой рамкой UIO объект, который соответствует входящему UIO селектору inUIOSelector
 
     !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
@@ -2492,17 +2619,134 @@
         if lPIPEResponseDict["ErrorFlag"]:
             raise Exception(
                 f"Exception was occured in child process (message): {lPIPEResponseDict['ErrorMessage']}, (traceback): {lPIPEResponseDict['ErrorTraceback']}")
         else:
             return lPIPEResponseDict["Result"]
     return True
 
+
+def UIOSelector_Focus(inUIOSelector):
+    """L+,W+: Установить фокус на приложение, в котором находится UIO объект
+
+    !ВНИМАНИЕ! ДАННАЯ ФУНКЦИОНАЛЬНОСТЬ В АВТОМАТИЧЕСКОМ РЕЖИМЕ ПОДДЕРЖИВАЕТ ВСЕ РАЗРЯДНОСТИ ПРИЛОЖЕНИЙ (32|64), КОТОРЫЕ ЗАПУЩЕНЫ В СЕСИИ. PYTHON x64 ИМЕЕТ ВОЗМОЖНОСТЬ ВЗЗАИМОДЕЙСТВИЯ С x32 UIO ОБЪЕКТАМИ, НО МЫ РЕКОМЕНДУЕМ ДОПОЛНИТЕЛЬНО ИСПОЛЬЗОВАТЬ ИНТЕРПРЕТАТОР PYTHON x32 (ПОДРОБНЕЕ СМ. ФУНКЦИЮ Configure())
+
+    .. code-block:: python
+
+        # UIDesktop: Взаимодействие с UI объектами приложений
+        from pyOpenRPA.Robot import UIDesktop
+        # 1С: UIO Селектор выбора базы
+        lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
+        UIDesktop.UIOSelector_Focus(lDemoBaseUIOSelector) # Установить фокус и подсветить UIO объект по UIO селектору
+
+    :param inUIOSelector: UIO селектор, который определяет UIO объект, для которого будет представлен перечень доступных активностей.
+    :type inUIOSelector: list, обязательный
+    """
+    #Конвертация селектора в формат UIO
+    inUIOSelector = Selector_Convert_Selector(inSelector=inUIOSelector, inToTypeStr="UIO")
+    #Check the bitness
+    lSafeOtherProcess = UIOSelector_SafeOtherGet_Process(inUIOSelector)
+    if lSafeOtherProcess is None:
+        UIO_Focus(UIOSelector_Get_UIO(inUIOSelector))
+    else:
+        # Run function from other process with help of PIPE
+        lPIPEResuestDict = {"ModuleName": "UIDesktop", "ActivityName": "UIOSelector_FocusHighlight",
+                            "ArgumentList": [inUIOSelector],
+                            "ArgumentDict": {}}
+        # Отправить запрос в дочерний процесс, который отвечает за работу с Windows окнами
+        ProcessCommunicator.ProcessChildSendObject(lSafeOtherProcess, lPIPEResuestDict)
+        # Get answer from child process
+        lPIPEResponseDict = ProcessCommunicator.ProcessChildReadWaitObject(lSafeOtherProcess)
+        if lPIPEResponseDict["ErrorFlag"]:
+            raise Exception(
+                f"Exception was occured in child process (message): {lPIPEResponseDict['ErrorMessage']}, (traceback): {lPIPEResponseDict['ErrorTraceback']}")
+        else:
+            return lPIPEResponseDict["Result"]
+    return True
+
+def UIOSelector_Click(inUIOSelector, inRuleStr="CC", inFocusBool = True):
+    """L+,W+: Выполнить клик по UI объекту
+        
+    !ВНИМАНИЕ! Функция использует мышь. Программные способы инициализации события нажатия мыши см. в перечне активностей объекта UIO
+
+    .. code-block:: python
+
+        # UIDesktop: Взаимодействие с UI объектами приложений
+        from pyOpenRPA.Robot import UIDesktop
+        # 1С: UIO Селектор выбора базы
+        lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
+        UIDesktop.UIOSelector_Click(lDemoBaseUIOSelector) # Выполнить клик по UIO объекту
+
+    :param inUIO: UIO объект, который будет подсвечен
+    :type inUIO: object UIO, обязательный
+    :param inRuleStr: Правило идентификации точки на прямоугольной области (правила формирования см. выше). Варианты: "LU","CU","RU","LC","CC","RC","LD","CD","RD".  По умолчанию "CC"
+    :type inRuleStr: str, опциональный
+    :param inFocusBool: True - выполнить фокусировку на объект перед нажатием, False - Не выполнять фокусировку (ускорение производительности робота)
+    :type inFocusBool: bool, опциональный
+    """
+    #Конвертация селектора в формат UIO
+    inUIOSelector = Selector_Convert_Selector(inSelector=inUIOSelector, inToTypeStr="UIO")
+    lUIO = UIOSelector_Get_UIO(inUIOSelector)
+    if inFocusBool: UIO_Focus(lUIO)
+    UIO_Click(lUIO, inRuleStr = inRuleStr)
+
+def UIOSelector_ClickRight(inUIOSelector, inRuleStr="CC", inFocusBool = True):
+    """L+,W+: Выполнить правый клик по UI объекту
+        
+    !ВНИМАНИЕ! Функция использует мышь. Программные способы инициализации события нажатия мыши см. в перечне активностей объекта UIO
+
+    .. code-block:: python
+
+        # UIDesktop: Взаимодействие с UI объектами приложений
+        from pyOpenRPA.Robot import UIDesktop
+        # 1С: UIO Селектор выбора базы
+        lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
+        UIDesktop.UIOSelector_ClickRight(lDemoBaseUIOSelector) # Выполнить правый клик по UIO объекту
+
+    :param inUIO: UIO объект, который будет подсвечен
+    :type inUIO: object UIO, обязательный
+    :param inRuleStr: Правило идентификации точки на прямоугольной области (правила формирования см. выше). Варианты: "LU","CU","RU","LC","CC","RC","LD","CD","RD".  По умолчанию "CC"
+    :type inRuleStr: str, опциональный
+    :param inFocusBool: True - выполнить фокусировку на объект перед нажатием, False - Не выполнять фокусировку (ускорение производительности робота)
+    :type inFocusBool: bool, опциональный
+    """
+    #Конвертация селектора в формат UIO
+    inUIOSelector = Selector_Convert_Selector(inSelector=inUIOSelector, inToTypeStr="UIO")
+    lUIO = UIOSelector_Get_UIO(inUIOSelector)
+    if inFocusBool: UIO_Focus(lUIO)
+    UIO_ClickRight(lUIO, inRuleStr = inRuleStr)
+
+def UIOSelector_ClickDouble(inUIOSelector, inRuleStr="CC", inFocusBool = True):
+    """L+,W+: Выполнить двойной левый клик по UI объекту
+        
+    !ВНИМАНИЕ! Функция использует мышь. Программные способы инициализации события нажатия мыши см. в перечне активностей объекта UIO
+
+    .. code-block:: python
+
+        # UIDesktop: Взаимодействие с UI объектами приложений
+        from pyOpenRPA.Robot import UIDesktop
+        # 1С: UIO Селектор выбора базы
+        lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
+        UIDesktop.UIOSelector_ClickDouble(lDemoBaseUIOSelector) # Выполнить двойной левый клик по UIO объекту
+
+    :param inUIO: UIO объект, который будет подсвечен
+    :type inUIO: object UIO, обязательный
+    :param inRuleStr: Правило идентификации точки на прямоугольной области (правила формирования см. выше). Варианты: "LU","CU","RU","LC","CC","RC","LD","CD","RD".  По умолчанию "CC"
+    :type inRuleStr: str, опциональный
+    :param inFocusBool: True - выполнить фокусировку на объект перед нажатием, False - Не выполнять фокусировку (ускорение производительности робота)
+    :type inFocusBool: bool, опциональный
+    """
+    #Конвертация селектора в формат UIO
+    inUIOSelector = Selector_Convert_Selector(inSelector=inUIOSelector, inToTypeStr="UIO")
+    lUIO = UIOSelector_Get_UIO(inUIOSelector)
+    if inFocusBool: UIO_Focus(lUIO)
+    UIO_ClickDouble(lUIO, inRuleStr = inRuleStr)
+
 #old: - draw_outline_new
-def UIO_Highlight(lWrapperObject,colour='green',thickness=2,fill=None,rect=None,inFlagSetFocus=False):
-    """L-,W+: Выполнить подсветку UIO объекта на экране
+def UIO_Highlight(lWrapperObject,colour='green',thickness=2,fill=None,rect=None,inFlagSetFocus=False, inHighlightCountInt=2):
+    """L+,W+: Выполнить подсветку UIO объекта на экране
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
         # 1С: UIO Селектор выбора базы
         lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
@@ -2566,15 +2810,15 @@
         win32functions.DeleteObject(brush_handle)
         win32functions.DeleteObject(pen_handle)
         # delete the Display context that we created
         win32functions.DeleteDC(dc)
 
 #old: - draw_outline_new_focus
 def UIO_FocusHighlight(lWrapperObject,colour='green',thickness=2,fill=None,rect=None):
-    """L-,W+: Установить фокус и выполнить подсветку UIO объекта на экране
+    """L+,W+: Установить фокус и выполнить подсветку UIO объекта на экране
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
         from pyOpenRPA.Robot import UIDesktop
         # 1С: UIO Селектор выбора базы
         lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
@@ -2587,20 +2831,140 @@
     :type colour: str, необязательный
     :param thickness: толщина подсветки UIO объекта. По умолчанию 2
     :type thickness: int, необязательный
     """
     if fill is None: fill = win32defines.BS_NULL
     UIO_Highlight(lWrapperObject,'green',2,fill,None,True)
 
+def UIO_Focus(lWrapperObject):
+    """L+,W+: Установить фокус UIO объекта на экране
+
+    .. code-block:: python
+
+        # UIDesktop: Взаимодействие с UI объектами приложений
+        from pyOpenRPA.Robot import UIDesktop
+        # 1С: UIO Селектор выбора базы
+        lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
+        lUIO = UIDesktop.UIOSelector_Get_UIO(lDemoBaseUIOSelector) # Получить UIO объект по UIO селектору
+        UIDesktop.UIO_Focus(lUIO) # Установить фокус на UIO объект
+
+    :param lWrapperObject: UIO объект, который будет подсвечен
+    :type lWrapperObject: object UIO, обязательный
+    """
+    if lWrapperObject is not None:
+        #Установить фокус на объект, чтобы было видно выделение
+        lWrapperObject.set_focus()
+        time.sleep(0.5)
+
 #Определить разрядность процесса
 lProcessBitnessStr = str(struct.calcsize("P") * 8)
 Usage.Process(inComponentStr="Robot")
 License.ConsoleVerify()
 
+from . import Screen
+def UIO_GetPoint(inUIO, inRuleStr="CC"):
+    """L+,W+: Получить точку по прямоугольной области UI объекта inUIO с учетом сумвольного указания точки inRuleStr
+        
+    !ВНИМАНИЕ! Функция использует мышь. Программные способы инициализации события нажатия мыши см. в перечне активностей объекта UIO
+
+    .. code-block:: python
+
+        # UIDesktop: Взаимодействие с UI объектами приложений
+        from pyOpenRPA.Robot import UIDesktop
+        # 1С: UIO Селектор выбора базы
+        lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
+        lUIO = UIDesktop.UIOSelector_Get_UIO(lDemoBaseUIOSelector) # Получить UIO объект по UIO селектору
+        UIDesktop.UIO_Click(lUIO) # Выполнить клик по UIO объекту
+
+    :param inUIO: UIO объект, который будет подсвечен
+    :type inUIO: object UIO, обязательный
+    :param inRuleStr: Правило идентификации точки на прямоугольной области (правила формирования см. выше). Варианты: "LU","CU","RU","LC","CC","RC","LD","CD","RD".  По умолчанию "CC"
+    :type inRuleStr: str, опциональный
+    :return: Точка на экране
+    :rtype: Screen.Point
+
+    """
+    lPoint = None
+    if CrossOS.IS_WINDOWS_BOOL: 
+        lBox = Screen.BoxParse(inUIO.element_info.rectangle)
+        lPoint = Screen.PointFromBox(inBox = lBox, inRuleStr = inRuleStr)
+    else:
+        lBox = Screen.BoxParse(LCompatibility.get_rect(inUIO))
+        lPoint = Screen.PointFromBox(inBox = lBox, inRuleStr = inRuleStr)
+    return lPoint
+
+def UIO_Click(inUIO, inRuleStr="CC"):
+    """L+,W+: Выполнить клик по UI объекту
+        
+    !ВНИМАНИЕ! Функция использует мышь. Программные способы инициализации события нажатия мыши см. в перечне активностей объекта UIO
+
+    .. code-block:: python
+
+        # UIDesktop: Взаимодействие с UI объектами приложений
+        from pyOpenRPA.Robot import UIDesktop
+        # 1С: UIO Селектор выбора базы
+        lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
+        lUIO = UIDesktop.UIOSelector_Get_UIO(lDemoBaseUIOSelector) # Получить UIO объект по UIO селектору
+        UIDesktop.UIO_Click(lUIO) # Выполнить клик по UIO объекту
+
+    :param inUIO: UIO объект, который будет подсвечен
+    :type inUIO: object UIO, обязательный
+    :param inRuleStr: Правило идентификации точки на прямоугольной области (правила формирования см. выше). Варианты: "LU","CU","RU","LC","CC","RC","LD","CD","RD".  По умолчанию "CC"
+    :type inRuleStr: str, опциональный
+
+    """
+    lPoint = UIO_GetPoint(inUIO,inRuleStr)
+    Screen.PointClick(lPoint)
+
+def UIO_ClickRight(inUIO, inRuleStr="CC"):
+    """L+,W+: Выполнить правый клик по UI объекту
+        
+    !ВНИМАНИЕ! Функция использует мышь. Программные способы инициализации события нажатия мыши см. в перечне активностей объекта UIO
+
+    .. code-block:: python
+
+        # UIDesktop: Взаимодействие с UI объектами приложений
+        from pyOpenRPA.Robot import UIDesktop
+        # 1С: UIO Селектор выбора базы
+        lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
+        lUIO = UIDesktop.UIOSelector_Get_UIO(lDemoBaseUIOSelector) # Получить UIO объект по UIO селектору
+        UIDesktop.UIO_ClickRight(lUIO) # Выполнить клик по UIO объекту
+
+    :param inUIO: UIO объект, который будет подсвечен
+    :type inUIO: object UIO, обязательный
+    :param inRuleStr: Правило идентификации точки на прямоугольной области (правила формирования см. выше). Варианты: "LU","CU","RU","LC","CC","RC","LD","CD","RD".  По умолчанию "CC"
+    :type inRuleStr: str, опциональный
+
+    """
+    lPoint = UIO_GetPoint(inUIO,inRuleStr)
+    Screen.PointClick(lPoint, inButtonStr="right")
+
+
+def UIO_ClickDouble(inUIO, inRuleStr="CC"):
+    """L+,W+: Выполнить двойной клик по UI объекту
+        
+    !ВНИМАНИЕ! Функция использует мышь. Программные способы инициализации события нажатия мыши см. в перечне активностей объекта UIO
 
+    .. code-block:: python
+
+        # UIDesktop: Взаимодействие с UI объектами приложений
+        from pyOpenRPA.Robot import UIDesktop
+        # 1С: UIO Селектор выбора базы
+        lDemoBaseUIOSelector = [{"title":"Запуск 1С:Предприятия","class_name":"V8TopLevelFrameTaxiStarter","backend":"uia"}]		
+        lUIO = UIDesktop.UIOSelector_Get_UIO(lDemoBaseUIOSelector) # Получить UIO объект по UIO селектору
+        UIDesktop.UIO_ClickDouble(lUIO) # Выполнить клик по UIO объекту
+
+    :param inUIO: UIO объект, который будет подсвечен
+    :type inUIO: object UIO, обязательный
+    :param inRuleStr: Правило идентификации точки на прямоугольной области (правила формирования см. выше). Варианты: "LU","CU","RU","LC","CC","RC","LD","CD","RD".  По умолчанию "CC"
+    :type inRuleStr: str, опциональный
+
+    """
+    lPoint = UIO_GetPoint(inUIO,inRuleStr)
+    Screen.PointClickDouble(lPoint)
 
 def GetFocused_UIO():
     """L-,W+: Получить UIO объект, на котором установлен фокус
 
     .. code-block:: python
 
         # UIDesktop: Взаимодействие с UI объектами приложений
@@ -2880,8 +3244,11 @@
         #Составление итогового CSS селектора
         if lGoUpFlag: raise ValueError("CSS doesn't support the go_up attribute")   
         else: lSelectorTmpStr = lSelectorTmpStr + lDelimiter + lOneLevelAttrStr
         lLevelInt+=1
     lCSSSelector = lSelectorTmpStr[1:]
 
     return lCSSSelector
-
+if CrossOS.IS_WINDOWS_BOOL == False:
+    from .Utils import LCompatibility
+else:
+    from .Utils import WCompatibility
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/UIWeb.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/UIWeb.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import JavascriptException
 import os
 import sys
 import json
 from pyOpenRPA.Tools import CrossOS
 from pyOpenRPA.Robot import UIDesktop
+if CrossOS.IS_WINDOWS_BOOL:
+    import win32api
 import time
 
 # XPATH CSS CHEAT CHEET: https://devhints.io/xpath
 # XPATH CSS CHEAT CHEET: https://devhints.io/css
 
 UIO_WAIT_SEC_FLOAT = 60
 UIO_WAIT_INTERVAL_SEC_FLOAT = 1.0
 
 gBrowser:webdriver.Chrome = None
-def BrowserChromeStart(inDriverExePathStr:str = None, inChromeExePathStr:str = None, inExtensionPathList:list = None, inProfilePathStr:str=None, inSaveAsPDFBool = False, inSavefileDefaultDirStr:str = None, inUrlStr:str = None, inModeStr: str = None, inMaximizeBool:bool = None) -> webdriver.Chrome:
+def BrowserChromeStart(inDriverExePathStr:str = None, inChromeExePathStr:str = None, inExtensionPathList:list = None, inProfilePathStr:str=None, inSaveAsPDFBool = False, inSavefileDefaultDirStr:str = None, inUrlStr:str = None, inModeStr: str = None, inMaximizeBool:bool = None, inDownloadAskBool=False) -> webdriver.Chrome:
     """L+,W+: Выполнить запуск браузера Chrome. Если вы скачали pyOpenRPA вместе с репозиторием, то будет использоваться встроенный браузер Google Chrome. Если установка pyOpenRPA производилась другим способом, то требуется указать расположение браузера Google Chrome и соответствующего WebDriver
 
     .. code-block:: python
 
         # UIWeb: Взаимодействие с ui web
         from pyOpenRPA.Robot import UIWeb
         UIWeb.BrowserChromeStart()
@@ -40,40 +42,48 @@
     :type inSavefileDefaultDirStr: str, опционально
     :param inUrlStr: Путь к странице, которую требуется открыть. По умолчанию адреса нет
     :type inUrlStr: str, опционально
     :param inModeStr: Формат запуска браузера. Доступные варианты: "NORMAL", "APP", "KIOSK". По умолчанию "NORMAL"
     :type inModeStr: str, опционально
     :param inMaximizeBool: True - развернуть на весь экран. False (по умолчанию) - не разворачивать.
     :type inMaximizeBool: bool, опционально
+    :param inDownloadAskBool: True - Спрашивать папку для сохранения перед каждой загрузкой из браузера. False (по умолчанию) - не спрашивать.
+    :type inDownloadAskBool: bool, опционально
     :return: Объект браузера Google Chrome
     :rtype: webdriver.Chrome
     """
     global gBrowser
     inDriverExePathStr = CrossOS.PathStr(inPathStr=inDriverExePathStr)
     inChromeExePathStr = CrossOS.PathStr(inPathStr=inChromeExePathStr)
     lExtensionPathList = []
     if inExtensionPathList is not None:
         for lItemStr in inExtensionPathList:
             lExtensionPathList.append(CrossOS.PathStr(inPathStr=lItemStr))
     inExtensionPathList = lExtensionPathList
     inChromeExePathStr = CrossOS.PathStr(inPathStr=inChromeExePathStr)
     inProfilePathStr = CrossOS.PathStr(inPathStr=inProfilePathStr)
     lResourcePathStr = os.path.abspath(os.path.join(sys.executable, "..","..", ".."))
-    # Путь по умолчанию к портативному браузеру и драйверу (если скачивался репозиторий pyOpenRPA
+    if CrossOS.IS_LINUX_BOOL: 
+        if os.path.exists(os.path.join("..", 'Resources')): lResourcePathStr = os.path.abspath(os.path.join("..", 'Resources'))
+        elif os.path.exists(os.path.join("..", "..", 'Resources')): lResourcePathStr = os.path.abspath(os.path.join("..", "..",'Resources'))
+        elif os.path.exists(os.path.join("..", "..","..", 'Resources')): lResourcePathStr = os.path.abspath(os.path.join("..", "..",".." 'Resources'))
+        elif os.path.exists('Resources'): lResourcePathStr = os.path.abspath('Resources')
+    # Путь по умолчанию к портативному браузеру и драйверу (если скачивался репозиторий pyOpenRPA'
     if inDriverExePathStr == None: 
         if CrossOS.IS_WINDOWS_BOOL: inDriverExePathStr = os.path.join(lResourcePathStr, "SeleniumWebDrivers", "Chrome", "chromedriver_win32 v84.0.4147.30", "chromedriver.exe")
         elif CrossOS.IS_LINUX_BOOL: inDriverExePathStr = os.path.join(lResourcePathStr, "SeleniumWebDrivers", "Chrome", "chromedriver_lin64 v103.0.5060.53", "chromedriver")
     if inChromeExePathStr == None: 
         if CrossOS.IS_WINDOWS_BOOL: inChromeExePathStr = os.path.join(lResourcePathStr, "WChrome64-840414730", "App", "Chrome-bin", "chrome.exe")
         elif CrossOS.IS_LINUX_BOOL: inChromeExePathStr = os.path.join(lResourcePathStr, "LChrome64-10305060114", "data", "chrome")
     if inExtensionPathList == None: inExtensionPathList = []
     if inModeStr==None: inModeStr="NORMAL"
     if inMaximizeBool==None: inMaximizeBool=False
     # Установка настроек окна печати, если необходимо
     lWebDriverChromeOptionsInstance = webdriver.ChromeOptions()
+    lWebDriverChromeOptionsInstance.add_experimental_option("excludeSwitches", ["enable-automation"])
     if inSaveAsPDFBool == True and inSavefileDefaultDirStr is not None:
         print_settings = {
         "recentDestinations": [{
             "id": "Save as PDF",
             "origin": "local",
             "account": "",
         }],
@@ -85,18 +95,22 @@
         prefs = {'printing.print_preview_sticky_settings.appState': json.dumps(print_settings),
                  "download.prompt_for_download": False,
                  "profile.default_content_setting_values.automatic_downloads": 1,
                  "download.default_directory": inSavefileDefaultDirStr,
                  "savefile.default_directory": inSavefileDefaultDirStr,
                  "download.directory_upgrade": True,
                  "safebrowsing.enabled": True}
-        
+        if inDownloadAskBool==True:
+            prefs["download.prompt_for_download"]=True
         lWebDriverChromeOptionsInstance.add_experimental_option('prefs', prefs)
         lWebDriverChromeOptionsInstance.add_argument('--kiosk-printing')
-
+    else:
+        if inDownloadAskBool==True:
+            prefs = {'download.prompt_for_download': True}
+            lWebDriverChromeOptionsInstance.add_experimental_option('prefs', prefs)
     lWebDriverChromeOptionsInstance.add_argument("disable-infobars")
     # Set full path to exe of the chrome
     lWebDriverChromeOptionsInstance.binary_location = inChromeExePathStr
     #lWebDriverChromeOptionsInstance2 = webdriver.ChromeOptions()
     if inProfilePathStr is not None:
         inProfilePathStr = os.path.abspath(inProfilePathStr)
         lWebDriverChromeOptionsInstance.add_argument(f"user-data-dir={os.path.abspath(inProfilePathStr)}")
@@ -108,14 +122,17 @@
         lWebDriverChromeOptionsInstance.add_argument(f'--app={inUrlStr}')
     elif inModeStr.upper()=="KIOSK" and inUrlStr!=None:
         lWebDriverChromeOptionsInstance.add_argument(f'--kiosk {inUrlStr}')
     if inMaximizeBool==True:
         lWebDriverChromeOptionsInstance.add_argument('--start-maximized')
     #if inDriverExePathStr == "built-in":
     # Run with specified web driver path
+    if CrossOS.IS_LINUX_BOOL:
+        lPathStr = CrossOS.PathJoinList(CrossOS.PathSplitList(inDriverExePathStr)[:-1]) 
+        os.environ["PATH"]+=f":{lPathStr}"
     gBrowser = webdriver.Chrome(executable_path = inDriverExePathStr, options=lWebDriverChromeOptionsInstance) 
     #from pyOpenRPA.Robot import Window
     #Window.DialogYesNo(inTitle="TEST", inBody="Далее взяли селектор")
     #else:
     #    lWebDriverInstance = webdriver.Chrome(options = lWebDriverChromeOptionsInstance)
     return gBrowser
 from ..Utils import __define__
@@ -127,33 +144,37 @@
         # UIWeb: Взаимодействие с ui web
         from pyOpenRPA.Robot import UIWeb
         UIWeb.BrowserChromeStart()
         UIWeb.BrowserFocus()
     """
     import psutil
     global gBrowser
-    driver_pid = gBrowser.service.process.pid
-    process = psutil.Process(driver_pid)
-    browser_pid = None
-    for child in process.children(recursive=True):
-        if browser_pid==None: browser_pid = child.pid
-        #print(f"ФОКУС ОКНА: {child.name()}:{child.pid}")
-        #if child.name() == "chrome.exe":
-        #    chrome_pid = child.pid
-        #    break
-    #print(chrome_pid)
-    if browser_pid!=None: 
-        UIBrowserSelector = [
-            {
-                "process": browser_pid,
-                "backend": "win32"
-            }
-        ]
-        UIDesktop.UIOSelector_Get_UIO(UIBrowserSelector).set_focus()
-
+    try:
+        driver_pid = gBrowser.service.process.pid
+        process = psutil.Process(driver_pid)
+        browser_pid = None
+        for child in process.children(recursive=True):
+            if browser_pid==None: browser_pid = child.pid
+            #if child.name() == "chrome.exe":
+            #    chrome_pid = child.pid
+            #    brea
+        if browser_pid!=None: 
+            if CrossOS.IS_WINDOWS_BOOL:
+                UIBrowserSelector = [
+                    {
+                        "process": browser_pid,
+                        "backend": "win32"
+                    }
+                ]
+                UIDesktop.UIOSelector_Get_UIO(UIBrowserSelector).set_focus()
+            else:
+                UIBrowserSelector=[{"pid": browser_pid,"backend": "wnck"}]
+                UIDesktop.UIOSelector_Focus(UIBrowserSelector)
+    except Exception as e:
+        pass
 
 def BrowserChange(inBrowser):
     """L+,W+: Выполнить смену активного браузера (при необходимости).
 
     .. code-block:: python
 
         # UIWeb: Взаимодействие с ui web
@@ -1598,15 +1619,17 @@
             return document.elementFromPoint(document.ORPAMouseXInt,document.ORPAMouseYInt);
         """
     try:
         global gMouseIsInitBool
         gMouseIsInitBool = False
         return PageJSExecute(lJSStr)
     except JavascriptException: raise JavascriptException("Отсутствуют координаты для идентификации веб-элемента. Пожалуйста, в следующий раз двигайте мышью")
-import win32api
+
+from . import Keyboard
+
 def MouseSearchChild():
     """L+,W+: Инициировать визуальный поиск UIO объекта с помощью указателя мыши. При наведении указателя мыши UIO объект выделяется зеленой рамкой. Остановить режим поиска можно с помощью зажима клавиши ctrl left на протяжении нескольких секунд. После этого в веб окне студии будет отображено дерево расположения искомого UIO объекта.
 
     .. code-block:: python
 
         # UIWeb: Взаимодействие с ui web
         from pyOpenRPA.Robot import UIWeb
@@ -1619,26 +1642,22 @@
     :return: UIO объект или None (если UIO не был обнаружен)
     """
     lGUISearchElementSelected=None
     #Настройка - частота обновления подсвечивания
     lTimeSleepSeconds=0.3
     #Ветка поиска в режиме реального времени
     #Сбросить нажатие Ctrl, если оно было
-    win32api.GetAsyncKeyState(16)
-    win32api.GetAsyncKeyState(17)
-    win32api.GetAsyncKeyState(18)
     #Инициализация
     UIOMouseSearchInit()
     lFlagLoop = True
-    (lX,lY) = win32api.GetCursorPos()
     lElementFounded=None
     while lFlagLoop:
         #Проверить, нажата ли клавиша Ctrl (код 17)
-        lFlagKeyPressedCtrl=bool(win32api.GetAsyncKeyState(17))
-        lAltBool=bool(win32api.GetAsyncKeyState(18)) or bool(win32api.GetAsyncKeyState(16))
+        lFlagKeyPressedCtrl=Keyboard.IsDown("shift")
+        lAltBool=Keyboard.IsDown("ctrl")
         #Подсветить объект, если мышка наведена над тем объектом, который не подсвечивался в прошлый раз
         if not lFlagKeyPressedCtrl:
             #Получить координаты мыши
             if lAltBool == False: # СВЕТИТЬ, НО НЕ ВЫБИРАТЬ
                 lElementFounded=UIOMouseSearchReturn(False)
             #Подсветить объект, если он мышь раньше стояла на другом объекте
             if lGUISearchElementSelected != lElementFounded:
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/Utils/JSONNormalize.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/JSONNormalize.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/Utils/ProcessBitness.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/ProcessBitness.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,49 +27,53 @@
         global mSettingsDict
         #Update values in settings from input
         mSettingsDict.update(inSettingsDict)
         #mSettingsDict = inSettingsDict
         ####################
         #Detect OS bitness
         ####BitnessOS#######
-        lBitnessOS="32";
-        if pywinauto.sysinfo.is_x64_OS():
-            lBitnessOS="64";
-        inSettingsDict["BitnessOS"]=lBitnessOS
+        lBitnessOS="32"
+        if CrossOS.IS_WINDOWS_BOOL:
+            if pywinauto.sysinfo.is_x64_OS():
+                lBitnessOS="64"
+            inSettingsDict["BitnessOS"]=lBitnessOS
+        else: 
+            lBitnessOS="64"
         ####################
         #Detect current process bitness
         ####BitnessProcessCurrent#######
         lBitnessProcessCurrent = str(struct.calcsize("P") * 8)
         inSettingsDict["BitnessProcessCurrent"]=lBitnessProcessCurrent
         #####################################
         #Create the other bitness process if OS is 64 and we have another Python path
         ##########################################################################
         #Check if OS is x64, else no 64 is applicable
-        if mSettingsDict["BitnessOS"]=="64":
-            #Check if current bitness is 64
-            if mSettingsDict["BitnessProcessCurrent"]=="64":
-                #create x32 if Python 32 path is exists
-                if mSettingsDict["Python32FullPath"] and mSettingsDict["Python32ProcessName"]:
-                    #Calculate python.exe folder path
-                    lPython32FolderPath= "\\".join(mSettingsDict["Python32FullPath"].split("\\")[:-1])
-                    lPython32NewNamePath = f"{lPython32FolderPath}\\{mSettingsDict['Python32ProcessName']}"
-                    if not os.path.isfile(lPython32NewNamePath):
-                        shutil.copyfile(mSettingsDict["Python32FullPath"],lPython32NewNamePath)
-                    #pdb.set_trace()
-                    mSettingsDict["Python32Process"] = subprocess.Popen([lPython32NewNamePath] + mSettingsDict["PythonArgs"],stdin=subprocess.PIPE,stdout=subprocess.PIPE,stderr=subprocess.PIPE)
-            else:
-                #bitness current process is 32
-                #return x64 if it is exists
-                if mSettingsDict["Python64Process"]:
-                    #Calculate python.exe folder path
-                    lPython64FolderPath= "\\".join(mSettingsDict["Python64FullPath"].split("\\")[:-1])
-                    lPython64NewNamePath = f"{lPython64FolderPath}\\{mSettingsDict['Python64ProcessName']}"
-                    if not os.path.isfile(lPython64NewNamePath):
-                        shutil.copyfile(mSettingsDict["Python64FullPath"],lPython64NewNamePath)
-                    mSettingsDict["Python64Process"] = subprocess.Popen([lPython64NewNamePath] + mSettingsDict["PythonArgs"],stdin=subprocess.PIPE,stdout=subprocess.PIPE,stderr=subprocess.PIPE)
+        if CrossOS.IS_WINDOWS_BOOL:
+            if mSettingsDict["BitnessOS"]=="64":
+                #Check if current bitness is 64
+                if mSettingsDict["BitnessProcessCurrent"]=="64":
+                    #create x32 if Python 32 path is exists
+                    if mSettingsDict["Python32FullPath"] and mSettingsDict["Python32ProcessName"]:
+                        #Calculate python.exe folder path
+                        lPython32FolderPath= "\\".join(mSettingsDict["Python32FullPath"].split("\\")[:-1])
+                        lPython32NewNamePath = f"{lPython32FolderPath}\\{mSettingsDict['Python32ProcessName']}"
+                        if not os.path.isfile(lPython32NewNamePath):
+                            shutil.copyfile(mSettingsDict["Python32FullPath"],lPython32NewNamePath)
+                        #pdb.set_trace()
+                        mSettingsDict["Python32Process"] = subprocess.Popen([lPython32NewNamePath] + mSettingsDict["PythonArgs"],stdin=subprocess.PIPE,stdout=subprocess.PIPE,stderr=subprocess.PIPE)
+                else:
+                    #bitness current process is 32
+                    #return x64 if it is exists
+                    if mSettingsDict["Python64Process"]:
+                        #Calculate python.exe folder path
+                        lPython64FolderPath= "\\".join(mSettingsDict["Python64FullPath"].split("\\")[:-1])
+                        lPython64NewNamePath = f"{lPython64FolderPath}\\{mSettingsDict['Python64ProcessName']}"
+                        if not os.path.isfile(lPython64NewNamePath):
+                            shutil.copyfile(mSettingsDict["Python64FullPath"],lPython64NewNamePath)
+                        mSettingsDict["Python64Process"] = subprocess.Popen([lPython64NewNamePath] + mSettingsDict["PythonArgs"],stdin=subprocess.PIPE,stdout=subprocess.PIPE,stderr=subprocess.PIPE)
 #Return the other module bitnes
 def OtherProcessGet():
     #Result template
     lResult = None
     global mSettingsDict
     #Check if OS is x64, else no 64 is applicable
     if mSettingsDict["BitnessOS"]=="64":
@@ -80,8 +84,8 @@
                 lResult = mSettingsDict["Python32Process"]
         else:
             #bitness current process is 32
             #return x64 if it is exists
             if mSettingsDict["Python64Process"]:
                 lResult = mSettingsDict["Python64Process"]
     #Exit
-    return lResult
+    return lResult
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/Utils/ProcessCommunicator.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/ProcessCommunicator.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/Utils/TimerRepeat.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/TimerRepeat.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/Utils/ValueVerify.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/Utils/ValueVerify.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Robot/__main__.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Robot/__main__.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Studio/JSONNormalize.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Studio/JSONNormalize.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Studio/ProcessCommunicator.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Studio/ProcessCommunicator.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Studio/Processor.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Studio/Processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,16 @@
             lDefStr = lSplitList[-1]
             lModule = sys.modules[lModuleStr]
             lModuleDefList = dir(lModule)
             if lDefStr in lModuleDefList:
                 lItemDef = getattr(lModule,lDefStr)
                 if callable(lItemDef): lDef=lItemDef
                 else: raise Exception("Def is not callable")
+        if lActivityItem.get("ArgList", None) == None: lActivityItem["ArgList"]=[]
+        if lActivityItem.get("ArgDict", None) == None: lActivityItem["ArgDict"]={} 
         # Обработка случая - аргумент строка. Актуально для XPATH и CSS селекторов
         if isinstance(lActivityItem["ArgList"], str): 
             try: lActivityItemResult = lDef(lActivityItem["ArgList"])
             except Exception as e: lActivityItemResult={"ErrorHeader":str(e), "ErrorTraceback":traceback.format_exc()}
         else:
             try:lActivityItemResult = lDef(*lActivityItem["ArgList"], **lActivityItem["ArgDict"])
             except Exception as e: lActivityItemResult={"ErrorHeader":str(e), "ErrorTraceback":traceback.format_exc()}
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Studio/RobotConnector.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Studio/RobotConnector.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Studio/Studio.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Studio/Studio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import argparse
 
 parser = argparse.ArgumentParser(description='pyOpenRPA (ORPA) CLI')
 parser.add_argument('file', help='Путь к файлу конфигурации')
 parser.add_argument('--mode', choices=['app', 'web'], default="app", help='Режим запуска: app - запуск в качестве приложения, web - запуск в качестве веб сервера')
 args = parser.parse_args()
-
-import win32gui
-import win32con
-# Получение дескриптора окна консоли
-hwnd = win32gui.GetForegroundWindow()
+from ..Utils import CrossOS
+if CrossOS.IS_WINDOWS_BOOL:
+    import win32gui
+    import win32con
+    # Получение дескриптора окна консоли
+    hwnd = win32gui.GetForegroundWindow()
 
 from http.server import BaseHTTPRequestHandler
 import json
 import os
 import sys
 import traceback
 if args.mode=="app": 
@@ -34,20 +35,24 @@
 from fastapi.templating import Jinja2Templates
 import uvicorn
 import io
 import importlib.util
 from starlette.responses import StreamingResponse
 from typing import Union
 import threading
-from ..Utils import CrossOS
+
 from ..Robot import UIWeb
 import time
 import requests
 lRepoPathStr = CrossOS.PathJoinList(CrossOS.PathSplitList(__file__)[:-4])
-lTesseractExeStr = os.path.join(lRepoPathStr, "Resources", "WTesseract64-400", "tesseract.exe")
+lTesseractExeStr = None
+if CrossOS.IS_WINDOWS_BOOL:
+    lTesseractExeStr = os.path.join(lRepoPathStr, "Resources", "WTesseract64-400", "tesseract.exe")
+else:
+    lTesseractExeStr = "tesseract"
 pytesseract.pytesseract.tesseract_cmd = lTesseractExeStr #old 'C:\\Program Files\\Tesseract-OCR\\tesseract.exe'
 lPackagePathStr = CrossOS.PathJoinList(CrossOS.PathSplitList(__file__)[:-2])
 lResourcePathStr = os.path.join(lPackagePathStr, "Resources")
 #Единый глобальный словарь (За основу взять из Settings.py)
 global gSettingsDict
 #Call Settings function from argv[1] file
 ################################################
@@ -116,15 +121,15 @@
 import pyOpenRPA
 import requests
 gProgramDataPathStr=""
 if CrossOS.IS_WINDOWS_BOOL: gProgramDataPathStr = "C:\\ProgramData"
 if CrossOS.IS_LINUX_BOOL: gProgramDataPathStr = os.path.expanduser("~/.config")
 gProgramDataPORPathStr = os.path.join(gProgramDataPathStr, "pyOpenRPA")
 
-if not os.path.exists(gProgramDataPORPathStr): os.mkdir(gProgramDataPORPathStr)
+if not os.path.exists(gProgramDataPORPathStr): os.makedirs(gProgramDataPORPathStr, exist_ok=True)
 DEFINE = None
 # ПАКЕТ ДЛЯ ВСТАВКИ В МОДУЛИ
 def cert_validate(in_cert_path_str = "orpa.key", in_version_str="1.4.0"):
     l_data = cert_load(in_cert_path_str = in_cert_path_str)
     result = False
     if l_data != None:
       required_fields = ["pc_str", "ver_str", "time_from_float", "time_to_float", "is_ee_bool", "is_online_bool"]
@@ -207,45 +212,46 @@
         self.mResponseContentCode = None
     #ResponseContentTypeFile
     def SendResponseContentTypeFile(self,inContentType,inFilePath):
         # Send response status code
         # Send headers
         self.mResponseContentCode = 200
         self.mResponseContentType=inContentType
+        inFilePath = CrossOS.PathStr(inPathStr = inFilePath)
         lFileObject = open(inFilePath, "rb") 
         lData = lFileObject.read()
         #Закрыть файловый объект
         lFileObject.close()       
         # Write content as utf-8 data
         return lData
  
     # GET
     def do_GET(self, inBodyStr):
-        lStudioFolder = "\\".join(__file__.split("\\")[:-1])
+        lStudioFolder = CrossOS.PathJoinList(CrossOS.PathSplitList(__file__)[:-1])
         #Мост между файлом и http запросом (новый формат)
         if self.path == "/":
             # Пример использования
             global gRender
             global DEFINE
             lVersionStr = __version__
             if DEFINE["is_ee_bool"]==True: lVersionStr+=" EE"
             else: lVersionStr+=" CE"
             if DEFINE["is_online_bool"]==True: lVersionStr+=" ONLINE"
-            lStr = gRender.Generate(inDataDict={"title":"pyOpenRPA (ORPA)", "subtitle":"Студия", "version":lVersionStr , "is_ee_bool": DEFINE["is_ee_bool"]})
+            lStr = gRender.Generate(inDataDict={"title":"pyOpenRPA (ORPA)", "subtitle":"Студия", "version":lVersionStr , "is_ee_bool": DEFINE["is_ee_bool"], "is_linux_bool": CrossOS.IS_LINUX_BOOL})
             self.mResponseContentCode = 200
             self.mResponseContentType="text/html"
             # Write content as utf-8 data
             return bytes(lStr, "utf8")
         #Мост между файлом и http запросом (новый формат)
         if self.path == '/favicon.ico':
             return self.SendResponseContentTypeFile('image/x-icon', os.path.join(lStudioFolder, "..\\Resources\\Web\\orpa\\favicon.ico"))
 		#Мост между файлом и http запросом (новый формат)
         if self.path == '/pyOpenRPA_logo.png' or self.path == '/orpa/resources/Web/orpa/logo.png':
             return self.SendResponseContentTypeFile('image/png', os.path.join(lStudioFolder, "..\\Resources\\Web\\orpa\\logo.png"))
-        if self.path == '/metadata.json': return self.SendResponseContentTypeFile('application/json', os.path.join(lStudioFolder, "..\\Resources\\Web\\orpa\\\styleset\\metadata.json"))
+        if self.path == '/metadata.json': return self.SendResponseContentTypeFile('application/json', os.path.join(lStudioFolder, "..\\Resources\\Web\\orpa\\styleset\\metadata.json"))
 
     # POST
     def do_POST(self, inBodyStr):
         #Restart studio
         if self.path == '/RestartStudio':
             os.execl(sys.executable,os.path.abspath(__file__),*sys.argv)
             sys.exit(0)
@@ -305,17 +311,21 @@
 from . import Processor
 
 # RestartOrpaLab
 @app.post(path="/api/orpa-lab-restart",response_class=JSONResponse,tags=["API"])
 def pyOpenRPA_OrpaLabRestart(inRequest:Request):
     # Recieve the data
     global gLogger
-    os.system(f"taskkill /F /IM orpa-lab.exe")
-    os.system(f"taskkill /F /IM jupyter-lab.exe")
-    os.system("start /B orpa-lab.exe -m jupyter lab --config=\"..\Resources\WConfigure\Orpa_lab_config.py")
+    if CrossOS.IS_WINDOWS_BOOL:
+        os.system(f"taskkill /F /IM orpa-lab.exe")
+        os.system(f"taskkill /F /IM jupyter-lab.exe")
+        os.system("start /B orpa-lab.exe -m jupyter lab --config=\"..\Resources\WConfigure\Orpa_lab_config.py")
+    else:
+        os.system(f"killall -9 orpa-lab -u $USER")
+        os.system(f'orpa-lab -m jupyterlab --config="../Resources/LConfigure/Orpa_lab_config.py" &')
     gLogger.info(f"Компонент orpa-lab перезапущен")
     
 # SetNewPath for orpa lab + restart orpa
 @app.post(path="/api/orpa-lab-set-path",response_class=JSONResponse,tags=["API"])
 def pyOpenRPA_OrpaLabSetPath(inRequest:Request):
     # Recieve the data
     global gLogger
@@ -330,17 +340,19 @@
 
 # OpenFolder in Explorer
 @app.post(path="/api/orpa-lab-open-path",response_class=JSONResponse,tags=["API"])
 def pyOpenRPA_OrpaLabOpenPath(inRequest:Request):
     # Recieve the data
     global gLogger
     location_str = config.orpa_lab_path_str
-    location_str = location_str.replace("/","\\")
-    os.system(f"explorer.exe {location_str}")
-
+    if CrossOS.IS_WINDOWS_BOOL:
+        location_str = location_str.replace("/","\\")
+        os.system(f"explorer.exe {location_str}")
+    else:
+        os.system(f"xdg-open {location_str}")
 
 # Execute activity list
 @app.post(path="/api/activity-list-execute",response_class=JSONResponse,tags=["API"])
 def pyOpenRPA_ActivityListExecute(inRequest:Request, inBodyStr:str = Body(...)):
     # Recieve the data
     global gLogger
     lValueStr = inBodyStr
@@ -382,45 +394,49 @@
 gSnipScreenPath = ""
 @app.post(path="/api/snipingtool-screenshot-render",tags=["API"])
 def snipingtool_screen_path(inRequest:Request, inBodyStr:str = Body(...)):
     global gSnipScreenPath
     lValueStr = inBodyStr
     # Превращение массива байт в объект
     lInput = json.loads(lValueStr)
-    gSnipScreenPath = lInput['Path']
+    gSnipScreenPath = CrossOS.PathStr(lInput['Path']) 
 @app.get(path="/api/snipingtool-screenshot-render",tags=["API"])
 def snipingtool_screen_render(inRequest:Request):
     global gSnipScreenPath
     return FileResponse(gSnipScreenPath)
 
 #Удаление элементов отображенных в img tree
 @app.post(path="/api/orpa-screen-img-tree-item-delete",tags=["API"])
 def img_tree_item_delete(inRequest:Request, inBodyStr:str = Body(...)):
     lValueStr = inBodyStr
     # Превращение массива байт в объект
     lInput = json.loads(lValueStr)
+    lInput['Path'] = CrossOS.PathStr(lInput['Path'])
     try: os.unlink(lInput['Path'])
     except Exception as e: return {"ErrorHeader":str(e), "ErrorTraceback":traceback.format_exc()}
 
 #Переименование элементов отображенных в img tree
 @app.post(path="/api/orpa-screen-img-tree-item-rename",tags=["API"])
 def img_tree_item_rename(inRequest:Request, inBodyStr:str = Body(...)):
     lValueStr = inBodyStr
     # Превращение массива байт в объект
     lInput = json.loads(lValueStr)
+    lInput['Path'] = CrossOS.PathStr(lInput['Path'])
+    lInput['NewPath'] = CrossOS.PathStr(lInput['NewPath'])
     try: os.rename(lInput['Path'], lInput["NewPath"])
     except Exception as e: return {"ErrorHeader":str(e), "ErrorTraceback":traceback.format_exc()}
 
 #Инициация тессеракта по изображению
 @app.post(path="/api/orpa-screen-tesseract-run",tags=["API"])
 def tesseract_result(inRequest:Request, inBodyStr:str = Body(...)):
     lValueStr = inBodyStr
     # Превращение массива байт в объект
     lInput = json.loads(lValueStr)
     lPath = lInput['Path']
+    lPath = CrossOS.PathStr(lPath)
     try:
         lTesseractResult = [pytesseract.image_to_string(Image.open(lPath), lang='rus+eng')]
         return lTesseractResult
     except Exception as e: return {"ErrorHeader":str(e), "ErrorTraceback":traceback.format_exc()}
 
     
 @app.get(path="/api/helper-def-list/{inTokenStr}",response_class=JSONResponse,tags=["API"])
@@ -523,21 +539,28 @@
     global args
     if args.mode=="app": 
         # Запуск адреса в браузере
         browser_portable = UIWeb.BrowserChromeStart(inMaximizeBool=True,inModeStr="APP", inUrlStr=f"http://localhost:{lPort}")
         UIWeb.gBrowser=None
         UIWeb.gBrowserHandle=None
         # Скрытие окна консоли
-        global hwnd
-        win32gui.ShowWindow(hwnd, win32con.SW_HIDE)
+        if CrossOS.IS_WINDOWS_BOOL:
+            global hwnd
+            win32gui.ShowWindow(hwnd, win32con.SW_HIDE)
         CheckChromePortable()
         #UIWeb.PageOpen(f"http://127.0.0.1:{lPort}")
     else:
-        # Запуск адреса в браузере
-        os.system(f"explorer http://localhost:{lPort}")
+        if CrossOS.IS_WINDOWS_BOOL:
+            # Запуск адреса в браузере
+            os.system(f"explorer http://localhost:{lPort}")
+        else:
+            pass
+            #print("send cmd")
+            #os.system(f"xdg-open http://localhost:{lPort}")
+        
 
 def CheckChromePortable():
     global browser_portable
     while True:
         if browser_portable!=None:
             js_str = "2+2"
             try:
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Studio/ValueVerify.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Studio/ValueVerify.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotDB/HowToUse` & `pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotDB/HowToUse`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotDB/RobotDB.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotDB/RobotDB.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotDB/Server.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotDB/Server.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotDB/ServerSettings.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotDB/ServerSettings.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotScreenActive/Screen.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotScreenActive/Screen.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Tools/RobotScreenActive/__main__.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Tools/RobotScreenActive/__main__.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Tools/Template.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Tools/Template.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Tools/Usage.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Tools/Usage.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Utils/CrossOS.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Utils/CrossOS.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Utils/Debugger.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Utils/Debugger.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Utils/Dictionary.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Utils/Dictionary.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Utils/Disk.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Utils/Disk.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Utils/License.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Utils/License.py`

 * *Files 22% similar despite different names*

```diff
@@ -98,45 +98,45 @@
 
 По всем вопросам Вы можете обратиться к правообладателю, контакты см. по адресу: 
 https://pyopenrpa.ru/Index/pyOpenRPA_product_service.pdf
 Используя ПО pyOpenRPA Вы осознаете свою ответственность в случаях нарушения лицензионного законодательства и совершения неправомерных действий.
 
 ВНИМАНИЕ! НЕЗНАНИЕ ЗАКОНА НЕ ОСВОБОЖДАЕТ ОТ ОТВЕТСТВЕННОСТИ.
             """.format(lCertificateKeyStr)
-            print(lTextStr)
+            #print(lTextStr)
             os.environ["PYOPENRPA_NODISP"]="1"
     return lCertificateExistsBool
 
 def ConsoleAccept():
     """ Start pyOpenRPA activation master
 
     :return: _description_
     :rtype: str
     """
     if "PYOPENRPA_NODISP" not in os.environ:
         lText="""
-░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
-░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
-░░░░░░░░░░░░░░░░░░░    ░░░░░   ░░░░░░░░░░░░
-░░░░░░░░░░░░░░░░░░░    ░░░░░   ░░░░░░░░░░░░
-░░░░░░░░░░░   ░░░░░    ░░░░░   ░░░░░░░░░░░░
-░░░░░░░░░░░   ░░░░░    ░░░░░   ░░░░░░░░░░░░
-░░░░░░░░░░░   ░░░░░    ░░░░░   ░░░░░░   ░░░
-░░░░░░░░░░░   ░░░░░    ░░░░░   ░░░    ░░░░░
-░░░░░░░░░░░   ░░░░░    ░░░░░       ░░░░░░░░
-░░░   ░░░░░   ░░░░░    ░░░░░    ░░░░░░░░░░░
-░░░░░    ░░   ░░░░░    ░░    ░░░░░░░░░░░░░░
-░░░░░░░       ░░░░░        ░░░░░░░░░░░░░░░░
-░░░░░░░░░░    ░░░░░    ░░░░░░░░░░░░░░░░░░░░
-░░░░░░░░░░░░    ░░░    ░░░░░░░░░░░░░░░░░░░░
-░░░░░░░░░░░░░░         ░░░░░░░░░░░░░░░░░░░░
-░░░░░░░░░░░░░░░░░      ░░░░░░░░░░░░░░░░░░░░
-░░░░░░░░░                        ░░░░░░░░░░
-░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
-░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
+###########################################
+###########################################
+###################    #####   ############
+###################    #####   ############
+###########   #####    #####   ############
+###########   #####    #####   ############
+###########   #####    #####   ######   ###
+###########   #####    #####   ###    #####
+###########   #####    #####       ########
+###   #####   #####    #####    ###########
+#####    ##   #####    ##    ##############
+#######       #####        ################
+##########    #####    ####################
+############    ###    ####################
+##############         ####################
+#################      ####################
+#########                        ##########
+###########################################
+###########################################
         """
         print(lText)
         time.sleep(2)
         lText="""
 (RUS LANGUAGE) 
 ***********************************************
 Добро пожаловать в систему активации pyOpenRPA | ORPA!
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Utils/Network.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Utils/Network.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Utils/Render.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Utils/Render.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA/Utils/StopSafe.py` & `pyOpenRPA-1.4.1/pyOpenRPA/Utils/StopSafe.py`

 * *Files identical despite different names*

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA.egg-info/PKG-INFO` & `pyOpenRPA-1.4.1/pyOpenRPA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyOpenRPA
-Version: 1.4.0
+Version: 1.4.1
 Summary: The powerful open source RPA platform for business
 Home-page: https://pyopenrpa.ru/
 Author: Ivan Maslov
 Author-email: Ivan.Maslov@pyopenrpa.ru
 License: Текст лицензии см. в файле: LICENSE.PDF (в корне) или по адресу: https://pyopenrpa.ru/license/oferta.pdf
 Description: <!-- pyOpenRPA documentation master file, created by
         sphinx-quickstart on Sat Dec 19 23:59:00 2020.
@@ -55,15 +55,15 @@
         Ivan Maslov contacts (CEO & FOUNDER): 
         
         - E-mail: Ivan.Maslov@pyOpenRPA.ru
         - Skype: MegaFinder
         - Web: https://pyopenrpa.ru/
         - Telegram: https://t.me/pyopenrpa
         - WhatsApp | Telegram: +7 906 722 39 25 | @IvanMaslov
-Keywords: pyOpenRPA OpenRPA RPA Robot Automation Robotization OpenSource IT4Business
+Keywords: pyOpenRPA ORPA OpenRPA RPA Robot Automation Robotization OpenSource
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Free For Educational Use
 Classifier: License :: Free For Home Use
 Classifier: License :: Free for non-commercial use
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `pyOpenRPA-1.4.0/pyOpenRPA.egg-info/SOURCES.txt` & `pyOpenRPA-1.4.1/pyOpenRPA.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -233,14 +233,16 @@
 pyOpenRPA/Resources/Web/orpa/logo.png
 pyOpenRPA/Resources/Web/orpa/orc.js
 pyOpenRPA/Resources/Web/orpa/orc.xhtml
 pyOpenRPA/Resources/Web/orpa/std.css
 pyOpenRPA/Resources/Web/orpa/std.js
 pyOpenRPA/Resources/Web/orpa/std.xhtml
 pyOpenRPA/Resources/Web/orpa/std_browser.js
+pyOpenRPA/Resources/Web/orpa/std_desktop.js
+pyOpenRPA/Resources/Web/orpa/std_desktop_linux.js
 pyOpenRPA/Resources/Web/orpa/std_floidd.css
 pyOpenRPA/Resources/Web/orpa/std_floidd.js
 pyOpenRPA/Resources/Web/orpa/std_helper.js
 pyOpenRPA/Resources/Web/orpa/styleset/Lato-Bold.woff2
 pyOpenRPA/Resources/Web/orpa/styleset/Lato-Italic.woff2
 pyOpenRPA/Resources/Web/orpa/styleset/Lato-Regular.woff2
 pyOpenRPA/Resources/Web/orpa/styleset/bg1.jpg
@@ -285,18 +287,20 @@
 pyOpenRPA/Robot/Test.py
 pyOpenRPA/Robot/UIDesktop.py
 pyOpenRPA/Robot/UIWeb.py
 pyOpenRPA/Robot/Window.py
 pyOpenRPA/Robot/__init__.py
 pyOpenRPA/Robot/__main__.py
 pyOpenRPA/Robot/Utils/JSONNormalize.py
+pyOpenRPA/Robot/Utils/LCompatibility.py
 pyOpenRPA/Robot/Utils/ProcessBitness.py
 pyOpenRPA/Robot/Utils/ProcessCommunicator.py
 pyOpenRPA/Robot/Utils/TimerRepeat.py
 pyOpenRPA/Robot/Utils/ValueVerify.py
+pyOpenRPA/Robot/Utils/WCompatibility.py
 pyOpenRPA/Robot/Utils/__init__.py
 pyOpenRPA/Studio/JSONNormalize.py
 pyOpenRPA/Studio/ProcessCommunicator.py
 pyOpenRPA/Studio/Processor.py
 pyOpenRPA/Studio/RobotConnector.py
 pyOpenRPA/Studio/Studio.py
 pyOpenRPA/Studio/ValueVerify.py
@@ -324,10 +328,12 @@
 pyOpenRPA/Utils/CrossOS.py
 pyOpenRPA/Utils/Debugger.py
 pyOpenRPA/Utils/Dictionary.py
 pyOpenRPA/Utils/Disk.py
 pyOpenRPA/Utils/License.py
 pyOpenRPA/Utils/Network.py
 pyOpenRPA/Utils/Render.py
+pyOpenRPA/Utils/SSH.py
 pyOpenRPA/Utils/StopSafe.py
 pyOpenRPA/Utils/Text.py
-pyOpenRPA/Utils/__define__.py
+pyOpenRPA/Utils/__define__.py
+pyOpenRPA/Utils/Administrator/__main__.py
```

### Comparing `pyOpenRPA-1.4.0/setup.py` & `pyOpenRPA-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,38 +47,40 @@
 		'Programming Language :: Python :: 3.10',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Software Development :: Testing',
         'Topic :: Software Development :: User Interfaces',
         'Topic :: Software Development :: Quality Assurance',
         'Topic :: Home Automation'
       ],
-      keywords='pyOpenRPA OpenRPA RPA Robot Automation Robotization OpenSource IT4Business',
+      keywords='pyOpenRPA ORPA OpenRPA RPA Robot Automation Robotization OpenSource',
       url='https://pyopenrpa.ru/',
       author='Ivan Maslov',
       author_email='Ivan.Maslov@pyopenrpa.ru',
       license='Текст лицензии см. в файле: LICENSE.PDF (в корне) или по адресу: https://pyopenrpa.ru/license/oferta.pdf',
       packages=find_packages(),
       install_requires=[
           'pillow>=6.0.0',
 		  'keyboard>=0.13.3',
+          'pyscreeze==0.1.21',
 		  'pyautogui<=0.9.52',
 		  'psutil>=5.6.2',
 		  'crypto>=1.4.1', 
 		  'schedule>=1.1.0', 
 		  'Jinja2>=2.2.11.2', 
-		  'selenium>=3.141.0',
+		  'selenium==3.141.0',
 		  'fastapi>=0.81.0',
 		  'uvicorn>=0.18.3',
           'python-multipart>=0.0.6',
           'autodocsumm>=0.2.10',
-          'screeninfo>=0.8.1'
+          'screeninfo>=0.8.1',
+          "pytesseract"
       ],
 	  extras_require={
         ':sys_platform == "win32"': [
-            'pywin32>=224', 'WMI>=1.4.9', 'pywinauto>=0.6.8'
+            'pywin32>=224', 'WMI>=1.4.9', 'pywinauto>=0.6.8', 'desktopmagic'
         ],
         ':"linux" in sys_platform': [
             'simplepam>=0.1.5', 'pyclip>=0.6.0'
         ]
 	},
       include_package_data=True,
       #data_files = datafiles,
```

