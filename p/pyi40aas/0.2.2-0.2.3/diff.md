# Comparing `tmp/pyi40aas-0.2.2.tar.gz` & `tmp/pyi40aas-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyi40aas-0.2.2.tar", last modified: Mon Feb 15 16:38:11 2021, max compression
+gzip compressed data, was "dist/pyi40aas-0.2.3.tar", last modified: Tue Jul  4 10:03:27 2023, max compression
```

## Comparing `pyi40aas-0.2.2.tar` & `pyi40aas-0.2.3.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/
--rwxrwxrwx   0 root         (0) root         (0)     1846 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/setup.py
--rw-r--r--   0 root         (0) root         (0)     8846 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/aas/
--rw-rw-rw-   0 root         (0) root         (0)      493 2020-12-09 18:43:08.000000 pyi40aas-0.2.2/aas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/aas/compliance_tool/
--rw-rw-rw-   0 root         (0) root         (0)     8221 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/compliance_tool/state_manager.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-24 13:11:26.000000 pyi40aas-0.2.2/aas/compliance_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10832 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/compliance_tool/compliance_check_aasx.py
--rw-rw-rw-   0 root         (0) root         (0)     8725 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/compliance_tool/compliance_check_xml.py
--rw-rw-rw-   0 root         (0) root         (0)    10256 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/compliance_tool/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     8952 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/compliance_tool/compliance_check_json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/aas/backend/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/backend/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24370 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/backend/couchdb.py
--rw-rw-rw-   0 root         (0) root         (0)     9455 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/backend/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/aas/examples/
--rwxrwxrwx   0 root         (0) root         (0)     7912 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/examples/tutorial_serialization_deserialization.py
--rwxrwxrwx   0 root         (0) root         (0)     5456 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/examples/tutorial_storage.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-24 13:11:26.000000 pyi40aas-0.2.2/aas/examples/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5451 2021-02-01 09:34:37.000000 pyi40aas-0.2.2/aas/examples/tutorial_backend_couchdb.py
--rwxrwxrwx   0 root         (0) root         (0)     9154 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/examples/tutorial_aasx.py
--rwxrwxrwx   0 root         (0) root         (0)     5265 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/examples/tutorial_create_simple_aas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/aas/examples/data/
--rw-rw-rw-   0 root         (0) root         (0)    40055 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/examples/data/example_aas.py
--rw-rw-rw-   0 root         (0) root         (0)    22824 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/examples/data/example_aas_missing_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)     4306 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/examples/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8178 2020-11-06 11:52:17.000000 pyi40aas-0.2.2/aas/examples/data/TestFile.pdf
--rw-rw-rw-   0 root         (0) root         (0)    12527 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/examples/data/example_aas_mandatory_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    52039 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/examples/data/_helper.py
--rw-rw-rw-   0 root         (0) root         (0)    17157 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/examples/data/example_submodel_template.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/examples/data/example_concept_description.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/aas/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    37353 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/aasx.py
--rw-rw-rw-   0 root         (0) root         (0)     4764 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/_generic.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/aas/adapter/xml/
--rw-rw-rw-   0 root         (0) root         (0)    71652 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/xml/xml_deserialization.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/xml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5826 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/xml/IEC61360.xsd
--rw-rw-rw-   0 root         (0) root         (0)    38707 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/xml/xml_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     6048 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/xml/AAS_ABAC.xsd
--rw-rw-rw-   0 root         (0) root         (0)    19366 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/xml/AAS.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/aas/adapter/json/
--rw-rw-rw-   0 root         (0) root         (0)     1228 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/json/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    43926 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/json/json_deserialization.py
--rw-rw-rw-   0 root         (0) root         (0)    25535 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/json/aasJSONSchema.json
--rw-rw-rw-   0 root         (0) root         (0)    31630 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/adapter/json/json_serialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/aas/model/
--rw-rw-rw-   0 root         (0) root         (0)      651 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/model/security.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5255 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/model/provider.py
--rw-rw-rw-   0 root         (0) root         (0)    10628 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/model/aas.py
--rw-rw-rw-   0 root         (0) root         (0)    24920 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/model/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)    10479 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/model/concept.py
--rw-rw-rw-   0 root         (0) root         (0)    54499 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/model/submodel.py
--rw-rw-rw-   0 root         (0) root         (0)    52482 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/model/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/aas/util/
--rw-rw-rw-   0 root         (0) root         (0)     5245 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/util/identification.py
--rw-rw-rw-   0 root         (0) root         (0)      135 2020-09-24 13:11:26.000000 pyi40aas-0.2.2/aas/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1246 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/aas/util/traversal.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-09-24 13:11:26.000000 pyi40aas-0.2.2/aas/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     6742 2021-02-15 16:36:21.000000 pyi40aas-0.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/pyi40aas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8846 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/pyi40aas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1761 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/pyi40aas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        4 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/pyi40aas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/pyi40aas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/pyi40aas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/pyi40aas.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       74 2021-02-15 16:38:11.000000 pyi40aas-0.2.2/pyi40aas.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1846 2023-07-04 10:03:24.000000 pyi40aas-0.2.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)     7997 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/aas/
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/aas/compliance_tool/
+-rw-rw-rw-   0 root         (0) root         (0)     8671 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/compliance_tool/state_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/compliance_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12206 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/compliance_tool/compliance_check_aasx.py
+-rw-rw-rw-   0 root         (0) root         (0)     9552 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/compliance_tool/compliance_check_xml.py
+-rw-rw-rw-   0 root         (0) root         (0)    10438 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/compliance_tool/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     9817 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/compliance_tool/compliance_check_json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/aas/backend/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/backend/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25071 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/backend/couchdb.py
+-rw-rw-rw-   0 root         (0) root         (0)     9767 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/backend/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/aas/examples/
+-rwxrwxrwx   0 root         (0) root         (0)     7912 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/tutorial_serialization_deserialization.py
+-rwxrwxrwx   0 root         (0) root         (0)     5456 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/tutorial_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5451 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/tutorial_backend_couchdb.py
+-rwxrwxrwx   0 root         (0) root         (0)     9154 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/tutorial_aasx.py
+-rwxrwxrwx   0 root         (0) root         (0)     5265 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/tutorial_create_simple_aas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/aas/examples/data/
+-rw-rw-rw-   0 root         (0) root         (0)    40743 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/data/example_aas.py
+-rw-rw-rw-   0 root         (0) root         (0)    23349 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/data/example_aas_missing_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4306 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8178 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/data/TestFile.pdf
+-rw-rw-rw-   0 root         (0) root         (0)    13280 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/data/example_aas_mandatory_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    52039 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/data/_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    17296 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/data/example_submodel_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     4403 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/examples/data/example_concept_description.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/aas/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    39102 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/aasx.py
+-rw-rw-rw-   0 root         (0) root         (0)     4764 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/_generic.py
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/aas/adapter/xml/
+-rw-rw-rw-   0 root         (0) root         (0)    72336 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/xml/xml_deserialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      879 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/xml/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5826 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/xml/IEC61360.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    38862 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/xml/xml_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     6048 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/xml/AAS_ABAC.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    19366 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/xml/AAS.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/aas/adapter/json/
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/json/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    45175 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/json/json_deserialization.py
+-rw-rw-rw-   0 root         (0) root         (0)    25535 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/json/aasJSONSchema.json
+-rw-rw-rw-   0 root         (0) root         (0)    32572 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/adapter/json/json_serialization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/aas/model/
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/model/security.py
+-rw-rw-rw-   0 root         (0) root         (0)     2723 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5920 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/model/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    10370 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/model/aas.py
+-rw-rw-rw-   0 root         (0) root         (0)    24996 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/model/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)    10644 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/model/concept.py
+-rw-rw-rw-   0 root         (0) root         (0)    52461 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/model/submodel.py
+-rw-rw-rw-   0 root         (0) root         (0)    51295 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/model/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/aas/util/
+-rw-rw-rw-   0 root         (0) root         (0)     5763 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/util/identification.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/util/traversal.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/aas/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     7285 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/NOTICE
+-rw-rw-rw-   0 root         (0) root         (0)    23611 2023-07-04 09:39:14.000000 pyi40aas-0.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/pyi40aas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7997 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/pyi40aas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1776 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/pyi40aas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/pyi40aas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/pyi40aas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/pyi40aas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/pyi40aas.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-07-04 10:03:27.000000 pyi40aas-0.2.3/pyi40aas.egg-info/requires.txt
```

### Comparing `pyi40aas-0.2.2/setup.py` & `pyi40aas-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyi40aas",
-    version="0.2.2",
+    version="0.2.3",
     author="Chair of Process Control Engineering, RWTH Aachen",
     author_email="m.thies@plt.rwth-aachen.de",
     description="An implementation of the Asset Administration Shell for Industry 4.0 systems",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.rwth-aachen.de/acplt/pyi40aas",
     packages=setuptools.find_packages(exclude=["test", "test.*"]),
```

### Comparing `pyi40aas-0.2.2/aas/compliance_tool/state_manager.py` & `pyi40aas-0.2.3/aas/compliance_tool/state_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
-This module defines a State Manager to store LogRecords for single steps in a compliance check of the compliance tool
+This module defines a :class:`~.ComplianceToolStateManager` to store `logging.LogRecords` for single steps in a
+compliance check of the compliance tool
 """
 import logging
 import enum
 import pprint
 from typing import List, Dict
 from aas.examples.data._helper import DataChecker
 
@@ -24,40 +25,42 @@
 
 
 class Step:
     """
     A step represents a single test stage in a test protocol of a ComplianceToolStateManager
 
     :ivar name: Name of the step
-    :ivar status: status of the step from type Status
+    :ivar ~.status: status of the step from type Status
     :ivar log_list: list of LogRecords which belong to this step
     """
     def __init__(self, name: str, status: Status, log_list: List[logging.LogRecord]):
         self.name = name
         self.status = status
         self.log_list = log_list
 
 
 class ComplianceToolStateManager(logging.Handler):
     """
-    "A ComplianceToolStateManager is used to create a report of a compliance check, divided into single Steps with
-    status and log. The manager provides methods to:
-    - add a new step
-    - set the step status
-    - set the step status from log
-    - add logs to a step by hand
-    - add logs to a step from a data checker
-    - be used as a logging.Handler which adds logs to the current step
-
-    example of a ComplianceTest for a schema check
-    Step 1: 'Open file'
-    Step 2: 'Read file and check if it is conform to the json syntax'
-    Step 3: 'Validate file against official json schema'
+    A ComplianceToolStateManager is used to create a report of a compliance check, divided into single
+    :class:`Steps <.Step>` with status and log. The manager provides methods to:
 
-    :ivar steps: List of steps
+        - Add a new step
+        - Set the step status
+        - Set the step status from log
+        - Add logs to a step by hand
+        - Add logs to a step from a data checker
+        - Be used as a `logging.Handler` which adds logs to the current step
+
+    Example of a ComplianceTest for a schema check:
+
+        * Step 1: `Open file`
+        * Step 2: `Read file and check if it is conform to the json syntax`
+        * Step 3: `Validate file against official json schema`
+
+    :ivar steps: List of :class:`Steps <.Step>`
     """
     def __init__(self):
         """
         steps: List of steps. Each step consist of a step name, a step status and LogRecords belong to to this step.
                The step name have to be unique in the list.
         """
         super().__init__()
@@ -78,25 +81,26 @@
         for step in self.steps:
             if status < step.status:
                 status = step.status
         return status
 
     def add_step(self, name: str) -> None:
         """
-        Adding a new step to the manager with a given name, status = NOT_EXECUTED and an empty list of records
+        Adding a new :class:`~.Step` to the manager with a given name, status = NOT_EXECUTED and an empty list of
+        records
 
-        :param name: Name of the step
+        :param name: Name of the :class:`~.Step`
         """
         self.steps.append(Step(name, Status.NOT_EXECUTED, []))
 
     def add_log_record(self, record: logging.LogRecord) -> None:
         """
-        Adds a LogRecord to the log list of the acutal step
+        Adds a `logging.LogRecord` to the log list of the actual :class:`~.Step`
 
-        :param record: LogRecord which should be added to the current step
+        :param record: `logging.LogRecord` which should be added to the current :class:`~.Step`
         """
         self.steps[-1].log_list.append(record)
 
     def set_step_status(self, status: Status) -> None:
         """
         Sets the status of the current step
 
