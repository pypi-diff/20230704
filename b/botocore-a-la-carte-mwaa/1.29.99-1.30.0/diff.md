# Comparing `tmp/botocore-a-la-carte-mwaa-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-mwaa-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-mwaa-1.29.99.tar", last modified: Sat Mar 25 01:22:52 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-mwaa-1.30.0.tar", last modified: Tue Jul  4 01:44:42 2023, max compression
```

## Comparing `botocore-a-la-carte-mwaa-1.29.99.tar` & `botocore-a-la-carte-mwaa-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:52.008106 botocore-a-la-carte-mwaa-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:51.000000 botocore-a-la-carte-mwaa-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-25 01:22:52.008106 botocore-a-la-carte-mwaa-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:52.008106 botocore-a-la-carte-mwaa-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:52.008106 botocore-a-la-carte-mwaa-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:52.008106 botocore-a-la-carte-mwaa-1.29.99/botocore/data/mwaa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:52.008106 botocore-a-la-carte-mwaa-1.29.99/botocore/data/mwaa/2020-07-01/
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-03-25 01:22:12.000000 botocore-a-la-carte-mwaa-1.29.99/botocore/data/mwaa/2020-07-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-mwaa-1.29.99/botocore/data/mwaa/2020-07-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-25 01:22:12.000000 botocore-a-la-carte-mwaa-1.29.99/botocore/data/mwaa/2020-07-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    59363 2023-03-25 01:22:12.000000 botocore-a-la-carte-mwaa-1.29.99/botocore/data/mwaa/2020-07-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:52.008106 botocore-a-la-carte-mwaa-1.29.99/botocore_a_la_carte_mwaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-25 01:22:51.000000 botocore-a-la-carte-mwaa-1.29.99/botocore_a_la_carte_mwaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-25 01:22:51.000000 botocore-a-la-carte-mwaa-1.29.99/botocore_a_la_carte_mwaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:51.000000 botocore-a-la-carte-mwaa-1.29.99/botocore_a_la_carte_mwaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:51.000000 botocore-a-la-carte-mwaa-1.29.99/botocore_a_la_carte_mwaa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:52.008106 botocore-a-la-carte-mwaa-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-25 01:22:51.000000 botocore-a-la-carte-mwaa-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:42.542668 botocore-a-la-carte-mwaa-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:42.000000 botocore-a-la-carte-mwaa-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-04 01:44:42.542668 botocore-a-la-carte-mwaa-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:42.542668 botocore-a-la-carte-mwaa-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:42.542668 botocore-a-la-carte-mwaa-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:42.542668 botocore-a-la-carte-mwaa-1.30.0/botocore/data/mwaa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:42.542668 botocore-a-la-carte-mwaa-1.30.0/botocore/data/mwaa/2020-07-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-04 01:44:02.000000 botocore-a-la-carte-mwaa-1.30.0/botocore/data/mwaa/2020-07-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-mwaa-1.30.0/botocore/data/mwaa/2020-07-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-04 01:44:02.000000 botocore-a-la-carte-mwaa-1.30.0/botocore/data/mwaa/2020-07-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    65954 2023-07-04 01:44:02.000000 botocore-a-la-carte-mwaa-1.30.0/botocore/data/mwaa/2020-07-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:42.542668 botocore-a-la-carte-mwaa-1.30.0/botocore_a_la_carte_mwaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-04 01:44:42.000000 botocore-a-la-carte-mwaa-1.30.0/botocore_a_la_carte_mwaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-04 01:44:42.000000 botocore-a-la-carte-mwaa-1.30.0/botocore_a_la_carte_mwaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:42.000000 botocore-a-la-carte-mwaa-1.30.0/botocore_a_la_carte_mwaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:42.000000 botocore-a-la-carte-mwaa-1.30.0/botocore_a_la_carte_mwaa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:42.542668 botocore-a-la-carte-mwaa-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-04 01:44:42.000000 botocore-a-la-carte-mwaa-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-mwaa-1.29.99/LICENSE.txt` & `botocore-a-la-carte-mwaa-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-mwaa-1.29.99/PKG-INFO` & `botocore-a-la-carte-mwaa-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-mwaa
-Version: 1.29.99
+Version: 1.30.0
 Summary: mwaa data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-mwaa-1.29.99/botocore/data/mwaa/2020-07-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-mwaa-1.30.0/botocore/data/mwaa/2020-07-01/endpoint-rule-set-1.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8951340663580246%*

 * *Differences: {"'parameters'": "{'Region': {'required': False}}",*

 * * "'rules'": "{0: {'conditions': {0: {'fn': 'isSet', 'argv': {0: {'ref': 'Endpoint'}}, delete: "*

 * *            "['assign']}}, 'rules': {0: {'type': 'error', 'error': 'Invalid Configuration: FIPS "*

 * *            "and custom endpoint are not supported', delete: ['rules']}, 1: {'conditions': [], "*

 * *            "'rules': {0: {'conditions': {0: {'argv': {insert: [(0, OrderedDict([('ref', "*

 * *            "'UseDualStack')]))], delete: [1]}}}, 'type': 'error', 'error': 'I […]*

```diff
@@ -5,15 +5,15 @@
             "documentation": "Override the endpoint used to send this request",
             "required": false,
             "type": "String"
         },
         "Region": {
             "builtIn": "AWS::Region",
             "documentation": "The AWS region used to dispatch the request.",
-            "required": true,
+            "required": false,
             "type": "String"
         },
         "UseDualStack": {
             "builtIn": "AWS::UseDualStack",
             "default": false,
             "documentation": "When true, use the dual-stack endpoint. If the configured endpoint does not support dual-stack, dispatching the request MAY return an error.",
             "required": true,
@@ -29,278 +29,322 @@
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
+                                    "ref": "UseFIPS"
+                                },
+                                true
                             ],
-                            "fn": "isSet"
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
+                                        },
+                                        {
+                                            "argv": [
+                                                {
+                                                    "ref": "UseDualStack"
+                                                },
+                                                true
+                                            ],
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
+                                                                "url": "https://airflow-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
+                                                            },
+                                                            "type": "endpoint"
+                                                        }
+                                                    ],
+                                                    "type": "tree"
+                                                }
                                             ],
-                                            "fn": "getAttr"
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
-                                        "url": "https://airflow-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
+                                                                "url": "https://airflow-fips.{Region}.{PartitionResult#dnsSuffix}"
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
-                                                "url": "https://airflow-fips.{Region}.{PartitionResult#dnsSuffix}"
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
+                                                                "url": "https://airflow.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                        "url": "https://airflow.{Region}.{PartitionResult#dualStackDnsSuffix}"
-                                    },
-                                    "type": "endpoint"
+                                    "rules": [
+                                        {
+                                            "conditions": [],
+                                            "endpoint": {
+                                                "headers": {},
+                                                "properties": {},
+                                                "url": "https://airflow.{Region}.{PartitionResult#dnsSuffix}"
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
-                        "url": "https://airflow.{Region}.{PartitionResult#dnsSuffix}"
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

### Comparing `botocore-a-la-carte-mwaa-1.29.99/botocore/data/mwaa/2020-07-01/service-2.json` & `botocore-a-la-carte-mwaa-1.30.0/botocore/data/mwaa/2020-07-01/service-2.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899712747281788%*

 * *Differences: {"'documentation'": "'<p><fullname>Amazon Managed Workflows for Apache Airflow</fullname> <p>This "*

 * *                    'section contains the Amazon Managed Workflows for Apache Airflow (MWAA) API '*

 * *                    'reference documentation. For more information, see <a '*

 * *                    'href="https://docs.aws.amazon.com/mwaa/latest/userguide/what-is-mwaa.html">What '*

 * *                    'is Amazon MWAA?</a>.</p> <p> <b>Endpoints</b> </p> <ul> <li> <p> '*

 * *                    '<code>api.airflow.{regio […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "documentation": "<p><fullname>Amazon Managed Workflows for Apache Airflow</fullname> <p>This section contains the Amazon Managed Workflows for Apache Airflow (MWAA) API reference documentation. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/what-is-mwaa.html\">What Is Amazon MWAA?</a>.</p> <p> <b>Endpoints</b> </p> <ul> <li> <p> <code>api.airflow.{region}.amazonaws.com</code> - This endpoint is used for environment management.</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_CreateEnvironment.html\">CreateEnvironment</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_DeleteEnvironment.html\">DeleteEnvironment</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_GetEnvironment.html\">GetEnvironment</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_ListEnvironments.html\">ListEnvironments</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_ListTagsForResource.html\">ListTagsForResource</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_TagResource.html\">TagResource</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_UntagResource.html\">UntagResource</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_UpdateEnvironment.html\">UpdateEnvironment</a> </p> </li> </ul> </li> <li> <p> <code>env.airflow.{region}.amazonaws.com</code> - This endpoint is used to operate the Airflow environment.</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_CreateCliToken.html \">CreateCliToken</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_CreateWebLoginToken.html\">CreateWebLoginToken</a> </p> </li> </ul> </li> <li> <p> <code>ops.airflow.{region}.amazonaws.com</code> - This endpoint is used to push environment metrics that track environment health.</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_PublishMetrics.html \">PublishMetrics</a> </p> </li> </ul> </li> </ul> <p> <b>Regions</b> </p> <p>For a list of regions that Amazon MWAA supports, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/what-is-mwaa.html#regions-mwaa\">Region availability</a> in the <i>Amazon MWAA User Guide</i>.</p></p>",
+    "documentation": "<p><fullname>Amazon Managed Workflows for Apache Airflow</fullname> <p>This section contains the Amazon Managed Workflows for Apache Airflow (MWAA) API reference documentation. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/what-is-mwaa.html\">What is Amazon MWAA?</a>.</p> <p> <b>Endpoints</b> </p> <ul> <li> <p> <code>api.airflow.{region}.amazonaws.com</code> - This endpoint is used for environment management.</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_CreateEnvironment.html\">CreateEnvironment</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_DeleteEnvironment.html\">DeleteEnvironment</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_GetEnvironment.html\">GetEnvironment</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_ListEnvironments.html\">ListEnvironments</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_ListTagsForResource.html\">ListTagsForResource</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_TagResource.html\">TagResource</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_UntagResource.html\">UntagResource</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_UpdateEnvironment.html\">UpdateEnvironment</a> </p> </li> </ul> </li> <li> <p> <code>env.airflow.{region}.amazonaws.com</code> - This endpoint is used to operate the Airflow environment.</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_CreateCliToken.html \">CreateCliToken</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_CreateWebLoginToken.html\">CreateWebLoginToken</a> </p> </li> </ul> </li> <li> <p> <code>ops.airflow.{region}.amazonaws.com</code> - This endpoint is used to push environment metrics that track environment health.</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/mwaa/latest/API/API_PublishMetrics.html \">PublishMetrics</a> </p> </li> </ul> </li> </ul> <p> <b>Regions</b> </p> <p>For a list of regions that Amazon MWAA supports, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/what-is-mwaa.html#regions-mwaa\">Region availability</a> in the <i>Amazon MWAA User Guide</i>.</p></p>",
     "metadata": {
         "apiVersion": "2020-07-01",
         "endpointPrefix": "airflow",
         "jsonVersion": "1.1",
         "protocol": "rest-json",
         "serviceFullName": "AmazonMWAA",
         "serviceId": "MWAA",
@@ -401,35 +401,35 @@
             },
             "type": "structure"
         },
         "CreateEnvironmentInput": {
             "documentation": "<p>This section contains the Amazon Managed Workflows for Apache Airflow (MWAA) API reference documentation to create an environment. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/get-started.html\">Get started with Amazon Managed Workflows for Apache Airflow</a>.</p>",
             "members": {
                 "AirflowConfigurationOptions": {
-                    "documentation": "<p>A list of key-value pairs containing the Apache Airflow configuration options you want to attach to your environment. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-env-variables.html\">Apache Airflow configuration options</a>.</p>",
+                    "documentation": "<p>A list of key-value pairs containing the Apache Airflow configuration options you want to attach to your environment. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-env-variables.html\">Apache Airflow configuration options</a>.</p>",
                     "shape": "AirflowConfigurationOptions"
                 },
                 "AirflowVersion": {
-                    "documentation": "<p>The Apache Airflow version for your environment. If no value is specified, it defaults to the latest version. Valid values: <code>1.10.12</code>, <code>2.0.2</code>, <code>2.2.2</code>, and <code>2.4.3</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/airflow-versions.html\">Apache Airflow versions on Amazon Managed Workflows for Apache Airflow (MWAA)</a>.</p>",
+                    "documentation": "<p>The Apache Airflow version for your environment. If no value is specified, it defaults to the latest version. Valid values: <code>1.10.12</code>, <code>2.0.2</code>, <code>2.2.2</code>, <code>2.4.3</code>, and <code>2.5.1</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/airflow-versions.html\">Apache Airflow versions on Amazon Managed Workflows for Apache Airflow (MWAA)</a>.</p>",
                     "shape": "AirflowVersion"
                 },
                 "DagS3Path": {
-                    "documentation": "<p>The relative path to the DAGs folder on your Amazon S3 bucket. For example, <code>dags</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-folder.html\">Adding or updating DAGs</a>.</p>",
+                    "documentation": "<p>The relative path to the DAGs folder on your Amazon S3 bucket. For example, <code>dags</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-folder.html\">Adding or updating DAGs</a>.</p>",
                     "shape": "RelativePath"
                 },
                 "EnvironmentClass": {
-                    "documentation": "<p>The environment class type. Valid values: <code>mw1.small</code>, <code>mw1.medium</code>, <code>mw1.large</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/environment-class.html\">Amazon MWAA environment class</a>.</p>",
+                    "documentation": "<p>The environment class type. Valid values: <code>mw1.small</code>, <code>mw1.medium</code>, <code>mw1.large</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/environment-class.html\">Amazon MWAA environment class</a>.</p>",
                     "shape": "EnvironmentClass"
                 },
                 "ExecutionRoleArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the execution role for your environment. An execution role is an Amazon Web Services Identity and Access Management (IAM) role that grants MWAA permission to access Amazon Web Services services and resources used by your environment. For example, <code>arn:aws:iam::123456789:role/my-execution-role</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-create-role.html\">Amazon MWAA Execution role</a>.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the execution role for your environment. An execution role is an Amazon Web Services Identity and Access Management (IAM) role that grants MWAA permission to access Amazon Web Services services and resources used by your environment. For example, <code>arn:aws:iam::123456789:role/my-execution-role</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-create-role.html\">Amazon MWAA Execution role</a>.</p>",
                     "shape": "IamRoleArn"
                 },
                 "KmsKey": {
-                    "documentation": "<p>The Amazon Web Services Key Management Service (KMS) key to encrypt the data in your environment. You can use an Amazon Web Services owned CMK, or a Customer managed CMK (advanced). To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/create-environment.html\">Create an Amazon MWAA environment</a>.</p>",
+                    "documentation": "<p>The Amazon Web Services Key Management Service (KMS) key to encrypt the data in your environment. You can use an Amazon Web Services owned CMK, or a Customer managed CMK (advanced). For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/create-environment.html\">Create an Amazon MWAA environment</a>.</p>",
                     "shape": "KmsKey"
                 },
                 "LoggingConfiguration": {
                     "documentation": "<p>Defines the Apache Airflow logs to send to CloudWatch Logs.</p>",
                     "shape": "LoggingConfigurationInput"
                 },
                 "MaxWorkers": {
@@ -443,47 +443,55 @@
                 "Name": {
                     "documentation": "<p>The name of the Amazon MWAA environment. For example, <code>MyMWAAEnvironment</code>.</p>",
                     "location": "uri",
                     "locationName": "Name",
                     "shape": "EnvironmentName"
                 },
                 "NetworkConfiguration": {
-                    "documentation": "<p>The VPC networking components used to secure and enable network traffic between the Amazon Web Services resources for your environment. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html\">About networking on Amazon MWAA</a>.</p>",
+                    "documentation": "<p>The VPC networking components used to secure and enable network traffic between the Amazon Web Services resources for your environment. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html\">About networking on Amazon MWAA</a>.</p>",
                     "shape": "NetworkConfiguration"
                 },
                 "PluginsS3ObjectVersion": {
-                    "documentation": "<p>The version of the plugins.zip file on your Amazon S3 bucket. A version must be specified each time a plugins.zip file is updated. To learn more, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">How S3 Versioning works</a>.</p>",
+                    "documentation": "<p>The version of the plugins.zip file on your Amazon S3 bucket. You must specify a version each time a plugins.zip file is updated. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">How S3 Versioning works</a>.</p>",
                     "shape": "S3ObjectVersion"
                 },
                 "PluginsS3Path": {
-                    "documentation": "<p>The relative path to the <code>plugins.zip</code> file on your Amazon S3 bucket. For example, <code>plugins.zip</code>. If specified, then the plugins.zip version is required. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html\">Installing custom plugins</a>.</p>",
+                    "documentation": "<p>The relative path to the <code>plugins.zip</code> file on your Amazon S3 bucket. For example, <code>plugins.zip</code>. If specified, then the <code>plugins.zip</code> version is required. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html\">Installing custom plugins</a>.</p>",
                     "shape": "RelativePath"
                 },
                 "RequirementsS3ObjectVersion": {
-                    "documentation": "<p>The version of the requirements.txt file on your Amazon S3 bucket. A version must be specified each time a requirements.txt file is updated. To learn more, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">How S3 Versioning works</a>.</p>",
+                    "documentation": "<p>The version of the <code>requirements.txt</code> file on your Amazon S3 bucket. You must specify a version each time a requirements.txt file is updated. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">How S3 Versioning works</a>.</p>",
                     "shape": "S3ObjectVersion"
                 },
                 "RequirementsS3Path": {
-                    "documentation": "<p>The relative path to the <code>requirements.txt</code> file on your Amazon S3 bucket. For example, <code>requirements.txt</code>. If specified, then a file version is required. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html\">Installing Python dependencies</a>.</p>",
+                    "documentation": "<p>The relative path to the <code>requirements.txt</code> file on your Amazon S3 bucket. For example, <code>requirements.txt</code>. If specified, then a version is required. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html\">Installing Python dependencies</a>.</p>",
                     "shape": "RelativePath"
                 },
                 "Schedulers": {
                     "documentation": "<p>The number of Apache Airflow schedulers to run in your environment. Valid values:</p> <ul> <li> <p>v2 - Accepts between 2 to 5. Defaults to 2.</p> </li> <li> <p>v1 - Accepts 1.</p> </li> </ul>",
                     "shape": "Schedulers"
                 },
                 "SourceBucketArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon S3 bucket where your DAG code and supporting files are stored. For example, <code>arn:aws:s3:::my-airflow-bucket-unique-name</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-s3-bucket.html\">Create an Amazon S3 bucket for Amazon MWAA</a>.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon S3 bucket where your DAG code and supporting files are stored. For example, <code>arn:aws:s3:::my-airflow-bucket-unique-name</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-s3-bucket.html\">Create an Amazon S3 bucket for Amazon MWAA</a>.</p>",
                     "shape": "S3BucketArn"
                 },
+                "StartupScriptS3ObjectVersion": {
+                    "documentation": "<p>The version of the startup shell script in your Amazon S3 bucket. You must specify the <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">version ID</a> that Amazon S3 assigns to the file every time you update the script. </p> <p> Version IDs are Unicode, UTF-8 encoded, URL-ready, opaque strings that are no more than 1,024 bytes long. The following is an example: </p> <p> <code>3sL4kqtJlcpXroDTDmJ+rmSpXd3dIbrHY+MTRCxf3vjVBH40Nr8X8gdRQBpUMLUo</code> </p> <p> For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html\">Using a startup script</a>. </p>",
+                    "shape": "S3ObjectVersion"
+                },
+                "StartupScriptS3Path": {
+                    "documentation": "<p>The relative path to the startup shell script in your Amazon S3 bucket. For example, <code>s3://mwaa-environment/startup.sh</code>.</p> <p> Amazon MWAA runs the script as your environment starts, and before running the Apache Airflow process. You can use this script to install dependencies, modify Apache Airflow configuration options, and set environment variables. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html\">Using a startup script</a>. </p>",
+                    "shape": "RelativePath"
+                },
                 "Tags": {
-                    "documentation": "<p>The key-value tag pairs you want to associate to your environment. For example, <code>\"Environment\": \"Staging\"</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a>.</p>",
+                    "documentation": "<p>The key-value tag pairs you want to associate to your environment. For example, <code>\"Environment\": \"Staging\"</code>. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a>.</p>",
                     "shape": "TagMap"
                 },
                 "WebserverAccessMode": {
-                    "documentation": "<p>The Apache Airflow <i>Web server</i> access mode. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-networking.html\">Apache Airflow access modes</a>.</p>",
+                    "documentation": "<p>The Apache Airflow <i>Web server</i> access mode. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-networking.html\">Apache Airflow access modes</a>.</p>",
                     "shape": "WebserverAccessMode"
                 },
                 "WeeklyMaintenanceWindowStart": {
                     "documentation": "<p>The day and time of the week in Coordinated Universal Time (UTC) 24-hour standard time to start weekly maintenance updates of your environment in the following format: <code>DAY:HH:MM</code>. For example: <code>TUE:03:30</code>. You can specify a start time in 30 minute increments only.</p>",
                     "shape": "WeeklyMaintenanceWindowStart"
                 }
             },
@@ -581,39 +589,39 @@
             "box": true,
             "type": "double"
         },
         "Environment": {
             "documentation": "<p>Describes an Amazon Managed Workflows for Apache Airflow (MWAA) environment.</p>",
             "members": {
                 "AirflowConfigurationOptions": {
-                    "documentation": "<p>A list of key-value pairs containing the Apache Airflow configuration options attached to your environment. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-env-variables.html\">Apache Airflow configuration options</a>.</p>",
+                    "documentation": "<p>A list of key-value pairs containing the Apache Airflow configuration options attached to your environment. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-env-variables.html\">Apache Airflow configuration options</a>.</p>",
                     "shape": "AirflowConfigurationOptions"
                 },
                 "AirflowVersion": {
-                    "documentation": "<p>The Apache Airflow version on your environment. Valid values: <code>1.10.12</code>, <code>2.0.2</code>, <code>2.2.2</code>, and <code>2.4.3</code>.</p>",
+                    "documentation": "<p>The Apache Airflow version on your environment. Valid values: <code>1.10.12</code>, <code>2.0.2</code>, <code>2.2.2</code>, <code>2.4.3</code>, and <code>2.5.1</code>.</p>",
                     "shape": "AirflowVersion"
                 },
                 "Arn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon MWAA environment.</p>",
                     "shape": "EnvironmentArn"
                 },
                 "CreatedAt": {
                     "documentation": "<p>The day and time the environment was created.</p>",
                     "shape": "CreatedAt"
                 },
                 "DagS3Path": {
-                    "documentation": "<p>The relative path to the DAGs folder on your Amazon S3 bucket. For example, <code>dags</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-folder.html\">Adding or updating DAGs</a>.</p>",
+                    "documentation": "<p>The relative path to the DAGs folder in your Amazon S3 bucket. For example, <code>s3://mwaa-environment/dags</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-folder.html\">Adding or updating DAGs</a>.</p>",
                     "shape": "RelativePath"
                 },
                 "EnvironmentClass": {
-                    "documentation": "<p>The environment class type. Valid values: <code>mw1.small</code>, <code>mw1.medium</code>, <code>mw1.large</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/environment-class.html\">Amazon MWAA environment class</a>.</p>",
+                    "documentation": "<p>The environment class type. Valid values: <code>mw1.small</code>, <code>mw1.medium</code>, <code>mw1.large</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/environment-class.html\">Amazon MWAA environment class</a>.</p>",
                     "shape": "EnvironmentClass"
                 },
                 "ExecutionRoleArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the execution role in IAM that allows MWAA to access Amazon Web Services resources in your environment. For example, <code>arn:aws:iam::123456789:role/my-execution-role</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-create-role.html\">Amazon MWAA Execution role</a>.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the execution role in IAM that allows MWAA to access Amazon Web Services resources in your environment. For example, <code>arn:aws:iam::123456789:role/my-execution-role</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-create-role.html\">Amazon MWAA Execution role</a>.</p>",
                     "shape": "IamRoleArn"
                 },
                 "KmsKey": {
                     "documentation": "<p>The Amazon Web Services Key Management Service (KMS) encryption key used to encrypt the data in your environment.</p>",
                     "shape": "KmsKey"
                 },
                 "LastUpdate": {
@@ -633,59 +641,67 @@
                     "shape": "MinWorkers"
                 },
                 "Name": {
                     "documentation": "<p>The name of the Amazon MWAA environment. For example, <code>MyMWAAEnvironment</code>.</p>",
                     "shape": "EnvironmentName"
                 },
                 "NetworkConfiguration": {
-                    "documentation": "<p>Describes the VPC networking components used to secure and enable network traffic between the Amazon Web Services resources for your environment. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html\">About networking on Amazon MWAA</a>.</p>",
+                    "documentation": "<p>Describes the VPC networking components used to secure and enable network traffic between the Amazon Web Services resources for your environment. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html\">About networking on Amazon MWAA</a>.</p>",
                     "shape": "NetworkConfiguration"
                 },
                 "PluginsS3ObjectVersion": {
-                    "documentation": "<p>The version of the plugins.zip file on your Amazon S3 bucket. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html\">Installing custom plugins</a>.</p>",
+                    "documentation": "<p>The version of the <code>plugins.zip</code> file in your Amazon S3 bucket. You must specify the <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">version ID</a> that Amazon S3 assigns to the file.</p> <p> Version IDs are Unicode, UTF-8 encoded, URL-ready, opaque strings that are no more than 1,024 bytes long. The following is an example: </p> <p> <code>3sL4kqtJlcpXroDTDmJ+rmSpXd3dIbrHY+MTRCxf3vjVBH40Nr8X8gdRQBpUMLUo</code> </p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html\">Installing custom plugins</a>.</p>",
                     "shape": "S3ObjectVersion"
                 },
                 "PluginsS3Path": {
-                    "documentation": "<p>The relative path to the <code>plugins.zip</code> file on your Amazon S3 bucket. For example, <code>plugins.zip</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html\">Installing custom plugins</a>.</p>",
+                    "documentation": "<p>The relative path to the file in your Amazon S3 bucket. For example, <code>s3://mwaa-environment/plugins.zip</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html\">Installing custom plugins</a>.</p>",
                     "shape": "RelativePath"
                 },
                 "RequirementsS3ObjectVersion": {
-                    "documentation": "<p>The version of the requirements.txt file on your Amazon S3 bucket. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html\">Installing Python dependencies</a>.</p>",
+                    "documentation": "<p>The version of the <code>requirements.txt </code> file on your Amazon S3 bucket. You must specify the <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">version ID</a> that Amazon S3 assigns to the file.</p> <p> Version IDs are Unicode, UTF-8 encoded, URL-ready, opaque strings that are no more than 1,024 bytes long. The following is an example: </p> <p> <code>3sL4kqtJlcpXroDTDmJ+rmSpXd3dIbrHY+MTRCxf3vjVBH40Nr8X8gdRQBpUMLUo</code> </p> <p> For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html\">Installing Python dependencies</a>. </p>",
                     "shape": "S3ObjectVersion"
                 },
                 "RequirementsS3Path": {
-                    "documentation": "<p>The relative path to the <code>requirements.txt</code> file on your Amazon S3 bucket. For example, <code>requirements.txt</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html\">Installing Python dependencies</a>.</p>",
+                    "documentation": "<p>The relative path to the <code>requirements.txt</code> file in your Amazon S3 bucket. For example, <code>s3://mwaa-environment/requirements.txt</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html\">Installing Python dependencies</a>.</p>",
                     "shape": "RelativePath"
                 },
                 "Schedulers": {
                     "documentation": "<p>The number of Apache Airflow schedulers that run in your Amazon MWAA environment.</p>",
                     "shape": "Schedulers"
                 },
                 "ServiceRoleArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) for the service-linked role of the environment. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-slr.html\">Amazon MWAA Service-linked role</a>.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) for the service-linked role of the environment. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-slr.html\">Amazon MWAA Service-linked role</a>.</p>",
                     "shape": "IamRoleArn"
                 },
                 "SourceBucketArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon S3 bucket where your DAG code and supporting files are stored. For example, <code>arn:aws:s3:::my-airflow-bucket-unique-name</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-s3-bucket.html\">Create an Amazon S3 bucket for Amazon MWAA</a>.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon S3 bucket where your DAG code and supporting files are stored. For example, <code>arn:aws:s3:::my-airflow-bucket-unique-name</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-s3-bucket.html\">Create an Amazon S3 bucket for Amazon MWAA</a>.</p>",
                     "shape": "S3BucketArn"
                 },
