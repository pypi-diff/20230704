# Comparing `tmp/botocore-a-la-carte-rolesanywhere-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-rolesanywhere-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-rolesanywhere-1.29.99.tar", last modified: Sat Mar 25 01:23:06 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-rolesanywhere-1.30.0.tar", last modified: Tue Jul  4 01:44:58 2023, max compression
```

## Comparing `botocore-a-la-carte-rolesanywhere-1.29.99.tar` & `botocore-a-la-carte-rolesanywhere-1.30.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:06.336947 botocore-a-la-carte-rolesanywhere-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:06.000000 botocore-a-la-carte-rolesanywhere-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-25 01:23:06.336947 botocore-a-la-carte-rolesanywhere-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:06.332947 botocore-a-la-carte-rolesanywhere-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:06.332947 botocore-a-la-carte-rolesanywhere-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:06.332947 botocore-a-la-carte-rolesanywhere-1.29.99/botocore/data/rolesanywhere/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:06.336947 botocore-a-la-carte-rolesanywhere-1.29.99/botocore/data/rolesanywhere/2018-05-10/
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-03-25 01:22:12.000000 botocore-a-la-carte-rolesanywhere-1.29.99/botocore/data/rolesanywhere/2018-05-10/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-25 01:22:12.000000 botocore-a-la-carte-rolesanywhere-1.29.99/botocore/data/rolesanywhere/2018-05-10/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    48569 2023-03-25 01:22:12.000000 botocore-a-la-carte-rolesanywhere-1.29.99/botocore/data/rolesanywhere/2018-05-10/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:06.336947 botocore-a-la-carte-rolesanywhere-1.29.99/botocore_a_la_carte_rolesanywhere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-25 01:23:06.000000 botocore-a-la-carte-rolesanywhere-1.29.99/botocore_a_la_carte_rolesanywhere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-25 01:23:06.000000 botocore-a-la-carte-rolesanywhere-1.29.99/botocore_a_la_carte_rolesanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:06.000000 botocore-a-la-carte-rolesanywhere-1.29.99/botocore_a_la_carte_rolesanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:06.000000 botocore-a-la-carte-rolesanywhere-1.29.99/botocore_a_la_carte_rolesanywhere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:06.336947 botocore-a-la-carte-rolesanywhere-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-25 01:23:06.000000 botocore-a-la-carte-rolesanywhere-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.730816 botocore-a-la-carte-rolesanywhere-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:58.000000 botocore-a-la-carte-rolesanywhere-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-04 01:44:58.730816 botocore-a-la-carte-rolesanywhere-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.730816 botocore-a-la-carte-rolesanywhere-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.730816 botocore-a-la-carte-rolesanywhere-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.730816 botocore-a-la-carte-rolesanywhere-1.30.0/botocore/data/rolesanywhere/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.730816 botocore-a-la-carte-rolesanywhere-1.30.0/botocore/data/rolesanywhere/2018-05-10/
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-04 01:44:02.000000 botocore-a-la-carte-rolesanywhere-1.30.0/botocore/data/rolesanywhere/2018-05-10/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-04 01:44:02.000000 botocore-a-la-carte-rolesanywhere-1.30.0/botocore/data/rolesanywhere/2018-05-10/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54731 2023-07-04 01:44:02.000000 botocore-a-la-carte-rolesanywhere-1.30.0/botocore/data/rolesanywhere/2018-05-10/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.730816 botocore-a-la-carte-rolesanywhere-1.30.0/botocore_a_la_carte_rolesanywhere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-04 01:44:58.000000 botocore-a-la-carte-rolesanywhere-1.30.0/botocore_a_la_carte_rolesanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-04 01:44:58.000000 botocore-a-la-carte-rolesanywhere-1.30.0/botocore_a_la_carte_rolesanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:58.000000 botocore-a-la-carte-rolesanywhere-1.30.0/botocore_a_la_carte_rolesanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:58.000000 botocore-a-la-carte-rolesanywhere-1.30.0/botocore_a_la_carte_rolesanywhere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:58.730816 botocore-a-la-carte-rolesanywhere-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-04 01:44:58.000000 botocore-a-la-carte-rolesanywhere-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-rolesanywhere-1.29.99/LICENSE.txt` & `botocore-a-la-carte-rolesanywhere-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rolesanywhere-1.29.99/PKG-INFO` & `botocore-a-la-carte-rolesanywhere-1.30.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-rolesanywhere
-Version: 1.29.99
+Version: 1.30.0
 Summary: rolesanywhere data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-rolesanywhere-1.29.99/botocore/data/rolesanywhere/2018-05-10/endpoint-rule-set-1.json` & `botocore-a-la-carte-rolesanywhere-1.30.0/botocore/data/rolesanywhere/2018-05-10/endpoint-rule-set-1.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8977382330246914%*

 * *Differences: {"'rules'": "{0: {'conditions': {0: {'fn': 'isSet', 'argv': {0: {'ref': 'Endpoint'}}, delete: "*

 * *            "['assign']}}, 'rules': {0: {'type': 'error', 'error': 'Invalid Configuration: FIPS "*

 * *            "and custom endpoint are not supported', delete: ['rules']}, 1: {'conditions': [], "*

 * *            "'rules': {0: {'conditions': {0: {'argv': {insert: [(0, OrderedDict([('ref', "*

 * *            "'UseDualStack')]))], delete: [1]}}}, 'type': 'error', 'error': 'Invalid "*

 * *            "Configuration: Dualstack and c […]*

```diff
@@ -29,287 +29,322 @@
     },
     "rules": [
         {
             "conditions": [
                 {
                     "argv": [
                         {
-                            "ref": "Region"
+                            "ref": "Endpoint"
                         }
                     ],
-                    "assign": "PartitionResult",
-                    "fn": "aws.partition"
+                    "fn": "isSet"
                 }
             ],
             "rules": [
                 {
                     "conditions": [
                         {
                             "argv": [
                                 {
-                                    "ref": "Endpoint"
-                                }
-                            ],
-                            "fn": "isSet"
-                        },
-                        {
-                            "argv": [
-                                {
-                                    "ref": "Endpoint"
-                                }
+                                    "ref": "UseFIPS"
+                                },
+                                true
                             ],
-                            "assign": "url",
-                            "fn": "parseURL"
+                            "fn": "booleanEquals"
                         }
                     ],
+                    "error": "Invalid Configuration: FIPS and custom endpoint are not supported",
+                    "type": "error"
+                },
+                {
+                    "conditions": [],
                     "rules": [
                         {
                             "conditions": [
                                 {
                                     "argv": [
                                         {
-                                            "ref": "UseFIPS"
+                                            "ref": "UseDualStack"
                                         },
                                         true
                                     ],
                                     "fn": "booleanEquals"
                                 }
                             ],
-                            "error": "Invalid Configuration: FIPS and custom endpoint are not supported",
+                            "error": "Invalid Configuration: Dualstack and custom endpoint are not supported",
                             "type": "error"
                         },
                         {
                             "conditions": [],
-                            "rules": [
-                                {
-                                    "conditions": [
-                                        {
-                                            "argv": [
-                                                {
-                                                    "ref": "UseDualStack"
-                                                },
-                                                true
-                                            ],
-                                            "fn": "booleanEquals"
-                                        }
-                                    ],
-                                    "error": "Invalid Configuration: Dualstack and custom endpoint are not supported",
-                                    "type": "error"
-                                },
-                                {
-                                    "conditions": [],
-                                    "endpoint": {
-                                        "headers": {},
-                                        "properties": {},
-                                        "url": {
-                                            "ref": "Endpoint"
-                                        }
-                                    },
-                                    "type": "endpoint"
+                            "endpoint": {
+                                "headers": {},
+                                "properties": {},
+                                "url": {
+                                    "ref": "Endpoint"
                                 }
-                            ],
-                            "type": "tree"
+                            },
+                            "type": "endpoint"
                         }
                     ],
                     "type": "tree"
-                },
+                }
+            ],
+            "type": "tree"
+        },
+        {
+            "conditions": [],
+            "rules": [
                 {
                     "conditions": [
                         {
                             "argv": [
                                 {
-                                    "ref": "UseFIPS"
-                                },
-                                true
-                            ],
-                            "fn": "booleanEquals"
-                        },
-                        {
-                            "argv": [
-                                {
-                                    "ref": "UseDualStack"
-                                },
-                                true
+                                    "ref": "Region"
+                                }
                             ],
-                            "fn": "booleanEquals"
+                            "fn": "isSet"
                         }
                     ],
                     "rules": [
                         {
                             "conditions": [
                                 {
                                     "argv": [
-                                        true,
+                                        {
+                                            "ref": "Region"
+                                        }
+                                    ],
+                                    "assign": "PartitionResult",
+                                    "fn": "aws.partition"
+                                }
+                            ],
+                            "rules": [
+                                {
+                                    "conditions": [
+                                        {
+                                            "argv": [
+                                                {
+                                                    "ref": "UseFIPS"
+                                                },
+                                                true
+                                            ],
+                                            "fn": "booleanEquals"
+                                        },
                                         {
                                             "argv": [
                                                 {
-                                                    "ref": "PartitionResult"
+                                                    "ref": "UseDualStack"
                                                 },
-                                                "supportsFIPS"
+                                                true
                                             ],
-                                            "fn": "getAttr"
+                                            "fn": "booleanEquals"
                                         }
                                     ],
-                                    "fn": "booleanEquals"
-                                },
-                                {
-                                    "argv": [
-                                        true,
+                                    "rules": [
                                         {
-                                            "argv": [
+                                            "conditions": [
                                                 {
-                                                    "ref": "PartitionResult"
+                                                    "argv": [
+                                                        true,
+                                                        {
+                                                            "argv": [
+                                                                {
+                                                                    "ref": "PartitionResult"
+                                                                },
+                                                                "supportsFIPS"
+                                                            ],
+                                                            "fn": "getAttr"
+                                                        }
+                                                    ],
+                                                    "fn": "booleanEquals"
                                                 },
-                                                "supportsDualStack"
+                                                {
+                                                    "argv": [
+                                                        true,
+                                                        {
+                                                            "argv": [
+                                                                {
+                                                                    "ref": "PartitionResult"
+                                                                },
+                                                                "supportsDualStack"
+                                                            ],
+                                                            "fn": "getAttr"
+                                                        }
+                                                    ],
+                                                    "fn": "booleanEquals"
+                                                }
                                             ],
-                                            "fn": "getAttr"
+                                            "rules": [
+                                                {
+                                                    "conditions": [],
+                                                    "rules": [
+                                                        {
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://rolesanywhere-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
+                                                            },
+                                                            "type": "endpoint"
+                                                        }
+                                                    ],
+                                                    "type": "tree"
+                                                }
+                                            ],
+                                            "type": "tree"
+                                        },
+                                        {
+                                            "conditions": [],
+                                            "error": "FIPS and DualStack are enabled, but this partition does not support one or both",
+                                            "type": "error"
                                         }
                                     ],
-                                    "fn": "booleanEquals"
-                                }
-                            ],
-                            "rules": [
-                                {
-                                    "conditions": [],
-                                    "endpoint": {
-                                        "headers": {},
-                                        "properties": {},
-                                        "url": "https://rolesanywhere-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
-                                    },
-                                    "type": "endpoint"
-                                }
-                            ],
-                            "type": "tree"
-                        },
-                        {
-                            "conditions": [],
-                            "error": "FIPS and DualStack are enabled, but this partition does not support one or both",
-                            "type": "error"
-                        }
-                    ],
-                    "type": "tree"
-                },
-                {
-                    "conditions": [
-                        {
-                            "argv": [
-                                {
-                                    "ref": "UseFIPS"
+                                    "type": "tree"
                                 },
-                                true
-                            ],
-                            "fn": "booleanEquals"
-                        }
-                    ],
-                    "rules": [
-                        {
-                            "conditions": [
                                 {
-                                    "argv": [
-                                        true,
+                                    "conditions": [
                                         {
                                             "argv": [
                                                 {
-                                                    "ref": "PartitionResult"
+                                                    "ref": "UseFIPS"
                                                 },
-                                                "supportsFIPS"
+                                                true
                                             ],
-                                            "fn": "getAttr"
+                                            "fn": "booleanEquals"
                                         }
                                     ],
-                                    "fn": "booleanEquals"
-                                }
-                            ],
-                            "rules": [
-                                {
-                                    "conditions": [],
                                     "rules": [
                                         {
+                                            "conditions": [
+                                                {
+                                                    "argv": [
+                                                        true,
+                                                        {
+                                                            "argv": [
+                                                                {
+                                                                    "ref": "PartitionResult"
+                                                                },
+                                                                "supportsFIPS"
+                                                            ],
+                                                            "fn": "getAttr"
+                                                        }
+                                                    ],
+                                                    "fn": "booleanEquals"
+                                                }
+                                            ],
+                                            "rules": [
+                                                {
+                                                    "conditions": [],
+                                                    "rules": [
+                                                        {
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://rolesanywhere-fips.{Region}.{PartitionResult#dnsSuffix}"
+                                                            },
+                                                            "type": "endpoint"
+                                                        }
+                                                    ],
+                                                    "type": "tree"
+                                                }
+                                            ],
+                                            "type": "tree"
+                                        },
+                                        {
                                             "conditions": [],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://rolesanywhere-fips.{Region}.{PartitionResult#dnsSuffix}"
-                                            },
-                                            "type": "endpoint"
+                                            "error": "FIPS is enabled but this partition does not support FIPS",
+                                            "type": "error"
                                         }
                                     ],
                                     "type": "tree"
-                                }
-                            ],
-                            "type": "tree"
-                        },
-                        {
-                            "conditions": [],
-                            "error": "FIPS is enabled but this partition does not support FIPS",
-                            "type": "error"
-                        }
-                    ],
-                    "type": "tree"
-                },
-                {
-                    "conditions": [
-                        {
-                            "argv": [
-                                {
-                                    "ref": "UseDualStack"
                                 },
-                                true
-                            ],
-                            "fn": "booleanEquals"
-                        }
-                    ],
-                    "rules": [
-                        {
-                            "conditions": [
                                 {
-                                    "argv": [
-                                        true,
+                                    "conditions": [
                                         {
                                             "argv": [
                                                 {
-                                                    "ref": "PartitionResult"
+                                                    "ref": "UseDualStack"
                                                 },
-                                                "supportsDualStack"
+                                                true
                                             ],
-                                            "fn": "getAttr"
+                                            "fn": "booleanEquals"
                                         }
                                     ],
-                                    "fn": "booleanEquals"
-                                }
-                            ],
-                            "rules": [
+                                    "rules": [
+                                        {
+                                            "conditions": [
+                                                {
+                                                    "argv": [
+                                                        true,
+                                                        {
+                                                            "argv": [
+                                                                {
+                                                                    "ref": "PartitionResult"
+                                                                },
+                                                                "supportsDualStack"
+                                                            ],
+                                                            "fn": "getAttr"
+                                                        }
+                                                    ],
+                                                    "fn": "booleanEquals"
+                                                }
+                                            ],
+                                            "rules": [
+                                                {
+                                                    "conditions": [],
+                                                    "rules": [
+                                                        {
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://rolesanywhere.{Region}.{PartitionResult#dualStackDnsSuffix}"
+                                                            },
+                                                            "type": "endpoint"
+                                                        }
+                                                    ],
+                                                    "type": "tree"
+                                                }
+                                            ],
+                                            "type": "tree"
+                                        },
+                                        {
+                                            "conditions": [],
+                                            "error": "DualStack is enabled but this partition does not support DualStack",
+                                            "type": "error"
+                                        }
+                                    ],
+                                    "type": "tree"
+                                },
                                 {
                                     "conditions": [],
-                                    "endpoint": {
-                                        "headers": {},
-                                        "properties": {},
-                                        "url": "https://rolesanywhere.{Region}.{PartitionResult#dualStackDnsSuffix}"
-                                    },
-                                    "type": "endpoint"
+                                    "rules": [
+                                        {
+                                            "conditions": [],
+                                            "endpoint": {
+                                                "headers": {},
+                                                "properties": {},
+                                                "url": "https://rolesanywhere.{Region}.{PartitionResult#dnsSuffix}"
+                                            },
+                                            "type": "endpoint"
+                                        }
+                                    ],
+                                    "type": "tree"
                                 }
                             ],
                             "type": "tree"
-                        },
-                        {
-                            "conditions": [],
-                            "error": "DualStack is enabled but this partition does not support DualStack",
-                            "type": "error"
                         }
                     ],
                     "type": "tree"
                 },
                 {
                     "conditions": [],
-                    "endpoint": {
-                        "headers": {},
-                        "properties": {},
-                        "url": "https://rolesanywhere.{Region}.{PartitionResult#dnsSuffix}"
-                    },
-                    "type": "endpoint"
+                    "error": "Invalid Configuration: Missing Region",
+                    "type": "error"
                 }
             ],
             "type": "tree"
         }
     ],
     "version": "1.0"
 }
```

### Comparing `botocore-a-la-carte-rolesanywhere-1.29.99/botocore/data/rolesanywhere/2018-05-10/paginators-1.json` & `botocore-a-la-carte-rolesanywhere-1.30.0/botocore/data/rolesanywhere/2018-05-10/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rolesanywhere-1.29.99/botocore/data/rolesanywhere/2018-05-10/service-2.json` & `botocore-a-la-carte-rolesanywhere-1.30.0/botocore/data/rolesanywhere/2018-05-10/service-2.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8727059613249171%*

 * *Differences: {"'documentation'": "'<p>Identity and Access Management Roles Anywhere provides a secure way for "*

 * *                    'your workloads such as servers, containers, and applications that run outside '*

 * *                    'of Amazon Web Services to obtain temporary Amazon Web Services credentials. '*

 * *                    'Your workloads can use the same IAM policies and roles you have for native '*

 * *                    'Amazon Web Services applications to access Amazon Web Services resources. '*

 * *                   […]*

```diff
@@ -1,23 +1,23 @@
 {
-    "documentation": "<p>AWS Identity and Access Management Roles Anywhere provides a secure way for your workloads such as servers, containers, and applications running outside of AWS to obtain Temporary AWS credentials. Your workloads can use the same IAM policies and roles that you have configured with native AWS applications to access AWS resources. Using IAM Roles Anywhere will eliminate the need to manage long term credentials for workloads running outside of AWS.</p> <p>To use IAM Roles Anywhere customer workloads will need to use X.509 certificates issued by their Certificate Authority (CA) . The Certificate Authority (CA) needs to be registered with IAM Roles Anywhere as a trust anchor to establish trust between customer PKI and IAM Roles Anywhere. Customers who do not manage their own PKI system can use AWS Certificate Manager Private Certificate Authority (ACM PCA) to create a Certificate Authority and use that to establish trust with IAM Roles Anywhere</p> <p>This guide describes the IAM rolesanywhere operations that you can call programmatically. For general information about IAM Roles Anywhere see <a href=\"https://docs.aws.amazon.com/\">https://docs.aws.amazon.com/</a> </p>",
+    "documentation": "<p>Identity and Access Management Roles Anywhere provides a secure way for your workloads such as servers, containers, and applications that run outside of Amazon Web Services to obtain temporary Amazon Web Services credentials. Your workloads can use the same IAM policies and roles you have for native Amazon Web Services applications to access Amazon Web Services resources. Using IAM Roles Anywhere eliminates the need to manage long-term credentials for workloads running outside of Amazon Web Services.</p> <p> To use IAM Roles Anywhere, your workloads must use X.509 certificates issued by their certificate authority (CA). You register the CA with IAM Roles Anywhere as a trust anchor to establish trust between your public key infrastructure (PKI) and IAM Roles Anywhere. If you don't manage your own PKI system, you can use Private Certificate Authority to create a CA and then use that to establish trust with IAM Roles Anywhere. </p> <p>This guide describes the IAM Roles Anywhere operations that you can call programmatically. For more information about IAM Roles Anywhere, see the <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/userguide/introduction.html\">IAM Roles Anywhere User Guide</a>.</p>",
     "metadata": {
         "apiVersion": "2018-05-10",
         "endpointPrefix": "rolesanywhere",
         "jsonVersion": "1.1",
         "protocol": "rest-json",
         "serviceFullName": "IAM Roles Anywhere",
         "serviceId": "RolesAnywhere",
         "signatureVersion": "v4",
         "signingName": "rolesanywhere",
         "uid": "rolesanywhere-2018-05-10"
     },
     "operations": {
         "CreateProfile": {
-            "documentation": "<p>Creates a profile. A profile is configuration resource to list the roles that RolesAnywhere service is trusted to assume. In addition, by applying a profile you can intersect permissions with IAM managed policies.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:CreateProfile</code>. </p>",
+            "documentation": "<p>Creates a <i>profile</i>, a list of the roles that Roles Anywhere service is trusted to assume. You use profiles to intersect permissions with IAM managed policies.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:CreateProfile</code>. </p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 }
@@ -32,15 +32,15 @@
             },
             "name": "CreateProfile",
             "output": {
                 "shape": "ProfileDetailResponse"
             }
         },
         "CreateTrustAnchor": {
-            "documentation": "<p>Creates a trust anchor. You establish trust between IAM Roles Anywhere and your certificate authority (CA) by configuring a trust anchor. A Trust Anchor is defined either as a reference to a AWS Certificate Manager Private Certificate Authority (ACM PCA), or by uploading a Certificate Authority (CA) certificate. Your AWS workloads can authenticate with the trust anchor using certificates issued by the trusted Certificate Authority (CA) in exchange for temporary AWS credentials.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:CreateTrustAnchor</code>. </p>",
+            "documentation": "<p>Creates a trust anchor to establish trust between IAM Roles Anywhere and your certificate authority (CA). You can define a trust anchor as a reference to an Private Certificate Authority (Private CA) or by uploading a CA certificate. Your Amazon Web Services workloads can authenticate with the trust anchor using certificates issued by the CA in exchange for temporary Amazon Web Services credentials.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:CreateTrustAnchor</code>. </p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 }
@@ -150,15 +150,15 @@
             },
             "name": "DisableCrl",
             "output": {
                 "shape": "CrlDetailResponse"
             }
         },
         "DisableProfile": {
-            "documentation": "<p>Disables a profile. When disabled, <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> requests with this profile fail.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:DisableProfile</code>. </p>",
+            "documentation": "<p>Disables a profile. When disabled, temporary credential requests with this profile fail.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:DisableProfile</code>. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 }
@@ -173,15 +173,15 @@
             },
             "name": "DisableProfile",
             "output": {
                 "shape": "ProfileDetailResponse"
             }
         },
         "DisableTrustAnchor": {
-            "documentation": "<p>Disables a trust anchor. When disabled, <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> requests specifying this trust anchor are unauthorized.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:DisableTrustAnchor</code>. </p>",
+            "documentation": "<p>Disables a trust anchor. When disabled, temporary credential requests specifying this trust anchor are unauthorized.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:DisableTrustAnchor</code>. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 }
@@ -219,15 +219,15 @@
             },
             "name": "EnableCrl",
             "output": {
                 "shape": "CrlDetailResponse"
             }
         },
         "EnableProfile": {
-            "documentation": "<p>Enables the roles in a profile to receive session credentials in <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a>. </p> <p> <b>Required permissions: </b> <code>rolesanywhere:EnableProfile</code>. </p>",
+            "documentation": "<p>Enables temporary credential requests for a profile. </p> <p> <b>Required permissions: </b> <code>rolesanywhere:EnableProfile</code>. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 }
@@ -308,15 +308,15 @@
             },
             "name": "GetProfile",
             "output": {
                 "shape": "ProfileDetailResponse"
             }
         },
         "GetSubject": {
-            "documentation": "<p>Gets a Subject. A Subject associates a certificate identity with authentication attempts by CreateSession. The Subject resources stores audit information such as status of the last authentication attempt, the certificate data used in the attempt, and the last time the associated identity attempted authentication. </p> <p> <b>Required permissions: </b> <code>rolesanywhere:GetSubject</code>. </p>",
+            "documentation": "<p>Gets a <i>subject</i>, which associates a certificate identity with authentication attempts. The subject stores auditing information such as the status of the last authentication attempt, the certificate data used in the attempt, and the last time the associated identity attempted authentication. </p> <p> <b>Required permissions: </b> <code>rolesanywhere:GetSubject</code>. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 }
@@ -357,15 +357,15 @@
             },
             "name": "GetTrustAnchor",
             "output": {
                 "shape": "TrustAnchorDetailResponse"
             }
         },
         "ImportCrl": {
-            "documentation": "<p>Imports the certificate revocation list (CRL). CRl is a list of certificates that have been revoked by the issuing certificate Authority (CA). IAM Roles Anywhere validates against the crl list before issuing credentials. </p> <p> <b>Required permissions: </b> <code>rolesanywhere:ImportCrl</code>. </p>",
+            "documentation": "<p>Imports the certificate revocation list (CRL). A CRL is a list of certificates that have been revoked by the issuing certificate Authority (CA). IAM Roles Anywhere validates against the CRL before issuing credentials. </p> <p> <b>Required permissions: </b> <code>rolesanywhere:ImportCrl</code>. </p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 }
@@ -380,15 +380,15 @@
             },
             "name": "ImportCrl",
             "output": {
                 "shape": "CrlDetailResponse"
             }
         },
         "ListCrls": {
-            "documentation": "<p>Lists all Crls in the authenticated account and Amazon Web Services Region.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:ListCrls</code>. </p>",
+            "documentation": "<p>Lists all certificate revocation lists (CRL) in the authenticated account and Amazon Web Services Region.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:ListCrls</code>. </p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 }
@@ -497,14 +497,66 @@
                 "shape": "ListRequest"
             },
             "name": "ListTrustAnchors",
             "output": {
                 "shape": "ListTrustAnchorsResponse"
             }
         },
+        "PutNotificationSettings": {
+            "documentation": "<p>Attaches a list of <i>notification settings</i> to a trust anchor.</p> <p>A notification setting includes information such as event name, threshold, status of the notification setting, and the channel to notify.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:PutNotificationSettings</code>. </p>",
+            "errors": [
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                }
+            ],
+            "http": {
+                "method": "PATCH",
+                "requestUri": "/put-notifications-settings",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "PutNotificationSettingsRequest"
+            },
+            "name": "PutNotificationSettings",
+            "output": {
+                "shape": "PutNotificationSettingsResponse"
+            }
+        },
+        "ResetNotificationSettings": {
+            "documentation": "<p>Resets the <i>custom notification setting</i> to IAM Roles Anywhere default setting. </p> <p> <b>Required permissions: </b> <code>rolesanywhere:ResetNotificationSettings</code>. </p>",
+            "errors": [
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "ResourceNotFoundException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                }
+            ],
+            "http": {
+                "method": "PATCH",
+                "requestUri": "/reset-notifications-settings",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "ResetNotificationSettingsRequest"
+            },
+            "name": "ResetNotificationSettings",
+            "output": {
+                "shape": "ResetNotificationSettingsResponse"
+            }
+        },
         "TagResource": {
             "documentation": "<p>Attaches tags to a resource.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:TagResource</code>. </p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
@@ -553,15 +605,15 @@
             },
             "name": "UntagResource",
             "output": {
                 "shape": "UntagResourceResponse"
             }
         },
         "UpdateCrl": {
-            "documentation": "<p>Updates the certificate revocation list (CRL). CRl is a list of certificates that have been revoked by the issuing certificate Authority (CA). IAM Roles Anywhere validates against the crl list before issuing credentials.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:UpdateCrl</code>. </p>",
+            "documentation": "<p>Updates the certificate revocation list (CRL). A CRL is a list of certificates that have been revoked by the issuing certificate authority (CA). IAM Roles Anywhere validates against the CRL before issuing credentials.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:UpdateCrl</code>. </p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -579,15 +631,15 @@
             },
             "name": "UpdateCrl",
             "output": {
                 "shape": "CrlDetailResponse"
             }
         },
         "UpdateProfile": {
-            "documentation": "<p>Updates the profile. A profile is configuration resource to list the roles that RolesAnywhere service is trusted to assume. In addition, by applying a profile you can scope-down permissions with IAM managed policies.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:UpdateProfile</code>. </p>",
+            "documentation": "<p>Updates a <i>profile</i>, a list of the roles that IAM Roles Anywhere service is trusted to assume. You use profiles to intersect permissions with IAM managed policies.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:UpdateProfile</code>. </p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -606,15 +658,15 @@
             },
             "name": "UpdateProfile",
             "output": {
                 "shape": "ProfileDetailResponse"
             }
         },
         "UpdateTrustAnchor": {
-            "documentation": "<p>Updates the trust anchor.You establish trust between IAM Roles Anywhere and your certificate authority (CA) by configuring a trust anchor. A Trust Anchor is defined either as a reference to a AWS Certificate Manager Private Certificate Authority (ACM PCA), or by uploading a Certificate Authority (CA) certificate. Your AWS workloads can authenticate with the trust anchor using certificates issued by the trusted Certificate Authority (CA) in exchange for temporary AWS credentials.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:UpdateTrustAnchor</code>. </p>",
+            "documentation": "<p>Updates a trust anchor. You establish trust between IAM Roles Anywhere and your certificate authority (CA) by configuring a trust anchor. You can define a trust anchor as a reference to an Private Certificate Authority (Private CA) or by uploading a CA certificate. Your Amazon Web Services workloads can authenticate with the trust anchor using certificates issued by the CA in exchange for temporary Amazon Web Services credentials.</p> <p> <b>Required permissions: </b> <code>rolesanywhere:UpdateTrustAnchor</code>. </p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -679,19 +731,19 @@
                     "shape": "ManagedPolicyList"
                 },
                 "name": {
                     "documentation": "<p>The name of the profile.</p>",
                     "shape": "ResourceName"
                 },
                 "requireInstanceProperties": {
-                    "documentation": "<p>Specifies whether instance properties are required in <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> requests with this profile. </p>",
+                    "documentation": "<p>Specifies whether instance properties are required in temporary credential requests with this profile. </p>",
                     "shape": "Boolean"
                 },
                 "roleArns": {
-                    "documentation": "<p>A list of IAM roles that this profile can assume in a <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> operation.</p>",
+                    "documentation": "<p>A list of IAM roles that this profile can assume in a temporary credential request.</p>",
                     "shape": "RoleArnList"
                 },
                 "sessionPolicy": {
                     "documentation": "<p>A session policy that applies to the trust boundary of the vended session credentials. </p>",
                     "shape": "String"
                 },
                 "tags": {
@@ -703,28 +755,32 @@
                 "name",
                 "roleArns"
             ],
             "type": "structure"
         },
         "CreateProfileRequestDurationSecondsInteger": {
             "box": true,
-            "max": 43200,
+            "max": 3600,
             "min": 900,
             "type": "integer"
         },
         "CreateTrustAnchorRequest": {
             "members": {
                 "enabled": {
                     "documentation": "<p>Specifies whether the trust anchor is enabled.</p>",
                     "shape": "Boolean"
                 },
                 "name": {
                     "documentation": "<p>The name of the trust anchor.</p>",
                     "shape": "ResourceName"
                 },
+                "notificationSettings": {
+                    "documentation": "<p>A list of notification settings to be associated to the trust anchor.</p>",
+                    "shape": "NotificationSettings"
+                },
                 "source": {
                     "documentation": "<p>The trust anchor type and its related certificate data.</p>",
                     "shape": "Source"
                 },
                 "tags": {
                     "documentation": "<p>The tags to attach to the trust anchor.</p>",
                     "shape": "TagList"
@@ -739,30 +795,30 @@
         "CredentialSummaries": {
             "member": {
                 "shape": "CredentialSummary"
             },
             "type": "list"
         },
         "CredentialSummary": {
-            "documentation": "<p>A record of a presented X509 credential to <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a>. </p>",
+            "documentation": "<p>A record of a presented X509 credential from a temporary credential request. </p>",
             "members": {
                 "enabled": {
                     "documentation": "<p>Indicates whether the credential is enabled.</p>",
                     "shape": "Boolean"
                 },
                 "failed": {
-                    "documentation": "<p>Indicates whether the <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> operation was successful. </p>",
+                    "documentation": "<p>Indicates whether the temporary credential request was successful. </p>",
                     "shape": "Boolean"
                 },
                 "issuer": {
                     "documentation": "<p>The fully qualified domain name of the issuing certificate for the presented end-entity certificate.</p>",
                     "shape": "String"
                 },
                 "seenAt": {
-                    "documentation": "<p>The ISO-8601 time stamp of when the certificate was last used in a <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> operation.</p>",
+                    "documentation": "<p>The ISO-8601 time stamp of when the certificate was last used in a temporary credential request.</p>",
                     "shape": "SyntheticTimestamp_date_time"
                 },
                 "serialNumber": {
                     "documentation": "<p>The serial number of the certificate.</p>",
                     "shape": "String"
                 },
                 "x509CertificateData": {
@@ -827,15 +883,15 @@
                 "shape": "CrlDetail"
             },
             "type": "list"
         },
         "ImportCrlRequest": {
             "members": {
                 "crlData": {
-                    "documentation": "<p>The x509 v3 specified certificate revocation list</p>",
+                    "documentation": "<p>The x509 v3 specified certificate revocation list (CRL).</p>",
                     "shape": "ImportCrlRequestCrlDataBlob"
                 },
                 "enabled": {
                     "documentation": "<p>Specifies whether the certificate revocation list (CRL) is enabled.</p>",
                     "shape": "Boolean"
                 },
                 "name": {
@@ -869,23 +925,23 @@
             },
             "type": "list"
         },
         "InstanceProperty": {
             "documentation": "<p>A key-value pair you set that identifies a property of the authenticating instance.</p>",
             "members": {
                 "failed": {
-                    "documentation": "<p>Indicates whether the <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> operation was successful. </p>",
+                    "documentation": "<p>Indicates whether the temporary credential request was successful. </p>",
                     "shape": "Boolean"
                 },
                 "properties": {
                     "documentation": "<p>A list of instanceProperty objects. </p>",
                     "shape": "InstancePropertyMap"
                 },
                 "seenAt": {
-                    "documentation": "<p>The ISO-8601 time stamp of when the certificate was last used in a <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> operation.</p>",
+                    "documentation": "<p>The ISO-8601 time stamp of when the certificate was last used in a temporary credential request.</p>",
                     "shape": "SyntheticTimestamp_date_time"
                 }
             },
             "type": "structure"
         },
         "InstancePropertyMap": {
             "key": {
@@ -915,37 +971,37 @@
         "ListCrlsResponse": {
             "members": {
                 "crls": {
                     "documentation": "<p>A list of certificate revocation lists (CRL). </p>",
                     "shape": "CrlDetails"
                 },
                 "nextToken": {
-                    "documentation": "<p>A token that indicates where the output should continue from, if a previous operation did not show all results. To get the next results, call the operation again with this value.</p>",
+                    "documentation": "<p>A token that indicates where the output should continue from, if a previous request did not show all results. To get the next results, make the request again with this value.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "ListProfilesResponse": {
             "members": {
                 "nextToken": {
-                    "documentation": "<p>A token that indicates where the output should continue from, if a previous operation did not show all results. To get the next results, call the operation again with this value.</p>",
+                    "documentation": "<p>A token that indicates where the output should continue from, if a previous request did not show all results. To get the next results, make the request again with this value.</p>",
                     "shape": "String"
                 },
                 "profiles": {
                     "documentation": "<p>A list of profiles.</p>",
                     "shape": "ProfileDetails"
                 }
             },
             "type": "structure"
         },
         "ListRequest": {
             "members": {
                 "nextToken": {
-                    "documentation": "<p>A token that indicates where the output should continue from, if a previous operation did not show all results. To get the next results, call the operation again with this value.</p>",
+                    "documentation": "<p>A token that indicates where the output should continue from, if a previous request did not show all results. To get the next results, make the request again with this value.</p>",
                     "location": "querystring",
                     "locationName": "nextToken",
                     "shape": "ListRequestNextTokenString"
                 },
                 "pageSize": {
                     "documentation": "<p>The number of resources in the paginated list. </p>",
                     "location": "querystring",
@@ -959,15 +1015,15 @@
             "max": 10000,
             "min": 1,
             "type": "string"
         },
         "ListSubjectsResponse": {
             "members": {
                 "nextToken": {
-                    "documentation": "<p>A token that indicates where the output should continue from, if a previous operation did not show all results. To get the next results, call the operation again with this value.</p>",
+                    "documentation": "<p>A token that indicates where the output should continue from, if a previous request did not show all results. To get the next results, make the request again with this value.</p>",
                     "shape": "String"
                 },
                 "subjects": {
                     "documentation": "<p>A list of subjects.</p>",
                     "shape": "SubjectSummaries"
                 }
             },
@@ -995,15 +1051,15 @@
                 }
             },
             "type": "structure"
         },
         "ListTrustAnchorsResponse": {
             "members": {
                 "nextToken": {
-                    "documentation": "<p>A token that indicates where the output should continue from, if a previous operation did not show all results. To get the next results, call the operation again with this value.</p>",
+                    "documentation": "<p>A token that indicates where the output should continue from, if a previous request did not show all results. To get the next results, make the request again with this value.</p>",
                     "shape": "String"
                 },
                 "trustAnchors": {
                     "documentation": "<p>A list of trust anchors.</p>",
                     "shape": "TrustAnchorDetails"
                 }
             },
@@ -1018,14 +1074,141 @@
             "type": "list"
         },
         "ManagedPolicyListMemberString": {
             "max": 200,
             "min": 1,
             "type": "string"
         },
+        "NotificationChannel": {
+            "enum": [
+                "ALL"
+            ],
+            "type": "string"
+        },
+        "NotificationEvent": {
+            "enum": [
+                "CA_CERTIFICATE_EXPIRY",
+                "END_ENTITY_CERTIFICATE_EXPIRY"
+            ],
+            "type": "string"
+        },
+        "NotificationSetting": {
+            "documentation": "<p> Customizable notification settings that will be applied to notification events. IAM Roles Anywhere consumes these settings while notifying across multiple channels - CloudWatch metrics, EventBridge, and Health Dashboard. </p>",
+            "members": {
+                "channel": {
+                    "documentation": "<p>The specified channel of notification. IAM Roles Anywhere uses CloudWatch metrics, EventBridge, and Health Dashboard to notify for an event.</p> <note> <p>In the absence of a specific channel, IAM Roles Anywhere applies this setting to 'ALL' channels.</p> </note>",
+                    "shape": "NotificationChannel"
+                },
+                "enabled": {
+                    "documentation": "<p>Indicates whether the notification setting is enabled.</p>",
+                    "shape": "Boolean"
+                },
+                "event": {
+                    "documentation": "<p>The event to which this notification setting is applied.</p>",
+                    "shape": "NotificationEvent"
+                },
+                "threshold": {
+                    "documentation": "<p>The number of days before a notification event. This value is required for a notification setting that is enabled.</p>",
+                    "shape": "NotificationSettingThresholdInteger"
+                }
+            },
+            "required": [
+                "enabled",
+                "event"
+            ],
+            "type": "structure"
+        },
+        "NotificationSettingDetail": {
+            "documentation": "<p>The state of a notification setting.</p> <p>A notification setting includes information such as event name, threshold, status of the notification setting, and the channel to notify.</p>",
+            "members": {
+                "channel": {
+                    "documentation": "<p>The specified channel of notification. IAM Roles Anywhere uses CloudWatch metrics, EventBridge, and Health Dashboard to notify for an event.</p> <note> <p>In the absence of a specific channel, IAM Roles Anywhere applies this setting to 'ALL' channels.</p> </note>",
+                    "shape": "NotificationChannel"
+                },
+                "configuredBy": {
+                    "documentation": "<p>The principal that configured the notification setting. For default settings configured by IAM Roles Anywhere, the value is <code>rolesanywhere.amazonaws.com</code>, and for customized notifications settings, it is the respective account ID. </p>",
+                    "shape": "NotificationSettingDetailConfiguredByString"
+                },
+                "enabled": {
+                    "documentation": "<p>Indicates whether the notification setting is enabled.</p>",
+                    "shape": "Boolean"
+                },
+                "event": {
+                    "documentation": "<p>The event to which this notification setting is applied.</p>",
+                    "shape": "NotificationEvent"
+                },
+                "threshold": {
+                    "documentation": "<p>The number of days before a notification event.</p>",
+                    "shape": "NotificationSettingDetailThresholdInteger"
+                }
+            },
+            "required": [
+                "enabled",
+                "event"
+            ],
+            "type": "structure"
+        },
+        "NotificationSettingDetailConfiguredByString": {
+            "max": 200,
+            "min": 1,
+            "type": "string"
+        },
+        "NotificationSettingDetailThresholdInteger": {
+            "box": true,
+            "max": 360,
+            "min": 1,
+            "type": "integer"
+        },
+        "NotificationSettingDetails": {
+            "max": 50,
+            "member": {
+                "shape": "NotificationSettingDetail"
+            },
+            "min": 0,
+            "type": "list"
+        },
+        "NotificationSettingKey": {
+            "documentation": "<p>A notification setting key to reset. A notification setting key includes the event and the channel. </p>",
+            "members": {
+                "channel": {
+                    "documentation": "<p>The specified channel of notification.</p>",
+                    "shape": "NotificationChannel"
+                },
+                "event": {
+                    "documentation": "<p>The notification setting event to reset.</p>",
+                    "shape": "NotificationEvent"
+                }
+            },
+            "required": [
+                "event"
+            ],
+            "type": "structure"
+        },
+        "NotificationSettingKeys": {
+            "max": 50,
+            "member": {
+                "shape": "NotificationSettingKey"
+            },
+            "min": 0,
+            "type": "list"
+        },
+        "NotificationSettingThresholdInteger": {
+            "box": true,
+            "max": 360,
+            "min": 1,
+            "type": "integer"
+        },
+        "NotificationSettings": {
+            "max": 50,
+            "member": {
+                "shape": "NotificationSetting"
+            },
+            "min": 0,
+            "type": "list"
+        },
         "ProfileArn": {
             "max": 1011,
             "min": 1,
             "pattern": "^arn:aws(-[^:]+)?:rolesanywhere(:.*){2}(:profile.*)$",
             "type": "string"
         },
         "ProfileDetail": {
@@ -1060,19 +1243,19 @@
                     "shape": "ProfileArn"
                 },
                 "profileId": {
                     "documentation": "<p>The unique identifier of the profile.</p>",
                     "shape": "Uuid"
                 },
                 "requireInstanceProperties": {
-                    "documentation": "<p>Specifies whether instance properties are required in <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> requests with this profile. </p>",
+                    "documentation": "<p>Specifies whether instance properties are required in temporary credential requests with this profile. </p>",
                     "shape": "Boolean"
                 },
                 "roleArns": {
-                    "documentation": "<p>A list of IAM roles that this profile can assume in a <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> operation.</p>",
+                    "documentation": "<p>A list of IAM roles that this profile can assume in a temporary credential request.</p>",
                     "shape": "RoleArnList"
                 },
                 "sessionPolicy": {
                     "documentation": "<p>A session policy that applies to the trust boundary of the vended session credentials. </p>",
                     "shape": "String"
                 },
                 "updatedAt": {
@@ -1093,14 +1276,70 @@
         },
         "ProfileDetails": {
             "member": {
                 "shape": "ProfileDetail"
             },
             "type": "list"
         },
+        "PutNotificationSettingsRequest": {
+            "members": {
+                "notificationSettings": {
+                    "documentation": "<p>A list of notification settings to be associated to the trust anchor.</p>",
+                    "shape": "NotificationSettings"
+                },
+                "trustAnchorId": {
+                    "documentation": "<p>The unique identifier of the trust anchor.</p>",
+                    "shape": "Uuid"
+                }
+            },
+            "required": [
+                "notificationSettings",
+                "trustAnchorId"
+            ],
+            "type": "structure"
+        },
+        "PutNotificationSettingsResponse": {
+            "members": {
+                "trustAnchor": {
+                    "shape": "TrustAnchorDetail"
+                }
+            },
+            "required": [
+                "trustAnchor"
+            ],
+            "type": "structure"
+        },
+        "ResetNotificationSettingsRequest": {
+            "members": {
+                "notificationSettingKeys": {
+                    "documentation": "<p>A list of notification setting keys to reset. A notification setting key includes the event and the channel. </p>",
+                    "shape": "NotificationSettingKeys"
+                },
+                "trustAnchorId": {
+                    "documentation": "<p>The unique identifier of the trust anchor.</p>",
+                    "shape": "Uuid"
+                }
+            },
+            "required": [
+                "notificationSettingKeys",
+                "trustAnchorId"
+            ],
+            "type": "structure"
+        },
+        "ResetNotificationSettingsResponse": {
+            "members": {
+                "trustAnchor": {
+                    "shape": "TrustAnchorDetail"
+                }
+            },
+            "required": [
+                "trustAnchor"
+            ],
+            "type": "structure"
+        },
         "ResourceName": {
             "max": 255,
             "min": 1,
             "pattern": "^[ a-zA-Z0-9-_]*$",
             "type": "string"
         },
         "ResourceNotFoundException": {
@@ -1201,49 +1440,54 @@
             },
             "type": "structure"
         },
         "SourceData": {
             "documentation": "<p>The data field of the trust anchor depending on its type. </p>",
             "members": {
                 "acmPcaArn": {
-                    "documentation": "<p>The root certificate of the Certificate Manager Private Certificate Authority specified by this ARN is used in trust validation for <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> operations. Included for trust anchors of type <code>AWS_ACM_PCA</code>. </p>",
+                    "documentation": "<p> The root certificate of the Private Certificate Authority specified by this ARN is used in trust validation for temporary credential requests. Included for trust anchors of type <code>AWS_ACM_PCA</code>. </p>",
                     "shape": "String"
                 },
                 "x509CertificateData": {
                     "documentation": "<p>The PEM-encoded data for the certificate anchor. Included for trust anchors of type <code>CERTIFICATE_BUNDLE</code>. </p>",
-                    "shape": "String"
+                    "shape": "SourceDataX509CertificateDataString"
                 }
             },
             "type": "structure",
             "union": true
         },
+        "SourceDataX509CertificateDataString": {
+            "max": 8000,
+            "min": 1,
+            "type": "string"
+        },
         "String": {
             "type": "string"
         },
         "SubjectDetail": {
             "documentation": "<p>The state of the subject after a read or write operation.</p>",
             "members": {
                 "createdAt": {
                     "documentation": "<p>The ISO-8601 timestamp when the subject was created. </p>",
                     "shape": "SyntheticTimestamp_date_time"
                 },
                 "credentials": {
-                    "documentation": "<p>The temporary session credentials vended at the last authenticating call with this Subject.</p>",
+                    "documentation": "<p>The temporary session credentials vended at the last authenticating call with this subject.</p>",
                     "shape": "CredentialSummaries"
                 },
                 "enabled": {
                     "documentation": "<p>The enabled status of the subject.</p>",
                     "shape": "Boolean"
                 },
                 "instanceProperties": {
                     "documentation": "<p>The specified instance properties associated with the request.</p>",
                     "shape": "InstanceProperties"
                 },
                 "lastSeenAt": {
-                    "documentation": "<p>The ISO-8601 timestamp of the last time this Subject requested temporary session credentials.</p>",
+                    "documentation": "<p>The ISO-8601 timestamp of the last time this subject requested temporary session credentials.</p>",
                     "shape": "SyntheticTimestamp_date_time"
                 },
                 "subjectArn": {
                     "documentation": "<p>The ARN of the resource.</p>",
                     "shape": "String"
                 },
                 "subjectId": {
@@ -1273,26 +1517,26 @@
         "SubjectSummaries": {
             "member": {
                 "shape": "SubjectSummary"
             },
             "type": "list"
         },
         "SubjectSummary": {
-            "documentation": "<p>A summary representation of Subject resources returned in read operations; primarily ListSubjects.</p>",
+            "documentation": "<p>A summary representation of subjects.</p>",
             "members": {
                 "createdAt": {
-                    "documentation": "<p>The ISO-8601 time stamp of when the certificate was first used in a <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> operation.</p>",
+                    "documentation": "<p>The ISO-8601 time stamp of when the certificate was first used in a temporary credential request.</p>",
                     "shape": "SyntheticTimestamp_date_time"
                 },
                 "enabled": {
-                    "documentation": "<p>The enabled status of the Subject. </p>",
+                    "documentation": "<p>The enabled status of the subject. </p>",
                     "shape": "Boolean"
                 },
                 "lastSeenAt": {
-                    "documentation": "<p>The ISO-8601 time stamp of when the certificate was last used in a <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> operation.</p>",
+                    "documentation": "<p>The ISO-8601 time stamp of when the certificate was last used in a temporary credential request.</p>",
                     "shape": "SyntheticTimestamp_date_time"
                 },
                 "subjectArn": {
                     "documentation": "<p>The ARN of the resource.</p>",
                     "shape": "String"
                 },
                 "subjectId": {
@@ -1336,23 +1580,23 @@
             "max": 128,
             "min": 1,
             "pattern": "^[ a-zA-Z0-9_.:/=+@-]*$",
             "sensitive": true,
             "type": "string"
         },
         "TagKeyList": {
-            "max": 50,
+            "max": 200,
             "member": {
                 "shape": "TagKey"
             },
             "min": 0,
             "type": "list"
         },
         "TagList": {
-            "max": 50,
+            "max": 200,
             "member": {
                 "shape": "Tag"
             },
             "min": 0,
             "type": "list"
         },
         "TagResourceRequest": {
@@ -1414,14 +1658,18 @@
                     "documentation": "<p>Indicates whether the trust anchor is enabled.</p>",
                     "shape": "Boolean"
                 },
                 "name": {
                     "documentation": "<p>The name of the trust anchor.</p>",
                     "shape": "ResourceName"
                 },
+                "notificationSettings": {
+                    "documentation": "<p>A list of notification settings to be associated to the trust anchor.</p>",
+                    "shape": "NotificationSettingDetails"
+                },
                 "source": {
                     "documentation": "<p>The trust anchor type and its related certificate data.</p>",
                     "shape": "Source"
                 },
                 "trustAnchorArn": {
                     "documentation": "<p>The ARN of the trust anchor.</p>",
                     "shape": "String"
@@ -1483,15 +1731,15 @@
         "UntagResourceResponse": {
             "members": {},
             "type": "structure"
         },
         "UpdateCrlRequest": {
             "members": {
                 "crlData": {
-                    "documentation": "<p>The x509 v3 specified certificate revocation list</p>",
+                    "documentation": "<p>The x509 v3 specified certificate revocation list (CRL).</p>",
                     "shape": "UpdateCrlRequestCrlDataBlob"
                 },
                 "crlId": {
                     "documentation": "<p>The unique identifier of the certificate revocation list (CRL).</p>",
                     "location": "uri",
                     "locationName": "crlId",
                     "shape": "Uuid"
@@ -1528,30 +1776,30 @@
                 "profileId": {
                     "documentation": "<p>The unique identifier of the profile.</p>",
                     "location": "uri",
                     "locationName": "profileId",
                     "shape": "Uuid"
                 },
                 "roleArns": {
-                    "documentation": "<p>A list of IAM roles that this profile can assume in a <a href=\"https://docs.aws.amazon.com/rolesanywhere/latest/APIReference/API_CreateSession.html\">CreateSession</a> operation.</p>",
+                    "documentation": "<p>A list of IAM roles that this profile can assume in a temporary credential request.</p>",
                     "shape": "RoleArnList"
                 },
                 "sessionPolicy": {
                     "documentation": "<p>A session policy that applies to the trust boundary of the vended session credentials. </p>",
                     "shape": "UpdateProfileRequestSessionPolicyString"
                 }
             },
             "required": [
                 "profileId"
             ],
             "type": "structure"
         },
         "UpdateProfileRequestDurationSecondsInteger": {
             "box": true,
-            "max": 43200,
+            "max": 3600,
             "min": 900,
             "type": "integer"
         },
         "UpdateProfileRequestSessionPolicyString": {
             "max": 100000,
             "min": 1,
             "type": "string"
```

### Comparing `botocore-a-la-carte-rolesanywhere-1.29.99/botocore_a_la_carte_rolesanywhere.egg-info/PKG-INFO` & `botocore-a-la-carte-rolesanywhere-1.30.0/botocore_a_la_carte_rolesanywhere.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-rolesanywhere
-Version: 1.29.99
+Version: 1.30.0
 Summary: rolesanywhere data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-rolesanywhere-1.29.99/setup.py` & `botocore-a-la-carte-rolesanywhere-1.30.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-rolesanywhere',
-    version="1.29.99",
+    version="1.30.0",
     description='rolesanywhere data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/rolesanywhere/*/*.json'],
```