@@ -108,19 +112,22 @@
         """
         Sets the status of the current step based on the log entries
         """
         self.steps[-1].status = Status.FAILED if len(self.steps[-1].log_list) > 0 else Status.SUCCESS
 
     def add_log_records_from_data_checker(self, data_checker: DataChecker) -> None:
         """
-        Sets the status of the current step and convert the checks to LogRecords and adds these to the current step
+        Sets the status of the current :class:`~.Step` and convert the checks to `logging.LogRecords` and adds these to
+        the current :class:`~.Step`
 
-        step: FAILED if the DataChecker consist at least one failed check otherwise SUCCESS
+        :class:`~.Step`: FAILED if the :class:`~aas.examples.data._helper.DataChecker` consist at least one failed
+        check otherwise SUCCESS
 
-        :param data_checker: DataChecker which checks should be added to the current step
+        :param data_checker: :class:`~aas.examples.data._helper.DataChecker` which checks should be added to the
+            current :class:`~.Step`
         """
         self.steps[-1].status = Status.SUCCESS if not any(True for _ in data_checker.failed_checks) else Status.FAILED
         for check in data_checker.checks:
             self.steps[-1].log_list.append(logging.LogRecord(name=__name__,
                                                              level=logging.INFO if check.result else logging.ERROR,
                                                              pathname='',
                                                              lineno=0,
@@ -131,30 +138,32 @@
                                                                          v, depth=2, width=2 ** 14, compact=True))
                                                                            for k, v in check.data.items())),
                                                              args=(),
                                                              exc_info=None))
 
     def get_error_logs_from_step(self, index: int) -> List[logging.LogRecord]:
         """
-        Returns a list of LogRecords of a step where the log level is logging.ERROR or logging.WARNING
+        Returns a list of `logging.LogRecords` of a step where the log level is `logging.ERROR` or `logging.WARNING`
 
-        :param index: step index in the step list of the manager
-        :return: List of LogRecords with log levell logging.ERROR or logging.WARNING
+        :param index: Step index in the Step list of the manager
+        :return: List of LogRecords with log level `logging.ERROR` or `logging.WARNING`
         """
         return [x for x in self.steps[index].log_list if x.levelno >= logging.WARNING]
 
     def format_step(self, index: int, verbose_level: int = 0) -> str:
         """
-        Creates a string for the step containing the status, the step name and the LogRecords if wanted
+        Creates a string for the step containing the status, the step name and the `logging.LogRecords` if wanted
 
-        :param index:  step index in the step list of the manager
+        :param index:  Step index in the step list of the manager
         :param verbose_level: Decision which kind of LogRecords should be in the string
-                              0: No LogRecords
-                              1: Only LogRecords with log level >= logging.WARNING
-                              2: All LogRecords
+
+                                - 0: No LogRecords
+                                - 1: Only LogRecords with log level >= logging.WARNING
+                                - 2: All LogRecords
+
         :return: formatted string of the step
         """
         STEP_STATUS: Dict[Status, str] = {
             Status.SUCCESS: '{:14}'.format('SUCCESS:'),
             Status.SUCCESS_WITH_WARNINGS: '{:14}'.format('WARNINGS:'),
             Status.FAILED: '{:14}'.format('FAILED:'),
             Status.NOT_EXECUTED: '{:14}'.format('NOT_EXECUTED:'),
@@ -170,26 +179,29 @@
                     if verbose_level == 1:
                         continue
                 string += '\n'+' - {:6} {}'.format(log.levelname + ':', log.getMessage())
         return string
 
     def format_state_manager(self, verbose_level: int = 0) -> str:
         """
-        Creates a report with all executed steps: containing the status, the step name and the LogRecords if wanted
+        Creates a report with all executed steps: Containing the status, the step name and the `logging.LogRecords` if
+        wanted
 
         :param verbose_level: Decision which kind of LogRecords should be in the string
-                              0: No LogRecords
-                              1: Only LogRecords with log level >= logging.WARNING
-                              2: All LogRecords
+
+                                - 0: No LogRecords
+                                - 1: Only LogRecords with log level >= logging.WARNING
+                                - 2: All LogRecords
+
         :return: formatted report
         """
         string = 'Compliance Test executed:\n'
         string += "\n".join(self.format_step(x, verbose_level) for x in range(len(self.steps)))
         return string
 
     def emit(self, record: logging.LogRecord):
         """
-        logging.Handler function for adding LogRecords from a logger to the current step
+        `logging.Handler` function for adding `logging.LogRecords` from a `logger` to the current :class:`~.Step`
 
-        :param record: LogRecord which should be added
+        :param record: `logging.LogRecord` which should be added
         """
         self.steps[-1].log_list.append(record)
```

### Comparing `pyi40aas-0.2.2/aas/compliance_tool/compliance_check_aasx.py` & `pyi40aas-0.2.3/aas/compliance_tool/compliance_check_aasx.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
 Module which offers functions to use in a confirmation tool related to AASX files
 
-check_deserialization: Checks if a AASX file can be deserialized
+:meth:`~aas.compliance_tool.compliance_check_aasx.check_deserialization`: Checks if a AASX file can be deserialized
 
-check_aas_example: Checks if a AASX file consist the data of the example data defined in
-                   aas.examples.data.example_aas.py
+:meth:`~aas.compliance_tool.compliance_check_aasx.check_aas_example`: Checks if a AASX file consist the data of the
+example data defined in aas.examples.data.example_aas.py
 
-check_aasx_files_equivalence: Checks if two AASX files have the same data regardless of their order
+:meth:`~aas.compliance_tool.compliance_check_aasx.check_aasx_files_equivalence`: Checks if two AASX files have the same
+data regardless of their order
 
-All functions reports any issues using the given StateManager by adding new steps and associated LogRecords
+All functions reports any issues using the given :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
+by adding new steps and associated LogRecords
 """
 import datetime
 import json
 import logging
 from typing import Optional, Tuple
 
 import pyecma376_2
@@ -31,22 +33,23 @@
 from .state_manager import ComplianceToolStateManager, Status
 
 
 def check_deserialization(file_path: str, state_manager: ComplianceToolStateManager,
                           file_info: Optional[str] = None) \
         -> Tuple[model.DictObjectStore, aasx.DictSupplementaryFileContainer, pyecma376_2.OPCCoreProperties]:
     """
-    Read a AASX file and reports any issues using the given StateManager
+    Read a AASX file and reports any issues using the given
+    :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
 
-    add the steps: 'Open {} file' and 'Read {} file'
+    Add the steps: `Open {} file' and 'Read {} file`
 
-    :param file_path: given file which should be deserialized
-    :param state_manager: manager to log the steps
-    :param file_info: additional information about the file for name of the steps
-    :return: returns the read object store
+    :param file_path: Given file which should be deserialized
+    :param state_manager: Manager to log the steps
+    :param file_info: Additional information about the file for name of the steps
+    :return: The read object store
     """
     logger = logging.getLogger('compliance_check')
     logger.addHandler(state_manager)
     logger.propagate = False
     logger.setLevel(logging.INFO)
 
     # create handler to get logger info
@@ -86,20 +89,22 @@
         reader.close()
 
     return obj_store, files, new_cp
 
 
 def check_aas_example(file_path: str, state_manager: ComplianceToolStateManager) -> None:
     """
-    Checks if a file contains all elements of the aas example and reports any issues using the given StateManager
+    Checks if a file contains all elements of the aas example and reports any issues using the given
+    :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
 
-    calls the check_deserialization and add the steps: 'Check if data is equal to example data'
+    Calls the :meth:`~aas.compliance_tool.compliance_check_aasx.check_deserialization` and add the steps:
+    `Check if data is equal to example data`
 
-    :param file_path: given file which should be checked
-    :param state_manager: manager to log the steps
+    :param file_path: Given file which should be checked
+    :param state_manager: :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager` to log the steps
     """
     logger = logging.getLogger('compliance_check')
     logger.addHandler(state_manager)
     logger.propagate = False
     logger.setLevel(logging.INFO)
 
     # create handler to get logger info
@@ -138,25 +143,38 @@
     cp.lastModifiedBy = "PyI40AAS Testing Framework Compliance Tool"
     cp.modified = datetime.datetime(2020, 1, 1, 0, 0, 1)
     cp.revision = "1.0"
     cp.version = "2.0.1"
     cp.title = "Test Title"
 
     checker2 = DataChecker(raise_immediately=False)
-    assert (isinstance(cp_new.created, datetime.datetime))
-    duration = cp_new.created - cp.created
-    checker2.check(duration.microseconds < 20, "created must be {}".format(cp.created), created=cp_new.created)
+    try:
+        assert(isinstance(cp_new.created, datetime.datetime))
+        checker2.check(isinstance(cp_new.created, datetime.datetime), "core property created must be of type datetime",
+                       created=type(cp_new.created))
+        duration = cp_new.created - cp.created
+        checker2.check(duration.microseconds < 20, "created must be {}".format(cp.created), created=cp_new.created)
+    except AssertionError:
+        checker2.check(isinstance(cp_new.created, datetime.datetime), "core property created must be of type datetime",
+                       created=type(cp_new.created))
+
     checker2.check(cp_new.creator == cp.creator, "creator must be {}".format(cp.creator), creator=cp_new.creator)
     checker2.check(cp_new.description == cp.description, "description must be {}".format(cp.description),
                    description=cp_new.description)
     checker2.check(cp_new.lastModifiedBy == cp.lastModifiedBy, "lastModifiedBy must be {}".format(cp.lastModifiedBy),
                    lastModifiedBy=cp_new.lastModifiedBy)
-    assert (isinstance(cp_new.modified, datetime.datetime))
-    duration = cp_new.modified - cp.modified
-    checker2.check(duration.microseconds < 20, "modified must be {}".format(cp.modified), modified=cp_new.modified)
+    try:
+        assert(isinstance(cp_new.modified, datetime.datetime))
+        checker2.check(isinstance(cp_new.modified, datetime.datetime), "modified bust be of type datetime",
+                       modified=type(cp_new.modified))
+        duration = cp_new.modified - cp.modified
+        checker2.check(duration.microseconds < 20, "modified must be {}".format(cp.modified), modified=cp_new.modified)
+    except AssertionError:
+        checker2.check(isinstance(cp_new.modified, datetime.datetime), "modified bust be of type datetime",
+                       modified=type(cp_new.modified))
     checker2.check(cp_new.revision == cp.revision, "revision must be {}".format(cp.revision), revision=cp_new.revision)
     checker2.check(cp_new.version == cp.version, "version must be {}".format(cp.version), version=cp_new.version)
     checker2.check(cp_new.title == cp.title, "title must be {}".format(cp.title), title=cp_new.title)
 
     # Check if file in file object is the same
     list_of_id_shorts = ["ExampleSubmodelCollectionUnordered", "ExampleFile"]
     obj = example_data.get_identifiable(model.Identifier("https://acplt.org/Test_Submodel", model.IdentifierType.IRI))
@@ -180,21 +198,23 @@
         state_manager.set_step_status(Status.FAILED)
     else:
         state_manager.set_step_status(Status.SUCCESS)
 
 
 def check_aasx_files_equivalence(file_path_1: str, file_path_2: str, state_manager: ComplianceToolStateManager) -> None:
     """
-    Checks if two aasx files contain the same elements in any order and reports any issues using the given StateManager
+    Checks if two aasx files contain the same elements in any order and reports any issues using the given
+    :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
 
-    calls the check_deserialization for ech file and add the steps: 'Check if data in files are equal'
+    calls the :meth:`~aas.compliance_tool.compliance_check_aasx.check_deserialization` for each file and add the steps:
+    `Check if data in files are equal`
 
-    :param file_path_1: given first file which should be checked
-    :param file_path_2: given second file which should be checked
-    :param state_manager: manager to log the steps
+    :param file_path_1: Given first file which should be checked
+    :param file_path_2: Given second file which should be checked
+    :param state_manager: :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager` to log the steps
     """
     logger = logging.getLogger('compliance_check')
     logger.addHandler(state_manager)
     logger.propagate = False
     logger.setLevel(logging.INFO)
 
     obj_store_1, files_1, cp_1 = check_deserialization(file_path_1, state_manager, 'first')
```

### Comparing `pyi40aas-0.2.2/aas/compliance_tool/compliance_check_xml.py` & `pyi40aas-0.2.3/aas/compliance_tool/compliance_check_xml.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
 Module which offers functions to use in a confirmation tool related to xml files
 
-check_schema: Checks if a xml file is conform to official JSON schema as defined in the 'Details of the Asset
-              Administration Shell' specification of Plattform Industrie 4.0
+:meth:`~aas.compliance_tool.compliance_check_xml.check_schema`: Checks if a xml file is conform to official JSON schema
+as defined in the 'Details of the Asset Administration Shell' specification of Plattform Industrie 4.0
 
-check_deserialization: Checks if a xml file can be deserialized
+:meth:`~aas.compliance_tool.compliance_check_xml.check_deserialization`: Checks if a xml file can be deserialized
 
-check_aas_example: Checks if a xml file consist the data of the example data defined in
-                   aas.examples.data.example_aas.py
+:meth:`~aas.compliance_tool.compliance_check_xml.check_aas_example`: Checks if a xml file consist the data of the
+example data defined in aas.examples.data.example_aas.py
 
-check_xml_files_equivalence: Checks if two xml files have the same data regardless of their order
+:meth:`~aas.compliance_tool.compliance_check_xml.check_xml_files_equivalence`: Checks if two xml files have the same
+data regardless of their order
 
-All functions reports any issues using the given StateManager by adding new steps and associated LogRecords
+All functions reports any issues using the given :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
+by adding new steps and associated LogRecords
 """
 
 from lxml import etree  # type: ignore
 import logging
 from typing import Optional
 
 from .. import model
@@ -30,21 +32,22 @@
 from ..examples.data import example_aas, create_example
 from ..examples.data._helper import AASDataChecker
 from .state_manager import ComplianceToolStateManager, Status
 
 
 def check_schema(file_path: str, state_manager: ComplianceToolStateManager) -> None:
     """
-    checks a given file against the official xml schema and reports any issues using the given StateManager
+    Checks a given file against the official xml schema and reports any issues using the given
+    :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
 
-    add the steps: 'Open file', 'Read file and check if it is conform to the xml syntax' and 'Validate file against
-    official xml schema'
+    Add the steps: `Open file`, `Read file`, `Check if it is conform to the xml syntax` and `Validate file against
+    official xml schema`
 
-    :param file_path: path to the file which should be checked
-    :param state_manager: manager to log the steps
+    :param file_path: Path to the file which should be checked
+    :param state_manager: :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager` to log the steps
     """
     logger = logging.getLogger('compliance_check')
     logger.addHandler(state_manager)
     logger.propagate = False
     logger.setLevel(logging.INFO)
 
     state_manager.add_step('Open file')
@@ -91,22 +94,23 @@
     state_manager.set_step_status(Status.SUCCESS)
     return
 
 
 def check_deserialization(file_path: str, state_manager: ComplianceToolStateManager,
                           file_info: Optional[str] = None) -> model.DictObjectStore:
     """
-    Deserializes a XML AAS file and reports any issues using the given StateManager
+    Deserializes a XML AAS file and reports any issues using the given
+    :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
 
-    add the steps: 'Open {} file' and 'Read {} file and check if it is conform to the xml schema'
+    Add the steps: `Open {} file` and `Read {} file` and `Check if it is conform to the xml schema`
 
-    :param file_path: given file which should be deserialized
-    :param state_manager: manager to log the steps
-    :param file_info: additional information about the file for name of the steps
-    :return: returns the deserialized object store
+    :param file_path: Given file which should be deserialized
+    :param state_manager: :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager` to log the steps
+    :param file_info: Additional information about the file for name of the steps
+    :return: The deserialized object store
     """
     logger = logging.getLogger('compliance_check')
     logger.addHandler(state_manager)
     logger.propagate = False
     logger.setLevel(logging.INFO)
 
     # create handler to get logger info
@@ -144,20 +148,22 @@
     state_manager.set_step_status_from_log()
 
     return obj_store
 
 
 def check_aas_example(file_path: str, state_manager: ComplianceToolStateManager) -> None:
     """
-    Checks if a file contains all elements of the aas example and reports any issues using the given StateManager
+    Checks if a file contains all elements of the aas example and reports any issues using the given
+    :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
 
-    calls the check_deserialization and add the steps: 'Check if data is equal to example data'
+    Calls the :meth:`~aas.compliance_tool.compliance_check_xml.check_deserialization` and add the steps: `Check if data
+    is equal to example data`
 
-    :param file_path: given file which should be checked
-    :param state_manager: manager to log the steps
+    :param file_path: Given file which should be checked
+    :param state_manager: :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager` to log the steps
     """
     # create handler to get logger info
     logger_example = logging.getLogger(example_aas.__name__)
     logger_example.addHandler(state_manager)
     logger_example.propagate = False
     logger_example.setLevel(logging.INFO)
 
@@ -174,21 +180,23 @@
     checker.check_object_store(obj_store, create_example())
 
     state_manager.add_log_records_from_data_checker(checker)
 
 
 def check_xml_files_equivalence(file_path_1: str, file_path_2: str, state_manager: ComplianceToolStateManager) -> None:
     """
-    Checks if two xml files contain the same elements in any order and reports any issues using the given StateManager
+    Checks if two xml files contain the same elements in any order and reports any issues using the given
+    :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
 
-    calls the check_deserialization for ech file and add the steps: 'Check if data in files are equal'
+    Calls the :meth:`~aas.compliance_tool.compliance_check_xml.check_deserialization` for each file and add the steps:
+    `Check if data in files are equal`
 
-    :param file_path_1: given first file which should be checked
-    :param file_path_2: given second file which should be checked
-    :param state_manager: manager to log the steps
+    :param file_path_1: Given first file which should be checked
+    :param file_path_2: Given second file which should be checked
+    :param state_manager: :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager` to log the steps
     """
     logger = logging.getLogger('compliance_check')
     logger.addHandler(state_manager)
     logger.propagate = False
     logger.setLevel(logging.INFO)
 
     obj_store_1 = check_deserialization(file_path_1, state_manager, 'first')
```

### Comparing `pyi40aas-0.2.2/aas/compliance_tool/cli.py` & `pyi40aas-0.2.3/aas/compliance_tool/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 from aas.compliance_tool import compliance_check_xml as compliance_tool_xml
 from aas.compliance_tool import compliance_check_aasx as compliance_tool_aasx
 from aas.adapter.json import write_aas_json_file
 from aas.examples.data import create_example, create_example_aas_binding, TEST_PDF_FILE
 from aas.compliance_tool.state_manager import ComplianceToolStateManager, Status
 
 
-def main():
+def parse_cli_arguments() -> argparse.ArgumentParser:
+    """
+    This function returns the argument-parser for the cli
+    """
     parser = argparse.ArgumentParser(
         prog='compliance_tool',
         description='Compliance tool for creating and checking json and xml files in compliance with "Details of the '
                     'Asset Administration Shell" specification of Plattform Industrie 4.0. \n\n'
                     'This tool has five features: \n'
                     '1. create a xml or json file or an AASX file using xml or json files with example aas elements\n'
                     '2. check if a given xml or json file is compliant with the official json or xml aas schema and '
@@ -77,15 +80,19 @@
                                                 "detailed success information", action='count', default=0)
     parser.add_argument('-q', '--quite', help="no information output if successful", action='store_true')
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument('--json', help="Use AAS json format when checking or creating files", action='store_true')
     group.add_argument('--xml', help="Use AAS xml format when checking or creating files", action='store_true')
     parser.add_argument('-l', '--logfile', help="Log file to be created in addition to output to stdout", default=None)
     parser.add_argument('--aasx', help="Create or read AASX files", action='store_true')
+    return parser
+
 
+def main():
+    parser = parse_cli_arguments()
     args = parser.parse_args()
 
     # Todo try to find out in which format the file is if not --json or --xml
 
     manager = ComplianceToolStateManager()
     logger = logging.getLogger(__name__)
     logger.propagate = False
```

### Comparing `pyi40aas-0.2.2/aas/compliance_tool/compliance_check_json.py` & `pyi40aas-0.2.3/aas/compliance_tool/compliance_check_json.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,46 +4,49 @@
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
 Module which offers functions to use in a confirmation tool related to json files
 
-check_schema: Checks if a json file is conform to official JSON schema as defined in the 'Details of the Asset
-              Administration Shell' specification of Plattform Industrie 4.0
+:meth:`~aas.compliance_tool.compliance_check_json.check_schema`: Checks if a json file is conform to official JSON
+schema as defined in the 'Details of the Asset Administration Shell' specification of Plattform Industrie 4.0
 
-check_deserialization: Checks if a json file can be deserialized
+:meth:`~aas.compliance_tool.compliance_check_json.check_deserialization`: Checks if a json file can be deserialized
 
-check_aas_example: Checks if a json file consist the data of the example data defined in
-                   aas.examples.data.example_aas.py
+:meth:`~aas.compliance_tool.compliance_check_json.check_aas_example`: Checks if a json file consist the data of the
+example data defined in aas.examples.data.example_aas.py
 
-check_json_files_equivalence: Checks if two json files have the same data regardless of their order
+:meth:`~aas.compliance_tool.compliance_check_json.check_json_files_equivalence`: Checks if two json files have the
+same data regardless of their order
 
-All functions reports any issues using the given StateManager by adding new steps and associated LogRecords
+All functions reports any issues using the given :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
+by adding new steps and associated LogRecords
 """
 import json
 import logging
 from typing import Optional
 
 from .. import model
 from ..adapter.json import json_deserialization, JSON_SCHEMA_FILE
 from ..examples.data import example_aas, create_example
 from ..examples.data._helper import AASDataChecker
 from .state_manager import ComplianceToolStateManager, Status
 
 
 def check_schema(file_path: str, state_manager: ComplianceToolStateManager) -> None:
     """
-    checks a given file against the official json schema and reports any issues using the given StateManager
+    Checks a given file against the official json schema and reports any issues using the given
+    :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
 
-    add the steps: 'Open file', 'Read file and check if it is conform to the json syntax' and 'Validate file against
-    official json schema'
+    Add the steps: `Open file`, `Read file and check if it is conform to the json syntax` and `Validate file against
+    official json schema`
 
-    :param file_path: path to the file which should be checked
-    :param state_manager: manager to log the steps
+    :param file_path: Path to the file which should be checked
+    :param state_manager: :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager` to log the steps
     """
     logger = logging.getLogger('compliance_check')
     logger.addHandler(state_manager)
     logger.propagate = False
     logger.setLevel(logging.INFO)
 
     state_manager.add_step('Open file')
@@ -95,22 +98,23 @@
     state_manager.set_step_status(Status.SUCCESS)
     return
 
 
 def check_deserialization(file_path: str, state_manager: ComplianceToolStateManager,
                           file_info: Optional[str] = None) -> model.DictObjectStore:
     """
-    Deserializes a JSON AAS file and reports any issues using the given StateManager
+    Deserializes a JSON AAS file and reports any issues using the given
+    :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
 
-    add the steps: 'Open {} file' and 'Read {} file and check if it is conform to the json schema'
+    Add the steps: `Open {} file` and `Read {} file` and `check if it is conform to the json schema`
 
-    :param file_path: given file which should be deserialized
-    :param state_manager: manager to log the steps
-    :param file_info: additional information about the file for name of the steps
-    :return: returns the deserialized object store
+    :param file_path: Given file which should be deserialized
+    :param state_manager: :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager` to log the steps
+    :param file_info: Additional information about the file for name of the steps
+    :return: The deserialized :class:`~aas.model.provider.DictObjectStore`
     """
     logger = logging.getLogger('compliance_check')
     logger.addHandler(state_manager)
     logger.propagate = False
     logger.setLevel(logging.INFO)
 
     # create handler to get logger info
@@ -148,20 +152,22 @@
     state_manager.set_step_status_from_log()
 
     return obj_store
 
 
 def check_aas_example(file_path: str, state_manager: ComplianceToolStateManager) -> None:
     """
-    Checks if a file contains all elements of the aas example and reports any issues using the given StateManager
+    Checks if a file contains all elements of the aas example and reports any issues using the given
+    :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
 
-    calls the check_deserialization and add the steps: 'Check if data is equal to example data'
+    Calls the :meth:`~aas.compliance_tool.compliance_check_json.check_deserialization` and add the steps:
+    `Check if data is equal to example data`
 
-    :param file_path: given file which should be checked
-    :param state_manager: manager to log the steps
+    :param file_path: Given file which should be checked
+    :param state_manager: :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager` to log the steps
     """
     # create handler to get logger info
     logger_example = logging.getLogger(example_aas.__name__)
     logger_example.addHandler(state_manager)
     logger_example.propagate = False
     logger_example.setLevel(logging.INFO)
 
@@ -178,21 +184,23 @@
     checker.check_object_store(obj_store, create_example())
 
     state_manager.add_log_records_from_data_checker(checker)
 
 
 def check_json_files_equivalence(file_path_1: str, file_path_2: str, state_manager: ComplianceToolStateManager) -> None:
     """
-    Checks if two json files contain the same elements in any order and reports any issues using the given StateManager
+    Checks if two json files contain the same elements in any order and reports any issues using the given
+    :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager`
 
-    calls the check_deserialization for ech file and add the steps: 'Check if data in files are equal'
+    Calls the :meth:`~aas.compliance_tool.compliance_check_json.check_deserialization` for ech file and add the steps:
+    `Check if data in files are equal`
 
-    :param file_path_1: given first file which should be checked
-    :param file_path_2: given second file which should be checked
-    :param state_manager: manager to log the steps
+    :param file_path_1: Given first file which should be checked
+    :param file_path_2: Given second file which should be checked
+    :param state_manager: :class:`~aas.compliance_tool.state_manager.ComplianceToolStateManager` to log the steps
     """
     logger = logging.getLogger('compliance_check')
     logger.addHandler(state_manager)
     logger.propagate = False
     logger.setLevel(logging.INFO)
 
     obj_store_1 = check_deserialization(file_path_1, state_manager, 'first')
```

### Comparing `pyi40aas-0.2.2/aas/backend/couchdb.py` & `pyi40aas-0.2.3/aas/backend/couchdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
-Todo: Add module docstring
+This module adds the functionality of storing and retrieving :class:`~aas.model.base.Identifiable` objects in a CouchDB.
+
+The :class:`~.CouchDBBackend` takes care of updating and committing objects from and to the CouchDB, while the
+:class:`~CouchDBObjectStore` handles adding, deleting and otherwise managing the AAS objects in a specific CouchDB.
 """
 import threading
 import weakref
 from typing import List, Dict, Any, Optional, Iterator, Iterable, Union, Tuple
 import urllib.parse
 import logging
 import json
@@ -28,16 +31,16 @@
 _http_pool_manager = urllib3.PoolManager()
 
 
 class CouchDBBackend(backends.Backend):
     """
     This Backend stores each Identifiable object as a single JSON document in the configured CouchDB database. Each
     document's id is build from the object's identifier using the pattern {idtype}-{idvalue}; the document's contents
-    comprise a single property "data", containing the JSON serialization of the PyI40AAS object. The aas.adapter.json
-    package is used for serialization and deserialization of objects.
+    comprise a single property "data", containing the JSON serialization of the PyI40AAS object. The
+    :ref:`adapter.json <adapter.json.__init__>` package is used for serialization and deserialization of objects.
     """
     @classmethod
     def update_object(cls,
                       updated_object: model.Referable,
                       store_object: model.Referable,
                       relative_path: List[str]) -> None:
 
@@ -172,16 +175,18 @@
 # Note: The HTTPPasswordMgr is not thread safe during writing, should be thread safe for reading only.
 
 
 def register_credentials(url: str, username: str, password: str):
     """
     Register the credentials of a CouchDB server to the global credentials store
 
-    Warning: Do not use this function, while other threads may be accessing the credentials via the CouchDBObjectStore
-             or update or commit functions of model.base.Referable objects!
+    .. Warning::
+
+        Do not use this function, while other threads may be accessing the credentials via the
+        :class:`~.CouchDBObjectStore` or update or commit functions of :class:`~.aas.model.base.Referable` objects!
 
     :param url: Toplevel URL
     :param username: Username to that CouchDB instance
     :param password: Password to the Username
     """
     url_parts = urllib.parse.urlparse(url)
     _credentials_store[url_parts.scheme + url_parts.netloc] = (username, password)
@@ -222,15 +227,16 @@
     """
     with _revision_store_lock:
         del _revision_store[url]
 
 
 class CouchDBObjectStore(model.AbstractObjectStore):
     """
-    An ObjectStore implementation for Identifiable PyI40AAS objects backed by a CouchDB database server.
+    An ObjectStore implementation for :class:`~aas.model.base.Identifiable` PyI40AAS objects backed by a CouchDB
+    database server.
 
     All methods of the `CouchDBObjectStore` are blocking, i.e. they stop the current thread's execution until they
     receive a response from the CouchDB server (or encounter a timeout). However, the `CouchDBObjectStore` objects are
     thread-safe, as long as no CouchDB credentials are added (via `register_credentials()`) during transactions.
     """
     def __init__(self, url: str, database: str):
         """
@@ -272,17 +278,18 @@
 
         # Create database
         logger.info("Creating CouchDB database %s/%s ...", self.url, self.database_name)
         CouchDBBackend.do_request("{}/{}".format(self.url, self.database_name), 'PUT')
 
     def get_identifiable(self, identifier: Union[str, model.Identifier]) -> model.Identifiable:
         """
-        Retrieve an AAS object from the CouchDB by its Identifier
+        Retrieve an AAS object from the CouchDB by its :class:`~aas.model.base.Identifier`
 
-        If the identifier is a string, it is assumed that the string is a correct couchdb-ID-string (according to the
+        If the :class:`~.aas.model.base.Identifier` is a string, it is assumed that the string is a correct
+        couchdb-ID-string (according to the
         internal conversion rules, see CouchDBObjectStore._transform_id() )
 
         :raises KeyError: If no such object is stored in the database
         :raises CouchDBError: If error occur during the request to the CouchDB server (see `_do_request()` for details)
         """
         if isinstance(identifier, model.Identifier):
             identifier = self._transform_id(identifier, False)
@@ -346,22 +353,24 @@
             raise
         with self._object_cache_lock:
             self._object_cache[x.identification] = x
         self.generate_source(x)  # Set the source of the object
 
     def discard(self, x: model.Identifiable, safe_delete=False) -> None:
         """
-        Delete an Identifiable AAS object from the CouchDB database
+        Delete an :class:`~aas.model.base.Identifiable` AAS object from the CouchDB database
 
         :param x: The object to be deleted
-        :param safe_delete: If True, only delete the object if it has not been modified in the database in comparison to
+        :param safe_delete: If `True`, only delete the object if it has not been modified in the database in comparison
+                            to
                             the provided revision. This uses the CouchDB revision token and thus only works with
                             CouchDBIdentifiable objects retrieved from this database.
         :raises KeyError: If the object does not exist in the database
-        :raises CouchDBConflictError: If safe_delete is true and the object has been modified or deleted in the database
+        :raises CouchDBConflictError: If safe_delete is `True` and the object has been modified or deleted in the
+            database
         :raises CouchDBError: If error occur during the request to the CouchDB server (see `_do_request()` for details)
         """
         logger.debug("Deleting object %s from CouchDB database ...", repr(x))
         rev = get_couchdb_revision("{}/{}/{}".format(self.url,
                                                      self.database_name,
                                                      self._transform_id(x.identification)))
 
@@ -400,19 +409,19 @@
                                                   self._transform_id(x.identification)))
         with self._object_cache_lock:
             del self._object_cache[x.identification]
         x.source = ""
 
     def __contains__(self, x: object) -> bool:
         """
-        Check if an object with the given Identifier or the same Identifier as the given object is contained in the
-        CouchDB database
+        Check if an object with the given :class:`~aas.model.base.Identifier` or the same
+        :class:`~aas.model.base.Identifier` as the given object is contained in the CouchDB database
 
-        :param x: AAS object Identifier or Identifiable AAS object
-        :return: True if such an object exists in the database, False otherwise
+        :param x: AAS object :class:`~aas.model.base.Identifier` or :class:`~aas.model.base.Identifiable` AAS object
+        :return: `True` if such an object exists in the database, `False` otherwise
         :raises CouchDBError: If error occur during the request to the CouchDB server (see `_do_request()` for details)
         """
         if isinstance(x, model.Identifier):
             identifier = x
         elif isinstance(x, model.Identifiable):
             identifier = x.identification
         else:
@@ -436,15 +445,15 @@
         """
         logger.debug("Fetching number of documents from database ...")
         data = CouchDBBackend.do_request("{}/{}".format(self.url, self.database_name))
         return data['doc_count']
 
     def __iter__(self) -> Iterator[model.Identifiable]:
         """
-        Iterate all Identifiables in the CouchDB database.
+        Iterate all :class:`~aas.model.base.Identifiable` objects in the CouchDB database.
 
         This method returns a lazy iterator, containing only a list of all identifiers in the database and retrieving
         the identifiable objects on the fly.
 
         :raises CouchDBError: If error occur during fetching the list of objects from the CouchDB server (see
                               `_do_request()` for details)
         """
@@ -473,15 +482,15 @@
         result = "{}-{}".format(identifier.id_type.name, identifier.id)
         if url_quote:
             result = urllib.parse.quote(result, safe='')
         return result
 
     def generate_source(self, identifiable: model.Identifiable):
         """
-        Generates the source string for an Identifiable object that is backed by the Couchdb
+        Generates the source string for an :class:`~aas.model.base.Identifiable` object that is backed by the Couchdb
 
         :param identifiable: Identifiable object
         """
         source: str = self.url.replace("https://", "couchdbs://").replace("http://", "couchdb://")
         source += "/" + self.database_name + "/" + self._transform_id(identifiable.identification)
         identifiable.source = source
```

### Comparing `pyi40aas-0.2.2/aas/backend/backends.py` & `pyi40aas-0.2.3/aas/backend/backends.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,56 +2,62 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
-This module provides a registry and and abstract base class for Backends. A backend is a class that allows to
+This module provides a registry and and abstract base class for Backends. A :class:`~.Backend` is a class that allows to
 synchronize Referable AAS objects or their included data with external data sources such as a remote API or a local
 source for real time data. Each backend provides access to one kind of data source.
 
-The data source of an individual object is specified as an URI in its `source` attribute. The schema part of that URI
-defines the type of data source and, in consequence, the backend class to use for synchronizing this object.
+The data source of an individual object is specified as an URI in its :attr:`~aas.model.base.Referable.source`
+attribute. The schema part of that URI defines the type of data source and, in consequence, the backend class to use
+for synchronizing this object.
 
 Custom backends for additional types of data sources can be implemented by subclassing the `Backend` class and
-implementing the `commit_object()` and `update_object()` class methods. These are used internally by the objects'
-`update()` and `commit()` methods when the backend is applicable for the relevant source URI. Then, the Backend class
-needs to be registered to handle update/commit requests for a specific URI schema, using `register_backend()`.
+implementing the :meth:`~.Backend.commit_object` and :meth:`~.Backend.update_object` class methods. These are used
+internally by the objects' :meth:`~aas.model.base.Referable.update` and :meth:`~aas.model.base.Referable.commit`
+methods when the backend is applicable for the relevant source URI. Then, the Backend class
+needs to be registered to handle update/commit requests for a specific URI schema, using
+:meth:`~aas.backend.backends.register_backend`.
+
 """
 import abc
 import re
 from typing import List, Dict, Type, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from ..model import Referable
 
 
 class Backend(metaclass=abc.ABCMeta):
     """
     Abstract base class for all Backend classes.
 
     Each Backend class is typically capable of synchronizing (updating/committing) objects with a type of external data
-    source, identifed by one or more source URI schemas. Custom backends for custom source URI schemas should inherit
-    from this class and be registered via `register_backend` to be used by Referable object's update() and commit()
-    methods when required.
+    source, identified by one or more source URI schemas. Custom backends for custom source URI schemas should inherit
+    from this class and be registered via :meth:`~aas.backend.backends.register_backend`. to be used by Referable
+    object's :meth:`~aas.model.base.Referable.update` and :meth:`~aas.model.base.Referable.commit` methods when
+    required.
     """
 
     @classmethod
     @abc.abstractmethod
     def commit_object(cls,
                       committed_object: "Referable",
                       store_object: "Referable",
                       relative_path: List[str]) -> None:
         """
         Function (class method) to be called when an object shall be committed (local changes pushed to the external
         data source) via this backend implementation.
 
-        It is automatically called by the `Referable.commit()` implementation, when the source URI of the object or
-        the source URI one of its ancestors in the AAS object containment hierarchy include an URI schema for which this
+        It is automatically called by the :meth:`~aas.model.base.Referable.commit` implementation, when the source
+        URI of the object or the source URI one of its ancestors in the AAS object containment hierarchy include an
+        URI schema for which this
         backend has been registered. Both of the objects are passed to this function: the one which shall be committed
         (`committed_object`) and its ancestor with the relevant source URI (`store_object`). They may be the same, the
         committed object has a source with the relevant schema itself. Additionally, the `relative_path` from the
         `store_object` down to the `committed_object` is provided.
 
         The backend MUST ensure to commit all local changes of at least the `committed_object` and all objects contained
         within it (if any) to the data source. It MAY additionally commit changes to other objects (i.e. the
@@ -78,15 +84,16 @@
                       updated_object: "Referable",
                       store_object: "Referable",
                       relative_path: List[str]) -> None:
         """
         Function (class method) to be called when an object shall be updated (local object updated with changes from the
         external data source) via this backend implementation.
 