+                "StartupScriptS3ObjectVersion": {
+                    "documentation": "<p>The version of the startup shell script in your Amazon S3 bucket. You must specify the <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">version ID</a> that Amazon S3 assigns to the file.</p> <p> Version IDs are Unicode, UTF-8 encoded, URL-ready, opaque strings that are no more than 1,024 bytes long. The following is an example: </p> <p> <code>3sL4kqtJlcpXroDTDmJ+rmSpXd3dIbrHY+MTRCxf3vjVBH40Nr8X8gdRQBpUMLUo</code> </p> <p> For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html\">Using a startup script</a>. </p>",
+                    "shape": "String"
+                },
+                "StartupScriptS3Path": {
+                    "documentation": "<p>The relative path to the startup shell script in your Amazon S3 bucket. For example, <code>s3://mwaa-environment/startup.sh</code>.</p> <p> Amazon MWAA runs the script as your environment starts, and before running the Apache Airflow process. You can use this script to install dependencies, modify Apache Airflow configuration options, and set environment variables. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html\">Using a startup script</a>. </p>",
+                    "shape": "String"
+                },
                 "Status": {
-                    "documentation": "<p>The status of the Amazon MWAA environment. Valid values:</p> <ul> <li> <p> <code>CREATING</code> - Indicates the request to create the environment is in progress.</p> </li> <li> <p> <code>CREATE_FAILED</code> - Indicates the request to create the environment failed, and the environment could not be created.</p> </li> <li> <p> <code>AVAILABLE</code> - Indicates the request was successful and the environment is ready to use.</p> </li> <li> <p> <code>UPDATING</code> - Indicates the request to update the environment is in progress.</p> </li> <li> <p> <code>DELETING</code> - Indicates the request to delete the environment is in progress.</p> </li> <li> <p> <code>DELETED</code> - Indicates the request to delete the environment is complete, and the environment has been deleted.</p> </li> <li> <p> <code>UNAVAILABLE</code> - Indicates the request failed, but the environment was unable to rollback and is not in a stable state.</p> </li> <li> <p> <code>UPDATE_FAILED</code> - Indicates the request to update the environment failed, and the environment has rolled back successfully and is ready to use.</p> </li> </ul> <p>We recommend reviewing our troubleshooting guide for a list of common errors and their solutions. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/troubleshooting.html\">Amazon MWAA troubleshooting</a>.</p>",
+                    "documentation": "<p>The status of the Amazon MWAA environment. Valid values:</p> <ul> <li> <p> <code>CREATING</code> - Indicates the request to create the environment is in progress.</p> </li> <li> <p> <code>CREATING_SNAPSHOT</code> - Indicates the request to update environment details, or upgrade the environment version, is in progress and Amazon MWAA is creating a storage volume snapshot of the Amazon RDS database cluster associated with the environment. A database snapshot is a backup created at a specific point in time. Amazon MWAA uses snapshots to recover environment metadata if the process to update or upgrade an environment fails.</p> </li> <li> <p> <code>CREATE_FAILED</code> - Indicates the request to create the environment failed, and the environment could not be created.</p> </li> <li> <p> <code>AVAILABLE</code> - Indicates the request was successful and the environment is ready to use.</p> </li> <li> <p> <code>UPDATING</code> - Indicates the request to update the environment is in progress.</p> </li> <li> <p> <code>ROLLING_BACK</code> - Indicates the request to update environment details, or upgrade the environment version, failed and Amazon MWAA is restoring the environment using the latest storage volume snapshot.</p> </li> <li> <p> <code>DELETING</code> - Indicates the request to delete the environment is in progress.</p> </li> <li> <p> <code>DELETED</code> - Indicates the request to delete the environment is complete, and the environment has been deleted.</p> </li> <li> <p> <code>UNAVAILABLE</code> - Indicates the request failed, but the environment was unable to rollback and is not in a stable state.</p> </li> <li> <p> <code>UPDATE_FAILED</code> - Indicates the request to update the environment failed, and the environment has rolled back successfully and is ready to use.</p> </li> </ul> <p>We recommend reviewing our troubleshooting guide for a list of common errors and their solutions. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/troubleshooting.html\">Amazon MWAA troubleshooting</a>.</p>",
                     "shape": "EnvironmentStatus"
                 },
                 "Tags": {
-                    "documentation": "<p>The key-value tag pairs associated to your environment. For example, <code>\"Environment\": \"Staging\"</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a>.</p>",
+                    "documentation": "<p>The key-value tag pairs associated to your environment. For example, <code>\"Environment\": \"Staging\"</code>. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a>.</p>",
                     "shape": "TagMap"
                 },
                 "WebserverAccessMode": {
-                    "documentation": "<p>The Apache Airflow <i>Web server</i> access mode. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-networking.html\">Apache Airflow access modes</a>.</p>",
+                    "documentation": "<p>The Apache Airflow <i>Web server</i> access mode. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-networking.html\">Apache Airflow access modes</a>.</p>",
                     "shape": "WebserverAccessMode"
                 },
                 "WebserverUrl": {
-                    "documentation": "<p>The Apache Airflow <i>Web server</i> host name for the Amazon MWAA environment. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/access-airflow-ui.html\">Accessing the Apache Airflow UI</a>.</p>",
+                    "documentation": "<p>The Apache Airflow <i>Web server</i> host name for the Amazon MWAA environment. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/access-airflow-ui.html\">Accessing the Apache Airflow UI</a>.</p>",
                     "shape": "WebserverUrl"
                 },
                 "WeeklyMaintenanceWindowStart": {
                     "documentation": "<p>The day and time of the week in Coordinated Universal Time (UTC) 24-hour standard time that weekly maintenance updates are scheduled. For example: <code>TUE:03:30</code>.</p>",
                     "shape": "WeeklyMaintenanceWindowStart"
                 }
             },
