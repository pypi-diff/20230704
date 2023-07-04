# Comparing `tmp/oarepo-vocabularies-2.0.4.tar.gz` & `tmp/oarepo-vocabularies-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-vocabularies-2.0.4.tar", last modified: Thu Jun 22 16:02:35 2023, max compression
+gzip compressed data, was "oarepo-vocabularies-2.0.5.tar", last modified: Tue Jul  4 08:39:28 2023, max compression
```

## Comparing `oarepo-vocabularies-2.0.4.tar` & `oarepo-vocabularies-2.0.5.tar`

### file list

```diff
@@ -1,134 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.602534 oarepo-vocabularies-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-22 16:02:35.602534 oarepo-vocabularies-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.582534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.586534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/models/ui.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.586534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.590534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.590534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/records/jsonschemas/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.590534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.590534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.594534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.594534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/components/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.594534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/custom_fields/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/ui_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.566534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.566534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/templates/oarepo_ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.594534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/templates/oarepo_ui/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.594534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.566534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.594534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.566534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.594534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.594534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.598534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/resources/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.566534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.570534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.598534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/main.html
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.598534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.570534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.574534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.570534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.598534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.598534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.598534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.570534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.598534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.598534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.574534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.598534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/collections/grid.overrides
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.598534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/sample.overrides
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/sample.variables
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.574534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.598534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next-scanner.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.602534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.602534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.602534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.602534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.602534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.602534 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileCatalog.js
--rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileLanguages.sh
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/initCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/translations.pot
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/webpack.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:02:35.586534 oarepo-vocabularies-2.0.4/oarepo_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-22 16:02:35.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-22 16:02:35.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:02:35.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-22 16:02:35.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 16:02:35.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 16:02:35.000000 oarepo-vocabularies-2.0.4/oarepo_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-22 16:02:35.602534 oarepo-vocabularies-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-22 15:57:48.000000 oarepo-vocabularies-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.755565 oarepo-vocabularies-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-04 08:39:28.755565 oarepo-vocabularies-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.743564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ext_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/models/ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/records/jsonschemas/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/components/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/custom_fields/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/ui_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.739564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.739564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/templates/oarepo_ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/templates/oarepo_ui/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.739564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.739564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/resources/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.739564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.739564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.743564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.743564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.743564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.743564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.743564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/collections/grid.overrides
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/sample.overrides
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/sample.variables
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.743564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.751564 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.755565 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.755565 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.755565 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.755565 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileCatalog.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileLanguages.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/translations.pot
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/webpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:28.747564 oarepo-vocabularies-2.0.5/oarepo_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-04 08:39:28.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-07-04 08:39:28.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:39:28.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-04 08:39:28.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-04 08:39:28.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 08:39:28.000000 oarepo-vocabularies-2.0.5/oarepo_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-04 08:39:28.755565 oarepo-vocabularies-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 08:35:17.000000 oarepo-vocabularies-2.0.5/setup.py
```

### Comparing `oarepo-vocabularies-2.0.4/LICENSE` & `oarepo-vocabularies-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/MANIFEST.in` & `oarepo-vocabularies-2.0.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/PKG-INFO` & `oarepo-vocabularies-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 2.0.4
+Version: 2.0.5
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo vocabularies
```

### Comparing `oarepo-vocabularies-2.0.4/README.md` & `oarepo-vocabularies-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ext.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ext.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,21 +12,37 @@
         """Flask application initialization."""
         self.init_config(app)
         self.init_resource(app)
         app.extensions["oarepo-vocabularies"] = self
 
     def init_config(self, app):
         """Initialize configuration."""
-        from . import config
+        from . import config, ext_config
 
         for k in dir(config):
             if k.startswith("OAREPO_VOCABULARIES_"):
                 app.config.setdefault(k, getattr(config, k))
             if k.startswith("DEFAULT_DATASTREAMS_"):
                 app.config.setdefault(k, {}).update(getattr(config, k))
             if k.startswith("DATASTREAMS_CONFIG_GENERATOR_"):
                 app.config.setdefault(k, getattr(config, k))
