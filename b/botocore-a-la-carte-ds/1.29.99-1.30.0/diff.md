# Comparing `tmp/botocore-a-la-carte-ds-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-ds-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ds-1.29.99.tar", last modified: Sat Mar 25 01:22:36 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-ds-1.30.0.tar", last modified: Tue Jul  4 01:44:26 2023, max compression
```

## Comparing `botocore-a-la-carte-ds-1.29.99.tar` & `botocore-a-la-carte-ds-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.271147 botocore-a-la-carte-ds-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:36.000000 botocore-a-la-carte-ds-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-25 01:22:36.271147 botocore-a-la-carte-ds-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.267147 botocore-a-la-carte-ds-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.267147 botocore-a-la-carte-ds-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.267147 botocore-a-la-carte-ds-1.29.99/botocore/data/ds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.271147 botocore-a-la-carte-ds-1.29.99/botocore/data/ds/2015-04-16/
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-03-25 01:22:12.000000 botocore-a-la-carte-ds-1.29.99/botocore/data/ds/2015-04-16/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-ds-1.29.99/botocore/data/ds/2015-04-16/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-03-25 01:22:12.000000 botocore-a-la-carte-ds-1.29.99/botocore/data/ds/2015-04-16/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   199685 2023-03-25 01:22:12.000000 botocore-a-la-carte-ds-1.29.99/botocore/data/ds/2015-04-16/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.271147 botocore-a-la-carte-ds-1.29.99/botocore_a_la_carte_ds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-25 01:22:36.000000 botocore-a-la-carte-ds-1.29.99/botocore_a_la_carte_ds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-25 01:22:36.000000 botocore-a-la-carte-ds-1.29.99/botocore_a_la_carte_ds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:36.000000 botocore-a-la-carte-ds-1.29.99/botocore_a_la_carte_ds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:36.000000 botocore-a-la-carte-ds-1.29.99/botocore_a_la_carte_ds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:36.271147 botocore-a-la-carte-ds-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-25 01:22:36.000000 botocore-a-la-carte-ds-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:26.934516 botocore-a-la-carte-ds-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:26.000000 botocore-a-la-carte-ds-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-04 01:44:26.934516 botocore-a-la-carte-ds-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:26.930516 botocore-a-la-carte-ds-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:26.934516 botocore-a-la-carte-ds-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:26.934516 botocore-a-la-carte-ds-1.30.0/botocore/data/ds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:26.934516 botocore-a-la-carte-ds-1.30.0/botocore/data/ds/2015-04-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-04 01:44:02.000000 botocore-a-la-carte-ds-1.30.0/botocore/data/ds/2015-04-16/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-ds-1.30.0/botocore/data/ds/2015-04-16/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-04 01:44:02.000000 botocore-a-la-carte-ds-1.30.0/botocore/data/ds/2015-04-16/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   200275 2023-07-04 01:44:02.000000 botocore-a-la-carte-ds-1.30.0/botocore/data/ds/2015-04-16/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:26.934516 botocore-a-la-carte-ds-1.30.0/botocore_a_la_carte_ds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-04 01:44:26.000000 botocore-a-la-carte-ds-1.30.0/botocore_a_la_carte_ds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-04 01:44:26.000000 botocore-a-la-carte-ds-1.30.0/botocore_a_la_carte_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:26.000000 botocore-a-la-carte-ds-1.30.0/botocore_a_la_carte_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:26.000000 botocore-a-la-carte-ds-1.30.0/botocore_a_la_carte_ds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:26.934516 botocore-a-la-carte-ds-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-04 01:44:26.000000 botocore-a-la-carte-ds-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-ds-1.29.99/LICENSE.txt` & `botocore-a-la-carte-ds-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ds-1.29.99/PKG-INFO` & `botocore-a-la-carte-ds-1.30.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ds
-Version: 1.29.99
+Version: 1.30.0
 Summary: ds data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ds-1.29.99/botocore/data/ds/2015-04-16/endpoint-rule-set-1.json` & `botocore-a-la-carte-ds-1.30.0/botocore/data/ds/2015-04-16/endpoint-rule-set-1.json`

 * *Files 21% similar despite different names*

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
+                                                                "url": "https://ds-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                        "url": "https://ds-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
+                                                                "url": "https://ds-fips.{Region}.{PartitionResult#dnsSuffix}"
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
-                                                "url": "https://ds-fips.{Region}.{PartitionResult#dnsSuffix}"
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
+                                                                "url": "https://ds.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                        "url": "https://ds.{Region}.{PartitionResult#dualStackDnsSuffix}"
-                                    },
-                                    "type": "endpoint"
+                                    "rules": [
+                                        {
+                                            "conditions": [],
+                                            "endpoint": {
+                                                "headers": {},
+                                                "properties": {},
+                                                "url": "https://ds.{Region}.{PartitionResult#dnsSuffix}"
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
-                        "url": "https://ds.{Region}.{PartitionResult#dnsSuffix}"
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

### Comparing `botocore-a-la-carte-ds-1.29.99/botocore/data/ds/2015-04-16/paginators-1.json` & `botocore-a-la-carte-ds-1.30.0/botocore/data/ds/2015-04-16/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ds-1.29.99/botocore/data/ds/2015-04-16/service-2.json` & `botocore-a-la-carte-ds-1.30.0/botocore/data/ds/2015-04-16/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996624969036413%*

 * *Differences: {"'shapes'": "{'DirectoryConfigurationSettingValue': {'pattern': '^[a-zA-Z0-9_]*$'}, "*

 * *             "'RemoteDomainName': {'max': 1024}, 'SettingEntry': {'members': {'Type': "*

 * *             "{'documentation': '<p>The type, or category, of a directory setting. Similar "*

 * *             'settings have the same type. For example, <code>Protocol</code>, '*

 * *             "<code>Cipher</code>, or <code>Certificate-Based Authentication</code>.</p>'}, "*

 * *             "'AllowedValues': {'documentation': '<p>The valid range  […]*

```diff
@@ -3698,14 +3698,17 @@
                 }
             },
             "type": "structure"
         },
         "DirectoryConfigurationSettingAllowedValues": {
             "type": "string"
         },
+        "DirectoryConfigurationSettingDataType": {
+            "type": "string"
+        },
         "DirectoryConfigurationSettingLastRequestedDateTime": {
             "type": "timestamp"
         },
         "DirectoryConfigurationSettingLastUpdatedDateTime": {
             "type": "timestamp"
         },
         "DirectoryConfigurationSettingName": {
@@ -3728,15 +3731,15 @@
         },
         "DirectoryConfigurationSettingType": {
             "type": "string"
         },
         "DirectoryConfigurationSettingValue": {
             "max": 255,
             "min": 1,
-            "pattern": "^[a-zA-Z0-9]*$",
+            "pattern": "^[a-zA-Z0-9_]*$",
             "type": "string"
         },
         "DirectoryConfigurationStatus": {
             "enum": [
                 "Requested",
                 "Updating",
                 "Updated",
@@ -5311,14 +5314,15 @@
                     "documentation": "<p>Identifier of the shared directory in the directory consumer account.</p>",
                     "shape": "DirectoryId"
                 }
             },
             "type": "structure"
         },
         "RemoteDomainName": {
+            "max": 1024,
             "pattern": "^([a-zA-Z0-9]+[\\\\.-])+([a-zA-Z0-9])+[.]?$",
             "type": "string"
         },
         "RemoteDomainNames": {
             "member": {
                 "shape": "RemoteDomainName"
             },
@@ -5568,21 +5572,25 @@
             },
             "type": "list"
         },
         "SettingEntry": {
             "documentation": "<p>Contains information about the specified configurable setting for a directory.</p>",
             "members": {
                 "AllowedValues": {
-                    "documentation": "<p>The valid range of values for the directory setting.</p>",
+                    "documentation": "<p>The valid range of values for the directory setting. These values depend on the <code>DataType</code> of your directory.</p>",
                     "shape": "DirectoryConfigurationSettingAllowedValues"
                 },
                 "AppliedValue": {
                     "documentation": "<p>The value of the directory setting that is applied to the directory.</p>",
                     "shape": "DirectoryConfigurationSettingValue"
                 },
+                "DataType": {
+                    "documentation": "<p>The data type of a directory setting. This is used to define the <code>AllowedValues</code> of a setting. For example a data type can be <code>Boolean</code>, <code>DurationInSeconds</code>, or <code>Enum</code>.</p>",
+                    "shape": "DirectoryConfigurationSettingDataType"
+                },
                 "LastRequestedDateTime": {
                     "documentation": "<p>The date and time when the request to update a directory setting was last submitted.</p>",
                     "shape": "DirectoryConfigurationSettingLastRequestedDateTime"
                 },
                 "LastUpdatedDateTime": {
                     "documentation": "<p>The date and time when the directory setting was last updated.</p>",
                     "shape": "DirectoryConfigurationSettingLastUpdatedDateTime"
@@ -5604,15 +5612,15 @@
                     "shape": "DirectoryConfigurationSettingRequestStatusMessage"
                 },
                 "RequestedValue": {
                     "documentation": "<p>The value that was last requested for the directory setting.</p>",
                     "shape": "DirectoryConfigurationSettingValue"
                 },
                 "Type": {
-                    "documentation": "<p>The type of directory setting. For example, <code>Protocol</code> or <code>Cipher</code>.</p>",
+                    "documentation": "<p>The type, or category, of a directory setting. Similar settings have the same type. For example, <code>Protocol</code>, <code>Cipher</code>, or <code>Certificate-Based Authentication</code>.</p>",
                     "shape": "DirectoryConfigurationSettingType"
                 }
             },
             "type": "structure"
         },
         "Settings": {
             "member": {
```

### Comparing `botocore-a-la-carte-ds-1.29.99/botocore_a_la_carte_ds.egg-info/PKG-INFO` & `botocore-a-la-carte-ds-1.30.0/botocore_a_la_carte_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ds
-Version: 1.29.99
+Version: 1.30.0
 Summary: ds data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ds-1.29.99/setup.py` & `botocore-a-la-carte-ds-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ds',
-    version="1.29.99",
+    version="1.30.0",
     description='ds data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ds/*/*.json'],
```