@@ -719,15 +735,17 @@
                 "CREATING",
                 "CREATE_FAILED",
                 "AVAILABLE",
                 "UPDATING",
                 "DELETING",
                 "DELETED",
                 "UNAVAILABLE",
-                "UPDATE_FAILED"
+                "UPDATE_FAILED",
+                "ROLLING_BACK",
+                "CREATING_SNAPSHOT"
             ],
             "type": "string"
         },
         "ErrorCode": {
             "type": "string"
         },
         "ErrorMessage": {
@@ -869,15 +887,15 @@
                 "ResourceArn"
             ],
             "type": "structure"
         },
         "ListTagsForResourceOutput": {
             "members": {
                 "Tags": {
-                    "documentation": "<p>The key-value tag pairs associated to your environment. To learn more, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a>.</p>",
+                    "documentation": "<p>The key-value tag pairs associated to your environment. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a>.</p>",
                     "shape": "TagMap"
                 }
             },
             "type": "structure"
         },
         "LoggingConfiguration": {
             "documentation": "<p>Describes the Apache Airflow log types that are published to CloudWatch Logs.</p>",
@@ -1028,22 +1046,22 @@
             "required": [
                 "Enabled",
                 "LogLevel"
             ],
             "type": "structure"
         },
         "NetworkConfiguration": {
-            "documentation": "<p>Describes the VPC networking components used to secure and enable network traffic between the Amazon Web Services resources for your environment. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html\">About networking on Amazon MWAA</a>.</p>",
+            "documentation": "<p>Describes the VPC networking components used to secure and enable network traffic between the Amazon Web Services resources for your environment. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html\">About networking on Amazon MWAA</a>.</p>",
             "members": {
                 "SecurityGroupIds": {
-                    "documentation": "<p>A list of security group IDs. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/vpc-security.html\">Security in your VPC on Amazon MWAA</a>.</p>",
+                    "documentation": "<p>A list of security group IDs. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/vpc-security.html\">Security in your VPC on Amazon MWAA</a>.</p>",
                     "shape": "SecurityGroupList"
                 },
                 "SubnetIds": {
-                    "documentation": "<p>A list of subnet IDs. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html\">About networking on Amazon MWAA</a>.</p>",
+                    "documentation": "<p>A list of subnet IDs. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html\">About networking on Amazon MWAA</a>.</p>",
                     "shape": "SubnetList"
                 }
             },
             "type": "structure"
         },
         "NextToken": {
             "max": 2048,
@@ -1192,15 +1210,15 @@
                 "ResourceArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon MWAA environment. For example, <code>arn:aws:airflow:us-east-1:123456789012:environment/MyMWAAEnvironment</code>.</p>",
                     "location": "uri",
                     "locationName": "ResourceArn",
                     "shape": "EnvironmentArn"
                 },
                 "Tags": {
-                    "documentation": "<p>The key-value tag pairs you want to associate to your environment. For example, <code>\"Environment\": \"Staging\"</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a>.</p>",
+                    "documentation": "<p>The key-value tag pairs you want to associate to your environment. For example, <code>\"Environment\": \"Staging\"</code>. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a>.</p>",
                     "shape": "TagMap"
                 }
             },
             "required": [
                 "ResourceArn",
                 "Tags"
             ],