-        It is automatically called by the `Referable.update()` implementation, when the source URI of the object or
+        It is automatically called by the :meth:`~aas.model.base.Referable.update` implementation, when the source URI
+        of the object or
         the source URI one of its ancestors in the AAS object containment hierarchy include an URI schema for which this
         backend has been registered. Both of the objects are passed to this function: the one which shall be update
         (`updated_object`) and its ancestor with the relevant source URI (`store_object`). They may be the same, the
         updated object has a source with the relevant schema itself. Additionally, the `relative_path` from the
         `store_object` down to the `updated_object` is provided.
 
         The backend MUST ensure to update at least the `updated_object` and all objects contained within it (if any)
@@ -131,19 +138,19 @@
 
 
 RE_URI_SCHEME = re.compile(r"^([a-zA-Z][a-zA-Z+\-\.]*):")
 
 
 def get_backend(url: str) -> Type[Backend]:
     """
-    Internal function to retrieve the Backend implementation for the external data source indentified by the given `url`
+    Internal function to retrieve the Backend implementation for the external data source identified by the given `url`
     via the url's schema.
 
     :param url: External data source URI to find an appropriate Backend implementation for
-    :return: A Backend class, capable of updating/commiting from/to the external data source
+    :return: A Backend class, capable of updating/committing from/to the external data source
     :raises UnknownBackendException: When no backend is available for that url
     """
     # TODO handle multiple backends per scheme
     scheme_match = RE_URI_SCHEME.match(url)
     if not scheme_match:
         raise ValueError("{} is not a valid URL with URI scheme.".format(url))
     scheme = scheme_match[1]
```

### Comparing `pyi40aas-0.2.2/aas/examples/tutorial_serialization_deserialization.py` & `pyi40aas-0.2.3/aas/examples/tutorial_serialization_deserialization.py`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/examples/tutorial_storage.py` & `pyi40aas-0.2.3/aas/examples/tutorial_storage.py`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/examples/tutorial_backend_couchdb.py` & `pyi40aas-0.2.3/aas/examples/tutorial_backend_couchdb.py`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/examples/tutorial_aasx.py` & `pyi40aas-0.2.3/aas/examples/tutorial_aasx.py`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/examples/tutorial_create_simple_aas.py` & `pyi40aas-0.2.3/aas/examples/tutorial_create_simple_aas.py`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/examples/data/example_aas.py` & `pyi40aas-0.2.3/aas/examples/data/example_aas.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,52 +2,56 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
-Module for the creation of an object store with an example asset administration shell, related asset and example
+Module for the creation of an :class:`ObjectStore <aas.model.provider.DictObjectStore>` with an example asset
+administration shell, related asset and example
 submodels and a concept dictionary containing an example concept description
 
-To get this object store use the function 'create_full_example'. If you want to get single example objects or want to
-get more information use the other functions.
+To get this object store use the function :meth:`~aas.examples.data.example_aas.create_full_example`.
+If you want to get single example objects or want to get more information use the other functions.
 """
 import logging
 
 from ._helper import AASDataChecker
 from ... import model
 
 logger = logging.getLogger(__name__)
 
 
 def create_full_example() -> model.DictObjectStore:
     """
-    creates an object store which is filled with an example asset, submodel, concept description and asset
-    administration shell using the function of this module
+    Creates an object store which is filled with an example :class:`~aas.model.aas.Asset`,
+    :class:`~aas.model.submodel.Submodel`, :class:`~aas.model.concept.ConceptDescription` and
+    :class:`~aas.model.aas.AssetAdministrationShell` using the functions of this module
 
-    :return: object store
+    :return: :class:`~aas.model.provider.DictObjectStore`
     """
     obj_store: model.DictObjectStore[model.Identifiable] = model.DictObjectStore()
     obj_store.add(create_example_asset_identification_submodel())
     obj_store.add(create_example_bill_of_material_submodel())
     obj_store.add(create_example_asset())
     obj_store.add(create_example_submodel())
     obj_store.add(create_example_concept_description())
     obj_store.add(create_example_asset_administration_shell(create_example_concept_dictionary()))
     return obj_store
 
 
 def create_example_asset_identification_submodel() -> model.Submodel:
     """
-    creates a submodel for the identification of the example asset containing two property elements according to
+    Creates a :class:`~aas.model.submodel.Submodel` for the identification of the example :class:`~aas.model.aas.Asset`
+    containing two :class:`~aas.model.submodel.Property` elements according to
     'Verwaltungssschale in der Praxis'
     https://www.plattform-i40.de/PI40/Redaktion/DE/Downloads/Publikation/2019-verwaltungsschale-in-der-praxis.html
 
     :return: example asset identification submodel
+
     """
     qualifier = model.Qualifier(
         type_='http://acplt.org/Qualifier/ExampleQualifier',
         value_type=model.datatypes.Int,
         value=100,
         value_id=model.Reference((model.Key(type_=model.KeyElements.GLOBAL_REFERENCE,
                                             local=False,
@@ -133,15 +137,16 @@
         qualifier=None,
         kind=model.ModelingKind.INSTANCE)
     return identification_submodel
 
 
 def create_example_bill_of_material_submodel() -> model.Submodel:
     """
-    creates a submodel for the bill of material of the example asset containing two entities one co-managed and one
+    Creates a :class:`~aas.model.submodel.Submodel` for the bill of material of the example
+    :class:`~aas.model.aas.Asset` containing two entities one co-managed and one
     self-managed
 
     :return: example bill of material submodel
     """
     submodel_element_property = model.Property(
         id_short='ExampleProperty',
         value_type=model.datatypes.String,
@@ -250,16 +255,16 @@
         qualifier=None,
         kind=model.ModelingKind.INSTANCE)
     return bill_of_material
 
 
 def create_example_asset() -> model.Asset:
     """
-    creates an example asset which holds references to the example asset identification submodel and bill of material
-    submodel
+    Creates an example :class:`~aas.model.aas.Asset` which holds references to the example asset identification
+    submodel and bill of material submodel
 
     :return: example asset
     """
     asset = model.Asset(
         kind=model.AssetKind.INSTANCE,
         identification=model.Identifier(id_='https://acplt.org/Test_Asset',
                                         id_type=model.IdentifierType.IRI),
@@ -283,15 +288,16 @@
                                                        id_type=model.KeyType.IRI),),
                                             model.Submodel))
     return asset
 
 
 def create_example_submodel() -> model.Submodel:
     """
-    creates an example submodel containing all kind of SubmodelElement objects
+    Creates an example :class:`~aas.model.submodel.Submodel` containing all kind of
+    :class:`~aas.model.submodel.SubmodelElement` objects
 
     :return: example submodel
     """
     submodel_element_property = model.Property(
         id_short='ExampleProperty',
         value_type=model.datatypes.String,
         value='exampleValue',
@@ -587,15 +593,15 @@
         qualifier=None,
         kind=model.ModelingKind.INSTANCE)
     return submodel
 
 
 def create_example_concept_description() -> model.ConceptDescription:
     """
-    creates an example concept description
+    Creates an example :class:`~aas.model.concept.ConceptDescription`
 
     :return: example concept description
     """
     concept_description = model.ConceptDescription(
         identification=model.Identifier(id_='https://acplt.org/Test_ConceptDescription',
                                         id_type=model.IdentifierType.IRI),
         is_case_of={model.Reference((model.Key(type_=model.KeyElements.GLOBAL_REFERENCE,
@@ -611,15 +617,16 @@
         administration=model.AdministrativeInformation(version='0.9',
                                                        revision='0'))
     return concept_description
 
 
 def create_example_concept_dictionary() -> model.ConceptDictionary:
     """
-    creates an example concept dictionary containing an reference to the example concept description
+    Creates an example :class:`~aas.model.concept.ConceptDictionary` containing an :class:`~aas.model.base.AASReference`
+    to the example :class:`~aas.model.concept.ConceptDescription`
 
     :return: example concept dictionary
     """
     concept_dictionary = model.ConceptDictionary(
         id_short='TestConceptDictionary',
         category=None,
         description={'en-us': 'An example concept dictionary for the test application',
@@ -632,18 +639,19 @@
                                                 model.ConceptDescription)})
     return concept_dictionary
 
 
 def create_example_asset_administration_shell(concept_dictionary: model.ConceptDictionary) -> \
         model.AssetAdministrationShell:
     """
-    creates an asset administration shell with references to the example asset and submodel and includes a given
-    concept dictionary
+    Creates an :class:`~aas.model.aas.AssetAdministrationShell` with references to an example
+    :class:`~aas.model.aas.Asset` and :class:`~aas.model.submodel.Submodel` and includes a given
+    :class:`~aas.model.concept.ConceptDictionary`
 
-    :return: example asset administration shell
+    :return: example :class:`~aas.model.aas.AssetAdministrationShell`
     """
     asset_administration_shell = model.AssetAdministrationShell(
         asset=model.AASReference((model.Key(type_=model.KeyElements.ASSET,
                                             local=False,
                                             value='https://acplt.org/Test_Asset',
                                             id_type=model.KeyType.IRI),),
                                  model.Asset),
@@ -654,25 +662,25 @@
         description={'en-us': 'An Example Asset Administration Shell for the test application',
                      'de': 'Ein Beispiel-Verwaltungsschale für eine Test-Anwendung'},
         parent=None,
         administration=model.AdministrativeInformation(version='0.9',
                                                        revision='0'),
         security=None,
         submodel={model.AASReference((model.Key(type_=model.KeyElements.SUBMODEL,
-                                                local=False,
+                                                local=True,
                                                 value='https://acplt.org/Test_Submodel',
                                                 id_type=model.KeyType.IRI),),
                                      model.Submodel),
                   model.AASReference((model.Key(type_=model.KeyElements.SUBMODEL,
-                                                local=False,
+                                                local=True,
                                                 value='http://acplt.org/Submodels/Assets/TestAsset/Identification',
                                                 id_type=model.KeyType.IRI),),
                                      model.Submodel),
                   model.AASReference((model.Key(type_=model.KeyElements.SUBMODEL,
-                                                local=False,
+                                                local=True,
                                                 value='http://acplt.org/Submodels/Assets/TestAsset/BillOfMaterial',
                                                 id_type=model.KeyType.IRI),),
                                      model.Submodel),
                   },
         concept_dictionary=[concept_dictionary],
         view=[],
         derived_from=model.AASReference((model.Key(type_=model.KeyElements.ASSET_ADMINISTRATION_SHELL,
```

### Comparing `pyi40aas-0.2.2/aas/examples/data/example_aas_missing_attributes.py` & `pyi40aas-0.2.3/aas/examples/data/example_aas_missing_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,43 +2,46 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
-Module for the creation of a object store with missing object attribute combination for testing the serialization
-
+Module for the creation of an :class:`ObjectStore <aas.model.provider.DictObjectStore>` with missing object attribute
+combination for testing the serialization
 """
 import logging
 
 from ... import model
 from ._helper import AASDataChecker
 
 logger = logging.getLogger(__name__)
 
 
 def create_full_example() -> model.DictObjectStore:
     """
-    creates an object store containing an example asset identification submodel, an example asset, an example submodel,
-    an example concept description and an example asset administration shell
+    Creates an :class:`~aas.model.provider.DictObjectStore` containing an example asset identification
+    :class:`~aas.model.submodel.Submodel`, an example :class:`~aas.model.aas.Asset`, an example
+    :class:`~aas.model.submodel.Submodel`,
+    an example :class:`~aas.model.concept.ConceptDescription` and an example
+    :class:`~aas.model.aas.AssetAdministrationShell`
 
-    :return: object store
+    :return: :class:`aas.model.provider.DictObjectStore`
     """
     obj_store: model.DictObjectStore[model.Identifiable] = model.DictObjectStore()
     obj_store.add(create_example_asset())
     obj_store.add(create_example_submodel())
     obj_store.add(create_example_concept_description())
     obj_store.add(create_example_asset_administration_shell(create_example_concept_dictionary()))
     return obj_store
 
 
 def create_example_asset() -> model.Asset:
     """
-    creates an example asset which holds references to the example asset identification submodel
+    Creates an example :class:`~aas.model.aas.Asset` which holds references to the example asset identification submodel
 
     :return: example asset
     """
     asset = model.Asset(
         kind=model.AssetKind.INSTANCE,
         identification=model.Identifier(id_='https://acplt.org/Test_Asset_Missing',
                                         id_type=model.IdentifierType.IRI),
@@ -51,15 +54,16 @@
         asset_identification_model=None,
         bill_of_material=None)
     return asset
 
 
 def create_example_submodel() -> model.Submodel:
     """
-    creates an example submodel containing all kind of SubmodelElement objects
+    Creates an example :class:`~aas.model.submodel.Submodel` containing all kind of
+    :class:`~aas.model.submodel.SubmodelElement`  objects
 
     :return: example submodel
     """
     qualifier = model.Qualifier(
         type_='http://acplt.org/Qualifier/ExampleQualifier',
         value_type=model.datatypes.String)
 
@@ -335,15 +339,15 @@
         qualifier=None,
         kind=model.ModelingKind.INSTANCE)
     return submodel
 
 
 def create_example_concept_description() -> model.ConceptDescription:
     """
-    creates an example concept description
+    Creates an example :class:`~aas.model.concept.ConceptDescription`
 
     :return: example concept description
     """
     concept_description = model.ConceptDescription(
         identification=model.Identifier(id_='https://acplt.org/Test_ConceptDescription_Missing',
                                         id_type=model.IdentifierType.IRI),
         is_case_of=None,
@@ -355,15 +359,16 @@
         administration=model.AdministrativeInformation(version='0.9',
                                                        revision='0'))
     return concept_description
 
 
 def create_example_concept_dictionary() -> model.ConceptDictionary:
     """
-    creates an example concept dictionary containing an reference to the example concept description
+    Creates an example :class:`~aas.model.concept.ConceptDictionary` containing an :class:`~aas.model.base.AASReference`
+    to the example :class:`~aas.model.concept.ConceptDescription`
 
     :return: example concept dictionary
     """
     concept_dictionary = model.ConceptDictionary(
         id_short='TestConceptDictionary',
         category=None,
         description={'en-us': 'An example concept dictionary for the test application',
@@ -376,15 +381,16 @@
                                                 model.ConceptDescription)})
     return concept_dictionary
 
 
 def create_example_asset_administration_shell(concept_dictionary: model.ConceptDictionary) -> \
         model.AssetAdministrationShell:
     """
-    creates an example asset administration shell containing references to the example asset and example submodel
+    Creates an example :class:`~aas.model.aas.AssetAdministrationShell` containing references to the example
+    :class:`~aas.model.Asset` and example :class:`~aas.model.submodel.Submodel`
 
     :return: example asset administration shell
     """
     view = model.View(
         id_short='ExampleView',
         contained_element={model.AASReference((model.Key(type_=model.KeyElements.SUBMODEL,
                                                          local=False,
@@ -407,15 +413,15 @@
         description={'en-us': 'An Example Asset Administration Shell for the test application',
                      'de': 'Ein Beispiel-Verwaltungsschale für eine Test-Anwendung'},
         parent=None,
         administration=model.AdministrativeInformation(version='0.9',
                                                        revision='0'),
         security=None,
         submodel={model.AASReference((model.Key(type_=model.KeyElements.SUBMODEL,
-                                                local=False,
+                                                local=True,
                                                 value='https://acplt.org/Test_Submodel_Missing',
                                                 id_type=model.KeyType.IRI),),
                                      model.Submodel)},
         concept_dictionary=[concept_dictionary],
         view=[view, view_2],
         derived_from=None)
     return asset_administration_shell
```

### Comparing `pyi40aas-0.2.2/aas/examples/data/__init__.py` & `pyi40aas-0.2.3/aas/examples/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/examples/data/TestFile.pdf` & `pyi40aas-0.2.3/aas/examples/data/TestFile.pdf`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/examples/data/example_aas_mandatory_attributes.py` & `pyi40aas-0.2.3/aas/examples/data/example_aas_mandatory_attributes.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,62 +2,67 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
-Module for the creation of an object store with an example asset administration shell, related asset and example
-submodels and a concept dictionary containing an example concept description. All objects only contain mandatory
+Module for the creation of an :class:`ObjectStore <aas.model.provider.DictObjectStore>` with an example
+:class:`~aas.model.aas.AssetAdministrationShell`, related :class:`~aas.model.aas.Asset` and example
+:class:`Submodels <aas.model.submodel.Submodel>` and a :class:`~aas.model.concept.ConceptDictionary` containing an
+example :class:`~aas.model.concept.ConceptDescription`. All objects only contain mandatory
 attributes.
 
-To get this object store use the function 'create_full_example'. If you want to get single example objects or want to
-get more information use the other functions.
+To get this object store use the function
+:meth:`~aas.examples.data.example_aas_mandatory_attributes.create_full_example`. If you want to get single example
+objects or want to get more information use the other functions.
 """
 import logging
 
 from ... import model
 from ._helper import AASDataChecker
 
 logger = logging.getLogger(__name__)
 
 
 def create_full_example() -> model.DictObjectStore:
     """
-    creates an object store which is filled with an example asset, submodel, concept description and asset
-    administration shell using the function of this module
+    Creates an :class:`~.aas.model.provider.DictObjectStore` which is filled with an example
+    :class:`~aas.model.aas.Asset`, :class:`~aas.model.submodel.Submodel`, :class:`~aas.model.concept.ConceptDescription`
+    and :class:`~aas.model.aas.AssetAdministrationShell` using the functions of this module
 
-    :return: object store
+    :return: :class:`~aas.model.provider.DictObjectStore`
     """
     obj_store: model.DictObjectStore[model.Identifiable] = model.DictObjectStore()
     obj_store.add(create_example_asset())
     obj_store.add(create_example_submodel())
     obj_store.add(create_example_empty_submodel())
     obj_store.add(create_example_concept_description())
     obj_store.add(create_example_asset_administration_shell(create_example_concept_dictionary()))
     obj_store.add(create_example_empty_asset_administration_shell())
     return obj_store
 
 
 def create_example_asset() -> model.Asset:
     """
-    creates an example asset where only the kind and identification attributes are set
+    Creates an example :class:`~aas.model.aas.Asset` where only the `kind` and `identification` attributes are set
 
-    :return: example asset
+    :return: example Asset
     """
     asset = model.Asset(
         kind=model.AssetKind.INSTANCE,
         identification=model.Identifier(id_='https://acplt.org/Test_Asset_Mandatory',
                                         id_type=model.IdentifierType.IRI))
     return asset
 
 
 def create_example_submodel() -> model.Submodel:
     """
-    creates an example submodel containing all kind of SubmodelElement objects where only mandatory attributes are set
+    Creates an example :class:`~aas.model.submodel.Submodel` containing all kind of
+    :class:`~aas.model.submodel.SubmodelElement` objects where only mandatory attributes are set
 
     :return: example submodel
     """
     submodel_element_property = model.Property(
         id_short='ExampleProperty',
         value_type=model.datatypes.String)
 