-        app.config.setdefault('VOCABULARIES_FACET_CACHE_SIZE', config.VOCABULARIES_FACET_CACHE_SIZE)
-        app.config.setdefault('VOCABULARIES_FACET_CACHE_TTL', config.VOCABULARIES_FACET_CACHE_TTL)
+        app.config.setdefault(
+            "VOCABULARIES_FACET_CACHE_SIZE", config.VOCABULARIES_FACET_CACHE_SIZE
+        )
+        app.config.setdefault(
+            "VOCABULARIES_FACET_CACHE_TTL", config.VOCABULARIES_FACET_CACHE_TTL
+        )
+
+        if "OAREPO_PERMISSIONS_PRESETS" not in app.config:
+            app.config["OAREPO_PERMISSIONS_PRESETS"] = {}
+
+        for k in ext_config.OAREPO_VOCABULARIES_PERMISSIONS_PRESETS:
+            if k not in app.config["OAREPO_PERMISSIONS_PRESETS"]:
+                app.config["OAREPO_PERMISSIONS_PRESETS"][
+                    k
+                ] = ext_config.OAREPO_VOCABULARIES_PERMISSIONS_PRESETS[k]
 
     def init_resource(self, app):
-        pass
+        """Initialize vocabulary resources."""
+        self.service = app.config["VOCABULARY_TYPE_SERVICE"](
+            config=app.config["VOCABULARY_TYPE_SERVICE_CONFIG"](),
+        )
```

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/fixtures.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/fixtures.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/models/ui.json` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/models/ui.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/records/api.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/records/api.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/resources/config.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/resources/records/ui.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/components/hierarchy.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/components/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/config.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/resources/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,37 @@
-from invenio_records_resources.services import Link
-from invenio_vocabularies.services import VocabulariesServiceConfig
+import marshmallow as ma
+from oarepo_ui.resources.config import RecordsUIResourceConfig
 
-from oarepo_vocabularies.records.api import Vocabulary
-from oarepo_vocabularies.services.components.hierarchy import HierarchyComponent
-from oarepo_vocabularies.services.schema import VocabularySchema
-from oarepo_vocabularies.services.search import VocabularySearchOptions
+from oarepo_vocabularies.ui.resources.components import VocabulariesSearchComponent
 
 
-class VocabulariesConfig(VocabulariesServiceConfig):
-    record_cls = Vocabulary
-    schema = VocabularySchema
-    search = VocabularySearchOptions
-    components = [*VocabulariesServiceConfig.components, HierarchyComponent]
+class InvenioVocabulariesUIResourceConfig(RecordsUIResourceConfig):
+    template_folder = "../templates"
     url_prefix = "/vocabularies/"
