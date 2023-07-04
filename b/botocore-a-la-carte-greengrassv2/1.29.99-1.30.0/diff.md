# Comparing `tmp/botocore-a-la-carte-greengrassv2-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-greengrassv2-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-greengrassv2-1.29.99.tar", last modified: Sat Mar 25 01:22:35 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-greengrassv2-1.30.0.tar", last modified: Tue Jul  4 01:44:25 2023, max compression
```

## Comparing `botocore-a-la-carte-greengrassv2-1.29.99.tar` & `botocore-a-la-carte-greengrassv2-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.319083 botocore-a-la-carte-greengrassv2-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:35.000000 botocore-a-la-carte-greengrassv2-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-25 01:22:35.315083 botocore-a-la-carte-greengrassv2-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.311082 botocore-a-la-carte-greengrassv2-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.311082 botocore-a-la-carte-greengrassv2-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.311082 botocore-a-la-carte-greengrassv2-1.29.99/botocore/data/greengrassv2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.315083 botocore-a-la-carte-greengrassv2-1.29.99/botocore/data/greengrassv2/2020-11-30/
--rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-03-25 01:22:12.000000 botocore-a-la-carte-greengrassv2-1.29.99/botocore/data/greengrassv2/2020-11-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-greengrassv2-1.29.99/botocore/data/greengrassv2/2020-11-30/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-25 01:22:12.000000 botocore-a-la-carte-greengrassv2-1.29.99/botocore/data/greengrassv2/2020-11-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   142709 2023-03-25 01:22:12.000000 botocore-a-la-carte-greengrassv2-1.29.99/botocore/data/greengrassv2/2020-11-30/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.315083 botocore-a-la-carte-greengrassv2-1.29.99/botocore_a_la_carte_greengrassv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-25 01:22:35.000000 botocore-a-la-carte-greengrassv2-1.29.99/botocore_a_la_carte_greengrassv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-25 01:22:35.000000 botocore-a-la-carte-greengrassv2-1.29.99/botocore_a_la_carte_greengrassv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:35.000000 botocore-a-la-carte-greengrassv2-1.29.99/botocore_a_la_carte_greengrassv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:35.000000 botocore-a-la-carte-greengrassv2-1.29.99/botocore_a_la_carte_greengrassv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:35.319083 botocore-a-la-carte-greengrassv2-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-25 01:22:35.000000 botocore-a-la-carte-greengrassv2-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:25.794500 botocore-a-la-carte-greengrassv2-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:25.000000 botocore-a-la-carte-greengrassv2-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-04 01:44:25.794500 botocore-a-la-carte-greengrassv2-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:25.794500 botocore-a-la-carte-greengrassv2-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:25.794500 botocore-a-la-carte-greengrassv2-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:25.794500 botocore-a-la-carte-greengrassv2-1.30.0/botocore/data/greengrassv2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:25.794500 botocore-a-la-carte-greengrassv2-1.30.0/botocore/data/greengrassv2/2020-11-30/
+-rw-r--r--   0 runner    (1001) docker     (123)    23970 2023-07-04 01:44:02.000000 botocore-a-la-carte-greengrassv2-1.30.0/botocore/data/greengrassv2/2020-11-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-greengrassv2-1.30.0/botocore/data/greengrassv2/2020-11-30/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-04 01:44:02.000000 botocore-a-la-carte-greengrassv2-1.30.0/botocore/data/greengrassv2/2020-11-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   143746 2023-07-04 01:44:02.000000 botocore-a-la-carte-greengrassv2-1.30.0/botocore/data/greengrassv2/2020-11-30/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:25.794500 botocore-a-la-carte-greengrassv2-1.30.0/botocore_a_la_carte_greengrassv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-04 01:44:25.000000 botocore-a-la-carte-greengrassv2-1.30.0/botocore_a_la_carte_greengrassv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-04 01:44:25.000000 botocore-a-la-carte-greengrassv2-1.30.0/botocore_a_la_carte_greengrassv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:25.000000 botocore-a-la-carte-greengrassv2-1.30.0/botocore_a_la_carte_greengrassv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:25.000000 botocore-a-la-carte-greengrassv2-1.30.0/botocore_a_la_carte_greengrassv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:25.794500 botocore-a-la-carte-greengrassv2-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-04 01:44:25.000000 botocore-a-la-carte-greengrassv2-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-greengrassv2-1.29.99/LICENSE.txt` & `botocore-a-la-carte-greengrassv2-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-greengrassv2-1.29.99/PKG-INFO` & `botocore-a-la-carte-greengrassv2-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-greengrassv2
-Version: 1.29.99
+Version: 1.30.0
 Summary: greengrassv2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-greengrassv2-1.29.99/botocore/data/greengrassv2/2020-11-30/endpoint-rule-set-1.json` & `botocore-a-la-carte-greengrassv2-1.30.0/botocore/data/greengrassv2/2020-11-30/endpoint-rule-set-1.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8955476787551441%*

 * *Differences: {"'parameters'": "{'Region': {'required': False}}",*

 * * "'rules'": "{0: {'conditions': {0: {'fn': 'isSet', 'argv': {0: {'ref': 'Endpoint'}}, delete: "*

 * *            "['assign']}}, 'rules': {0: {'type': 'error', 'error': 'Invalid Configuration: FIPS "*

 * *            "and custom endpoint are not supported', delete: ['rules']}, 1: {'rules': {0: "*

 * *            "{'conditions': {0: {'fn': 'booleanEquals', 'argv': {0: {'ref': 'UseDualStack'}, "*

 * *            "insert: [(1, True)], delete: [1]}}}, 'type': 'error', 'error': 'In […]*

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
@@ -29,426 +29,414 @@
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
+                                                                "supportsFIPS"
+                                                            ],
+                                                            "fn": "getAttr"
+                                                        }
+                                                    ],
+                                                    "fn": "booleanEquals"
+                                                },
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
+                                                                "url": "https://greengrass-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
+                                        }
+                                    ],
+                                    "type": "tree"
                                 },
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
+                                                            "conditions": [
+                                                                {
+                                                                    "argv": [
+                                                                        {
+                                                                            "ref": "Region"
+                                                                        },
+                                                                        "us-gov-east-1"
+                                                                    ],
+                                                                    "fn": "stringEquals"
+                                                                }
+                                                            ],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://greengrass.us-gov-east-1.amazonaws.com"
+                                                            },
+                                                            "type": "endpoint"
+                                                        },
+                                                        {
+                                                            "conditions": [
+                                                                {
+                                                                    "argv": [
+                                                                        {
+                                                                            "ref": "Region"
+                                                                        },
+                                                                        "us-gov-west-1"
+                                                                    ],
+                                                                    "fn": "stringEquals"
+                                                                }
+                                                            ],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://greengrass.us-gov-west-1.amazonaws.com"
+                                                            },
+                                                            "type": "endpoint"
+                                                        },
+                                                        {
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://greengrass-fips.{Region}.{PartitionResult#dnsSuffix}"
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
-                                                "url": "https://greengrass-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
+                                                                "url": "https://greengrass.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
                                     "rules": [
                                         {
                                             "conditions": [
                                                 {
                                                     "argv": [
                                                         {
                                                             "ref": "Region"
                                                         },
-                                                        "us-gov-east-1"
+                                                        "dataplane-us-gov-east-1"
                                                     ],
                                                     "fn": "stringEquals"
                                                 }
                                             ],
                                             "endpoint": {
                                                 "headers": {},
-                                                "properties": {},
-                                                "url": "https://greengrass.us-gov-east-1.amazonaws.com"
+                                                "properties": {
+                                                    "authSchemes": [
+                                                        {
+                                                            "name": "sigv4",
+                                                            "signingName": "greengrass",
+                                                            "signingRegion": "us-gov-east-1"
+                                                        }
+                                                    ]
+                                                },
+                                                "url": "https://greengrass-ats.iot.us-gov-east-1.amazonaws.com"
                                             },
                                             "type": "endpoint"
                                         },
                                         {
                                             "conditions": [
                                                 {
                                                     "argv": [
                                                         {
                                                             "ref": "Region"
                                                         },
-                                                        "us-gov-west-1"
+                                                        "dataplane-us-gov-west-1"
                                                     ],
                                                     "fn": "stringEquals"
                                                 }
                                             ],
                                             "endpoint": {
                                                 "headers": {},
-                                                "properties": {},
-                                                "url": "https://greengrass.us-gov-west-1.amazonaws.com"
+                                                "properties": {
+                                                    "authSchemes": [
+                                                        {
+                                                            "name": "sigv4",
+                                                            "signingName": "greengrass",
+                                                            "signingRegion": "us-gov-west-1"
+                                                        }
+                                                    ]
+                                                },
+                                                "url": "https://greengrass-ats.iot.us-gov-west-1.amazonaws.com"
                                             },
                                             "type": "endpoint"
                                         },
                                         {
                                             "conditions": [],
                                             "endpoint": {
                                                 "headers": {},
                                                 "properties": {},
-                                                "url": "https://greengrass-fips.{Region}.{PartitionResult#dnsSuffix}"
-                                            },
-                                            "type": "endpoint"
-                                        }
-                                    ],
-                                    "type": "tree"
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
-                                },
-                                true
-                            ],
-                            "fn": "booleanEquals"
-                        }
-                    ],
-                    "rules": [
-                        {
-                            "conditions": [
-                                {
-                                    "argv": [
-                                        true,
-                                        {
-                                            "argv": [
-                                                {
-                                                    "ref": "PartitionResult"
-                                                },
-                                                "supportsDualStack"
-                                            ],
-                                            "fn": "getAttr"
-                                        }
-                                    ],
-                                    "fn": "booleanEquals"
-                                }
-                            ],
-                            "rules": [
-                                {
-                                    "conditions": [],
-                                    "rules": [
-                                        {
-                                            "conditions": [],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://greengrass.{Region}.{PartitionResult#dualStackDnsSuffix}"
+                                                "url": "https://greengrass.{Region}.{PartitionResult#dnsSuffix}"
                                             },
                                             "type": "endpoint"
                                         }
                                     ],
                                     "type": "tree"
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
-                    "rules": [
-                        {
-                            "conditions": [
-                                {
-                                    "argv": [
-                                        {
-                                            "ref": "Region"
-                                        },
-                                        "dataplane-us-gov-east-1"
-                                    ],
-                                    "fn": "stringEquals"
-                                }
-                            ],
-                            "endpoint": {
-                                "headers": {},
-                                "properties": {
-                                    "authSchemes": [
-                                        {
-                                            "name": "sigv4",
-                                            "signingName": "greengrass",
-                                            "signingRegion": "us-gov-east-1"
-                                        }
-                                    ]
-                                },
-                                "url": "https://greengrass-ats.iot.us-gov-east-1.amazonaws.com"
-                            },
-                            "type": "endpoint"
-                        },
-                        {
-                            "conditions": [
-                                {
-                                    "argv": [
-                                        {
-                                            "ref": "Region"
-                                        },
-                                        "dataplane-us-gov-west-1"
-                                    ],
-                                    "fn": "stringEquals"
-                                }
-                            ],
-                            "endpoint": {
-                                "headers": {},
-                                "properties": {
-                                    "authSchemes": [
-                                        {
-                                            "name": "sigv4",
-                                            "signingName": "greengrass",
-                                            "signingRegion": "us-gov-west-1"
-                                        }
-                                    ]
-                                },
-                                "url": "https://greengrass-ats.iot.us-gov-west-1.amazonaws.com"
-                            },
-                            "type": "endpoint"
-                        },
-                        {
-                            "conditions": [
-                                {
-                                    "argv": [
-                                        {
-                                            "ref": "Region"
-                                        },
-                                        "us-gov-east-1"
-                                    ],
-                                    "fn": "stringEquals"
-                                }
-                            ],
-                            "endpoint": {
-                                "headers": {},
-                                "properties": {},
-                                "url": "https://greengrass.us-gov-east-1.amazonaws.com"
-                            },
-                            "type": "endpoint"
-                        },
-                        {
-                            "conditions": [
-                                {
-                                    "argv": [
-                                        {
-                                            "ref": "Region"
-                                        },
-                                        "us-gov-west-1"
-                                    ],
-                                    "fn": "stringEquals"
-                                }
-                            ],
-                            "endpoint": {
-                                "headers": {},
-                                "properties": {},
-                                "url": "https://greengrass.us-gov-west-1.amazonaws.com"
-                            },
-                            "type": "endpoint"
-                        },
-                        {
-                            "conditions": [],
-                            "endpoint": {
-                                "headers": {},
-                                "properties": {},
-                                "url": "https://greengrass.{Region}.{PartitionResult#dnsSuffix}"
-                            },
-                            "type": "endpoint"
-                        }
-                    ],
-                    "type": "tree"
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

### Comparing `botocore-a-la-carte-greengrassv2-1.29.99/botocore/data/greengrassv2/2020-11-30/paginators-1.json` & `botocore-a-la-carte-greengrassv2-1.30.0/botocore/data/greengrassv2/2020-11-30/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-greengrassv2-1.29.99/botocore/data/greengrassv2/2020-11-30/service-2.json` & `botocore-a-la-carte-greengrassv2-1.30.0/botocore/data/greengrassv2/2020-11-30/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999912028103359%*

 * *Differences: {"'shapes'": "{'EffectiveDeployment': {'members': {'coreDeviceExecutionStatus': {'documentation': "*

 * *             '"<p>The status of the deployment job on the Greengrass core device.</p> <ul> <li> '*

 * *             '<p> <code>IN_PROGRESS</code> – The deployment job is running.</p> </li> <li> <p> '*

 * *             '<code>QUEUED</code> – The deployment job is in the job queue and waiting to run.</p> '*

 * *             '</li> <li> <p> <code>FAILED</code> – The deployment failed. For more information, '*

 * *             'see  […]*

```diff
@@ -1886,15 +1886,15 @@
             },
             "type": "structure"
         },
         "EffectiveDeployment": {
             "documentation": "<p>Contains information about a deployment job that IoT Greengrass sends to a Greengrass core device.</p>",
             "members": {
                 "coreDeviceExecutionStatus": {
-                    "documentation": "<p>The status of the deployment job on the Greengrass core device.</p>",
+                    "documentation": "<p>The status of the deployment job on the Greengrass core device.</p> <ul> <li> <p> <code>IN_PROGRESS</code> \u2013 The deployment job is running.</p> </li> <li> <p> <code>QUEUED</code> \u2013 The deployment job is in the job queue and waiting to run.</p> </li> <li> <p> <code>FAILED</code> \u2013 The deployment failed. For more information, see the <code>statusDetails</code> field.</p> </li> <li> <p> <code>COMPLETED</code> \u2013 The deployment to an IoT thing was completed successfully.</p> </li> <li> <p> <code>TIMED_OUT</code> \u2013 The deployment didn't complete in the allotted time. </p> </li> <li> <p> <code>CANCELED</code> \u2013 The deployment was canceled by the user.</p> </li> <li> <p> <code>REJECTED</code> \u2013 The deployment was rejected. For more information, see the <code>statusDetails</code> field.</p> </li> <li> <p> <code>SUCCEEDED</code> \u2013 The deployment to an IoT thing group was completed successfully.</p> </li> </ul>",
                     "shape": "EffectiveDeploymentExecutionStatus"
                 },
                 "creationTimestamp": {
                     "documentation": "<p>The time at which the deployment was created, expressed in ISO 8601 format.</p>",
                     "shape": "Timestamp"
                 },
                 "deploymentId": {
@@ -1970,15 +1970,16 @@
             "enum": [
                 "IN_PROGRESS",
                 "QUEUED",
                 "FAILED",
                 "COMPLETED",
                 "TIMED_OUT",
                 "CANCELED",
-                "REJECTED"
+                "REJECTED",
+                "SUCCEEDED"
             ],
             "type": "string"
         },
         "EffectiveDeploymentStatusDetails": {
             "documentation": "<p>Contains all error-related information for the deployment record. The status details will be null if the deployment is in a success state.</p> <note> <p>Greengrass nucleus v2.8.0 or later is required to get an accurate <code>errorStack</code> and <code>errorTypes</code> response. This field will not be returned for earlier Greengrass nucleus versions.</p> </note>",
             "members": {
                 "errorStack": {
@@ -2266,19 +2267,19 @@
                     "shape": "ComponentVersionString"
                 },
                 "isRoot": {
                     "documentation": "<p>Whether or not the component is a root component.</p>",
                     "shape": "IsRoot"
                 },
                 "lastInstallationSource": {
-                    "documentation": "<p>The most recent deployment source that brought the component to the Greengrass core device. For a thing group deployment or thing deployment, the source will be the The ID of the deployment. and for local deployments it will be <code>LOCAL</code>.</p>",
+                    "documentation": "<p>The most recent deployment source that brought the component to the Greengrass core device. For a thing group deployment or thing deployment, the source will be the The ID of the deployment. and for local deployments it will be <code>LOCAL</code>.</p> <note> <p>Any deployment will attempt to reinstall currently broken components on the device, which will update the last installation source.</p> </note>",
                     "shape": "NonEmptyString"
                 },
                 "lastReportedTimestamp": {
-                    "documentation": "<p>The last time the Greengrass core device sent a message containing a certain component to the Amazon Web Services Cloud.</p> <p>A component does not need to see a state change for this field to update.</p>",
+                    "documentation": "<p>The last time the Greengrass core device sent a message containing a component's state to the Amazon Web Services Cloud.</p> <p>A component does not need to see a state change for this field to update.</p>",
                     "shape": "Timestamp"
                 },
                 "lastStatusChangeTimestamp": {
                     "documentation": "<p>The status of how current the data is.</p> <p>This response is based off of component state changes. The status reflects component disruptions and deployments. If a component only sees a configuration update during a deployment, it might not undergo a state change and this status would not be updated.</p>",
                     "shape": "Timestamp"
                 },
                 "lifecycleState": {
```

### Comparing `botocore-a-la-carte-greengrassv2-1.29.99/botocore_a_la_carte_greengrassv2.egg-info/PKG-INFO` & `botocore-a-la-carte-greengrassv2-1.30.0/botocore_a_la_carte_greengrassv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-greengrassv2
-Version: 1.29.99
+Version: 1.30.0
 Summary: greengrassv2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-greengrassv2-1.29.99/setup.py` & `botocore-a-la-carte-greengrassv2-1.30.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-greengrassv2',
-    version="1.29.99",
+    version="1.30.0",
     description='greengrassv2 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/greengrassv2/*/*.json'],
```