@@ -147,79 +152,81 @@
                           submodel_element_submodel_element_collection_unordered,
                           submodel_element_submodel_element_collection_unordered_2))
     return submodel
 
 
 def create_example_empty_submodel() -> model.Submodel:
     """
-    creates an example empty submodel where only the identification attribute is set
+    Creates an example empty :class:`~aas.model.submodel.Submodel` where only the identification attribute is set
 
     :return: example submodel
     """
     return model.Submodel(
         identification=model.Identifier(id_='https://acplt.org/Test_Submodel2_Mandatory',
                                         id_type=model.IdentifierType.IRI))
 
 
 def create_example_concept_description() -> model.ConceptDescription:
     """
-    creates an example concept description where only the identification attribute is set
+    Creates an example :class:`~aas.model.concept.ConceptDescription` where only the identification attribute is set
 
     :return: example concept description
     """
     concept_description = model.ConceptDescription(
         identification=model.Identifier(id_='https://acplt.org/Test_ConceptDescription_Mandatory',
                                         id_type=model.IdentifierType.IRI))
     return concept_description
 
 
 def create_example_concept_dictionary() -> model.ConceptDictionary:
     """
-    creates an example concept dictionary where only the id_short attribute is set
+    creates an example :class:`~aas.model.concept.ConceptDictionary` where only the `id_short` attribute is set
 
     :return: example concept dictionary
     """
     concept_dictionary = model.ConceptDictionary(
         id_short='TestConceptDictionary')
     return concept_dictionary
 
 
 def create_example_asset_administration_shell(concept_dictionary: model.ConceptDictionary) -> \
         model.AssetAdministrationShell:
     """
-    creates an example asset administration shell containing references to the example asset, the example submodels and
-    including the example concept dictionary
+    Creates an example :class:`~aas.model.aas.AssetAdministrationShell` containing references to the example
+    :class:`~aas.model.aas.Asset`, the example :class:`Submodels <aas.model.submodel.Submodel>` and
+    including the example :class:`~aas.model.concept.ConceptDictionary`
 
     :return: example asset administration shell
     """
     asset_administration_shell = model.AssetAdministrationShell(
         asset=model.AASReference((model.Key(type_=model.KeyElements.ASSET,
                                             local=False,
                                             value='https://acplt.org/Test_Asset_Mandatory',
                                             id_type=model.KeyType.IRI),),
                                  model.Asset),
         identification=model.Identifier(id_='https://acplt.org/Test_AssetAdministrationShell_Mandatory',
                                         id_type=model.IdentifierType.IRI),
         submodel={model.AASReference((model.Key(type_=model.KeyElements.SUBMODEL,
-                                                local=False,
+                                                local=True,
                                                 value='https://acplt.org/Test_Submodel_Mandatory',
                                                 id_type=model.KeyType.IRI),),
                                      model.Submodel),
                   model.AASReference((model.Key(type_=model.KeyElements.SUBMODEL,
-                                                local=False,
+                                                local=True,
                                                 value='https://acplt.org/Test_Submodel2_Mandatory',
                                                 id_type=model.KeyType.IRI),),
                                      model.Submodel)},
         concept_dictionary=[concept_dictionary])
     return asset_administration_shell
 
 
 def create_example_empty_asset_administration_shell() -> model.AssetAdministrationShell:
     """
-    creates an example empty asset administration shell where only the reference to the asset and the identification
+    Creates an example empty :class:`~aas.model.aas.AssetAdministrationShell` where only the reference to the
+    :class:`~aas.model.aas.Asset` and the identification
     attribute is set
 
     :return: example asset administration shell
     """
     asset_administration_shell = model.AssetAdministrationShell(
         asset=model.AASReference((model.Key(type_=model.KeyElements.ASSET,
                                             local=False,
```

### Comparing `pyi40aas-0.2.2/aas/examples/data/_helper.py` & `pyi40aas-0.2.3/aas/examples/data/_helper.py`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/examples/data/example_submodel_template.py` & `pyi40aas-0.2.3/aas/examples/data/example_submodel_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
-Module for the creation of an example submodel template containing all kind of submodel elements where the kind is
-always TEMPLATE.
-
+Module for the creation of an example :class:`~aas.model.submodel.Submodel` template containing all kind of
+:class:`SubmodelElements <aas.model.submodel.SubmodelElement>` where the kind is
+always `TEMPLATE`.
 """
 import logging
 
 from ... import model
 from ._helper import AASDataChecker
 
 logger = logging.getLogger(__name__)
 
 
 def create_example_submodel_template() -> model.Submodel:
     """
-    creates an example submodel template containing all kind of SubmodelElement objects where the kind is always
-    TEMPLATE
+    Creates an example :class:`~aas.model.submodel.Submodel` template containing all kind of
+    :class:`~aas.model.submodel.SubmodelElement` objects where the kind is always
+    `TEMPLATE`
 
     :return: example submodel
     """
     submodel_element_property = model.Property(
         id_short='ExampleProperty',
         value_type=model.datatypes.String,
         value=None,
```

### Comparing `pyi40aas-0.2.2/aas/examples/data/example_concept_description.py` & `pyi40aas-0.2.3/aas/examples/data/example_concept_description.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
-Module for creation of an example concept description
+Module for creation of an example :class:`~aas.model.concept.ConceptDescription`
 """
 import logging
 
 from ... import model
 from ._helper import AASDataChecker
 from ...model.concept import *
 
 logger = logging.getLogger(__name__)
 
 
 def create_iec61360_concept_description() -> IEC61360ConceptDescription:
     """
-    Creates a ConceptDescription after the IEC61360 standard
+    Creates a :class:`~aas.model.concept.ConceptDescription` after the IEC61360 standard
 
     :return: Example concept description
     """
     identification = model.Identifier(id_='http://acplt.org/DataSpecifciations/Example/Identification',
                                       id_type=model.IdentifierType.IRI)
     return IEC61360ConceptDescription(
         identification=identification,
```

### Comparing `pyi40aas-0.2.2/aas/adapter/aasx.py` & `pyi40aas-0.2.3/aas/adapter/aasx.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
+.. _adapter.aasx:
+
 Functionality for reading and writing AASX files according to "Details of the Asset Administration Shell Part 1 V2.0",
 section 7.
 
 The AASX file format is built upon the Open Packaging Conventions (OPC; ECMA 376-2). We use the `pyecma376_2` library
 for low level OPC reading and writing. It currently supports all required features except for embedded digital
 signatures.
 
-Writing and reading of AASX packages is performed through the AASXReader and AASXWriter classes. Each instance of these
-classes wraps an existing AASX file resp. a file to be created and allows to read/write the included AAS objects
-into/form object stores. For handling of embedded supplementary files, this module provides the
-`AbstractSupplementaryFileContainer` class interface and the `DictSupplementaryFileContainer` implementation.
+Writing and reading of AASX packages is performed through the :class:`~.AASXReader` and :class:`~.AASXWriter` classes.
+Each instance of these classes wraps an existing AASX file resp. a file to be created and allows to read/write the
+included AAS objects into/form :class:`ObjectStores <aas.model.provider.AbstractObjectStore>`.
+For handling of embedded supplementary files, this module provides the
+:class:`~.AbstractSupplementaryFileContainer` class
+interface and the :class:`~.DictSupplementaryFileContainer` implementation.
 """
 
 import abc
 import hashlib
 import io
 import itertools
 import logging
@@ -44,14 +48,16 @@
 
 class AASXReader:
     """
     An AASXReader wraps an existing AASX package file to allow reading its contents and metadata.
 
     Basic usage:
 
+    .. code-block:: python
+
         objects = DictObjectStore()
         files = DictSupplementaryFileContainer()
         with AASXReader("filename.aasx") as reader:
             meta_data = reader.get_core_properties()
             reader.read_into(objects, files)
     """
     def __init__(self, file: Union[os.PathLike, str, IO]):
@@ -84,14 +90,16 @@
     def get_thumbnail(self) -> Optional[bytes]:
         """
         Retrieve the packages thumbnail image
 
         The thumbnail image file is read into memory and returned as bytes object. You may use some python image library
         for further processing or conversion, e.g. `pillow`:
 
+        .. code-block:: python
+
             import io
             from PIL import Image
             thumbnail = Image.open(io.BytesIO(reader.get_thumbnail()))
 
         :return: The AASX package thumbnail's file contents or None if no thumbnail is provided
         """
         try:
@@ -102,28 +110,35 @@
         with self.reader.open_part(thumbnail_part) as p:
             return p.read()
 
     def read_into(self, object_store: model.AbstractObjectStore,
                   file_store: "AbstractSupplementaryFileContainer",
                   override_existing: bool = False) -> Set[model.Identifier]:
         """
-        Read the contents of the AASX package and add them into a given ObjectStore
+        Read the contents of the AASX package and add them into a given
+        :class:`ObjectStore <aas.model.provider.AbstractObjectStore>`
 
         This function does the main job of reading the AASX file's contents. It traverses the relationships within the
         package to find AAS JSON or XML parts, parses them and adds the contained AAS objects into the provided
-        `object_store`. While doing so, it searches all parsed Submodels for File objects to extract the supplementary
-        files. The referenced supplementary files are added to the given `file_store` and the File objects' values are
-        updated with the absolute name of the supplementary file to allow for robust resolution the file within the
+        `object_store`. While doing so, it searches all parsed :class:`Submodels <aas.model.submodel.Submodel>` for
+        :class:`~aas.model.submodel.File` objects to extract the supplementary
+        files. The referenced supplementary files are added to the given `file_store` and the
+        :class:`~aas.model.submodel.File` objects' values are updated with the absolute name of the supplementary file
+        to allow for robust resolution the file within the
         `file_store` later.
 
-        :param object_store: An ObjectStore to add the AAS objects from the AASX file to
-        :param file_store: A SupplementaryFileContainer to add the embedded supplementary files to
-        :param override_existing: If True, existing objects in the object store are overridden with objects from the
-            AASX that have the same Identifer. Default behavior is to skip those objects from the AASX.
-        :return: A set of the Identifiers of all Identifiable objects parsed from the AASX file
+        :param object_store: An :class:`ObjectStore <aas.model.provider.AbstractObjectStore>` to add the AAS objects
+                             from the AASX file to
+        :param file_store: A :class:`SupplementaryFileContainer <.AbstractSupplementaryFileContainer>` to add the
+                           embedded supplementary files to
+        :param override_existing: If `True`, existing objects in the object store are overridden with objects from the
+            AASX that have the same :class:`~aas.model.base.Identifier`. Default behavior is to skip those objects from
+            the AASX.
+        :return: A set of the :class:`Identifiers <aas.model.base.Identifier>` of all
+                 :class:`~aas.model.base.Identifiable` objects parsed from the AASX file
         """
         # Find AASX-Origin part
         core_rels = self.reader.get_related_parts_by_type()
         try:
             aasx_origin_part = core_rels[RELATIONSHIP_TYPE_AASX_ORIGIN][0]
         except IndexError as e:
             raise ValueError("Not a valid AASX file: aasx-origin Relationship is missing.") from e
@@ -156,15 +171,15 @@
 
     def _read_aas_part_into(self, part_name: str,
                             object_store: model.AbstractObjectStore,
                             file_store: "AbstractSupplementaryFileContainer",
                             read_identifiables: Set[model.Identifier],
                             override_existing: bool) -> None:
         """
-        Helper function for `read_into()` to read and process the contents of an AAS-spec part of the AASX file.
+        Helper function for :meth:`read_into()` to read and process the contents of an AAS-spec part of the AASX file.
 
         This method primarily checks for duplicate objects. It uses `_parse_aas_parse()` to do the actual parsing and
         `_collect_supplementary_files()` for supplementary file processing of non-duplicate objects.
 
         :param part_name: The OPC part name to read
         :param object_store: An ObjectStore to add the AAS objects from the AASX file to
         :param file_store: A SupplementaryFileContainer to add the embedded supplementary files to, which are reference
@@ -246,30 +261,33 @@
 
 class AASXWriter:
     """
     An AASXWriter wraps a new AASX package file to write its contents to it piece by piece.
 
     Basic usage:
 
+    .. code-block:: python
+
         # object_store and file_store are expected to be given (e.g. some storage backend or previously created data)
         cp = OPCCoreProperties()
         cp.creator = "ACPLT"
         cp.created = datetime.datetime.now()
 
         with AASXWriter("filename.aasx") as writer:
             writer.write_aas(Identifier("https://acplt.org/AssetAdministrationShell", IdentifierType.IRI),
                              object_store,
                              file_store)
             writer.write_aas(Identifier("https://acplt.org/AssetAdministrationShell2", IdentifierType.IRI),
                              object_store,
                              file_store)
             writer.write_core_properties(cp)
 
-    Attention: The AASXWriter must always be closed using the close() method or its context manager functionality (as
-    shown above). Otherwise the resulting AASX file will lack important data structures and will not be readable.
+    **Attention:** The AASXWriter must always be closed using the :meth:`~.AASXWriter.close` method or its context
+    manager functionality (as shown above). Otherwise the resulting AASX file will lack important data structures
+    and will not be readable.
     """
     AASX_ORIGIN_PART_NAME = "/aasx/aasx-origin"
 
     def __init__(self, file: Union[os.PathLike, str, IO]):
         """
         Create a new AASX package in the given file and open the AASXWriter to add contents to the package.
 
@@ -300,34 +318,39 @@
     def write_aas(self,
                   aas_id: model.Identifier,
                   object_store: model.AbstractObjectStore,
                   file_store: "AbstractSupplementaryFileContainer",
                   write_json: bool = False,
                   submodel_split_parts: bool = True) -> None:
         """
-        Convenience method to add an Asset Administration Shell with all included and referenced objects to the AASX
-        package according to the part name conventions from DotAAS.
+        Convenience method to add an :class:`~aas.model.aas.AssetAdministrationShell` with all included and referenced
+        objects to the AASX package according to the part name conventions from DotAAS.
 
-        This method takes the AAS's Identifier (as `aas_id`) to retrieve it from the given object_store. References to
-        the Asset, ConceptDescriptions and Submodels are also resolved using the object_store. All of these objects are
-        written to aas-spec parts in the AASX package, follwing the conventions presented in "Details of the Asset
+        This method takes the AAS's :class:`~aas.model.base.Identifier` (as `aas_id`) to retrieve it from the given
+        object_store. :class:`References <~aas.model.base.Reference>` to
+        the :class:`~aas.model.aas.Asset`, :class:`ConceptDescriptions <aas.model.concept.ConceptDescription>` and
+        :class:`Submodels <aas.model.submodel.Submodel>` are also resolved using the object_store. All of these objects
+        are written to aas-spec parts in the AASX package, following the conventions presented in "Details of the Asset
         Administration Shell". For each Submodel, a aas-spec-split part is used. Supplementary files which are
         referenced by a File object in any of the Submodels, are also added to the AASX package.
 
-        Internally, this method uses `write_aas_objects()` to write the individual AASX parts for the AAS and each
-        submodel.
+        Internally, this method uses :meth:`aas.adapter.aasx.AASXWriter.write_aas_objects` to write the individual AASX
+        parts for the AAS and each submodel.
 
-        :param aas_id: Identifier of the AAS to be added to the AASX file
-        :param object_store: ObjectStore to retrieve the Identifiable AAS objects (AAS, Asset, ConceptDescriptions and
-            Submodels) from
-        :param file_store: SupplementaryFileContainer to retrieve supplementary files from, which are referenced by File
-            objects
-        :param write_json:  If True, JSON parts are created for the AAS and each submodel in the AASX package file
-            instead of XML parts. Defaults to False.
-        :param submodel_split_parts: If True (default), submodels are written to separate AASX parts instead of being
+        :param aas_id: :class:`~aas.model.base.Identifier` of the :class:`~aas.model.aas.AssetAdministrationShell` to
+            be added to the AASX file
+        :param object_store: :class:`ObjectStore <aas.model.provider.AbstractObjectStore>` to retrieve the
+            :class:`~aas.model.base.Identifiable` AAS objects (:class:`~aas.model.aas.AssetAdministrationShell`,
+            :class:`~aas.model.aas.Asset`, :class:`~aas.model.concept.ConceptDescription` and
+            :class:`~aas.model.submodel.Submodel`) from
+        :param file_store: :class:`SupplementaryFileContainer <aas.adapter.aasx.AbstractSupplementaryFileContainer>` to
+            retrieve supplementary files from, which are referenced by :class:`~aas.model.submodel.File` objects
+        :param write_json:  If `True`, JSON parts are created for the AAS and each submodel in the AASX package file
+            instead of XML parts. Defaults to `False`.
+        :param submodel_split_parts: If `True` (default), submodels are written to separate AASX parts instead of being
             included in the AAS part with in the AASX package.
         """
         aas_friendly_name = self._aas_name_friendlyfier.get_friendly_name(aas_id)
         aas_part_name = "/aasx/{0}/{0}.aas.{1}".format(aas_friendly_name, "json" if write_json else "xml")
 
         aas = object_store.get_identifiable(aas_id)
         if not isinstance(aas, model.AssetAdministrationShell):
@@ -378,30 +401,34 @@
                           write_json: bool = False,
                           split_part: bool = False,
                           additional_relationships: Iterable[pyecma376_2.OPCRelationship] = ()) -> None:
         """
         Write a defined list of AAS objects to an XML or JSON part in the AASX package and append the referenced
         supplementary files to the package.
 
-        This method takes the AAS's Identifier (as `aas_id`) to retrieve it from the given object_store. If the list
-        of written objects includes Submodel objects, Supplementary files which are referenced by File objects within
+        This method takes the AAS's :class:`~aas.model.base.Identifier` (as `aas_id`) to retrieve it from the given
+        object_store. If the list
+        of written objects includes :class:`aas.model.submodel.Submodel` objects, Supplementary files which are
+        referenced by :class:`~aas.model.submodel.File` objects within
         those submodels, are also added to the AASX package.
 
         You must make sure to call this method only once per unique `part_name` on a single package instance.
 
         :param part_name: Name of the Part within the AASX package to write the files to. Must be a valid ECMA376-2
             part name and unique within the package. The extension of the part should match the data format (i.e.
             '.json' if `write_json` else '.xml').
-        :param object_ids: A list of identifiers of the objects to be written to the AASX package. Only these
-            Identifiable objects (and included Referable objects) are written to the package.
-        :param object_store: The objects store to retrieve the Identifable objects from
-        :param file_store: The SupplementaryFileContainer to retrieve supplementary files from (if there are any `File`
+        :param object_ids: A list of :class:`Identifiers <aas.model.base.Identifier>` of the objects to be written to
+            the AASX package. Only these :class:`~aas.model.base.Identifiable` objects (and included
+            :class:`~aas.model.base.Referable` objects) are written to the package.
+        :param object_store: The objects store to retrieve the :class:`~aas.model.base.Identifiable` objects from
+        :param file_store: The :class:`SupplementaryFileContainer <aas.adapter.aasx.AbstractSupplementaryFileContainer>`
+            to retrieve supplementary files from (if there are any :class:`~aas.model.submodel.File`
             objects within the written objects.
-        :param write_json: If True, the part is written as a JSON file instead of an XML file. Defaults to False.
-        :param split_part: If True, no aas-spec relationship is added from the aasx-origin to this part. You must make
+        :param write_json: If `True`, the part is written as a JSON file instead of an XML file. Defaults to `False`.
+        :param split_part: If `True`, no aas-spec relationship is added from the aasx-origin to this part. You must make
             sure to reference it via a aas-spec-split relationship from another aas-spec part
         :param additional_relationships: Optional OPC/ECMA376 relationships which should originate at the AAS object
             part to be written, in addition to the aas-suppl relationships which are created automatically.
         """
         logger.debug("Writing AASX part {} with AAS objects ...".format(part_name))
 
         objects: model.DictObjectStore[model.Identifiable] = model.DictObjectStore()
@@ -469,30 +496,32 @@
                 additional_relationships),
             part_name)
 
     def write_core_properties(self, core_properties: pyecma376_2.OPCCoreProperties):
         """
         Write OPC Core Properties (meta data) to the AASX package file.
 
-        Attention: This method may only be called once for each AASXWriter!
+        .. Attention::
+            This method may only be called once for each AASXWriter!
 
         :param core_properties: The OPCCoreProperties object with the meta data to be written to the package file
         """
         if self._properties_part is not None:
             raise RuntimeError("Core Properties have already been written.")
         logger.debug("Writing core properties to AASX package ...")
         with self.writer.open_part(pyecma376_2.DEFAULT_CORE_PROPERTIES_NAME, "application/xml") as p:
             core_properties.write_xml(p)
         self._properties_part = pyecma376_2.DEFAULT_CORE_PROPERTIES_NAME
 
     def write_thumbnail(self, name: str, data: bytearray, content_type: str):
         """
         Write an image file as thumbnail image to the AASX package.
 
-        Attention: This method may only be called once for each AASXWriter!
+        .. Attention::
+            This method may only be called once for each AASXWriter!
 
         :param name: The OPC part name of the thumbnail part. Should not contain '/' or URI-encoded '/' or '\'.
         :param data: The image file's binary contents to be written
         :param content_type: OPC content type (MIME type) of the image file
         """
         if self._thumbnail_part is not None:
             raise RuntimeError("package thumbnail has already been written to {}.".format(self._thumbnail_part))
@@ -571,21 +600,26 @@
     def get_friendly_name(self, identifier: model.Identifier):
         """
         Generate a friendly name from an AAS identifier.
 
         According to section 7.6 of "Details of the Asset Administration Shell", all non-alphanumerical characters are
         replaced with underscores. We also replace all non-ASCII characters to generate valid URIs as the result.
         If this replacement results in a collision with a previously generated friendly name of this NameFriendlifier,
-        a number is appended with underscore to the friendly name. Example
+        a number is appended with underscore to the friendly name.
+
+        Example:
+
+        .. code-block:: python
+
+            friendlyfier = NameFriendlyfier()
+            friendlyfier.get_friendly_name(model.Identifier("http://example.com/AAS-a", model.IdentifierType.IRI))
+             > "http___example_com_AAS_a"
 
-            >>> friendlyfier = NameFriendlyfier()
-            >>> friendlyfier.get_friendly_name(model.Identifier("http://example.com/AAS-a", model.IdentifierType.IRI))
-            "http___example_com_AAS_a"
-            >>> friendlyfier.get_friendly_name(model.Identifier("http://example.com/AAS+a", model.IdentifierType.IRI))
-            "http___example_com_AAS_a_1"
+            friendlyfier.get_friendly_name(model.Identifier("http://example.com/AAS+a", model.IdentifierType.IRI))
+             >  "http___example_com_AAS_a_1"
 
         """
         # friendlify name
         raw_name = self.RE_NON_ALPHANUMERICAL.sub('_', identifier.id)
 
         # Unify name (avoid collisions)
         amended_name = raw_name
@@ -599,16 +633,16 @@
 
 
 class AbstractSupplementaryFileContainer(metaclass=abc.ABCMeta):
     """
     Abstract interface for containers of supplementary files for AASs.
 
     Supplementary files may be PDF files or other binary or textual files, referenced in a File object of an AAS by
-    their name. They are used to provide associated documents without embedding their contents (as Blob object) in the
-    AAS.
+    their name. They are used to provide associated documents without embedding their contents (as
+    :class:`~aas.model.submodel.Blob` object) in the AAS.
 
     A SupplementaryFileContainer keeps track of the name and content_type (MIME type) for each file. Additionally it
     allows to resolve name conflicts by comparing the files' contents and providing an alternative name for a dissimilar
     new file. It also provides each files sha256 hash sum to allow name conflict checking in other classes (e.g. when
     writing AASX files).
     """
     @abc.abstractmethod
```

### Comparing `pyi40aas-0.2.2/aas/adapter/_generic.py` & `pyi40aas-0.2.3/aas/adapter/_generic.py`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/adapter/xml/xml_deserialization.py` & `pyi40aas-0.2.3/aas/adapter/xml/xml_deserialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,34 +2,43 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
+.. _adapter.xml.xml_deserialization:
+
 Module for deserializing Asset Administration Shell data from the official XML format
 
 This module provides the following functions for parsing XML documents:
-- read_aas_xml_element() constructs a single object from an XML document containing a single element
-- read_aas_xml_file_into() constructs all elements of an XML document and stores them in a given object store
-- read_aas_xml_file() constructs all elements of an XML document and returns them in a DictObjectStore
+
+- :meth:`~aas.adapter.xml.xml_deserialization.read_aas_xml_element` constructs a single object from an XML document
+  containing a single element
+- :meth:`~aas.adapter.xml.xml_deserialization.read_aas_xml_file_into` constructs all elements of an XML document and
+  stores them in a given :class:`ObjectStore <aas.model.provider.AbstractObjectStore>`
+- :meth:`~aas.adapter.xml.xml_deserialization.read_aas_xml_file` constructs all elements of an XML document and returns
+  them in a :class:`~aas.model.provider.DictObjectStore`
 
 These functions take a decoder class as keyword argument, which allows parsing in failsafe (default) or non-failsafe
 mode. Parsing stripped elements - used in the HTTP adapter - is also possible. It is also possible to subclass the
 default decoder class and provide an own decoder.
 
 In failsafe mode errors regarding missing attributes and elements or invalid values are caught and logged.
 In non-failsafe mode any error would abort parsing.
-Error handling is done only by _failsafe_construct() in this module. Nearly all constructor functions are called
-by other constructor functions via _failsafe_construct(), so an error chain is constructed in the error case,
+Error handling is done only by `_failsafe_construct()` in this module. Nearly all constructor functions are called
+by other constructor functions via `_failsafe_construct()`, so an error chain is constructed in the error case,
 which allows printing stacktrace-like error messages like the following in the error case (in failsafe mode of course):
 
-KeyError: aas:identification on line 252 has no attribute with name idType!
- -> Failed to construct aas:identification on line 252 using construct_identifier!
- -> Failed to construct aas:conceptDescription on line 247 using construct_concept_description!
+
+.. code-block::
+
+    KeyError: aas:identification on line 252 has no attribute with name idType!
+        -> Failed to construct aas:identification on line 252 using construct_identifier!
+        -> Failed to construct aas:conceptDescription on line 247 using construct_concept_description!
 
 
 Unlike the JSON deserialization, parsing is done top-down. Elements with a specific tag are searched on the level
 directly below the level of the current xml element (in terms of parent and child relation) and parsed when
 found. Constructor functions of these elements will then again search for mandatory and optional child elements
 and construct them if available, and so on.
 """
@@ -392,15 +401,15 @@
 
 class AASFromXmlDecoder:
     """
     The default XML decoder class.
 
     It parses XML documents in a failsafe manner, meaning any errors encountered will be logged and invalid XML elements
     will be skipped.
-    Most member functions support the object_class parameter. It was introduced so they can be overwritten
+    Most member functions support the `object_class` parameter. It was introduced so they can be overwritten
     in subclasses, which allows constructing instances of subtypes.
     """
     failsafe = True
     stripped = False
 
     @classmethod
     def _amend_abstract_attributes(cls, obj: object, element: etree.Element) -> None:
@@ -1214,15 +1223,15 @@
 def read_aas_xml_element(file: IO, construct: XMLConstructables, failsafe: bool = True, stripped: bool = False,
                          decoder: Optional[Type[AASFromXmlDecoder]] = None, **constructor_kwargs) -> Optional[object]:
     """
     Construct a single object from an XML string. The namespaces have to be declared on the object itself, since there
     is no surrounding aasenv element.
 
     :param file: A filename or file-like object to read the XML-serialized data from
-    :param construct: A member of the enum XML_CONSTRUCTABLES, specifying which type to construct.
+    :param construct: A member of the enum :class:`~.XMLConstructables`, specifying which type to construct.
     :param failsafe: If true, the document is parsed in a failsafe way: missing attributes and elements are logged
                      instead of causing exceptions. Defect objects are skipped.
                      This parameter is ignored if a decoder class is specified.
     :param stripped: If true, stripped XML elements are parsed.
                      See https://git.rwth-aachen.de/acplt/pyi40aas/-/issues/91
                      This parameter is ignored if a decoder class is specified.
     :param decoder: The decoder class used to decode the XML elements
@@ -1313,30 +1322,31 @@
 
 def read_aas_xml_file_into(object_store: model.AbstractObjectStore[model.Identifiable], file: IO,
                            replace_existing: bool = False, ignore_existing: bool = False, failsafe: bool = True,
                            stripped: bool = False, decoder: Optional[Type[AASFromXmlDecoder]] = None,
                            **parser_kwargs: Any) -> Set[model.Identifier]:
     """
     Read an Asset Administration Shell XML file according to 'Details of the Asset Administration Shell', chapter 5.4
-    into a given object store.
+    into a given :class:`ObjectStore <aas.model.provider.AbstractObjectStore>`.
 
-    :param object_store: The object store in which the identifiable objects should be stored
+    :param object_store: The :class:`ObjectStore <aas.model.provider.AbstractObjectStore>` in which the
+                         :class:`~aas.model.base.Identifiable` objects should be stored
     :param file: A filename or file-like object to read the XML-serialized data from
     :param replace_existing: Whether to replace existing objects with the same identifier in the object store or not
     :param ignore_existing: Whether to ignore existing objects (e.g. log a message) or raise an error.
                             This parameter is ignored if replace_existing is True.
-    :param failsafe: If true, the document is parsed in a failsafe way: missing attributes and elements are logged
+    :param failsafe: If `True`, the document is parsed in a failsafe way: missing attributes and elements are logged
                      instead of causing exceptions. Defect objects are skipped.
                      This parameter is ignored if a decoder class is specified.
-    :param stripped: If true, stripped XML elements are parsed.
+    :param stripped: If `True`, stripped XML elements are parsed.
                      See https://git.rwth-aachen.de/acplt/pyi40aas/-/issues/91
                      This parameter is ignored if a decoder class is specified.
     :param decoder: The decoder class used to decode the XML elements
     :param parser_kwargs: Keyword arguments passed to the XMLParser constructor
-    :return: A set of identifiers that were added to object_store
+    :return: A set of :class:`Identifiers <aas.model.base.Identifier>` that were added to object_store
     """
     ret: Set[model.Identifier] = set()
 
     decoder_ = _select_decoder(failsafe, stripped, decoder)
 
     element_constructors: Dict[str, Callable[..., model.Identifiable]] = {
         "assetAdministrationShell": decoder_.construct_asset_administration_shell,
@@ -1382,17 +1392,18 @@
             object_store.add(element)
             ret.add(element.identification)
     return ret
 
 
 def read_aas_xml_file(file: IO, **kwargs: Any) -> model.DictObjectStore[model.Identifiable]:
     """
-    A wrapper of read_aas_xml_file_into(), that reads all objects in an empty DictObjectStore. This function supports
-    the same keyword arguments as read_aas_xml_file_into().
+    A wrapper of :meth:`~aas.adapter.xml.xml_deserialization.read_aas_xml_file_into`, that reads all objects in an
+    empty :class:`~aas.model.provider.DictObjectStore`. This function supports
+    the same keyword arguments as :meth:`~aas.adapter.xml.xml_deserialization.read_aas_xml_file_into`.
 
     :param file: A filename or file-like object to read the XML-serialized data from
-    :param kwargs: Keyword arguments passed to read_aas_xml_file_into()
-    :return: A DictObjectStore containing all AAS objects from the XML file
+    :param kwargs: Keyword arguments passed to :meth:`~aas.adapter.xml.xml_deserialization.read_aas_xml_file_into`
+    :return: A :class:`~aas.model.provider.DictObjectStore` containing all AAS objects from the XML file
     """
     object_store: model.DictObjectStore[model.Identifiable] = model.DictObjectStore()
     read_aas_xml_file_into(object_store, file, **kwargs)
     return object_store
```

### Comparing `pyi40aas-0.2.2/aas/adapter/xml/__init__.py` & `pyi40aas-0.2.3/aas/adapter/xml/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
+.. _adapter.xml.__init__:
+
 This package contains functionality for serialization and deserialization of PyI40AAS objects into/from XML.
 
-xml_serialization:
-    The module offers a function to write an ObjectStore to a given file.
+:ref:`xml_serialization <adapter.xml.xml_serialization>`: The module offers a function to write an
+:class:`ObjectStore <aas.model.provider.AbstractObjectStore>` to a given file.
 
-xml_deserialization.py
-    The module offers a function to create an ObjectStore from a given xml document.
+:ref:`xml_deserialization <adapter.xml.xml_deserialization>`: The module offers a function to create an
+:class:`ObjectStore <aas.model.provider.AbstractObjectStore>` from a given xml document.
 """
 import os.path
 
 from .xml_serialization import write_aas_xml_file
 from .xml_deserialization import AASFromXmlDecoder, StrictAASFromXmlDecoder, StrippedAASFromXmlDecoder, \
     StrictStrippedAASFromXmlDecoder, XMLConstructables, read_aas_xml_file, read_aas_xml_file_into, read_aas_xml_element
```

### Comparing `pyi40aas-0.2.2/aas/adapter/xml/IEC61360.xsd` & `pyi40aas-0.2.3/aas/adapter/xml/IEC61360.xsd`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/adapter/xml/xml_serialization.py` & `pyi40aas-0.2.3/aas/adapter/xml/xml_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
+.. _adapter.xml.xml_serialization:
+
 Module for serializing Asset Administration Shell data to the official XML format
 
 How to use:
-- For generating an XML-File from a model.registry.AbstractObjectStore, check out the function "write_aas_xml_file".
+
+- For generating an XML-File from a :class:`~aas.model.provider.AbstractObjectStore`, check out the function
+  :meth:`~aas.adapter.xml.xml_serialization.write_aas_xml_file`.
 - For serializing any object to an XML fragment, that fits the XML specification from 'Details of the
   Asset Administration Shell', chapter 5.4, check out `<your_object_class_name_here>_to_xml()`. These functions return
-  an xml.etree.ElementTree.Element object to be serialized into XML.
+  an :class:`xml.etree.ElementTree.Element` object to be serialized into XML.
 """
 
 from lxml import etree  # type: ignore
 from typing import Dict, IO, Optional
 import base64
 
 from aas import model
@@ -848,17 +852,17 @@
                        data: model.AbstractObjectStore,
                        **kwargs) -> None:
     """
     Write a set of AAS objects to an Asset Administration Shell XML file according to 'Details of the Asset
     Administration Shell', chapter 5.4
 
     :param file: A file-like object to write the XML-serialized data to
-    :param data: ObjectStore which contains different objects of the AAS meta model which should be serialized to an
-                 XML file
-    :param kwargs: Additional keyword arguments to be passed to tree.write()
+    :param data: :class:`ObjectStore <aas.model.provider.AbstractObjectStore>` which contains different objects of the
+                 AAS meta model which should be serialized to an XML file
+    :param kwargs: Additional keyword arguments to be passed to `tree.write()`
     """
     # separate different kind of objects
     assets = []
     asset_administration_shells = []
     submodels = []
     concept_descriptions = []
     for obj in data:
```

### Comparing `pyi40aas-0.2.2/aas/adapter/xml/AAS_ABAC.xsd` & `pyi40aas-0.2.3/aas/adapter/xml/AAS_ABAC.xsd`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/adapter/xml/AAS.xsd` & `pyi40aas-0.2.3/aas/adapter/xml/AAS.xsd`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/adapter/json/json_deserialization.py` & `pyi40aas-0.2.3/aas/adapter/json/json_deserialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,35 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
+.. _adapter.json.json_deserialization:
+
 Module for deserializing Asset Administration Shell data from the official JSON format
 
-The module provides custom JSONDecoder classes `AASFromJsonDecoder` and `StrictAASFromJsonDecoder` to be used with
-the Python standard `json` module. They contain a custom `object_hook` function to detect encoded AAS objects within the
-JSON data and convert them to PyI40AAS objects while parsing. Additionally, there's the `read_json_aas_file()` function,
-that takes a complete AAS JSON file, reads its contents and returns the contained AAS objects as DictObjectStore.
-
-This job is performed in a bottom-up approach: The `object_hook()` method gets called for every parsed JSON object
-(as dict) and checks for existence of the `modelType` attribute. If it is present, the `AAS_CLASS_PARSERS` dict defines,
-which of the constructor methods of the class is to be used for converting the dict into an object. Embedded
+The module provides custom JSONDecoder classes :class:`~.AASFromJsonDecoder` and :class:`~.StrictAASFromJsonDecoder` to
+be used with the Python standard `json` module.
+
+Furthermore it provides two classes :class:`~aas.adapter.json.json_deserialization.StrippedAASFromJsonDecoder` and
+:class:`~aas.adapter.json.json_deserialization.StrictStrippedAASFromJsonDecoder` for parsing stripped JSON objects,
+which are used in the http adapter (see https://git.rwth-aachen.de/acplt/pyi40aas/-/issues/91).
+The classes contain a custom :meth:`~aas.adapter.json.json_deserialization.AASFromJsonDecoder.object_hook` function
+to detect encoded AAS objects within the JSON data and convert them to PyI40AAS objects while parsing. Additionally,
+there's the :meth:`~aas.adapter.json.json_deserialization.read_aas_json_file_into` function, that takes a complete
+AAS JSON file, reads its contents and stores the objects in the provided
+:class:`~aas.model.provider.AbstractObjectStore`. :meth:`~aas.adapter.json.json_deserialization.read_aas_json_file` is
+a wrapper for this function. Instead of storing the objects in a given :class:`~aas.model.provider.AbstractObjectStore`,
+it returns a :class:`~aas.model.provider.DictObjectStore` containing parsed objects.
+
+The deserialization is performed in a bottom-up approach: The `object_hook()` method gets called for every parsed JSON
+object (as dict) and checks for existence of the `modelType` attribute. If it is present, the `AAS_CLASS_PARSERS` dict
+defines, which of the constructor methods of the class is to be used for converting the dict into an object. Embedded
 objects that should have a `modelType` themselves are expected to be converted already. Other embedded objects are
 converted using a number of helper constructor methods.
 """
 import base64
 import json
 import logging
 import pprint
@@ -89,16 +100,20 @@
 
 
 class AASFromJsonDecoder(json.JSONDecoder):
     """
     Custom JSONDecoder class to use the `json` module for deserializing Asset Administration Shell data from the
     official JSON format
 
-    The class contains a custom `object_hook` function to detect encoded AAS objects within the JSON data and convert
-    them to PyI40AAS objects while parsing. Typical usage:
+    The class contains a custom :meth:`~.AASFromJsonDecoder.object_hook` function to detect encoded AAS objects within
+    the JSON data and convert them to PyI40AAS objects while parsing.
+
+    Typical usage:
+
+    .. code-block:: python
 
         data = json.loads(json_string, cls=AASFromJsonDecoder)
 
     The `object_hook` function uses a set of `_construct_*()` methods, one for each
     AAS object type to transform the JSON objects in to PyI40AAS objects. These constructor methods are divided into two
     parts: "Helper Constructor Methods", that are used to construct PyI40AAS types without a `modelType` attribute as
     embedded objects within other PyI40AAS objects, and "Direct Constructor Methods" for PyI40AAS type
@@ -107,27 +122,30 @@
     the `modelType` attribute.
 
     This class may be subclassed to override some of the constructor functions, e.g. to construct objects of specialized
     subclasses of the PyI40AAS object classes instead of these normal classes from the `model` package. To simplify this
     tasks, (nearly) all the constructor methods take a parameter `object_type` defaulting to the normal PyI40AAS object
     class, that can be overridden in a derived function:
 
+    .. code-block:: python
+
         class EnhancedAsset(model.Asset):
             pass
 
         class EnhancedAASDecoder(AASFromJsonDecoder):
             @classmethod
             def _construct_asset(cls, dct):
                 return super()._construct_asset(dct, object_class=EnhancedAsset)
 
-    :cvar failsafe: If True (the default), don't raise Exceptions for missing attributes and wrong types, but instead
+
+    :cvar failsafe: If `True` (the default), don't raise Exceptions for missing attributes and wrong types, but instead
                     skip defective objects and use logger to output warnings. Use StrictAASFromJsonDecoder for a
                     non-failsafe version.
-    :cvar stripped: If True, the JSON objects will be parsed in a stripped manner, excluding some attributes.
-                    Defaults to False.
+    :cvar stripped: If `True`, the JSON objects will be parsed in a stripped manner, excluding some attributes.
+                    Defaults to `False`.
                     See https://git.rwth-aachen.de/acplt/pyi40aas/-/issues/91
     """
     failsafe = True
     stripped = False
 
     def __init__(self, *args, **kwargs):
         json.JSONDecoder.__init__(self, object_hook=self.object_hook, *args, **kwargs)
@@ -673,15 +691,15 @@
 
 
 class StrictAASFromJsonDecoder(AASFromJsonDecoder):
     """
     A strict version of the AASFromJsonDecoder class for deserializing Asset Administration Shell data from the
     official JSON format
 
-    This version has set failsafe = False, which will lead to Exceptions raised for every missing attribute or wrong
+    This version has set `failsafe = False`, which will lead to Exceptions raised for every missing attribute or wrong
     object type.
     """
     failsafe = False
 
 
 class StrippedAASFromJsonDecoder(AASFromJsonDecoder):
     """
@@ -699,19 +717,19 @@
 
 def _select_decoder(failsafe: bool, stripped: bool, decoder: Optional[Type[AASFromJsonDecoder]]) \
         -> Type[AASFromJsonDecoder]:
     """
     Returns the correct decoder based on the parameters failsafe and stripped. If a decoder class is given, failsafe
     and stripped are ignored.
 
-    :param failsafe: If true, a failsafe decoder is selected. Ignored if a decoder class is specified.
-    :param stripped: If true, a decoder for parsing stripped JSON objects is selected. Ignored if a decoder class is
+    :param failsafe: If `True`, a failsafe decoder is selected. Ignored if a decoder class is specified.
+    :param stripped: If `True`, a decoder for parsing stripped JSON objects is selected. Ignored if a decoder class is
                      specified.
     :param decoder: Is returned, if specified.
-    :return: A AASFromJsonDecoder (sub)class.
+    :return: An :class:`~.AASFromJsonDecoder` (sub)class.
     """
     if decoder is not None:
         return decoder
     if failsafe:
         if stripped:
             return StrippedAASFromJsonDecoder
         return AASFromJsonDecoder
@@ -724,27 +742,28 @@
 def read_aas_json_file_into(object_store: model.AbstractObjectStore, file: IO, replace_existing: bool = False,
                             ignore_existing: bool = False, failsafe: bool = True, stripped: bool = False,
                             decoder: Optional[Type[AASFromJsonDecoder]] = None) -> Set[model.Identifier]:
     """
     Read an Asset Administration Shell JSON file according to 'Details of the Asset Administration Shell', chapter 5.5
     into a given object store.
 
-    :param object_store: The object store in which the identifiable objects should be stored
+    :param object_store: The :class:`ObjectStore <aas.model.provider.AbstractObjectStore>` in which the identifiable
+                         objects should be stored
     :param file: A file-like object to read the JSON-serialized data from
     :param replace_existing: Whether to replace existing objects with the same identifier in the object store or not
     :param ignore_existing: Whether to ignore existing objects (e.g. log a message) or raise an error.
-                            This parameter is ignored if replace_existing is True.
-    :param failsafe: If true, the document is parsed in a failsafe way: missing attributes and elements are logged
+                            This parameter is ignored if replace_existing is `True`.
+    :param failsafe: If `True`, the document is parsed in a failsafe way: Missing attributes and elements are logged
                      instead of causing exceptions. Defect objects are skipped.
                      This parameter is ignored if a decoder class is specified.
-    :param stripped: If true, stripped JSON objects are parsed.
+    :param stripped: If `True`, stripped JSON objects are parsed.
                      See https://git.rwth-aachen.de/acplt/pyi40aas/-/issues/91
                      This parameter is ignored if a decoder class is specified.
     :param decoder: The decoder class used to decode the JSON objects
-    :return: A set of identifiers that were added to object_store
+    :return: A set of :class:`Identifiers <aas.model.base.Identifier>` that were added to object_store
     """
     ret: Set[model.Identifier] = set()
     decoder_ = _select_decoder(failsafe, stripped, decoder)
 
     # read, parse and convert JSON file
     data = json.load(file, cls=decoder_)
 
@@ -794,17 +813,18 @@
             else:
                 raise TypeError(error_message)
     return ret
 
 
 def read_aas_json_file(file: IO, **kwargs) -> model.DictObjectStore[model.Identifiable]:
     """
-    A wrapper of read_aas_json_file_into(), that reads all objects in an empty DictObjectStore. This function supports
-    the same keyword arguments as read_aas_json_file_into().
+    A wrapper of :meth:`~aas.adapter.json.json_deserialization.read_aas_json_file_into`, that reads all objects in an
+    empty :class:`~aas.model.provider.DictObjectStore`. This function supports the same keyword arguments as
+    :meth:`~aas.adapter.json.json_deserialization.read_aas_json_file_into`.
 
     :param file: A filename or file-like object to read the JSON-serialized data from
-    :param kwargs: Keyword arguments passed to read_aas_json_file_into()
-    :return: A DictObjectStore containing all AAS objects from the JSON file
+    :param kwargs: Keyword arguments passed to :meth:`~aas.adapter.json.json_deserialization.read_aas_json_file_into`
+    :return: A :class:`~aas.model.provider.DictObjectStore` containing all AAS objects from the JSON file
     """
     object_store: model.DictObjectStore[model.Identifiable] = model.DictObjectStore()
     read_aas_json_file_into(object_store, file, **kwargs)
     return object_store
```

### Comparing `pyi40aas-0.2.2/aas/adapter/json/aasJSONSchema.json` & `pyi40aas-0.2.3/aas/adapter/json/aasJSONSchema.json`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/adapter/json/json_serialization.py` & `pyi40aas-0.2.3/aas/adapter/json/json_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,35 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
+.. _adapter.json.json_serialization:
+
 Module for serializing Asset Administration Shell objects to the official JSON format
 
-The module provides an custom JSONEncoder class `AASToJsonEncoder` to be used with the Python standard `json` module.
-It contains a custom `default` function which converts PyI40AAS objects to simple python types for an automatic
-JSON serialization. Additionally, there's the `write_aas_json_file()` function, that takes a complete ObjectStore and
-writes all contained AAS objects into a JSON file.
-
-This job is performed in an iterative approach: The `default()` function gets called for every object and checks if an
-object is an PyI40AAS object. In this case, it calls a special function for the respective PyI40AAS class which converts
-the object (but not the contained objects) into a simple Python dict, which is serializable. Any contained
-PyI40AAS objects are included into the dict as they are to be converted later on. The special helper function
-`abstract_classes_to_json()` is called by most of the conversion functions to handle all the attributes of abstract base
-classes.
+The module provides an custom JSONEncoder classes :class:`~.AASToJsonEncoder` and :class:`~.StrippedAASToJsonEncoder`
+to be used with the Python standard `json` module. While the former serializes objects as defined in the specification,
+the latter serializes stripped objects, excluding some attributes
+(see https://git.rwth-aachen.de/acplt/pyi40aas/-/issues/91).
+Each class contains a custom :meth:`~.AASToJsonEncoder.default` function which converts PyI40AAS objects to simple
+python types for an automatic JSON serialization.
+To simplify the usage of this module, the :meth:`~aas.adapter.json.json_serialization.write_aas_json_file` and
+:meth:`~aas.adapter.json.json_serialization.object_store_to_json` are provided.
+The former is used to serialize a given :class:`~aas.model.provider.AbstractObjectStore` to a file, while the latter
+serializes the object store to a string and returns it.
+
+The serialization is performed in an iterative approach: The :meth:`~.AASToJsonEncoder.default` function gets called for
+every object and checks if an object is an PyI40AAS object. In this case, it calls a special function for the respective
+PyI40AAS class which converts the object (but not the contained objects) into a simple Python dict, which is
+serializable. Any contained  PyI40AAS objects are included into the dict as they are to be converted later on.
+The special helper function :meth:`~.AASToJsonEncoder._abstract_classes_to_json` is called by most of the conversion
+functions to handle all the attributes of abstract base classes.
 """
 import base64
 import inspect
 from typing import List, Dict, IO, Optional, Type
 import json
 
 from aas import model
@@ -31,25 +39,35 @@
 
 class AASToJsonEncoder(json.JSONEncoder):
     """
     Custom JSONDecoder class to use the `json` module for serializing Asset Administration Shell data into the
     official JSON format
 
     The class overrides the `default()` method to transform PyI40AAS objects into dicts that may be serialized by the
-    standard encode method. Typical usage:
+    standard encode method.
+
+    Typical usage:
+
+    .. code-block:: python
 
         json_string = json.dumps(data, cls=AASToJsonEncoder)
 
     :cvar stripped: If True, the JSON objects will be serialized in a stripped manner, excluding some attributes.
-                    Defaults to False.
+                    Defaults to `False`.
                     See https://git.rwth-aachen.de/acplt/pyi40aas/-/issues/91
     """
     stripped = False
 
     def default(self, obj: object) -> object:
+        """
+        The overwritten `default` method for `json.JSONEncoder`
+
+        :param obj: The object to serialize to json
+        :return: The serialized object
+        """
         if isinstance(obj, model.AssetAdministrationShell):
             return self._asset_administration_shell_to_json(obj)
         if isinstance(obj, model.Identifier):
             return self._identifier_to_json(obj)
         if isinstance(obj, model.AdministrativeInformation):
             return self._administrative_information_to_json(obj)
         if isinstance(obj, model.Reference):
@@ -711,35 +729,37 @@
 
 def object_store_to_json(data: model.AbstractObjectStore, stripped: bool = False,
                          encoder: Optional[Type[AASToJsonEncoder]] = None, **kwargs) -> str:
     """
     Create a json serialization of a set of AAS objects according to 'Details of the Asset Administration Shell',
     chapter 5.5
 
-    :param data: ObjectStore which contains different objects of the AAS meta model which should be serialized to a
+    :param data: :class:`ObjectStore <aas.model.provider.AbstractObjectStore>` which contains different objects of the
+                 AAS meta model which should be serialized to a
                  JSON file
     :param stripped: If true, objects are serialized to stripped json objects..
                      See https://git.rwth-aachen.de/acplt/pyi40aas/-/issues/91
                      This parameter is ignored if an encoder class is specified.
     :param encoder: The encoder class used to encoder the JSON objects
-    :param kwargs: Additional keyword arguments to be passed to json.dump()
+    :param kwargs: Additional keyword arguments to be passed to `json.dumps()`
     """
     encoder_ = _select_encoder(stripped, encoder)
     # serialize object to json
     return json.dumps(_create_dict(data), cls=encoder_, **kwargs)
 
 
 def write_aas_json_file(file: IO, data: model.AbstractObjectStore, stripped: bool = False,
                         encoder: Optional[Type[AASToJsonEncoder]] = None, **kwargs) -> None:
     """
     Write a set of AAS objects to an Asset Administration Shell JSON file according to 'Details of the Asset
     Administration Shell', chapter 5.5
 
     :param file: A file-like object to write the JSON-serialized data to
-    :param data: ObjectStore which contains different objects of the AAS meta model which should be serialized to a
+    :param data: :class:`ObjectStore <aas.model.provider.AbstractObjectStore>` which contains different objects of the
+                 AAS meta model which should be serialized to a
                  JSON file
     :param stripped: If true, objects are serialized to stripped json objects..
                      See https://git.rwth-aachen.de/acplt/pyi40aas/-/issues/91
                      This parameter is ignored if an encoder class is specified.
     :param encoder: The encoder class used to encoder the JSON objects
     :param kwargs: Additional keyword arguments to be passed to json.dumps()
     """
```

### Comparing `pyi40aas-0.2.2/aas/model/security.py` & `pyi40aas-0.2.3/aas/model/security.py`

 * *Files identical despite different names*

### Comparing `pyi40aas-0.2.2/aas/model/__init__.py` & `pyi40aas-0.2.3/aas/model/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 """
 This package contains a python implementation of the meta-model of the AssetAdministrationShell.
-The model is divided into 5 modules, splitting it where it in sensible parts. However, all classes (except for the
+The model is divided into 5 modules, splitting it in sensible parts. However, all classes (except for the
 specialized Concept Descriptions) are imported into this top-level package, for simple imports like
 
+.. code-block:: python
+
     from aas.model import AssetAdministrationShell, Asset, Submodel, Property
 
 The different modules are:
 
 aas.py
     The main module, implementing high-level structures, such as AssetAdministrationShell, Asset and ConceptDictionary.
 
 base.py
     Basic structures of the model, including all abstract classes and enumerations. This provides inheritance for the
     higher level structures.
 
+concept.py
+    :class:`~aas.model.concept.ConceptDescription` from the AAS meta model
+    as well as specialized :class:`ConceptDescriptions <aas.model.concept.ConceptDescription>` like
+    :class:`~aas.model.concept.IEC61360ConceptDescription`
+
 provider.py
-    Providers for AAS objects, in order to store and retrieve identifiable objects by their Identifier.
+    Providers for AAS objects, in order to store and retrieve :class:`~aas.model.base.Identifiable` objects by their
+    :class:`~aas.model.base.Identifier`.
 
 security.py
     Security model of the AAS. Currently not existing.
 
 submodel.py
     Meta-model of the submodels and events.
 """
```

### Comparing `pyi40aas-0.2.2/aas/model/aas.py` & `pyi40aas-0.2.3/aas/model/aas.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
 The main module of the AAS meta-model. It is used to define the class structures of high level elements such as
-AssetAdministrationShell and Asset.
+:class:`~.AssetAdministrationShell` and :class:`~.Asset`.
 
 This module contains the following classes from an up-to-down-level:
- - AssetAdministrationShell
- - Asset
- - View
+
+ - :class:`~.AssetAdministrationShell`
+ - :class:`~.Asset`
+ - :class:`~.View`
 """
 
 from typing import Optional, Set, Iterable, TYPE_CHECKING
 
 from . import base, concept
 from .security import Security
 from .submodel import Submodel
@@ -24,92 +25,87 @@
 
 class View(base.Referable, base.HasSemantics):
     """
     A view is a collection of referable elements w.r.t. to a specific viewpoint of one or more stakeholders.
 
     todo: what does this exactly?
 
-    :ivar contained_element: Unordered list of references to elements of class Referable
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar contained_element: Unordered list of :class:`References <aas.model.base.Reference>` to elements of class
+        :class:`~aas.model.base.Referable`
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                     It affects the expected existence of attributes and the applicability of constraints.
+                     (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next :class:`~aas.model.base.Referable` parent element of
+        the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: :class:`~aas.model.base.Identifier` of the semantic definition of the element. It is called
+        semantic id of the element. The semantic id may either reference an external global id or it may reference a
+        :class:`~aas.model.base.Referable` model element of kind=Type that defines the semantics of the element.
+        (inherited from :class:`~aas.model.base.HasSemantics`)
     """
     def __init__(self,
                  id_short: str,
                  contained_element: Optional[Set[base.AASReference]] = None,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None):
         """
-        Initializer of View
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param contained_element: Unordered list of references to elements of class Referable
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
         TODO: Add instruction what to do after construction
         """
-
         super().__init__()
         self.id_short = id_short
         self.contained_element: Set[base.AASReference] = set() if contained_element is None else contained_element
         self.category: Optional[str] = category
         self.description: Optional[base.LangStringSet] = dict() if description is None else description
         self.parent: Optional[base.Namespace] = parent
         self.semantic_id: Optional[base.Reference] = semantic_id
 
 
 class Asset(base.Identifiable):
     """
     An Asset describes meta data of an asset that is represented by an AAS
 
-    The asset may either represent an asset type or an asset instance. The asset has a globally unique identifier plus
-    – if needed – additional domain specific (proprietary) identifiers.
+    The asset may either represent an asset type or an asset instance. The asset has a globally unique
+    :class:`~aas.model.base.Identifier` plus – if needed – additional domain specific (proprietary) identifiers.
 
     :ivar kind: Denotes whether the Asset is of kind "Type" or "Instance".
-    :ivar asset_identification_model: A reference to a Submodel that defines the handling of additional domain
+    :ivar ~.identification: The globally unique identification of the element.
+        (inherited from :class:`~aas.model.base.Identifiable`)
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                     It affects the expected existence of attributes and the applicability of constraints.
+                     (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next :class:`~aas.model.base.Referable` parent element of
+        the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar administration: Administrative information of an :class:`~aas.model.base.Identifiable` element.
+        (inherited from :class:`~aas.model.base.Identifiable`)
+    :ivar asset_identification_model: A :class:`~aas.model.base.AASReference` to a :class:`~aas.model.submodel.Submodel`
+                                      that defines the handling of additional domain
                                       specific (proprietary) Identifiers for the asset like e.g. serial number etc
-    :ivar bill_of_material: Bill of material of the asset represented by a submodel of the same AAS. This submodel
+    :ivar bill_of_material: Bill of material of the asset represented by a :class:`~aas.model.submodel.Submodel` of the
+                            same AAS. This submodel
                             contains a set of entities describing the material used to compose the composite I4.0
                             Component.
     """
 
     def __init__(self,
                  kind: base.AssetKind,
                  identification: base.Identifier,
                  id_short: str = "",
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  administration: Optional[base.AdministrativeInformation] = None,
                  asset_identification_model: Optional[base.AASReference[Submodel]] = None,
                  bill_of_material: Optional[base.AASReference[Submodel]] = None):
-        """
-        Initializer of Asset
-
-        :param kind: Denotes whether the Asset is of kind "Type" or "Instance".
-        :param identification: The globally unique identification of the element. (from base.Identifiable)
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param administration: Administrative information of an identifiable element. (from base.Identifiable)
-        :param asset_identification_model: A reference to a Submodel that defines the handling of additional domain
-                                           specific (proprietary) Identifiers for the asset like e.g. serial number etc
-        :param bill_of_material: Bill of material of the asset represented by a submodel of the same AAS. This submodel
-                                 contains a set of entities describing the material used to compose the composite I4.0
-                                 Component.
-        """
         super().__init__()
         self.kind: base.AssetKind = kind
         self.identification: base.Identifier = identification
         self.id_short = id_short
         self.category: Optional[str] = category
         self.description: Optional[base.LangStringSet] = dict() if description is None else description
         self.parent: Optional[base.Namespace] = parent
@@ -118,54 +114,49 @@
         self.bill_of_material: Optional[base.AASReference[Submodel]] = bill_of_material
 
 
 class AssetAdministrationShell(base.Identifiable, base.Namespace):
     """
     An Asset Administration Shell
 
-    :ivar asset: reference to the asset the AAS is representing.
-    :ivar security: Definition of the security relevant aspects of the AAS.
-    :ivar submodel: Unordered list of submodels to describe typically the asset of an AAS.
-    :ivar concept_dictionary: Unordered list of concept dictionaries. The concept dictionaries typically contain only
+    :ivar asset: :class:`~aas.model.base.Reference` to the :class:`~.Asset` the AAS is representing.
+    :ivar ~.identification: The globally unique identification of the element.
+        (inherited from :class:`~aas.model.base.Identifiable`)
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                     It affects the expected existence of attributes and the applicability of constraints.
+                     (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next :class:`~aas.model.base.Referable` parent element of
+        the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar administration: Administrative information of an :class:`~aas.model.base.Identifiable` element.
+        (inherited from :class:`~aas.model.base.Identifiable`)
+    :ivar ~.security: Definition of the security relevant aspects of the AAS.
+    :ivar ~.submodel: Unordered list of :class:`AASReferences <aas.model.base.AASReference>` to
+        :class:`Submodels <aas.model.submodel.Submodel>` to describe typically the asset of an AAS.
+    :ivar concept_dictionary: Unordered list of :class:`ConceptDictionaries <aas.model.concept.ConceptDictionary>`.
+                              The concept dictionaries typically contain only
                               descriptions for elements that are also used within the AAS
-    :ivar view: Unordered list of stakeholder specific views that can group the elements of the AAS.
-    :ivar derived_from: The reference to the AAS the AAs was derived from
+    :ivar view: Unordered list of stakeholder specific :class:`Views <~.View>` that can group the elements of the AAS.
+    :ivar derived_from: The :class:`~aas.model.base.AASReference` to the AAS the AAs was derived from
     """
     def __init__(self,
                  asset: base.AASReference[Asset],
                  identification: base.Identifier,
                  id_short: str = "",
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  administration: Optional[base.AdministrativeInformation] = None,
                  security: Optional[Security] = None,
                  submodel: Optional[Set[base.AASReference[Submodel]]] = None,
                  concept_dictionary: Iterable[concept.ConceptDictionary] = (),
                  view: Iterable[View] = (),
                  derived_from: Optional[base.AASReference["AssetAdministrationShell"]] = None):
-        """
-        Initializer of AssetAdministrationShell
-        :param asset: reference to the asset the AAS is representing.
-        :param identification: The globally unique identification of the element. (from base.Identifiable)
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param administration: Administrative information of an identifiable element. (from base.Identifiable)
-        :param security: Definition of the security relevant aspects of the AAS.
-        :param submodel: Unordered list of submodels to describe typically the asset of an AAS.
-        :param concept_dictionary: Unordered list of concept dictionaries. The concept dictionaries typically contain
-                                   only descriptions for elements that are also used within the AAS
-        :param view: Unordered list of stakeholder specific views that can group the elements of the AAS.
-        :param derived_from: The reference to the AAS the AAS was derived from
-        """
-
         super().__init__()
         self.identification: base.Identifier = identification
         self.id_short = id_short
         self.category: Optional[str] = category
         self.description: Optional[base.LangStringSet] = dict() if description is None else description
         self.parent: Optional[base.Namespace] = parent
         self.administration: Optional[base.AdministrativeInformation] = administration
```

### Comparing `pyi40aas-0.2.2/aas/model/datatypes.py` & `pyi40aas-0.2.3/aas/model/datatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 
 See https://www.w3.org/TR/xmlschema-2/#built-in-datatypes for the XSD simple type hierarchy and more information on the
 datatypes. All types from this type hierarchy (except for `token` and its descendants) are implemented or aliased in
 this module using their pythonized: Duration, DateTime, GMonthDay, String, Integer, Decimal, Short …. These types are
 meant to be used directly for data values in the context of Asset Administration Shells.
 
 There are three conversion functions for useage in PyI40AAS' model and adapters:
-* `xsd_repr()` serializes any XSD type from this module into it's lexical representation
-* `from_xsd()` parses an XSD type from its lexical representation (its required to name the type for unambiguous
-  conversion)
-* `trivial_cast()` type-cast a python value into an XSD type, if this is trivially possible. Meant for fixing the type
-  of Properties' values automatically, esp. for literal values.
+
+* :meth:`~aas.model.datatypes.xsd_repr` serializes any XSD type from this module into it's lexical representation
+* :meth:`~aas.model.datatypes.from_xsd` parses an XSD type from its lexical representation (its required to name the
+  type for unambiguous conversion)
+* :meth:`~aas.model.datatypes.trivial_cast` type-cast a python value into an XSD type, if this is trivially possible.
+  Meant for fixing the type of Properties' values automatically, esp. for literal values.
 """
 import base64
 import datetime
 import decimal
 import re
 from typing import Type, Union, Dict, Optional
```

### Comparing `pyi40aas-0.2.2/aas/model/concept.py` & `pyi40aas-0.2.3/aas/model/concept.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,95 +2,90 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
-This module contains the classes `ConceptDescription` and `ConceptDictionary` from the AAS meta model as well as
-specialized ConceptDescriptions like `IEC61360ConceptDescription`.
+This module contains the classes :class:`~.ConceptDescription` and :class:`~.ConceptDictionary` from the AAS meta model
+as well as specialized ConceptDescriptions like :class:`~.IEC61360ConceptDescription`.
 """
 from enum import unique, Enum
 from typing import Optional, Set, Type
 
 from . import base, datatypes
 
 
 class ConceptDescription(base.Identifiable):
     """
-    The semantics of a property or other elements that may have a semantic description is defined by a concept
-    description.
+    The semantics of a :class:`~.Property` or other elements that may have a semantic description is defined by a
+    concept description.
 
     The description of the concept should follow a standardized schema (realized as data specification template).
 
-    :ivar is_case_of: Unordered list of global references to external definitions the concept is compatible to or was
-                      derived from.
-                      Note: Compare to is-case-of relationship in ISO 13584-32 & IEC EN 61360
+    :ivar ~.identification: The globally unique identification of the element.
+            (inherited from :class:`~aas.model.base.Identifiable`)
+    :ivar is_case_of: Unordered list of global :class:`References <aas.model.base.Reference>` to external definitions
+        the concept is compatible to or was derived from.
+        *Note:* Compare to is-case-of relationship in ISO 13584-32 & IEC EN 61360
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                     It affects the expected existence of attributes and the applicability of constraints.
+                     (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next :class:`~aas.model.base.Referable` parent element of
+        the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar administration: Administrative information of an :class:`~aas.model.base.Identifiable` element.
+        (inherited from :class:`~aas.model.base.Identifiable`)
     """
 
     def __init__(self,
                  identification: base.Identifier,
                  is_case_of: Optional[Set[base.Reference]] = None,
                  id_short: str = "",
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  administration: Optional[base.AdministrativeInformation] = None):
-        """
-        Initializer of ConceptDescription
-
-        :param identification: The globally unique identification of the element. (from base.Identifiable)
-        :param is_case_of: Unordered list of global references to external definitions the concept is compatible to or
-                           was derived from.
-                           Note: Compare to is-case-of relationship in ISO 13584-32 & IEC EN 61360
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param administration: Administrative information of an identifiable element. (from base.Identifiable)
-        """
         super().__init__()
         self.identification: base.Identifier = identification
         self.is_case_of: Set[base.Reference] = set() if is_case_of is None else is_case_of
         self.id_short = id_short
         self.category: Optional[str] = category
         self.description: Optional[base.LangStringSet] = dict() if description is None else description
         self.parent: Optional[base.Namespace] = parent
         self.administration: Optional[base.AdministrativeInformation] = administration
 
 
 class ConceptDictionary(base.Referable):
     """
-    A dictionary containing concept descriptions.
+    A dictionary containing :class:`ConceptDescriptions <.ConceptDescription>`.
 
     Typically a concept description dictionary of an AAS contains only concept descriptions of elements used within
     submodels of the AAS.
 
-
-    :param concept_description: Unordered list of references to elements of class ConceptDescription
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                     It affects the expected existence of attributes and the applicability of constraints.
+                     (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next :class:`~aas.model.base.Referable` parent element of
+        the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar concept_description: Unordered list of :class:`References <aas.model.base.AASReference>` to elements of class
+        :class:`~.ConceptDescription`
     """
     def __init__(self,
                  id_short: str,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  concept_description: Optional[Set[base.AASReference[ConceptDescription]]] = None):
         """
-        Initializer of ConceptDictionary
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints. (from
-                         base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param concept_description: Unordered list of references to elements of class ConceptDescription
-
         TODO: Add instruction what to do after construction
         """
         super().__init__()
         self.id_short = id_short
         self.category: Optional[str] = category
         self.description: Optional[base.LangStringSet] = dict() if description is None else description
         self.parent: Optional[base.Namespace] = parent
@@ -128,15 +123,43 @@
     MAX = 1
     NOM = 2
     TYP = 3
 
 
 class IEC61360ConceptDescription(ConceptDescription):
     """
-    A specialized ConceptDescription to define concepts according to IEC61360
+    A specialized :class:`~.ConceptDescription` to define concepts according to IEC61360
+
+    :ivar ~.identification: The globally unique identification of the element.
+            (inherited from :class:`~aas.model.base.Identifiable`)
+    :ivar preferred_name: Preferred of the data object
+    :ivar data_type: Data type of the data object
+    :ivar definition: Definition of the data object
+    :ivar short_name: Short name of the data object
+    :ivar is_case_of: Unordered list of global :class:`References <aas.model.base.Reference>` to external definitions
+        the concept is compatible to or was derived from.
+        *Note:* Compare to is-case-of relationship in ISO 13584-32 & IEC EN 61360
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                     It affects the expected existence of attributes and the applicability of constraints.
+                     (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next :class:`~aas.model.base.Referable` parent element of
+        the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar administration: Administrative information of an :class:`~aas.model.base.Identifiable` element.
+        (inherited from :class:`~aas.model.base.Identifiable`)
+    :ivar unit_id: Reference to a unit id (optional)
+    :ivar source_of_definition: Source of the definition (optional)
+    :ivar symbol: Unit symbol (optional)
+    :ivar value_format: Format of the values (optional)
+    :ivar value_list: List of values (optional)
+    :ivar value: Value data type object (optional)
+    :ivar value_id: :class:`~aas.model.base.Reference` to the value (optional)
+    :ivar level_types: Set of level types of the DataSpecificationContent (optional)
     """
     def __init__(self,
                  identification: base.Identifier,
                  preferred_name: base.LangStringSet,
                  data_type: Optional[IEC61360DataType] = None,
                  definition: Optional[base.LangStringSet] = None,
                  short_name: Optional[base.LangStringSet] = None,
@@ -152,42 +175,14 @@
                  symbol: Optional[str] = None,
                  value_format: base.DataTypeDef = None,
                  value_list: Optional[base.ValueList] = None,
                  value: Optional[base.ValueDataType] = None,
                  value_id: Optional[base.Reference] = None,
                  level_types: Set[IEC61360LevelType] = None,
                  ):
-        """
-        Initializer of IEC61360ConceptDescription
-
-        :param identification: The globally unique identification of the element. (from base.Identifiable)
-        :param preferred_name: preferred of the data object
-        :param short_name: short name of the data object
-        :param data_type: data type of the data object
-        :param definition: definition of the data object
-        :param is_case_of: Unordered list of global references to external definitions the concept is compatible to or
-                           was derived from.
-                           Note: Compare to is-case-of relationship in ISO 13584-32 & IEC EN 61360
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints. (from
-                         base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param administration: Administrative information of an identifiable element. (from base.Identifiable)
-        :param unit: unit of the data object (optional)
-        :param unit_id: reference to a unit id (optional)
-        :param source_of_definition: source of the definition (optional)
-        :param symbol: unit symbol (optional)
-        :param value_format: format of the values (optional)
-        :param value_list: list of values (optional)
-        :param value: value data type object (optional)
-        :param value_id: Reference to the value (optional)
-        :param level_types: Set of level types of the DataSpecificationContent (optional)
-        """
         super().__init__(identification, is_case_of, id_short, category, description, parent, administration)
         self.preferred_name: base.LangStringSet = preferred_name
         self.short_name: Optional[base.LangStringSet] = short_name
         self.data_type: Optional[IEC61360DataType] = data_type
         self.definition: Optional[base.LangStringSet] = definition
         self.unit: Optional[str] = unit
         self.unit_id: Optional[base.Reference] = unit_id
```

### Comparing `pyi40aas-0.2.2/aas/model/submodel.py` & `pyi40aas-0.2.3/aas/model/submodel.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,30 +33,14 @@
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of SubmodelElement
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__()
         self.id_short = id_short
         self.category: Optional[str] = category
         self.description: Optional[base.LangStringSet] = dict() if description is None else description
@@ -70,49 +54,48 @@
     """
     A Submodel defines a specific aspect of the asset represented by the AAS.
 
     A submodel is used to structure the virtual representation and technical functionality of an Administration Shell
     into distinguishable parts. Each submodel refers to a well-defined domain or subject matter. Submodels can become
     standardized and thus become submodels types. Submodels can have different life-cycles.
 
-    :ivar submodel_element: Unordered list of submodel elements
+    :ivar ~.identification: The globally unique :class:`~aas.model.base.Identification` of the element.
+        (inherited from :class:`~aas.model.base.Identifiable`)
+    :ivar submodel_element: Unordered list of :class:`SubmodelElements <.SubmodelElement>`
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar administration: :class:`~aas.model.base.AdministrativeInformation` of an :class:`~aas.model.base.Identifiable`
+        element. (inherited from :class:`~aas.model.base.Identifiable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  identification: base.Identifier,
                  submodel_element: Iterable[SubmodelElement] = (),
                  id_short: str = "",
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  administration: Optional[base.AdministrativeInformation] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
-        """
-        Initializer of Submodel
-
-        :param identification: The globally unique identification of the element. (from base.Identifiable)
-        :param submodel_element: Unordered list of submodel elements
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param administration: Administrative information of an identifiable element. (from base.Identifiable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-        """
-
         super().__init__()
         self.identification: base.Identifier = identification
         self.submodel_element = base.NamespaceSet(self, submodel_element)
         self.id_short = id_short
         self.category: Optional[str] = category
         self.description: Optional[base.LangStringSet] = dict() if description is None else description
         self.parent: Optional[base.Namespace] = parent
@@ -124,88 +107,85 @@
 
 class DataElement(SubmodelElement, metaclass=abc.ABCMeta):
     """
     A data element is a submodel element that is not further composed out of other submodel elements.
     A data element is a submodel element that has a value. The type of value differs for different subtypes
     of data elements.
 
-    << abstract >>
+    <<abstract>>
+
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
     @abc.abstractmethod
     def __init__(self,
                  id_short: str,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
-        """
-        Initializer of DataElement
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-        """
-
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
 
 
 class Property(DataElement):
     """
-    A property is a data element that has a single value.
+    A property is a :class:`~.DataElement` that has a single value.
+
+    **Constraint AASd-007:** if both, the value and the valueId are present then the value needs to be
+    identical to the value of the referenced coded value in valueId
 
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
     :ivar value_type: Data type of the value
     :ivar value: The value of the property instance.
-    :ivar value_id: Reference to the global unique id of a coded value.
-                    Constraint AASd-007: if both, the value and the valueId are present then the value needs to be
-                                         identical to the value of the referenced coded value in valueId
+    :ivar value_id: :class:`~aas.model.base.Reference` to the global unique id of a coded value
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  id_short: str,
                  value_type: base.DataTypeDef,
                  value: Optional[base.ValueDataType] = None,
                  value_id: Optional[base.Reference] = None,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of Property
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param value_type: Data type of the value
-        :param value: The value of the property instance.
-        :param value_id: Reference to the global unique id of a coded value.
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.value_type: Type[datatypes.AnyXSDType] = value_type
         self._value: Optional[base.ValueDataType] = (datatypes.trivial_cast(value, value_type)
                                                      if value is not None else None)
@@ -223,102 +203,98 @@
             self._value = datatypes.trivial_cast(value, self.value_type)
 
 
 class MultiLanguageProperty(DataElement):
     """
     A property is a data element that has a multi language value.
 
+    **Constraint AASd-012:** if both, the value and the valueId are present then for each string in a
+    specific language the meaning must be the same as specified in valueId.
+
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
     :ivar value: The value of the property instance.
-    :ivar value_id: Reference to the global unique id of a coded value.
-                    Constraint AASd-012: if both, the value and the valueId are present then for each string in a
-                                         specific language the meaning must be the same as specified in valueId.
+    :ivar value_id: :class:`~aas.model.base.Reference` to the global unique id of a coded value.
+
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  id_short: str,
                  value: Optional[base.LangStringSet] = None,
                  value_id: Optional[base.Reference] = None,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of MultiLanguageProperty
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param value: The value of the property instance.
-        :param value_id: Reference to the global unique id of a coded value.
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                           (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.value: base.LangStringSet = dict() if value is None else value
         self.value_id: Optional[base.Reference] = value_id
 
 
 class Range(DataElement):
     """
-    A property is a data element that has a multi language value.
+    A range data element is a data element that defines a range with min and max.
+
+    **Constraint AASd-013:** In case of a range with kind=Instance either the min or the max value or both need
+    to be defined
 
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
     :ivar value_type: Data type of the min and max
     :ivar min: The minimum value of the range. If the min value is missing then the value is assumed to be negative
                 infinite.
-                Constraint AASd-013: In case of a range with kind=Instance either the min or the max value or both need
-                                     to be defined
     :ivar max: The maximum of the range. If the max value is missing then the value is assumed to be positive infinite
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  id_short: str,
                  value_type: base.DataTypeDef,
                  min: Optional[base.ValueDataType] = None,
                  max: Optional[base.ValueDataType] = None,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of Range
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param value_type: Data type of the min and max
-        :param min: The minimum value of the range. If the min value is missing then the value is assumed to be
-                     negative infinite.
-        :param max: The maximum of the range. If the max value is missing then the value is assumed to be positive
-                     infinite
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.value_type: base.DataTypeDef = value_type
         self._min: Optional[base.ValueDataType] = datatypes.trivial_cast(min, value_type) if min is not None else None
         self._max: Optional[base.ValueDataType] = datatypes.trivial_cast(max, value_type) if max is not None else None
@@ -346,378 +322,362 @@
             self._max = datatypes.trivial_cast(value, self.value_type)
 
 
 class Blob(DataElement):
     """
     A BLOB is a data element that represents a file that is contained with its source code in the value attribute.
 
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
     :ivar value: The value of the BLOB instance of a blob data element.
-                 Note: In contrast to the file property the file content is stored directly as value in
+                 *Note:* In contrast to the file property the file content is stored directly as value in
                  the Blob data element.
     :ivar mime_type: Mime type of the content of the BLOB. The mime type states which file extension the file has.
                      Valid values are e.g. “application/json”, “application/xls”, ”image/jpg”. The allowed values
                      are defined as in RFC2046.
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
+
     """
 
     def __init__(self,
                  id_short: str,
                  mime_type: base.MimeType,
                  value: Optional[base.BlobType] = None,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of Blob
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param value: The value of the BLOB instance of a blob data element.
-                      Note: In contrast to the file property the file content is stored directly as value in the Blob
-                            data element.
-        :param mime_type: Mime type of the content of the BLOB. The mime type states which file extension the file has.
-                          Valid values are e.g. “application/json”, “application/xls”, ”image/jpg”. The allowed values
-                          are defined as in RFC2046.
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.value: Optional[base.BlobType] = value
         self.mime_type: base.MimeType = mime_type
 
 
 class File(DataElement):
     """
     A File is a data element that represents a file via its path description.
 
-    :ivar value: Path and name of the referenced file (without file extension). The path can be absolute or relative.
-                 Note: The file extension is defined by using a qualifier of type “MimeType”.
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
     :ivar mime_type: Mime type of the content of the File.
+    :ivar value: Path and name of the referenced file (without file extension). The path can be absolute or relative.
+                 *Note:* The file extension is defined by using a qualifier of type “MimeType”.
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  id_short: str,
                  mime_type: base.MimeType,
                  value: Optional[base.PathType] = None,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of File
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param mime_type: Mime type of the content of the File.
-        :param value: Path and name of the referenced file (without file extension). The path can be absolute or
-                      relative.
-                      Note: The file extension is defined by using a qualifier of type “MimeType”.
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.value: Optional[base.PathType] = value
         self.mime_type: base.MimeType = mime_type
 
 
 class ReferenceElement(DataElement):
     """
-    A reference element is a data element that defines a reference to another element within the same or another AAS
-    or a reference to an external object or entity.
+    A reference element is a data element that defines a :class:`~aas.model.base.Reference` to another element within
+    the same or another AAS or a reference to an external object or entity.
 
-    :ivar value: Reference to any other referable element of the same of any other AAS
-                 or a reference to an external object or entity.
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar value: :class:`~aas.model.base.Reference` to any other :class:`~aas.model.base.Referable` element of the same
+                 of any other AAS or a reference to an external object or entity.
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  id_short: str,
                  value: Optional[base.Reference] = None,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of ReferenceElement
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param value: Reference to any other referable element of the same of any other AAS or a reference to an
-                      external object or entity.
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.value: Optional[base.Reference] = value
 
 
 class SubmodelElementCollection(SubmodelElement, base.Namespace, metaclass=abc.ABCMeta):
     """
     A submodel element collection is a set or list of submodel elements.
 
-    << abstract >>
+    <<abstract>>
 
-    :ivar value: Ordered or unordered list of submodel elements
-    :ivar ordered: If ordered=false then the elements in the property collection are not ordered. If ordered=true then
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar value: Ordered or unordered list of :class:`SubmodelElements <.SubmodelElement>`
+    :ivar ordered: If `ordered=False` then the elements in the property collection are not ordered. If `ordered=True`
+                   then
                    the elements in the collection are ordered.
                    `ordered` shall not be set directly, instead one of the subclasses
-                   `SubmodelElementCollectionOrdered` or `SubmodelElementCollectionUnordered` shall be used.
+                   :class:`~.SubmodelElementCollectionOrdered` or :class:`~.SubmodelElementCollectionUnordered` shall
+                   be used.
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
     @abc.abstractmethod
     def __init__(self,
                  id_short: str,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of SubmodelElementCollection
-
-        This class is abstract and should not used for instances; instead one of the subclasses
-        `SubmodelElementCollectionOrdered` or `SubmodelElementCollectionUnordered` shall be used.
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.value: base.NamespaceSet[SubmodelElement] = None  # type: ignore
 
     @property
     @abc.abstractmethod
-    def ordered(self):
+    def ordered(self) -> bool:
         pass
 
 
 class SubmodelElementCollectionOrdered(SubmodelElementCollection):
     """
-    A SubmodelElementCollectionOrdered is an ordered list of submodel elements.
+    A SubmodelElementCollectionOrdered is an ordered list of :class:`SubmodelElements <.SubmodelElement>`.
+
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar value: Ordered or unordered list of :class:`SubmodelElements <.SubmodelElement>`
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  id_short: str,
                  value: Iterable[SubmodelElement] = (),
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of SubmodelElementCollection
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param value: Ordered list of submodel elements.
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.value = base.OrderedNamespaceSet(self, value)
 
     @property
-    def ordered(self):
+    def ordered(self) -> bool:
         return True
 
 
 class SubmodelElementCollectionUnordered(SubmodelElementCollection):
     """
-    A SubmodelElementCollectionOrdered is an unordered list of submodel elements.
+    A SubmodelElementCollectionOrdered is an unordered list of :class:`SubmodelElements <.SubmodelElement>`.
+
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar value: Ordered or unordered list of :class:`SubmodelElements <.SubmodelElement>`
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  id_short: str,
                  value: Iterable[SubmodelElement] = (),
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of SubmodelElementCollection
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param value: Unordered list of submodel elements.
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.value = base.NamespaceSet(self, value)
 
     @property
-    def ordered(self):
+    def ordered(self) -> bool:
         return False
 
 
 class RelationshipElement(SubmodelElement):
     """
     A relationship element is used to define a relationship between two referable elements.
 
-    :ivar first: Reference to the first element in the relationship taking the role of the subject which have to be of
-                 class Referable.
-
-    :ivar second: Reference to the second element in the relationship taking the role of the object which have to be of
-                 class Referable.
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar first: :class:`~aas.model.base.Reference` to the first element in the relationship taking the role of the
+        subject which have to be of class :class:`~aas.model.base.Referable`.
+    :ivar second: :class:`~aas.model.base.Reference` to the second element in the relationship taking the role of the
+        object which have to be of class :class:`~aas.model.base.Referable`.
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  id_short: str,
                  first: base.AASReference,
                  second: base.AASReference,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of RelationshipElement
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param first: Reference to the first element in the relationship taking the role of the subject which have to
-                      be of class Referable.
-        :param second: Reference to the second element in the relationship taking the role of the object which have to
-                       be of class Referable.
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.first: base.AASReference = first
         self.second: base.AASReference = second
 
 
 class AnnotatedRelationshipElement(RelationshipElement, base.Namespace):
     """
     An annotated relationship element is a relationship element that can be annotated with additional data elements.
 
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
     :ivar annotation: Unordered list of annotations that hold for the relationship between to elements
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  id_short: str,
                  first: base.AASReference,
                  second: base.AASReference,
                  annotation: Optional[Iterable[DataElement]] = None,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of AnnotatedRelationshipElement
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param annotation: Unordered list of annotations that hold for the relationship between two elements
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, first, second, category, description, parent, semantic_id, qualifier, kind)
         if annotation is None:
             self.annotation: base.NamespaceSet[DataElement] = base.NamespaceSet(self)
         else:
@@ -731,151 +691,145 @@
     :ivar value: Describes the needed argument for an operation via a submodel element of kind=Type.
                  Constraint AASd-008: The submodel element value of an operation variable shall be of kind=Template.
     """
 
     def __init__(self,
                  value: SubmodelElement):
         """
-        Initializer of OperationVariable
-
-        :param value: Describes the needed argument for an operation via a submodel element of kind=Type.
-
         TODO: Add instruction what to do after construction
         """
         # Constraint AASd-008: The submodel element shall be of kind=Template.
         self.value: SubmodelElement = value  # TODO check the kind of the object in value
 
 
 class Operation(SubmodelElement):
     """
-    An operation is a submodel element with input and output variables.
+    An operation is a :class:`~.SubmodelElement` with input and output variables.
 
-    :ivar input_variable: list of input parameters of the operation
-    :ivar output_variable: of output parameters of the operation
-    :ivar in_output_variable: of parameters that are input and output of the operation
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar input_variable: list of input :class:`OperationVariables <.OperationVariable>` of the operation
+    :ivar output_variable: of output :class:`OperationVariables <.OperationVariable>` of the operation
+    :ivar in_output_variable: List of :class:`OperationVariables <.OperationVariable>` that are input and output
+        of the operation
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
     def __init__(self,
                  id_short: str,
                  input_variable: Optional[List[OperationVariable]] = None,
                  output_variable:  Optional[List[OperationVariable]] = None,
                  in_output_variable:  Optional[List[OperationVariable]] = None,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of Operation
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param input_variable: list of input parameters of the operation
-        :param output_variable: list output parameters of the operation
-        :param in_output_variable: list of parameters that is input and output of the operation
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.input_variable = input_variable if input_variable is not None else []
         self.output_variable = output_variable if output_variable is not None else []
         self.in_output_variable = in_output_variable if in_output_variable is not None else []
 
 
 class Capability(SubmodelElement):
     """
     A capability is the implementation-independent description of the potential of an asset to achieve a certain effect
     in the physical or virtual world
+
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  id_short: str,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of Capability
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
 
 
 class Entity(SubmodelElement, base.Namespace):
     """
     An entity is a submodel element that is used to model entities
 
+    **Constraint AASd-014:** The asset attribute must be set if entityType is set to “SelfManagedEntity”. It
+    is empty otherwise.
+
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
     :ivar entity_type: Describes whether the entity is a co-managed or a self-managed entity.
     :ivar statement: Unordered list of statements applicable to the entity, typically with a qualified value.
     :ivar asset: Reference to the asset the entity is representing.
-                 Constraint AASd-014: The asset attribute must be set if entityType is set to “SelfManagedEntity”. It
-                 is empty otherwise.
+
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  id_short: str,
                  entity_type: base.EntityType,
                  statement: Iterable[SubmodelElement] = (),
                  asset: Optional[base.AASReference["aas.Asset"]] = None,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of Entity
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param entity_type: Describes whether the entity is a co-managed or a self-managed entity.
-        :param statement: Unordered list of statements applicable to the entity, typically with a qualified value.
-        :param asset: Reference to the asset the entity is representing.
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.entity_type: base.EntityType = entity_type
         self.statement = base.NamespaceSet(self, statement)
         if self.entity_type == base.EntityType.SELF_MANAGED_ENTITY and asset is None:
@@ -885,77 +839,77 @@
         else:
             self.asset = None
 
 
 class Event(SubmodelElement, metaclass=abc.ABCMeta):
     """
     An event
+
+    <<abstract>>
+
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
     @abc.abstractmethod
     def __init__(self,
                  id_short: str,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
-        """
-        Initializer of Event
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-        """
-
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
 
 
 class BasicEvent(Event):
     """
     An event
 
-    :ivar observed: Reference to the data or other elements that are being observed
+    :ivar id_short: Identifying string of the element within its name space.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar observed: :class:`~aas.model.base.AASReference` to the data or other elements that are being observed
+    :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
+                    It affects the expected existence of attributes and the applicability of constraints.
+                    (inherited from :class:`~aas.model.base.Referable`)
+    :ivar description: Description or comments on the element. (inherited from :class:`~aas.model.base.Referable`)
+    :ivar parent: :class:`~aas.model.base.Reference` to the next referable parent element of the element.
+        (inherited from :class:`~aas.model.base.Referable`)
+    :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
+         element. The semantic id may either reference an external global id or it may reference a
+         referable model element of kind=Type that defines the semantics of the element.
+         (inherited from :class:`~aas.model.base.HasSemantics`)
+    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+         (inherited from :class:`~aas.model.base.Qualifiable`)
+    :ivar kind: Kind of the element: either type or instance. Default = Instance.
+        (inherited from :class:`~aas.model.base.HasKind`)
     """
 
     def __init__(self,
                  id_short: str,
                  observed: base.AASReference,
                  category: Optional[str] = None,
                  description: Optional[base.LangStringSet] = None,
                  parent: Optional[base.Namespace] = None,
                  semantic_id: Optional[base.Reference] = None,
                  qualifier: Optional[Set[base.Constraint]] = None,
                  kind: base.ModelingKind = base.ModelingKind.INSTANCE):
         """
-        Initializer of BasicEvent
-
-        :param id_short: Identifying string of the element within its name space. (from base.Referable)
-        :param observed: Reference to the data or other elements that are being observed
-        :param category: The category is a value that gives further meta information w.r.t. to the class of the element.
-                         It affects the expected existence of attributes and the applicability of constraints.
-                         (from base.Referable)
-        :param description: Description or comments on the element. (from base.Referable)
-        :param parent: Reference to the next referable parent element of the element. (from base.Referable)
-        :param semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the
-                            element. The semantic id may either reference an external global id or it may reference a
-                            referable model element of kind=Type that defines the semantics of the element.
-                            (from base.HasSemantics)
-        :param qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
-                          (from base.Qualifiable)
-        :param kind: Kind of the element: either type or instance. Default = Instance. (from base.HasKind)
-
         TODO: Add instruction what to do after construction
         """
 
         super().__init__(id_short, category, description, parent, semantic_id, qualifier, kind)
         self.observed: base.AASReference = observed
```

### Comparing `pyi40aas-0.2.2/aas/model/base.py` & `pyi40aas-0.2.3/aas/model/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,47 +54,49 @@
 
 @unique
 class KeyElements(Enum):
     """
     Enumeration for denoting which kind of entity is referenced. They can be categorized in ReferableElements,
     IdentifiableElements and other KeyElements
 
-    # IdentifiableElements starting from 0
-    :cvar ASSET: asset
-    :cvar ASSET_ADMINISTRATION_SHELL: asset administration shell
-    :cvar CONCEPT_DESCRIPTION: concept description
-    :cvar SUBMODEL: submodel
+    **IdentifiableElements starting from 0**
+
+    :cvar ASSET: :class:`~aas.model.aas.Asset`
+    :cvar ASSET_ADMINISTRATION_SHELL: :class:`~aas.model.aas.AssetAdministrationShell`
+    :cvar CONCEPT_DESCRIPTION: :class:`~aas.model.concept.ConceptDescription`
+    :cvar SUBMODEL: :class:`~aas.model.submodel.Submodel`
+
+    **ReferableElements starting from 1000**
 
-    # ReferableElements starting from 1000
     :cvar ACCESS_PERMISSION_RULE: access permission rule
-    :cvar ANNOTATED_RELATIONSHIP_ELEMENT: annotated relationship element
-    :cvar BASIC_EVENT: basic event
-    :cvar BLOB: blob
-    :cvar CAPABILITY: capability
-    :cvar CONCEPT_DICTIONARY: concept dictionary
-    :cvar DATA_ELEMENT: data element,
-                        Note: Date Element is abstract, i. e. if a key uses "DATA_ELEMENT" the reference may be
-                              Property, File etc.
-    :cvar ENTITY: entity
-    :cvar EVENT: event, Note: Event is abstract
-    :cvar FILE: file
+    :cvar ANNOTATED_RELATIONSHIP_ELEMENT: :class:`~aas.model.submodel.AnnotatedRelationshipElement`
+    :cvar BASIC_EVENT: :class:`~aas.model.submodel.BasicEvent`
+    :cvar BLOB: :class:`~aas.model.submodel.Blob`
+    :cvar CAPABILITY: :class:`~aas.model.submodel.Capability`
+    :cvar CONCEPT_DICTIONARY: :class:`~aas.model.concept.ConceptDictionary`
+    :cvar DATA_ELEMENT: :class:`~aas.model.submodel.DataElement` *Note:* Date Element is abstract, i. e. if a key uses
+        "DATA_ELEMENT" the reference may be Property, File etc.
+    :cvar ENTITY: :class:`~aas.model.submodel.Entity`
+    :cvar EVENT: :class:`~aas.model.submodel.Event`, *Note:* Event is abstract
+    :cvar FILE: :class:`~aas.model.submodel.File`
     :cvar MULTI_LANGUAGE_PROPERTY: property with a value that can be provided in multiple languages
-    :cvar OPERATION: operation
-    :cvar PROPERTY: property
-    :cvar RANGE: range with min and max
-    :cvar REFERENCE_ELEMENT: reference
-    :cvar RELATIONSHIP_ELEMENT: relationship
-    :cvar SUBMODEL_ELEMENT: submodel element,
-                            Note: Submodel Element is abstract, i.e. if a key uses “SUBMODEL_ELEMENT” the reference may
-                                  be a Property, a SubmodelElementCollection, an Operation etc.
-    :cvar SUBMODEL_ELEMENT_COLLECTION: collection of submodel elements
-    :cvar VIEW: view
+    :cvar OPERATION: :class:`~aas.model.submodel.Operation`
+    :cvar PROPERTY: :class:`~aas.model.submodel.Property`
+    :cvar RANGE: :class:`~aas.model.submodel.Range` with min and max
+    :cvar REFERENCE_ELEMENT: :class:`aas.model.submodel.ReferenceElement`
+    :cvar RELATIONSHIP_ELEMENT: :class:`~aas.model.submodel.RelationshipElement`
+    :cvar SUBMODEL_ELEMENT: :class:`~aas.model.submodel.SubmodelElement`, Note: Submodel Element is abstract,
+        i.e. if a key uses “SUBMODEL_ELEMENT” the reference may be a :class:`~aas.model.submodel.Property`, a
+        :class:`~aas.model.submodel.SubmodelElementCollection`, an :class:`~aas.model.submodel.Operation` etc.
+    :cvar SUBMODEL_ELEMENT_COLLECTION: :class:`~aas.model.submodel.SubmodelElementCollection`
+    :cvar VIEW: :class:`~aas.model.aas.View`
 
-    # KeyElements starting from 2000
-    :cvar GLOBAL_REFERENCE: reference to an element not belonging to an asset administration shel
+    **KeyElements starting from 2000**
+
+    :cvar GLOBAL_REFERENCE: reference to an element not belonging to an asset administration shell
     :cvar FRAGMENT_REFERENCE: unique reference to an element within a file. The file itself is assumed to be part of an
                              asset administration shell.
     """
 
     # IdentifiableElements starting from 0
     ASSET = 0
     ASSET_ADMINISTRATION_SHELL = 1
@@ -169,34 +171,34 @@
 
 @unique
 class ModelingKind(Enum):
     """
     Enumeration for denoting whether an element is a type or an instance.
 
     :cvar TEMPLATE: Software element which specifies the common attributes shared by all instances of the template
-    :cvar INSTANCE: concrete, clearly identifiable component of a certain template,
-                    Note: It becomes an individual entity of a template, for example a device model, by defining
-                          specific property values.
-                    Note: In an object oriented view, an instance denotes an object of a template (class).
+    :cvar INSTANCE: concrete, clearly identifiable component of a certain template.
+        *Note:*  It becomes an individual entity of a template, for example a device model, by defining
+        specific property values.
+        *Note:* In an object oriented view, an instance denotes an object of a template (class).
     """
 
     TEMPLATE = 0
     INSTANCE = 1
 
 
 @unique
 class AssetKind(Enum):
     """
     Enumeration for denoting whether an element is a type or an instance.
 
     :cvar TYPE: hardware or software element which specifies the common attributes shared by all instances of the type
     :cvar INSTANCE: concrete, clearly identifiable component of a certain type,
-                    Note: It becomes an individual entity of a type, for example a device, by defining specific
-                          property values.
-                    Note: In an object oriented view, an instance denotes an object of a class (of a type)
+                    *Note:* It becomes an individual entity of a type, for example a device, by defining specific
+                    property values.
+                    *Note:* In an object oriented view, an instance denotes an object of a class (of a type)
     """
 
     TYPE = 0
     INSTANCE = 1
 
 
 class Key:
@@ -216,26 +218,14 @@
 
     def __init__(self,
                  type_: KeyElements,
                  local: bool,
                  value: str,
                  id_type: KeyType):
         """
-        Initializer of Key
-
-        :param type_: Denote which kind of entity is referenced. In case type = GlobalReference then the element is a
-                      global unique id. In all other cases the key references a model element of the same or of another
-                      AAS. The name of the model element is explicitly listed.
-        :param local: Denotes if the key references a model element of the same AAS (=true) or not (=false). In case of
-                      local = false the key may reference a model element of another AAS or an entity outside any AAS
-                      that has a global unique id.
-        :param value: The key value, for example an IRDI if the idType=IRDI
-        :param id_type: Type of the key value. In case of idType = idShort local shall be true. In case
-                        type=GlobalReference idType shall not be IdShort.
-
         TODO: Add instruction what to do after construction
         """
         self.type: KeyElements
         self.local: bool
         self.value: str
         self.id_type: KeyType
         super().__setattr__('type', type_)
@@ -262,26 +252,26 @@
                 and self.type == other.type)
 
     def __hash__(self):
         return hash((self.id_type, self.value, self.local, self.type))
 
     def get_identifier(self) -> Optional["Identifier"]:
         """
-        Get an identifier object corresponding to this key, if it is a global key.
+        Get an :class:`~.Identifier` object corresponding to this key, if it is a global key.
 
-        :return: None if this is no global key, otherwise a corresponding identifier object
+        :return: None if this is no global key, otherwise a corresponding :class:`~.Identifier` object
         """
         if self.id_type.is_local_key_type:
             return None
         return Identifier(self.value, IdentifierType(self.id_type.value))
 
     @staticmethod
     def from_referable(referable: "Referable") -> "Key":
         """
-        Construct a key for a given Referable (or Identifiable) object
+        Construct a key for a given :class:`~.Referable` (or :class:`~.Identifiable`) object
         """
         # Get the `type` by finding the first class from the base classes list (via inspect.getmro), that is contained
         # in KEY_ELEMENTS_CLASSES
         from . import KEY_ELEMENTS_CLASSES
         try:
             key_type = next(iter(KEY_ELEMENTS_CLASSES[t]
                                  for t in inspect.getmro(type(referable))
@@ -297,31 +287,27 @@
             return Key(key_type, local, referable.id_short, KeyType.IDSHORT)
 
 
 class AdministrativeInformation:
     """
     Administrative meta-information for an element like version information.
 
+    **Constraint AASd-005:** A revision requires a version. This means, if there is no version there is no revision
+    either
+
     :ivar version: Version of the element.
     :ivar revision: Revision of the element.
-    Constraint AASd-005: A revision requires a version. This means, if there is no version there is no revision
-                         neither.
     """
 
     def __init__(self,
                  version: Optional[str] = None,
                  revision: Optional[str] = None):
         """
         Initializer of AdministrativeInformation
 
-        :param version: Version of the element.
-        :param revision: Revision of the element.
-
-        Constraint AASd-005: A revision requires a version. This means, if there is no version there is no revision
-                             neither.
         :raises ValueError: If version is None and revision is not None
 
         TODO: Add instruction what to do after construction
         """
         if version is None and revision is not None:
             raise ValueError("A revision requires a version. This means, if there is no version there is no revision "
                              "neither.")
@@ -335,41 +321,36 @@
         if self.version is None:
             raise ValueError("A revision requires a version. This means, if there is no version there is no revision "
                              "neither. Please set version first.")
         else:
             self._revision = revision
 
     def __eq__(self, other) -> bool:
+        if not isinstance(other, AdministrativeInformation):
+            return NotImplemented
         return self.version == other.version and self._revision == other._revision
 
     def __repr__(self) -> str:
         return "AdministrativeInformation(version={}, revision={})".format(self.version, self.revision)
 
     revision = property(_get_revision, _set_revision)
 
 
 class Identifier:
     """
     Used to uniquely identify an entity by using an identifier.
 
     :ivar id: Identifier of the element. Its type is defined in id_type.
-    :ivar id_type: Type of the Identifier, e.g. URI, IRDI etc. The supported Identifier types are defined in
-                   the enumeration "IdentifierType".
+    :ivar id_type: :class:`~.IdentifierType`, e.g. URI, IRDI etc.
     """
 
     def __init__(self,
                  id_: str,
                  id_type: IdentifierType):
         """
-        Initializer of Identifier
-
-        :param id_: Identifier of the element. Its type is defined in id_type.
-        :param id_type: Type of the Identifier, e.g. URI, IRDI etc. The supported Identifier types are defined in the
-                        enumeration "IdentifierType".
-
         TODO: Add instruction what to do after construction
         """
         self.id: str
         self.id_type: IdentifierType
         super().__setattr__('id', id_)
         super().__setattr__('id_type', id_type)
 
@@ -390,27 +371,31 @@
 
 
 class Referable(metaclass=abc.ABCMeta):
     """
     An element that is referable by its id_short. This id is not globally unique. This id is unique within
     the name space of the element.
 
-    << abstract >>
+    <<abstract>>
+
+    **Constraint AASd-001:** In case of a referable element not being an identifiable element this id is
+    mandatory and used for referring to the element in its name space.
+
+    **Constraint AASd-002:** idShort shall only feature letters, digits, underscore ("_"); starting
+    mandatory with a letter.
+
+    **Constraint AASd-003:** idShort shall be matched case insensitive.
+
+    **Constraint AASd-004:** Add parent in case of non identifiable elements.
 
     :ivar id_short: Identifying string of the element within its name space.
-                    Constraint AASd-001: In case of a referable element not being an identifiable element this id is
-                                         mandatory and used for referring to the element in its name space.
-                    Constraint AASd-002: idShort shall only feature letters, digits, underscore ("_"); starting
-                                         mandatory with a letter.
-                    Constraint AASd-003: idShort shall be matched case insensitive.
     :ivar category: The category is a value that gives further meta information w.r.t. to the class of the element.
                     It affects the expected existence of attributes and the applicability of constraints.
     :ivar description: Description or comments on the element.
     :ivar parent: Reference to the next referable parent element of the element.
-                  Constraint AASd-004: Add parent in case of non identifiable elements.
     :ivar source: Source of the object, an URI, that defines where this object's data originates from.
                   This is used to specify where the Referable should be updated from and committed to.
                   Default is an empty string, making it use the source of its ancestor, if possible.
     """
     @abc.abstractmethod
     def __init__(self):
         super().__init__()
@@ -457,17 +442,17 @@
         :raises ValueError: if the constraint is not fulfilled
         :raises KeyError: if the new idShort causes a name collision in the parent Namespace
         """
 
         if id_short is None and not hasattr(self, 'identification'):
             raise ValueError("The id_short for not identifiable elements is mandatory")
         test_id_short: str = str(id_short)
-        if not re.match("^[a-zA-Z0-9_]*$", test_id_short):
+        if not re.fullmatch("[a-zA-Z0-9_]*", test_id_short):
             raise ValueError("The id_short must contain only letters, digits and underscore")
-        if not re.match("^([a-zA-Z].*|)$", test_id_short):
+        if len(test_id_short) > 0 and not test_id_short[0].isalpha():
             raise ValueError("The id_short must start with a letter")
 
         if self.parent is not None and id_short != self.id_short:
             for set_ in self.parent.namespace_element_sets:
                 if id_short in set_:
                     raise KeyError("Referable with id_short '{}' is already present in the parent Namespace"
                                    .format(id_short))
@@ -604,15 +589,16 @@
 
 
 _RT = TypeVar('_RT', bound=Referable)
 
 
 class UnexpectedTypeError(TypeError):
     """
-    Exception to be raised by Reference.resolve() if the retrieved object has not the expected type.
+    Exception to be raised by :meth:`~aas.model.base.AASReference.resolve` if the retrieved object has not the
+    expected type.
 
     :ivar value: The object of unexpected type
     """
     def __init__(self, value: Referable, *args):
         super().__init__(*args)
         self.value = value
 
@@ -660,39 +646,38 @@
         if len(self.key) != len(other.key):
             return False
         return all(k1 == k2 for k1, k2 in zip(self.key, other.key))
 
 
 class AASReference(Reference, Generic[_RT]):
     """
-    Typed Reference to any referable Asset Administration Shell object.
+    Typed :class:`~.Reference` to any :class:`~.Referable` :class:`~aas.model.aas.AssetAdministrationShell` object.
 
     This is a special construct of the implementation to allow typed references and dereferencing.
+
+    :ivar key: Ordered list of unique references in its name space, each key referencing an element. The complete
+            list of keys may for example be concatenated to a path that then gives unique access to an element
+            or entity (inherited from :class:`~.Reference`).
+    :ivar: type: The type of the referenced object (additional parameter, not from the AAS Metamodel),
+        Initialisation parameter: `target_type`
     """
     def __init__(self,
                  key: Tuple[Key, ...],
                  target_type: Type[_RT]):
         """
-        Initializer of AASReference
-
-        :param key: Ordered list of unique reference in its name space, each key referencing an element. The complete
-                    list of keys may for example be concatenated to a path that then gives unique access to an element
-                    or entity.
-        :param: type_: The type of the referenced object (additional parameter, not from the AAS Metamodel)
-
         TODO: Add instruction what to do after construction
         """
         # TODO check keys for validity. GlobalReference and Fragment-Type keys are not allowed here
         super().__init__(key)
         self.type: Type[_RT]
         object.__setattr__(self, 'type', target_type)
 
     def resolve(self, provider_: "provider.AbstractObjectProvider") -> _RT:
         """
-        Follow the reference and retrieve the Referable object it points to
+        Follow the :class:`~.Reference` and retrieve the :class:`~.Referable` object it points to
 
         :return: The referenced object (or a proxy object for it)
         :raises IndexError: If the list of keys is empty
         :raises TypeError: If one of the intermediate objects on the path is not a Namespace
         :raises UnexpectedTypeError: If the retrieved object is not of the expected type (or one of its subclasses). The
                                      object is stored in the `value` attribute of the exception
         :raises KeyError: If the reference could not be resolved
@@ -733,18 +718,18 @@
         if not isinstance(item, self.type):
             raise UnexpectedTypeError(item, "Retrieved object {} is not an instance of referenced type {}"
                                             .format(item, self.type.__name__))
         return item
 
     def get_identifier(self) -> Identifier:
         """
-        Retrieve the Identifier of the Identifiable object, which is referenced or in which the referenced Referable is
-        contained.
+        Retrieve the :class:`~.Identifier` of the :class:`~.Identifiable` object, which is referenced or in which the
+        referenced :class:`~.Referable` is contained.
 
-        :raises ValueError: If this Reference does not include a Key with global KeyType (IRDI, IRI, CUSTOM)
+        :raises ValueError: If this :class:`~.Reference` does not include a Key with global KeyType (IRDI, IRI, CUSTOM)
         """
         try:
             last_identifier = next(key.get_identifier()
                                    for key in reversed(self.key)
                                    if key.get_identifier())
             return last_identifier  # type: ignore  # MyPy doesn't get the generator expression above
         except StopIteration:
@@ -753,18 +738,20 @@
 
     def __repr__(self) -> str:
         return "AASReference(type={}, key={})".format(self.type.__name__, self.key)
 
     @staticmethod
     def from_referable(referable: Referable) -> "AASReference":
         """
-        Construct a Reference to a given Referable AAS object
+        Construct an :class:`~.AASReference` to a given :class:`~.Referable` AAS object
 
-        This requires that the Referable object is Identifiable itself or is a child-, grand-child-, etc. object of an
-        Identifiable object. Additionally, the object must be an instance of a known Referable type.
+        This requires that the :class:`~.Referable` object is :class:`~.Identifiable` itself or is a
+        child-, grand-child-, etc. object of an
+        :class:`~.Identifiable` object. Additionally, the object must be an instance of a known :class:`~.Referable`
+        type.
 
         :raises ValueError: If no Identifiable object is found while traversing the object's ancestors
         """
         # Get the first class from the base classes list (via inspect.getmro), that is contained in KEY_ELEMENTS_CLASSES
         from . import KEY_ELEMENTS_CLASSES
         try:
             ref_type = next(iter(t for t in inspect.getmro(type(referable)) if t in KEY_ELEMENTS_CLASSES))
@@ -781,20 +768,20 @@
             if ref.parent is None or not isinstance(ref.parent, Referable):
                 raise ValueError("The given Referable object is not embedded within an Identifiable object")
             ref = ref.parent
 
 
 class Identifiable(Referable, metaclass=abc.ABCMeta):
     """
-    An element that has a globally unique identifier.
+    An element that has a globally unique :class:`~.Identifier`.
 
-    << abstract >>
+    <<abstract>>
 
-    :ivar administration: Administrative information of an identifiable element.
-    :ivar identification: The globally unique identification of the element.
+    :ivar administration: :class:`~.AdministrativeInformation` of an identifiable element.
+    :ivar ~.identification: The globally unique identification of the element.
     """
     @abc.abstractmethod
     def __init__(self):
         super().__init__()
         self.administration: Optional[AdministrativeInformation] = None
         self.identification: Identifier = Identifier("", IdentifierType.IRDI)
 
@@ -802,15 +789,15 @@
         return "{}[{}]".format(self.__class__.__name__, self.identification)
 
 
 class HasSemantics(metaclass=abc.ABCMeta):
     """
     Element that can have a semantic definition.
 
-    << abstract >>
+    <<abstract>>
 
     :ivar semantic_id: Identifier of the semantic definition of the element. It is called semantic id of the element.
                        The semantic id may either reference an external global id or it may reference a referable model
                        element of kind=Type that defines the semantics of the element.
     """
     @abc.abstractmethod
     def __init__(self):
@@ -819,15 +806,15 @@
 
 
 class HasKind(metaclass=abc.ABCMeta):
     """
     An element with a kind is an element that can either represent a type or an instance.
     Default for an element is that it is representing an instance.
 
-    << abstract >>
+    <<abstract>>
 
     :ivar kind: Kind of the element: either type or instance. Default = Instance.
     """
     @abc.abstractmethod
     def __init__(self):
         super().__init__()
         self._kind: ModelingKind = ModelingKind.INSTANCE
@@ -837,89 +824,77 @@
         return self._kind
 
 
 class Constraint(metaclass=abc.ABCMeta):
     """
     A constraint is used to further qualify an element.
 
-    << abstract >>
+    <<abstract>>
     """
     @abc.abstractmethod
     def __init__(self):
         pass
 
 
 class Qualifiable(metaclass=abc.ABCMeta):
     """
     The value of a qualifiable element may be further qualified by one or more qualifiers or complex formulas.
 
-    << abstract >>
+    <<abstract>>
 
-    :ivar qualifier: Unordered list of Constraints that gives additional qualification of a qualifiable element.
+    :ivar qualifier: Unordered list of :class:`Constraints <~.Constraint>` that gives additional qualification of a
+        qualifiable element.
     """
     @abc.abstractmethod
     def __init__(self):
         super().__init__()
         self.qualifier: Set[Constraint] = set()
 
 
 class Formula(Constraint):
     """
     A formula is used to describe constraints by a logical expression.
 
-    :ivar depends_on: Unordered list of references to referable or even external global elements that are used in the
+    :ivar depends_on: Unordered list of :class:`References <~.Reference>` to :class:`~.Referable` or even external
+                      global elements that are used in the
                       logical expression. The value of the referenced elements needs to be accessible so that
                       it can be evaluated in the formula to true or false in the corresponding logical expression
                       it is used in.
     """
 
     def __init__(self,
                  depends_on: Optional[Set[Reference]] = None):
         """
-        Initializer of Formula
-
-        :param depends_on: Unordered of references to referable or even external global elements that are used in the
-                           logical expression. The value of the referenced elements needs to be accessible so that
-                           it can be evaluated in the formula to true or false in the corresponding logical expression
-                           it is used in.
-
         TODO: Add instruction what to do after construction
         """
         super().__init__()
         self.depends_on: Set[Reference] = set() if depends_on is None else depends_on
 
 
 class Qualifier(Constraint, HasSemantics):
     """
     A qualifier is a type-value pair that makes additional statements w.r.t. the value of the element.
 
+    **Constraint AASd-006:** if both, the value and the valueId are present then the value needs to be
+    identical to the value of the referenced coded value in Qualifier/valueId.
+
     :ivar type: The type of the qualifier that is applied to the element.
     :ivar value_type: Data type of the qualifier value
     :ivar value: The value of the qualifier.
-                 Constraint AASd-006: if both, the value and the valueId are present then the value needs to be
-                                      identical to the value of the referenced coded value in Qualifier/valueId.
     :ivar value_id: Reference to the global unique id of a coded value.
     :ivar semantic_id: The semantic_id defined in the HasSemantics class.
     """
 
     def __init__(self,
                  type_: QualifierType,
                  value_type: DataTypeDef,
                  value: Optional[ValueDataType] = None,
                  value_id: Optional[Reference] = None,
                  semantic_id: Optional[Reference] = None):
         """
-        Initializer of Qualifier
-
-        :param type_: The type of the qualifier that is applied to the element.
-        :param value_type: Data type of the qualifier value
-        :param value: The value of the qualifier.
-        :param value_id: Reference to the global unique id of a coded value.
-        :param semantic_id: The semantic_id defined in the HasSemantics class.
-
         TODO: Add instruction what to do after construction
         """
         super().__init__()
         self.type: QualifierType = type_
         self.value_type: Type[datatypes.AnyXSDType] = value_type
         self._value: Optional[ValueDataType] = datatypes.trivial_cast(value, value_type) if value is not None else None
         self.value_id: Optional[Reference] = value_id
@@ -940,15 +915,15 @@
             self._value = datatypes.trivial_cast(value, self.value_type)
 
 
 class ValueReferencePair:
     """
     A value reference pair within a value list. Each value has a global unique id defining its semantic.
 
-    << Data Type >>
+    <<DataType>>
 
     :ivar value: The value of the referenced concept definition of the value in value_id
     :ivar value_id: Global unique id of the value.
     """
 
     def __init__(self,
                  value_type: DataTypeDef,
@@ -985,65 +960,69 @@
 
 
 ValueList = Set[ValueReferencePair]
 
 
 class Namespace(metaclass=abc.ABCMeta):
     """
-    Abstract baseclass for all objects which form a Namespace to hold Referable objects and resolve them by their
-    id_short.
+    Abstract baseclass for all objects which form a Namespace to hold :class:`~.Referable` objects and resolve them by
+    their id_short.
 
-    A Namespace can contain multiple NamespaceSets, which contain Referable objects of different types. However, the
-    id_short of each object must be unique across all NamespaceSets of one Namespace.
+    A Namespace can contain multiple :class:`NamespaceSets <~.NamespaceSet>`, which contain :class:`~.Referable` objects
+    of different types. However, the id_short of each object must be unique across all NamespaceSets of one Namespace.
 
     :ivar namespace_element_sets: A list of all NamespaceSets of this Namespace
     """
     @abc.abstractmethod
     def __init__(self) -> None:
         super().__init__()
         self.namespace_element_sets: List[NamespaceSet] = []
 
     def get_referable(self, id_short: str) -> Referable:
         """
-        Find a Referable in this Namespaces by its id_short
+        Find a :class:`~.Referable` in this Namespaces by its `id_short`
 
-        :raises KeyError: If no such Referable can be found
+        :raises KeyError: If no such :class:`~.Referable` can be found
         """
         for dict_ in self.namespace_element_sets:
             if id_short in dict_:
                 return dict_.get_referable(id_short)
         raise KeyError("Referable with id_short {} not found in this namespace".format(id_short))
 
     def remove_referable(self, id_short: str) -> None:
         """
-        Remove a Referable from this Namespace by its id_short
+        Remove a :class:`~.Referable` from this Namespace by its `id_short`
 
-        :raises KeyError: If no such Referable can be found
+        :raises KeyError: If no such :class:`~.Referable` can be found
         """
         for dict_ in self.namespace_element_sets:
             if id_short in dict_:
                 return dict_.remove(id_short)
         raise KeyError("Referable with id_short {} not found in this namespace".format(id_short))
 
     def __iter__(self) -> Iterator[_RT]:
         return itertools.chain.from_iterable(self.namespace_element_sets)
 
 
 class NamespaceSet(MutableSet[_RT], Generic[_RT]):
     """
-    Helper class for storing Referable objects of a given type in a Namespace and find them by their id_short.
+    Helper class for storing :class:`~.Referable` objects of a given type in a :class:`~.Namespace` and find them by
+    their `id_short`.
 
-    This class behaves much like a set of Referable objects of a defined type, but uses a dict internally to rapidly
-    find those objects by their id_short. Additionally, it manages the `parent` attribute of the stored Referables and
-    ensures the uniqueness of their id_short within the Namespace.
+    This class behaves much like a set of :class:`~.Referable` objects of a defined type, but uses a dict internally to
+    rapidly
+    find those objects by their `id_short`. Additionally, it manages the `parent` attribute of the stored
+    :class:`Referables <~.Referable>` and
+    ensures the uniqueness of their id_short within the :class:`~.Namespace`.
 
     Use `add()`, `remove()`, `pop()`, `discard()`, `clear()`, `len()`, `x in` checks and iteration  just like on a
-    normal set of Referables. To get a referable by its id_short, use `get_referable()` or `get()` (the latter one
+    normal set of :class:`Referables <~.Referable>`. To get a :class:`~.Referable` by its `id_short`, use
+    `get_referable()` or `get()` (the latter one
     allows a default argument and returns None instead of raising a KeyError). As a bonus, the `x in` check supports
-    checking for existence of id_short *or* a concrete Referable object.
+    checking for existence of id_short *or* a concrete :class:`~.Referable` object.
     """
     def __init__(self, parent: Namespace, items: Iterable[_RT] = ()) -> None:
         """
         Initialize a new NamespaceSet.
 
         This initializer automatically takes care of adding this set to the `namespace_element_sets` list of the
         Namespace.
@@ -1113,27 +1092,27 @@
     def clear(self) -> None:
         for value in self._backend.values():
             value.parent = None
         self._backend.clear()
 
     def get_referable(self, key) -> _RT:
         """
-        Find an object in this set by its id_short
+        Find an object in this set by its `id_short`
 
         :raises KeyError: If no such object can be found
         """
         return self._backend[key]
 
     def get(self, key, default: Optional[_RT] = None) -> Optional[_RT]:
         """
-        Find an object in this set by its id_short, with fallback parameter
+        Find an object in this set by its `id_short`, with fallback parameter
 
         :param default: An object to be returned, if no object with the given id_short is found
-        :return: The Referable object with the given id_short in the set. Otherwise the `default` object or None, if
-                 none is given.
+        :return: The :class:`~.Referable` object with the given id_short in the set. Otherwise the `default` object or
+            None, if none is given.
         """
         return self._backend.get(key, default)
 
     def update_nss_from(self, other: "NamespaceSet"):
         """
         Update a NamespaceSet from a given NamespaceSet.
 
@@ -1161,15 +1140,16 @@
             self.add(referable_to_add)  # type: ignore
         for referable_to_remove in referables_to_remove:
             self.remove(referable_to_remove)  # type: ignore
 
 
 class OrderedNamespaceSet(NamespaceSet[_RT], MutableSequence[_RT], Generic[_RT]):
     """
-    A specialized version of NamespaceSet, that keeps track of the order of the stored Referable objects.
+    A specialized version of :class:`~.NamespaceSet`, that keeps track of the order of the stored
+    :class:`~.Referable` objects.
 
     Additionally to the MutableSet interface of NamespaceSet, this class provides a set-like interface (actually it
     is derived from MutableSequence). However, we don't permit duplicate entries in the ordered list of objects.
     """
     def __init__(self, parent: Namespace, items: Iterable[_RT] = ()) -> None:
         """
         Initialize a new OrderedNamespaceSet.
```

### Comparing `pyi40aas-0.2.2/aas/util/identification.py` & `pyi40aas-0.2.3/aas/util/identification.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,33 +2,35 @@
 #
 # This program and the accompanying materials are made available under the terms of the Eclipse Public License v. 2.0
 # which is available at https://www.eclipse.org/legal/epl-2.0, or the Apache License, Version 2.0 which is available
 # at https://www.apache.org/licenses/LICENSE-2.0.
 #
 # SPDX-License-Identifier: EPL-2.0 OR Apache-2.0
 """
-This module generates identifiers.
+This module generates :class:`Identifiers <aas.model.base.Identifier>`.
 
-Generate [identifier]:  -> Try:
-Abstract                -> AbstractIdentifierGenerator
-UUID                    -> UUIDGenerator
-IRI                     -> NamespaceIRIGenerator
+To Generate [identifier]:  -> Try:
+
+- Abstract                -> :class:`~.AbstractIdentifierGenerator`
+- UUID                    -> :class:`~.UUIDGenerator`
+- IRI                     -> :class:`NamespaceIRIGenerator`
 """
 
 import abc
 import re
 import uuid
 from typing import Optional, Dict, Union, Set
 
 from .. import model
 
 
 class AbstractIdentifierGenerator(metaclass=abc.ABCMeta):
     """
-    Abstract base class for identifier generators that generate identifiers based on an internal schema and an
+    Abstract base class for identifier generators that generate :class:`Identifiers <aas.model.base.Identifier>` based
+    on an internal schema and an
     (optional) proposal.
 
     Different Implementations of IdentifierGenerators may generate differently formed ids, e.g. URNs, HTTP-scheme IRIs,
     IRDIs, etc. Some of them may use a given private namespace and create ids within this namespace, others may just
     use long random numbers to ensure uniqueness.
     """
     @abc.abstractmethod
@@ -57,17 +59,23 @@
         return model.Identifier("urn:uuid:{}".format(uuid_), model.IdentifierType.IRI)
 
 
 class NamespaceIRIGenerator(AbstractIdentifierGenerator):
     """
     An IdentifierGenerator, that generates IRIs in a given namespace, checking uniqueness against a Registry.
 
-    Identifiers are generated by concatenating a fixed namespace with the proposed suffix. To verify uniqueness, the
-    existence of the identification is checked by querying the given Registry. If a collision is detected, a number
-    is prepended
+    :class:`Identifiers <aas.model.base.Identifier>` are generated by concatenating a fixed namespace with the proposed
+    suffix. To verify uniqueness, the
+    existence of the identification is checked by querying the given Registry. If a collision
+    is detected, a number is prepended
+
+    :ivar namespace: The IRI Namespace to generate Identifications in. It must be a valid IRI (starting with a
+                     scheme) and end on either #, /, or = to form a reasonable namespace.
+    :ivar ~.provider: An :class:`~aas.model.provider.AbstractObjectProvider` to check existence of
+        :class:`Identifiers <aas.model.base.Identifier>`
     """
     def __init__(self, namespace: str, provider: model.AbstractObjectProvider):
         """
         Create a new NamespaceIRIGenerator
         :param namespace: The IRI Namespace to generate Identifications in. It must be a valid IRI (starting with a
                           scheme) and end on either #, /, or = to form a reasonable namespace.
         :param provider: An AbstractObjectProvider to check existence of Identifiers
```

### Comparing `pyi40aas-0.2.2/README.md` & `pyi40aas-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,36 @@
-
 # PyI40AAS – Python Industry 4.0 Asset Administration Shell
 
-The PyI40AAS project aims to provide an implementation of the Asset Administration Shell (AAS) for Industry 4.0 Systems, compliant
-with the meta model and interface specification provided in
+### ⚠️ This project is now known as basyx-python-sdk, available here: https://github.com/eclipse-basyx/basyx-python-sdk
+
+⚠️⚠️⚠️ **This project is deprecated** ⚠️⚠️⚠️
+
+The PyI40AAS project aims to provide an implementation of the Asset Administration Shell (AAS) for Industry 4.0 Systems,
+compliant with the meta model and interface specification provided in
 [the document “Details of the Asset Administration Shell” (v2.0.1)](https://www.plattform-i40.de/PI40/Redaktion/DE/Downloads/Publikation/Details-of-the-Asset-Administration-Shell-Part1.html).
 
 
 ## Features
 
 * Modelling of AASs as Python objects (according to DotAAS sec. 4)
-* (De-)serialization of AAS objects into/from JSON and XML (according to DotAAS sec. 5) 
-* Reading and writing of AASX package files (according to DotAAS sec. 7)
-* Storing of AAS objects in CouchDB
+    * **except for**: Security extension of the metamodel (according to DotAAS sec. 5), *HasDataSpecification*
+* Reading and writing of AASX package files (according to DotAAS sec. 6)
+* (De-)serialization of AAS objects into/from JSON and XML (according to DotAAS sec. 7) 
+* Storing of AAS objects in CouchDB, Backend infrastructure for easy expansion 
 * Compliance checking of AAS XML and JSON files
 
 
 ### Project Structure
 
-The PyI40AAS project provides the `aas` Python package with 5 submodules:
+The PyI40AAS project provides the `aas` Python package with 6 submodules:
 
 * `aas.model`: The AAS metamodel implemented in python
-* `aas.adapter`: Adapters for various file formats and storage backends
-* `aas.compliance_tools`: Compliance checker for AAS files
+* `aas.adapter`: Adapters for various file formats 
+* `aas.backend`: Backend infrastructure for storing and retrieving AAS objects
+* `aas.compliance_tool`: Compliance checker for AAS files
 * `aas.util`: Provides utilities
 * `aas.examples`: Example data and tutorials
 
 
 ## License
 
 The PyI40AAS project is dual-licensed under the terms of the Eclipse Public License - v 2.0 and the
@@ -37,18 +42,18 @@
 file.
 
 
 ## Dependencies
 
 PyI40AAS requires the following Python packages to be installed for production usage. These dependencies are listed in
 `setup.py` to be fetched automatically when installing with `pip`:
-* `python-dateutil` (BSD 3-clause License)
 * `lxml` (BSD 3-clause License, using `libxml2` under MIT License)
-* `urllib3` (MIT License)
+* `python-dateutil` (BSD 3-clause License)
 * `pyecma376-2` (Apache License v2.0)
+* `urllib3` (MIT License)
 
 Optional production usage dependencies:
 * For using the Compliance Tool to validate JSON files against the JSON Schema: `jsonschema` and its
 dependencies (MIT License, Apache License, PSF License)
 
 Development/testing/example dependencies (see `requirements.txt`):
 * `jsonschema` and its dependencies (MIT License, Apache License, PSF License)
@@ -57,15 +62,15 @@
 
 ## Getting Started
 
 ### Installation
 
 For production usage and building applications with PyI40AAS, we recommended installation from PyPI:
 
-```python
+```bash
 pip install pyi40aas
 ```
 
 
 ### Example
 
 The following code example shows how to create a `Submodel` with a `Property` serialize it into an XML file using PyI40AAS:
@@ -109,21 +114,24 @@
 ```
 
 
 ### Examples and Tutorials
 
 For further examples and tutorials, check out the `aas.examples`-package. Here is a quick overview:
 
-* `aas.examples.tutorial_create_simple_aas`: Creating an Asset Administration Shell with all required objects via Python
-  code
+* `aas.examples.tutorial_create_simple_aas`: Create an Asset Administration Shell, including an Asset object and a 
+  Submodel
 * `aas.examples.tutorial_storage`: Manage a larger number of Asset Administration Shells in an ObjectStore and resolve
   references
-* `aas.examples.tutorial_serialization_deserialization`: Export or import AAS objects to/from JSON and XML documents
-* `aas.examples.tutorial_aasx`: Export or import AAS objects with auxiliary files to/from AASX package files
-* `aas.examples.tutorial_backend_couchdb`: Store, manage and update AAS objects in a CouchDB database
+* `aas.examples.tutorial_serialization_deserialization`: Use the JSON and XML serialization/deserialization for
+  single objects or full standard-compliant files 
+* `aas.examples.tutorial_aasx`: Export Asset Administration Shells with related objects and auxiliary files to AASX 
+  package files
+* `aas.examples.tutorial_backend_couchdb`: Use the *Backends* interface (`update()/commit()` methods) to manage and
+  retrieve AAS objects in a CouchDB document database 
 
 
 ### Compliance Tool
 
 The PyI40AAS project contains a compliance tool for testing xml and json files is provided in the 
 `aas.compliance_tool`-package. Following functionalities are supported:
```

### Comparing `pyi40aas-0.2.2/pyi40aas.egg-info/SOURCES.txt` & `pyi40aas-0.2.3/pyi40aas.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+NOTICE
 README.md
 setup.py
 aas/__init__.py
 aas/py.typed
 aas/adapter/__init__.py
 aas/adapter/_generic.py
 aas/adapter/aasx.py
```