-    links_item = {
-        **VocabulariesServiceConfig.links_item,
-        "vocabulary": Link(
-            "{+api}/vocabularies/{type}",
-            vars=lambda record, vars: vars.update(
-                {
-                    "type": record.type.id,
-                }
-            ),
-        ),
-        "parent": Link(
-            "{+api}/vocabularies/{type}/{parent}",
-            vars=lambda record, vars: vars.update(
-                {
-                    "type": record.type.id,
-                    "parent": record.get("hierarchy", {}).get("parent"),
-                }
-            ),
-            when=lambda obj, ctx: bool(obj.get("hierarchy", {}).get("parent")),
-        ),
-        "children": Link(
-            "{+api}/vocabularies/{type}?h-parent={id}",
-            vars=lambda record, vars: vars.update(
-                {
-                    "type": record.type.id,
-                    "id": record.pid.pid_value,
-                }
-            ),
-        ),
-        "descendants": Link(
-            "{+api}/vocabularies/{type}?h-ancestor={id}",
-            vars=lambda record, vars: vars.update(
-                {
-                    "type": record.type.id,
-                    "id": record.pid.pid_value,
-                }
-            ),
-        ),
+    blueprint_name = "oarepo_vocabularies_ui"
+    ui_serializer_class = (
+        "oarepo_vocabularies.resources.records.ui.VocabularyUIJSONSerializer"
+    )
+    api_service = "vocabularies"
+    layout = "oarepo_vocabularies_ui"
+
+    templates = {
+        "detail": {
+            "layout": "oarepo_vocabularies_ui/detail.html",
+            "blocks": {
+                "record_main_content": "oarepo_vocabularies_ui/main.html",
+                "record_sidebar": "oarepo_vocabularies_ui/sidebar.html",
+                "record_descendants": "oarepo_vocabularies_ui/descendants.html"
+            },
+        },
+        "search": {"layout": "oarepo_vocabularies_ui/search.html"},
+    }
+
+    routes = {
+        "search": "/<vocabulary_type>/",
+        "detail": "/<vocabulary_type>/<pid_value>",
+        "export": "/<vocabulary_type>/<pid_value>/export/<export_format>",
     }
+
+    components = [VocabulariesSearchComponent]
+
+    request_vocabulary_type_args = {"vocabulary_type": ma.fields.Str()}
```

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/custom_fields/hierarchy.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/custom_fields/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/facets.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/facets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import cachetools
 from flask import current_app
 from invenio_records_resources.services.records.facets import TermsFacet
 from invenio_vocabularies.services.facets import VocabularyLabels
 
 
 class VocabularyFacet(TermsFacet):
```

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/schema.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/search.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/search.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/services/ui_schema.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/services/ui_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/translations/messages.pot` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/ext.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/resources/components.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/resources/components.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,32 @@
+from functools import partial
+
 from invenio_records_resources.services.records.components import ServiceComponent
 
 
 class VocabulariesSearchComponent(ServiceComponent):
     def before_ui_search(self, *, resource, search_options, view_args, **kwargs):
         vocabulary_type = view_args["vocabulary_type"]
         api_service = resource._api_service
         search_options.setdefault(
             "endpoint",
             api_service.config.links_search["self"].expand(
                 None, {"type": vocabulary_type, "api": "/api"}
             ),
         )
+        
+    def before_ui_detail(self, *, extra_context, resource, identity, view_args, record, **kwargs):
+        vocabulary_type = view_args["vocabulary_type"]
+        api_service = resource._api_service 
+        search_options = dict(
+            api_config=api_service.config,
+            identity=identity,
+            endpoint=api_service.config.links_search["self"].expand(
+                None, {"type": vocabulary_type, "api": "/api"}
+            ),
+            initial_filters=[["h-parent",record['id']]]
+        )
+        search_config = partial(resource.config.search_app_config, **search_options)
+        extra_context.setdefault(
+            "search_app_config",
+            search_config
+        )
```

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/resources/resource.py` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/resources/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/main.html` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/main.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,29 @@
 <!-- place your record detail main content in here ... -->
 <h1 style="margin-bottom: 1em">{%- value "title" -%}</h1>
 <dl class="ui very basic table">
   <dt>{{ _('vocabulary.vocabulary') }}</dt>
   <dd>
     <a href="/vocabularies/{{data.type}}">{{ _("vocabulary." + data.type) }}</a>
   </dd>
-  {% for l in (data.nonpreferredLabels or []) %}
-  {% if l.en %}
-    <dt>{{_("vocabulary.nonpreferredLabels_en")}}</dt>
-    <dd>{{l.en}}</dd>
-  {% endif %}
-  {% endfor %}
-  {% for l in (data.nonpreferredLabels or []) %}
-  {% if l.cs %}
-    <dt>{{_("vocabulary.nonpreferredLabels_cs")}}</dt>
-    <dd>{{l.cs}}</dd>
-  {% endif %}
-  {% endfor %}
-
-  {% for prop, val in (data.props or {}).items() %}
+  {% for l in (data.nonpreferredLabels or []) %} {% if l.en %}
+  <dt>{{_("vocabulary.nonpreferredLabels_en")}}</dt>
+  <dd>{{l.en}}</dd>
+  {% endif %} {% endfor %} {% for l in (data.nonpreferredLabels or []) %} {% if
+  l.cs %}
+  <dt>{{_("vocabulary.nonpreferredLabels_cs")}}</dt>
+  <dd>{{l.cs}}</dd>
+  {% endif %} {% endfor %} {% for prop, val in (data.props or {}).items() %}
   <dt>{{_("vocabulary." + prop)}}</dt>
   <dd>{{val}}</dd>
-  {% endfor %} 
-  {% field "created" %} 
-  {% field "updated" %}
-  {% if 'hint' in data and data.hint.cs %}
+  {% endfor %} {% field "created" %} {% field "updated" %} {% if 'hint' in data
+  and data.hint.cs %}
   <dt>{{_("vocabulary.hint_cs")}}</dt>
   <dd>{{data.hint.cs}}</dd>
-  {% endif %}
-  {% if 'hint' in data and data.hint.en %}
+  {% endif %} {% if 'hint' in data and data.hint.en %}
   <dt>{{_("vocabulary.hint_en")}}</dt>
   <dd>{{data.hint.en}}</dd>
-  {% endif %}
-  {% if data.relatedURI %}
-  {% for t in data.relatedURI.items() %}
-    <dt>{{_("vocabulary.relatedURI_" + t.0)}}</dt>
-    <dd>{{t.1}}</dd>
-  {% endfor %}
-  {% endif %}
-
+  {% endif %} {% if data.relatedURI %} {% for t in data.relatedURI.items() %}
+  <dt>{{_("vocabulary.relatedURI_" + t.0)}}</dt>
+  <dd>{{t.1}}</dd>
+  {% endfor %} {% endif %}
 </dl>
```

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/sidebar.html` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/sidebar.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,51 @@
 <!-- place your record sidebar content in here ... -->
 <section id="export-record" aria-label="Export" class="ui segment exports">
-<h2 class="ui small header">{{_('Export')}}</h2>
-<div id="recordExportDownload">
+  <h2 class="ui small header">{{_('Export')}}</h2>
+  <div id="recordExportDownload">
     <div class="ui grid">
-    <div class="eleven wide column">
+      <div class="eleven wide column">
         <div
-        role="listbox"
-        aria-expanded="false"
-        class="ui fluid selection dropdown"
-        tabindex="0"
+          role="listbox"
+          aria-expanded="false"
+          class="ui fluid selection dropdown"
+          tabindex="0"
         >
-        <div
+          <div
             aria-atomic="true"
             aria-live="polite"
             role="alert"
             class="divider text"
-        >
+          >
             JSON
-        </div>
-        <i aria-hidden="true" class="dropdown icon"></i>
-        <div class="menu transition">
+          </div>
+          <i aria-hidden="true" class="dropdown icon"></i>
+          <div class="menu transition">
             <div
-            style="pointer-events: all"
-            role="option"
-            aria-checked="true"
-            aria-selected="true"
-            class="active selected item"
+              style="pointer-events: all"
+              role="option"
+              aria-checked="true"
+              aria-selected="true"
+              class="active selected item"
             >
-            <span class="text">JSON</span>
+              <span class="text">JSON</span>
             </div>
+          </div>
         </div>
-        </div>
-    </div>
-    <div class="five wide column pl-0">
+      </div>
+      <div class="five wide column pl-0">
         <a
-        href="{{export_path}}/json"
-        title="Download file"
-        class="ui fluid button"
-        role="button"
-        >Export</a
+          href="{{export_path}}/json"
+          title="Download file"
+          class="ui fluid button"
+          role="button"
+          >Export</a
         >
+      </div>
     </div>
-    </div>
-</div>
-</section>
-<section aria-label="Links" class="ui segment">
-    <h2 class="ui small header">{{_('Links')}}</h2>
-    {% set ui_links = {} %}
-    {% for key, value in data.links.items() %}
-        {% set _ = ui_links.update({key: value.replace('/api/', '/')}) %}
-    {% endfor %}
-    {%- value ui=ui_links, component="sidebar_links" -%}
+  </div>
 </section>
 
 <section aria-label="API" class="ui segment">
-    <h2 class="ui small header">{{_('API')}} {{_('Links')}}</h2>
-    {%- value ui=data.links, component="sidebar_links" -%}
+  <h2 class="ui small header">{{_('API')}} {{_('Links')}}</h2>
+  {%- value ui=data.links, component="sidebar_links" -%}
 </section>
```

#### html2text {}

```diff
@@ -1,12 +1,8 @@
 
 ***** {{_('Export')}} *****
 JSON
 JSON
 Export
 
-***** {{_('Links')}} *****
-{% set ui_links = {} %} {% for key, value in data.links.items() %} {% set _ =
-ui_links.update({key: value.replace('/api/', '/')}) %} {% endfor %} {%- value
-ui=ui_links, component="sidebar_links" -%}
 ***** {{_('API')}} {{_('Links')}} *****
 {%- value ui=data.links, component="sidebar_links" -%}
```

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -8,8 +8,8 @@
 In the sample-component.js you can define your own javascript functions etc for your custom component.
 Then import the file here
 
 import "./sample-component.js"
 */
 
 // This file will import the css templates for your custom components
-import "../../less/oarepo_vocabularies_ui/custom-components.less"
+import "../../less/oarepo_vocabularies_ui/custom-components.less";
```

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem.jsx` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem.jsx`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 import React from "react";
 import PropTypes from "prop-types";
 import Overridable from "react-overridable";
-
-import _get from "lodash/get";
-import _join from "lodash/join";
-import _truncate from "lodash/truncate";
 import _upperFirst from "lodash/upperFirst";
 import _toPairs from "lodash/toPairs";
 import _chunk from "lodash/chunk";
 
 import { Item, Table, Label, Grid } from "semantic-ui-react";
 import { withState, buildUID } from "react-searchkit";
 
@@ -38,15 +34,14 @@
       ))}
     </Grid>
   );
 };
 
 export const VocabularyResultsListItemComponent = ({ result, appName }) => {
   const { title_l10n: title = "No title", id, props: itemProps } = result;
-
   // TODO: serialize links->self in UI serializer and use here
   const viewLink = new URL(
     id,
     new URL(window.location.pathname, window.location.origin)
   );
   return (
     <Overridable
```

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,55 +1,63 @@
 import {
     createSearchAppInit
-} from '@js/invenio_search_ui'
+} from "@js/invenio_search_ui";
 import {
     BucketAggregationElement,
     BucketAggregationValuesElement,
-    CountElement,
     ErrorElement,
     SearchAppFacets,
     SearchAppSearchbarContainer,
     SearchFiltersToggleElement,
-    SearchAppSort
-} from '@js/oarepo_ui/search'
+    SearchAppSort,
+    SearchAppResultOptions,
+    SearchAppResults,
+    SearchAppLayout,
+    EmptyResultsElement,
+} from "@js/oarepo_ui/search";
 import {
     VocabularyResultsListItemWithState
-} from './components'
+} from "./components";
 import {
     parametrize,
     overrideStore
-} from 'react-overridable'
+} from "react-overridable";
+import React from "react";
+const appName = "OarepoVocabularies.Search";
+const SearchAppSearchbarContainerWithConfig = parametrize(
+    SearchAppSearchbarContainer, {
+        appName: appName
+    }
+);
+const ResultsListItemWithConfig = parametrize(
+    VocabularyResultsListItemWithState, {
+        appName: appName
+    }
+);
 
-const appName = 'OarepoVocabularies.Search'
-
-const SearchAppSearchbarContainerWithConfig = parametrize(SearchAppSearchbarContainer, {
-    appName: appName
-})
-const ResultsListItemWithConfig = parametrize(VocabularyResultsListItemWithState, {
-    appName: appName
-})
 // const ResultsGridItemWithConfig = parametrize(ResultsGridItemWithState, { appName: appName })
-
 export const defaultComponents = {
     [`${appName}.BucketAggregation.element`]: BucketAggregationElement,
     [`${appName}.BucketAggregationValues.element`]: BucketAggregationValuesElement,
-    [`${appName}.Count.element`]: CountElement,
-    // [`${appName}.EmptyResults.element`]: EmptyResultsElement,
+    [`${appName}.EmptyResults.element`]: EmptyResultsElement,
     [`${appName}.Error.element`]: ErrorElement,
     // [`${appName}.ResultsGrid.item`]: ResultsGridItemWithConfig,
     [`${appName}.ResultsList.item`]: ResultsListItemWithConfig,
     [`${appName}.SearchApp.facets`]: SearchAppFacets,
     [`${appName}.SearchApp.searchbarContainer`]: SearchAppSearchbarContainerWithConfig,
     [`${appName}.SearchApp.sort`]: SearchAppSort,
     [`${appName}.SearchFilters.Toggle.element`]: SearchFiltersToggleElement,
-}
 
-const overriddenComponents = overrideStore.getAll()
+    [`${appName}.SearchApp.resultOptions`]: SearchAppResultOptions,
+    [`${appName}.SearchApp.results`]: SearchAppResults,
+    [`${appName}.SearchApp.layout`]: SearchAppLayout,
+};
+const overriddenComponents = overrideStore.getAll();
 
 createSearchAppInit({
         ...defaultComponents,
         ...overriddenComponents
     },
     true,
-    'invenio-search-config',
-    true,
-)
+    "invenio-search-config",
+    true
+);
```

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next-scanner.config.js` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next-scanner.config.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/messages.po` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/messages.po` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/messages.po` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/messages.po` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/package.json` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/package.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileCatalog.js` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileCatalog.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/initCatalog.js` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/initCatalog.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/translations.pot` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/translations.pot`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies.egg-info/PKG-INFO` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 2.0.4
+Version: 2.0.5
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo vocabularies
```

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies.egg-info/SOURCES.txt` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 pyproject.toml
 setup.cfg
 setup.py
 oarepo_vocabularies/__init__.py
 oarepo_vocabularies/cli.py
 oarepo_vocabularies/config.py
 oarepo_vocabularies/ext.py
+oarepo_vocabularies/ext_config.py
 oarepo_vocabularies/fixtures.py
+oarepo_vocabularies/proxies.py
 oarepo_vocabularies/views.py
 oarepo_vocabularies.egg-info/PKG-INFO
 oarepo_vocabularies.egg-info/SOURCES.txt
 oarepo_vocabularies.egg-info/dependency_links.txt
 oarepo_vocabularies.egg-info/entry_points.txt
 oarepo_vocabularies.egg-info/requires.txt
 oarepo_vocabularies.egg-info/top_level.txt
@@ -25,16 +27,18 @@
 oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
 oarepo_vocabularies/resources/config.py
 oarepo_vocabularies/resources/records/__init__.py
 oarepo_vocabularies/resources/records/ui.py
 oarepo_vocabularies/services/__init__.py
 oarepo_vocabularies/services/config.py
 oarepo_vocabularies/services/facets.py
+oarepo_vocabularies/services/permissions.py
 oarepo_vocabularies/services/schema.py
 oarepo_vocabularies/services/search.py
+oarepo_vocabularies/services/service.py
 oarepo_vocabularies/services/ui_schema.py
 oarepo_vocabularies/services/components/__init__.py
 oarepo_vocabularies/services/components/hierarchy.py
 oarepo_vocabularies/services/custom_fields/__init__.py
 oarepo_vocabularies/services/custom_fields/hierarchy.py
 oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2
 oarepo_vocabularies/translations/__init__.py
@@ -48,22 +52,24 @@
 oarepo_vocabularies/ui/ext.py
 oarepo_vocabularies/ui/proxies.py
 oarepo_vocabularies/ui/views.py
 oarepo_vocabularies/ui/resources/__init__.py
 oarepo_vocabularies/ui/resources/components.py
 oarepo_vocabularies/ui/resources/config.py
 oarepo_vocabularies/ui/resources/resource.py
+oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/detail.html
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/main.html
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/sidebar.html
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
 oarepo_vocabularies/ui/theme/webpack.py
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
+oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem.jsx
 oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
 oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
 oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
 oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
 oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/collections/grid.overrides
```

### Comparing `oarepo-vocabularies-2.0.4/oarepo_vocabularies.egg-info/entry_points.txt` & `oarepo-vocabularies-2.0.5/oarepo_vocabularies.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.4/setup.cfg` & `oarepo-vocabularies-2.0.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-vocabularies
-version = 2.0.4
+version = 2.0.5
 description = Support for custom fields and hierarchy on Invenio vocabularies
 authors = Mirek Simek <miroslav.simek@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

