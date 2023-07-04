# Comparing `tmp/botocore-a-la-carte-ssm-incidents-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-ssm-incidents-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ssm-incidents-1.29.99.tar", last modified: Sat Mar 25 01:23:07 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-ssm-incidents-1.30.0.tar", last modified: Tue Jul  4 01:44:58 2023, max compression
```

## Comparing `botocore-a-la-carte-ssm-incidents-1.29.99.tar` & `botocore-a-la-carte-ssm-incidents-1.30.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:07.024984 botocore-a-la-carte-ssm-incidents-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:06.000000 botocore-a-la-carte-ssm-incidents-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-25 01:23:07.024984 botocore-a-la-carte-ssm-incidents-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:07.024984 botocore-a-la-carte-ssm-incidents-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:07.024984 botocore-a-la-carte-ssm-incidents-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:07.024984 botocore-a-la-carte-ssm-incidents-1.29.99/botocore/data/ssm-incidents/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:07.024984 botocore-a-la-carte-ssm-incidents-1.29.99/botocore/data/ssm-incidents/2018-05-10/
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-03-25 01:22:12.000000 botocore-a-la-carte-ssm-incidents-1.29.99/botocore/data/ssm-incidents/2018-05-10/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-ssm-incidents-1.29.99/botocore/data/ssm-incidents/2018-05-10/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-25 01:22:12.000000 botocore-a-la-carte-ssm-incidents-1.29.99/botocore/data/ssm-incidents/2018-05-10/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    98167 2023-03-25 01:22:12.000000 botocore-a-la-carte-ssm-incidents-1.29.99/botocore/data/ssm-incidents/2018-05-10/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-25 01:22:12.000000 botocore-a-la-carte-ssm-incidents-1.29.99/botocore/data/ssm-incidents/2018-05-10/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:07.024984 botocore-a-la-carte-ssm-incidents-1.29.99/botocore_a_la_carte_ssm_incidents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-25 01:23:06.000000 botocore-a-la-carte-ssm-incidents-1.29.99/botocore_a_la_carte_ssm_incidents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-25 01:23:06.000000 botocore-a-la-carte-ssm-incidents-1.29.99/botocore_a_la_carte_ssm_incidents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:06.000000 botocore-a-la-carte-ssm-incidents-1.29.99/botocore_a_la_carte_ssm_incidents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:06.000000 botocore-a-la-carte-ssm-incidents-1.29.99/botocore_a_la_carte_ssm_incidents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:07.024984 botocore-a-la-carte-ssm-incidents-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-25 01:23:06.000000 botocore-a-la-carte-ssm-incidents-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.850817 botocore-a-la-carte-ssm-incidents-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:58.000000 botocore-a-la-carte-ssm-incidents-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-04 01:44:58.850817 botocore-a-la-carte-ssm-incidents-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.850817 botocore-a-la-carte-ssm-incidents-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.850817 botocore-a-la-carte-ssm-incidents-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.850817 botocore-a-la-carte-ssm-incidents-1.30.0/botocore/data/ssm-incidents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.850817 botocore-a-la-carte-ssm-incidents-1.30.0/botocore/data/ssm-incidents/2018-05-10/
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-04 01:44:02.000000 botocore-a-la-carte-ssm-incidents-1.30.0/botocore/data/ssm-incidents/2018-05-10/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-ssm-incidents-1.30.0/botocore/data/ssm-incidents/2018-05-10/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-04 01:44:02.000000 botocore-a-la-carte-ssm-incidents-1.30.0/botocore/data/ssm-incidents/2018-05-10/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    98191 2023-07-04 01:44:02.000000 botocore-a-la-carte-ssm-incidents-1.30.0/botocore/data/ssm-incidents/2018-05-10/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-04 01:44:02.000000 botocore-a-la-carte-ssm-incidents-1.30.0/botocore/data/ssm-incidents/2018-05-10/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:58.850817 botocore-a-la-carte-ssm-incidents-1.30.0/botocore_a_la_carte_ssm_incidents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-04 01:44:58.000000 botocore-a-la-carte-ssm-incidents-1.30.0/botocore_a_la_carte_ssm_incidents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-04 01:44:58.000000 botocore-a-la-carte-ssm-incidents-1.30.0/botocore_a_la_carte_ssm_incidents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:58.000000 botocore-a-la-carte-ssm-incidents-1.30.0/botocore_a_la_carte_ssm_incidents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:58.000000 botocore-a-la-carte-ssm-incidents-1.30.0/botocore_a_la_carte_ssm_incidents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:58.850817 botocore-a-la-carte-ssm-incidents-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-04 01:44:58.000000 botocore-a-la-carte-ssm-incidents-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-ssm-incidents-1.29.99/LICENSE.txt` & `botocore-a-la-carte-ssm-incidents-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ssm-incidents-1.29.99/PKG-INFO` & `botocore-a-la-carte-ssm-incidents-1.30.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ssm-incidents
-Version: 1.29.99
+Version: 1.30.0
 Summary: ssm-incidents data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ssm-incidents-1.29.99/botocore/data/ssm-incidents/2018-05-10/endpoint-rule-set-1.json` & `botocore-a-la-carte-ssm-incidents-1.30.0/botocore/data/ssm-incidents/2018-05-10/endpoint-rule-set-1.json`

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
+                                                                "url": "https://ssm-incidents-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                        "url": "https://ssm-incidents-fips.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
+                                                                "url": "https://ssm-incidents-fips.{Region}.{PartitionResult#dnsSuffix}"
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
-                                                "url": "https://ssm-incidents-fips.{Region}.{PartitionResult#dnsSuffix}"
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
+                                                                "url": "https://ssm-incidents.{Region}.{PartitionResult#dualStackDnsSuffix}"
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
-                                        "url": "https://ssm-incidents.{Region}.{PartitionResult#dualStackDnsSuffix}"
-                                    },
-                                    "type": "endpoint"
+                                    "rules": [
+                                        {
+                                            "conditions": [],
+                                            "endpoint": {
+                                                "headers": {},
+                                                "properties": {},
+                                                "url": "https://ssm-incidents.{Region}.{PartitionResult#dnsSuffix}"
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
-                        "url": "https://ssm-incidents.{Region}.{PartitionResult#dnsSuffix}"
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

### Comparing `botocore-a-la-carte-ssm-incidents-1.29.99/botocore/data/ssm-incidents/2018-05-10/paginators-1.json` & `botocore-a-la-carte-ssm-incidents-1.30.0/botocore/data/ssm-incidents/2018-05-10/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ssm-incidents-1.29.99/botocore/data/ssm-incidents/2018-05-10/service-2.json` & `botocore-a-la-carte-ssm-incidents-1.30.0/botocore/data/ssm-incidents/2018-05-10/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997612098898468%*

 * *Differences: {"'operations'": "{'CreateTimelineEvent': {'documentation': '<p>Creates a custom timeline event on "*

 * *                 'the incident details page of an incident record. Incident Manager automatically '*

 * *                 'creates timeline events that mark key moments during an incident. You can create '*

 * *                 'custom timeline events to mark important events that Incident Manager can detect '*

 * *                 "automatically.</p>'}}",*

 * * "'shapes'": "{'CreateTimelineEventInput': {'members': {'clientToke […]*

```diff
@@ -81,15 +81,15 @@
             },
             "name": "CreateResponsePlan",
             "output": {
                 "shape": "CreateResponsePlanOutput"
             }
         },
         "CreateTimelineEvent": {
-            "documentation": "<p>Creates a custom timeline event on the incident details page of an incident record. Timeline events are automatically created by Incident Manager, marking key moment during an incident. You can create custom timeline events to mark important events that are automatically detected by Incident Manager.</p>",
+            "documentation": "<p>Creates a custom timeline event on the incident details page of an incident record. Incident Manager automatically creates timeline events that mark key moments during an incident. You can create custom timeline events to mark important events that Incident Manager can detect automatically.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -1229,36 +1229,36 @@
                 "arn"
             ],
             "type": "structure"
         },
         "CreateTimelineEventInput": {
             "members": {
                 "clientToken": {
-                    "documentation": "<p>A token ensuring that the action is called only once with the specified details.</p>",
+                    "documentation": "<p>A token that ensures that a client calls the action only once with the specified details.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientToken"
                 },
                 "eventData": {
                     "documentation": "<p>A short description of the event.</p>",
                     "shape": "EventData"
                 },
                 "eventReferences": {
-                    "documentation": "<p>Adds one or more references to the <code>TimelineEvent</code>. A reference can be an Amazon Web Services resource involved in the incident or in some way associated with it. When you specify a reference, you enter the Amazon Resource Name (ARN) of the resource. You can also specify a related item. As an example, you could specify the ARN of an Amazon DynamoDB (DynamoDB) table. The table for this example is the resource. You could also specify a Amazon CloudWatch metric for that table. The metric is the related item.</p>",
+                    "documentation": "<p>Adds one or more references to the <code>TimelineEvent</code>. A reference is an Amazon Web Services resource involved or associated with the incident. To specify a reference, enter its Amazon Resource Name (ARN). You can also specify a related item associated with a resource. For example, to specify an Amazon DynamoDB (DynamoDB) table as a resource, use the table's ARN. You can also specify an Amazon CloudWatch metric associated with the DynamoDB table as a related item.</p>",
                     "shape": "EventReferenceList"
                 },
                 "eventTime": {
                     "documentation": "<p>The time that the event occurred.</p>",
                     "shape": "Timestamp"
                 },
                 "eventType": {
-                    "documentation": "<p>The type of the event. You can create timeline events of type <code>Custom Event</code>.</p>",
+                    "documentation": "<p>The type of event. You can create timeline events of type <code>Custom Event</code>.</p>",
                     "shape": "TimelineEventType"
                 },
                 "incidentRecordArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the incident record to which the event will be added.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the incident record that the action adds the incident to.</p>",
                     "shape": "Arn"
                 }
             },
             "required": [
                 "eventData",
                 "eventTime",
                 "eventType",
@@ -1371,15 +1371,15 @@
         "DeleteResponsePlanOutput": {
             "members": {},
             "type": "structure"
         },
         "DeleteTimelineEventInput": {
             "members": {
                 "eventId": {
-                    "documentation": "<p>The ID of the event you are updating. You can find this by using <code>ListTimelineEvents</code>.</p>",
+                    "documentation": "<p>The ID of the event to update. You can use <code>ListTimelineEvents</code> to find an event's ID.</p>",
                     "shape": "UUID"
                 },
                 "incidentRecordArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the incident that includes the timeline event.</p>",
                     "shape": "Arn"
                 }
             },
@@ -1889,15 +1889,15 @@
         },
         "IncidentSource": {
             "max": 50,
             "min": 0,
             "type": "string"
         },
         "IncidentSummary": {
-            "max": 4000,
+            "max": 8000,
             "min": 0,
             "type": "string"
         },
         "IncidentTemplate": {
             "documentation": "<p>Basic details used in creating a response plan. The response plan is then used to create an incident record.</p>",
             "members": {
                 "dedupeString": {
@@ -2038,15 +2038,15 @@
             },
             "type": "structure",
             "union": true
         },
         "ListIncidentRecordsInput": {
             "members": {
                 "filters": {
-                    "documentation": "<p>Filters the list of incident records through which you are searching. You can filter on the following keys:</p> <ul> <li> <p> <code>creationTime</code> </p> </li> <li> <p> <code>impact</code> </p> </li> <li> <p> <code>status</code> </p> </li> <li> <p> <code>createdBy</code> </p> </li> </ul> <p>Note the following when deciding how to use Filters:</p> <ul> <li> <p>If you don't specify a Filter, the response includes all incident records.</p> </li> <li> <p>If you specify more than one filter in a single request, the response returns incident records that match all filters.</p> </li> <li> <p>If you specify a filter with more than one value, the response returns incident records that match any of the values provided.</p> </li> </ul>",
+                    "documentation": "<p>Filters the list of incident records you want to search through. You can filter on the following keys:</p> <ul> <li> <p> <code>creationTime</code> </p> </li> <li> <p> <code>impact</code> </p> </li> <li> <p> <code>status</code> </p> </li> <li> <p> <code>createdBy</code> </p> </li> </ul> <p>Note the following when when you use Filters:</p> <ul> <li> <p>If you don't specify a Filter, the response includes all incident records.</p> </li> <li> <p>If you specify more than one filter in a single request, the response returns incident records that match all filters.</p> </li> <li> <p>If you specify a filter with more than one value, the response returns incident records that match any of the values provided.</p> </li> </ul>",
                     "shape": "FilterList"
                 },
                 "maxResults": {
                     "documentation": "<p>The maximum number of results per page.</p>",
                     "shape": "MaxResults"
                 },
                 "nextToken": {
@@ -2191,15 +2191,15 @@
                 "tags"
             ],
             "type": "structure"
         },
         "ListTimelineEventsInput": {
             "members": {
                 "filters": {
-                    "documentation": "<p>Filters the timeline events based on the provided conditional values. You can filter timeline events using the following keys:</p> <ul> <li> <p> <code>eventTime</code> </p> </li> <li> <p> <code>eventType</code> </p> </li> </ul> <p>Note the following when deciding how to use Filters:</p> <ul> <li> <p>If you don't specify a Filter, the response includes all timeline events.</p> </li> <li> <p>If you specify more than one filter in a single request, the response returns timeline events that match all filters.</p> </li> <li> <p>If you specify a filter with more than one value, the response returns timeline events that match any of the values provided.</p> </li> </ul>",
+                    "documentation": "<p>Filters the timeline events based on the provided conditional values. You can filter timeline events with the following keys:</p> <ul> <li> <p> <code>eventTime</code> </p> </li> <li> <p> <code>eventType</code> </p> </li> </ul> <p>Note the following when deciding how to use Filters:</p> <ul> <li> <p>If you don't specify a Filter, the response includes all timeline events.</p> </li> <li> <p>If you specify more than one filter in a single request, the response returns timeline events that match all filters.</p> </li> <li> <p>If you specify a filter with more than one value, the response returns timeline events that match any of the values provided.</p> </li> </ul>",
                     "shape": "FilterList"
                 },
                 "incidentRecordArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the incident that includes the timeline event.</p>",
                     "shape": "Arn"
                 },
                 "maxResults": {
@@ -2207,15 +2207,15 @@
                     "shape": "MaxResults"
                 },
                 "nextToken": {
                     "documentation": "<p>The pagination token to continue to the next page of results.</p>",
                     "shape": "NextToken"
                 },
                 "sortBy": {
-                    "documentation": "<p>Sort by the specified key value pair.</p>",
+                    "documentation": "<p>Sort timeline events by the specified key value pair.</p>",
                     "shape": "TimelineEventSort"
                 },
                 "sortOrder": {
                     "documentation": "<p>Sorts the order of timeline events by the value specified in the <code>sortBy</code> field.</p>",
                     "shape": "SortOrder"
                 }
             },
@@ -2393,15 +2393,15 @@
             },
             "required": [
                 "policyId"
             ],
             "type": "structure"
         },
         "RawData": {
-            "max": 4000,
+            "max": 10000,
             "min": 0,
             "type": "string"
         },
         "RegionInfo": {
             "documentation": "<p>Information about a Amazon Web Services Region in your replication set.</p>",
             "members": {
                 "sseKmsKeyId": {
@@ -2852,15 +2852,15 @@
                     "shape": "ClientToken"
                 },
                 "impact": {
                     "documentation": "<p>Defines the impact to the customers. Providing an impact overwrites the impact provided by a response plan.</p> <p class=\"title\"> <b>Possible impacts:</b> </p> <ul> <li> <p> <code>1</code> - Critical impact, this typically relates to full application failure that impacts many to all customers. </p> </li> <li> <p> <code>2</code> - High impact, partial application failure with impact to many customers.</p> </li> <li> <p> <code>3</code> - Medium impact, the application is providing reduced service to customers.</p> </li> <li> <p> <code>4</code> - Low impact, customer might aren't impacted by the problem yet.</p> </li> <li> <p> <code>5</code> - No impact, customers aren't currently impacted but urgent action is needed to avoid impact.</p> </li> </ul>",
                     "shape": "Impact"
                 },
                 "relatedItems": {
-                    "documentation": "<p>Add related items to the incident for other responders to use. Related items are AWS resources, external links, or files uploaded to an Amazon S3 bucket. </p>",
+                    "documentation": "<p>Add related items to the incident for other responders to use. Related items are Amazon Web Services resources, external links, or files uploaded to an Amazon S3 bucket. </p>",
                     "shape": "RelatedItemList"
                 },
                 "responsePlanArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the response plan that pre-defines summary, chat channels, Amazon SNS topics, runbooks, title, and impact of the incident. </p>",
                     "shape": "Arn"
                 },
                 "title": {
@@ -3142,28 +3142,28 @@
                     "shape": "Arn"
                 },
                 "chatChannel": {
                     "documentation": "<p>The Chatbot chat channel where responders can collaborate.</p>",
                     "shape": "ChatChannel"
                 },
                 "clientToken": {
-                    "documentation": "<p>A token that ensures that the operation is called only once with the specified details.</p>",
+                    "documentation": "<p>A token that ensures that a client calls the operation only once with the specified details.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientToken"
                 },
                 "impact": {
-                    "documentation": "<p>Defines the impact of the incident to customers and applications. Providing an impact overwrites the impact provided by the response plan.</p> <p class=\"title\"> <b>Possible impacts:</b> </p> <ul> <li> <p> <code>1</code> - Critical impact, full application failure that impacts many to all customers. </p> </li> <li> <p> <code>2</code> - High impact, partial application failure with impact to many customers.</p> </li> <li> <p> <code>3</code> - Medium impact, the application is providing reduced service to customers.</p> </li> <li> <p> <code>4</code> - Low impact, customer aren't impacted by the problem yet.</p> </li> <li> <p> <code>5</code> - No impact, customers aren't currently impacted but urgent action is needed to avoid impact.</p> </li> </ul>",
+                    "documentation": "<p>Defines the impact of the incident to customers and applications. If you provide an impact for an incident, it overwrites the impact provided by the response plan.</p> <p class=\"title\"> <b>Possible impacts:</b> </p> <ul> <li> <p> <code>1</code> - Critical impact, full application failure that impacts many to all customers. </p> </li> <li> <p> <code>2</code> - High impact, partial application failure with impact to many customers.</p> </li> <li> <p> <code>3</code> - Medium impact, the application is providing reduced service to customers.</p> </li> <li> <p> <code>4</code> - Low impact, customer aren't impacted by the problem yet.</p> </li> <li> <p> <code>5</code> - No impact, customers aren't currently impacted but urgent action is needed to avoid impact.</p> </li> </ul>",
                     "shape": "Impact"
                 },
                 "notificationTargets": {
-                    "documentation": "<p>The Amazon SNS targets that are notified when updates are made to an incident.</p> <p>Using multiple SNS topics creates redundancy in the event that a Region is down during the incident.</p>",
+                    "documentation": "<p>The Amazon SNS targets that Incident Manager notifies when a client updates an incident.</p> <p>Using multiple SNS topics creates redundancy in the event that a Region is down during the incident.</p>",
                     "shape": "NotificationTargetSet"
                 },
                 "status": {
-                    "documentation": "<p>The status of the incident. An incident can be <code>Open</code> or <code>Resolved</code>.</p>",
+                    "documentation": "<p>The status of the incident. Possible statuses are <code>Open</code> or <code>Resolved</code>.</p>",
                     "shape": "IncidentRecordStatus"
                 },
                 "summary": {
                     "documentation": "<p>A longer description of what occurred during the incident.</p>",
                     "shape": "IncidentSummary"
                 },
                 "title": {
@@ -3179,24 +3179,24 @@
         "UpdateIncidentRecordOutput": {
             "members": {},
             "type": "structure"
         },
         "UpdateRelatedItemsInput": {
             "members": {
                 "clientToken": {
-                    "documentation": "<p>A token ensuring that the operation is called only once with the specified details.</p>",
+                    "documentation": "<p>A token that ensures that a client calls the operation only once with the specified details.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientToken"
                 },
                 "incidentRecordArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the incident record containing the related items you are updating.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the incident record that contains the related items that you update.</p>",
                     "shape": "Arn"
                 },
                 "relatedItemsUpdate": {
-                    "documentation": "<p>Details about the item you are adding or deleting.</p>",
+                    "documentation": "<p>Details about the item that you are add to, or delete from, an incident.</p>",
                     "shape": "RelatedItemsUpdate"
                 }
             },
             "required": [
                 "incidentRecordArn",
                 "relatedItemsUpdate"
             ],
@@ -3319,36 +3319,36 @@
         "UpdateResponsePlanOutput": {
             "members": {},
             "type": "structure"
         },
         "UpdateTimelineEventInput": {
             "members": {
                 "clientToken": {
-                    "documentation": "<p>A token ensuring that the operation is called only once with the specified details.</p>",
+                    "documentation": "<p>A token that ensures that a client calls the operation only once with the specified details.</p>",
                     "idempotencyToken": true,
                     "shape": "ClientToken"
                 },
                 "eventData": {
                     "documentation": "<p>A short description of the event.</p>",
                     "shape": "EventData"
                 },
                 "eventId": {
-                    "documentation": "<p>The ID of the event you are updating. You can find this by using <code>ListTimelineEvents</code>.</p>",
+                    "documentation": "<p>The ID of the event to update. You can use <code>ListTimelineEvents</code> to find an event's ID.</p>",
                     "shape": "UUID"
                 },
                 "eventReferences": {
-                    "documentation": "<p>Updates all existing references in a <code>TimelineEvent</code>. A reference can be an Amazon Web Services resource involved in the incident or in some way associated with it. When you specify a reference, you enter the Amazon Resource Name (ARN) of the resource. You can also specify a related item. As an example, you could specify the ARN of an Amazon DynamoDB (DynamoDB) table. The table for this example is the resource. You could also specify a Amazon CloudWatch metric for that table. The metric is the related item.</p> <important> <p>This update action overrides all existing references. If you want to keep existing references, you must specify them in the call. If you don't, this action removes them and enters only new references.</p> </important>",
+                    "documentation": "<p>Updates all existing references in a <code>TimelineEvent</code>. A reference is an Amazon Web Services resource involved or associated with the incident. To specify a reference, enter its Amazon Resource Name (ARN). You can also specify a related item associated with that resource. For example, to specify an Amazon DynamoDB (DynamoDB) table as a resource, use its ARN. You can also specify an Amazon CloudWatch metric associated with the DynamoDB table as a related item.</p> <important> <p>This update action overrides all existing references. If you want to keep existing references, you must specify them in the call. If you don't, this action removes any existing references and enters only new references.</p> </important>",
                     "shape": "EventReferenceList"
                 },
                 "eventTime": {
                     "documentation": "<p>The time that the event occurred.</p>",
                     "shape": "Timestamp"
                 },
                 "eventType": {
-                    "documentation": "<p>The type of the event. You can update events of type <code>Custom Event</code>.</p>",
+                    "documentation": "<p>The type of event. You can update events of type <code>Custom Event</code>.</p>",
                     "shape": "TimelineEventType"
                 },
                 "incidentRecordArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the incident that includes the timeline event.</p>",
                     "shape": "Arn"
                 }
             },
```

### Comparing `botocore-a-la-carte-ssm-incidents-1.29.99/botocore/data/ssm-incidents/2018-05-10/waiters-2.json` & `botocore-a-la-carte-ssm-incidents-1.30.0/botocore/data/ssm-incidents/2018-05-10/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ssm-incidents-1.29.99/botocore_a_la_carte_ssm_incidents.egg-info/PKG-INFO` & `botocore-a-la-carte-ssm-incidents-1.30.0/botocore_a_la_carte_ssm_incidents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ssm-incidents
-Version: 1.29.99
+Version: 1.30.0
 Summary: ssm-incidents data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ssm-incidents-1.29.99/botocore_a_la_carte_ssm_incidents.egg-info/SOURCES.txt` & `botocore-a-la-carte-ssm-incidents-1.30.0/botocore_a_la_carte_ssm_incidents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ssm-incidents-1.29.99/setup.py` & `botocore-a-la-carte-ssm-incidents-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ssm-incidents',
-    version="1.29.99",
+    version="1.30.0",
     description='ssm-incidents data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ssm-incidents/*/*.json'],
```

