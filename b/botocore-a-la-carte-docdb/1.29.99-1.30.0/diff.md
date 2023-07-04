# Comparing `tmp/botocore-a-la-carte-docdb-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-docdb-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-docdb-1.29.99.tar", last modified: Sat Mar 25 01:22:35 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-docdb-1.30.0.tar", last modified: Tue Jul  4 01:44:25 2023, max compression
```

## Comparing `botocore-a-la-carte-docdb-1.29.99.tar` & `botocore-a-la-carte-docdb-1.30.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.203075 botocore-a-la-carte-docdb-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:34.000000 botocore-a-la-carte-docdb-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-25 01:22:35.203075 botocore-a-la-carte-docdb-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.203075 botocore-a-la-carte-docdb-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.203075 botocore-a-la-carte-docdb-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.203075 botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.203075 botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/2014-10-31/
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-03-25 01:22:12.000000 botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/2014-10-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/2014-10-31/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-25 01:22:12.000000 botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/2014-10-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   230092 2023-03-25 01:22:12.000000 botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/2014-10-31/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-25 01:22:12.000000 botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/2014-10-31/service-2.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-03-25 01:22:12.000000 botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/2014-10-31/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:35.203075 botocore-a-la-carte-docdb-1.29.99/botocore_a_la_carte_docdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-25 01:22:35.000000 botocore-a-la-carte-docdb-1.29.99/botocore_a_la_carte_docdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-25 01:22:35.000000 botocore-a-la-carte-docdb-1.29.99/botocore_a_la_carte_docdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:35.000000 botocore-a-la-carte-docdb-1.29.99/botocore_a_la_carte_docdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:35.000000 botocore-a-la-carte-docdb-1.29.99/botocore_a_la_carte_docdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:35.203075 botocore-a-la-carte-docdb-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-25 01:22:34.000000 botocore-a-la-carte-docdb-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:25.862501 botocore-a-la-carte-docdb-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:25.000000 botocore-a-la-carte-docdb-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-04 01:44:25.862501 botocore-a-la-carte-docdb-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:25.858501 botocore-a-la-carte-docdb-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:25.858501 botocore-a-la-carte-docdb-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:25.858501 botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:25.862501 botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/2014-10-31/
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-04 01:44:02.000000 botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/2014-10-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/2014-10-31/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-04 01:44:02.000000 botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/2014-10-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   230813 2023-07-04 01:44:02.000000 botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/2014-10-31/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-04 01:44:02.000000 botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/2014-10-31/service-2.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-04 01:44:02.000000 botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/2014-10-31/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:25.862501 botocore-a-la-carte-docdb-1.30.0/botocore_a_la_carte_docdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-04 01:44:25.000000 botocore-a-la-carte-docdb-1.30.0/botocore_a_la_carte_docdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-04 01:44:25.000000 botocore-a-la-carte-docdb-1.30.0/botocore_a_la_carte_docdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:25.000000 botocore-a-la-carte-docdb-1.30.0/botocore_a_la_carte_docdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:25.000000 botocore-a-la-carte-docdb-1.30.0/botocore_a_la_carte_docdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:25.862501 botocore-a-la-carte-docdb-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-04 01:44:25.000000 botocore-a-la-carte-docdb-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-docdb-1.29.99/LICENSE.txt` & `botocore-a-la-carte-docdb-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-docdb-1.29.99/PKG-INFO` & `botocore-a-la-carte-docdb-1.30.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-docdb
-Version: 1.29.99
+Version: 1.30.0
 Summary: docdb data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/2014-10-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/2014-10-31/endpoint-rule-set-1.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8977382330246914%*

 * *Differences: {"'rules'": "{0: {'conditions': {0: {'fn': 'isSet', 'argv': {0: {'ref': 'Endpoint'}}, delete: "*

 * *            "['assign']}}, 'rules': {0: {'type': 'error', 'error': 'Invalid Configuration: FIPS "*

 * *            "and custom endpoint are not supported', delete: ['rules']}, 1: {'conditions': [], "*

 * *            "'rules': {0: {'conditions': {0: {'argv': {insert: [(0, OrderedDict([('ref', "*

 * *            "'UseDualStack')]))], delete: [1]}}}, 'type': 'error', 'error': 'Invalid "*

 * *            "Configuration: Dualstack and c […]*

```diff
@@ -29,407 +29,347 @@
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
-                                        "url": "https://rds-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                                        "rds.ca-central-1"
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
-                                                "url": "https://rds-fips.ca-central-1.amazonaws.com"
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
-                                                        "rds.us-east-1"
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
-                                                "url": "https://rds-fips.us-east-1.amazonaws.com"
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
-                                                        "rds.us-east-2"
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://rds-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                                "url": "https://rds-fips.us-east-2.amazonaws.com"
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
-                                                        "rds.us-west-1"
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
-                                                "url": "https://rds-fips.us-west-1.amazonaws.com"
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
+                                                            "conditions": [
+                                                                {
+                                                                    "argv": [
+                                                                        "aws-us-gov",
+                                                                        {
+                                                                            "argv": [
+                                                                                {
+                                                                                    "ref": "PartitionResult"
+                                                                                },
+                                                                                "name"
+                                                                            ],
+                                                                            "fn": "getAttr"
+                                                                        }
+                                                                    ],
+                                                                    "fn": "stringEquals"
+                                                                }
+                                                            ],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://rds.{Region}.amazonaws.com"
+                                                            },
+                                                            "type": "endpoint"
                                                         },
-                                                        "rds.us-west-2"
+                                                        {
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://rds-fips.{Region}.{PartitionResult#dnsSuffix}"
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
-                                                "url": "https://rds-fips.us-west-2.amazonaws.com"
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
-                                                        "aws-us-gov",
+                                                        true,
                                                         {
                                                             "argv": [
                                                                 {
                                                                     "ref": "PartitionResult"
                                                                 },
-                                                                "name"
+                                                                "supportsDualStack"
                                                             ],
                                                             "fn": "getAttr"
                                                         }
                                                     ],
-                                                    "fn": "stringEquals"
+                                                    "fn": "booleanEquals"
                                                 }
                                             ],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://rds.{Region}.{PartitionResult#dnsSuffix}"
-                                            },
-                                            "type": "endpoint"
+                                            "rules": [
+                                                {
+                                                    "conditions": [],
+                                                    "rules": [
+                                                        {
+                                                            "conditions": [],
+                                                            "endpoint": {
+                                                                "headers": {},
+                                                                "properties": {},
+                                                                "url": "https://rds.{Region}.{PartitionResult#dualStackDnsSuffix}"
+                                                            },
+                                                            "type": "endpoint"
+                                                        }
+                                                    ],
+                                                    "type": "tree"
+                                                }
+                                            ],
+                                            "type": "tree"
                                         },
                                         {
                                             "conditions": [],
-                                            "endpoint": {
-                                                "headers": {},
-                                                "properties": {},
-                                                "url": "https://rds-fips.{Region}.{PartitionResult#dnsSuffix}"
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
+                                                "url": "https://rds.{Region}.{PartitionResult#dnsSuffix}"
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
-                                        "url": "https://rds.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                        "url": "https://rds.{Region}.{PartitionResult#dnsSuffix}"
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

### Comparing `botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/2014-10-31/paginators-1.json` & `botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/2014-10-31/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/2014-10-31/service-2.json` & `botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/2014-10-31/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999997355938994%*

 * *Differences: {"'shapes'": "{'GlobalCluster': {'members': {'GlobalClusterResourceId': {'documentation': '<p>The "*

 * *             'Amazon Web Services Region-unique, immutable identifier for the global database '*

 * *             'cluster. This identifier is found in CloudTrail log entries whenever the KMS '*

 * *             "customer master key (CMK) for the cluster is accessed. </p>'}}}, "*

 * *             "'RestoreDBClusterFromSnapshotMessage': {'members': {'DBClusterParameterGroupName': "*

 * *             "OrderedDict([('shape', 'Strin […]*

```diff
@@ -3898,15 +3898,15 @@
                     "shape": "GlobalClusterIdentifier"
                 },
                 "GlobalClusterMembers": {
                     "documentation": "<p>The list of cluster IDs for secondary clusters within the global cluster. Currently limited to one item. </p>",
                     "shape": "GlobalClusterMemberList"
                 },
                 "GlobalClusterResourceId": {
-                    "documentation": "<p>The Amazon Web Services Region-unique, immutable identifier for the global database cluster. This identifier is found in AWS CloudTrail log entries whenever the AWS KMS customer master key (CMK) for the cluster is accessed. </p>",
+                    "documentation": "<p>The Amazon Web Services Region-unique, immutable identifier for the global database cluster. This identifier is found in CloudTrail log entries whenever the KMS customer master key (CMK) for the cluster is accessed. </p>",
                     "shape": "String"
                 },
                 "Status": {
                     "documentation": "<p>Specifies the current state of this global cluster.</p>",
                     "shape": "String"
                 },
                 "StorageEncrypted": {
@@ -4914,14 +4914,18 @@
                     "documentation": "<p>Provides the list of Amazon EC2 Availability Zones that instances in the restored DB cluster can be created in.</p>",
                     "shape": "AvailabilityZones"
                 },
                 "DBClusterIdentifier": {
                     "documentation": "<p>The name of the cluster to create from the snapshot or cluster snapshot. This parameter isn't case sensitive.</p> <p>Constraints:</p> <ul> <li> <p>Must contain from 1 to 63 letters, numbers, or hyphens.</p> </li> <li> <p>The first character must be a letter.</p> </li> <li> <p>Cannot end with a hyphen or contain two consecutive hyphens.</p> </li> </ul> <p>Example: <code>my-snapshot-id</code> </p>",
                     "shape": "String"
                 },
+                "DBClusterParameterGroupName": {
+                    "documentation": "<p>The name of the DB cluster parameter group to associate with this DB cluster.</p> <p> <i>Type:</i> String. \u00a0 \u00a0 \u00a0 <i>Required:</i> No.</p> <p>If this argument is omitted, the default DB cluster parameter group is used. If supplied, must match the name of an existing default DB cluster parameter group. The string must consist of from 1 to 255 letters, numbers or hyphens. Its first character must be a letter, and it cannot end with a hyphen or contain two consecutive hyphens.</p>",
+                    "shape": "String"
+                },
                 "DBSubnetGroupName": {
                     "documentation": "<p>The name of the subnet group to use for the new cluster.</p> <p>Constraints: If provided, must match the name of an existing <code>DBSubnetGroup</code>.</p> <p>Example: <code>mySubnetgroup</code> </p>",
                     "shape": "String"
                 },
                 "DeletionProtection": {
                     "documentation": "<p>Specifies whether this cluster can be deleted. If <code>DeletionProtection</code> is enabled, the cluster cannot be deleted unless it is modified and <code>DeletionProtection</code> is disabled. <code>DeletionProtection</code> protects clusters from being accidentally deleted.</p>",
                     "shape": "BooleanOptional"
@@ -5002,15 +5006,15 @@
                     "shape": "IntegerOptional"
                 },
                 "RestoreToTime": {
                     "documentation": "<p>The date and time to restore the cluster to.</p> <p>Valid values: A time in Universal Coordinated Time (UTC) format.</p> <p>Constraints:</p> <ul> <li> <p>Must be before the latest restorable time for the instance.</p> </li> <li> <p>Must be specified if the <code>UseLatestRestorableTime</code> parameter is not provided.</p> </li> <li> <p>Cannot be specified if the <code>UseLatestRestorableTime</code> parameter is <code>true</code>.</p> </li> <li> <p>Cannot be specified if the <code>RestoreType</code> parameter is <code>copy-on-write</code>.</p> </li> </ul> <p>Example: <code>2015-03-07T23:45:00Z</code> </p>",
                     "shape": "TStamp"
                 },
                 "RestoreType": {
-                    "documentation": "<p>The type of restore to be performed. You can specify one of the following values:</p> <ul> <li> <p> <code>full-copy</code> - The new DB cluster is restored as a full copy of the source DB cluster.</p> </li> <li> <p> <code>copy-on-write</code> - The new DB cluster is restored as a clone of the source DB cluster.</p> </li> </ul> <p>If you don't specify a <code>RestoreType</code> value, then the new DB cluster is restored as a full copy of the source DB cluster.</p>",
+                    "documentation": "<p>The type of restore to be performed. You can specify one of the following values:</p> <ul> <li> <p> <code>full-copy</code> - The new DB cluster is restored as a full copy of the source DB cluster.</p> </li> <li> <p> <code>copy-on-write</code> - The new DB cluster is restored as a clone of the source DB cluster.</p> </li> </ul> <p>Constraints: You can't specify <code>copy-on-write</code> if the engine version of the source DB cluster is earlier than 1.11.</p> <p>If you don't specify a <code>RestoreType</code> value, then the new DB cluster is restored as a full copy of the source DB cluster.</p>",
                     "shape": "String"
                 },
                 "SourceDBClusterIdentifier": {
                     "documentation": "<p>The identifier of the source cluster from which to restore.</p> <p>Constraints:</p> <ul> <li> <p>Must match the identifier of an existing <code>DBCluster</code>.</p> </li> </ul>",
                     "shape": "String"
                 },
                 "Tags": {
```

### Comparing `botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/2014-10-31/service-2.sdk-extras.json` & `botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/2014-10-31/service-2.sdk-extras.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-docdb-1.29.99/botocore/data/docdb/2014-10-31/waiters-2.json` & `botocore-a-la-carte-docdb-1.30.0/botocore/data/docdb/2014-10-31/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-docdb-1.29.99/botocore_a_la_carte_docdb.egg-info/PKG-INFO` & `botocore-a-la-carte-docdb-1.30.0/botocore_a_la_carte_docdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-docdb
-Version: 1.29.99
+Version: 1.30.0
 Summary: docdb data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-docdb-1.29.99/botocore_a_la_carte_docdb.egg-info/SOURCES.txt` & `botocore-a-la-carte-docdb-1.30.0/botocore_a_la_carte_docdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-docdb-1.29.99/setup.py` & `botocore-a-la-carte-docdb-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-docdb',
-    version="1.29.99",
+    version="1.30.0",
     description='docdb data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/docdb/*/*.json'],
```

