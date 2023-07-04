# Comparing `tmp/botocore-a-la-carte-compute-optimizer-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-compute-optimizer-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-compute-optimizer-1.29.99.tar", last modified: Sat Mar 25 01:22:27 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-compute-optimizer-1.30.0.tar", last modified: Tue Jul  4 01:44:18 2023, max compression
```

## Comparing `botocore-a-la-carte-compute-optimizer-1.29.99.tar` & `botocore-a-la-carte-compute-optimizer-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:27.826639 botocore-a-la-carte-compute-optimizer-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:27.000000 botocore-a-la-carte-compute-optimizer-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-25 01:22:27.826639 botocore-a-la-carte-compute-optimizer-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:27.826639 botocore-a-la-carte-compute-optimizer-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:27.826639 botocore-a-la-carte-compute-optimizer-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:27.826639 botocore-a-la-carte-compute-optimizer-1.29.99/botocore/data/compute-optimizer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:27.826639 botocore-a-la-carte-compute-optimizer-1.29.99/botocore/data/compute-optimizer/2019-11-01/
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-03-25 01:22:12.000000 botocore-a-la-carte-compute-optimizer-1.29.99/botocore/data/compute-optimizer/2019-11-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-compute-optimizer-1.29.99/botocore/data/compute-optimizer/2019-11-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-25 01:22:12.000000 botocore-a-la-carte-compute-optimizer-1.29.99/botocore/data/compute-optimizer/2019-11-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   214919 2023-03-25 01:22:12.000000 botocore-a-la-carte-compute-optimizer-1.29.99/botocore/data/compute-optimizer/2019-11-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:27.826639 botocore-a-la-carte-compute-optimizer-1.29.99/botocore_a_la_carte_compute_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-25 01:22:27.000000 botocore-a-la-carte-compute-optimizer-1.29.99/botocore_a_la_carte_compute_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-25 01:22:27.000000 botocore-a-la-carte-compute-optimizer-1.29.99/botocore_a_la_carte_compute_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:27.000000 botocore-a-la-carte-compute-optimizer-1.29.99/botocore_a_la_carte_compute_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:27.000000 botocore-a-la-carte-compute-optimizer-1.29.99/botocore_a_la_carte_compute_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:27.826639 botocore-a-la-carte-compute-optimizer-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-25 01:22:27.000000 botocore-a-la-carte-compute-optimizer-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:18.654425 botocore-a-la-carte-compute-optimizer-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:18.000000 botocore-a-la-carte-compute-optimizer-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-04 01:44:18.654425 botocore-a-la-carte-compute-optimizer-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:18.654425 botocore-a-la-carte-compute-optimizer-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:18.654425 botocore-a-la-carte-compute-optimizer-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:18.654425 botocore-a-la-carte-compute-optimizer-1.30.0/botocore/data/compute-optimizer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:18.654425 botocore-a-la-carte-compute-optimizer-1.30.0/botocore/data/compute-optimizer/2019-11-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17668 2023-07-04 01:44:02.000000 botocore-a-la-carte-compute-optimizer-1.30.0/botocore/data/compute-optimizer/2019-11-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-compute-optimizer-1.30.0/botocore/data/compute-optimizer/2019-11-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-04 01:44:02.000000 botocore-a-la-carte-compute-optimizer-1.30.0/botocore/data/compute-optimizer/2019-11-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   225149 2023-07-04 01:44:02.000000 botocore-a-la-carte-compute-optimizer-1.30.0/botocore/data/compute-optimizer/2019-11-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:18.654425 botocore-a-la-carte-compute-optimizer-1.30.0/botocore_a_la_carte_compute_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-04 01:44:18.000000 botocore-a-la-carte-compute-optimizer-1.30.0/botocore_a_la_carte_compute_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-04 01:44:18.000000 botocore-a-la-carte-compute-optimizer-1.30.0/botocore_a_la_carte_compute_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:18.000000 botocore-a-la-carte-compute-optimizer-1.30.0/botocore_a_la_carte_compute_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:18.000000 botocore-a-la-carte-compute-optimizer-1.30.0/botocore_a_la_carte_compute_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:18.654425 botocore-a-la-carte-compute-optimizer-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-04 01:44:18.000000 botocore-a-la-carte-compute-optimizer-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-compute-optimizer-1.29.99/LICENSE.txt` & `botocore-a-la-carte-compute-optimizer-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-compute-optimizer-1.29.99/PKG-INFO` & `botocore-a-la-carte-compute-optimizer-1.30.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-compute-optimizer
-Version: 1.29.99
+Version: 1.30.0
 Summary: compute-optimizer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-compute-optimizer-1.29.99/botocore/data/compute-optimizer/2019-11-01/paginators-1.json` & `botocore-a-la-carte-compute-optimizer-1.30.0/botocore/data/compute-optimizer/2019-11-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-compute-optimizer-1.29.99/botocore/data/compute-optimizer/2019-11-01/service-2.json` & `botocore-a-la-carte-compute-optimizer-1.30.0/botocore/data/compute-optimizer/2019-11-01/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960695757412807%*

 * *Differences: {"'shapes'": "{'AutoScalingGroupRecommendation': {'members': {'inferredWorkloadTypes': "*

 * *             "{'documentation': '<p>The applications that might be running on the instances in the "*

 * *             'Auto Scaling group as inferred by Compute Optimizer.</p> <p>Compute Optimizer can '*

 * *             'infer if one of the following applications might be running on the instances:</p> '*

 * *             '<ul> <li> <p> <code>AmazonEmr</code> - Infers that Amazon EMR might be running on '*

 * *             'the instances. […]*

```diff
@@ -951,15 +951,15 @@
                     "shape": "EffectiveRecommendationPreferences"
                 },
                 "finding": {
                     "documentation": "<p>The finding classification of the Auto Scaling group.</p> <p>Findings for Auto Scaling groups include:</p> <ul> <li> <p> <b> <code>NotOptimized</code> </b>\u2014An Auto Scaling group is considered not optimized when Compute Optimizer identifies a recommendation that can provide better performance for your workload.</p> </li> <li> <p> <b> <code>Optimized</code> </b>\u2014An Auto Scaling group is considered optimized when Compute Optimizer determines that the group is correctly provisioned to run your workload based on the chosen instance type. For optimized resources, Compute Optimizer might recommend a new generation instance type.</p> </li> </ul>",
                     "shape": "Finding"
                 },
                 "inferredWorkloadTypes": {
-                    "documentation": "<p>The applications that might be running on the instances in the Auto Scaling group as inferred by Compute Optimizer.</p> <p>Compute Optimizer can infer if one of the following applications might be running on the instances:</p> <ul> <li> <p> <code>AmazonEmr</code> - Infers that Amazon EMR might be running on the instances.</p> </li> <li> <p> <code>ApacheCassandra</code> - Infers that Apache Cassandra might be running on the instances.</p> </li> <li> <p> <code>ApacheHadoop</code> - Infers that Apache Hadoop might be running on the instances.</p> </li> <li> <p> <code>Memcached</code> - Infers that Memcached might be running on the instances.</p> </li> <li> <p> <code>NGINX</code> - Infers that NGINX might be running on the instances.</p> </li> <li> <p> <code>PostgreSql</code> - Infers that PostgreSQL might be running on the instances.</p> </li> <li> <p> <code>Redis</code> - Infers that Redis might be running on the instances.</p> </li> </ul>",
+                    "documentation": "<p>The applications that might be running on the instances in the Auto Scaling group as inferred by Compute Optimizer.</p> <p>Compute Optimizer can infer if one of the following applications might be running on the instances:</p> <ul> <li> <p> <code>AmazonEmr</code> - Infers that Amazon EMR might be running on the instances.</p> </li> <li> <p> <code>ApacheCassandra</code> - Infers that Apache Cassandra might be running on the instances.</p> </li> <li> <p> <code>ApacheHadoop</code> - Infers that Apache Hadoop might be running on the instances.</p> </li> <li> <p> <code>Memcached</code> - Infers that Memcached might be running on the instances.</p> </li> <li> <p> <code>NGINX</code> - Infers that NGINX might be running on the instances.</p> </li> <li> <p> <code>PostgreSql</code> - Infers that PostgreSQL might be running on the instances.</p> </li> <li> <p> <code>Redis</code> - Infers that Redis might be running on the instances.</p> </li> <li> <p> <code>Kafka</code> - Infers that Kafka might be running on the instance.</p> </li> <li> <p> <code>SQLServer</code> - Infers that SQLServer might be running on the instance.</p> </li> </ul>",
                     "shape": "InferredWorkloadTypes"
                 },
                 "lastRefreshTimestamp": {
                     "documentation": "<p>The timestamp of when the Auto Scaling group recommendation was last generated.</p>",
                     "shape": "LastRefreshTimestamp"
                 },
                 "lookBackPeriodInDays": {
@@ -1204,15 +1204,15 @@
         "DestinationKeyPrefix": {
             "type": "string"
         },
         "EBSFilter": {
             "documentation": "<p>Describes a filter that returns a more specific list of Amazon Elastic Block Store (Amazon EBS) volume recommendations. Use this filter with the <a>GetEBSVolumeRecommendations</a> action.</p> <p>You can use <code>LambdaFunctionRecommendationFilter</code> with the <a>GetLambdaFunctionRecommendations</a> action, <code>JobFilter</code> with the <a>DescribeRecommendationExportJobs</a> action, and <code>Filter</code> with the <a>GetAutoScalingGroupRecommendations</a> and <a>GetEC2InstanceRecommendations</a> actions.</p>",
             "members": {
                 "name": {
-                    "documentation": "<p>The name of the filter.</p> <p>Specify <code>Finding</code> to return recommendations with a specific finding classification (for example, <code>NotOptimized</code>).</p>",
+                    "documentation": "<p>The name of the filter.</p> <p>Specify <code>Finding</code> to return recommendations with a specific finding classification (for example, <code>NotOptimized</code>).</p> <p>You can filter your Amazon EBS volume recommendations by <code>tag:key</code> and <code>tag-key</code> tags.</p> <p>A <code>tag:key</code> is a key and value combination of a tag assigned to your Amazon EBS volume recommendations. Use the tag key in the filter name and the tag value as the filter value. For example, to find all Amazon EBS volume recommendations that have a tag with the key of <code>Owner</code> and the value of <code>TeamA</code>, specify <code>tag:Owner</code> for the filter name and <code>TeamA</code> for the filter value.</p> <p>A <code>tag-key</code> is the key of a tag assigned to your Amazon EBS volume recommendations. Use this filter to find all of your Amazon EBS volume recommendations that have a tag with a specific key. This doesn\u2019t consider the tag value. For example, you can find your Amazon EBS volume recommendations with a tag key value of <code>Owner</code> or without any tag keys assigned.</p>",
                     "shape": "EBSFilterName"
                 },
                 "values": {
                     "documentation": "<p>The value of the filter.</p> <p>The valid values are <code>Optimized</code>, or <code>NotOptimized</code>.</p>",
                     "shape": "FilterValues"
                 }
             },
@@ -1386,26 +1386,30 @@
                     "documentation": "<p> The Amazon Resource Name (ARN) of the current Amazon ECS service. </p> <p> The following is the format of the ARN: </p> <p> <code>arn:aws:ecs:region:aws_account_id:service/cluster-name/service-name</code> </p>",
                     "shape": "ServiceArn"
                 },
                 "serviceRecommendationOptions": {
                     "documentation": "<p> An array of objects that describe the recommendation options for the Amazon ECS service. </p>",
                     "shape": "ECSServiceRecommendationOptions"
                 },
+                "tags": {
+                    "documentation": "<p> A list of tags assigned to your Amazon ECS service recommendations. </p>",
+                    "shape": "Tags"
+                },
                 "utilizationMetrics": {
                     "documentation": "<p> An array of objects that describe the utilization metrics of the Amazon ECS service. </p>",
                     "shape": "ECSServiceUtilizationMetrics"
                 }
             },
             "type": "structure"
         },
         "ECSServiceRecommendationFilter": {
             "documentation": "<p> Describes a filter that returns a more specific list of Amazon ECS service recommendations. Use this filter with the <a>GetECSServiceRecommendations</a> action. </p>",
             "members": {
                 "name": {
-                    "documentation": "<p> The name of the filter. </p> <p> Specify <code>Finding</code> to return recommendations with a specific finding classification. </p> <p> Specify <code>FindingReasonCode</code> to return recommendations with a specific finding reason code. </p>",
+                    "documentation": "<p> The name of the filter. </p> <p> Specify <code>Finding</code> to return recommendations with a specific finding classification. </p> <p> Specify <code>FindingReasonCode</code> to return recommendations with a specific finding reason code. </p> <p>You can filter your Amazon ECS service recommendations by <code>tag:key</code> and <code>tag-key</code> tags.</p> <p>A <code>tag:key</code> is a key and value combination of a tag assigned to your Amazon ECS service recommendations. Use the tag key in the filter name and the tag value as the filter value. For example, to find all Amazon ECS service recommendations that have a tag with the key of <code>Owner</code> and the value of <code>TeamA</code>, specify <code>tag:Owner</code> for the filter name and <code>TeamA</code> for the filter value.</p> <p>A <code>tag-key</code> is the key of a tag assigned to your Amazon ECS service recommendations. Use this filter to find all of your Amazon ECS service recommendations that have a tag with a specific key. This doesn\u2019t consider the tag value. For example, you can find your Amazon ECS service recommendations with a tag key value of <code>Owner</code> or without any tag keys assigned.</p>",
                     "shape": "ECSServiceRecommendationFilterName"
                 },
                 "values": {
                     "documentation": "<p> The value of the filter. </p> <p>The valid values for this parameter are as follows:</p> <ul> <li> <p>If you specify the <code>name</code> parameter as <code>Finding</code>, specify <code>Optimized</code>, <code>NotOptimized</code>, or <code>Unavailable</code>.</p> </li> <li> <p>If you specify the <code>name</code> parameter as <code>FindingReasonCode</code>, specify <code>CPUUnderprovisioned</code>, <code>CPUOverprovisioned</code>, <code>MemoryUnderprovisioned</code>, or <code>MemoryOverprovisioned</code>.</p> </li> </ul>",
                     "shape": "FilterValues"
                 }
             },
@@ -1926,15 +1930,16 @@
                 "RecommendationOptionsMemory",
                 "RecommendationOptionsCpu",
                 "RecommendationOptionsSavingsOpportunityPercentage",
                 "RecommendationOptionsEstimatedMonthlySavingsCurrency",
                 "RecommendationOptionsEstimatedMonthlySavingsValue",
                 "RecommendationOptionsContainerRecommendations",
                 "RecommendationOptionsProjectedUtilizationMetricsCpuMaximum",
-                "RecommendationOptionsProjectedUtilizationMetricsMemoryMaximum"
+                "RecommendationOptionsProjectedUtilizationMetricsMemoryMaximum",
+                "Tags"
             ],
             "type": "string"
         },
         "ExportableECSServiceFields": {
             "member": {
                 "shape": "ExportableECSServiceField"
             },
@@ -1990,15 +1995,19 @@
                 "RecommendationOptionsEstimatedMonthlySavingsCurrency",
                 "RecommendationOptionsEstimatedMonthlySavingsValue",
                 "EffectiveRecommendationPreferencesCpuVendorArchitectures",
                 "EffectiveRecommendationPreferencesEnhancedInfrastructureMetrics",
                 "EffectiveRecommendationPreferencesInferredWorkloadTypes",
                 "InferredWorkloadTypes",
                 "RecommendationOptionsMigrationEffort",
-                "EffectiveRecommendationPreferencesExternalMetricsSource"
+                "EffectiveRecommendationPreferencesExternalMetricsSource",
+                "InstanceState",
+                "Tags",
+                "ExternalMetricStatusCode",
+                "ExternalMetricStatusReason"
             ],
             "type": "string"
         },
         "ExportableInstanceFields": {
             "member": {
                 "shape": "ExportableInstanceField"
             },
@@ -2027,15 +2036,16 @@
                 "RecommendationOptionsProjectedUtilizationMetricsDurationLowerBound",
                 "RecommendationOptionsProjectedUtilizationMetricsDurationUpperBound",
                 "RecommendationOptionsProjectedUtilizationMetricsDurationExpected",
                 "LastRefreshTimestamp",
                 "CurrentPerformanceRisk",
                 "RecommendationOptionsSavingsOpportunityPercentage",
                 "RecommendationOptionsEstimatedMonthlySavingsCurrency",
-                "RecommendationOptionsEstimatedMonthlySavingsValue"
+                "RecommendationOptionsEstimatedMonthlySavingsValue",
+                "Tags"
             ],
             "type": "string"
         },
         "ExportableLambdaFunctionFields": {
             "member": {
                 "shape": "ExportableLambdaFunctionField"
             },
@@ -2066,24 +2076,58 @@
                 "RecommendationOptionsConfigurationVolumeSize",
                 "RecommendationOptionsMonthlyPrice",
                 "RecommendationOptionsPerformanceRisk",
                 "LastRefreshTimestamp",
                 "CurrentPerformanceRisk",
                 "RecommendationOptionsSavingsOpportunityPercentage",
                 "RecommendationOptionsEstimatedMonthlySavingsCurrency",
-                "RecommendationOptionsEstimatedMonthlySavingsValue"
+                "RecommendationOptionsEstimatedMonthlySavingsValue",
+                "RootVolume",
+                "Tags"
             ],
             "type": "string"
         },
         "ExportableVolumeFields": {
             "member": {
                 "shape": "ExportableVolumeField"
             },
             "type": "list"
         },
+        "ExternalMetricStatus": {
+            "documentation": "<p> Describes Compute Optimizer's integration status with your chosen external metric provider. For example, Datadog. </p>",
+            "members": {
+                "statusCode": {
+                    "documentation": "<p> The status code for Compute Optimizer's integration with an external metrics provider. </p>",
+                    "shape": "ExternalMetricStatusCode"
+                },
+                "statusReason": {
+                    "documentation": "<p> The reason for Compute Optimizer's integration status with your external metric provider. </p>",
+                    "shape": "ExternalMetricStatusReason"
+                }
+            },
+            "type": "structure"
+        },
+        "ExternalMetricStatusCode": {
+            "enum": [
+                "NO_EXTERNAL_METRIC_SET",
+                "INTEGRATION_SUCCESS",
+                "DATADOG_INTEGRATION_ERROR",
+                "DYNATRACE_INTEGRATION_ERROR",
+                "NEWRELIC_INTEGRATION_ERROR",
+                "INSTANA_INTEGRATION_ERROR",
+                "INSUFFICIENT_DATADOG_METRICS",
+                "INSUFFICIENT_DYNATRACE_METRICS",
+                "INSUFFICIENT_NEWRELIC_METRICS",
+                "INSUFFICIENT_INSTANA_METRICS"
+            ],
+            "type": "string"
+        },
+        "ExternalMetricStatusReason": {
+            "type": "string"
+        },
         "ExternalMetricsPreference": {
             "documentation": "<p> Describes the external metrics preferences for EC2 rightsizing recommendations. </p>",
             "members": {
                 "source": {
                     "documentation": "<p> Contains the source options for external metrics preferences. </p>",
                     "shape": "ExternalMetricsSource"
                 }
@@ -2108,29 +2152,30 @@
             ],
             "type": "string"
         },
         "Filter": {
             "documentation": "<p>Describes a filter that returns a more specific list of recommendations. Use this filter with the <a>GetAutoScalingGroupRecommendations</a> and <a>GetEC2InstanceRecommendations</a> actions.</p> <p>You can use <code>EBSFilter</code> with the <a>GetEBSVolumeRecommendations</a> action, <code>LambdaFunctionRecommendationFilter</code> with the <a>GetLambdaFunctionRecommendations</a> action, and <code>JobFilter</code> with the <a>DescribeRecommendationExportJobs</a> action.</p>",
             "members": {
                 "name": {
-                    "documentation": "<p>The name of the filter.</p> <p>Specify <code>Finding</code> to return recommendations with a specific finding classification (for example, <code>Underprovisioned</code>).</p> <p>Specify <code>RecommendationSourceType</code> to return recommendations of a specific resource type (for example, <code>Ec2Instance</code>).</p> <p>Specify <code>FindingReasonCodes</code> to return recommendations with a specific finding reason code (for example, <code>CPUUnderprovisioned</code>).</p>",
+                    "documentation": "<p>The name of the filter.</p> <p>Specify <code>Finding</code> to return recommendations with a specific finding classification. For example, <code>Underprovisioned</code>.</p> <p>Specify <code>RecommendationSourceType</code> to return recommendations of a specific resource type. For example, <code>Ec2Instance</code>.</p> <p>Specify <code>FindingReasonCodes</code> to return recommendations with a specific finding reason code. For example, <code>CPUUnderprovisioned</code>.</p> <p>Specify <code>InferredWorkloadTypes</code> to return recommendations of a specific inferred workload. For example, <code>Redis</code>.</p> <p>You can filter your EC2 instance recommendations by <code>tag:key</code> and <code>tag-key</code> tags.</p> <p>A <code>tag:key</code> is a key and value combination of a tag assigned to your recommendations. Use the tag key in the filter name and the tag value as the filter value. For example, to find all recommendations that have a tag with the key of <code>Owner</code> and the value of <code>TeamA</code>, specify <code>tag:Owner</code> for the filter name and <code>TeamA</code> for the filter value.</p> <p>A <code>tag-key</code> is the key of a tag assigned to your recommendations. Use this filter to find all of your recommendations that have a tag with a specific key. This doesn\u2019t consider the tag value. For example, you can find your recommendations with a tag key value of <code>Owner</code> or without any tag keys assigned.</p>",
                     "shape": "FilterName"
                 },
                 "values": {
                     "documentation": "<p>The value of the filter.</p> <p>The valid values for this parameter are as follows, depending on what you specify for the <code>name</code> parameter and the resource type that you wish to filter results for:</p> <ul> <li> <p>Specify <code>Optimized</code> or <code>NotOptimized</code> if you specify the <code>name</code> parameter as <code>Finding</code> and you want to filter results for Auto Scaling groups.</p> </li> <li> <p>Specify <code>Underprovisioned</code>, <code>Overprovisioned</code>, or <code>Optimized</code> if you specify the <code>name</code> parameter as <code>Finding</code> and you want to filter results for EC2 instances.</p> </li> <li> <p>Specify <code>Ec2Instance</code> or <code>AutoScalingGroup</code> if you specify the <code>name</code> parameter as <code>RecommendationSourceType</code>.</p> </li> <li> <p>Specify one of the following options if you specify the <code>name</code> parameter as <code>FindingReasonCodes</code>:</p> <ul> <li> <p> <b> <code>CPUOverprovisioned</code> </b> \u2014 The instance\u2019s CPU configuration can be sized down while still meeting the performance requirements of your workload.</p> </li> <li> <p> <b> <code>CPUUnderprovisioned</code> </b> \u2014 The instance\u2019s CPU configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better CPU performance.</p> </li> <li> <p> <b> <code>MemoryOverprovisioned</code> </b> \u2014 The instance\u2019s memory configuration can be sized down while still meeting the performance requirements of your workload.</p> </li> <li> <p> <b> <code>MemoryUnderprovisioned</code> </b> \u2014 The instance\u2019s memory configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better memory performance.</p> </li> <li> <p> <b> <code>EBSThroughputOverprovisioned</code> </b> \u2014 The instance\u2019s EBS throughput configuration can be sized down while still meeting the performance requirements of your workload.</p> </li> <li> <p> <b> <code>EBSThroughputUnderprovisioned</code> </b> \u2014 The instance\u2019s EBS throughput configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better EBS throughput performance.</p> </li> <li> <p> <b> <code>EBSIOPSOverprovisioned</code> </b> \u2014 The instance\u2019s EBS IOPS configuration can be sized down while still meeting the performance requirements of your workload.</p> </li> <li> <p> <b> <code>EBSIOPSUnderprovisioned</code> </b> \u2014 The instance\u2019s EBS IOPS configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better EBS IOPS performance.</p> </li> <li> <p> <b> <code>NetworkBandwidthOverprovisioned</code> </b> \u2014 The instance\u2019s network bandwidth configuration can be sized down while still meeting the performance requirements of your workload.</p> </li> <li> <p> <b> <code>NetworkBandwidthUnderprovisioned</code> </b> \u2014 The instance\u2019s network bandwidth configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better network bandwidth performance. This finding reason happens when the <code>NetworkIn</code> or <code>NetworkOut</code> performance of an instance is impacted.</p> </li> <li> <p> <b> <code>NetworkPPSOverprovisioned</code> </b> \u2014 The instance\u2019s network PPS (packets per second) configuration can be sized down while still meeting the performance requirements of your workload.</p> </li> <li> <p> <b> <code>NetworkPPSUnderprovisioned</code> </b> \u2014 The instance\u2019s network PPS (packets per second) configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better network PPS performance.</p> </li> <li> <p> <b> <code>DiskIOPSOverprovisioned</code> </b> \u2014 The instance\u2019s disk IOPS configuration can be sized down while still meeting the performance requirements of your workload.</p> </li> <li> <p> <b> <code>DiskIOPSUnderprovisioned</code> </b> \u2014 The instance\u2019s disk IOPS configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better disk IOPS performance.</p> </li> <li> <p> <b> <code>DiskThroughputOverprovisioned</code> </b> \u2014 The instance\u2019s disk throughput configuration can be sized down while still meeting the performance requirements of your workload.</p> </li> <li> <p> <b> <code>DiskThroughputUnderprovisioned</code> </b> \u2014 The instance\u2019s disk throughput configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better disk throughput performance.</p> </li> </ul> </li> </ul>",
                     "shape": "FilterValues"
                 }
             },
             "type": "structure"
         },
         "FilterName": {
             "enum": [
                 "Finding",
                 "FindingReasonCodes",
-                "RecommendationSourceType"
+                "RecommendationSourceType",
+                "InferredWorkloadTypes"
             ],
             "type": "string"
         },
         "FilterValue": {
             "type": "string"
         },
         "FilterValues": {
@@ -2653,24 +2698,45 @@
         },
         "Identifier": {
             "type": "string"
         },
         "IncludeMemberAccounts": {
             "type": "boolean"
         },
+        "InferredWorkloadSaving": {
+            "documentation": "<p> The estimated monthly savings after you adjust the configurations of your instances running on the inferred workload types to the recommended configurations. If the <code>inferredWorkloadTypes</code> list contains multiple entries, then the savings are the sum of the monthly savings from instances that run the exact combination of the inferred workload types. </p>",
+            "members": {
+                "estimatedMonthlySavings": {
+                    "documentation": "<p>An object that describes the estimated monthly savings amount possible by adopting Compute Optimizer recommendations for a given resource. This is based on the On-Demand instance pricing.</p>",
+                    "shape": "EstimatedMonthlySavings"
+                },
+                "inferredWorkloadTypes": {
+                    "documentation": "<p>The applications that might be running on the instance as inferred by Compute Optimizer.</p> <p>Compute Optimizer can infer if one of the following applications might be running on the instance:</p> <ul> <li> <p> <code>AmazonEmr</code> - Infers that Amazon EMR might be running on the instance.</p> </li> <li> <p> <code>ApacheCassandra</code> - Infers that Apache Cassandra might be running on the instance.</p> </li> <li> <p> <code>ApacheHadoop</code> - Infers that Apache Hadoop might be running on the instance.</p> </li> <li> <p> <code>Memcached</code> - Infers that Memcached might be running on the instance.</p> </li> <li> <p> <code>NGINX</code> - Infers that NGINX might be running on the instance.</p> </li> <li> <p> <code>PostgreSql</code> - Infers that PostgreSQL might be running on the instance.</p> </li> <li> <p> <code>Redis</code> - Infers that Redis might be running on the instance.</p> </li> <li> <p> <code>Kafka</code> - Infers that Kafka might be running on the instance.</p> </li> <li> <p> <code>SQLServer</code> - Infers that SQLServer might be running on the instance.</p> </li> </ul>",
+                    "shape": "InferredWorkloadTypes"
+                }
+            },
+            "type": "structure"
+        },
+        "InferredWorkloadSavings": {
+            "member": {
+                "shape": "InferredWorkloadSaving"
+            },
+            "type": "list"
+        },
         "InferredWorkloadType": {
             "enum": [
                 "AmazonEmr",
                 "ApacheCassandra",
                 "ApacheHadoop",
                 "Memcached",
                 "Nginx",
                 "PostgreSql",
                 "Redis",
-                "Kafka"
+                "Kafka",
+                "SQLServer"
             ],
             "type": "string"
         },
         "InferredWorkloadTypes": {
             "member": {
                 "shape": "InferredWorkloadType"
             },
@@ -2710,34 +2776,42 @@
                     "documentation": "<p>The risk of the current instance not meeting the performance needs of its workloads. The higher the risk, the more likely the current instance cannot meet the performance requirements of its workload.</p>",
                     "shape": "CurrentPerformanceRisk"
                 },
                 "effectiveRecommendationPreferences": {
                     "documentation": "<p>An object that describes the effective recommendation preferences for the instance.</p>",
                     "shape": "EffectiveRecommendationPreferences"
                 },
+                "externalMetricStatus": {
+                    "documentation": "<p> An object that describes Compute Optimizer's integration status with your external metrics provider. </p>",
+                    "shape": "ExternalMetricStatus"
+                },
                 "finding": {
                     "documentation": "<p>The finding classification of the instance.</p> <p>Findings for instances include:</p> <ul> <li> <p> <b> <code>Underprovisioned</code> </b>\u2014An instance is considered under-provisioned when at least one specification of your instance, such as CPU, memory, or network, does not meet the performance requirements of your workload. Under-provisioned instances may lead to poor application performance.</p> </li> <li> <p> <b> <code>Overprovisioned</code> </b>\u2014An instance is considered over-provisioned when at least one specification of your instance, such as CPU, memory, or network, can be sized down while still meeting the performance requirements of your workload, and no specification is under-provisioned. Over-provisioned instances may lead to unnecessary infrastructure cost.</p> </li> <li> <p> <b> <code>Optimized</code> </b>\u2014An instance is considered optimized when all specifications of your instance, such as CPU, memory, and network, meet the performance requirements of your workload and is not over provisioned. For optimized resources, Compute Optimizer might recommend a new generation instance type.</p> </li> </ul>",
                     "shape": "Finding"
                 },
                 "findingReasonCodes": {
-                    "documentation": "<p>The reason for the finding classification of the instance.</p> <p>Finding reason codes for instances include:</p> <ul> <li> <p> <b> <code>CPUOverprovisioned</code> </b> \u2014 The instance\u2019s CPU configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>CPUUtilization</code> metric of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>CPUUnderprovisioned</code> </b> \u2014 The instance\u2019s CPU configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better CPU performance. This is identified by analyzing the <code>CPUUtilization</code> metric of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>MemoryOverprovisioned</code> </b> \u2014 The instance\u2019s memory configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the memory utilization metric of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>MemoryUnderprovisioned</code> </b> \u2014 The instance\u2019s memory configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better memory performance. This is identified by analyzing the memory utilization metric of the current instance during the look-back period.</p> <note> <p>Memory utilization is analyzed only for resources that have the unified CloudWatch agent installed on them. For more information, see <a href=\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/metrics.html#cw-agent\">Enabling memory utilization with the Amazon CloudWatch Agent</a> in the <i>Compute Optimizer User Guide</i>. On Linux instances, Compute Optimizer analyses the <code>mem_used_percent</code> metric in the <code>CWAgent</code> namespace, or the legacy <code>MemoryUtilization</code> metric in the <code>System/Linux</code> namespace. On Windows instances, Compute Optimizer analyses the <code>Memory % Committed Bytes In Use</code> metric in the <code>CWAgent</code> namespace.</p> </note> </li> <li> <p> <b> <code>EBSThroughputOverprovisioned</code> </b> \u2014 The instance\u2019s EBS throughput configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>VolumeReadOps</code> and <code>VolumeWriteOps</code> metrics of EBS volumes attached to the current instance during the look-back period.</p> </li> <li> <p> <b> <code>EBSThroughputUnderprovisioned</code> </b> \u2014 The instance\u2019s EBS throughput configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better EBS throughput performance. This is identified by analyzing the <code>VolumeReadOps</code> and <code>VolumeWriteOps</code> metrics of EBS volumes attached to the current instance during the look-back period.</p> </li> <li> <p> <b> <code>EBSIOPSOverprovisioned</code> </b> \u2014 The instance\u2019s EBS IOPS configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>VolumeReadBytes</code> and <code>VolumeWriteBytes</code> metric of EBS volumes attached to the current instance during the look-back period.</p> </li> <li> <p> <b> <code>EBSIOPSUnderprovisioned</code> </b> \u2014 The instance\u2019s EBS IOPS configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better EBS IOPS performance. This is identified by analyzing the <code>VolumeReadBytes</code> and <code>VolumeWriteBytes</code> metric of EBS volumes attached to the current instance during the look-back period.</p> </li> <li> <p> <b> <code>NetworkBandwidthOverprovisioned</code> </b> \u2014 The instance\u2019s network bandwidth configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>NetworkIn</code> and <code>NetworkOut</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>NetworkBandwidthUnderprovisioned</code> </b> \u2014 The instance\u2019s network bandwidth configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better network bandwidth performance. This is identified by analyzing the <code>NetworkIn</code> and <code>NetworkOut</code> metrics of the current instance during the look-back period. This finding reason happens when the <code>NetworkIn</code> or <code>NetworkOut</code> performance of an instance is impacted.</p> </li> <li> <p> <b> <code>NetworkPPSOverprovisioned</code> </b> \u2014 The instance\u2019s network PPS (packets per second) configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>NetworkPacketsIn</code> and <code>NetworkPacketsIn</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>NetworkPPSUnderprovisioned</code> </b> \u2014 The instance\u2019s network PPS (packets per second) configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better network PPS performance. This is identified by analyzing the <code>NetworkPacketsIn</code> and <code>NetworkPacketsIn</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>DiskIOPSOverprovisioned</code> </b> \u2014 The instance\u2019s disk IOPS configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>DiskReadOps</code> and <code>DiskWriteOps</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>DiskIOPSUnderprovisioned</code> </b> \u2014 The instance\u2019s disk IOPS configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better disk IOPS performance. This is identified by analyzing the <code>DiskReadOps</code> and <code>DiskWriteOps</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>DiskThroughputOverprovisioned</code> </b> \u2014 The instance\u2019s disk throughput configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>DiskReadBytes</code> and <code>DiskWriteBytes</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>DiskThroughputUnderprovisioned</code> </b> \u2014 The instance\u2019s disk throughput configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better disk throughput performance. This is identified by analyzing the <code>DiskReadBytes</code> and <code>DiskWriteBytes</code> metrics of the current instance during the look-back period.</p> </li> </ul> <note> <p>For more information about instance metrics, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/viewing_metrics_with_cloudwatch.html\">List the available CloudWatch metrics for your instances</a> in the <i>Amazon Elastic Compute Cloud User Guide</i>. For more information about EBS volume metrics, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using_cloudwatch_ebs.html\">Amazon CloudWatch metrics for Amazon EBS</a> in the <i>Amazon Elastic Compute Cloud User Guide</i>.</p> </note>",
+                    "documentation": "<p>The reason for the finding classification of the instance.</p> <p>Finding reason codes for instances include:</p> <ul> <li> <p> <b> <code>CPUOverprovisioned</code> </b> \u2014 The instance\u2019s CPU configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>CPUUtilization</code> metric of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>CPUUnderprovisioned</code> </b> \u2014 The instance\u2019s CPU configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better CPU performance. This is identified by analyzing the <code>CPUUtilization</code> metric of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>MemoryOverprovisioned</code> </b> \u2014 The instance\u2019s memory configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the memory utilization metric of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>MemoryUnderprovisioned</code> </b> \u2014 The instance\u2019s memory configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better memory performance. This is identified by analyzing the memory utilization metric of the current instance during the look-back period.</p> <note> <p>Memory utilization is analyzed only for resources that have the unified CloudWatch agent installed on them. For more information, see <a href=\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/metrics.html#cw-agent\">Enabling memory utilization with the Amazon CloudWatch Agent</a> in the <i>Compute Optimizer User Guide</i>. On Linux instances, Compute Optimizer analyses the <code>mem_used_percent</code> metric in the <code>CWAgent</code> namespace, or the legacy <code>MemoryUtilization</code> metric in the <code>System/Linux</code> namespace. On Windows instances, Compute Optimizer analyses the <code>Memory % Committed Bytes In Use</code> metric in the <code>CWAgent</code> namespace.</p> </note> </li> <li> <p> <b> <code>EBSThroughputOverprovisioned</code> </b> \u2014 The instance\u2019s EBS throughput configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>VolumeReadBytes</code> and <code>VolumeWriteBytes</code> metrics of EBS volumes attached to the current instance during the look-back period.</p> </li> <li> <p> <b> <code>EBSThroughputUnderprovisioned</code> </b> \u2014 The instance\u2019s EBS throughput configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better EBS throughput performance. This is identified by analyzing the <code>VolumeReadBytes</code> and <code>VolumeWriteBytes</code> metrics of EBS volumes attached to the current instance during the look-back period.</p> </li> <li> <p> <b> <code>EBSIOPSOverprovisioned</code> </b> \u2014 The instance\u2019s EBS IOPS configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>VolumeReadOps</code> and <code>VolumeWriteOps</code> metric of EBS volumes attached to the current instance during the look-back period.</p> </li> <li> <p> <b> <code>EBSIOPSUnderprovisioned</code> </b> \u2014 The instance\u2019s EBS IOPS configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better EBS IOPS performance. This is identified by analyzing the <code>VolumeReadOps</code> and <code>VolumeWriteOps</code> metric of EBS volumes attached to the current instance during the look-back period.</p> </li> <li> <p> <b> <code>NetworkBandwidthOverprovisioned</code> </b> \u2014 The instance\u2019s network bandwidth configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>NetworkIn</code> and <code>NetworkOut</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>NetworkBandwidthUnderprovisioned</code> </b> \u2014 The instance\u2019s network bandwidth configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better network bandwidth performance. This is identified by analyzing the <code>NetworkIn</code> and <code>NetworkOut</code> metrics of the current instance during the look-back period. This finding reason happens when the <code>NetworkIn</code> or <code>NetworkOut</code> performance of an instance is impacted.</p> </li> <li> <p> <b> <code>NetworkPPSOverprovisioned</code> </b> \u2014 The instance\u2019s network PPS (packets per second) configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>NetworkPacketsIn</code> and <code>NetworkPacketsIn</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>NetworkPPSUnderprovisioned</code> </b> \u2014 The instance\u2019s network PPS (packets per second) configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better network PPS performance. This is identified by analyzing the <code>NetworkPacketsIn</code> and <code>NetworkPacketsIn</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>DiskIOPSOverprovisioned</code> </b> \u2014 The instance\u2019s disk IOPS configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>DiskReadOps</code> and <code>DiskWriteOps</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>DiskIOPSUnderprovisioned</code> </b> \u2014 The instance\u2019s disk IOPS configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better disk IOPS performance. This is identified by analyzing the <code>DiskReadOps</code> and <code>DiskWriteOps</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>DiskThroughputOverprovisioned</code> </b> \u2014 The instance\u2019s disk throughput configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>DiskReadBytes</code> and <code>DiskWriteBytes</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>DiskThroughputUnderprovisioned</code> </b> \u2014 The instance\u2019s disk throughput configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better disk throughput performance. This is identified by analyzing the <code>DiskReadBytes</code> and <code>DiskWriteBytes</code> metrics of the current instance during the look-back period.</p> </li> </ul> <note> <p>For more information about instance metrics, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/viewing_metrics_with_cloudwatch.html\">List the available CloudWatch metrics for your instances</a> in the <i>Amazon Elastic Compute Cloud User Guide</i>. For more information about EBS volume metrics, see <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using_cloudwatch_ebs.html\">Amazon CloudWatch metrics for Amazon EBS</a> in the <i>Amazon Elastic Compute Cloud User Guide</i>.</p> </note>",
                     "shape": "InstanceRecommendationFindingReasonCodes"
                 },
                 "inferredWorkloadTypes": {
-                    "documentation": "<p>The applications that might be running on the instance as inferred by Compute Optimizer.</p> <p>Compute Optimizer can infer if one of the following applications might be running on the instance:</p> <ul> <li> <p> <code>AmazonEmr</code> - Infers that Amazon EMR might be running on the instance.</p> </li> <li> <p> <code>ApacheCassandra</code> - Infers that Apache Cassandra might be running on the instance.</p> </li> <li> <p> <code>ApacheHadoop</code> - Infers that Apache Hadoop might be running on the instance.</p> </li> <li> <p> <code>Memcached</code> - Infers that Memcached might be running on the instance.</p> </li> <li> <p> <code>NGINX</code> - Infers that NGINX might be running on the instance.</p> </li> <li> <p> <code>PostgreSql</code> - Infers that PostgreSQL might be running on the instance.</p> </li> <li> <p> <code>Redis</code> - Infers that Redis might be running on the instance.</p> </li> <li> <p> <code>Kafka</code> - Infers that Kafka might be running on the instance.</p> </li> </ul>",
+                    "documentation": "<p>The applications that might be running on the instance as inferred by Compute Optimizer.</p> <p>Compute Optimizer can infer if one of the following applications might be running on the instance:</p> <ul> <li> <p> <code>AmazonEmr</code> - Infers that Amazon EMR might be running on the instance.</p> </li> <li> <p> <code>ApacheCassandra</code> - Infers that Apache Cassandra might be running on the instance.</p> </li> <li> <p> <code>ApacheHadoop</code> - Infers that Apache Hadoop might be running on the instance.</p> </li> <li> <p> <code>Memcached</code> - Infers that Memcached might be running on the instance.</p> </li> <li> <p> <code>NGINX</code> - Infers that NGINX might be running on the instance.</p> </li> <li> <p> <code>PostgreSql</code> - Infers that PostgreSQL might be running on the instance.</p> </li> <li> <p> <code>Redis</code> - Infers that Redis might be running on the instance.</p> </li> <li> <p> <code>Kafka</code> - Infers that Kafka might be running on the instance.</p> </li> <li> <p> <code>SQLServer</code> - Infers that SQLServer might be running on the instance.</p> </li> </ul>",
                     "shape": "InferredWorkloadTypes"
                 },
                 "instanceArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the current instance.</p>",
                     "shape": "InstanceArn"
                 },
                 "instanceName": {
                     "documentation": "<p>The name of the current instance.</p>",
                     "shape": "InstanceName"
                 },
+                "instanceState": {
+                    "documentation": "<p> The state of the instance when the recommendation was generated. </p>",
+                    "shape": "InstanceState"
+                },
                 "lastRefreshTimestamp": {
                     "documentation": "<p>The timestamp of when the instance recommendation was last generated.</p>",
                     "shape": "LastRefreshTimestamp"
                 },
                 "lookBackPeriodInDays": {
                     "documentation": "<p>The number of days for which utilization metrics were analyzed for the instance.</p>",
                     "shape": "LookBackPeriodInDays"
@@ -2746,14 +2820,18 @@
                     "documentation": "<p>An array of objects that describe the recommendation options for the instance.</p>",
                     "shape": "RecommendationOptions"
                 },
                 "recommendationSources": {
                     "documentation": "<p>An array of objects that describe the source resource of the recommendation.</p>",
                     "shape": "RecommendationSources"
                 },
+                "tags": {
+                    "documentation": "<p> A list of tags assigned to your Amazon EC2 instance recommendations. </p>",
+                    "shape": "Tags"
+                },
                 "utilizationMetrics": {
                     "documentation": "<p>An array of objects that describe the utilization metrics of the instance.</p>",
                     "shape": "UtilizationMetrics"
                 }
             },
             "type": "structure"
         },
@@ -2820,14 +2898,25 @@
         },
         "InstanceRecommendations": {
             "member": {
                 "shape": "InstanceRecommendation"
             },
             "type": "list"
         },
+        "InstanceState": {
+            "enum": [
+                "pending",
+                "running",
+                "shutting-down",
+                "terminated",
+                "stopping",
+                "stopped"
+            ],
+            "type": "string"
+        },
         "InstanceType": {
             "type": "string"
         },
         "InternalServerException": {
             "documentation": "<p>An internal error has occurred. Try your call again.</p>",
             "exception": true,
             "fault": true,
@@ -3017,26 +3106,30 @@
                     "documentation": "<p>An array of objects that describe the memory configuration recommendation options for the function.</p>",
                     "shape": "LambdaFunctionMemoryRecommendationOptions"
                 },
                 "numberOfInvocations": {
                     "documentation": "<p>The number of times your function code was applied during the look-back period.</p>",
                     "shape": "NumberOfInvocations"
                 },
+                "tags": {
+                    "documentation": "<p> A list of tags assigned to your Lambda function recommendations. </p>",
+                    "shape": "Tags"
+                },
                 "utilizationMetrics": {
                     "documentation": "<p>An array of objects that describe the utilization metrics of the function.</p>",
                     "shape": "LambdaFunctionUtilizationMetrics"
                 }
             },
             "type": "structure"
         },
         "LambdaFunctionRecommendationFilter": {
             "documentation": "<p>Describes a filter that returns a more specific list of Lambda function recommendations. Use this filter with the <a>GetLambdaFunctionRecommendations</a> action.</p> <p>You can use <code>EBSFilter</code> with the <a>GetEBSVolumeRecommendations</a> action, <code>JobFilter</code> with the <a>DescribeRecommendationExportJobs</a> action, and <code>Filter</code> with the <a>GetAutoScalingGroupRecommendations</a> and <a>GetEC2InstanceRecommendations</a> actions.</p>",
             "members": {
                 "name": {
-                    "documentation": "<p>The name of the filter.</p> <p>Specify <code>Finding</code> to return recommendations with a specific finding classification (for example, <code>NotOptimized</code>).</p> <p>Specify <code>FindingReasonCode</code> to return recommendations with a specific finding reason code (for example, <code>MemoryUnderprovisioned</code>).</p>",
+                    "documentation": "<p>The name of the filter.</p> <p>Specify <code>Finding</code> to return recommendations with a specific finding classification (for example, <code>NotOptimized</code>).</p> <p>Specify <code>FindingReasonCode</code> to return recommendations with a specific finding reason code (for example, <code>MemoryUnderprovisioned</code>).</p> <p>You can filter your Lambda function recommendations by <code>tag:key</code> and <code>tag-key</code> tags.</p> <p>A <code>tag:key</code> is a key and value combination of a tag assigned to your Lambda function recommendations. Use the tag key in the filter name and the tag value as the filter value. For example, to find all Lambda function recommendations that have a tag with the key of <code>Owner</code> and the value of <code>TeamA</code>, specify <code>tag:Owner</code> for the filter name and <code>TeamA</code> for the filter value.</p> <p>A <code>tag-key</code> is the key of a tag assigned to your Lambda function recommendations. Use this filter to find all of your Lambda function recommendations that have a tag with a specific key. This doesn\u2019t consider the tag value. For example, you can find your Lambda function recommendations with a tag key value of <code>Owner</code> or without any tag keys assigned.</p>",
                     "shape": "LambdaFunctionRecommendationFilterName"
                 },
                 "values": {
                     "documentation": "<p>The value of the filter.</p> <p>The valid values for this parameter are as follows, depending on what you specify for the <code>name</code> parameter:</p> <ul> <li> <p>Specify <code>Optimized</code>, <code>NotOptimized</code>, or <code>Unavailable</code> if you specify the <code>name</code> parameter as <code>Finding</code>.</p> </li> <li> <p>Specify <code>MemoryOverprovisioned</code>, <code>MemoryUnderprovisioned</code>, <code>InsufficientData</code>, or <code>Inconclusive</code> if you specify the <code>name</code> parameter as <code>FindingReasonCode</code>.</p> </li> </ul>",
                     "shape": "FilterValues"
                 }
             },
@@ -3517,14 +3610,18 @@
                     "documentation": "<p>The Amazon Web Services account ID of the recommendation summary.</p>",
                     "shape": "AccountId"
                 },
                 "currentPerformanceRiskRatings": {
                     "documentation": "<p>An object that describes the performance risk ratings for a given resource type.</p>",
                     "shape": "CurrentPerformanceRiskRatings"
                 },
+                "inferredWorkloadSavings": {
+                    "documentation": "<p> An array of objects that describes the estimated monthly saving amounts for the instances running on the specified <code>inferredWorkloadTypes</code>. The array contains the top three savings opportunites for the instances running inferred workload types. </p>",
+                    "shape": "InferredWorkloadSavings"
+                },
                 "recommendationResourceType": {
                     "documentation": "<p>The resource type that the recommendation summary applies to.</p>",
                     "shape": "RecommendationSourceType"
                 },
                 "savingsOpportunity": {
                     "documentation": "<p>An object that describes the savings opportunity for a given resource type. Savings opportunity includes the estimated monthly savings amount and percentage.</p>",
                     "shape": "SavingsOpportunity"
@@ -3584,14 +3681,17 @@
                 "EbsVolume",
                 "LambdaFunction",
                 "NotApplicable",
                 "EcsService"
             ],
             "type": "string"
         },
+        "RootVolume": {
+            "type": "boolean"
+        },
         "S3Destination": {
             "documentation": "<p>Describes the destination Amazon Simple Storage Service (Amazon S3) bucket name and object keys of a recommendations export file, and its associated metadata file.</p>",
             "members": {
                 "bucket": {
                     "documentation": "<p>The name of the Amazon S3 bucket used as the destination of an export file.</p>",
                     "shape": "DestinationBucket"
                 },
@@ -3620,15 +3720,15 @@
             },
             "type": "structure"
         },
         "SavingsOpportunity": {
             "documentation": "<p>Describes the savings opportunity for recommendations of a given resource type or for the recommendation option of an individual resource.</p> <p>Savings opportunity represents the estimated monthly savings you can achieve by implementing a given Compute Optimizer recommendation.</p> <important> <p>Savings opportunity data requires that you opt in to Cost Explorer, as well as activate <b>Receive Amazon EC2 resource recommendations</b> in the Cost Explorer preferences page. That creates a connection between Cost Explorer and Compute Optimizer. With this connection, Cost Explorer generates savings estimates considering the price of existing resources, the price of recommended resources, and historical usage data. Estimated monthly savings reflects the projected dollar savings associated with each of the recommendations generated. For more information, see <a href=\"https://docs.aws.amazon.com/cost-management/latest/userguide/ce-enable.html\">Enabling Cost Explorer</a> and <a href=\"https://docs.aws.amazon.com/cost-management/latest/userguide/ce-rightsizing.html\">Optimizing your cost with Rightsizing Recommendations</a> in the <i>Cost Management User Guide</i>.</p> </important>",
             "members": {
                 "estimatedMonthlySavings": {
-                    "documentation": "<p>An object that describes the estimated monthly savings amount possible, based on On-Demand instance pricing, by adopting Compute Optimizer recommendations for a given resource.</p>",
+                    "documentation": "<p>An object that describes the estimated monthly savings amount possible by adopting Compute Optimizer recommendations for a given resource. This is based on the On-Demand instance pricing..</p>",
                     "shape": "EstimatedMonthlySavings"
                 },
                 "savingsOpportunityPercentage": {
                     "documentation": "<p>The estimated monthly savings possible as a percentage of monthly cost by adopting Compute Optimizer recommendations for a given resource.</p>",
                     "shape": "SavingsOpportunityPercentage"
                 }
             },
@@ -3743,14 +3843,40 @@
                 }
             },
             "type": "structure"
         },
         "SummaryValue": {
             "type": "double"
         },
+        "Tag": {
+            "documentation": "<p> A list of tag key and value pairs that you define. </p>",
+            "members": {
+                "key": {
+                    "documentation": "<p> One part of a key-value pair that makes up a tag. A key is a general label that acts like a category for more specific tag values. </p>",
+                    "shape": "TagKey"
+                },
+                "value": {
+                    "documentation": "<p> One part of a key-value pair that make up a tag. A value acts as a descriptor within a tag category (key). The value can be empty or null. </p>",
+                    "shape": "TagValue"
+                }
+            },
+            "type": "structure"
+        },
+        "TagKey": {
+            "type": "string"
+        },
+        "TagValue": {
+            "type": "string"
+        },
+        "Tags": {
+            "member": {
+                "shape": "Tag"
+            },
+            "type": "list"
+        },
         "TaskDefinitionArn": {
             "type": "string"
         },
         "ThrottlingException": {
             "documentation": "<p>The request was denied due to request throttling.</p>",
             "exception": true,
             "members": {
@@ -3855,14 +3981,18 @@
         },
         "VolumeBurstThroughput": {
             "type": "integer"
         },
         "VolumeConfiguration": {
             "documentation": "<p>Describes the configuration of an Amazon Elastic Block Store (Amazon EBS) volume.</p>",
             "members": {
+                "rootVolume": {
+                    "documentation": "<p> Contains the image used to boot the instance during launch. </p>",
+                    "shape": "RootVolume"
+                },
                 "volumeBaselineIOPS": {
                     "documentation": "<p>The baseline IOPS of the volume.</p>",
                     "shape": "VolumeBaselineIOPS"
                 },
                 "volumeBaselineThroughput": {
                     "documentation": "<p>The baseline throughput of the volume.</p>",
                     "shape": "VolumeBaselineThroughput"
@@ -3909,14 +4039,18 @@
                     "documentation": "<p>The timestamp of when the volume recommendation was last generated.</p>",
                     "shape": "LastRefreshTimestamp"
                 },
                 "lookBackPeriodInDays": {
                     "documentation": "<p>The number of days for which utilization metrics were analyzed for the volume.</p>",
                     "shape": "LookBackPeriodInDays"
                 },
+                "tags": {
+                    "documentation": "<p> A list of tags assigned to your Amazon EBS volume recommendations. </p>",
+                    "shape": "Tags"
+                },
                 "utilizationMetrics": {
                     "documentation": "<p>An array of objects that describe the utilization metrics of the volume.</p>",
                     "shape": "EBSUtilizationMetrics"
                 },
                 "volumeArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the current volume.</p>",
                     "shape": "VolumeArn"
```

### Comparing `botocore-a-la-carte-compute-optimizer-1.29.99/botocore_a_la_carte_compute_optimizer.egg-info/PKG-INFO` & `botocore-a-la-carte-compute-optimizer-1.30.0/botocore_a_la_carte_compute_optimizer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-compute-optimizer
-Version: 1.29.99
+Version: 1.30.0
 Summary: compute-optimizer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-compute-optimizer-1.29.99/setup.py` & `botocore-a-la-carte-compute-optimizer-1.30.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-compute-optimizer',
-    version="1.29.99",
+    version="1.30.0",
     description='compute-optimizer data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/compute-optimizer/*/*.json'],
```