@@ -1282,31 +1300,31 @@
         },
         "UpdateCreatedAt": {
             "type": "timestamp"
         },
         "UpdateEnvironmentInput": {
             "members": {
                 "AirflowConfigurationOptions": {
-                    "documentation": "<p>A list of key-value pairs containing the Apache Airflow configuration options you want to attach to your environment. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-env-variables.html\">Apache Airflow configuration options</a>.</p>",
+                    "documentation": "<p>A list of key-value pairs containing the Apache Airflow configuration options you want to attach to your environment. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-env-variables.html\">Apache Airflow configuration options</a>.</p>",
                     "shape": "AirflowConfigurationOptions"
                 },
                 "AirflowVersion": {
-                    "documentation": "<p>The Apache Airflow version for your environment. If no value is specified, defaults to the latest version. Valid values: <code>1.10.12</code>, <code>2.0.2</code>, <code>2.2.2</code>, and <code>2.4.3</code>.</p>",
+                    "documentation": "<p>The Apache Airflow version for your environment. To upgrade your environment, specify a newer version of Apache Airflow supported by Amazon MWAA.</p> <p>Before you upgrade an environment, make sure your requirements, DAGs, plugins, and other resources used in your workflows are compatible with the new Apache Airflow version. For more information about updating your resources, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/upgrading-environment.html\">Upgrading an Amazon MWAA environment</a>.</p> <p>Valid values: <code>1.10.12</code>, <code>2.0.2</code>, <code>2.2.2</code>, <code>2.4.3</code>, and <code>2.5.1</code>.</p>",
                     "shape": "AirflowVersion"
                 },
                 "DagS3Path": {
-                    "documentation": "<p>The relative path to the DAGs folder on your Amazon S3 bucket. For example, <code>dags</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-folder.html\">Adding or updating DAGs</a>.</p>",
+                    "documentation": "<p>The relative path to the DAGs folder on your Amazon S3 bucket. For example, <code>dags</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-folder.html\">Adding or updating DAGs</a>.</p>",
                     "shape": "RelativePath"
                 },
                 "EnvironmentClass": {
-                    "documentation": "<p>The environment class type. Valid values: <code>mw1.small</code>, <code>mw1.medium</code>, <code>mw1.large</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/environment-class.html\">Amazon MWAA environment class</a>.</p>",
+                    "documentation": "<p>The environment class type. Valid values: <code>mw1.small</code>, <code>mw1.medium</code>, <code>mw1.large</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/environment-class.html\">Amazon MWAA environment class</a>.</p>",
                     "shape": "EnvironmentClass"
                 },
                 "ExecutionRoleArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the execution role in IAM that allows MWAA to access Amazon Web Services resources in your environment. For example, <code>arn:aws:iam::123456789:role/my-execution-role</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-create-role.html\">Amazon MWAA Execution role</a>.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the execution role in IAM that allows MWAA to access Amazon Web Services resources in your environment. For example, <code>arn:aws:iam::123456789:role/my-execution-role</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-create-role.html\">Amazon MWAA Execution role</a>.</p>",
                     "shape": "IamRoleArn"
                 },
                 "LoggingConfiguration": {
                     "documentation": "<p>The Apache Airflow log types to send to CloudWatch Logs.</p>",
                     "shape": "LoggingConfigurationInput"
                 },
                 "MaxWorkers": {
@@ -1320,43 +1338,51 @@
                 "Name": {
                     "documentation": "<p>The name of your Amazon MWAA environment. For example, <code>MyMWAAEnvironment</code>.</p>",
                     "location": "uri",
                     "locationName": "Name",
                     "shape": "EnvironmentName"
                 },
                 "NetworkConfiguration": {
-                    "documentation": "<p>The VPC networking components used to secure and enable network traffic between the Amazon Web Services resources for your environment. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html\">About networking on Amazon MWAA</a>.</p>",
+                    "documentation": "<p>The VPC networking components used to secure and enable network traffic between the Amazon Web Services resources for your environment. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html\">About networking on Amazon MWAA</a>.</p>",
                     "shape": "UpdateNetworkConfigurationInput"
                 },
                 "PluginsS3ObjectVersion": {
-                    "documentation": "<p>The version of the plugins.zip file on your Amazon S3 bucket. A version must be specified each time a plugins.zip file is updated. To learn more, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">How S3 Versioning works</a>.</p>",
+                    "documentation": "<p>The version of the plugins.zip file on your Amazon S3 bucket. You must specify a version each time a <code>plugins.zip</code> file is updated. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">How S3 Versioning works</a>.</p>",
                     "shape": "S3ObjectVersion"
                 },
                 "PluginsS3Path": {
-                    "documentation": "<p>The relative path to the <code>plugins.zip</code> file on your Amazon S3 bucket. For example, <code>plugins.zip</code>. If specified, then the plugins.zip version is required. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html\">Installing custom plugins</a>.</p>",
+                    "documentation": "<p>The relative path to the <code>plugins.zip</code> file on your Amazon S3 bucket. For example, <code>plugins.zip</code>. If specified, then the plugins.zip version is required. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html\">Installing custom plugins</a>.</p>",
                     "shape": "RelativePath"
                 },
                 "RequirementsS3ObjectVersion": {
-                    "documentation": "<p>The version of the requirements.txt file on your Amazon S3 bucket. A version must be specified each time a requirements.txt file is updated. To learn more, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">How S3 Versioning works</a>.</p>",
+                    "documentation": "<p>The version of the requirements.txt file on your Amazon S3 bucket. You must specify a version each time a <code>requirements.txt</code> file is updated. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">How S3 Versioning works</a>.</p>",
                     "shape": "S3ObjectVersion"
                 },
                 "RequirementsS3Path": {
-                    "documentation": "<p>The relative path to the <code>requirements.txt</code> file on your Amazon S3 bucket. For example, <code>requirements.txt</code>. If specified, then a file version is required. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html\">Installing Python dependencies</a>.</p>",
+                    "documentation": "<p>The relative path to the <code>requirements.txt</code> file on your Amazon S3 bucket. For example, <code>requirements.txt</code>. If specified, then a file version is required. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html\">Installing Python dependencies</a>.</p>",
                     "shape": "RelativePath"
                 },
                 "Schedulers": {
                     "documentation": "<p>The number of Apache Airflow schedulers to run in your Amazon MWAA environment.</p>",
                     "shape": "Schedulers"
                 },
                 "SourceBucketArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon S3 bucket where your DAG code and supporting files are stored. For example, <code>arn:aws:s3:::my-airflow-bucket-unique-name</code>. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-s3-bucket.html\">Create an Amazon S3 bucket for Amazon MWAA</a>.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the Amazon S3 bucket where your DAG code and supporting files are stored. For example, <code>arn:aws:s3:::my-airflow-bucket-unique-name</code>. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/mwaa-s3-bucket.html\">Create an Amazon S3 bucket for Amazon MWAA</a>.</p>",
                     "shape": "S3BucketArn"
                 },
+                "StartupScriptS3ObjectVersion": {
+                    "documentation": "<p> The version of the startup shell script in your Amazon S3 bucket. You must specify the <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/versioning-workflows.html\">version ID</a> that Amazon S3 assigns to the file every time you update the script. </p> <p> Version IDs are Unicode, UTF-8 encoded, URL-ready, opaque strings that are no more than 1,024 bytes long. The following is an example: </p> <p> <code>3sL4kqtJlcpXroDTDmJ+rmSpXd3dIbrHY+MTRCxf3vjVBH40Nr8X8gdRQBpUMLUo</code> </p> <p> For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html\">Using a startup script</a>. </p>",
+                    "shape": "S3ObjectVersion"
+                },
+                "StartupScriptS3Path": {
+                    "documentation": "<p>The relative path to the startup shell script in your Amazon S3 bucket. For example, <code>s3://mwaa-environment/startup.sh</code>.</p> <p> Amazon MWAA runs the script as your environment starts, and before running the Apache Airflow process. You can use this script to install dependencies, modify Apache Airflow configuration options, and set environment variables. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html\">Using a startup script</a>. </p>",
+                    "shape": "RelativePath"
+                },
                 "WebserverAccessMode": {
-                    "documentation": "<p>The Apache Airflow <i>Web server</i> access mode. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-networking.html\">Apache Airflow access modes</a>.</p>",
+                    "documentation": "<p>The Apache Airflow <i>Web server</i> access mode. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-networking.html\">Apache Airflow access modes</a>.</p>",
                     "shape": "WebserverAccessMode"
                 },
                 "WeeklyMaintenanceWindowStart": {
                     "documentation": "<p>The day and time of the week in Coordinated Universal Time (UTC) 24-hour standard time to start weekly maintenance updates of your environment in the following format: <code>DAY:HH:MM</code>. For example: <code>TUE:03:30</code>. You can specify a start time in 30 minute increments only.</p>",
                     "shape": "WeeklyMaintenanceWindowStart"
                 }
             },
