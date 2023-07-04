# Comparing `tmp/botocore-a-la-carte-healthlake-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-healthlake-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-healthlake-1.29.99.tar", last modified: Sat Mar 25 01:22:36 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-healthlake-1.30.0.tar", last modified: Tue Jul  4 01:44:27 2023, max compression
```

## Comparing `botocore-a-la-carte-healthlake-1.29.99.tar` & `botocore-a-la-carte-healthlake-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.747179 botocore-a-la-carte-healthlake-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:36.000000 botocore-a-la-carte-healthlake-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-25 01:22:36.747179 botocore-a-la-carte-healthlake-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.747179 botocore-a-la-carte-healthlake-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.747179 botocore-a-la-carte-healthlake-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.747179 botocore-a-la-carte-healthlake-1.29.99/botocore/data/healthlake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.747179 botocore-a-la-carte-healthlake-1.29.99/botocore/data/healthlake/2017-07-01/
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-03-25 01:22:12.000000 botocore-a-la-carte-healthlake-1.29.99/botocore/data/healthlake/2017-07-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-healthlake-1.29.99/botocore/data/healthlake/2017-07-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-25 01:22:12.000000 botocore-a-la-carte-healthlake-1.29.99/botocore/data/healthlake/2017-07-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    39816 2023-03-25 01:22:12.000000 botocore-a-la-carte-healthlake-1.29.99/botocore/data/healthlake/2017-07-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:36.747179 botocore-a-la-carte-healthlake-1.29.99/botocore_a_la_carte_healthlake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-25 01:22:36.000000 botocore-a-la-carte-healthlake-1.29.99/botocore_a_la_carte_healthlake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-25 01:22:36.000000 botocore-a-la-carte-healthlake-1.29.99/botocore_a_la_carte_healthlake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:36.000000 botocore-a-la-carte-healthlake-1.29.99/botocore_a_la_carte_healthlake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:36.000000 botocore-a-la-carte-healthlake-1.29.99/botocore_a_la_carte_healthlake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:36.751180 botocore-a-la-carte-healthlake-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-25 01:22:36.000000 botocore-a-la-carte-healthlake-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.242519 botocore-a-la-carte-healthlake-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:26.000000 botocore-a-la-carte-healthlake-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-04 01:44:27.242519 botocore-a-la-carte-healthlake-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.242519 botocore-a-la-carte-healthlake-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.242519 botocore-a-la-carte-healthlake-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.242519 botocore-a-la-carte-healthlake-1.30.0/botocore/data/healthlake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.242519 botocore-a-la-carte-healthlake-1.30.0/botocore/data/healthlake/2017-07-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-07-04 01:44:02.000000 botocore-a-la-carte-healthlake-1.30.0/botocore/data/healthlake/2017-07-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-healthlake-1.30.0/botocore/data/healthlake/2017-07-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 01:44:02.000000 botocore-a-la-carte-healthlake-1.30.0/botocore/data/healthlake/2017-07-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42875 2023-07-04 01:44:02.000000 botocore-a-la-carte-healthlake-1.30.0/botocore/data/healthlake/2017-07-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:27.242519 botocore-a-la-carte-healthlake-1.30.0/botocore_a_la_carte_healthlake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-04 01:44:27.000000 botocore-a-la-carte-healthlake-1.30.0/botocore_a_la_carte_healthlake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-04 01:44:27.000000 botocore-a-la-carte-healthlake-1.30.0/botocore_a_la_carte_healthlake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:27.000000 botocore-a-la-carte-healthlake-1.30.0/botocore_a_la_carte_healthlake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:27.000000 botocore-a-la-carte-healthlake-1.30.0/botocore_a_la_carte_healthlake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:27.242519 botocore-a-la-carte-healthlake-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-04 01:44:26.000000 botocore-a-la-carte-healthlake-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-healthlake-1.29.99/LICENSE.txt` & `botocore-a-la-carte-healthlake-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-healthlake-1.29.99/PKG-INFO` & `botocore-a-la-carte-healthlake-1.30.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-healthlake
-Version: 1.29.99
+Version: 1.30.0
 Summary: healthlake data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-healthlake-1.29.99/botocore/data/healthlake/2017-07-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-healthlake-1.30.0/botocore/data/healthlake/2017-07-01/endpoint-rule-set-1.json`

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
+                                                                "url": "https://healthlake-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                        "url": "https://healthlake-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
+                                                                "url": "https://healthlake-fips.{Region}.{PartitionResult#dnsSuffix}"
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
-                                                "url": "https://healthlake-fips.{Region}.{PartitionResult#dnsSuffix}"
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
+                                                                "url": "https://healthlake.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                        "url": "https://healthlake.{Region}.{PartitionResult#dualStackDnsSuffix}"
-                                    },
-                                    "type": "endpoint"
+                                    "rules": [
+                                        {
+                                            "conditions": [],
+                                            "endpoint": {
+                                                "headers": {},
+                                                "properties": {},
+                                                "url": "https://healthlake.{Region}.{PartitionResult#dnsSuffix}"
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
-                        "url": "https://healthlake.{Region}.{PartitionResult#dnsSuffix}"
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

### Comparing `botocore-a-la-carte-healthlake-1.29.99/botocore/data/healthlake/2017-07-01/service-2.json` & `botocore-a-la-carte-healthlake-1.30.0/botocore/data/healthlake/2017-07-01/service-2.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9924559922442324%*

 * *Differences: {"'operations'": "{'TagResource': {'documentation': '<p> Adds a user specified key and value tag "*

 * *                 "to a Data Store. </p>'}}",*

 * * "'shapes'": "{'CreateFHIRDatastoreRequest': {'members': {'IdentityProviderConfiguration': "*

 * *             "OrderedDict([('shape', 'IdentityProviderConfiguration'), ('documentation', '<p>The "*

 * *             'configuration of the identity provider that you want to use for your Data '*

 * *             "Store.</p>')])}}, 'CreateFHIRDatastoreResponse': {'members': {'Datastore […]*

```diff
@@ -328,15 +328,15 @@
             },
             "name": "StartFHIRImportJob",
             "output": {
                 "shape": "StartFHIRImportJobResponse"
             }
         },
         "TagResource": {
-            "documentation": "<p> Adds a user specifed key and value tag to a Data Store. </p>",
+            "documentation": "<p> Adds a user specified key and value tag to a Data Store. </p>",
             "errors": [
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 }
@@ -389,14 +389,24 @@
         },
         "AmazonResourceName": {
             "max": 1011,
             "min": 1,
             "pattern": "^arn:aws((-us-gov)|(-iso)|(-iso-b)|(-cn))?:healthlake:[a-z0-9-]+:\\d{12}:datastore\\/fhir\\/.{32}",
             "type": "string"
         },
+        "AuthorizationStrategy": {
+            "enum": [
+                "SMART_ON_FHIR_V1",
+                "AWS_AUTH"
+            ],
+            "type": "string"
+        },
+        "Boolean": {
+            "type": "boolean"
+        },
         "BoundedLengthString": {
             "max": 5000,
             "min": 1,
             "pattern": "[\\P{M}\\p{M}]{1,5000}",
             "type": "string"
         },
         "ClientTokenString": {
@@ -408,14 +418,17 @@
         "CmkType": {
             "enum": [
                 "CUSTOMER_MANAGED_KMS_KEY",
                 "AWS_OWNED_KMS_KEY"
             ],
             "type": "string"
         },
+        "ConfigurationMetadata": {
+            "type": "string"
+        },
         "ConflictException": {
             "documentation": "<p>The Data Store is in a transition state and the user requested action can not be performed.</p>",
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "String"
                 }
@@ -433,14 +446,18 @@
                     "documentation": "<p>The user generated name for the Data Store.</p>",
                     "shape": "DatastoreName"
                 },
                 "DatastoreTypeVersion": {
                     "documentation": "<p>The FHIR version of the Data Store. The only supported version is R4.</p>",
                     "shape": "FHIRVersion"
                 },
+                "IdentityProviderConfiguration": {
+                    "documentation": "<p>The configuration of the identity provider that you want to use for your Data Store.</p>",
+                    "shape": "IdentityProviderConfiguration"
+                },
                 "PreloadDataConfig": {
                     "documentation": "<p>Optional parameter to preload data upon creation of the Data Store. Currently, the only supported preloaded data is synthetic data generated from Synthea.</p>",
                     "shape": "PreloadDataConfig"
                 },
                 "SseConfiguration": {
                     "documentation": "<p> The server-side encryption key configuration for a customer provided encryption key specified for creating a Data Store. </p>",
                     "shape": "SseConfiguration"
@@ -454,19 +471,19 @@
                 "DatastoreTypeVersion"
             ],
             "type": "structure"
         },
         "CreateFHIRDatastoreResponse": {
             "members": {
                 "DatastoreArn": {
-                    "documentation": "<p>The datastore ARN is generated during the creation of the Data Store and can be found in the output from the initial Data Store creation call.</p>",
+                    "documentation": "<p>The Data Store ARN is generated during the creation of the Data Store and can be found in the output from the initial Data Store creation call.</p>",
                     "shape": "DatastoreArn"
                 },
                 "DatastoreEndpoint": {
-                    "documentation": "<p>The AWS endpoint for the created Data Store. For preview, only US-east-1 endpoints are supported.</p>",
+                    "documentation": "<p>The AWS endpoint for the created Data Store. </p>",
                     "shape": "BoundedLengthString"
                 },
                 "DatastoreId": {
                     "documentation": "<p>The AWS-generated Data Store id. This id is in the output from the initial Data Store creation call.</p>",
                     "shape": "DatastoreId"
                 },
                 "DatastoreStatus": {
@@ -517,15 +534,15 @@
         "DatastoreName": {
             "max": 256,
             "min": 1,
             "pattern": "^([\\p{L}\\p{Z}\\p{N}_.:/=+\\-%@]*)$",
             "type": "string"
         },
         "DatastoreProperties": {
-            "documentation": "<p>Displays the properties of the Data Store, including the ID, Arn, name, and the status of the Data Store.</p>",
+            "documentation": "<p>Displays the properties of the Data Store, including the ID, ARN, name, and the status of the Data Store.</p>",
             "members": {
                 "CreatedAt": {
                     "documentation": "<p>The time that a Data Store was created. </p>",
                     "shape": "Timestamp"
                 },
                 "DatastoreArn": {
                     "documentation": "<p>The Amazon Resource Name used in the creation of the Data Store.</p>",
@@ -547,14 +564,18 @@
                     "documentation": "<p>The status of the Data Store. Possible statuses are 'CREATING', 'ACTIVE', 'DELETING', or 'DELETED'.</p>",
                     "shape": "DatastoreStatus"
                 },
                 "DatastoreTypeVersion": {
                     "documentation": "<p>The FHIR version. Only R4 version data is supported.</p>",
                     "shape": "FHIRVersion"
                 },
+                "IdentityProviderConfiguration": {
+                    "documentation": "<p>The identity provider that you selected when you created the Data Store.</p>",
+                    "shape": "IdentityProviderConfiguration"
+                },
                 "PreloadDataConfig": {
                     "documentation": "<p>The preloaded data configuration for the Data Store. Only data preloaded from Synthea is supported.</p>",
                     "shape": "PreloadDataConfig"
                 },
                 "SseConfiguration": {
                     "documentation": "<p> The server-side encryption key configuration for a customer provided encryption key (CMK). </p>",
                     "shape": "SseConfiguration"
@@ -587,14 +608,17 @@
         "DeleteFHIRDatastoreRequest": {
             "members": {
                 "DatastoreId": {
                     "documentation": "<p> The AWS-generated ID for the Data Store to be deleted.</p>",
                     "shape": "DatastoreId"
                 }
             },
+            "required": [
+                "DatastoreId"
+            ],
             "type": "structure"
         },
         "DeleteFHIRDatastoreResponse": {
             "members": {
                 "DatastoreArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) that gives Amazon HealthLake access permission.</p>",
                     "shape": "DatastoreArn"
@@ -619,18 +643,21 @@
                 "DatastoreEndpoint"
             ],
             "type": "structure"
         },
         "DescribeFHIRDatastoreRequest": {
             "members": {
                 "DatastoreId": {
-                    "documentation": "<p>The AWS-generated Data Store id. This is part of the \u2018CreateFHIRDatastore\u2019 output.</p>",
+                    "documentation": "<p>The AWS-generated Data Store ID.</p>",
                     "shape": "DatastoreId"
                 }
             },
+            "required": [
+                "DatastoreId"
+            ],
             "type": "structure"
         },
         "DescribeFHIRDatastoreResponse": {
             "members": {
                 "DatastoreProperties": {
                     "documentation": "<p>All properties associated with a Data Store, including the Data Store ID, Data Store ARN, Data Store name, Data Store status, created at, Data Store type version, and Data Store endpoint.</p>",
                     "shape": "DatastoreProperties"
@@ -768,14 +795,39 @@
         },
         "IamRoleArn": {
             "max": 2048,
             "min": 20,
             "pattern": "arn:aws(-[^:]+)?:iam::[0-9]{12}:role/.+",
             "type": "string"
         },
+        "IdentityProviderConfiguration": {
+            "documentation": "<p>The identity provider configuration that you gave when the Data Store was created.</p>",
+            "members": {
+                "AuthorizationStrategy": {
+                    "documentation": "<p>The authorization strategy that you selected when you created the Data Store.</p>",
+                    "shape": "AuthorizationStrategy"
+                },
+                "FineGrainedAuthorizationEnabled": {
+                    "documentation": "<p>If you enabled fine-grained authorization when you created the Data Store.</p>",
+                    "shape": "Boolean"
+                },
+                "IdpLambdaArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Lambda function that you want to use to decode the access token created by the authorization server.</p>",
+                    "shape": "LambdaArn"
+                },
+                "Metadata": {
+                    "documentation": "<p>The JSON metadata elements that you want to use in your identity provider configuration. Required elements are listed based on the launch specification of the SMART application. For more information on all possible elements, see <a href=\"https://build.fhir.org/ig/HL7/smart-app-launch/conformance.html#metadata\">Metadata</a> in SMART's App Launch specification.</p> <p> <code>authorization_endpoint</code>: The URL to the OAuth2 authorization endpoint.</p> <p> <code>grant_types_supported</code>: An array of grant types that are supported at the token endpoint. You must provide at least one grant type option. Valid options are <code>authorization_code</code> and <code>client_credentials</code>.</p> <p> <code>token_endpoint</code>: The URL to the OAuth2 token endpoint.</p> <p> <code>capabilities</code>: An array of strings of the SMART capabilities that the authorization server supports.</p> <p> <code>code_challenge_methods_supported</code>: An array of strings of supported PKCE code challenge methods. You must include the <code>S256</code> method in the array of PKCE code challenge methods.</p>",
+                    "shape": "ConfigurationMetadata"
+                }
+            },
+            "required": [
+                "AuthorizationStrategy"
+            ],
+            "type": "structure"
+        },
         "ImportJobProperties": {
             "documentation": "<p>Displays the properties of the import job, including the ID, Arn, Name, and the status of the Data Store.</p>",
             "members": {
                 "DataAccessRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) that gives Amazon HealthLake access to your input data.</p>",
                     "shape": "IamRoleArn"
                 },
@@ -799,15 +851,15 @@
                     "documentation": "<p>The user-generated name for an Import job.</p>",
                     "shape": "JobName"
                 },
                 "JobOutputDataConfig": {
                     "shape": "OutputDataConfig"
                 },
                 "JobStatus": {
-                    "documentation": "<p>The job status for an Import job. Possible statuses are SUBMITTED, IN_PROGRESS, COMPLETED, FAILED.</p>",
+                    "documentation": "<p>The job status for an Import job. Possible statuses are SUBMITTED, IN_PROGRESS, COMPLETED_WITH_ERRORS, COMPLETED, FAILED.</p>",
                     "shape": "JobStatus"
                 },
                 "Message": {
                     "documentation": "<p>An explanation of any errors that may have occurred during the FHIR import job. </p>",
                     "shape": "Message"
                 },
                 "SubmitTime": {
@@ -866,15 +918,19 @@
         },
         "JobStatus": {
             "enum": [
                 "SUBMITTED",
                 "IN_PROGRESS",
                 "COMPLETED_WITH_ERRORS",
                 "COMPLETED",
-                "FAILED"
+                "FAILED",
+                "CANCEL_SUBMITTED",
+                "CANCEL_IN_PROGRESS",
+                "CANCEL_COMPLETED",
+                "CANCEL_FAILED"
             ],
             "type": "string"
         },
         "KmsEncryptionConfig": {
             "documentation": "<p> The customer-managed-key(CMK) used when creating a Data Store. If a customer owned key is not specified, an AWS owned key will be used for encryption. </p>",
             "members": {
                 "CmkType": {
@@ -887,14 +943,20 @@
                 }
             },
             "required": [
                 "CmkType"
             ],
             "type": "structure"
         },
+        "LambdaArn": {
+            "max": 256,
+            "min": 49,
+            "pattern": "arn:aws:lambda:[a-z]{2}-[a-z]+-\\d{1}:\\d{12}:function:[a-zA-Z0-9\\-_\\.]+(:(\\$LATEST|[a-zA-Z0-9\\-_]+))?",
+            "type": "string"
+        },
         "ListFHIRDatastoresRequest": {
             "members": {
                 "Filter": {
                     "documentation": "<p>Lists all filters associated with a FHIR Data Store request.</p>",
                     "shape": "DatastoreFilter"
                 },
                 "MaxResults": {
@@ -1260,15 +1322,15 @@
             "documentation": "<p> A tag is a label consisting of a user-defined key and value. The form for tags is {\"Key\", \"Value\"} </p>",
             "members": {
                 "Key": {
                     "documentation": "<p> The key portion of a tag. Tag keys are case sensitive. </p>",
                     "shape": "TagKey"
                 },
                 "Value": {
-                    "documentation": "<p> The value portion of tag. Tag values are case sensitive. </p>",
+                    "documentation": "<p> The value portion of a tag. Tag values are case sensitive. </p>",
                     "shape": "TagValue"
                 }
             },
             "required": [
                 "Key",
                 "Value"
             ],
```

### Comparing `botocore-a-la-carte-healthlake-1.29.99/botocore_a_la_carte_healthlake.egg-info/PKG-INFO` & `botocore-a-la-carte-healthlake-1.30.0/botocore_a_la_carte_healthlake.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-healthlake
-Version: 1.29.99
+Version: 1.30.0
 Summary: healthlake data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-healthlake-1.29.99/setup.py` & `botocore-a-la-carte-healthlake-1.30.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-healthlake',
-    version="1.29.99",
+    version="1.30.0",
     description='healthlake data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/healthlake/*/*.json'],
```

