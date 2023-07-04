# Comparing `tmp/botocore-a-la-carte-fsx-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-fsx-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-fsx-1.29.99.tar", last modified: Sat Mar 25 01:22:48 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-fsx-1.30.0.tar", last modified: Tue Jul  4 01:44:38 2023, max compression
```

## Comparing `botocore-a-la-carte-fsx-1.29.99.tar` & `botocore-a-la-carte-fsx-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:48.063893 botocore-a-la-carte-fsx-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:47.000000 botocore-a-la-carte-fsx-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-25 01:22:48.063893 botocore-a-la-carte-fsx-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:48.059893 botocore-a-la-carte-fsx-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:48.059893 botocore-a-la-carte-fsx-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:48.059893 botocore-a-la-carte-fsx-1.29.99/botocore/data/fsx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:48.063893 botocore-a-la-carte-fsx-1.29.99/botocore/data/fsx/2018-03-01/
--rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-03-25 01:22:12.000000 botocore-a-la-carte-fsx-1.29.99/botocore/data/fsx/2018-03-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    14242 2023-03-25 01:22:12.000000 botocore-a-la-carte-fsx-1.29.99/botocore/data/fsx/2018-03-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-25 01:22:12.000000 botocore-a-la-carte-fsx-1.29.99/botocore/data/fsx/2018-03-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   363491 2023-03-25 01:22:12.000000 botocore-a-la-carte-fsx-1.29.99/botocore/data/fsx/2018-03-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:48.063893 botocore-a-la-carte-fsx-1.29.99/botocore_a_la_carte_fsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-25 01:22:48.000000 botocore-a-la-carte-fsx-1.29.99/botocore_a_la_carte_fsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-25 01:22:48.000000 botocore-a-la-carte-fsx-1.29.99/botocore_a_la_carte_fsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:48.000000 botocore-a-la-carte-fsx-1.29.99/botocore_a_la_carte_fsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:48.000000 botocore-a-la-carte-fsx-1.29.99/botocore_a_la_carte_fsx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:48.063893 botocore-a-la-carte-fsx-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-25 01:22:47.000000 botocore-a-la-carte-fsx-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:38.950635 botocore-a-la-carte-fsx-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:38.000000 botocore-a-la-carte-fsx-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:44:38.950635 botocore-a-la-carte-fsx-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:38.946635 botocore-a-la-carte-fsx-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:38.946635 botocore-a-la-carte-fsx-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:38.946635 botocore-a-la-carte-fsx-1.30.0/botocore/data/fsx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:38.950635 botocore-a-la-carte-fsx-1.30.0/botocore/data/fsx/2018-03-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-04 01:44:02.000000 botocore-a-la-carte-fsx-1.30.0/botocore/data/fsx/2018-03-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14242 2023-07-04 01:44:02.000000 botocore-a-la-carte-fsx-1.30.0/botocore/data/fsx/2018-03-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-04 01:44:02.000000 botocore-a-la-carte-fsx-1.30.0/botocore/data/fsx/2018-03-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   365813 2023-07-04 01:44:02.000000 botocore-a-la-carte-fsx-1.30.0/botocore/data/fsx/2018-03-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:38.950635 botocore-a-la-carte-fsx-1.30.0/botocore_a_la_carte_fsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:44:38.000000 botocore-a-la-carte-fsx-1.30.0/botocore_a_la_carte_fsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-04 01:44:38.000000 botocore-a-la-carte-fsx-1.30.0/botocore_a_la_carte_fsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:38.000000 botocore-a-la-carte-fsx-1.30.0/botocore_a_la_carte_fsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:38.000000 botocore-a-la-carte-fsx-1.30.0/botocore_a_la_carte_fsx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:38.950635 botocore-a-la-carte-fsx-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-04 01:44:38.000000 botocore-a-la-carte-fsx-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-fsx-1.29.99/LICENSE.txt` & `botocore-a-la-carte-fsx-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-fsx-1.29.99/PKG-INFO` & `botocore-a-la-carte-fsx-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-fsx
-Version: 1.29.99
+Version: 1.30.0
 Summary: fsx data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-fsx-1.29.99/botocore/data/fsx/2018-03-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-fsx-1.30.0/botocore/data/fsx/2018-03-01/endpoint-rule-set-1.json`

 * *Files 17% similar despite different names*

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
@@ -29,411 +29,322 @@
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
                                         {
-                                            "argv": [
-                                                {
-                                                    "ref": "PartitionResult"
-                                                },
-                                                "supportsFIPS"
-                                            ],
-                                            "fn": "getAttr"
+                                            "ref": "Region"
                                         }
                                     ],
-                                    "fn": "booleanEquals"
-                                },
+                                    "assign": "PartitionResult",
+                                    "fn": "aws.partition"
+                                }
+                            ],
+                            "rules": [
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
-                                        }
-                                    ],
-                                    "fn": "booleanEquals"
-                                }
-                            ],
-                            "rules": [
-                                {
-                                    "conditions": [],
-                                    "endpoint": {
-                                        "headers": {},
-                                        "properties": {},
-                                        "url": "https://fsx-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                }
-                            ],
-                            "rules": [
-                                {
-                                    "conditions": [],
                                     "rules": [
                                         {
                                             "conditions": [
                                                 {
                                                     "argv": [
+                                                        true,
                                                         {
-                                                            "ref": "Region"
-                                                        },
-                                                        "prod-ca-central-1"
+                                                            "argv": [
+                                                                {
+                                                                    "ref": "PartitionResult"
+                                                                },
+                                                                "supportsFIPS"
+                                                            ],
+                                                            "fn": "getAttr"
+                                                        }
                                                     ],
-                                                    "fn": "stringEquals"
-                                                }
-                                            ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://fsx-fips.ca-central-1.amazonaws.com"
-                                            },
-                                            "type": "endpoint"
-                                        },
-                                        {
-                                            "conditions": [
+                                                    "fn": "booleanEquals"
+                                                },
                                                 {
                                                     "argv": [
+                                                        true,
                                                         {
-                                                            "ref": "Region"
-                                                        },
-                                                        "prod-us-east-1"
+                                                            "argv": [
+                                                                {
+                                                                    "ref": "PartitionResult"
+                                                                },
+                                                                "supportsDualStack"
+                                                            ],
+                                                            "fn": "getAttr"
+                                                        }
                                                     ],
-                                                    "fn": "stringEquals"
+                                                    "fn": "booleanEquals"
                                                 }
                                             ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://fsx-fips.us-east-1.amazonaws.com"
-                                            },
-                                            "type": "endpoint"
-                                        },
-                                        {
-                                            "conditions": [
+                                            "rules": [
                                                 {
-                                                    "argv": [
+                                                    "conditions": [],
+                                                    "rules": [
                                                         {
-                                                            "ref": "Region"
-                                                        },
-                                                        "prod-us-east-2"
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://fsx-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
+                                                            },
+                                                            "type": "endpoint"
+                                                        }
                                                     ],
-                                                    "fn": "stringEquals"
+                                                    "type": "tree"
                                                 }
                                             ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://fsx-fips.us-east-2.amazonaws.com"
-                                            },
-                                            "type": "endpoint"
+                                            "type": "tree"
                                         },
                                         {
+                                            "conditions": [],
+                                            "error": "FIPS and DualStack are enabled, but this partition does not support one or both",
+                                            "type": "error"
+                                        }
+                                    ],
+                                    "type": "tree"
+                                },
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
+                                        }
+                                    ],
+                                    "rules": [
+                                        {
                                             "conditions": [
                                                 {
                                                     "argv": [
+                                                        true,
                                                         {
-                                                            "ref": "Region"
-                                                        },
-                                                        "prod-us-west-1"
+                                                            "argv": [
+                                                                {
+                                                                    "ref": "PartitionResult"
+                                                                },
+                                                                "supportsFIPS"
+                                                            ],
+                                                            "fn": "getAttr"
+                                                        }
                                                     ],
-                                                    "fn": "stringEquals"
+                                                    "fn": "booleanEquals"
                                                 }
                                             ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://fsx-fips.us-west-1.amazonaws.com"
-                                            },
-                                            "type": "endpoint"
-                                        },
-                                        {
-                                            "conditions": [
+                                            "rules": [
                                                 {
-                                                    "argv": [
+                                                    "conditions": [],
+                                                    "rules": [
                                                         {
-                                                            "ref": "Region"
-                                                        },
-                                                        "prod-us-west-2"
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://fsx-fips.{Region}.{PartitionResult#dnsSuffix}"
+                                                            },
+                                                            "type": "endpoint"
+                                                        }
                                                     ],
-                                                    "fn": "stringEquals"
+                                                    "type": "tree"
                                                 }
                                             ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://fsx-fips.us-west-2.amazonaws.com"
-                                            },
-                                            "type": "endpoint"
+                                            "type": "tree"
                                         },
                                         {
+                                            "conditions": [],
+                                            "error": "FIPS is enabled but this partition does not support FIPS",
+                                            "type": "error"
+                                        }
+                                    ],
+                                    "type": "tree"
+                                },
+                                {
+                                    "conditions": [
+                                        {
+                                            "argv": [
+                                                {
+                                                    "ref": "UseDualStack"
+                                                },
+                                                true
+                                            ],
+                                            "fn": "booleanEquals"
+                                        }
+                                    ],
+                                    "rules": [
+                                        {
                                             "conditions": [
                                                 {
                                                     "argv": [
+                                                        true,
                                                         {
-                                                            "ref": "Region"
-                                                        },
-                                                        "prod-us-gov-east-1"
+                                                            "argv": [
+                                                                {
+                                                                    "ref": "PartitionResult"
+                                                                },
+                                                                "supportsDualStack"
+                                                            ],
+                                                            "fn": "getAttr"
+                                                        }
                                                     ],
-                                                    "fn": "stringEquals"
+                                                    "fn": "booleanEquals"
                                                 }
                                             ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://fsx-fips.us-gov-east-1.amazonaws.com"
-                                            },
-                                            "type": "endpoint"
-                                        },
-                                        {
-                                            "conditions": [
+                                            "rules": [
                                                 {
-                                                    "argv": [
+                                                    "conditions": [],
+                                                    "rules": [
                                                         {
-                                                            "ref": "Region"
-                                                        },
-                                                        "prod-us-gov-west-1"
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://fsx.{Region}.{PartitionResult#dualStackDnsSuffix}"
+                                                            },
+                                                            "type": "endpoint"
+                                                        }
                                                     ],
-                                                    "fn": "stringEquals"
+                                                    "type": "tree"
                                                 }
                                             ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://fsx-fips.us-gov-west-1.amazonaws.com"
-                                            },
-                                            "type": "endpoint"
+                                            "type": "tree"
                                         },
                                         {
                                             "conditions": [],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://fsx-fips.{Region}.{PartitionResult#dnsSuffix}"
-                                            },
-                                            "type": "endpoint"
+                                            "error": "DualStack is enabled but this partition does not support DualStack",
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
+                                    "conditions": [],
+                                    "rules": [
                                         {
-                                            "argv": [
-                                                {
-                                                    "ref": "PartitionResult"
-                                                },
-                                                "supportsDualStack"
-                                            ],
-                                            "fn": "getAttr"
+                                            "conditions": [],
+                                            "endpoint": {
+                                                "headers": {},
+                                                "properties": {},
+                                                "url": "https://fsx.{Region}.{PartitionResult#dnsSuffix}"
+                                            },
+                                            "type": "endpoint"
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
-                                        "url": "https://fsx.{Region}.{PartitionResult#dualStackDnsSuffix}"
-                                    },
-                                    "type": "endpoint"
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
-                        "url": "https://fsx.{Region}.{PartitionResult#dnsSuffix}"
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

### Comparing `botocore-a-la-carte-fsx-1.29.99/botocore/data/fsx/2018-03-01/examples-1.json` & `botocore-a-la-carte-fsx-1.30.0/botocore/data/fsx/2018-03-01/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-fsx-1.29.99/botocore/data/fsx/2018-03-01/paginators-1.json` & `botocore-a-la-carte-fsx-1.30.0/botocore/data/fsx/2018-03-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-fsx-1.29.99/botocore/data/fsx/2018-03-01/service-2.json` & `botocore-a-la-carte-fsx-1.30.0/botocore/data/fsx/2018-03-01/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990954998161243%*

 * *Differences: {"'operations'": "{'CreateDataRepositoryAssociation': {'documentation': '<p>Creates an Amazon FSx "*

 * *                 'for Lustre data repository association (DRA). A data repository association is a '*

 * *                 'link between a directory on the file system and an Amazon S3 bucket or prefix. '*

 * *                 'You can have a maximum of 8 data repository associations on a file system. Data '*

 * *                 'repository associations are supported on all FSx for Lustre 2.12 and newer file '*

 * *             […]*

```diff
@@ -158,15 +158,15 @@
             },
             "name": "CreateBackup",
             "output": {
                 "shape": "CreateBackupResponse"
             }
         },
         "CreateDataRepositoryAssociation": {
-            "documentation": "<p>Creates an Amazon FSx for Lustre data repository association (DRA). A data repository association is a link between a directory on the file system and an Amazon S3 bucket or prefix. You can have a maximum of 8 data repository associations on a file system. Data repository associations are supported only for file systems with the <code>Persistent_2</code> deployment type.</p> <p>Each data repository association must have a unique Amazon FSx file system directory and a unique S3 bucket or prefix associated with it. You can configure a data repository association for automatic import only, for automatic export only, or for both. To learn more about linking a data repository to your file system, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/create-dra-linked-data-repo.html\">Linking your file system to an S3 bucket</a>.</p> <note> <p> <code>CreateDataRepositoryAssociation</code> isn't supported on Amazon File Cache resources. To create a DRA on Amazon File Cache, use the <code>CreateFileCache</code> operation.</p> </note>",
+            "documentation": "<p>Creates an Amazon FSx for Lustre data repository association (DRA). A data repository association is a link between a directory on the file system and an Amazon S3 bucket or prefix. You can have a maximum of 8 data repository associations on a file system. Data repository associations are supported on all FSx for Lustre 2.12 and newer file systems, excluding <code>scratch_1</code> deployment type.</p> <p>Each data repository association must have a unique Amazon FSx file system directory and a unique S3 bucket or prefix associated with it. You can configure a data repository association for automatic import only, for automatic export only, or for both. To learn more about linking a data repository to your file system, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/create-dra-linked-data-repo.html\">Linking your file system to an S3 bucket</a>.</p> <note> <p> <code>CreateDataRepositoryAssociation</code> isn't supported on Amazon File Cache resources. To create a DRA on Amazon File Cache, use the <code>CreateFileCache</code> operation.</p> </note>",
             "errors": [
                 {
                     "shape": "BadRequest"
                 },
                 {
                     "shape": "UnsupportedOperation"
                 },
@@ -542,15 +542,15 @@
             },
             "name": "DeleteBackup",
             "output": {
                 "shape": "DeleteBackupResponse"
             }
         },
         "DeleteDataRepositoryAssociation": {
-            "documentation": "<p>Deletes a data repository association on an Amazon FSx for Lustre file system. Deleting the data repository association unlinks the file system from the Amazon S3 bucket. When deleting a data repository association, you have the option of deleting the data in the file system that corresponds to the data repository association. Data repository associations are supported only for file systems with the <code>Persistent_2</code> deployment type.</p>",
+            "documentation": "<p>Deletes a data repository association on an Amazon FSx for Lustre file system. Deleting the data repository association unlinks the file system from the Amazon S3 bucket. When deleting a data repository association, you have the option of deleting the data in the file system that corresponds to the data repository association. Data repository associations are supported on all FSx for Lustre 2.12 and newer file systems, excluding <code>scratch_1</code> deployment type.</p>",
             "errors": [
                 {
                     "shape": "BadRequest"
                 },
                 {
                     "shape": "IncompatibleParameterError"
                 },
@@ -705,14 +705,17 @@
                     "shape": "IncompatibleParameterError"
                 },
                 {
                     "shape": "InternalServerError"
                 },
                 {
                     "shape": "VolumeNotFound"
+                },
+                {
+                    "shape": "ServiceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -751,15 +754,15 @@
             },
             "name": "DescribeBackups",
             "output": {
                 "shape": "DescribeBackupsResponse"
             }
         },
         "DescribeDataRepositoryAssociations": {
-            "documentation": "<p>Returns the description of specific Amazon FSx for Lustre or Amazon File Cache data repository associations, if one or more <code>AssociationIds</code> values are provided in the request, or if filters are used in the request. Data repository associations are supported only for Amazon FSx for Lustre file systems with the <code>Persistent_2</code> deployment type and for Amazon File Cache resources.</p> <p>You can use filters to narrow the response to include just data repository associations for specific file systems (use the <code>file-system-id</code> filter with the ID of the file system) or caches (use the <code>file-cache-id</code> filter with the ID of the cache), or data repository associations for a specific repository type (use the <code>data-repository-type</code> filter with a value of <code>S3</code> or <code>NFS</code>). If you don't use filters, the response returns all data repository associations owned by your Amazon Web Services account in the Amazon Web Services Region of the endpoint that you're calling.</p> <p>When retrieving all data repository associations, you can paginate the response by using the optional <code>MaxResults</code> parameter to limit the number of data repository associations returned in a response. If more data repository associations remain, a <code>NextToken</code> value is returned in the response. In this case, send a later request with the <code>NextToken</code> request parameter set to the value of <code>NextToken</code> from the last response.</p>",
+            "documentation": "<p>Returns the description of specific Amazon FSx for Lustre or Amazon File Cache data repository associations, if one or more <code>AssociationIds</code> values are provided in the request, or if filters are used in the request. Data repository associations are supported on Amazon File Cache resources and all FSx for Lustre 2.12 and newer file systems, excluding <code>scratch_1</code> deployment type.</p> <p>You can use filters to narrow the response to include just data repository associations for specific file systems (use the <code>file-system-id</code> filter with the ID of the file system) or caches (use the <code>file-cache-id</code> filter with the ID of the cache), or data repository associations for a specific repository type (use the <code>data-repository-type</code> filter with a value of <code>S3</code> or <code>NFS</code>). If you don't use filters, the response returns all data repository associations owned by your Amazon Web Services account in the Amazon Web Services Region of the endpoint that you're calling.</p> <p>When retrieving all data repository associations, you can paginate the response by using the optional <code>MaxResults</code> parameter to limit the number of data repository associations returned in a response. If more data repository associations remain, a <code>NextToken</code> value is returned in the response. In this case, send a later request with the <code>NextToken</code> request parameter set to the value of <code>NextToken</code> from the last response.</p>",
             "errors": [
                 {
                     "shape": "BadRequest"
                 },
                 {
                     "shape": "FileSystemNotFound"
                 },
@@ -1140,15 +1143,15 @@
             },
             "name": "UntagResource",
             "output": {
                 "shape": "UntagResourceResponse"
             }
         },
         "UpdateDataRepositoryAssociation": {
-            "documentation": "<p>Updates the configuration of an existing data repository association on an Amazon FSx for Lustre file system. Data repository associations are supported only for file systems with the <code>Persistent_2</code> deployment type.</p>",
+            "documentation": "<p>Updates the configuration of an existing data repository association on an Amazon FSx for Lustre file system. Data repository associations are supported on all FSx for Lustre 2.12 and newer file systems, excluding <code>scratch_1</code> deployment type.</p>",
             "errors": [
                 {
                     "shape": "BadRequest"
                 },
                 {
                     "shape": "IncompatibleParameterError"
                 },
@@ -1210,15 +1213,15 @@
             },
             "name": "UpdateFileCache",
             "output": {
                 "shape": "UpdateFileCacheResponse"
             }
         },
         "UpdateFileSystem": {
-            "documentation": "<p>Use this operation to update the configuration of an existing Amazon FSx file system. You can update multiple properties in a single request.</p> <p>For Amazon FSx for Windows File Server file systems, you can update the following properties:</p> <ul> <li> <p> <code>AuditLogConfiguration</code> </p> </li> <li> <p> <code>AutomaticBackupRetentionDays</code> </p> </li> <li> <p> <code>DailyAutomaticBackupStartTime</code> </p> </li> <li> <p> <code>SelfManagedActiveDirectoryConfiguration</code> </p> </li> <li> <p> <code>StorageCapacity</code> </p> </li> <li> <p> <code>ThroughputCapacity</code> </p> </li> <li> <p> <code>WeeklyMaintenanceStartTime</code> </p> </li> </ul> <p>For Amazon FSx for Lustre file systems, you can update the following properties:</p> <ul> <li> <p> <code>AutoImportPolicy</code> </p> </li> <li> <p> <code>AutomaticBackupRetentionDays</code> </p> </li> <li> <p> <code>DailyAutomaticBackupStartTime</code> </p> </li> <li> <p> <code>DataCompressionType</code> </p> </li> <li> <p> <code>LustreRootSquashConfiguration</code> </p> </li> <li> <p> <code>StorageCapacity</code> </p> </li> <li> <p> <code>WeeklyMaintenanceStartTime</code> </p> </li> </ul> <p>For Amazon FSx for NetApp ONTAP file systems, you can update the following properties:</p> <ul> <li> <p> <code>AutomaticBackupRetentionDays</code> </p> </li> <li> <p> <code>DailyAutomaticBackupStartTime</code> </p> </li> <li> <p> <code>DiskIopsConfiguration</code> </p> </li> <li> <p> <code>FsxAdminPassword</code> </p> </li> <li> <p> <code>StorageCapacity</code> </p> </li> <li> <p> <code>ThroughputCapacity</code> </p> </li> <li> <p> <code>WeeklyMaintenanceStartTime</code> </p> </li> </ul> <p>For the Amazon FSx for OpenZFS file systems, you can update the following properties:</p> <ul> <li> <p> <code>AutomaticBackupRetentionDays</code> </p> </li> <li> <p> <code>CopyTagsToBackups</code> </p> </li> <li> <p> <code>CopyTagsToVolumes</code> </p> </li> <li> <p> <code>DailyAutomaticBackupStartTime</code> </p> </li> <li> <p> <code>ThroughputCapacity</code> </p> </li> <li> <p> <code>WeeklyMaintenanceStartTime</code> </p> </li> </ul>",
+            "documentation": "<p>Use this operation to update the configuration of an existing Amazon FSx file system. You can update multiple properties in a single request.</p> <p>For FSx for Windows File Server file systems, you can update the following properties:</p> <ul> <li> <p> <code>AuditLogConfiguration</code> </p> </li> <li> <p> <code>AutomaticBackupRetentionDays</code> </p> </li> <li> <p> <code>DailyAutomaticBackupStartTime</code> </p> </li> <li> <p> <code>SelfManagedActiveDirectoryConfiguration</code> </p> </li> <li> <p> <code>StorageCapacity</code> </p> </li> <li> <p> <code>ThroughputCapacity</code> </p> </li> <li> <p> <code>WeeklyMaintenanceStartTime</code> </p> </li> </ul> <p>For FSx for Lustre file systems, you can update the following properties:</p> <ul> <li> <p> <code>AutoImportPolicy</code> </p> </li> <li> <p> <code>AutomaticBackupRetentionDays</code> </p> </li> <li> <p> <code>DailyAutomaticBackupStartTime</code> </p> </li> <li> <p> <code>DataCompressionType</code> </p> </li> <li> <p> <code>LustreRootSquashConfiguration</code> </p> </li> <li> <p> <code>StorageCapacity</code> </p> </li> <li> <p> <code>WeeklyMaintenanceStartTime</code> </p> </li> </ul> <p>For FSx for ONTAP file systems, you can update the following properties:</p> <ul> <li> <p> <code>AddRouteTableIds</code> </p> </li> <li> <p> <code>AutomaticBackupRetentionDays</code> </p> </li> <li> <p> <code>DailyAutomaticBackupStartTime</code> </p> </li> <li> <p> <code>DiskIopsConfiguration</code> </p> </li> <li> <p> <code>FsxAdminPassword</code> </p> </li> <li> <p> <code>RemoveRouteTableIds</code> </p> </li> <li> <p> <code>StorageCapacity</code> </p> </li> <li> <p> <code>ThroughputCapacity</code> </p> </li> <li> <p> <code>WeeklyMaintenanceStartTime</code> </p> </li> </ul> <p>For FSx for OpenZFS file systems, you can update the following properties:</p> <ul> <li> <p> <code>AutomaticBackupRetentionDays</code> </p> </li> <li> <p> <code>CopyTagsToBackups</code> </p> </li> <li> <p> <code>CopyTagsToVolumes</code> </p> </li> <li> <p> <code>DailyAutomaticBackupStartTime</code> </p> </li> <li> <p> <code>DiskIopsConfiguration</code> </p> </li> <li> <p> <code>StorageCapacity</code> </p> </li> <li> <p> <code>ThroughputCapacity</code> </p> </li> <li> <p> <code>WeeklyMaintenanceStartTime</code> </p> </li> </ul>",
             "errors": [
                 {
                     "shape": "BadRequest"
                 },
                 {
                     "shape": "UnsupportedOperation"
                 },
@@ -1276,15 +1279,15 @@
             },
             "name": "UpdateSnapshot",
             "output": {
                 "shape": "UpdateSnapshotResponse"
             }
         },
         "UpdateStorageVirtualMachine": {
-            "documentation": "<p>Updates an Amazon FSx for ONTAP storage virtual machine (SVM).</p>",
+            "documentation": "<p>Updates an FSx for ONTAP storage virtual machine (SVM).</p>",
             "errors": [
                 {
                     "shape": "BadRequest"
                 },
                 {
                     "shape": "IncompatibleParameterError"
                 },
@@ -1556,25 +1559,25 @@
                     "documentation": "<p>An array of the DNS aliases that Amazon FSx is associating with the file system.</p>",
                     "shape": "Aliases"
                 }
             },
             "type": "structure"
         },
         "AutoExportPolicy": {
-            "documentation": "<p>Describes a data repository association's automatic export policy. The <code>AutoExportPolicy</code> defines the types of updated objects on the file system that will be automatically exported to the data repository. As you create, modify, or delete files, Amazon FSx for Lustre automatically exports the defined changes asynchronously once your application finishes modifying the file.</p> <p>This <code>AutoExportPolicy</code> is supported only for Amazon FSx for Lustre file systems with the <code>Persistent_2</code> deployment type.</p>",
+            "documentation": "<p>Describes a data repository association's automatic export policy. The <code>AutoExportPolicy</code> defines the types of updated objects on the file system that will be automatically exported to the data repository. As you create, modify, or delete files, Amazon FSx for Lustre automatically exports the defined changes asynchronously once your application finishes modifying the file.</p> <p>The <code>AutoExportPolicy</code> is only supported on Amazon FSx for Lustre file systems with a data repository association.</p>",
             "members": {
                 "Events": {
                     "documentation": "<p>The <code>AutoExportPolicy</code> can have the following event values:</p> <ul> <li> <p> <code>NEW</code> - New files and directories are automatically exported to the data repository as they are added to the file system.</p> </li> <li> <p> <code>CHANGED</code> - Changes to files and directories on the file system are automatically exported to the data repository.</p> </li> <li> <p> <code>DELETED</code> - Files and directories are automatically deleted on the data repository when they are deleted on the file system.</p> </li> </ul> <p>You can define any combination of event types for your <code>AutoExportPolicy</code>.</p>",
                     "shape": "EventTypes"
                 }
             },
             "type": "structure"
         },
         "AutoImportPolicy": {
-            "documentation": "<p>Describes the data repository association's automatic import policy. The AutoImportPolicy defines how Amazon FSx keeps your file metadata and directory listings up to date by importing changes to your Amazon FSx for Lustre file system as you modify objects in a linked S3 bucket.</p> <p>The <code>AutoImportPolicy</code> is supported only for Amazon FSx for Lustre file systems with the <code>Persistent_2</code> deployment type.</p>",
+            "documentation": "<p>Describes the data repository association's automatic import policy. The AutoImportPolicy defines how Amazon FSx keeps your file metadata and directory listings up to date by importing changes to your Amazon FSx for Lustre file system as you modify objects in a linked S3 bucket.</p> <p>The <code>AutoImportPolicy</code> is only supported on Amazon FSx for Lustre file systems with a data repository association.</p>",
             "members": {
                 "Events": {
                     "documentation": "<p>The <code>AutoImportPolicy</code> can have the following event values:</p> <ul> <li> <p> <code>NEW</code> - Amazon FSx automatically imports metadata of files added to the linked S3 bucket that do not currently exist in the FSx file system.</p> </li> <li> <p> <code>CHANGED</code> - Amazon FSx automatically updates file metadata and invalidates existing file content on the file system as files change in the data repository.</p> </li> <li> <p> <code>DELETED</code> - Amazon FSx automatically deletes files on the file system as corresponding files are deleted in the data repository.</p> </li> </ul> <p>You can define any combination of event types for your <code>AutoImportPolicy</code>.</p>",
                     "shape": "EventTypes"
                 }
             },
             "type": "structure"
@@ -1585,15 +1588,15 @@
                 "NEW",
                 "NEW_CHANGED",
                 "NEW_CHANGED_DELETED"
             ],
             "type": "string"
         },
         "AutomaticBackupRetentionDays": {
-            "documentation": "<p>The number of days to retain automatic backups. Setting this property to <code>0</code> disables automatic backups. You can retain automatic backups for a maximum of 90 days. The default is <code>0</code>.</p>",
+            "documentation": "<p>The number of days to retain automatic backups. Setting this property to <code>0</code> disables automatic backups. You can retain automatic backups for a maximum of 90 days. The default is <code>30</code>.</p>",
             "max": 90,
             "min": 0,
             "type": "integer"
         },
         "Backup": {
             "documentation": "<p>A backup of an Amazon FSx for Windows File Server, Amazon FSx for Lustre file system, Amazon FSx for NetApp ONTAP volume, or Amazon FSx for OpenZFS file system.</p>",
             "members": {
@@ -1810,15 +1813,15 @@
         },
         "CapacityToRelease": {
             "max": 2147483647,
             "min": 1,
             "type": "long"
         },
         "ClientRequestToken": {
-            "documentation": "<p>(Optional) An idempotency token for resource creation, in a string of up to 64 ASCII characters. This token is automatically filled on your behalf when you use the Command Line Interface (CLI) or an Amazon Web Services SDK.</p>",
+            "documentation": "<p>(Optional) An idempotency token for resource creation, in a string of up to 63 ASCII characters. This token is automatically filled on your behalf when you use the Command Line Interface (CLI) or an Amazon Web Services SDK.</p>",
             "max": 63,
             "min": 1,
             "pattern": "[A-za-z0-9_.-]{0,63}$",
             "type": "string"
         },
         "CompletionReport": {
             "documentation": "<p>Provides a report detailing the data repository task results of the files processed that match the criteria specified in the report <code>Scope</code> parameter. FSx delivers the report to the file system's linked data repository in Amazon S3, using the path specified in the report <code>Path</code> parameter. You can specify whether or not a report gets generated for a task using the <code>Enabled</code> parameter.</p>",
@@ -1828,15 +1831,15 @@
                     "shape": "Flag"
                 },
                 "Format": {
                     "documentation": "<p>Required if <code>Enabled</code> is set to <code>true</code>. Specifies the format of the <code>CompletionReport</code>. <code>REPORT_CSV_20191124</code> is the only format currently supported. When <code>Format</code> is set to <code>REPORT_CSV_20191124</code>, the <code>CompletionReport</code> is provided in CSV format, and is delivered to <code>{path}/task-{id}/failures.csv</code>. </p>",
                     "shape": "ReportFormat"
                 },
                 "Path": {
-                    "documentation": "<p>Required if <code>Enabled</code> is set to <code>true</code>. Specifies the location of the report on the file system's linked S3 data repository. An absolute path that defines where the completion report will be stored in the destination location. The <code>Path</code> you provide must be located within the file system\u2019s ExportPath. An example <code>Path</code> value is \"s3://myBucket/myExportPath/optionalPrefix\". The report provides the following information for each file in the report: FilePath, FileStatus, and ErrorCode. To learn more about a file system's <code>ExportPath</code>, see . </p>",
+                    "documentation": "<p>Required if <code>Enabled</code> is set to <code>true</code>. Specifies the location of the report on the file system's linked S3 data repository. An absolute path that defines where the completion report will be stored in the destination location. The <code>Path</code> you provide must be located within the file system\u2019s ExportPath. An example <code>Path</code> value is \"s3://myBucket/myExportPath/optionalPrefix\". The report provides the following information for each file in the report: FilePath, FileStatus, and ErrorCode.</p>",
                     "shape": "ArchivePath"
                 },
                 "Scope": {
                     "documentation": "<p>Required if <code>Enabled</code> is set to <code>true</code>. Specifies the scope of the <code>CompletionReport</code>; <code>FAILED_FILES_ONLY</code> is the only scope currently supported. When <code>Scope</code> is set to <code>FAILED_FILES_ONLY</code>, the <code>CompletionReport</code> only contains information about files that the data repository task failed to process.</p>",
                     "shape": "ReportScope"
                 }
             },
@@ -1891,15 +1894,15 @@
         "CopyTagsToDataRepositoryAssociations": {
             "type": "boolean"
         },
         "CreateBackupRequest": {
             "documentation": "<p>The request object for the <code>CreateBackup</code> operation.</p>",
             "members": {
                 "ClientRequestToken": {
-                    "documentation": "<p>(Optional) A string of up to 64 ASCII characters that Amazon FSx uses to ensure idempotent creation. This string is automatically filled on your behalf when you use the Command Line Interface (CLI) or an Amazon Web Services SDK.</p>",
+                    "documentation": "<p>(Optional) A string of up to 63 ASCII characters that Amazon FSx uses to ensure idempotent creation. This string is automatically filled on your behalf when you use the Command Line Interface (CLI) or an Amazon Web Services SDK.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientRequestToken"
                 },
                 "FileSystemId": {
                     "documentation": "<p>The ID of the file system to back up.</p>",
                     "shape": "FileSystemId"
                 },
@@ -2049,15 +2052,15 @@
                 "MetadataConfiguration"
             ],
             "type": "structure"
         },
         "CreateFileCacheRequest": {
             "members": {
                 "ClientRequestToken": {
-                    "documentation": "<p>An idempotency token for resource creation, in a string of up to 64 ASCII characters. This token is automatically filled on your behalf when you use the Command Line Interface (CLI) or an Amazon Web Services SDK.</p> <p>By using the idempotent operation, you can retry a <code>CreateFileCache</code> operation without the risk of creating an extra cache. This approach can be useful when an initial call fails in a way that makes it unclear whether a cache was created. Examples are if a transport level timeout occurred, or your connection was reset. If you use the same client request token and the initial call created a cache, the client receives success as long as the parameters are the same.</p>",
+                    "documentation": "<p>An idempotency token for resource creation, in a string of up to 63 ASCII characters. This token is automatically filled on your behalf when you use the Command Line Interface (CLI) or an Amazon Web Services SDK.</p> <p>By using the idempotent operation, you can retry a <code>CreateFileCache</code> operation without the risk of creating an extra cache. This approach can be useful when an initial call fails in a way that makes it unclear whether a cache was created. Examples are if a transport level timeout occurred, or your connection was reset. If you use the same client request token and the initial call created a cache, the client receives success as long as the parameters are the same.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientRequestToken"
                 },
                 "CopyTagsToDataRepositoryAssociations": {
                     "documentation": "<p>A boolean flag indicating whether tags for the cache should be copied to data repository associations. This value defaults to false.</p>",
                     "shape": "CopyTagsToDataRepositoryAssociations"
                 },
@@ -2116,15 +2119,15 @@
         "CreateFileSystemFromBackupRequest": {
             "documentation": "<p>The request object for the <code>CreateFileSystemFromBackup</code> operation.</p>",
             "members": {
                 "BackupId": {
                     "shape": "BackupId"
                 },
                 "ClientRequestToken": {
-                    "documentation": "<p>A string of up to 64 ASCII characters that Amazon FSx uses to ensure idempotent creation. This string is automatically filled on your behalf when you use the Command Line Interface (CLI) or an Amazon Web Services SDK.</p>",
+                    "documentation": "<p>A string of up to 63 ASCII characters that Amazon FSx uses to ensure idempotent creation. This string is automatically filled on your behalf when you use the Command Line Interface (CLI) or an Amazon Web Services SDK.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientRequestToken"
                 },
                 "FileSystemTypeVersion": {
                     "documentation": "<p>Sets the version for the Amazon FSx for Lustre file system that you're creating from a backup. Valid values are <code>2.10</code> and <code>2.12</code>.</p> <p>You don't need to specify <code>FileSystemTypeVersion</code> because it will be applied using the backup's <code>FileSystemTypeVersion</code> setting. If you choose to specify <code>FileSystemTypeVersion</code> when creating from backup, the value must match the backup's <code>FileSystemTypeVersion</code> setting.</p>",
                     "shape": "FileSystemTypeVersion"
                 },
@@ -2176,52 +2179,53 @@
                     "documentation": "<p>A description of the file system.</p>",
                     "shape": "FileSystem"
                 }
             },
             "type": "structure"
         },
         "CreateFileSystemLustreConfiguration": {
-            "documentation": "<p>The Lustre configuration for the file system being created.</p> <note> <p>The following parameters are not supported for file systems with the <code>Persistent_2</code> deployment type. Instead, use <code>CreateDataRepositoryAssociation</code> to create a data repository association to link your Lustre file system to a data repository.</p> <ul> <li> <p> <code>AutoImportPolicy</code> </p> </li> <li> <p> <code>ExportPath</code> </p> </li> <li> <p> <code>ImportedChunkSize</code> </p> </li> <li> <p> <code>ImportPath</code> </p> </li> </ul> </note>",
+            "documentation": "<p>The Lustre configuration for the file system being created.</p> <note> <p>The following parameters are not supported for file systems with a data repository association created with .</p> <ul> <li> <p> <code>AutoImportPolicy</code> </p> </li> <li> <p> <code>ExportPath</code> </p> </li> <li> <p> <code>ImportedChunkSize</code> </p> </li> <li> <p> <code>ImportPath</code> </p> </li> </ul> </note>",
             "members": {
                 "AutoImportPolicy": {
-                    "documentation": "<p> (Optional) Available with <code>Scratch</code> and <code>Persistent_1</code> deployment types. When you create your file system, your existing S3 objects appear as file and directory listings. Use this property to choose how Amazon FSx keeps your file and directory listings up to date as you add or modify objects in your linked S3 bucket. <code>AutoImportPolicy</code> can have the following values:</p> <ul> <li> <p> <code>NONE</code> - (Default) AutoImport is off. Amazon FSx only updates file and directory listings from the linked S3 bucket when the file system is created. FSx does not update file and directory listings for any new or changed objects after choosing this option.</p> </li> <li> <p> <code>NEW</code> - AutoImport is on. Amazon FSx automatically imports directory listings of any new objects added to the linked S3 bucket that do not currently exist in the FSx file system. </p> </li> <li> <p> <code>NEW_CHANGED</code> - AutoImport is on. Amazon FSx automatically imports file and directory listings of any new objects added to the S3 bucket and any existing objects that are changed in the S3 bucket after you choose this option.</p> </li> <li> <p> <code>NEW_CHANGED_DELETED</code> - AutoImport is on. Amazon FSx automatically imports file and directory listings of any new objects added to the S3 bucket, any existing objects that are changed in the S3 bucket, and any objects that were deleted in the S3 bucket.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/older-deployment-types.html#legacy-auto-import-from-s3\"> Automatically import updates from your S3 bucket</a>.</p> <note> <p>This parameter is not supported for file systems with the <code>Persistent_2</code> deployment type. Instead, use <code>CreateDataRepositoryAssociation</code> to create a data repository association to link your Lustre file system to a data repository.</p> </note>",
+                    "documentation": "<p> (Optional) When you create your file system, your existing S3 objects appear as file and directory listings. Use this parameter to choose how Amazon FSx keeps your file and directory listings up to date as you add or modify objects in your linked S3 bucket. <code>AutoImportPolicy</code> can have the following values:</p> <ul> <li> <p> <code>NONE</code> - (Default) AutoImport is off. Amazon FSx only updates file and directory listings from the linked S3 bucket when the file system is created. FSx does not update file and directory listings for any new or changed objects after choosing this option.</p> </li> <li> <p> <code>NEW</code> - AutoImport is on. Amazon FSx automatically imports directory listings of any new objects added to the linked S3 bucket that do not currently exist in the FSx file system. </p> </li> <li> <p> <code>NEW_CHANGED</code> - AutoImport is on. Amazon FSx automatically imports file and directory listings of any new objects added to the S3 bucket and any existing objects that are changed in the S3 bucket after you choose this option.</p> </li> <li> <p> <code>NEW_CHANGED_DELETED</code> - AutoImport is on. Amazon FSx automatically imports file and directory listings of any new objects added to the S3 bucket, any existing objects that are changed in the S3 bucket, and any objects that were deleted in the S3 bucket.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/older-deployment-types.html#legacy-auto-import-from-s3\"> Automatically import updates from your S3 bucket</a>.</p> <note> <p>This parameter is not supported for file systems with a data repository association.</p> </note>",
                     "shape": "AutoImportPolicyType"
                 },
                 "AutomaticBackupRetentionDays": {
+                    "documentation": "<p>The number of days to retain automatic backups. Setting this property to <code>0</code> disables automatic backups. You can retain automatic backups for a maximum of 90 days. The default is <code>0</code>.</p>",
                     "shape": "AutomaticBackupRetentionDays"
                 },
                 "CopyTagsToBackups": {
                     "documentation": "<p>(Optional) Not available for use with file systems that are linked to a data repository. A boolean flag indicating whether tags for the file system should be copied to backups. The default value is false. If <code>CopyTagsToBackups</code> is set to true, all file system tags are copied to all automatic and user-initiated backups when the user doesn't specify any backup-specific tags. If <code>CopyTagsToBackups</code> is set to true and you specify one or more backup tags, only the specified tags are copied to backups. If you specify one or more tags when creating a user-initiated backup, no tags are copied from the file system, regardless of this value.</p> <p>(Default = <code>false</code>)</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/using-backups-fsx.html\"> Working with backups</a> in the <i>Amazon FSx for Lustre User Guide</i>.</p>",
                     "shape": "Flag"
                 },
                 "DailyAutomaticBackupStartTime": {
                     "shape": "DailyTime"
                 },
                 "DataCompressionType": {
                     "documentation": "<p>Sets the data compression configuration for the file system. <code>DataCompressionType</code> can have the following values:</p> <ul> <li> <p> <code>NONE</code> - (Default) Data compression is turned off when the file system is created.</p> </li> <li> <p> <code>LZ4</code> - Data compression is turned on with the LZ4 algorithm.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/data-compression.html\">Lustre data compression</a> in the <i>Amazon FSx for Lustre User Guide</i>.</p>",
                     "shape": "DataCompressionType"
                 },
                 "DeploymentType": {
-                    "documentation": "<p>(Optional) Choose <code>SCRATCH_1</code> and <code>SCRATCH_2</code> deployment types when you need temporary storage and shorter-term processing of data. The <code>SCRATCH_2</code> deployment type provides in-transit encryption of data and higher burst throughput capacity than <code>SCRATCH_1</code>.</p> <p>Choose <code>PERSISTENT_1</code> for longer-term storage and for throughput-focused workloads that aren\u2019t latency-sensitive. <code>PERSISTENT_1</code> supports encryption of data in transit, and is available in all Amazon Web Services Regions in which FSx for Lustre is available.</p> <p>Choose <code>PERSISTENT_2</code> for longer-term storage and for latency-sensitive workloads that require the highest levels of IOPS/throughput. <code>PERSISTENT_2</code> supports SSD storage, and offers higher <code>PerUnitStorageThroughput</code> (up to 1000 MB/s/TiB). <code>PERSISTENT_2</code> is available in a limited number of Amazon Web Services Regions. For more information, and an up-to-date list of Amazon Web Services Regions in which <code>PERSISTENT_2</code> is available, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/using-fsx-lustre.html#lustre-deployment-types\">File system deployment options for FSx for Lustre</a> in the <i>Amazon FSx for Lustre User Guide</i>.</p> <note> <p>If you choose <code>PERSISTENT_2</code>, and you set <code>FileSystemTypeVersion</code> to <code>2.10</code>, the <code>CreateFileSystem</code> operation fails.</p> </note> <p>Encryption of data in transit is automatically turned on when you access <code>SCRATCH_2</code>, <code>PERSISTENT_1</code> and <code>PERSISTENT_2</code> file systems from Amazon EC2 instances that <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/data- protection.html\">support automatic encryption</a> in the Amazon Web Services Regions where they are available. For more information about encryption in transit for FSx for Lustre file systems, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/encryption-in-transit-fsxl.html\">Encrypting data in transit</a> in the <i>Amazon FSx for Lustre User Guide</i>. </p> <p>(Default = <code>SCRATCH_1</code>)</p>",
+                    "documentation": "<p>(Optional) Choose <code>SCRATCH_1</code> and <code>SCRATCH_2</code> deployment types when you need temporary storage and shorter-term processing of data. The <code>SCRATCH_2</code> deployment type provides in-transit encryption of data and higher burst throughput capacity than <code>SCRATCH_1</code>.</p> <p>Choose <code>PERSISTENT_1</code> for longer-term storage and for throughput-focused workloads that aren\u2019t latency-sensitive. <code>PERSISTENT_1</code> supports encryption of data in transit, and is available in all Amazon Web Services Regions in which FSx for Lustre is available.</p> <p>Choose <code>PERSISTENT_2</code> for longer-term storage and for latency-sensitive workloads that require the highest levels of IOPS/throughput. <code>PERSISTENT_2</code> supports SSD storage, and offers higher <code>PerUnitStorageThroughput</code> (up to 1000 MB/s/TiB). <code>PERSISTENT_2</code> is available in a limited number of Amazon Web Services Regions. For more information, and an up-to-date list of Amazon Web Services Regions in which <code>PERSISTENT_2</code> is available, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/using-fsx-lustre.html#lustre-deployment-types\">File system deployment options for FSx for Lustre</a> in the <i>Amazon FSx for Lustre User Guide</i>.</p> <note> <p>If you choose <code>PERSISTENT_2</code>, and you set <code>FileSystemTypeVersion</code> to <code>2.10</code>, the <code>CreateFileSystem</code> operation fails.</p> </note> <p>Encryption of data in transit is automatically turned on when you access <code>SCRATCH_2</code>, <code>PERSISTENT_1</code> and <code>PERSISTENT_2</code> file systems from Amazon EC2 instances that support automatic encryption in the Amazon Web Services Regions where they are available. For more information about encryption in transit for FSx for Lustre file systems, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/encryption-in-transit-fsxl.html\">Encrypting data in transit</a> in the <i>Amazon FSx for Lustre User Guide</i>. </p> <p>(Default = <code>SCRATCH_1</code>)</p>",
                     "shape": "LustreDeploymentType"
                 },
                 "DriveCacheType": {
                     "documentation": "<p>The type of drive cache used by <code>PERSISTENT_1</code> file systems that are provisioned with HDD storage devices. This parameter is required when storage type is HDD. Set this property to <code>READ</code> to improve the performance for frequently accessed files by caching up to 20% of the total storage capacity of the file system.</p> <p>This parameter is required when <code>StorageType</code> is set to <code>HDD</code>.</p>",
                     "shape": "DriveCacheType"
                 },
                 "ExportPath": {
-                    "documentation": "<p>(Optional) Available with <code>Scratch</code> and <code>Persistent_1</code> deployment types. Specifies the path in the Amazon S3 bucket where the root of your Amazon FSx file system is exported. The path must use the same Amazon S3 bucket as specified in ImportPath. You can provide an optional prefix to which new and changed data is to be exported from your Amazon FSx for Lustre file system. If an <code>ExportPath</code> value is not provided, Amazon FSx sets a default export path, <code>s3://import-bucket/FSxLustre[creation-timestamp]</code>. The timestamp is in UTC format, for example <code>s3://import-bucket/FSxLustre20181105T222312Z</code>.</p> <p>The Amazon S3 export bucket must be the same as the import bucket specified by <code>ImportPath</code>. If you specify only a bucket name, such as <code>s3://import-bucket</code>, you get a 1:1 mapping of file system objects to S3 bucket objects. This mapping means that the input data in S3 is overwritten on export. If you provide a custom prefix in the export path, such as <code>s3://import-bucket/[custom-optional-prefix]</code>, Amazon FSx exports the contents of your file system to that export prefix in the Amazon S3 bucket.</p> <note> <p>This parameter is not supported for file systems with the <code>Persistent_2</code> deployment type. Instead, use <code>CreateDataRepositoryAssociation</code> to create a data repository association to link your Lustre file system to a data repository.</p> </note>",
+                    "documentation": "<p>(Optional) Specifies the path in the Amazon S3 bucket where the root of your Amazon FSx file system is exported. The path must use the same Amazon S3 bucket as specified in ImportPath. You can provide an optional prefix to which new and changed data is to be exported from your Amazon FSx for Lustre file system. If an <code>ExportPath</code> value is not provided, Amazon FSx sets a default export path, <code>s3://import-bucket/FSxLustre[creation-timestamp]</code>. The timestamp is in UTC format, for example <code>s3://import-bucket/FSxLustre20181105T222312Z</code>.</p> <p>The Amazon S3 export bucket must be the same as the import bucket specified by <code>ImportPath</code>. If you specify only a bucket name, such as <code>s3://import-bucket</code>, you get a 1:1 mapping of file system objects to S3 bucket objects. This mapping means that the input data in S3 is overwritten on export. If you provide a custom prefix in the export path, such as <code>s3://import-bucket/[custom-optional-prefix]</code>, Amazon FSx exports the contents of your file system to that export prefix in the Amazon S3 bucket.</p> <note> <p>This parameter is not supported for file systems with a data repository association.</p> </note>",
                     "shape": "ArchivePath"
                 },
                 "ImportPath": {
-                    "documentation": "<p>(Optional) The path to the Amazon S3 bucket (including the optional prefix) that you're using as the data repository for your Amazon FSx for Lustre file system. The root of your FSx for Lustre file system will be mapped to the root of the Amazon S3 bucket you select. An example is <code>s3://import-bucket/optional-prefix</code>. If you specify a prefix after the Amazon S3 bucket name, only object keys with that prefix are loaded into the file system.</p> <note> <p>This parameter is not supported for file systems with the <code>Persistent_2</code> deployment type. Instead, use <code>CreateDataRepositoryAssociation</code> to create a data repository association to link your Lustre file system to a data repository.</p> </note>",
+                    "documentation": "<p>(Optional) The path to the Amazon S3 bucket (including the optional prefix) that you're using as the data repository for your Amazon FSx for Lustre file system. The root of your FSx for Lustre file system will be mapped to the root of the Amazon S3 bucket you select. An example is <code>s3://import-bucket/optional-prefix</code>. If you specify a prefix after the Amazon S3 bucket name, only object keys with that prefix are loaded into the file system.</p> <note> <p>This parameter is not supported for file systems with a data repository association.</p> </note>",
                     "shape": "ArchivePath"
                 },
                 "ImportedFileChunkSize": {
-                    "documentation": "<p>(Optional) For files imported from a data repository, this value determines the stripe count and maximum amount of data per file (in MiB) stored on a single physical disk. The maximum number of disks that a single file can be striped across is limited by the total number of disks that make up the file system.</p> <p>The default chunk size is 1,024 MiB (1 GiB) and can go as high as 512,000 MiB (500 GiB). Amazon S3 objects have a maximum size of 5 TB.</p> <p>This parameter is not supported for file systems with the <code>Persistent_2</code> deployment type. Instead, use <code>CreateDataRepositoryAssociation</code> to create a data repository association to link your Lustre file system to a data repository.</p>",
+                    "documentation": "<p>(Optional) For files imported from a data repository, this value determines the stripe count and maximum amount of data per file (in MiB) stored on a single physical disk. The maximum number of disks that a single file can be striped across is limited by the total number of disks that make up the file system.</p> <p>The default chunk size is 1,024 MiB (1 GiB) and can go as high as 512,000 MiB (500 GiB). Amazon S3 objects have a maximum size of 5 TB.</p> <note> <p>This parameter is not supported for file systems with a data repository association.</p> </note>",
                     "shape": "Megabytes"
                 },
                 "LogConfiguration": {
                     "documentation": "<p>The Lustre logging configuration used when creating an Amazon FSx for Lustre file system. When logging is enabled, Lustre logs error and warning events for data repositories associated with your file system to Amazon CloudWatch Logs.</p>",
                     "shape": "LustreLogCreateConfiguration"
                 },
                 "PerUnitStorageThroughput": {
@@ -2253,15 +2257,15 @@
                     "shape": "OntapDeploymentType"
                 },
                 "DiskIopsConfiguration": {
                     "documentation": "<p>The SSD IOPS configuration for the FSx for ONTAP file system.</p>",
                     "shape": "DiskIopsConfiguration"
                 },
                 "EndpointIpAddressRange": {
-                    "documentation": "<p>(Multi-AZ only) Specifies the IP address range in which the endpoints to access your file system will be created. By default in the Amazon FSx API, Amazon FSx selects an unused IP address range for you from the 198.19.* range. By default in the Amazon FSx console, Amazon FSx chooses the last 64 IP addresses from the VPC\u2019s primary CIDR range to use as the endpoint IP address range for the file system. You can have overlapping endpoint IP addresses for file systems deployed in the same VPC/route tables.</p>",
+                    "documentation": "<p>(Multi-AZ only) Specifies the IP address range in which the endpoints to access your file system will be created. By default in the Amazon FSx API, Amazon FSx selects an unused IP address range for you from the 198.19.* range. By default in the Amazon FSx console, Amazon FSx chooses the last 64 IP addresses from the VPC\u2019s primary CIDR range to use as the endpoint IP address range for the file system. You can have overlapping endpoint IP addresses for file systems deployed in the same VPC/route tables, as long as they don't overlap with any subnet.</p>",
                     "shape": "IpAddressRange"
                 },
                 "FsxAdminPassword": {
                     "documentation": "<p>The ONTAP administrative password for the <code>fsxadmin</code> user with which you administer your file system using the NetApp ONTAP CLI and REST API.</p>",
                     "shape": "AdminPassword"
                 },
                 "PreferredSubnetId": {
@@ -2300,26 +2304,26 @@
                     "documentation": "<p>A Boolean value indicating whether tags for the file system should be copied to volumes. This value defaults to <code>false</code>. If it's set to <code>true</code>, all tags for the file system are copied to volumes where the user doesn't specify tags. If this value is <code>true</code>, and you specify one or more tags, only the specified tags are copied to volumes. If you specify one or more tags when creating the volume, no tags are copied from the file system, regardless of this value.</p>",
                     "shape": "Flag"
                 },
                 "DailyAutomaticBackupStartTime": {
                     "shape": "DailyTime"
                 },
                 "DeploymentType": {
-                    "documentation": "<p>Specifies the file system deployment type. Single AZ deployment types are configured for redundancy within a single Availability Zone in an Amazon Web Services Region . Valid values are the following:</p> <ul> <li> <p> <code>SINGLE_AZ_1</code>- (Default) Creates file systems with throughput capacities of 64 - 4,096 MB/s. <code>Single_AZ_1</code> is available in all Amazon Web Services Regions where Amazon FSx for OpenZFS is available, except US West (Oregon).</p> </li> <li> <p> <code>SINGLE_AZ_2</code>- Creates file systems with throughput capacities of 160 - 10,240 MB/s using an NVMe L2ARC cache. <code>Single_AZ_2</code> is available only in the US East (N. Virginia), US East (Ohio), US West (Oregon), and Europe (Ireland) Amazon Web Services Regions.</p> </li> </ul> <p>For more information, see: <a href=\"https://docs.aws.amazon.com/fsx/latest/OpenZFSGuide/availability-durability.html#available-aws-regions\">Deployment type availability</a> and <a href=\"https://docs.aws.amazon.com/fsx/latest/OpenZFSGuide/performance.html#zfs-fs-performance\">File system performance</a> in the <i>Amazon FSx for OpenZFS User Guide</i>.</p>",
+                    "documentation": "<p>Specifies the file system deployment type. Single AZ deployment types are configured for redundancy within a single Availability Zone in an Amazon Web Services Region . Valid values are the following:</p> <ul> <li> <p> <code>SINGLE_AZ_1</code>- (Default) Creates file systems with throughput capacities of 64 - 4,096 MBps. <code>Single_AZ_1</code> is available in all Amazon Web Services Regions where Amazon FSx for OpenZFS is available.</p> </li> <li> <p> <code>SINGLE_AZ_2</code>- Creates file systems with throughput capacities of 160 - 10,240 MB/s using an NVMe L2ARC cache. <code>Single_AZ_2</code> is available only in the US East (N. Virginia), US East (Ohio), US West (Oregon), and Europe (Ireland) Amazon Web Services Regions.</p> </li> </ul> <p>For more information, see: <a href=\"https://docs.aws.amazon.com/fsx/latest/OpenZFSGuide/availability-durability.html#available-aws-regions\">Deployment type availability</a> and <a href=\"https://docs.aws.amazon.com/fsx/latest/OpenZFSGuide/performance.html#zfs-fs-performance\">File system performance</a> in the <i>Amazon FSx for OpenZFS User Guide</i>.</p>",
                     "shape": "OpenZFSDeploymentType"
                 },
                 "DiskIopsConfiguration": {
                     "shape": "DiskIopsConfiguration"
                 },
                 "RootVolumeConfiguration": {
                     "documentation": "<p>The configuration Amazon FSx uses when creating the root value of the Amazon FSx for OpenZFS file system. All volumes are children of the root volume. </p>",
                     "shape": "OpenZFSCreateRootVolumeConfiguration"
                 },
                 "ThroughputCapacity": {
-                    "documentation": "<p>Specifies the throughput of an Amazon FSx for OpenZFS file system, measured in megabytes per second (MB/s). Valid values depend on the DeploymentType you choose, as follows:</p> <ul> <li> <p>For <code>SINGLE_AZ_1</code>, valid values are 64, 128, 256, 512, 1024, 2048, 3072, or 4096 MB/s.</p> </li> <li> <p>For <code>SINGLE_AZ_2</code>, valid values are 160, 320, 640, 1280, 2560, 3840, 5120, 7680, or 10240 MB/s.</p> </li> </ul> <p>You pay for additional throughput capacity that you provision.</p>",
+                    "documentation": "<p>Specifies the throughput of an Amazon FSx for OpenZFS file system, measured in megabytes per second (MBps). Valid values depend on the DeploymentType you choose, as follows:</p> <ul> <li> <p>For <code>SINGLE_AZ_1</code>, valid values are 64, 128, 256, 512, 1024, 2048, 3072, or 4096 MBps.</p> </li> <li> <p>For <code>SINGLE_AZ_2</code>, valid values are 160, 320, 640, 1280, 2560, 3840, 5120, 7680, or 10240 MBps.</p> </li> </ul> <p>You pay for additional throughput capacity that you provision.</p>",
                     "shape": "MegabytesPerSecond"
                 },
                 "WeeklyMaintenanceStartTime": {
                     "shape": "WeeklyTime"
                 }
             },
             "required": [
@@ -2328,15 +2332,15 @@
             ],
             "type": "structure"
         },
         "CreateFileSystemRequest": {
             "documentation": "<p>The request object used to create a new Amazon FSx file system.</p>",
             "members": {
                 "ClientRequestToken": {
-                    "documentation": "<p>A string of up to 64 ASCII characters that Amazon FSx uses to ensure idempotent creation. This string is automatically filled on your behalf when you use the Command Line Interface (CLI) or an Amazon Web Services SDK.</p>",
+                    "documentation": "<p>A string of up to 63 ASCII characters that Amazon FSx uses to ensure idempotent creation. This string is automatically filled on your behalf when you use the Command Line Interface (CLI) or an Amazon Web Services SDK.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientRequestToken"
                 },
                 "FileSystemType": {
                     "documentation": "<p>The type of Amazon FSx file system to create. Valid values are <code>WINDOWS</code>, <code>LUSTRE</code>, <code>ONTAP</code>, and <code>OPENZFS</code>.</p>",
                     "shape": "FileSystemType"
                 },
@@ -2411,15 +2415,15 @@
                     "shape": "AlternateDNSNames"
                 },
                 "AuditLogConfiguration": {
                     "documentation": "<p>The configuration that Amazon FSx for Windows File Server uses to audit and log user accesses of files, folders, and file shares on the Amazon FSx for Windows File Server file system.</p>",
                     "shape": "WindowsAuditLogCreateConfiguration"
                 },
                 "AutomaticBackupRetentionDays": {
-                    "documentation": "<p>The number of days to retain automatic backups. The default is to retain backups for 7 days. Setting this value to 0 disables the creation of automatic backups. The maximum retention period for backups is 90 days.</p>",
+                    "documentation": "<p>The number of days to retain automatic backups. Setting this property to <code>0</code> disables automatic backups. You can retain automatic backups for a maximum of 90 days. The default is <code>30</code>.</p>",
                     "shape": "AutomaticBackupRetentionDays"
                 },
                 "CopyTagsToBackups": {
                     "documentation": "<p>A boolean flag indicating whether tags for the file system should be copied to backups. This value defaults to false. If it's set to true, all tags for the file system are copied to all automatic and user-initiated backups where the user doesn't specify tags. If this value is true, and you specify one or more tags, only the specified tags are copied to backups. If you specify one or more tags when creating a user-initiated backup, no tags are copied from the file system, regardless of this value.</p>",
                     "shape": "Flag"
                 },
                 "DailyAutomaticBackupStartTime": {
@@ -2455,35 +2459,35 @@
             "documentation": "<p>Specifies the configuration of the ONTAP volume that you are creating.</p>",
             "members": {
                 "CopyTagsToBackups": {
                     "documentation": "<p>A boolean flag indicating whether tags for the volume should be copied to backups. This value defaults to false. If it's set to true, all tags for the volume are copied to all automatic and user-initiated backups where the user doesn't specify tags. If this value is true, and you specify one or more tags, only the specified tags are copied to backups. If you specify one or more tags when creating a user-initiated backup, no tags are copied from the volume, regardless of this value.</p>",
                     "shape": "Flag"
                 },
                 "JunctionPath": {
-                    "documentation": "<p>Specifies the location in the SVM's namespace where the volume is mounted. The <code>JunctionPath</code> must have a leading forward slash, such as <code>/vol3</code>.</p>",
+                    "documentation": "<p>Specifies the location in the SVM's namespace where the volume is mounted. This parameter is required. The <code>JunctionPath</code> must have a leading forward slash, such as <code>/vol3</code>.</p>",
                     "shape": "JunctionPath"
                 },
                 "OntapVolumeType": {
                     "documentation": "<p>Specifies the type of volume you are creating. Valid values are the following:</p> <ul> <li> <p> <code>RW</code> specifies a read/write volume. <code>RW</code> is the default.</p> </li> <li> <p> <code>DP</code> specifies a data-protection volume. A <code>DP</code> volume is read-only and can be used as the destination of a NetApp SnapMirror relationship.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/volume-types\">Volume types</a> in the <i>Amazon FSx for NetApp ONTAP User Guide</i>.</p>",
                     "shape": "InputOntapVolumeType"
                 },
                 "SecurityStyle": {
                     "documentation": "<p>Specifies the security style for the volume. If a volume's security style is not specified, it is automatically set to the root volume's security style. The security style determines the type of permissions that FSx for ONTAP uses to control data access. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/managing-volumes.html#volume-security-style\">Volume security style</a> in the <i>Amazon FSx for NetApp ONTAP User Guide</i>. Specify one of the following values:</p> <ul> <li> <p> <code>UNIX</code> if the file system is managed by a UNIX administrator, the majority of users are NFS clients, and an application accessing the data uses a UNIX user as the service account. </p> </li> <li> <p> <code>NTFS</code> if the file system is managed by a Windows administrator, the majority of users are SMB clients, and an application accessing the data uses a Windows user as the service account.</p> </li> <li> <p> <code>MIXED</code> if the file system is managed by both UNIX and Windows administrators and users consist of both NFS and SMB clients.</p> </li> </ul>",
                     "shape": "SecurityStyle"
                 },
                 "SizeInMegabytes": {
-                    "documentation": "<p>Specifies the size of the volume, in megabytes (MB), that you are creating.</p>",
+                    "documentation": "<p>Specifies the size of the volume, in megabytes (MB), that you are creating. Provide any whole number in the range of 20\u2013104857600 to specify the size of the volume.</p>",
                     "shape": "VolumeCapacity"
                 },
                 "SnapshotPolicy": {
                     "documentation": "<p>Specifies the snapshot policy for the volume. There are three built-in snapshot policies:</p> <ul> <li> <p> <code>default</code>: This is the default policy. A maximum of six hourly snapshots taken five minutes past the hour. A maximum of two daily snapshots taken Monday through Saturday at 10 minutes after midnight. A maximum of two weekly snapshots taken every Sunday at 15 minutes after midnight.</p> </li> <li> <p> <code>default-1weekly</code>: This policy is the same as the <code>default</code> policy except that it only retains one snapshot from the weekly schedule.</p> </li> <li> <p> <code>none</code>: This policy does not take any snapshots. This policy can be assigned to volumes to prevent automatic snapshots from being taken.</p> </li> </ul> <p>You can also provide the name of a custom policy that you created with the ONTAP CLI or REST API.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/snapshots-ontap.html#snapshot-policies\">Snapshot policies</a> in the <i>Amazon FSx for NetApp ONTAP User Guide</i>.</p>",
                     "shape": "SnapshotPolicy"
                 },
                 "StorageEfficiencyEnabled": {
-                    "documentation": "<p>Set to true to enable deduplication, compression, and compaction storage efficiency features on the volume.</p>",
+                    "documentation": "<p>Set to true to enable deduplication, compression, and compaction storage efficiency features on the volume, or set to false to disable them. This parameter is required.</p>",
                     "shape": "Flag"
                 },
                 "StorageVirtualMachineId": {
                     "documentation": "<p>Specifies the ONTAP SVM in which to create the volume.</p>",
                     "shape": "StorageVirtualMachineId"
                 },
                 "TieringPolicy": {
@@ -2733,15 +2737,15 @@
             "type": "structure"
         },
         "CreationTime": {
             "documentation": "<p>The time that the resource was created, in seconds (since 1970-01-01T00:00:00Z), also known as Unix time.</p>",
             "type": "timestamp"
         },
         "DNSName": {
-            "documentation": "<p>The Domain Name Service (DNS) name for the file system. You can mount your file system using its DNS name.</p>",
+            "documentation": "<p>The file system's DNS name. You can mount your file system using its DNS name.</p>",
             "max": 275,
             "min": 16,
             "pattern": "^((fs|fc)i?-[0-9a-f]{8,}\\..{4,253})$",
             "type": "string"
         },
         "DailyTime": {
             "documentation": "<p>A recurring daily time, in the format <code>HH:MM</code>. <code>HH</code> is the zero-padded hour of the day (0-23), and <code>MM</code> is the zero-padded minute of the hour. For example, <code>05:00</code> specifies 5 AM daily. </p>",
@@ -2754,15 +2758,15 @@
             "enum": [
                 "NONE",
                 "LZ4"
             ],
             "type": "string"
         },
         "DataRepositoryAssociation": {
-            "documentation": "<p>The configuration of a data repository association that links an Amazon FSx for Lustre file system to an Amazon S3 bucket or an Amazon File Cache resource to an Amazon S3 bucket or an NFS file system. The data repository association configuration object is returned in the response of the following operations:</p> <ul> <li> <p> <code>CreateDataRepositoryAssociation</code> </p> </li> <li> <p> <code>UpdateDataRepositoryAssociation</code> </p> </li> <li> <p> <code>DescribeDataRepositoryAssociations</code> </p> </li> </ul> <p>Data repository associations are supported only for an Amazon FSx for Lustre file system with the <code>Persistent_2</code> deployment type and for an Amazon File Cache resource.</p>",
+            "documentation": "<p>The configuration of a data repository association that links an Amazon FSx for Lustre file system to an Amazon S3 bucket or an Amazon File Cache resource to an Amazon S3 bucket or an NFS file system. The data repository association configuration object is returned in the response of the following operations:</p> <ul> <li> <p> <code>CreateDataRepositoryAssociation</code> </p> </li> <li> <p> <code>UpdateDataRepositoryAssociation</code> </p> </li> <li> <p> <code>DescribeDataRepositoryAssociations</code> </p> </li> </ul> <p>Data repository associations are supported on Amazon File Cache resources and all FSx for Lustre 2.12 and newer file systems, excluding <code>scratch_1</code> deployment type.</p>",
             "members": {
                 "AssociationId": {
                     "documentation": "<p>The system-generated, unique ID of the data repository association.</p>",
                     "shape": "DataRepositoryAssociationId"
                 },
                 "BatchImportMetaDataOnCreate": {
                     "documentation": "<p>A boolean flag indicating whether an import data repository task to import metadata should run after the data repository association is created. The task runs if this flag is set to <code>true</code>.</p> <note> <p> <code>BatchImportMetaDataOnCreate</code> is not supported for data repositories linked to an Amazon File Cache resource.</p> </note>",
@@ -2849,15 +2853,15 @@
             "max": 100,
             "member": {
                 "shape": "DataRepositoryAssociation"
             },
             "type": "list"
         },
         "DataRepositoryConfiguration": {
-            "documentation": "<p>The data repository configuration object for Lustre file systems returned in the response of the <code>CreateFileSystem</code> operation.</p> <p>This data type is not supported for file systems with the <code>Persistent_2</code> deployment type. Instead, use .</p>",
+            "documentation": "<p>The data repository configuration object for Lustre file systems returned in the response of the <code>CreateFileSystem</code> operation.</p> <p>This data type is not supported on file systems with a data repository association. For file systems with a data repository association, see .</p>",
             "members": {
                 "AutoImportPolicy": {
                     "documentation": "<p>Describes the file system's linked S3 data repository's <code>AutoImportPolicy</code>. The AutoImportPolicy configures how Amazon FSx keeps your file and directory listings up to date as you add or modify objects in your linked S3 bucket. <code>AutoImportPolicy</code> can have the following values:</p> <ul> <li> <p> <code>NONE</code> - (Default) AutoImport is off. Amazon FSx only updates file and directory listings from the linked S3 bucket when the file system is created. FSx does not update file and directory listings for any new or changed objects after choosing this option.</p> </li> <li> <p> <code>NEW</code> - AutoImport is on. Amazon FSx automatically imports directory listings of any new objects added to the linked S3 bucket that do not currently exist in the FSx file system. </p> </li> <li> <p> <code>NEW_CHANGED</code> - AutoImport is on. Amazon FSx automatically imports file and directory listings of any new objects added to the S3 bucket and any existing objects that are changed in the S3 bucket after you choose this option.</p> </li> <li> <p> <code>NEW_CHANGED_DELETED</code> - AutoImport is on. Amazon FSx automatically imports file and directory listings of any new objects added to the S3 bucket, any existing objects that are changed in the S3 bucket, and any objects that were deleted in the S3 bucket.</p> </li> </ul>",
                     "shape": "AutoImportPolicyType"
                 },
                 "ExportPath": {
                     "documentation": "<p>The export path to the Amazon S3 bucket (and prefix) that you are using to store new and changed Lustre file system files in S3.</p>",
@@ -2953,15 +2957,15 @@
                     "shape": "Tags"
                 },
                 "TaskId": {
                     "documentation": "<p>The system-generated, unique 17-digit ID of the data repository task.</p>",
                     "shape": "TaskId"
                 },
                 "Type": {
-                    "documentation": "<p>The type of data repository task.</p> <ul> <li> <p> <code>EXPORT_TO_REPOSITORY</code> tasks export from your Amazon FSx for Lustre file system to a linked data repository.</p> </li> <li> <p> <code>IMPORT_METADATA_FROM_REPOSITORY</code> tasks import metadata changes from a linked S3 bucket to your Amazon FSx for Lustre file system.</p> </li> <li> <p> <code>AUTO_RELEASE_DATA</code> tasks automatically release files from an Amazon File Cache resource.</p> </li> </ul>",
+                    "documentation": "<p>The type of data repository task.</p> <ul> <li> <p> <code>EXPORT_TO_REPOSITORY</code> tasks export from your Amazon FSx for Lustre file system to a linked data repository.</p> </li> <li> <p> <code>IMPORT_METADATA_FROM_REPOSITORY</code> tasks import metadata changes from a linked S3 bucket to your Amazon FSx for Lustre file system.</p> </li> <li> <p> <code>AUTO_RELEASE_DATA</code> tasks automatically release files from an Amazon File Cache resource.</p> </li> <li> <p> <code>RELEASE_DATA_FROM_FILESYSTEM</code> tasks are not supported.</p> </li> </ul>",
                     "shape": "DataRepositoryTaskType"
                 }
             },
             "required": [
                 "TaskId",
                 "Lifecycle",
                 "Type",
@@ -3121,15 +3125,15 @@
             "documentation": "<p>The request object for the <code>DeleteBackup</code> operation.</p>",
             "members": {
                 "BackupId": {
                     "documentation": "<p>The ID of the backup that you want to delete.</p>",
                     "shape": "BackupId"
                 },
                 "ClientRequestToken": {
-                    "documentation": "<p>A string of up to 64 ASCII characters that Amazon FSx uses to ensure idempotent deletion. This parameter is automatically filled on your behalf when using the CLI or SDK.</p>",
+                    "documentation": "<p>A string of up to 63 ASCII characters that Amazon FSx uses to ensure idempotent deletion. This parameter is automatically filled on your behalf when using the CLI or SDK.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientRequestToken"
                 }
             },
             "required": [
                 "BackupId"
             ],
@@ -3289,15 +3293,15 @@
             },
             "type": "structure"
         },
         "DeleteFileSystemRequest": {
             "documentation": "<p>The request object for <code>DeleteFileSystem</code> operation.</p>",
             "members": {
                 "ClientRequestToken": {
-                    "documentation": "<p>A string of up to 64 ASCII characters that Amazon FSx uses to ensure idempotent deletion. This token is automatically filled on your behalf when using the Command Line Interface (CLI) or an Amazon Web Services SDK.</p>",
+                    "documentation": "<p>A string of up to 63 ASCII characters that Amazon FSx uses to ensure idempotent deletion. This token is automatically filled on your behalf when using the Command Line Interface (CLI) or an Amazon Web Services SDK.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientRequestToken"
                 },
                 "FileSystemId": {
                     "documentation": "<p>The ID of the file system that you want to delete.</p>",
                     "shape": "FileSystemId"
                 },
@@ -3853,22 +3857,22 @@
                     "documentation": "<p>An array of one or more DNS aliases that Amazon FSx is attempting to disassociate from the file system.</p>",
                     "shape": "Aliases"
                 }
             },
             "type": "structure"
         },
         "DiskIopsConfiguration": {
-            "documentation": "<p>The SSD IOPS (input/output operations per second) configuration for an Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS file system. The default is 3 IOPS per GB of storage capacity, but you can provision additional IOPS per GB of storage. The configuration consists of the total number of provisioned SSD IOPS and how the amount was provisioned (by the customer or by the system).</p>",
+            "documentation": "<p>The SSD IOPS (input/output operations per second) configuration for an Amazon FSx for NetApp ONTAP or FSx for OpenZFS file system. By default, Amazon FSx automatically provisions 3 IOPS per GB of storage capacity. You can provision additional IOPS per GB of storage. The configuration consists of the total number of provisioned SSD IOPS and how it is was provisioned, or the mode (by the customer or by Amazon FSx).</p>",
             "members": {
                 "Iops": {
                     "documentation": "<p>The total number of SSD IOPS provisioned for the file system.</p>",
                     "shape": "Iops"
                 },
                 "Mode": {
-                    "documentation": "<p>Specifies whether the number of IOPS for the file system is using the system default (<code>AUTOMATIC</code>) or was provisioned by the customer (<code>USER_PROVISIONED</code>).</p>",
+                    "documentation": "<p>Specifies whether the file system is using the <code>AUTOMATIC</code> setting of SSD IOPS of 3 IOPS per GB of storage capacity, , or if it using a <code>USER_PROVISIONED</code> value.</p>",
                     "shape": "DiskIopsConfigurationMode"
                 }
             },
             "type": "structure"
         },
         "DiskIopsConfigurationMode": {
             "enum": [
@@ -4251,15 +4255,15 @@
                     "shape": "OntapFileSystemConfiguration"
                 },
                 "OpenZFSConfiguration": {
                     "documentation": "<p>The configuration for this Amazon FSx for OpenZFS file system.</p>",
                     "shape": "OpenZFSFileSystemConfiguration"
                 },
                 "OwnerId": {
-                    "documentation": "<p>The Amazon Web Services account that created the file system. If the file system was created by an Identity and Access Management (IAM) user, the Amazon Web Services account to which the IAM user belongs is the owner.</p>",
+                    "documentation": "<p>The Amazon Web Services account that created the file system. If the file system was created by a user in IAM Identity Center, the Amazon Web Services account to which the IAM user belongs is the owner.</p>",
                     "shape": "AWSAccountId"
                 },
                 "ResourceARN": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the file system resource.</p>",
                     "shape": "ResourceARN"
                 },
                 "StorageCapacity": {
@@ -5013,21 +5017,25 @@
                     "shape": "OntapDeploymentType"
                 },
                 "DiskIopsConfiguration": {
                     "documentation": "<p>The SSD IOPS configuration for the ONTAP file system, specifying the number of provisioned IOPS and the provision mode.</p>",
                     "shape": "DiskIopsConfiguration"
                 },
                 "EndpointIpAddressRange": {
-                    "documentation": "<p>(Multi-AZ only) The IP address range in which the endpoints to access your file system are created.</p> <important> <p>The Endpoint IP address range you select for your file system must exist outside the VPC's CIDR range and must be at least /30 or larger. If you do not specify this optional parameter, Amazon FSx will automatically select a CIDR block for you.</p> </important>",
+                    "documentation": "<p>(Multi-AZ only) Specifies the IP address range in which the endpoints to access your file system will be created. By default in the Amazon FSx API, Amazon FSx selects an unused IP address range for you from the 198.19.* range. By default in the Amazon FSx console, Amazon FSx chooses the last 64 IP addresses from the VPC\u2019s primary CIDR range to use as the endpoint IP address range for the file system. You can have overlapping endpoint IP addresses for file systems deployed in the same VPC/route tables.</p>",
                     "shape": "IpAddressRange"
                 },
                 "Endpoints": {
                     "documentation": "<p>The <code>Management</code> and <code>Intercluster</code> endpoints that are used to access data or to manage the file system using the NetApp ONTAP CLI, REST API, or NetApp SnapMirror.</p>",
                     "shape": "FileSystemEndpoints"
                 },
+                "FsxAdminPassword": {
+                    "documentation": "<p>You can use the <code>fsxadmin</code> user account to access the NetApp ONTAP CLI and REST API. The password value is always redacted in the response.</p>",
+                    "shape": "AdminPassword"
+                },
                 "PreferredSubnetId": {
                     "shape": "SubnetId"
                 },
                 "RouteTableIds": {
                     "documentation": "<p>(Multi-AZ only) The VPC route tables in which your file system's endpoints are created.</p>",
                     "shape": "RouteTableIds"
                 },
@@ -5382,15 +5390,15 @@
         },
         "PerUnitStorageThroughput": {
             "max": 1000,
             "min": 12,
             "type": "integer"
         },
         "ProgressPercent": {
-            "documentation": "<p>The current percent of progress of an asynchronous task.</p>",
+            "documentation": "<p>Displays the current percent of progress of an asynchronous task.</p>",
             "max": 100,
             "min": 0,
             "type": "integer"
         },
         "ReadOnly": {
             "type": "boolean"
         },
@@ -5625,15 +5633,15 @@
                     "documentation": "<p>The user name for the service account on your self-managed AD domain that FSx uses to join to your AD domain.</p>",
                     "shape": "DirectoryUserName"
                 }
             },
             "type": "structure"
         },
         "SelfManagedActiveDirectoryConfiguration": {
-            "documentation": "<p>The configuration that Amazon FSx uses to join a FSx for Windows File Server file system or an ONTAP storage virtual machine (SVM) to a self-managed (including on-premises) Microsoft Active Directory (AD) directory. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/WindowsGuide/self-managed-AD.html\"> Using Amazon FSx with your self-managed Microsoft Active Directory</a> or <a href=\"https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/managing-svms.html\">Managing SVMs</a>.</p>",
+            "documentation": "<p>The configuration that Amazon FSx uses to join a FSx for Windows File Server file system or an FSx for ONTAP storage virtual machine (SVM) to a self-managed (including on-premises) Microsoft Active Directory (AD) directory. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/WindowsGuide/self-managed-AD.html\"> Using Amazon FSx for Windows with your self-managed Microsoft Active Directory</a> or <a href=\"https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/managing-svms.html\">Managing FSx for ONTAP SVMs</a>.</p>",
             "members": {
                 "DnsIps": {
                     "documentation": "<p>A list of up to three IP addresses of DNS servers or domain controllers in the self-managed AD directory. </p>",
                     "shape": "DnsIps"
                 },
                 "DomainName": {
                     "documentation": "<p>The fully qualified domain name of the self-managed AD directory, such as <code>corp.example.com</code>.</p>",
@@ -5661,26 +5669,38 @@
                 "UserName",
                 "Password",
                 "DnsIps"
             ],
             "type": "structure"
         },
         "SelfManagedActiveDirectoryConfigurationUpdates": {
-            "documentation": "<p>The configuration that Amazon FSx uses to join the Windows File Server instance to a self-managed Microsoft Active Directory (AD) directory.</p>",
+            "documentation": "<p>Specifies changes you are making to the self-managed Microsoft Active Directory (AD) configuration to which an FSx for Windows File Server file system or an FSx for ONTAP SVM is joined.</p>",
             "members": {
                 "DnsIps": {
-                    "documentation": "<p>A list of up to three IP addresses of DNS servers or domain controllers in the self-managed AD directory.</p>",
+                    "documentation": "<p>A list of up to three DNS server or domain controller IP addresses in your self-managed AD domain.</p>",
                     "shape": "DnsIps"
                 },
+                "DomainName": {
+                    "documentation": "<p>Specifies an updated fully qualified domain name of your self-managed AD configuration.</p>",
+                    "shape": "ActiveDirectoryFullyQualifiedName"
+                },
+                "FileSystemAdministratorsGroup": {
+                    "documentation": "<p>Specifies the updated name of the self-managed AD domain group whose members are granted administrative privileges for the Amazon FSx resource.</p>",
+                    "shape": "FileSystemAdministratorsGroupName"
+                },
+                "OrganizationalUnitDistinguishedName": {
+                    "documentation": "<p>Specifies an updated fully qualified distinguished name of the organization unit within your self-managed AD.</p>",
+                    "shape": "OrganizationalUnitDistinguishedName"
+                },
                 "Password": {
-                    "documentation": "<p>The password for the service account on your self-managed AD domain that Amazon FSx will use to join to your AD domain.</p>",
+                    "documentation": "<p>Specifies the updated password for the service account on your self-managed AD domain. Amazon FSx uses this account to join to your self-managed AD domain.</p>",
                     "shape": "DirectoryPassword"
                 },
                 "UserName": {
-                    "documentation": "<p>The user name for the service account on your self-managed AD domain that Amazon FSx will use to join to your AD domain. This account must have the permission to join computers to the domain in the organizational unit provided in <code>OrganizationalUnitDistinguishedName</code>.</p>",
+                    "documentation": "<p>Specifies the updated user name for the service account on your self-managed AD domain. Amazon FSx uses this account to join to your self-managed AD domain.</p> <p>This account must have the permissions required to join computers to the domain in the organizational unit provided in <code>OrganizationalUnitDistinguishedName</code>.</p>",
                     "shape": "DirectoryUserName"
                 }
             },
             "type": "structure"
         },
         "ServiceLimit": {
             "documentation": "<p>The types of limits on your service utilization. Limits include file system count, total throughput capacity, total storage, and total user-initiated backups. These limits apply for a specific account in a specific Amazon Web Services Region. You can increase some of them by contacting Amazon Web Services Support.</p>",
@@ -5873,21 +5893,21 @@
                 "PENDING",
                 "COMPLETED",
                 "UPDATED_OPTIMIZING"
             ],
             "type": "string"
         },
         "StorageCapacity": {
-            "documentation": "<p>The storage capacity for your Amazon FSx file system, in gibibytes.</p>",
+            "documentation": "<p>Specifies the file system's storage capacity, in gibibytes (GiB).</p>",
             "max": 2147483647,
             "min": 0,
             "type": "integer"
         },
         "StorageType": {
-            "documentation": "<p>The storage type for your Amazon FSx file system.</p>",
+            "documentation": "<p>Specifies the file system's storage type.</p>",
             "enum": [
                 "SSD",
                 "HDD"
             ],
             "type": "string"
         },
         "StorageVirtualMachine": {
@@ -6070,18 +6090,18 @@
             },
             "type": "list"
         },
         "SucceededCount": {
             "type": "long"
         },
         "SvmActiveDirectoryConfiguration": {
-            "documentation": "<p>Describes the configuration of the Microsoft Active Directory (AD) directory to which the Amazon FSx for ONTAP storage virtual machine (SVM) is joined. Pleae note, account credentials are not returned in the response payload.</p>",
+            "documentation": "<p>Describes the Microsoft Active Directory (AD) directory configuration to which the FSx for ONTAP storage virtual machine (SVM) is joined. Note that account credentials are not returned in the response payload.</p>",
             "members": {
                 "NetBiosName": {
-                    "documentation": "<p>The NetBIOS name of the Active Directory computer object that is joined to your SVM.</p>",
+                    "documentation": "<p>The NetBIOS name of the AD computer object to which the SVM is joined.</p>",
                     "shape": "NetBiosAlias"
                 },
                 "SelfManagedActiveDirectoryConfiguration": {
                     "shape": "SelfManagedActiveDirectoryAttributes"
                 }
             },
             "type": "structure"
@@ -6342,18 +6362,19 @@
             },
             "type": "structure"
         },
         "UpdateFileSystemLustreConfiguration": {
             "documentation": "<p>The configuration object for Amazon FSx for Lustre file systems used in the <code>UpdateFileSystem</code> operation.</p>",
             "members": {
                 "AutoImportPolicy": {
-                    "documentation": "<p> (Optional) When you create your file system, your existing S3 objects appear as file and directory listings. Use this property to choose how Amazon FSx keeps your file and directory listing up to date as you add or modify objects in your linked S3 bucket. <code>AutoImportPolicy</code> can have the following values:</p> <ul> <li> <p> <code>NONE</code> - (Default) AutoImport is off. Amazon FSx only updates file and directory listings from the linked S3 bucket when the file system is created. FSx does not update the file and directory listing for any new or changed objects after choosing this option.</p> </li> <li> <p> <code>NEW</code> - AutoImport is on. Amazon FSx automatically imports directory listings of any new objects added to the linked S3 bucket that do not currently exist in the FSx file system. </p> </li> <li> <p> <code>NEW_CHANGED</code> - AutoImport is on. Amazon FSx automatically imports file and directory listings of any new objects added to the S3 bucket and any existing objects that are changed in the S3 bucket after you choose this option.</p> </li> <li> <p> <code>NEW_CHANGED_DELETED</code> - AutoImport is on. Amazon FSx automatically imports file and directory listings of any new objects added to the S3 bucket, any existing objects that are changed in the S3 bucket, and any objects that were deleted in the S3 bucket.</p> </li> </ul> <p>The <code>AutoImportPolicy</code> parameter is not supported for Lustre file systems with the <code>Persistent_2</code> deployment type. Instead, use to update a data repository association on your <code>Persistent_2</code> file system.</p>",
+                    "documentation": "<p> (Optional) When you create your file system, your existing S3 objects appear as file and directory listings. Use this property to choose how Amazon FSx keeps your file and directory listing up to date as you add or modify objects in your linked S3 bucket. <code>AutoImportPolicy</code> can have the following values:</p> <ul> <li> <p> <code>NONE</code> - (Default) AutoImport is off. Amazon FSx only updates file and directory listings from the linked S3 bucket when the file system is created. FSx does not update the file and directory listing for any new or changed objects after choosing this option.</p> </li> <li> <p> <code>NEW</code> - AutoImport is on. Amazon FSx automatically imports directory listings of any new objects added to the linked S3 bucket that do not currently exist in the FSx file system. </p> </li> <li> <p> <code>NEW_CHANGED</code> - AutoImport is on. Amazon FSx automatically imports file and directory listings of any new objects added to the S3 bucket and any existing objects that are changed in the S3 bucket after you choose this option.</p> </li> <li> <p> <code>NEW_CHANGED_DELETED</code> - AutoImport is on. Amazon FSx automatically imports file and directory listings of any new objects added to the S3 bucket, any existing objects that are changed in the S3 bucket, and any objects that were deleted in the S3 bucket.</p> </li> </ul> <p>This parameter is not supported for file systems with a data repository association.</p>",
                     "shape": "AutoImportPolicyType"
                 },
                 "AutomaticBackupRetentionDays": {
+                    "documentation": "<p>The number of days to retain automatic backups. Setting this property to <code>0</code> disables automatic backups. You can retain automatic backups for a maximum of 90 days. The default is <code>0</code>.</p>",
                     "shape": "AutomaticBackupRetentionDays"
                 },
                 "DailyAutomaticBackupStartTime": {
                     "shape": "DailyTime"
                 },
                 "DataCompressionType": {
                     "documentation": "<p>Sets the data compression configuration for the file system. <code>DataCompressionType</code> can have the following values:</p> <ul> <li> <p> <code>NONE</code> - Data compression is turned off for the file system.</p> </li> <li> <p> <code>LZ4</code> - Data compression is turned on with the LZ4 algorithm.</p> </li> </ul> <p>If you don't use <code>DataCompressionType</code>, the file system retains its current data compression configuration.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/data-compression.html\">Lustre data compression</a>.</p>",
@@ -6384,27 +6405,27 @@
                 "AutomaticBackupRetentionDays": {
                     "shape": "AutomaticBackupRetentionDays"
                 },
                 "DailyAutomaticBackupStartTime": {
                     "shape": "DailyTime"
                 },
                 "DiskIopsConfiguration": {
-                    "documentation": "<p>The SSD IOPS (input/output operations per second) configuration for an Amazon FSx for NetApp ONTAP file system. The default is 3 IOPS per GB of storage capacity, but you can provision additional IOPS per GB of storage. The configuration consists of an IOPS mode (<code>AUTOMATIC</code> or <code>USER_PROVISIONED</code>), and in the case of <code>USER_PROVISIONED</code> IOPS, the total number of SSD IOPS provisioned.</p>",
+                    "documentation": "<p>The SSD IOPS (input output operations per second) configuration for an Amazon FSx for NetApp ONTAP file system. The default is 3 IOPS per GB of storage capacity, but you can provision additional IOPS per GB of storage. The configuration consists of an IOPS mode (<code>AUTOMATIC</code> or <code>USER_PROVISIONED</code>), and in the case of <code>USER_PROVISIONED</code> IOPS, the total number of SSD IOPS provisioned. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/increase-primary-storage.html\">Updating SSD storage capacity and IOPS</a>.</p>",
                     "shape": "DiskIopsConfiguration"
                 },
                 "FsxAdminPassword": {
-                    "documentation": "<p>The ONTAP administrative password for the <code>fsxadmin</code> user.</p>",
+                    "documentation": "<p>Update the password for the <code>fsxadmin</code> user by entering a new password. You use the <code>fsxadmin</code> user to access the NetApp ONTAP CLI and REST API to manage your file system resources. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/managing-resources-ontap-apps.html\">Managing resources using NetApp Applicaton</a>.</p>",
                     "shape": "AdminPassword"
                 },
                 "RemoveRouteTableIds": {
                     "documentation": "<p>(Multi-AZ only) A list of IDs of existing virtual private cloud (VPC) route tables to disassociate (remove) from your Amazon FSx for NetApp ONTAP file system. You can use the API operation to retrieve the list of VPC route table IDs for a file system.</p>",
                     "shape": "RouteTableIds"
                 },
                 "ThroughputCapacity": {
-                    "documentation": "<p>Specifies the throughput of an FSx for NetApp ONTAP file system, measured in megabytes per second (MBps). Valid values are 128, 256, 512, 1024, 2048, and 4096 MBps.</p>",
+                    "documentation": "<p>Enter a new value to change the amount of throughput capacity for the file system. Throughput capacity is measured in megabytes per second (MBps). Valid values are 128, 256, 512, 1024, 2048, and 4096 MBps. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/managing-throughput-capacity.html\">Managing throughput capacity</a> in the FSx for ONTAP User Guide.</p>",
                     "shape": "MegabytesPerSecond"
                 },
                 "WeeklyMaintenanceStartTime": {
                     "shape": "WeeklyTime"
                 }
             },
             "type": "structure"
@@ -6439,34 +6460,34 @@
             },
             "type": "structure"
         },
         "UpdateFileSystemRequest": {
             "documentation": "<p>The request object for the <code>UpdateFileSystem</code> operation.</p>",
             "members": {
                 "ClientRequestToken": {
-                    "documentation": "<p>A string of up to 64 ASCII characters that Amazon FSx uses to ensure idempotent updates. This string is automatically filled on your behalf when you use the Command Line Interface (CLI) or an Amazon Web Services SDK.</p>",
+                    "documentation": "<p>A string of up to 63 ASCII characters that Amazon FSx uses to ensure idempotent updates. This string is automatically filled on your behalf when you use the Command Line Interface (CLI) or an Amazon Web Services SDK.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientRequestToken"
                 },
                 "FileSystemId": {
                     "documentation": "<p>The ID of the file system that you are updating.</p>",
                     "shape": "FileSystemId"
                 },
                 "LustreConfiguration": {
                     "shape": "UpdateFileSystemLustreConfiguration"
                 },
                 "OntapConfiguration": {
                     "shape": "UpdateFileSystemOntapConfiguration"
                 },
                 "OpenZFSConfiguration": {
-                    "documentation": "<p>The configuration updates for an Amazon FSx for OpenZFS file system.</p>",
+                    "documentation": "<p>The configuration updates for an FSx for OpenZFS file system.</p>",
                     "shape": "UpdateFileSystemOpenZFSConfiguration"
                 },
                 "StorageCapacity": {
-                    "documentation": "<p>Use this parameter to increase the storage capacity of an Amazon FSx for Windows File Server, Amazon FSx for Lustre, or Amazon FSx for NetApp ONTAP file system. Specifies the storage capacity target value, in GiB, to increase the storage capacity for the file system that you're updating. </p> <note> <p>You can't make a storage capacity increase request if there is an existing storage capacity increase request in progress.</p> </note> <p>For Windows file systems, the storage capacity target value must be at least 10 percent greater than the current storage capacity value. To increase storage capacity, the file system must have at least 16 MBps of throughput capacity. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/WindowsGuide/managing-storage-capacity.html\">Managing storage capacity</a> in the <i>Amazon FSx for Windows File Server User Guide</i>.</p> <p>For Lustre file systems, the storage capacity target value can be the following:</p> <ul> <li> <p>For <code>SCRATCH_2</code>, <code>PERSISTENT_1</code>, and <code>PERSISTENT_2 SSD</code> deployment types, valid values are in multiples of 2400 GiB. The value must be greater than the current storage capacity.</p> </li> <li> <p>For <code>PERSISTENT HDD</code> file systems, valid values are multiples of 6000 GiB for 12-MBps throughput per TiB file systems and multiples of 1800 GiB for 40-MBps throughput per TiB file systems. The values must be greater than the current storage capacity.</p> </li> <li> <p>For <code>SCRATCH_1</code> file systems, you can't increase the storage capacity.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/managing-storage-capacity.html\">Managing storage and throughput capacity</a> in the <i>Amazon FSx for Lustre User Guide</i>.</p> <p>For ONTAP file systems, the storage capacity target value must be at least 10 percent greater than the current storage capacity value. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/managing-storage-capacity.html\">Managing storage capacity and provisioned IOPS</a> in the <i>Amazon FSx for NetApp ONTAP User Guide</i>.</p>",
+                    "documentation": "<p>Use this parameter to increase the storage capacity of an FSx for Windows File Server, FSx for Lustre, FSx for OpenZFS, or FSx for ONTAP file system. Specifies the storage capacity target value, in GiB, to increase the storage capacity for the file system that you're updating. </p> <note> <p>You can't make a storage capacity increase request if there is an existing storage capacity increase request in progress.</p> </note> <p>For Lustre file systems, the storage capacity target value can be the following:</p> <ul> <li> <p>For <code>SCRATCH_2</code>, <code>PERSISTENT_1</code>, and <code>PERSISTENT_2 SSD</code> deployment types, valid values are in multiples of 2400 GiB. The value must be greater than the current storage capacity.</p> </li> <li> <p>For <code>PERSISTENT HDD</code> file systems, valid values are multiples of 6000 GiB for 12-MBps throughput per TiB file systems and multiples of 1800 GiB for 40-MBps throughput per TiB file systems. The values must be greater than the current storage capacity.</p> </li> <li> <p>For <code>SCRATCH_1</code> file systems, you can't increase the storage capacity.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/LustreGuide/managing-storage-capacity.html\">Managing storage and throughput capacity</a> in the <i>FSx for Lustre User Guide</i>.</p> <p>For FSx for OpenZFS file systems, the storage capacity target value must be at least 10 percent greater than the current storage capacity value. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/OpenZFSGuide/managing-storage-capacity.html\">Managing storage capacity</a> in the <i>FSx for OpenZFS User Guide</i>.</p> <p>For Windows file systems, the storage capacity target value must be at least 10 percent greater than the current storage capacity value. To increase storage capacity, the file system must have at least 16 MBps of throughput capacity. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/WindowsGuide/managing-storage-capacity.html\">Managing storage capacity</a> in the <i>Amazon FSxfor Windows File Server User Guide</i>.</p> <p>For ONTAP file systems, the storage capacity target value must be at least 10 percent greater than the current storage capacity value. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/managing-storage-capacity.html\">Managing storage capacity and provisioned IOPS</a> in the <i>Amazon FSx for NetApp ONTAP User Guide</i>.</p>",
                     "shape": "StorageCapacity"
                 },
                 "WindowsConfiguration": {
                     "documentation": "<p>The configuration updates for an Amazon FSx for Windows File Server file system.</p>",
                     "shape": "UpdateFileSystemWindowsConfiguration"
                 }
             },
@@ -6489,15 +6510,15 @@
             "documentation": "<p>Updates the configuration for an existing Amazon FSx for Windows File Server file system. Amazon FSx only overwrites existing properties with non-null values provided in the request.</p>",
             "members": {
                 "AuditLogConfiguration": {
                     "documentation": "<p>The configuration that Amazon FSx for Windows File Server uses to audit and log user accesses of files, folders, and file shares on the Amazon FSx for Windows File Server file system..</p>",
                     "shape": "WindowsAuditLogCreateConfiguration"
                 },
                 "AutomaticBackupRetentionDays": {
-                    "documentation": "<p>The number of days to retain automatic daily backups. Setting this to zero (0) disables automatic daily backups. You can retain automatic daily backups for a maximum of 90 days. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/WindowsGuide/using-backups.html#automatic-backups\">Working with Automatic Daily Backups</a>.</p>",
+                    "documentation": "<p>The number of days to retain automatic backups. Setting this property to <code>0</code> disables automatic backups. You can retain automatic backups for a maximum of 90 days. The default is <code>30</code>. For more information, see <a href=\"https://docs.aws.amazon.com/fsx/latest/WindowsGuide/using-backups.html#automatic-backups\">Working with Automatic Daily Backups</a>.</p>",
                     "shape": "AutomaticBackupRetentionDays"
                 },
                 "DailyAutomaticBackupStartTime": {
                     "documentation": "<p>The preferred time to start the daily automatic backup, in the UTC time zone, for example, <code>02:00</code> </p>",
                     "shape": "DailyTime"
                 },
                 "SelfManagedActiveDirectoryConfiguration": {
@@ -6612,27 +6633,27 @@
                 }
             },
             "type": "structure"
         },
         "UpdateStorageVirtualMachineRequest": {
             "members": {
                 "ActiveDirectoryConfiguration": {
-                    "documentation": "<p>Updates the Microsoft Active Directory (AD) configuration for an SVM that is joined to an AD.</p>",
+                    "documentation": "<p>Specifies updates to an SVM's Microsoft Active Directory (AD) configuration.</p>",
                     "shape": "UpdateSvmActiveDirectoryConfiguration"
                 },
                 "ClientRequestToken": {
                     "idempotencyToken": true,
                     "shape": "ClientRequestToken"
                 },
                 "StorageVirtualMachineId": {
                     "documentation": "<p>The ID of the SVM that you want to update, in the format <code>svm-0123456789abcdef0</code>.</p>",
                     "shape": "StorageVirtualMachineId"
                 },
                 "SvmAdminPassword": {
-                    "documentation": "<p>Enter a new SvmAdminPassword if you are updating it.</p>",
+                    "documentation": "<p>Specifies a new SvmAdminPassword.</p>",
                     "shape": "AdminPassword"
                 }
             },
             "required": [
                 "StorageVirtualMachineId"
             ],
             "type": "structure"
@@ -6642,16 +6663,20 @@
                 "StorageVirtualMachine": {
                     "shape": "StorageVirtualMachine"
                 }
             },
             "type": "structure"
         },
         "UpdateSvmActiveDirectoryConfiguration": {
-            "documentation": "<p>Updates the Microsoft Active Directory (AD) configuration of an SVM joined to an AD. Please note, account credentials are not returned in the response payload.</p>",
+            "documentation": "<p>Specifies updates to an FSx for ONTAP storage virtual machine's (SVM) Microsoft Active Directory (AD) configuration. Note that account credentials are not returned in the response payload.</p>",
             "members": {
+                "NetBiosName": {
+                    "documentation": "<p>Specifies an updated NetBIOS name of the AD computer object <code>NetBiosName</code> to which an SVM is joined.</p>",
+                    "shape": "NetBiosAlias"
+                },
                 "SelfManagedActiveDirectoryConfiguration": {
                     "shape": "SelfManagedActiveDirectoryConfigurationUpdates"
                 }
             },
             "type": "structure"
         },
         "UpdateVolumeRequest": {
```

### Comparing `botocore-a-la-carte-fsx-1.29.99/botocore_a_la_carte_fsx.egg-info/PKG-INFO` & `botocore-a-la-carte-fsx-1.30.0/botocore_a_la_carte_fsx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-fsx
-Version: 1.29.99
+Version: 1.30.0
 Summary: fsx data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-fsx-1.29.99/setup.py` & `botocore-a-la-carte-fsx-1.30.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-fsx',
-    version="1.29.99",
+    version="1.30.0",
     description='fsx data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/fsx/*/*.json'],
```