@@ -1385,18 +1411,18 @@
                     "documentation": "<p>The error message that corresponds to the error code.</p>",
                     "shape": "ErrorMessage"
                 }
             },
             "type": "structure"
         },
         "UpdateNetworkConfigurationInput": {
-            "documentation": "<p>Defines the VPC networking components used to secure and enable network traffic between the Amazon Web Services resources for your environment. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html\">About networking on Amazon MWAA</a>.</p>",
+            "documentation": "<p>Defines the VPC networking components used to secure and enable network traffic between the Amazon Web Services resources for your environment. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/networking-about.html\">About networking on Amazon MWAA</a>.</p>",
             "members": {
                 "SecurityGroupIds": {
-                    "documentation": "<p>A list of security group IDs. A security group must be attached to the same VPC as the subnets. To learn more, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/vpc-security.html\">Security in your VPC on Amazon MWAA</a>.</p>",
+                    "documentation": "<p>A list of security group IDs. A security group must be attached to the same VPC as the subnets. For more information, see <a href=\"https://docs.aws.amazon.com/mwaa/latest/userguide/vpc-security.html\">Security in your VPC on Amazon MWAA</a>.</p>",
                     "shape": "SecurityGroupList"
                 }
             },
             "required": [
                 "SecurityGroupIds"
             ],
             "type": "structure"
```

### Comparing `botocore-a-la-carte-mwaa-1.29.99/botocore_a_la_carte_mwaa.egg-info/PKG-INFO` & `botocore-a-la-carte-mwaa-1.30.0/botocore_a_la_carte_mwaa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-mwaa
-Version: 1.29.99
+Version: 1.30.0
 Summary: mwaa data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-mwaa-1.29.99/setup.py` & `botocore-a-la-carte-mwaa-1.30.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-mwaa',
-    version="1.29.99",
+    version="1.30.0",
     description='mwaa data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/mwaa/*/*.json'],
```

