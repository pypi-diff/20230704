# Comparing `tmp/botocore-a-la-carte-ecr-public-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-ecr-public-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ecr-public-1.29.99.tar", last modified: Sat Mar 25 01:22:39 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-ecr-public-1.30.0.tar", last modified: Tue Jul  4 01:44:30 2023, max compression
```

## Comparing `botocore-a-la-carte-ecr-public-1.29.99.tar` & `botocore-a-la-carte-ecr-public-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:39.459361 botocore-a-la-carte-ecr-public-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:39.000000 botocore-a-la-carte-ecr-public-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-25 01:22:39.459361 botocore-a-la-carte-ecr-public-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:39.459361 botocore-a-la-carte-ecr-public-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:39.459361 botocore-a-la-carte-ecr-public-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:39.459361 botocore-a-la-carte-ecr-public-1.29.99/botocore/data/ecr-public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:39.459361 botocore-a-la-carte-ecr-public-1.29.99/botocore/data/ecr-public/2020-10-30/
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-03-25 01:22:12.000000 botocore-a-la-carte-ecr-public-1.29.99/botocore/data/ecr-public/2020-10-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-ecr-public-1.29.99/botocore/data/ecr-public/2020-10-30/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-25 01:22:12.000000 botocore-a-la-carte-ecr-public-1.29.99/botocore/data/ecr-public/2020-10-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    83616 2023-03-25 01:22:12.000000 botocore-a-la-carte-ecr-public-1.29.99/botocore/data/ecr-public/2020-10-30/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:39.459361 botocore-a-la-carte-ecr-public-1.29.99/botocore_a_la_carte_ecr_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-25 01:22:39.000000 botocore-a-la-carte-ecr-public-1.29.99/botocore_a_la_carte_ecr_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-25 01:22:39.000000 botocore-a-la-carte-ecr-public-1.29.99/botocore_a_la_carte_ecr_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:39.000000 botocore-a-la-carte-ecr-public-1.29.99/botocore_a_la_carte_ecr_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:39.000000 botocore-a-la-carte-ecr-public-1.29.99/botocore_a_la_carte_ecr_public.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:39.459361 botocore-a-la-carte-ecr-public-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-25 01:22:39.000000 botocore-a-la-carte-ecr-public-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.222546 botocore-a-la-carte-ecr-public-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:29.000000 botocore-a-la-carte-ecr-public-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-04 01:44:30.222546 botocore-a-la-carte-ecr-public-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.218546 botocore-a-la-carte-ecr-public-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.218546 botocore-a-la-carte-ecr-public-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.218546 botocore-a-la-carte-ecr-public-1.30.0/botocore/data/ecr-public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.222546 botocore-a-la-carte-ecr-public-1.30.0/botocore/data/ecr-public/2020-10-30/
+-rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-07-04 01:44:02.000000 botocore-a-la-carte-ecr-public-1.30.0/botocore/data/ecr-public/2020-10-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-ecr-public-1.30.0/botocore/data/ecr-public/2020-10-30/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-04 01:44:02.000000 botocore-a-la-carte-ecr-public-1.30.0/botocore/data/ecr-public/2020-10-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    83643 2023-07-04 01:44:02.000000 botocore-a-la-carte-ecr-public-1.30.0/botocore/data/ecr-public/2020-10-30/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.222546 botocore-a-la-carte-ecr-public-1.30.0/botocore_a_la_carte_ecr_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-04 01:44:30.000000 botocore-a-la-carte-ecr-public-1.30.0/botocore_a_la_carte_ecr_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-04 01:44:30.000000 botocore-a-la-carte-ecr-public-1.30.0/botocore_a_la_carte_ecr_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:30.000000 botocore-a-la-carte-ecr-public-1.30.0/botocore_a_la_carte_ecr_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:30.000000 botocore-a-la-carte-ecr-public-1.30.0/botocore_a_la_carte_ecr_public.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:30.222546 botocore-a-la-carte-ecr-public-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-04 01:44:29.000000 botocore-a-la-carte-ecr-public-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-ecr-public-1.29.99/LICENSE.txt` & `botocore-a-la-carte-ecr-public-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecr-public-1.29.99/PKG-INFO` & `botocore-a-la-carte-ecr-public-1.30.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ecr-public
-Version: 1.29.99
+Version: 1.30.0
 Summary: ecr-public data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ecr-public-1.29.99/botocore/data/ecr-public/2020-10-30/endpoint-rule-set-1.json` & `botocore-a-la-carte-ecr-public-1.30.0/botocore/data/ecr-public/2020-10-30/endpoint-rule-set-1.json`

 * *Files 22% similar despite different names*

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
@@ -29,281 +29,322 @@
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
+                                                                "url": "https://api.ecr-public-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                        "url": "https://api.ecr-public-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                    "endpoint": {
-                                        "headers": {},
-                                        "properties": {},
-                                        "url": "https://api.ecr-public-fips.{Region}.{PartitionResult#dnsSuffix}"
-                                    },
-                                    "type": "endpoint"
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
+                                                                "url": "https://api.ecr-public-fips.{Region}.{PartitionResult#dnsSuffix}"
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
+                                            "error": "FIPS is enabled but this partition does not support FIPS",
+                                            "type": "error"
+                                        }
+                                    ],
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
+                                                                "url": "https://api.ecr-public.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                        "url": "https://api.ecr-public.{Region}.{PartitionResult#dualStackDnsSuffix}"
-                                    },
-                                    "type": "endpoint"
+                                    "rules": [
+                                        {
+                                            "conditions": [],
+                                            "endpoint": {
+                                                "headers": {},
+                                                "properties": {},
+                                                "url": "https://api.ecr-public.{Region}.{PartitionResult#dnsSuffix}"
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
-                        "url": "https://api.ecr-public.{Region}.{PartitionResult#dnsSuffix}"
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

### Comparing `botocore-a-la-carte-ecr-public-1.29.99/botocore/data/ecr-public/2020-10-30/paginators-1.json` & `botocore-a-la-carte-ecr-public-1.30.0/botocore/data/ecr-public/2020-10-30/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecr-public-1.29.99/botocore/data/ecr-public/2020-10-30/service-2.json` & `botocore-a-la-carte-ecr-public-1.30.0/botocore/data/ecr-public/2020-10-30/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999953392990306%*

 * *Differences: {"'shapes'": "{'BatchDeleteImageRequest': {'members': {'registryId': {'shape': "*

 * *             '\'RegistryIdOrAlias\', \'documentation\': "<p>The Amazon Web Services account ID, or '*

 * *             "registry alias, that's associated with the registry that contains the image to "*

 * *             'delete. If you do not specify a registry, the default public registry is '*

 * *             'assumed.</p>"}}}}'}*

```diff
@@ -814,16 +814,16 @@
         "BatchDeleteImageRequest": {
             "members": {
                 "imageIds": {
                     "documentation": "<p>A list of image ID references that correspond to images to delete. The format of the <code>imageIds</code> reference is <code>imageTag=tag</code> or <code>imageDigest=digest</code>.</p>",
                     "shape": "ImageIdentifierList"
                 },
                 "registryId": {
-                    "documentation": "<p>The Amazon Web Services account ID that's associated with the registry that contains the image to delete. If you do not specify a registry, the default public registry is assumed.</p>",
-                    "shape": "RegistryId"
+                    "documentation": "<p>The Amazon Web Services account ID, or registry alias, that's associated with the registry that contains the image to delete. If you do not specify a registry, the default public registry is assumed.</p>",
+                    "shape": "RegistryIdOrAlias"
                 },
                 "repositoryName": {
                     "documentation": "<p>The repository in a public registry that contains the image to delete.</p>",
                     "shape": "RepositoryName"
                 }
             },
             "required": [
```

### Comparing `botocore-a-la-carte-ecr-public-1.29.99/botocore_a_la_carte_ecr_public.egg-info/PKG-INFO` & `botocore-a-la-carte-ecr-public-1.30.0/botocore_a_la_carte_ecr_public.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ecr-public
-Version: 1.29.99
+Version: 1.30.0
 Summary: ecr-public data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ecr-public-1.29.99/setup.py` & `botocore-a-la-carte-ecr-public-1.30.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ecr-public',
-    version="1.29.99",
+    version="1.30.0",
     description='ecr-public data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ecr-public/*/*.json'],
```

