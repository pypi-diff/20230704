# Comparing `tmp/botocore-a-la-carte-sagemaker-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-sagemaker-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-sagemaker-1.29.99.tar", last modified: Sat Mar 25 01:23:10 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-sagemaker-1.30.0.tar", last modified: Tue Jul  4 01:45:02 2023, max compression
```

## Comparing `botocore-a-la-carte-sagemaker-1.29.99.tar` & `botocore-a-la-carte-sagemaker-1.30.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:10.465193 botocore-a-la-carte-sagemaker-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:10.000000 botocore-a-la-carte-sagemaker-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-25 01:23:10.465193 botocore-a-la-carte-sagemaker-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:10.461193 botocore-a-la-carte-sagemaker-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:10.461193 botocore-a-la-carte-sagemaker-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:10.461193 botocore-a-la-carte-sagemaker-1.29.99/botocore/data/sagemaker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:10.465193 botocore-a-la-carte-sagemaker-1.29.99/botocore/data/sagemaker/2017-07-24/
--rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-03-25 01:22:12.000000 botocore-a-la-carte-sagemaker-1.29.99/botocore/data/sagemaker/2017-07-24/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-sagemaker-1.29.99/botocore/data/sagemaker/2017-07-24/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-03-25 01:22:12.000000 botocore-a-la-carte-sagemaker-1.29.99/botocore/data/sagemaker/2017-07-24/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)  1598863 2023-03-25 01:22:12.000000 botocore-a-la-carte-sagemaker-1.29.99/botocore/data/sagemaker/2017-07-24/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-03-25 01:22:12.000000 botocore-a-la-carte-sagemaker-1.29.99/botocore/data/sagemaker/2017-07-24/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:10.465193 botocore-a-la-carte-sagemaker-1.29.99/botocore_a_la_carte_sagemaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-25 01:23:10.000000 botocore-a-la-carte-sagemaker-1.29.99/botocore_a_la_carte_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-25 01:23:10.000000 botocore-a-la-carte-sagemaker-1.29.99/botocore_a_la_carte_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:10.000000 botocore-a-la-carte-sagemaker-1.29.99/botocore_a_la_carte_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:10.000000 botocore-a-la-carte-sagemaker-1.29.99/botocore_a_la_carte_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:10.465193 botocore-a-la-carte-sagemaker-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-25 01:23:10.000000 botocore-a-la-carte-sagemaker-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:02.846853 botocore-a-la-carte-sagemaker-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:45:02.000000 botocore-a-la-carte-sagemaker-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-04 01:45:02.846853 botocore-a-la-carte-sagemaker-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:02.842853 botocore-a-la-carte-sagemaker-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:02.842853 botocore-a-la-carte-sagemaker-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:02.842853 botocore-a-la-carte-sagemaker-1.30.0/botocore/data/sagemaker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:02.846853 botocore-a-la-carte-sagemaker-1.30.0/botocore/data/sagemaker/2017-07-24/
+-rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-04 01:44:02.000000 botocore-a-la-carte-sagemaker-1.30.0/botocore/data/sagemaker/2017-07-24/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-sagemaker-1.30.0/botocore/data/sagemaker/2017-07-24/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-07-04 01:44:02.000000 botocore-a-la-carte-sagemaker-1.30.0/botocore/data/sagemaker/2017-07-24/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1666996 2023-07-04 01:44:02.000000 botocore-a-la-carte-sagemaker-1.30.0/botocore/data/sagemaker/2017-07-24/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-07-04 01:44:02.000000 botocore-a-la-carte-sagemaker-1.30.0/botocore/data/sagemaker/2017-07-24/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:02.846853 botocore-a-la-carte-sagemaker-1.30.0/botocore_a_la_carte_sagemaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-04 01:45:02.000000 botocore-a-la-carte-sagemaker-1.30.0/botocore_a_la_carte_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-04 01:45:02.000000 botocore-a-la-carte-sagemaker-1.30.0/botocore_a_la_carte_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:45:02.000000 botocore-a-la-carte-sagemaker-1.30.0/botocore_a_la_carte_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:45:02.000000 botocore-a-la-carte-sagemaker-1.30.0/botocore_a_la_carte_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:45:02.846853 botocore-a-la-carte-sagemaker-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-04 01:45:02.000000 botocore-a-la-carte-sagemaker-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-sagemaker-1.29.99/LICENSE.txt` & `botocore-a-la-carte-sagemaker-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-1.29.99/PKG-INFO` & `botocore-a-la-carte-sagemaker-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sagemaker
-Version: 1.29.99
+Version: 1.30.0
 Summary: sagemaker data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sagemaker-1.29.99/botocore/data/sagemaker/2017-07-24/endpoint-rule-set-1.json` & `botocore-a-la-carte-sagemaker-1.30.0/botocore/data/sagemaker/2017-07-24/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-1.29.99/botocore/data/sagemaker/2017-07-24/paginators-1.json` & `botocore-a-la-carte-sagemaker-1.30.0/botocore/data/sagemaker/2017-07-24/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-1.29.99/botocore/data/sagemaker/2017-07-24/service-2.json` & `botocore-a-la-carte-sagemaker-1.30.0/botocore/data/sagemaker/2017-07-24/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964248811114034%*

 * *Differences: {"'operations'": "{'AddTags': {'documentation': '<p>Adds or overwrites one or more tags for the "*

 * *                 'specified SageMaker resource. You can add tags to notebook instances, training '*

 * *                 'jobs, hyperparameter tuning jobs, batch transform jobs, models, labeling jobs, '*

 * *                 'work teams, endpoint configurations, and endpoints.</p> <p>Each tag consists of '*

 * *                 'a key and an optional value. Tag keys must be unique per resource. For more '*

 * *                 'in […]*

```diff
@@ -33,29 +33,29 @@
             },
             "name": "AddAssociation",
             "output": {
                 "shape": "AddAssociationResponse"
             }
         },
         "AddTags": {
-            "documentation": "<p>Adds or overwrites one or more tags for the specified SageMaker resource. You can add tags to notebook instances, training jobs, hyperparameter tuning jobs, batch transform jobs, models, labeling jobs, work teams, endpoint configurations, and endpoints.</p> <p>Each tag consists of a key and an optional value. Tag keys must be unique per resource. For more information about tags, see For more information, see <a href=\"https://aws.amazon.com/answers/account-management/aws-tagging-strategies/\">Amazon Web Services Tagging Strategies</a>.</p> <note> <p>Tags that you add to a hyperparameter tuning job by calling this API are also added to any training jobs that the hyperparameter tuning job launches after you call this API, but not to training jobs that the hyperparameter tuning job launched before you called this API. To make sure that the tags associated with a hyperparameter tuning job are also added to all training jobs that the hyperparameter tuning job launches, add the tags when you first create the tuning job by specifying them in the <code>Tags</code> parameter of <a>CreateHyperParameterTuningJob</a> </p> </note> <note> <p>Tags that you add to a SageMaker Studio Domain or User Profile by calling this API are also added to any Apps that the Domain or User Profile launches after you call this API, but not to Apps that the Domain or User Profile launched before you called this API. To make sure that the tags associated with a Domain or User Profile are also added to all Apps that the Domain or User Profile launches, add the tags when you first create the Domain or User Profile by specifying them in the <code>Tags</code> parameter of <a>CreateDomain</a> or <a>CreateUserProfile</a>.</p> </note>",
+            "documentation": "<p>Adds or overwrites one or more tags for the specified SageMaker resource. You can add tags to notebook instances, training jobs, hyperparameter tuning jobs, batch transform jobs, models, labeling jobs, work teams, endpoint configurations, and endpoints.</p> <p>Each tag consists of a key and an optional value. Tag keys must be unique per resource. For more information about tags, see For more information, see <a href=\"https://aws.amazon.com/answers/account-management/aws-tagging-strategies/\">Amazon Web Services Tagging Strategies</a>.</p> <note> <p>Tags that you add to a hyperparameter tuning job by calling this API are also added to any training jobs that the hyperparameter tuning job launches after you call this API, but not to training jobs that the hyperparameter tuning job launched before you called this API. To make sure that the tags associated with a hyperparameter tuning job are also added to all training jobs that the hyperparameter tuning job launches, add the tags when you first create the tuning job by specifying them in the <code>Tags</code> parameter of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateHyperParameterTuningJob.html\">CreateHyperParameterTuningJob</a> </p> </note> <note> <p>Tags that you add to a SageMaker Studio Domain or User Profile by calling this API are also added to any Apps that the Domain or User Profile launches after you call this API, but not to Apps that the Domain or User Profile launched before you called this API. To make sure that the tags associated with a Domain or User Profile are also added to all Apps that the Domain or User Profile launches, add the tags when you first create the Domain or User Profile by specifying them in the <code>Tags</code> parameter of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateDomain.html\">CreateDomain</a> or <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateUserProfile.html\">CreateUserProfile</a>.</p> </note>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "AddTagsInput"
             },
             "name": "AddTags",
             "output": {
                 "shape": "AddTagsOutput"
             }
         },
         "AssociateTrialComponent": {
-            "documentation": "<p>Associates a trial component with a trial. A trial component can be associated with multiple trials. To disassociate a trial component from a trial, call the <a>DisassociateTrialComponent</a> API.</p>",
+            "documentation": "<p>Associates a trial component with a trial. A trial component can be associated with multiple trials. To disassociate a trial component from a trial, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DisassociateTrialComponent.html\">DisassociateTrialComponent</a> API.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 },
                 {
                     "shape": "ResourceLimitExceeded"
                 }
@@ -176,15 +176,15 @@
             },
             "name": "CreateArtifact",
             "output": {
                 "shape": "CreateArtifactResponse"
             }
         },
         "CreateAutoMLJob": {
-            "documentation": "<p>Creates an Autopilot job.</p> <p>Find the best-performing model after you run an Autopilot job by calling .</p> <p>For information about how to use Autopilot, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-automate-model-development.html\">Automate Model Development with Amazon SageMaker Autopilot</a>.</p>",
+            "documentation": "<p>Creates an Autopilot job also referred to as Autopilot experiment or AutoML job.</p> <note> <p>We recommend using the new versions <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJobV2.html\">CreateAutoMLJobV2</a> and <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeAutoMLJobV2.html\">DescribeAutoMLJobV2</a>, which offer backward compatibility.</p> <p> <code>CreateAutoMLJobV2</code> can manage tabular problem types identical to those of its previous version <code>CreateAutoMLJob</code>, as well as non-tabular problem types such as image or text classification.</p> <p>Find guidelines about how to migrate a <code>CreateAutoMLJob</code> to <code>CreateAutoMLJobV2</code> in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-automate-model-development-create-experiment-api.html#autopilot-create-experiment-api-migrate-v1-v2\">Migrate a CreateAutoMLJob to CreateAutoMLJobV2</a>.</p> </note> <p>You can find the best-performing model after you run an AutoML job by calling <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeAutoMLJobV2.html\">DescribeAutoMLJobV2</a> (recommended) or <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeAutoMLJob.html\">DescribeAutoMLJob</a>.</p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 },
                 {
                     "shape": "ResourceLimitExceeded"
                 }
@@ -198,15 +198,15 @@
             },
             "name": "CreateAutoMLJob",
             "output": {
                 "shape": "CreateAutoMLJobResponse"
             }
         },
         "CreateAutoMLJobV2": {
-            "documentation": "<p>Creates an Amazon SageMaker AutoML job that uses non-tabular data such as images or text for Computer Vision or Natural Language Processing problems.</p> <p>Find the resulting model after you run an AutoML job V2 by calling .</p> <p>To create an <code>AutoMLJob</code> using tabular data, see .</p> <note> <p>This API action is callable through SageMaker Canvas only. Calling it directly from the CLI or an SDK results in an error.</p> </note>",
+            "documentation": "<p>Creates an Autopilot job also referred to as Autopilot experiment or AutoML job V2.</p> <note> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJobV2.html\">CreateAutoMLJobV2</a> and <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeAutoMLJobV2.html\">DescribeAutoMLJobV2</a> are new versions of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJob.html\">CreateAutoMLJob</a> and <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeAutoMLJob.html\">DescribeAutoMLJob</a> which offer backward compatibility.</p> <p> <code>CreateAutoMLJobV2</code> can manage tabular problem types identical to those of its previous version <code>CreateAutoMLJob</code>, as well as non-tabular problem types such as image or text classification.</p> <p>Find guidelines about how to migrate a <code>CreateAutoMLJob</code> to <code>CreateAutoMLJobV2</code> in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-automate-model-development-create-experiment-api.html#autopilot-create-experiment-api-migrate-v1-v2\">Migrate a CreateAutoMLJob to CreateAutoMLJobV2</a>.</p> </note> <p>For the list of available problem types supported by <code>CreateAutoMLJobV2</code>, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AutoMLProblemTypeConfig.html\">AutoMLProblemTypeConfig</a>.</p> <p>You can find the best-performing model after you run an AutoML job V2 by calling <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeAutoMLJobV2.html\">DescribeAutoMLJobV2</a>.</p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 },
                 {
                     "shape": "ResourceLimitExceeded"
                 }
@@ -234,15 +234,15 @@
             },
             "name": "CreateCodeRepository",
             "output": {
                 "shape": "CreateCodeRepositoryOutput"
             }
         },
         "CreateCompilationJob": {
-            "documentation": "<p>Starts a model compilation job. After the model has been compiled, Amazon SageMaker saves the resulting model artifacts to an Amazon Simple Storage Service (Amazon S3) bucket that you specify. </p> <p>If you choose to host your model using Amazon SageMaker hosting services, you can use the resulting model artifacts as part of the model. You can also use the artifacts with Amazon Web Services IoT Greengrass. In that case, deploy them as an ML resource.</p> <p>In the request body, you provide the following:</p> <ul> <li> <p>A name for the compilation job</p> </li> <li> <p> Information about the input model artifacts </p> </li> <li> <p>The output location for the compiled model and the device (target) that the model runs on </p> </li> <li> <p>The Amazon Resource Name (ARN) of the IAM role that Amazon SageMaker assumes to perform the model compilation job. </p> </li> </ul> <p>You can also provide a <code>Tag</code> to track the model compilation job's resource use and costs. The response body contains the <code>CompilationJobArn</code> for the compiled job.</p> <p>To stop a model compilation job, use <a>StopCompilationJob</a>. To get information about a particular model compilation job, use <a>DescribeCompilationJob</a>. To get information about multiple model compilation jobs, use <a>ListCompilationJobs</a>.</p>",
+            "documentation": "<p>Starts a model compilation job. After the model has been compiled, Amazon SageMaker saves the resulting model artifacts to an Amazon Simple Storage Service (Amazon S3) bucket that you specify. </p> <p>If you choose to host your model using Amazon SageMaker hosting services, you can use the resulting model artifacts as part of the model. You can also use the artifacts with Amazon Web Services IoT Greengrass. In that case, deploy them as an ML resource.</p> <p>In the request body, you provide the following:</p> <ul> <li> <p>A name for the compilation job</p> </li> <li> <p> Information about the input model artifacts </p> </li> <li> <p>The output location for the compiled model and the device (target) that the model runs on </p> </li> <li> <p>The Amazon Resource Name (ARN) of the IAM role that Amazon SageMaker assumes to perform the model compilation job. </p> </li> </ul> <p>You can also provide a <code>Tag</code> to track the model compilation job's resource use and costs. The response body contains the <code>CompilationJobArn</code> for the compiled job.</p> <p>To stop a model compilation job, use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_StopCompilationJob.html\">StopCompilationJob</a>. To get information about a particular model compilation job, use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeCompilationJob.html\">DescribeCompilationJob</a>. To get information about multiple model compilation jobs, use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ListCompilationJobs.html\">ListCompilationJobs</a>.</p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 },
                 {
                     "shape": "ResourceLimitExceeded"
                 }
@@ -389,15 +389,15 @@
             },
             "input": {
                 "shape": "CreateEdgePackagingJobRequest"
             },
             "name": "CreateEdgePackagingJob"
         },
         "CreateEndpoint": {
-            "documentation": "<p>Creates an endpoint using the endpoint configuration specified in the request. SageMaker uses the endpoint to provision resources and deploy models. You create the endpoint configuration with the <a>CreateEndpointConfig</a> API. </p> <p> Use this API to deploy models using SageMaker hosting services. </p> <p>For an example that calls this method when deploying a model to SageMaker hosting services, see the <a href=\"https://github.com/aws/amazon-sagemaker-examples/blob/master/sagemaker-fundamentals/create-endpoint/create_endpoint.ipynb\">Create Endpoint example notebook.</a> </p> <note> <p> You must not delete an <code>EndpointConfig</code> that is in use by an endpoint that is live or while the <code>UpdateEndpoint</code> or <code>CreateEndpoint</code> operations are being performed on the endpoint. To update an endpoint, you must create a new <code>EndpointConfig</code>.</p> </note> <p>The endpoint name must be unique within an Amazon Web Services Region in your Amazon Web Services account. </p> <p>When it receives the request, SageMaker creates the endpoint, launches the resources (ML compute instances), and deploys the model(s) on them. </p> <note> <p>When you call <a>CreateEndpoint</a>, a load call is made to DynamoDB to verify that your endpoint configuration exists. When you read data from a DynamoDB table supporting <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html\"> <code>Eventually Consistent Reads</code> </a>, the response might not reflect the results of a recently completed write operation. The response might include some stale data. If the dependent entities are not yet in DynamoDB, this causes a validation error. If you repeat your read request after a short time, the response should return the latest data. So retry logic is recommended to handle these possible issues. We also recommend that customers call <a>DescribeEndpointConfig</a> before calling <a>CreateEndpoint</a> to minimize the potential impact of a DynamoDB eventually consistent read.</p> </note> <p>When SageMaker receives the request, it sets the endpoint status to <code>Creating</code>. After it creates the endpoint, it sets the status to <code>InService</code>. SageMaker can then process incoming requests for inferences. To check the status of an endpoint, use the <a>DescribeEndpoint</a> API.</p> <p>If any of the models hosted at this endpoint get model data from an Amazon S3 location, SageMaker uses Amazon Web Services Security Token Service to download model artifacts from the S3 path you provided. Amazon Web Services STS is activated in your Amazon Web Services account by default. If you previously deactivated Amazon Web Services STS for a region, you need to reactivate Amazon Web Services STS for that region. For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_enable-regions.html\">Activating and Deactivating Amazon Web Services STS in an Amazon Web Services Region</a> in the <i>Amazon Web Services Identity and Access Management User Guide</i>.</p> <note> <p> To add the IAM role policies for using this API operation, go to the <a href=\"https://console.aws.amazon.com/iam/\">IAM console</a>, and choose Roles in the left navigation pane. Search the IAM role that you want to grant access to use the <a>CreateEndpoint</a> and <a>CreateEndpointConfig</a> API operations, add the following policies to the role. </p> <ul> <li> <p>Option 1: For a full SageMaker access, search and attach the <code>AmazonSageMakerFullAccess</code> policy.</p> </li> <li> <p>Option 2: For granting a limited access to an IAM role, paste the following Action elements manually into the JSON file of the IAM role: </p> <p> <code>\"Action\": [\"sagemaker:CreateEndpoint\", \"sagemaker:CreateEndpointConfig\"]</code> </p> <p> <code>\"Resource\": [</code> </p> <p> <code>\"arn:aws:sagemaker:region:account-id:endpoint/endpointName\"</code> </p> <p> <code>\"arn:aws:sagemaker:region:account-id:endpoint-config/endpointConfigName\"</code> </p> <p> <code>]</code> </p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/api-permissions-reference.html\">SageMaker API Permissions: Actions, Permissions, and Resources Reference</a>.</p> </li> </ul> </note>",
+            "documentation": "<p>Creates an endpoint using the endpoint configuration specified in the request. SageMaker uses the endpoint to provision resources and deploy models. You create the endpoint configuration with the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpointConfig.html\">CreateEndpointConfig</a> API. </p> <p> Use this API to deploy models using SageMaker hosting services. </p> <p>For an example that calls this method when deploying a model to SageMaker hosting services, see the <a href=\"https://github.com/aws/amazon-sagemaker-examples/blob/master/sagemaker-fundamentals/create-endpoint/create_endpoint.ipynb\">Create Endpoint example notebook.</a> </p> <note> <p> You must not delete an <code>EndpointConfig</code> that is in use by an endpoint that is live or while the <code>UpdateEndpoint</code> or <code>CreateEndpoint</code> operations are being performed on the endpoint. To update an endpoint, you must create a new <code>EndpointConfig</code>.</p> </note> <p>The endpoint name must be unique within an Amazon Web Services Region in your Amazon Web Services account. </p> <p>When it receives the request, SageMaker creates the endpoint, launches the resources (ML compute instances), and deploys the model(s) on them. </p> <note> <p>When you call <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpoint.html\">CreateEndpoint</a>, a load call is made to DynamoDB to verify that your endpoint configuration exists. When you read data from a DynamoDB table supporting <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html\"> <code>Eventually Consistent Reads</code> </a>, the response might not reflect the results of a recently completed write operation. The response might include some stale data. If the dependent entities are not yet in DynamoDB, this causes a validation error. If you repeat your read request after a short time, the response should return the latest data. So retry logic is recommended to handle these possible issues. We also recommend that customers call <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeEndpointConfig.html\">DescribeEndpointConfig</a> before calling <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpoint.html\">CreateEndpoint</a> to minimize the potential impact of a DynamoDB eventually consistent read.</p> </note> <p>When SageMaker receives the request, it sets the endpoint status to <code>Creating</code>. After it creates the endpoint, it sets the status to <code>InService</code>. SageMaker can then process incoming requests for inferences. To check the status of an endpoint, use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeEndpoint.html\">DescribeEndpoint</a> API.</p> <p>If any of the models hosted at this endpoint get model data from an Amazon S3 location, SageMaker uses Amazon Web Services Security Token Service to download model artifacts from the S3 path you provided. Amazon Web Services STS is activated in your Amazon Web Services account by default. If you previously deactivated Amazon Web Services STS for a region, you need to reactivate Amazon Web Services STS for that region. For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_enable-regions.html\">Activating and Deactivating Amazon Web Services STS in an Amazon Web Services Region</a> in the <i>Amazon Web Services Identity and Access Management User Guide</i>.</p> <note> <p> To add the IAM role policies for using this API operation, go to the <a href=\"https://console.aws.amazon.com/iam/\">IAM console</a>, and choose Roles in the left navigation pane. Search the IAM role that you want to grant access to use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpoint.html\">CreateEndpoint</a> and <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpointConfig.html\">CreateEndpointConfig</a> API operations, add the following policies to the role. </p> <ul> <li> <p>Option 1: For a full SageMaker access, search and attach the <code>AmazonSageMakerFullAccess</code> policy.</p> </li> <li> <p>Option 2: For granting a limited access to an IAM role, paste the following Action elements manually into the JSON file of the IAM role: </p> <p> <code>\"Action\": [\"sagemaker:CreateEndpoint\", \"sagemaker:CreateEndpointConfig\"]</code> </p> <p> <code>\"Resource\": [</code> </p> <p> <code>\"arn:aws:sagemaker:region:account-id:endpoint/endpointName\"</code> </p> <p> <code>\"arn:aws:sagemaker:region:account-id:endpoint-config/endpointConfigName\"</code> </p> <p> <code>]</code> </p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/api-permissions-reference.html\">SageMaker API Permissions: Actions, Permissions, and Resources Reference</a>.</p> </li> </ul> </note>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -408,15 +408,15 @@
             },
             "name": "CreateEndpoint",
             "output": {
                 "shape": "CreateEndpointOutput"
             }
         },
         "CreateEndpointConfig": {
-            "documentation": "<p>Creates an endpoint configuration that SageMaker hosting services uses to deploy models. In the configuration, you identify one or more models, created using the <code>CreateModel</code> API, to deploy and the resources that you want SageMaker to provision. Then you call the <a>CreateEndpoint</a> API.</p> <note> <p> Use this API if you want to use SageMaker hosting services to deploy models into production. </p> </note> <p>In the request, you define a <code>ProductionVariant</code>, for each model that you want to deploy. Each <code>ProductionVariant</code> parameter also describes the resources that you want SageMaker to provision. This includes the number and type of ML compute instances to deploy. </p> <p>If you are hosting multiple models, you also assign a <code>VariantWeight</code> to specify how much traffic you want to allocate to each model. For example, suppose that you want to host two models, A and B, and you assign traffic weight 2 for model A and 1 for model B. SageMaker distributes two-thirds of the traffic to Model A, and one-third to model B. </p> <note> <p>When you call <a>CreateEndpoint</a>, a load call is made to DynamoDB to verify that your endpoint configuration exists. When you read data from a DynamoDB table supporting <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html\"> <code>Eventually Consistent Reads</code> </a>, the response might not reflect the results of a recently completed write operation. The response might include some stale data. If the dependent entities are not yet in DynamoDB, this causes a validation error. If you repeat your read request after a short time, the response should return the latest data. So retry logic is recommended to handle these possible issues. We also recommend that customers call <a>DescribeEndpointConfig</a> before calling <a>CreateEndpoint</a> to minimize the potential impact of a DynamoDB eventually consistent read.</p> </note>",
+            "documentation": "<p>Creates an endpoint configuration that SageMaker hosting services uses to deploy models. In the configuration, you identify one or more models, created using the <code>CreateModel</code> API, to deploy and the resources that you want SageMaker to provision. Then you call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpoint.html\">CreateEndpoint</a> API.</p> <note> <p> Use this API if you want to use SageMaker hosting services to deploy models into production. </p> </note> <p>In the request, you define a <code>ProductionVariant</code>, for each model that you want to deploy. Each <code>ProductionVariant</code> parameter also describes the resources that you want SageMaker to provision. This includes the number and type of ML compute instances to deploy. </p> <p>If you are hosting multiple models, you also assign a <code>VariantWeight</code> to specify how much traffic you want to allocate to each model. For example, suppose that you want to host two models, A and B, and you assign traffic weight 2 for model A and 1 for model B. SageMaker distributes two-thirds of the traffic to Model A, and one-third to model B. </p> <note> <p>When you call <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpoint.html\">CreateEndpoint</a>, a load call is made to DynamoDB to verify that your endpoint configuration exists. When you read data from a DynamoDB table supporting <a href=\"https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html\"> <code>Eventually Consistent Reads</code> </a>, the response might not reflect the results of a recently completed write operation. The response might include some stale data. If the dependent entities are not yet in DynamoDB, this causes a validation error. If you repeat your read request after a short time, the response should return the latest data. So retry logic is recommended to handle these possible issues. We also recommend that customers call <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeEndpointConfig.html\">DescribeEndpointConfig</a> before calling <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpoint.html\">CreateEndpoint</a> to minimize the potential impact of a DynamoDB eventually consistent read.</p> </note>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -427,15 +427,15 @@
             },
             "name": "CreateEndpointConfig",
             "output": {
                 "shape": "CreateEndpointConfigOutput"
             }
         },
         "CreateExperiment": {
-            "documentation": "<p>Creates a SageMaker <i>experiment</i>. An experiment is a collection of <i>trials</i> that are observed, compared and evaluated as a group. A trial is a set of steps, called <i>trial components</i>, that produce a machine learning model.</p> <note> <p>In the Studio UI, trials are referred to as <i>run groups</i> and trial components are referred to as <i>runs</i>.</p> </note> <p>The goal of an experiment is to determine the components that produce the best model. Multiple trials are performed, each one isolating and measuring the impact of a change to one or more inputs, while keeping the remaining inputs constant.</p> <p>When you use SageMaker Studio or the SageMaker Python SDK, all experiments, trials, and trial components are automatically tracked, logged, and indexed. When you use the Amazon Web Services SDK for Python (Boto), you must use the logging APIs provided by the SDK.</p> <p>You can add tags to experiments, trials, trial components and then use the <a>Search</a> API to search for the tags.</p> <p>To add a description to an experiment, specify the optional <code>Description</code> parameter. To add a description later, or to change the description, call the <a>UpdateExperiment</a> API.</p> <p>To get a list of all your experiments, call the <a>ListExperiments</a> API. To view an experiment's properties, call the <a>DescribeExperiment</a> API. To get a list of all the trials associated with an experiment, call the <a>ListTrials</a> API. To create a trial call the <a>CreateTrial</a> API.</p>",
+            "documentation": "<p>Creates a SageMaker <i>experiment</i>. An experiment is a collection of <i>trials</i> that are observed, compared and evaluated as a group. A trial is a set of steps, called <i>trial components</i>, that produce a machine learning model.</p> <note> <p>In the Studio UI, trials are referred to as <i>run groups</i> and trial components are referred to as <i>runs</i>.</p> </note> <p>The goal of an experiment is to determine the components that produce the best model. Multiple trials are performed, each one isolating and measuring the impact of a change to one or more inputs, while keeping the remaining inputs constant.</p> <p>When you use SageMaker Studio or the SageMaker Python SDK, all experiments, trials, and trial components are automatically tracked, logged, and indexed. When you use the Amazon Web Services SDK for Python (Boto), you must use the logging APIs provided by the SDK.</p> <p>You can add tags to experiments, trials, trial components and then use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API to search for the tags.</p> <p>To add a description to an experiment, specify the optional <code>Description</code> parameter. To add a description later, or to change the description, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateExperiment.html\">UpdateExperiment</a> API.</p> <p>To get a list of all your experiments, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ListExperiments.html\">ListExperiments</a> API. To view an experiment's properties, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeExperiment.html\">DescribeExperiment</a> API. To get a list of all the trials associated with an experiment, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ListTrials.html\">ListTrials</a> API. To create a trial call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateTrial.html\">CreateTrial</a> API.</p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -943,15 +943,15 @@
             },
             "name": "CreatePresignedDomainUrl",
             "output": {
                 "shape": "CreatePresignedDomainUrlResponse"
             }
         },
         "CreatePresignedNotebookInstanceUrl": {
-            "documentation": "<p>Returns a URL that you can use to connect to the Jupyter server from a notebook instance. In the SageMaker console, when you choose <code>Open</code> next to a notebook instance, SageMaker opens a new tab showing the Jupyter server home page from the notebook instance. The console uses this API to get the URL and show the page.</p> <p> The IAM role or user used to call this API defines the permissions to access the notebook instance. Once the presigned URL is created, no additional permission is required to access this URL. IAM authorization policies for this API are also enforced for every HTTP request and WebSocket frame that attempts to connect to the notebook instance.</p> <p>You can restrict access to this API and to the URL that it returns to a list of IP addresses that you specify. Use the <code>NotIpAddress</code> condition operator and the <code>aws:SourceIP</code> condition context key to specify the list of IP addresses that you want to have access to the notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/security_iam_id-based-policy-examples.html#nbi-ip-filter\">Limit Access to a Notebook Instance by IP Address</a>.</p> <note> <p>The URL that you get from a call to <a>CreatePresignedNotebookInstanceUrl</a> is valid only for 5 minutes. If you try to use the URL after the 5-minute limit expires, you are directed to the Amazon Web Services console sign-in page.</p> </note>",
+            "documentation": "<p>Returns a URL that you can use to connect to the Jupyter server from a notebook instance. In the SageMaker console, when you choose <code>Open</code> next to a notebook instance, SageMaker opens a new tab showing the Jupyter server home page from the notebook instance. The console uses this API to get the URL and show the page.</p> <p> The IAM role or user used to call this API defines the permissions to access the notebook instance. Once the presigned URL is created, no additional permission is required to access this URL. IAM authorization policies for this API are also enforced for every HTTP request and WebSocket frame that attempts to connect to the notebook instance.</p> <p>You can restrict access to this API and to the URL that it returns to a list of IP addresses that you specify. Use the <code>NotIpAddress</code> condition operator and the <code>aws:SourceIP</code> condition context key to specify the list of IP addresses that you want to have access to the notebook instance. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/security_iam_id-based-policy-examples.html#nbi-ip-filter\">Limit Access to a Notebook Instance by IP Address</a>.</p> <note> <p>The URL that you get from a call to <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreatePresignedNotebookInstanceUrl.html\">CreatePresignedNotebookInstanceUrl</a> is valid only for 5 minutes. If you try to use the URL after the 5-minute limit expires, you are directed to the Amazon Web Services console sign-in page.</p> </note>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreatePresignedNotebookInstanceUrlInput"
             },
@@ -1092,15 +1092,15 @@
             },
             "name": "CreateTransformJob",
             "output": {
                 "shape": "CreateTransformJobResponse"
             }
         },
         "CreateTrial": {
-            "documentation": "<p>Creates an SageMaker <i>trial</i>. A trial is a set of steps called <i>trial components</i> that produce a machine learning model. A trial is part of a single SageMaker <i>experiment</i>.</p> <p>When you use SageMaker Studio or the SageMaker Python SDK, all experiments, trials, and trial components are automatically tracked, logged, and indexed. When you use the Amazon Web Services SDK for Python (Boto), you must use the logging APIs provided by the SDK.</p> <p>You can add tags to a trial and then use the <a>Search</a> API to search for the tags.</p> <p>To get a list of all your trials, call the <a>ListTrials</a> API. To view a trial's properties, call the <a>DescribeTrial</a> API. To create a trial component, call the <a>CreateTrialComponent</a> API.</p>",
+            "documentation": "<p>Creates an SageMaker <i>trial</i>. A trial is a set of steps called <i>trial components</i> that produce a machine learning model. A trial is part of a single SageMaker <i>experiment</i>.</p> <p>When you use SageMaker Studio or the SageMaker Python SDK, all experiments, trials, and trial components are automatically tracked, logged, and indexed. When you use the Amazon Web Services SDK for Python (Boto), you must use the logging APIs provided by the SDK.</p> <p>You can add tags to a trial and then use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API to search for the tags.</p> <p>To get a list of all your trials, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ListTrials.html\">ListTrials</a> API. To view a trial's properties, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeTrial.html\">DescribeTrial</a> API. To create a trial component, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateTrialComponent.html\">CreateTrialComponent</a> API.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 },
                 {
                     "shape": "ResourceLimitExceeded"
                 }
@@ -1114,15 +1114,15 @@
             },
             "name": "CreateTrial",
             "output": {
                 "shape": "CreateTrialResponse"
             }
         },
         "CreateTrialComponent": {
-            "documentation": "<p>Creates a <i>trial component</i>, which is a stage of a machine learning <i>trial</i>. A trial is composed of one or more trial components. A trial component can be used in multiple trials.</p> <p>Trial components include pre-processing jobs, training jobs, and batch transform jobs.</p> <p>When you use SageMaker Studio or the SageMaker Python SDK, all experiments, trials, and trial components are automatically tracked, logged, and indexed. When you use the Amazon Web Services SDK for Python (Boto), you must use the logging APIs provided by the SDK.</p> <p>You can add tags to a trial component and then use the <a>Search</a> API to search for the tags.</p>",
+            "documentation": "<p>Creates a <i>trial component</i>, which is a stage of a machine learning <i>trial</i>. A trial is composed of one or more trial components. A trial component can be used in multiple trials.</p> <p>Trial components include pre-processing jobs, training jobs, and batch transform jobs.</p> <p>When you use SageMaker Studio or the SageMaker Python SDK, all experiments, trials, and trial components are automatically tracked, logged, and indexed. When you use the Amazon Web Services SDK for Python (Boto), you must use the logging APIs provided by the SDK.</p> <p>You can add tags to a trial component and then use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API to search for the tags.</p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -1155,15 +1155,15 @@
             },
             "name": "CreateUserProfile",
             "output": {
                 "shape": "CreateUserProfileResponse"
             }
         },
         "CreateWorkforce": {
-            "documentation": "<p>Use this operation to create a workforce. This operation will return an error if a workforce already exists in the Amazon Web Services Region that you specify. You can only create one workforce in each Amazon Web Services Region per Amazon Web Services account.</p> <p>If you want to create a new workforce in an Amazon Web Services Region where a workforce already exists, use the API operation to delete the existing workforce and then use <code>CreateWorkforce</code> to create a new workforce.</p> <p>To create a private workforce using Amazon Cognito, you must specify a Cognito user pool in <code>CognitoConfig</code>. You can also create an Amazon Cognito workforce using the Amazon SageMaker console. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sms-workforce-create-private.html\"> Create a Private Workforce (Amazon Cognito)</a>.</p> <p>To create a private workforce using your own OIDC Identity Provider (IdP), specify your IdP configuration in <code>OidcConfig</code>. Your OIDC IdP must support <i>groups</i> because groups are used by Ground Truth and Amazon A2I to create work teams. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sms-workforce-create-private-oidc.html\"> Create a Private Workforce (OIDC IdP)</a>.</p>",
+            "documentation": "<p>Use this operation to create a workforce. This operation will return an error if a workforce already exists in the Amazon Web Services Region that you specify. You can only create one workforce in each Amazon Web Services Region per Amazon Web Services account.</p> <p>If you want to create a new workforce in an Amazon Web Services Region where a workforce already exists, use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DeleteWorkforce.html\">DeleteWorkforce</a> API operation to delete the existing workforce and then use <code>CreateWorkforce</code> to create a new workforce.</p> <p>To create a private workforce using Amazon Cognito, you must specify a Cognito user pool in <code>CognitoConfig</code>. You can also create an Amazon Cognito workforce using the Amazon SageMaker console. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sms-workforce-create-private.html\"> Create a Private Workforce (Amazon Cognito)</a>.</p> <p>To create a private workforce using your own OIDC Identity Provider (IdP), specify your IdP configuration in <code>OidcConfig</code>. Your OIDC IdP must support <i>groups</i> because groups are used by Ground Truth and Amazon A2I to create work teams. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sms-workforce-create-private-oidc.html\"> Create a Private Workforce (OIDC IdP)</a>.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreateWorkforceRequest"
             },
@@ -1429,15 +1429,15 @@
             },
             "input": {
                 "shape": "DeleteEndpointConfigInput"
             },
             "name": "DeleteEndpointConfig"
         },
         "DeleteExperiment": {
-            "documentation": "<p>Deletes an SageMaker experiment. All trials associated with the experiment must be deleted first. Use the <a>ListTrials</a> API to get a list of the trials associated with the experiment.</p>",
+            "documentation": "<p>Deletes an SageMaker experiment. All trials associated with the experiment must be deleted first. Use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ListTrials.html\">ListTrials</a> API to get a list of the trials associated with the experiment.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -1524,15 +1524,15 @@
             },
             "input": {
                 "shape": "DeleteHubContentRequest"
             },
             "name": "DeleteHubContent"
         },
         "DeleteHumanTaskUi": {
-            "documentation": "<p>Use this operation to delete a human task user interface (worker task template).</p> <p> To see a list of human task user interfaces (work task templates) in your account, use . When you delete a worker task template, it no longer appears when you call <code>ListHumanTaskUis</code>.</p>",
+            "documentation": "<p>Use this operation to delete a human task user interface (worker task template).</p> <p> To see a list of human task user interfaces (work task templates) in your account, use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ListHumanTaskUis.html\">ListHumanTaskUis</a>. When you delete a worker task template, it no longer appears when you call <code>ListHumanTaskUis</code>.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -1855,15 +1855,15 @@
             },
             "name": "DeleteTags",
             "output": {
                 "shape": "DeleteTagsOutput"
             }
         },
         "DeleteTrial": {
-            "documentation": "<p>Deletes the specified trial. All trial components that make up the trial must be deleted first. Use the <a>DescribeTrialComponent</a> API to get the list of trial components.</p>",
+            "documentation": "<p>Deletes the specified trial. All trial components that make up the trial must be deleted first. Use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeTrialComponent.html\">DescribeTrialComponent</a> API to get the list of trial components.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -1874,15 +1874,15 @@
             },
             "name": "DeleteTrial",
             "output": {
                 "shape": "DeleteTrialResponse"
             }
         },
         "DeleteTrialComponent": {
-            "documentation": "<p>Deletes the specified trial component. A trial component must be disassociated from all trials before the trial component can be deleted. To disassociate a trial component from a trial, call the <a>DisassociateTrialComponent</a> API.</p>",
+            "documentation": "<p>Deletes the specified trial component. A trial component must be disassociated from all trials before the trial component can be deleted. To disassociate a trial component from a trial, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DisassociateTrialComponent.html\">DisassociateTrialComponent</a> API.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -1912,15 +1912,15 @@
             },
             "input": {
                 "shape": "DeleteUserProfileRequest"
             },
             "name": "DeleteUserProfile"
         },
         "DeleteWorkforce": {
-            "documentation": "<p>Use this operation to delete a workforce.</p> <p>If you want to create a new workforce in an Amazon Web Services Region where a workforce already exists, use this operation to delete the existing workforce and then use to create a new workforce.</p> <important> <p>If a private workforce contains one or more work teams, you must use the operation to delete all work teams before you delete the workforce. If you try to delete a workforce that contains one or more work teams, you will recieve a <code>ResourceInUse</code> error.</p> </important>",
+            "documentation": "<p>Use this operation to delete a workforce.</p> <p>If you want to create a new workforce in an Amazon Web Services Region where a workforce already exists, use this operation to delete the existing workforce and then use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateWorkforce.html\">CreateWorkforce</a> to create a new workforce.</p> <important> <p>If a private workforce contains one or more work teams, you must use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DeleteWorkteam.html\">DeleteWorkteam</a> operation to delete all work teams before you delete the workforce. If you try to delete a workforce that contains one or more work teams, you will recieve a <code>ResourceInUse</code> error.</p> </important>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteWorkforceRequest"
             },
@@ -2046,15 +2046,15 @@
             },
             "name": "DescribeArtifact",
             "output": {
                 "shape": "DescribeArtifactResponse"
             }
         },
         "DescribeAutoMLJob": {
-            "documentation": "<p>Returns information about an Amazon SageMaker AutoML job.</p>",
+            "documentation": "<p>Returns information about an AutoML job created by calling <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJob.html\">CreateAutoMLJob</a>.</p> <note> <p>AutoML jobs created by calling <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJobV2.html\">CreateAutoMLJobV2</a> cannot be described by <code>DescribeAutoMLJob</code>.</p> </note>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -2065,15 +2065,15 @@
             },
             "name": "DescribeAutoMLJob",
             "output": {
                 "shape": "DescribeAutoMLJobResponse"
             }
         },
         "DescribeAutoMLJobV2": {
-            "documentation": "<p>Returns information about an Amazon SageMaker AutoML V2 job.</p> <note> <p>This API action is callable through SageMaker Canvas only. Calling it directly from the CLI or an SDK results in an error.</p> </note>",
+            "documentation": "<p>Returns information about an AutoML job created by calling <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJobV2.html\">CreateAutoMLJobV2</a> or <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJob.html\">CreateAutoMLJob</a>.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -2098,15 +2098,15 @@
             },
             "name": "DescribeCodeRepository",
             "output": {
                 "shape": "DescribeCodeRepositoryOutput"
             }
         },
         "DescribeCompilationJob": {
-            "documentation": "<p>Returns information about a model compilation job.</p> <p>To create a model compilation job, use <a>CreateCompilationJob</a>. To get information about multiple model compilation jobs, use <a>ListCompilationJobs</a>.</p>",
+            "documentation": "<p>Returns information about a model compilation job.</p> <p>To create a model compilation job, use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateCompilationJob.html\">CreateCompilationJob</a>. To get information about multiple model compilation jobs, use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ListCompilationJobs.html\">ListCompilationJobs</a>.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -2411,15 +2411,15 @@
             },
             "name": "DescribeHumanTaskUi",
             "output": {
                 "shape": "DescribeHumanTaskUiResponse"
             }
         },
         "DescribeHyperParameterTuningJob": {
-            "documentation": "<p>Gets a description of a hyperparameter tuning job.</p>",
+            "documentation": "<p>Returns a description of a hyperparameter tuning job, depending on the fields selected. These fields can include the name, Amazon Resource Name (ARN), job status of your tuning job and more.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -3007,15 +3007,15 @@
             },
             "name": "DisableSagemakerServicecatalogPortfolio",
             "output": {
                 "shape": "DisableSagemakerServicecatalogPortfolioOutput"
             }
         },
         "DisassociateTrialComponent": {
-            "documentation": "<p>Disassociates a trial component from a trial. This doesn't effect other trials the component is associated with. Before you can delete a component, you must disassociate the component from all trials it is associated with. To associate a trial component with a trial, call the <a>AssociateTrialComponent</a> API.</p> <p>To get a list of the trials a component is associated with, use the <a>Search</a> API. Specify <code>ExperimentTrialComponent</code> for the <code>Resource</code> parameter. The list appears in the response under <code>Results.TrialComponent.Parents</code>.</p>",
+            "documentation": "<p>Disassociates a trial component from a trial. This doesn't effect other trials the component is associated with. Before you can delete a component, you must disassociate the component from all trials it is associated with. To associate a trial component with a trial, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AssociateTrialComponent.html\">AssociateTrialComponent</a> API.</p> <p>To get a list of the trials a component is associated with, use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API. Specify <code>ExperimentTrialComponent</code> for the <code>Resource</code> parameter. The list appears in the response under <code>Results.TrialComponent.Parents</code>.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -3305,15 +3305,15 @@
             },
             "name": "ListCodeRepositories",
             "output": {
                 "shape": "ListCodeRepositoriesOutput"
             }
         },
         "ListCompilationJobs": {
-            "documentation": "<p>Lists model compilation jobs that satisfy various filters.</p> <p>To create a model compilation job, use <a>CreateCompilationJob</a>. To get information about a particular model compilation job you have created, use <a>DescribeCompilationJob</a>.</p>",
+            "documentation": "<p>Lists model compilation jobs that satisfy various filters.</p> <p>To create a model compilation job, use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateCompilationJob.html\">CreateCompilationJob</a>. To get information about a particular model compilation job you have created, use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeCompilationJob.html\">DescribeCompilationJob</a>.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListCompilationJobsRequest"
             },
@@ -3558,15 +3558,15 @@
             },
             "name": "ListHumanTaskUis",
             "output": {
                 "shape": "ListHumanTaskUisResponse"
             }
         },
         "ListHyperParameterTuningJobs": {
-            "documentation": "<p>Gets a list of <a>HyperParameterTuningJobSummary</a> objects that describe the hyperparameter tuning jobs launched in your account.</p>",
+            "documentation": "<p>Gets a list of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobSummary.html\">HyperParameterTuningJobSummary</a> objects that describe the hyperparameter tuning jobs launched in your account.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListHyperParameterTuningJobsRequest"
             },
@@ -3910,15 +3910,15 @@
             },
             "name": "ListMonitoringSchedules",
             "output": {
                 "shape": "ListMonitoringSchedulesResponse"
             }
         },
         "ListNotebookInstanceLifecycleConfigs": {
-            "documentation": "<p>Lists notebook instance lifestyle configurations created with the <a>CreateNotebookInstanceLifecycleConfig</a> API.</p>",
+            "documentation": "<p>Lists notebook instance lifestyle configurations created with the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateNotebookInstanceLifecycleConfig.html\">CreateNotebookInstanceLifecycleConfig</a> API.</p>",
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListNotebookInstanceLifecycleConfigsInput"
             },
@@ -4126,15 +4126,15 @@
             },
             "name": "ListTrainingJobs",
             "output": {
                 "shape": "ListTrainingJobsResponse"
             }
         },
         "ListTrainingJobsForHyperParameterTuningJob": {
-            "documentation": "<p>Gets a list of <a>TrainingJobSummary</a> objects that describe the training jobs that a hyperparameter tuning job launched.</p>",
+            "documentation": "<p>Gets a list of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_TrainingJobSummary.html\">TrainingJobSummary</a> objects that describe the training jobs that a hyperparameter tuning job launched.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -4493,15 +4493,15 @@
             },
             "input": {
                 "shape": "StopAutoMLJobRequest"
             },
             "name": "StopAutoMLJob"
         },
         "StopCompilationJob": {
-            "documentation": "<p>Stops a model compilation job.</p> <p> To stop a job, Amazon SageMaker sends the algorithm the SIGTERM signal. This gracefully shuts the job down. If the job hasn't stopped, it sends the SIGKILL signal.</p> <p>When it receives a <code>StopCompilationJob</code> request, Amazon SageMaker changes the <a>CompilationJobSummary$CompilationJobStatus</a> of the job to <code>Stopping</code>. After Amazon SageMaker stops the job, it sets the <a>CompilationJobSummary$CompilationJobStatus</a> to <code>Stopped</code>. </p>",
+            "documentation": "<p>Stops a model compilation job.</p> <p> To stop a job, Amazon SageMaker sends the algorithm the SIGTERM signal. This gracefully shuts the job down. If the job hasn't stopped, it sends the SIGKILL signal.</p> <p>When it receives a <code>StopCompilationJob</code> request, Amazon SageMaker changes the <code>CompilationJobStatus</code> of the job to <code>Stopping</code>. After Amazon SageMaker stops the job, it sets the <code>CompilationJobStatus</code> to <code>Stopped</code>. </p>",
             "errors": [
                 {
                     "shape": "ResourceNotFound"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -4846,15 +4846,15 @@
             },
             "name": "UpdateDomain",
             "output": {
                 "shape": "UpdateDomainResponse"
             }
         },
         "UpdateEndpoint": {
-            "documentation": "<p>Deploys the new <code>EndpointConfig</code> specified in the request, switches to using newly created endpoint, and then deletes resources provisioned for the endpoint using the previous <code>EndpointConfig</code> (there is no availability loss). </p> <p>When SageMaker receives the request, it sets the endpoint status to <code>Updating</code>. After updating the endpoint, it sets the status to <code>InService</code>. To check the status of an endpoint, use the <a>DescribeEndpoint</a> API. </p> <note> <p>You must not delete an <code>EndpointConfig</code> in use by an endpoint that is live or while the <code>UpdateEndpoint</code> or <code>CreateEndpoint</code> operations are being performed on the endpoint. To update an endpoint, you must create a new <code>EndpointConfig</code>.</p> <p>If you delete the <code>EndpointConfig</code> of an endpoint that is active or being created or updated you may lose visibility into the instance type the endpoint is using. The endpoint must be deleted in order to stop incurring charges.</p> </note>",
+            "documentation": "<p>Deploys the new <code>EndpointConfig</code> specified in the request, switches to using newly created endpoint, and then deletes resources provisioned for the endpoint using the previous <code>EndpointConfig</code> (there is no availability loss). </p> <p>When SageMaker receives the request, it sets the endpoint status to <code>Updating</code>. After updating the endpoint, it sets the status to <code>InService</code>. To check the status of an endpoint, use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeEndpoint.html\">DescribeEndpoint</a> API. </p> <note> <p>You must not delete an <code>EndpointConfig</code> in use by an endpoint that is live or while the <code>UpdateEndpoint</code> or <code>CreateEndpoint</code> operations are being performed on the endpoint. To update an endpoint, you must create a new <code>EndpointConfig</code>.</p> <p>If you delete the <code>EndpointConfig</code> of an endpoint that is active or being created or updated you may lose visibility into the instance type the endpoint is using. The endpoint must be deleted in order to stop incurring charges.</p> </note>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -4865,15 +4865,15 @@
             },
             "name": "UpdateEndpoint",
             "output": {
                 "shape": "UpdateEndpointOutput"
             }
         },
         "UpdateEndpointWeightsAndCapacities": {
-            "documentation": "<p>Updates variant weight of one or more variants associated with an existing endpoint, or capacity of one variant associated with an existing endpoint. When it receives the request, SageMaker sets the endpoint status to <code>Updating</code>. After updating the endpoint, it sets the status to <code>InService</code>. To check the status of an endpoint, use the <a>DescribeEndpoint</a> API. </p>",
+            "documentation": "<p>Updates variant weight of one or more variants associated with an existing endpoint, or capacity of one variant associated with an existing endpoint. When it receives the request, SageMaker sets the endpoint status to <code>Updating</code>. After updating the endpoint, it sets the status to <code>InService</code>. To check the status of an endpoint, use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeEndpoint.html\">DescribeEndpoint</a> API. </p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -4960,15 +4960,15 @@
             },
             "name": "UpdateHub",
             "output": {
                 "shape": "UpdateHubResponse"
             }
         },
         "UpdateImage": {
-            "documentation": "<p>Updates the properties of a SageMaker image. To change the image's tags, use the <a>AddTags</a> and <a>DeleteTags</a> APIs.</p>",
+            "documentation": "<p>Updates the properties of a SageMaker image. To change the image's tags, use the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AddTags.html\">AddTags</a> and <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DeleteTags.html\">DeleteTags</a> APIs.</p>",
             "errors": [
                 {
                     "shape": "ResourceInUse"
                 },
                 {
                     "shape": "ResourceNotFound"
                 }
@@ -5004,15 +5004,15 @@
             },
             "name": "UpdateImageVersion",
             "output": {
                 "shape": "UpdateImageVersionResponse"
             }
         },
         "UpdateInferenceExperiment": {
-            "documentation": "<p> Updates an inference experiment that you created. The status of the inference experiment has to be either <code>Created</code>, <code>Running</code>. For more information on the status of an inference experiment, see <a>DescribeInferenceExperimentResponse$Status</a>. </p>",
+            "documentation": "<p> Updates an inference experiment that you created. The status of the inference experiment has to be either <code>Created</code>, <code>Running</code>. For more information on the status of an inference experiment, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeInferenceExperiment.html\">DescribeInferenceExperiment</a>. </p>",
             "errors": [
                 {
                     "shape": "ConflictException"
                 },
                 {
                     "shape": "ResourceNotFound"
                 }
@@ -5128,15 +5128,15 @@
             },
             "name": "UpdateNotebookInstance",
             "output": {
                 "shape": "UpdateNotebookInstanceOutput"
             }
         },
         "UpdateNotebookInstanceLifecycleConfig": {
-            "documentation": "<p>Updates a notebook instance lifecycle configuration created with the <a>CreateNotebookInstanceLifecycleConfig</a> API.</p>",
+            "documentation": "<p>Updates a notebook instance lifecycle configuration created with the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateNotebookInstanceLifecycleConfig.html\">CreateNotebookInstanceLifecycleConfig</a> API.</p>",
             "errors": [
                 {
                     "shape": "ResourceLimitExceeded"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -5312,15 +5312,15 @@
             },
             "name": "UpdateUserProfile",
             "output": {
                 "shape": "UpdateUserProfileResponse"
             }
         },
         "UpdateWorkforce": {
-            "documentation": "<p>Use this operation to update your workforce. You can use this operation to require that workers use specific IP addresses to work on tasks and to update your OpenID Connect (OIDC) Identity Provider (IdP) workforce configuration.</p> <p>The worker portal is now supported in VPC and public internet.</p> <p> Use <code>SourceIpConfig</code> to restrict worker access to tasks to a specific range of IP addresses. You specify allowed IP addresses by creating a list of up to ten <a href=\"https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html\">CIDRs</a>. By default, a workforce isn't restricted to specific IP addresses. If you specify a range of IP addresses, workers who attempt to access tasks using any IP address outside the specified range are denied and get a <code>Not Found</code> error message on the worker portal.</p> <p>To restrict access to all the workers in public internet, add the <code>SourceIpConfig</code> CIDR value as \"10.0.0.0/16\".</p> <important> <p>Amazon SageMaker does not support Source Ip restriction for worker portals in VPC.</p> </important> <p>Use <code>OidcConfig</code> to update the configuration of a workforce created using your own OIDC IdP. </p> <important> <p>You can only update your OIDC IdP configuration when there are no work teams associated with your workforce. You can delete work teams using the operation.</p> </important> <p>After restricting access to a range of IP addresses or updating your OIDC IdP configuration with this operation, you can view details about your update workforce using the operation.</p> <important> <p>This operation only applies to private workforces.</p> </important>",
+            "documentation": "<p>Use this operation to update your workforce. You can use this operation to require that workers use specific IP addresses to work on tasks and to update your OpenID Connect (OIDC) Identity Provider (IdP) workforce configuration.</p> <p>The worker portal is now supported in VPC and public internet.</p> <p> Use <code>SourceIpConfig</code> to restrict worker access to tasks to a specific range of IP addresses. You specify allowed IP addresses by creating a list of up to ten <a href=\"https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html\">CIDRs</a>. By default, a workforce isn't restricted to specific IP addresses. If you specify a range of IP addresses, workers who attempt to access tasks using any IP address outside the specified range are denied and get a <code>Not Found</code> error message on the worker portal.</p> <p>To restrict access to all the workers in public internet, add the <code>SourceIpConfig</code> CIDR value as \"10.0.0.0/16\".</p> <important> <p>Amazon SageMaker does not support Source Ip restriction for worker portals in VPC.</p> </important> <p>Use <code>OidcConfig</code> to update the configuration of a workforce created using your own OIDC IdP. </p> <important> <p>You can only update your OIDC IdP configuration when there are no work teams associated with your workforce. You can delete work teams using the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DeleteWorkteam.html\">DeleteWorkteam</a> operation.</p> </important> <p>After restricting access to a range of IP addresses or updating your OIDC IdP configuration with this operation, you can view details about your update workforce using the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeWorkforce.html\">DescribeWorkforce</a> operation.</p> <important> <p>This operation only applies to private workforces.</p> </important>",
             "errors": [
                 {
                     "shape": "ConflictException"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -5574,14 +5574,35 @@
         },
         "AgentVersions": {
             "member": {
                 "shape": "AgentVersion"
             },
             "type": "list"
         },
+        "AggregationTransformationValue": {
+            "enum": [
+                "sum",
+                "avg",
+                "first",
+                "min",
+                "max"
+            ],
+            "type": "string"
+        },
+        "AggregationTransformations": {
+            "key": {
+                "shape": "TransformationAttributeName"
+            },
+            "max": 50,
+            "min": 1,
+            "type": "map",
+            "value": {
+                "shape": "AggregationTransformationValue"
+            }
+        },
         "Alarm": {
             "documentation": "<p>An Amazon CloudWatch alarm configured to monitor metrics on an endpoint.</p>",
             "members": {
                 "AlarmName": {
                     "documentation": "<p>The name of a CloudWatch alarm in your account.</p>",
                     "shape": "AlarmName"
                 }
@@ -5617,30 +5638,30 @@
             "enum": [
                 "Name",
                 "CreationTime"
             ],
             "type": "string"
         },
         "AlgorithmSpecification": {
-            "documentation": "<p>Specifies the training algorithm to use in a <a>CreateTrainingJob</a> request.</p> <p>For more information about algorithms provided by SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/algos.html\">Algorithms</a>. For information about using your own algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>. </p>",
+            "documentation": "<p>Specifies the training algorithm to use in a <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateTrainingJob.html\">CreateTrainingJob</a> request.</p> <p>For more information about algorithms provided by SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/algos.html\">Algorithms</a>. For information about using your own algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>. </p>",
             "members": {
                 "AlgorithmName": {
                     "documentation": "<p>The name of the algorithm resource to use for the training job. This must be an algorithm resource that you created or subscribe to on Amazon Web Services Marketplace.</p> <note> <p>You must specify either the algorithm name to the <code>AlgorithmName</code> parameter or the image URI of the algorithm container to the <code>TrainingImage</code> parameter.</p> <p>Note that the <code>AlgorithmName</code> parameter is mutually exclusive with the <code>TrainingImage</code> parameter. If you specify a value for the <code>AlgorithmName</code> parameter, you can't specify a value for <code>TrainingImage</code>, and vice versa.</p> <p>If you specify values for both parameters, the training job might break; if you don't specify any value for both parameters, the training job might raise a <code>null</code> error.</p> </note>",
                     "shape": "ArnOrName"
                 },
                 "ContainerArguments": {
                     "documentation": "<p>The arguments for a container used to run a training job. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms-training-algo-dockerfile.html\">How Amazon SageMaker Runs Your Training Image</a> for additional information.</p>",
                     "shape": "TrainingContainerArguments"
                 },
                 "ContainerEntrypoint": {
                     "documentation": "<p>The <a href=\"https://docs.docker.com/engine/reference/builder/\">entrypoint script for a Docker container</a> used to run a training job. This script takes precedence over the default train processing instructions. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms-training-algo-dockerfile.html\">How Amazon SageMaker Runs Your Training Image</a> for more information.</p>",
                     "shape": "TrainingContainerEntrypoint"
                 },
                 "EnableSageMakerMetricsTimeSeries": {
-                    "documentation": "<p>To generate and save time-series metrics during training, set to <code>true</code>. The default is <code>false</code> and time-series metrics aren't generated except in the following cases:</p> <ul> <li> <p>You use one of the SageMaker built-in algorithms</p> </li> <li> <p>You use one of the following <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/pre-built-containers-frameworks-deep-learning.html\">Prebuilt SageMaker Docker Images</a>:</p> <ul> <li> <p>Tensorflow (version &gt;= 1.15)</p> </li> <li> <p>MXNet (version &gt;= 1.6)</p> </li> <li> <p>PyTorch (version &gt;= 1.3)</p> </li> </ul> </li> <li> <p>You specify at least one <a>MetricDefinition</a> </p> </li> </ul>",
+                    "documentation": "<p>To generate and save time-series metrics during training, set to <code>true</code>. The default is <code>false</code> and time-series metrics aren't generated except in the following cases:</p> <ul> <li> <p>You use one of the SageMaker built-in algorithms</p> </li> <li> <p>You use one of the following <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/pre-built-containers-frameworks-deep-learning.html\">Prebuilt SageMaker Docker Images</a>:</p> <ul> <li> <p>Tensorflow (version &gt;= 1.15)</p> </li> <li> <p>MXNet (version &gt;= 1.6)</p> </li> <li> <p>PyTorch (version &gt;= 1.3)</p> </li> </ul> </li> <li> <p>You specify at least one <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_MetricDefinition.html\">MetricDefinition</a> </p> </li> </ul>",
                     "shape": "Boolean"
                 },
                 "MetricDefinitions": {
                     "documentation": "<p>A list of metric definition objects. Each object specifies the metric name and regular expressions used to parse algorithm logs. SageMaker publishes each metric to Amazon CloudWatch.</p>",
                     "shape": "MetricDefinitionList"
                 },
                 "TrainingImage": {
@@ -5955,15 +5976,17 @@
                 "ml.g5.2xlarge",
                 "ml.g5.4xlarge",
                 "ml.g5.8xlarge",
                 "ml.g5.16xlarge",
                 "ml.g5.12xlarge",
                 "ml.g5.24xlarge",
                 "ml.g5.48xlarge",
-                "ml.geospatial.interactive"
+                "ml.geospatial.interactive",
+                "ml.p4d.24xlarge",
+                "ml.p4de.24xlarge"
             ],
             "type": "string"
         },
         "AppList": {
             "member": {
                 "shape": "AppDetails"
             },
@@ -6272,14 +6295,18 @@
         "AsyncInferenceNotificationConfig": {
             "documentation": "<p>Specifies the configuration for notifications of inference results for asynchronous inference.</p>",
             "members": {
                 "ErrorTopic": {
                     "documentation": "<p>Amazon SNS topic to post a notification to when inference fails. If no topic is provided, no notification is sent on failure.</p>",
                     "shape": "SnsTopicArn"
                 },
+                "IncludeInferenceResponseIn": {
+                    "documentation": "<p>The Amazon SNS topics where you want the inference response to be included.</p> <note> <p>The inference response is included only if the response size is less than or equal to 128 KB.</p> </note>",
+                    "shape": "AsyncNotificationTopicTypeList"
+                },
                 "SuccessTopic": {
                     "documentation": "<p>Amazon SNS topic to post a notification to when inference completes successfully. If no topic is provided, no notification is sent on success.</p>",
                     "shape": "SnsTopicArn"
                 }
             },
             "type": "structure"
         },
@@ -6290,24 +6317,40 @@
                     "documentation": "<p>The Amazon Web Services Key Management Service (Amazon Web Services KMS) key that SageMaker uses to encrypt the asynchronous inference output in Amazon S3.</p> <p/>",
                     "shape": "KmsKeyId"
                 },
                 "NotificationConfig": {
                     "documentation": "<p>Specifies the configuration for notifications of inference results for asynchronous inference.</p>",
                     "shape": "AsyncInferenceNotificationConfig"
                 },
+                "S3FailurePath": {
+                    "documentation": "<p>The Amazon S3 location to upload failure inference responses to.</p>",
+                    "shape": "DestinationS3Uri"
+                },
                 "S3OutputPath": {
                     "documentation": "<p>The Amazon S3 location to upload inference responses to.</p>",
                     "shape": "DestinationS3Uri"
                 }
             },
-            "required": [
-                "S3OutputPath"
-            ],
             "type": "structure"
         },
+        "AsyncNotificationTopicTypeList": {
+            "max": 2,
+            "member": {
+                "shape": "AsyncNotificationTopicTypes"
+            },
+            "min": 0,
+            "type": "list"
+        },
+        "AsyncNotificationTopicTypes": {
+            "enum": [
+                "SUCCESS_NOTIFICATION_TOPIC",
+                "ERROR_NOTIFICATION_TOPIC"
+            ],
+            "type": "string"
+        },
         "AthenaCatalog": {
             "documentation": "<p>The name of the data catalog used in Athena query execution.</p>",
             "max": 256,
             "min": 1,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\t]*",
             "type": "string"
         },
@@ -6428,15 +6471,15 @@
             ],
             "type": "string"
         },
         "AutoMLAlgorithmConfig": {
             "documentation": "<p>The collection of algorithms run on a dataset for training the model candidates of an Autopilot job.</p>",
             "members": {
                 "AutoMLAlgorithms": {
-                    "documentation": "<p>The selection of algorithms run on a dataset to train the model candidates of an Autopilot job. </p> <note> <p>Selected algorithms must belong to the list corresponding to the training mode set in <code> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AutoMLJobConfig.html#sagemaker-Type-AutoMLJobConfig-Mode\">AutoMLJobConfig.Mode</a> </code> (<code>ENSEMBLING</code> or <code>HYPERPARAMETER_TUNING</code>). Choose a minimum of 1 algorithm. </p> </note> <ul> <li> <p>In <code>ENSEMBLING</code> mode:</p> <ul> <li> <p>\"catboost\"</p> </li> <li> <p>\"extra-trees\"</p> </li> <li> <p>\"fastai\"</p> </li> <li> <p>\"lightgbm\"</p> </li> <li> <p>\"linear-learner\"</p> </li> <li> <p>\"nn-torch\"</p> </li> <li> <p>\"randomforest\"</p> </li> <li> <p>\"xgboost\"</p> </li> </ul> </li> <li> <p>In <code>HYPERPARAMETER_TUNING</code> mode:</p> <ul> <li> <p>\"linear-learner\"</p> </li> <li> <p>\"mlp\"</p> </li> <li> <p>\"xgboost\"</p> </li> </ul> </li> </ul>",
+                    "documentation": "<p>The selection of algorithms run on a dataset to train the model candidates of an Autopilot job. </p> <note> <p>Selected algorithms must belong to the list corresponding to the training mode set in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AutoMLJobConfig.html#sagemaker-Type-AutoMLJobConfig-Mode\">AutoMLJobConfig.Mode</a> (<code>ENSEMBLING</code> or <code>HYPERPARAMETER_TUNING</code>). Choose a minimum of 1 algorithm. </p> </note> <ul> <li> <p>In <code>ENSEMBLING</code> mode:</p> <ul> <li> <p>\"catboost\"</p> </li> <li> <p>\"extra-trees\"</p> </li> <li> <p>\"fastai\"</p> </li> <li> <p>\"lightgbm\"</p> </li> <li> <p>\"linear-learner\"</p> </li> <li> <p>\"nn-torch\"</p> </li> <li> <p>\"randomforest\"</p> </li> <li> <p>\"xgboost\"</p> </li> </ul> </li> <li> <p>In <code>HYPERPARAMETER_TUNING</code> mode:</p> <ul> <li> <p>\"linear-learner\"</p> </li> <li> <p>\"mlp\"</p> </li> <li> <p>\"xgboost\"</p> </li> </ul> </li> </ul>",
                     "shape": "AutoMLAlgorithms"
                 }
             },
             "required": [
                 "AutoMLAlgorithms"
             ],
             "type": "structure"
@@ -6486,15 +6529,15 @@
                     "documentation": "<p>The failure reason.</p>",
                     "shape": "AutoMLFailureReason"
                 },
                 "FinalAutoMLJobObjectiveMetric": {
                     "shape": "FinalAutoMLJobObjectiveMetric"
                 },
                 "InferenceContainerDefinitions": {
-                    "documentation": "<p>The mapping of all supported processing unit (CPU, GPU, etc...) to inference container definitions for the candidate. This field is populated for the V2 API only (for example, for jobs created by calling <code>CreateAutoMLJobV2</code>).</p>",
+                    "documentation": "<p>The mapping of all supported processing unit (CPU, GPU, etc...) to inference container definitions for the candidate. This field is populated for the AutoML jobs V2 (for example, for jobs created by calling <code>CreateAutoMLJobV2</code>) related to image or text classification problem types only.</p>",
                     "shape": "AutoMLInferenceContainerDefinitions"
                 },
                 "InferenceContainers": {
                     "documentation": "<p>Information about the recommended inference container definitions.</p>",
                     "shape": "AutoMLContainerDefinitions"
                 },
                 "LastModifiedTime": {
@@ -6516,15 +6559,15 @@
             ],
             "type": "structure"
         },
         "AutoMLCandidateGenerationConfig": {
             "documentation": "<p>Stores the configuration information for how a candidate is generated (optional).</p>",
             "members": {
                 "AlgorithmsConfig": {
-                    "documentation": "<p>Stores the configuration information for the selection of algorithms used to train the model candidates.</p> <p>The list of available algorithms to choose from depends on the training mode set in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AutoMLJobConfig.html\"> <code>AutoMLJobConfig.Mode</code> </a>.</p> <ul> <li> <p> <code>AlgorithmsConfig</code> should not be set in <code>AUTO</code> training mode.</p> </li> <li> <p>When <code>AlgorithmsConfig</code> is provided, one <code>AutoMLAlgorithms</code> attribute must be set and one only.</p> <p>If the list of algorithms provided as values for <code>AutoMLAlgorithms</code> is empty, <code>AutoMLCandidateGenerationConfig</code> uses the full set of algorithms for the given training mode.</p> </li> <li> <p>When <code>AlgorithmsConfig</code> is not provided, <code>AutoMLCandidateGenerationConfig</code> uses the full set of algorithms for the given training mode.</p> </li> </ul> <p>For the list of all algorithms per training mode, see .</p> <p>For more information on each algorithm, see the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-model-support-validation.html#autopilot-algorithm-support\">Algorithm support</a> section in Autopilot developer guide.</p>",
+                    "documentation": "<p>Stores the configuration information for the selection of algorithms used to train the model candidates.</p> <p>The list of available algorithms to choose from depends on the training mode set in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AutoMLJobConfig.html\"> <code>AutoMLJobConfig.Mode</code> </a>.</p> <ul> <li> <p> <code>AlgorithmsConfig</code> should not be set in <code>AUTO</code> training mode.</p> </li> <li> <p>When <code>AlgorithmsConfig</code> is provided, one <code>AutoMLAlgorithms</code> attribute must be set and one only.</p> <p>If the list of algorithms provided as values for <code>AutoMLAlgorithms</code> is empty, <code>AutoMLCandidateGenerationConfig</code> uses the full set of algorithms for the given training mode.</p> </li> <li> <p>When <code>AlgorithmsConfig</code> is not provided, <code>AutoMLCandidateGenerationConfig</code> uses the full set of algorithms for the given training mode.</p> </li> </ul> <p>For the list of all algorithms per training mode, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AutoMLAlgorithmConfig.html\"> AutoMLAlgorithmConfig</a>.</p> <p>For more information on each algorithm, see the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-model-support-validation.html#autopilot-algorithm-support\">Algorithm support</a> section in Autopilot developer guide.</p>",
                     "shape": "AutoMLAlgorithmsConfig"
                 },
                 "FeatureSpecificationS3Uri": {
                     "documentation": "<p>A URL to the Amazon S3 data source containing selected features from the input data source to run an Autopilot job. You can input <code>FeatureAttributeNames</code> (optional) in JSON format as shown below: </p> <p> <code>{ \"FeatureAttributeNames\":[\"col1\", \"col2\", ...] }</code>.</p> <p>You can also specify the data type of the feature (optional) in the format shown below:</p> <p> <code>{ \"FeatureDataTypes\":{\"col1\":\"numeric\", \"col2\":\"categorical\" ... } }</code> </p> <note> <p>These column keys may not include the target column.</p> </note> <p>In ensembling mode, Autopilot only supports the following data types: <code>numeric</code>, <code>categorical</code>, <code>text</code>, and <code>datetime</code>. In HPO mode, Autopilot can support <code>numeric</code>, <code>categorical</code>, <code>text</code>, <code>datetime</code>, and <code>sequence</code>.</p> <p>If only <code>FeatureDataTypes</code> is provided, the column keys (<code>col1</code>, <code>col2</code>,..) should be a subset of the column names in the input data. </p> <p>If both <code>FeatureDataTypes</code> and <code>FeatureAttributeNames</code> are provided, then the column keys should be a subset of the column names provided in <code>FeatureAttributeNames</code>. </p> <p>The key name <code>FeatureAttributeNames</code> is fixed. The values listed in <code>[\"col1\", \"col2\", ...]</code> are case sensitive and should be a list of strings containing unique values that are a subset of the column names in the input data. The list of columns provided must not include the target column.</p>",
                     "shape": "S3Uri"
                 }
             },
@@ -6556,32 +6599,36 @@
         "AutoMLCandidates": {
             "member": {
                 "shape": "AutoMLCandidate"
             },
             "type": "list"
         },
         "AutoMLChannel": {
-            "documentation": "<p>A channel is a named input source that training algorithms can consume. The validation dataset size is limited to less than 2 GB. The training dataset size must be less than 100 GB. For more information, see .</p> <note> <p>A validation dataset must contain the same headers as the training dataset.</p> </note> <p/>",
+            "documentation": "<p>A channel is a named input source that training algorithms can consume. The validation dataset size is limited to less than 2 GB. The training dataset size must be less than 100 GB. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Channel.html\"> Channel</a>.</p> <note> <p>A validation dataset must contain the same headers as the training dataset.</p> </note> <p/>",
             "members": {
                 "ChannelType": {
-                    "documentation": "<p>The channel type (optional) is an <code>enum</code> string. The default value is <code>training</code>. Channels for training and validation must share the same <code>ContentType</code> and <code>TargetAttributeName</code>. For information on specifying training and validation channel types, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-datasets-problem-types.html#autopilot-data-sources-training-or-validation\"> <code>How to specify training and validation datasets</code> </a>.</p>",
+                    "documentation": "<p>The channel type (optional) is an <code>enum</code> string. The default value is <code>training</code>. Channels for training and validation must share the same <code>ContentType</code> and <code>TargetAttributeName</code>. For information on specifying training and validation channel types, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-datasets-problem-types.html#autopilot-data-sources-training-or-validation\">How to specify training and validation datasets</a>.</p>",
                     "shape": "AutoMLChannelType"
                 },
                 "CompressionType": {
                     "documentation": "<p>You can use <code>Gzip</code> or <code>None</code>. The default value is <code>None</code>.</p>",
                     "shape": "CompressionType"
                 },
                 "ContentType": {
                     "documentation": "<p>The content type of the data from the input source. You can use <code>text/csv;header=present</code> or <code>x-application/vnd.amazon+parquet</code>. The default value is <code>text/csv;header=present</code>.</p>",
                     "shape": "ContentType"
                 },
                 "DataSource": {
                     "documentation": "<p>The data source for an AutoML channel.</p>",
                     "shape": "AutoMLDataSource"
                 },
+                "SampleWeightAttributeName": {
+                    "documentation": "<p>If specified, this column name indicates which column of the dataset should be treated as sample weights for use by the objective metric during the training, evaluation, and the selection of the best model. This column is not considered as a predictive feature. For more information on Autopilot metrics, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-metrics-validation.html\">Metrics and validation</a>.</p> <p>Sample weights should be numeric, non-negative, with larger values indicating which rows are more important than others. Data points that have invalid or no weight value are excluded.</p> <p>Support for sample weights is available in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AutoMLAlgorithmConfig.html\">Ensembling</a> mode only.</p>",
+                    "shape": "SampleWeightAttributeName"
+                },
                 "TargetAttributeName": {
                     "documentation": "<p>The name of the target variable in supervised learning, usually represented by 'y'.</p>",
                     "shape": "TargetAttributeName"
                 }
             },
             "required": [
                 "DataSource",
@@ -6593,26 +6640,26 @@
             "enum": [
                 "training",
                 "validation"
             ],
             "type": "string"
         },
         "AutoMLContainerDefinition": {
-            "documentation": "<p>A list of container definitions that describe the different containers that make up an AutoML candidate. For more information, see .</p>",
+            "documentation": "<p>A list of container definitions that describe the different containers that make up an AutoML candidate. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ContainerDefinition.html\"> ContainerDefinition</a>.</p>",
             "members": {
                 "Environment": {
-                    "documentation": "<p>The environment variables to set in the container. For more information, see .</p>",
+                    "documentation": "<p>The environment variables to set in the container. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ContainerDefinition.html\"> ContainerDefinition</a>.</p>",
                     "shape": "EnvironmentMap"
                 },
                 "Image": {
-                    "documentation": "<p>The Amazon Elastic Container Registry (Amazon ECR) path of the container. For more information, see .</p>",
+                    "documentation": "<p>The Amazon Elastic Container Registry (Amazon ECR) path of the container. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ContainerDefinition.html\"> ContainerDefinition</a>.</p>",
                     "shape": "ContainerImage"
                 },
                 "ModelDataUrl": {
-                    "documentation": "<p>The location of the model artifacts. For more information, see .</p>",
+                    "documentation": "<p>The location of the model artifacts. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ContainerDefinition.html\"> ContainerDefinition</a>.</p>",
                     "shape": "Url"
                 }
             },
             "required": [
                 "Image",
                 "ModelDataUrl"
             ],
@@ -6635,15 +6682,15 @@
             },
             "required": [
                 "S3DataSource"
             ],
             "type": "structure"
         },
         "AutoMLDataSplitConfig": {
-            "documentation": "<p>This structure specifies how to split the data into train and validation datasets.</p> <p>If you are using the V1 API (for example <code>CreateAutoMLJob</code>) or the V2 API for Natural Language Processing problems (for example <code>CreateAutoMLJobV2</code> with a <code>TextClassificationJobConfig</code> problem type), the validation and training datasets must contain the same headers. Also, for V1 API jobs, the validation dataset must be less than 2 GB in size.</p>",
+            "documentation": "<p>This structure specifies how to split the data into train and validation datasets.</p> <p>The validation and training datasets must contain the same headers. For jobs created by calling <code>CreateAutoMLJob</code>, the validation dataset must be less than 2 GB in size.</p>",
             "members": {
                 "ValidationFraction": {
                     "documentation": "<p>The validation fraction (optional) is a float that specifies the portion of the training dataset to be used for validation. The default value is 0.2, and values must be greater than 0 and less than 1. We recommend setting this value to be less than 0.5.</p>",
                     "shape": "ValidationFraction"
                 }
             },
             "type": "structure"
@@ -6690,48 +6737,48 @@
                     "documentation": "<p>The URL of the notebook location.</p>",
                     "shape": "DataExplorationNotebookLocation"
                 }
             },
             "type": "structure"
         },
         "AutoMLJobChannel": {
-            "documentation": "<p>A channel is a named input source that training algorithms can consume. This channel is used for the non tabular training data of an AutoML job using the V2 API. For tabular training data, see . For more information, see .</p>",
+            "documentation": "<p>A channel is a named input source that training algorithms can consume. This channel is used for AutoML jobs V2 (jobs created by calling <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJobV2.html\">CreateAutoMLJobV2</a>).</p>",
             "members": {
                 "ChannelType": {
-                    "documentation": "<p>The type of channel. Defines whether the data are used for training or validation. The default value is <code>training</code>. Channels for <code>training</code> and <code>validation</code> must share the same <code>ContentType</code> </p>",
+                    "documentation": "<p>The type of channel. Defines whether the data are used for training or validation. The default value is <code>training</code>. Channels for <code>training</code> and <code>validation</code> must share the same <code>ContentType</code> </p> <note> <p>The type of channel defaults to <code>training</code> for the time-series forecasting problem type.</p> </note>",
                     "shape": "AutoMLChannelType"
                 },
                 "CompressionType": {
-                    "documentation": "<p>The allowed compression types depend on the input format. We allow the compression type <code>Gzip</code> for <code>S3Prefix</code> inputs only. For all other inputs, the compression type should be <code>None</code>. If no compression type is provided, we default to <code>None</code>.</p>",
+                    "documentation": "<p>The allowed compression types depend on the input format and problem type. We allow the compression type <code>Gzip</code> for <code>S3Prefix</code> inputs on tabular data only. For all other inputs, the compression type should be <code>None</code>. If no compression type is provided, we default to <code>None</code>.</p>",
                     "shape": "CompressionType"
                 },
                 "ContentType": {
-                    "documentation": "<p>The content type of the data from the input source. The following are the allowed content types for different problems:</p> <ul> <li> <p>ImageClassification: <code>image/png</code>, <code>image/jpeg</code>, <code>image/*</code> </p> </li> <li> <p>TextClassification: <code>text/csv;header=present</code> </p> </li> </ul>",
+                    "documentation": "<p>The content type of the data from the input source. The following are the allowed content types for different problems:</p> <ul> <li> <p>For tabular problem types: <code>text/csv;header=present</code> or <code>x-application/vnd.amazon+parquet</code>. The default value is <code>text/csv;header=present</code>.</p> </li> <li> <p>For image classification: <code>image/png</code>, <code>image/jpeg</code>, or <code>image/*</code>. The default value is <code>image/*</code>.</p> </li> <li> <p>For text classification: <code>text/csv;header=present</code> or <code>x-application/vnd.amazon+parquet</code>. The default value is <code>text/csv;header=present</code>.</p> </li> <li> <p>For time-series forecasting: <code>text/csv;header=present</code> or <code>x-application/vnd.amazon+parquet</code>. The default value is <code>text/csv;header=present</code>.</p> </li> </ul>",
                     "shape": "ContentType"
                 },
                 "DataSource": {
-                    "documentation": "<p>The data source for an AutoML channel.</p>",
+                    "documentation": "<p>The data source for an AutoML channel (Required).</p>",
                     "shape": "AutoMLDataSource"
                 }
             },
             "type": "structure"
         },
         "AutoMLJobCompletionCriteria": {
             "documentation": "<p>How long a job is allowed to run, or how many candidates a job is allowed to generate.</p>",
             "members": {
                 "MaxAutoMLJobRuntimeInSeconds": {
                     "documentation": "<p>The maximum runtime, in seconds, an AutoML job has to complete.</p> <p>If an AutoML job exceeds the maximum runtime, the job is stopped automatically and its processing is ended gracefully. The AutoML job identifies the best model whose training was completed and marks it as the best-performing model. Any unfinished steps of the job, such as automatic one-click Autopilot model deployment, are not completed.</p>",
                     "shape": "MaxAutoMLJobRuntimeInSeconds"
                 },
                 "MaxCandidates": {
-                    "documentation": "<p>The maximum number of times a training job is allowed to run.</p> <p>For V2 jobs (jobs created by calling <code>CreateAutoMLJobV2</code>), the supported value is 1.</p>",
+                    "documentation": "<p>The maximum number of times a training job is allowed to run.</p> <p>For text and image classification, as well as time-series forecasting problem types, the supported value is 1. For tabular problem types, the maximum value is 750.</p>",
                     "shape": "MaxCandidates"
                 },
                 "MaxRuntimePerTrainingJobInSeconds": {
-                    "documentation": "<p>The maximum time, in seconds, that each training job executed inside hyperparameter tuning is allowed to run as part of a hyperparameter tuning job. For more information, see the used by the action.</p> <p>For V2 jobs (jobs created by calling <code>CreateAutoMLJobV2</code>), this field controls the runtime of the job candidate.</p>",
+                    "documentation": "<p>The maximum time, in seconds, that each training job executed inside hyperparameter tuning is allowed to run as part of a hyperparameter tuning job. For more information, see the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_StoppingCondition.html\">StoppingCondition</a> used by the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateHyperParameterTuningJob.html\">CreateHyperParameterTuningJob</a> action.</p> <p>For job V2s (jobs created by calling <code>CreateAutoMLJobV2</code>), this field controls the runtime of the job candidate.</p>",
                     "shape": "MaxRuntimePerTrainingJobInSeconds"
                 }
             },
             "type": "structure"
         },
         "AutoMLJobConfig": {
             "documentation": "<p>A collection of settings used for an AutoML job.</p>",
@@ -6745,15 +6792,15 @@
                     "shape": "AutoMLJobCompletionCriteria"
                 },
                 "DataSplitConfig": {
                     "documentation": "<p>The configuration for splitting the input training dataset.</p> <p>Type: AutoMLDataSplitConfig</p>",
                     "shape": "AutoMLDataSplitConfig"
                 },
                 "Mode": {
-                    "documentation": "<p>The method that Autopilot uses to train the data. You can either specify the mode manually or let Autopilot choose for you based on the dataset size by selecting <code>AUTO</code>. In <code>AUTO</code> mode, Autopilot chooses <code>ENSEMBLING</code> for datasets smaller than 100 MB, and <code>HYPERPARAMETER_TUNING</code> for larger ones.</p> <p>The <code>ENSEMBLING</code> mode uses a multi-stack ensemble model to predict classification and regression tasks directly from your dataset. This machine learning mode combines several base models to produce an optimal predictive model. It then uses a stacking ensemble method to combine predictions from contributing members. A multi-stack ensemble model can provide better performance over a single model by combining the predictive capabilities of multiple models. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-model-support-validation.html#autopilot-algorithm-suppprt\">Autopilot algorithm support</a> for a list of algorithms supported by <code>ENSEMBLING</code> mode.</p> <p>The <code>HYPERPARAMETER_TUNING</code> (HPO) mode uses the best hyperparameters to train the best version of a model. HPO automatically selects an algorithm for the type of problem you want to solve. Then HPO finds the best hyperparameters according to your objective metric. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-model-support-validation.html#autopilot-algorithm-suppprt\">Autopilot algorithm support</a> for a list of algorithms supported by <code>HYPERPARAMETER_TUNING</code> mode.</p>",
+                    "documentation": "<p>The method that Autopilot uses to train the data. You can either specify the mode manually or let Autopilot choose for you based on the dataset size by selecting <code>AUTO</code>. In <code>AUTO</code> mode, Autopilot chooses <code>ENSEMBLING</code> for datasets smaller than 100 MB, and <code>HYPERPARAMETER_TUNING</code> for larger ones.</p> <p>The <code>ENSEMBLING</code> mode uses a multi-stack ensemble model to predict classification and regression tasks directly from your dataset. This machine learning mode combines several base models to produce an optimal predictive model. It then uses a stacking ensemble method to combine predictions from contributing members. A multi-stack ensemble model can provide better performance over a single model by combining the predictive capabilities of multiple models. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-model-support-validation.html#autopilot-algorithm-support\">Autopilot algorithm support</a> for a list of algorithms supported by <code>ENSEMBLING</code> mode.</p> <p>The <code>HYPERPARAMETER_TUNING</code> (HPO) mode uses the best hyperparameters to train the best version of a model. HPO automatically selects an algorithm for the type of problem you want to solve. Then HPO finds the best hyperparameters according to your objective metric. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-model-support-validation.html#autopilot-algorithm-support\">Autopilot algorithm support</a> for a list of algorithms supported by <code>HYPERPARAMETER_TUNING</code> mode.</p>",
                     "shape": "AutoMLMode"
                 },
                 "SecurityConfig": {
                     "documentation": "<p>The security configuration for traffic encryption or Amazon VPC settings.</p>",
                     "shape": "AutoMLSecurityConfig"
                 }
             },
@@ -6770,18 +6817,18 @@
         "AutoMLJobName": {
             "max": 32,
             "min": 1,
             "pattern": "^[a-zA-Z0-9](-*[a-zA-Z0-9]){0,31}",
             "type": "string"
         },
         "AutoMLJobObjective": {
-            "documentation": "<p>Specifies a metric to minimize or maximize as the objective of a job. V2 API jobs (for example jobs created by calling <code>CreateAutoMLJobV2</code>), support <code>Accuracy</code> only.</p>",
+            "documentation": "<p>Specifies a metric to minimize or maximize as the objective of a job.</p>",
             "members": {
                 "MetricName": {
-                    "documentation": "<p>The name of the objective metric used to measure the predictive quality of a machine learning system. This metric is optimized during training to provide the best estimate for model parameter values from data.</p> <p>Here are the options:</p> <dl> <dt>Accuracy</dt> <dd> <p>The ratio of the number of correctly classified items to the total number of (correctly and incorrectly) classified items. It is used for both binary and multiclass classification. Accuracy measures how close the predicted class values are to the actual values. Values for accuracy metrics vary between zero (0) and one (1). A value of 1 indicates perfect accuracy, and 0 indicates perfect inaccuracy.</p> </dd> <dt>AUC</dt> <dd> <p>The area under the curve (AUC) metric is used to compare and evaluate binary classification by algorithms that return probabilities, such as logistic regression. To map the probabilities into classifications, these are compared against a threshold value. </p> <p>The relevant curve is the receiver operating characteristic curve (ROC curve). The ROC curve plots the true positive rate (TPR) of predictions (or recall) against the false positive rate (FPR) as a function of the threshold value, above which a prediction is considered positive. Increasing the threshold results in fewer false positives, but more false negatives. </p> <p>AUC is the area under this ROC curve. Therefore, AUC provides an aggregated measure of the model performance across all possible classification thresholds. AUC scores vary between 0 and 1. A score of 1 indicates perfect accuracy, and a score of one half (0.5) indicates that the prediction is not better than a random classifier. </p> </dd> <dt>BalancedAccuracy</dt> <dd> <p> <code>BalancedAccuracy</code> is a metric that measures the ratio of accurate predictions to all predictions. This ratio is calculated after normalizing true positives (TP) and true negatives (TN) by the total number of positive (P) and negative (N) values. It is used in both binary and multiclass classification and is defined as follows: 0.5*((TP/P)+(TN/N)), with values ranging from 0 to 1. <code>BalancedAccuracy</code> gives a better measure of accuracy when the number of positives or negatives differ greatly from each other in an imbalanced dataset. For example, when only 1% of email is spam. </p> </dd> <dt>F1</dt> <dd> <p>The <code>F1</code> score is the harmonic mean of the precision and recall, defined as follows: F1 = 2 * (precision * recall) / (precision + recall). It is used for binary classification into classes traditionally referred to as positive and negative. Predictions are said to be true when they match their actual (correct) class, and false when they do not. </p> <p>Precision is the ratio of the true positive predictions to all positive predictions, and it includes the false positives in a dataset. Precision measures the quality of the prediction when it predicts the positive class. </p> <p>Recall (or sensitivity) is the ratio of the true positive predictions to all actual positive instances. Recall measures how completely a model predicts the actual class members in a dataset. </p> <p>F1 scores vary between 0 and 1. A score of 1 indicates the best possible performance, and 0 indicates the worst.</p> </dd> <dt>F1macro</dt> <dd> <p>The <code>F1macro</code> score applies F1 scoring to multiclass classification problems. It does this by calculating the precision and recall, and then taking their harmonic mean to calculate the F1 score for each class. Lastly, the F1macro averages the individual scores to obtain the <code>F1macro</code> score. <code>F1macro</code> scores vary between 0 and 1. A score of 1 indicates the best possible performance, and 0 indicates the worst.</p> </dd> <dt>MAE</dt> <dd> <p>The mean absolute error (MAE) is a measure of how different the predicted and actual values are, when they're averaged over all values. MAE is commonly used in regression analysis to understand model prediction error. If there is linear regression, MAE represents the average distance from a predicted line to the actual value. MAE is defined as the sum of absolute errors divided by the number of observations. Values range from 0 to infinity, with smaller numbers indicating a better model fit to the data.</p> </dd> <dt>MSE</dt> <dd> <p>The mean squared error (MSE) is the average of the squared differences between the predicted and actual values. It is used for regression. MSE values are always positive. The better a model is at predicting the actual values, the smaller the MSE value is</p> </dd> <dt>Precision</dt> <dd> <p>Precision measures how well an algorithm predicts the true positives (TP) out of all of the positives that it identifies. It is defined as follows: Precision = TP/(TP+FP), with values ranging from zero (0) to one (1), and is used in binary classification. Precision is an important metric when the cost of a false positive is high. For example, the cost of a false positive is very high if an airplane safety system is falsely deemed safe to fly. A false positive (FP) reflects a positive prediction that is actually negative in the data.</p> </dd> <dt>PrecisionMacro</dt> <dd> <p>The precision macro computes precision for multiclass classification problems. It does this by calculating precision for each class and averaging scores to obtain precision for several classes. <code>PrecisionMacro</code> scores range from zero (0) to one (1). Higher scores reflect the model's ability to predict true positives (TP) out of all of the positives that it identifies, averaged across multiple classes.</p> </dd> <dt>R2</dt> <dd> <p>R2, also known as the coefficient of determination, is used in regression to quantify how much a model can explain the variance of a dependent variable. Values range from one (1) to negative one (-1). Higher numbers indicate a higher fraction of explained variability. <code>R2</code> values close to zero (0) indicate that very little of the dependent variable can be explained by the model. Negative values indicate a poor fit and that the model is outperformed by a constant function. For linear regression, this is a horizontal line.</p> </dd> <dt>Recall</dt> <dd> <p>Recall measures how well an algorithm correctly predicts all of the true positives (TP) in a dataset. A true positive is a positive prediction that is also an actual positive value in the data. Recall is defined as follows: Recall = TP/(TP+FN), with values ranging from 0 to 1. Higher scores reflect a better ability of the model to predict true positives (TP) in the data, and is used in binary classification. </p> <p>Recall is important when testing for cancer because it's used to find all of the true positives. A false positive (FP) reflects a positive prediction that is actually negative in the data. It is often insufficient to measure only recall, because predicting every output as a true positive yield a perfect recall score.</p> </dd> <dt>RecallMacro</dt> <dd> <p>The RecallMacro computes recall for multiclass classification problems by calculating recall for each class and averaging scores to obtain recall for several classes. RecallMacro scores range from 0 to 1. Higher scores reflect the model's ability to predict true positives (TP) in a dataset. Whereas, a true positive reflects a positive prediction that is also an actual positive value in the data. It is often insufficient to measure only recall, because predicting every output as a true positive yields a perfect recall score.</p> </dd> <dt>RMSE</dt> <dd> <p>Root mean squared error (RMSE) measures the square root of the squared difference between predicted and actual values, and it's averaged over all values. It is used in regression analysis to understand model prediction error. It's an important metric to indicate the presence of large model errors and outliers. Values range from zero (0) to infinity, with smaller numbers indicating a better model fit to the data. RMSE is dependent on scale, and should not be used to compare datasets of different sizes.</p> </dd> </dl> <p>If you do not specify a metric explicitly, the default behavior is to automatically use:</p> <ul> <li> <p> <code>MSE</code>: for regression.</p> </li> <li> <p> <code>F1</code>: for binary classification</p> </li> <li> <p> <code>Accuracy</code>: for multiclass classification.</p> </li> </ul>",
+                    "documentation": "<p>The name of the objective metric used to measure the predictive quality of a machine learning system. During training, the model's parameters are updated iteratively to optimize its performance based on the feedback provided by the objective metric when evaluating the model on the validation dataset.</p> <p>For the list of all available metrics supported by Autopilot, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-metrics-validation.html#autopilot-metrics\">Autopilot metrics</a>.</p> <p>If you do not specify a metric explicitly, the default behavior is to automatically use:</p> <ul> <li> <p>For tabular problem types:</p> <ul> <li> <p>Regression: <code>MSE</code>.</p> </li> <li> <p>Binary classification: <code>F1</code>.</p> </li> <li> <p>Multiclass classification: <code>Accuracy</code>.</p> </li> </ul> </li> <li> <p>For image or text classification problem types: <code>Accuracy</code> </p> </li> <li> <p>For time-series forecasting problem types: <code>AverageWeightedQuantileLoss</code> </p> </li> </ul>",
                     "shape": "AutoMLMetricEnum"
                 }
             },
             "required": [
                 "MetricName"
             ],
             "type": "structure"
@@ -6808,15 +6855,16 @@
                 "GeneratingExplainabilityReport",
                 "Completed",
                 "ExplainabilityError",
                 "DeployingModel",
                 "ModelDeploymentError",
                 "GeneratingModelInsightsReport",
                 "ModelInsightsError",
-                "TrainingModels"
+                "TrainingModels",
+                "PreTraining"
             ],
             "type": "string"
         },
         "AutoMLJobStatus": {
             "enum": [
                 "Completed",
                 "InProgress",
@@ -6907,15 +6955,19 @@
                 "RMSE",
                 "MAE",
                 "R2",
                 "BalancedAccuracy",
                 "Precision",
                 "PrecisionMacro",
                 "Recall",
-                "RecallMacro"
+                "RecallMacro",
+                "MAPE",
+                "MASE",
+                "WAPE",
+                "AverageWeightedQuantileLoss"
             ],
             "type": "string"
         },
         "AutoMLMetricExtendedEnum": {
             "enum": [
                 "Accuracy",
                 "MSE",
@@ -6927,15 +6979,19 @@
                 "R2",
                 "BalancedAccuracy",
                 "Precision",
                 "PrecisionMacro",
                 "Recall",
                 "RecallMacro",
                 "LogLoss",
-                "InferenceLatency"
+                "InferenceLatency",
+                "MAPE",
+                "MASE",
+                "WAPE",
+                "AverageWeightedQuantileLoss"
             ],
             "type": "string"
         },
         "AutoMLMode": {
             "enum": [
                 "AUTO",
                 "ENSEMBLING",
@@ -6980,35 +7036,79 @@
             "member": {
                 "shape": "AutoMLPartialFailureReason"
             },
             "min": 1,
             "type": "list"
         },
         "AutoMLProblemTypeConfig": {
-            "documentation": "<p>A collection of settings specific to the problem type used to configure an AutoML job using the V2 API. There must be one and only one config of the following type.</p>",
+            "documentation": "<p>A collection of settings specific to the problem type used to configure an AutoML job V2. There must be one and only one config of the following type.</p>",
             "members": {
                 "ImageClassificationJobConfig": {
-                    "documentation": "<p>Settings used to configure an AutoML job using the V2 API for the image classification problem type.</p>",
+                    "documentation": "<p>Settings used to configure an AutoML job V2 for the image classification problem type.</p>",
                     "shape": "ImageClassificationJobConfig"
                 },
+                "TabularJobConfig": {
+                    "documentation": "<p>Settings used to configure an AutoML job V2 for a tabular problem type (regression, classification).</p>",
+                    "shape": "TabularJobConfig"
+                },
                 "TextClassificationJobConfig": {
-                    "documentation": "<p>Settings used to configure an AutoML job using the V2 API for the text classification problem type.</p>",
+                    "documentation": "<p>Settings used to configure an AutoML job V2 for the text classification problem type.</p>",
                     "shape": "TextClassificationJobConfig"
+                },
+                "TimeSeriesForecastingJobConfig": {
+                    "documentation": "<p>Settings used to configure an AutoML job V2 for a time-series forecasting problem type.</p> <note> <p>The <code>TimeSeriesForecastingJobConfig</code> problem type is only available in private beta. Contact Amazon Web Services Support or your account manager to learn more about access privileges.</p> </note>",
+                    "shape": "TimeSeriesForecastingJobConfig"
+                }
+            },
+            "type": "structure",
+            "union": true
+        },
+        "AutoMLProblemTypeConfigName": {
+            "enum": [
+                "ImageClassification",
+                "TextClassification",
+                "Tabular",
+                "TimeSeriesForecasting"
+            ],
+            "type": "string"
+        },
+        "AutoMLProblemTypeResolvedAttributes": {
+            "documentation": "<p>The resolved attributes specific to the problem type of an AutoML job V2.</p>",
+            "members": {
+                "TabularResolvedAttributes": {
+                    "documentation": "<p>Defines the resolved attributes for the <code>TABULAR</code> problem type.</p>",
+                    "shape": "TabularResolvedAttributes"
                 }
             },
             "type": "structure",
             "union": true
         },
         "AutoMLProcessingUnit": {
             "enum": [
                 "CPU",
                 "GPU"
             ],
             "type": "string"
         },
+        "AutoMLResolvedAttributes": {
+            "documentation": "<p>The resolved attributes used to configure an AutoML job V2.</p>",
+            "members": {
+                "AutoMLJobObjective": {
+                    "shape": "AutoMLJobObjective"
+                },
+                "AutoMLProblemTypeResolvedAttributes": {
+                    "documentation": "<p>Defines the resolved attributes specific to a problem type.</p>",
+                    "shape": "AutoMLProblemTypeResolvedAttributes"
+                },
+                "CompletionCriteria": {
+                    "shape": "AutoMLJobCompletionCriteria"
+                }
+            },
+            "type": "structure"
+        },
         "AutoMLS3DataSource": {
             "documentation": "<p>Describes the Amazon S3 data source.</p>",
             "members": {
                 "S3DataType": {
                     "documentation": "<p>The data type. </p> <ul> <li> <p>If you choose <code>S3Prefix</code>, <code>S3Uri</code> identifies a key name prefix. SageMaker uses all objects that match the specified key name prefix for model training.</p> <p>The <code>S3Prefix</code> should have the following format:</p> <p> <code>s3://DOC-EXAMPLE-BUCKET/DOC-EXAMPLE-FOLDER-OR-FILE</code> </p> </li> <li> <p>If you choose <code>ManifestFile</code>, <code>S3Uri</code> identifies an object that is a manifest file containing a list of object keys that you want SageMaker to use for model training.</p> <p>A <code>ManifestFile</code> should have the format shown below:</p> <p> <code>[ {\"prefix\": \"s3://DOC-EXAMPLE-BUCKET/DOC-EXAMPLE-FOLDER/DOC-EXAMPLE-PREFIX/\"}, </code> </p> <p> <code>\"DOC-EXAMPLE-RELATIVE-PATH/DOC-EXAMPLE-FOLDER/DATA-1\",</code> </p> <p> <code>\"DOC-EXAMPLE-RELATIVE-PATH/DOC-EXAMPLE-FOLDER/DATA-2\",</code> </p> <p> <code>... \"DOC-EXAMPLE-RELATIVE-PATH/DOC-EXAMPLE-FOLDER/DATA-N\" ]</code> </p> </li> <li> <p>If you choose <code>AugmentedManifestFile</code>, <code>S3Uri</code> identifies an object that is an augmented manifest file in JSON lines format. This file contains the data you want to use for model training. <code>AugmentedManifestFile</code> is available for V2 API jobs only (for example, for jobs created by calling <code>CreateAutoMLJobV2</code>).</p> <p>Here is a minimal, single-record example of an <code>AugmentedManifestFile</code>:</p> <p> <code>{\"source-ref\": \"s3://DOC-EXAMPLE-BUCKET/DOC-EXAMPLE-FOLDER/cats/cat.jpg\",</code> </p> <p> <code>\"label-metadata\": {\"class-name\": \"cat\"</code> }</p> <p>For more information on <code>AugmentedManifestFile</code>, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/augmented-manifest.html\">Provide Dataset Metadata to Training Jobs with an Augmented Manifest File</a>.</p> </li> </ul>",
                     "shape": "AutoMLS3DataType"
                 },
@@ -7060,31 +7160,80 @@
         "AutoMLSortOrder": {
             "enum": [
                 "Ascending",
                 "Descending"
             ],
             "type": "string"
         },
+        "AutoParameter": {
+            "documentation": "<p>The name and an example value of the hyperparameter that you want to use in Autotune. If Automatic model tuning (AMT) determines that your hyperparameter is eligible for Autotune, an optimal hyperparameter range is selected for you.</p>",
+            "members": {
+                "Name": {
+                    "documentation": "<p>The name of the hyperparameter to optimize using Autotune.</p>",
+                    "shape": "ParameterKey"
+                },
+                "ValueHint": {
+                    "documentation": "<p>An example value of the hyperparameter to optimize using Autotune.</p>",
+                    "shape": "ParameterValue"
+                }
+            },
+            "required": [
+                "Name",
+                "ValueHint"
+            ],
+            "type": "structure"
+        },
+        "AutoParameters": {
+            "max": 100,
+            "member": {
+                "shape": "AutoParameter"
+            },
+            "min": 0,
+            "type": "list"
+        },
         "AutoRollbackConfig": {
             "documentation": "<p>Automatic rollback configuration for handling endpoint deployment failures and recovery.</p>",
             "members": {
                 "Alarms": {
                     "documentation": "<p>List of CloudWatch alarms in your account that are configured to monitor metrics on an endpoint. If any alarms are tripped during a deployment, SageMaker rolls back the deployment.</p>",
                     "shape": "AlarmList"
                 }
             },
             "type": "structure"
         },
+        "Autotune": {
+            "documentation": "<p>A flag to indicate if you want to use Autotune to automatically find optimal values for the following fields:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobConfig.html#sagemaker-Type-HyperParameterTuningJobConfig-ParameterRanges\">ParameterRanges</a>: The names and ranges of parameters that a hyperparameter tuning job can optimize.</p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ResourceLimits.html\">ResourceLimits</a>: The maximum resources that can be used for a training job. These resources include the maximum number of training jobs, the maximum runtime of a tuning job, and the maximum number of training jobs to run at the same time.</p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobConfig.html#sagemaker-Type-HyperParameterTuningJobConfig-TrainingJobEarlyStoppingType\">TrainingJobEarlyStoppingType</a>: A flag that specifies whether or not to use early stopping for training jobs launched by a hyperparameter tuning job.</p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTrainingJobDefinition.html#sagemaker-Type-HyperParameterTrainingJobDefinition-RetryStrategy\">RetryStrategy</a>: The number of times to retry a training job.</p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobConfig.html\">Strategy</a>: Specifies how hyperparameter tuning chooses the combinations of hyperparameter values to use for the training jobs that it launches.</p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ConvergenceDetected.html\">ConvergenceDetected</a>: A flag to indicate that Automatic model tuning (AMT) has detected model convergence.</p> </li> </ul>",
+            "members": {
+                "Mode": {
+                    "documentation": "<p>Set <code>Mode</code> to <code>Enabled</code> if you want to use Autotune.</p>",
+                    "shape": "AutotuneMode"
+                }
+            },
+            "required": [
+                "Mode"
+            ],
+            "type": "structure"
+        },
+        "AutotuneMode": {
+            "enum": [
+                "Enabled"
+            ],
+            "type": "string"
+        },
         "AwsManagedHumanLoopRequestSource": {
             "enum": [
                 "AWS/Rekognition/DetectModerationLabels/Image/V3",
                 "AWS/Textract/AnalyzeDocument/Forms/V1"
             ],
             "type": "string"
         },
+        "BacktestResultsLocation": {
+            "min": 1,
+            "type": "string"
+        },
         "BatchDataCaptureConfig": {
             "documentation": "<p>Configuration to control how SageMaker captures inference data for batch transform jobs.</p>",
             "members": {
                 "DestinationS3Uri": {
                     "documentation": "<p>The Amazon S3 location being used to capture the data.</p>",
                     "shape": "S3Uri"
                 },
@@ -7372,14 +7521,18 @@
             "min": 10,
             "pattern": "^[a-zA-Z0-9]+$",
             "type": "string"
         },
         "CandidateArtifactLocations": {
             "documentation": "<p>The location of artifacts for an AutoML candidate job.</p>",
             "members": {
+                "BacktestResults": {
+                    "documentation": "<p>The Amazon S3 prefix to the accuracy metrics and the inference results observed over the testing window. Available only for the time-series forecasting problem type.</p>",
+                    "shape": "BacktestResultsLocation"
+                },
                 "Explainability": {
                     "documentation": "<p>The Amazon S3 prefix to the explainability artifacts generated for the AutoML candidate.</p>",
                     "shape": "ExplainabilityLocation"
                 },
                 "ModelInsights": {
                     "documentation": "<p>The Amazon S3 prefix to the model insight artifacts generated for the AutoML candidate.</p>",
                     "shape": "ModelInsightsLocation"
@@ -7390,14 +7543,24 @@
             ],
             "type": "structure"
         },
         "CandidateDefinitionNotebookLocation": {
             "min": 1,
             "type": "string"
         },
+        "CandidateGenerationConfig": {
+            "documentation": "<p>Stores the configuration information for how model candidates are generated using an AutoML job V2.</p>",
+            "members": {
+                "AlgorithmsConfig": {
+                    "documentation": "<p>Stores the configuration information for the selection of algorithms used to train model candidates on tabular data.</p> <p>The list of available algorithms to choose from depends on the training mode set in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_TabularJobConfig.html\"> <code>TabularJobConfig.Mode</code> </a>.</p> <ul> <li> <p> <code>AlgorithmsConfig</code> should not be set in <code>AUTO</code> training mode.</p> </li> <li> <p>When <code>AlgorithmsConfig</code> is provided, one <code>AutoMLAlgorithms</code> attribute must be set and one only.</p> <p>If the list of algorithms provided as values for <code>AutoMLAlgorithms</code> is empty, <code>CandidateGenerationConfig</code> uses the full set of algorithms for the given training mode.</p> </li> <li> <p>When <code>AlgorithmsConfig</code> is not provided, <code>CandidateGenerationConfig</code> uses the full set of algorithms for the given training mode.</p> </li> </ul> <p>For the list of all algorithms per problem type and training mode, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AutoMLAlgorithmConfig.html\"> AutoMLAlgorithmConfig</a>.</p> <p>For more information on each algorithm, see the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-model-support-validation.html#autopilot-algorithm-support\">Algorithm support</a> section in Autopilot developer guide.</p>",
+                    "shape": "AutoMLAlgorithmsConfig"
+                }
+            },
+            "type": "structure"
+        },
         "CandidateName": {
             "max": 64,
             "min": 1,
             "type": "string"
         },
         "CandidateProperties": {
             "documentation": "<p>The properties of an AutoML candidate job.</p>",
@@ -7453,25 +7616,29 @@
         "CandidateSteps": {
             "member": {
                 "shape": "AutoMLCandidateStep"
             },
             "type": "list"
         },
         "CanvasAppSettings": {
-            "documentation": "<p>The SageMaker Canvas app settings.</p>",
+            "documentation": "<p>The SageMaker Canvas application settings.</p>",
             "members": {
+                "ModelRegisterSettings": {
+                    "documentation": "<p>The model registry settings for the SageMaker Canvas application.</p>",
+                    "shape": "ModelRegisterSettings"
+                },
                 "TimeSeriesForecastingSettings": {
-                    "documentation": "<p>Time series forecast settings for the Canvas app.</p>",
+                    "documentation": "<p>Time series forecast settings for the Canvas application.</p>",
                     "shape": "TimeSeriesForecastingSettings"
                 }
             },
             "type": "structure"
         },
         "CapacitySize": {
-            "documentation": "<p>Specifies the endpoint capacity to activate for production.</p>",
+            "documentation": "<p>Specifies the type and size of the endpoint capacity to activate for a blue/green deployment, a rolling deployment, or a rollback strategy. You can specify your batches as either instance count or the overall percentage or your fleet.</p> <p>For a rollback strategy, if you don't specify the fields in this object, or if you set the <code>Value</code> to 100%, then SageMaker uses a blue/green rollback strategy and rolls all traffic back to the blue fleet.</p>",
             "members": {
                 "Type": {
                     "documentation": "<p>Specifies the endpoint capacity type.</p> <ul> <li> <p> <code>INSTANCE_COUNT</code>: The endpoint activates based on the number of instances.</p> </li> <li> <p> <code>CAPACITY_PERCENT</code>: The endpoint activates based on the specified percentage of capacity.</p> </li> </ul>",
                     "shape": "CapacitySizeType"
                 },
                 "Value": {
                     "documentation": "<p>Defines the capacity size, either as a number of instances or a capacity percentage.</p>",
@@ -7647,15 +7814,15 @@
                     "shape": "ContentType"
                 },
                 "DataSource": {
                     "documentation": "<p>The location of the channel data.</p>",
                     "shape": "DataSource"
                 },
                 "InputMode": {
-                    "documentation": "<p>(Optional) The input mode to use for the data channel in a training job. If you don't set a value for <code>InputMode</code>, SageMaker uses the value set for <code>TrainingInputMode</code>. Use this parameter to override the <code>TrainingInputMode</code> setting in a <a>AlgorithmSpecification</a> request when you have a channel that needs a different input mode from the training job's general setting. To download the data from Amazon Simple Storage Service (Amazon S3) to the provisioned ML storage volume, and mount the directory to a Docker volume, use <code>File</code> input mode. To stream data directly from Amazon S3 to the container, choose <code>Pipe</code> input mode.</p> <p>To use a model for incremental training, choose <code>File</code> input model.</p>",
+                    "documentation": "<p>(Optional) The input mode to use for the data channel in a training job. If you don't set a value for <code>InputMode</code>, SageMaker uses the value set for <code>TrainingInputMode</code>. Use this parameter to override the <code>TrainingInputMode</code> setting in a <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AlgorithmSpecification.html\">AlgorithmSpecification</a> request when you have a channel that needs a different input mode from the training job's general setting. To download the data from Amazon Simple Storage Service (Amazon S3) to the provisioned ML storage volume, and mount the directory to a Docker volume, use <code>File</code> input mode. To stream data directly from Amazon S3 to the container, choose <code>Pipe</code> input mode.</p> <p>To use a model for incremental training, choose <code>File</code> input model.</p>",
                     "shape": "TrainingInputMode"
                 },
                 "RecordWrapperType": {
                     "documentation": "<p/> <p>Specify RecordIO as the value when input data is in raw format but the training algorithm requires the RecordIO format. In this case, SageMaker wraps each individual S3 object in a RecordIO record. If the input data is already in RecordIO format, you don't need to set this attribute. For more information, see <a href=\"https://mxnet.apache.org/api/architecture/note_data_loading#data-format\">Create a Dataset Using RecordIO</a>. </p> <p>In File mode, leave this field unset or set it to None.</p>",
                     "shape": "RecordWrapper"
                 },
                 "ShuffleConfig": {
@@ -8469,29 +8636,33 @@
                     "shape": "ContainerHostname"
                 },
                 "Environment": {
                     "documentation": "<p>The environment variables to set in the Docker container. Each key and value in the <code>Environment</code> string to string map can have length of up to 1024. We support up to 16 entries in the map. </p>",
                     "shape": "EnvironmentMap"
                 },
                 "Image": {
-                    "documentation": "<p>The path where inference code is stored. This can be either in Amazon EC2 Container Registry or in a Docker registry that is accessible from the same VPC that you configure for your endpoint. If you are using your own custom algorithm instead of an algorithm provided by SageMaker, the inference code must meet SageMaker requirements. SageMaker supports both <code>registry/repository[:tag]</code> and <code>registry/repository[@digest]</code> image path formats. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a> </p>",
+                    "documentation": "<p>The path where inference code is stored. This can be either in Amazon EC2 Container Registry or in a Docker registry that is accessible from the same VPC that you configure for your endpoint. If you are using your own custom algorithm instead of an algorithm provided by SageMaker, the inference code must meet SageMaker requirements. SageMaker supports both <code>registry/repository[:tag]</code> and <code>registry/repository[@digest]</code> image path formats. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>. </p> <note> <p>The model artifacts in an Amazon S3 bucket and the Docker image for inference container in Amazon EC2 Container Registry must be in the same region as the model or endpoint you are creating.</p> </note>",
                     "shape": "ContainerImage"
                 },
                 "ImageConfig": {
-                    "documentation": "<p>Specifies whether the model container is in Amazon ECR or a private Docker registry accessible from your Amazon Virtual Private Cloud (VPC). For information about storing containers in a private Docker registry, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms-containers-inference-private.html\">Use a Private Docker Registry for Real-Time Inference Containers</a> </p>",
+                    "documentation": "<p>Specifies whether the model container is in Amazon ECR or a private Docker registry accessible from your Amazon Virtual Private Cloud (VPC). For information about storing containers in a private Docker registry, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms-containers-inference-private.html\">Use a Private Docker Registry for Real-Time Inference Containers</a>. </p> <note> <p>The model artifacts in an Amazon S3 bucket and the Docker image for inference container in Amazon EC2 Container Registry must be in the same region as the model or endpoint you are creating.</p> </note>",
                     "shape": "ImageConfig"
                 },
                 "InferenceSpecificationName": {
                     "documentation": "<p>The inference specification name in the model package version.</p>",
                     "shape": "InferenceSpecificationName"
                 },
                 "Mode": {
                     "documentation": "<p>Whether the container hosts a single model or multiple models.</p>",
                     "shape": "ContainerMode"
                 },
+                "ModelDataSource": {
+                    "documentation": "<p>Specifies the location of ML model data to deploy.</p> <note> <p>Currently you cannot use <code>ModelDataSource</code> in conjunction with SageMaker batch transform, SageMaker serverless endpoints, SageMaker multi-model endpoints, and SageMaker Marketplace.</p> </note>",
+                    "shape": "ModelDataSource"
+                },
                 "ModelDataUrl": {
                     "documentation": "<p>The S3 path where the model artifacts, which result from model training, are stored. This path must point to a single gzip compressed tar archive (.tar.gz suffix). The S3 path is required for SageMaker built-in algorithms, but not if you use your own algorithms. For more information on built-in algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-algo-docker-registry-paths.html\">Common Parameters</a>. </p> <note> <p>The model artifacts must be in an S3 bucket that is in the same region as the model or endpoint you are creating.</p> </note> <p>If you provide a value for this parameter, SageMaker uses Amazon Web Services Security Token Service to download model artifacts from the S3 path you provide. Amazon Web Services STS is activated in your Amazon Web Services account by default. If you previously deactivated Amazon Web Services STS for a region, you need to reactivate Amazon Web Services STS for that region. For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_enable-regions.html\">Activating and Deactivating Amazon Web Services STS in an Amazon Web Services Region</a> in the <i>Amazon Web Services Identity and Access Management User Guide</i>.</p> <important> <p>If you use a built-in algorithm to create a model, SageMaker requires that you provide a S3 path to the model artifacts in <code>ModelDataUrl</code>.</p> </important>",
                     "shape": "Url"
                 },
                 "ModelPackageName": {
                     "documentation": "<p>The name or Amazon Resource Name (ARN) of the model package to use to create the model.</p>",
                     "shape": "VersionedArnOrName"
@@ -8923,35 +9094,35 @@
                     "shape": "AutoMLJobConfig"
                 },
                 "AutoMLJobName": {
                     "documentation": "<p>Identifies an Autopilot job. The name must be unique to your account and is case insensitive.</p>",
                     "shape": "AutoMLJobName"
                 },
                 "AutoMLJobObjective": {
-                    "documentation": "<p>Defines the objective metric used to measure the predictive quality of an AutoML job. You provide an <a>AutoMLJobObjective$MetricName</a> and Autopilot infers whether to minimize or maximize it. For , only <code>Accuracy</code> is supported.</p>",
+                    "documentation": "<p>Specifies a metric to minimize or maximize as the objective of a job. If not specified, the default objective metric depends on the problem type. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AutoMLJobObjective.html\">AutoMLJobObjective</a> for the default values.</p>",
                     "shape": "AutoMLJobObjective"
                 },
                 "GenerateCandidateDefinitionsOnly": {
                     "documentation": "<p>Generates possible candidates without training the models. A candidate is a combination of data preprocessors, algorithms, and algorithm parameter settings.</p>",
                     "shape": "GenerateCandidateDefinitionsOnly"
                 },
                 "InputDataConfig": {
-                    "documentation": "<p>An array of channel objects that describes the input data and its location. Each channel is a named input source. Similar to <code>InputDataConfig</code> supported by . Format(s) supported: CSV, Parquet. A minimum of 500 rows is required for the training dataset. There is not a minimum number of rows required for the validation dataset.</p>",
+                    "documentation": "<p>An array of channel objects that describes the input data and its location. Each channel is a named input source. Similar to <code>InputDataConfig</code> supported by <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTrainingJobDefinition.html\">HyperParameterTrainingJobDefinition</a>. Format(s) supported: CSV, Parquet. A minimum of 500 rows is required for the training dataset. There is not a minimum number of rows required for the validation dataset.</p>",
                     "shape": "AutoMLInputDataConfig"
                 },
                 "ModelDeployConfig": {
                     "documentation": "<p>Specifies how to generate the endpoint name for an automatic one-click Autopilot model deployment.</p>",
                     "shape": "ModelDeployConfig"
                 },
                 "OutputDataConfig": {
                     "documentation": "<p>Provides information about encryption and the Amazon S3 output path needed to store artifacts from an AutoML job. Format(s) supported: CSV.</p>",
                     "shape": "AutoMLOutputDataConfig"
                 },
                 "ProblemType": {
-                    "documentation": "<p>Defines the type of supervised learning problem available for the candidates. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-automate-model-development-problem-types.html\"> Amazon SageMaker Autopilot problem types and algorithm support</a>.</p>",
+                    "documentation": "<p>Defines the type of supervised learning problem available for the candidates. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-datasets-problem-types.html#autopilot-problem-types\"> Amazon SageMaker Autopilot problem types</a>.</p>",
                     "shape": "ProblemType"
                 },
                 "RoleArn": {
                     "documentation": "<p>The ARN of the role that is used to access the data.</p>",
                     "shape": "RoleArn"
                 },
                 "Tags": {
@@ -8978,31 +9149,31 @@
                 "AutoMLJobArn"
             ],
             "type": "structure"
         },
         "CreateAutoMLJobV2Request": {
             "members": {
                 "AutoMLJobInputDataConfig": {
-                    "documentation": "<p>An array of channel objects describing the input data and their location. Each channel is a named input source. Similar to <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJob.html#sagemaker-CreateAutoMLJob-request-InputDataConfig\">InputDataConfig</a> supported by <code>CreateAutoMLJob</code>. The supported formats depend on the problem type:</p> <ul> <li> <p>ImageClassification: S3Prefix, <code>ManifestFile</code>, <code>AugmentedManifestFile</code> </p> </li> <li> <p>TextClassification: S3Prefix</p> </li> </ul>",
+                    "documentation": "<p>An array of channel objects describing the input data and their location. Each channel is a named input source. Similar to the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJob.html#sagemaker-CreateAutoMLJob-request-InputDataConfig\">InputDataConfig</a> attribute in the <code>CreateAutoMLJob</code> input parameters. The supported formats depend on the problem type:</p> <ul> <li> <p>For tabular problem types: <code>S3Prefix</code>, <code>ManifestFile</code>.</p> </li> <li> <p>For image classification: <code>S3Prefix</code>, <code>ManifestFile</code>, <code>AugmentedManifestFile</code>.</p> </li> <li> <p>For text classification: <code>S3Prefix</code>.</p> </li> <li> <p>For time-series forecasting: <code>S3Prefix</code>.</p> </li> </ul>",
                     "shape": "AutoMLJobInputDataConfig"
                 },
                 "AutoMLJobName": {
                     "documentation": "<p>Identifies an Autopilot job. The name must be unique to your account and is case insensitive.</p>",
                     "shape": "AutoMLJobName"
                 },
                 "AutoMLJobObjective": {
-                    "documentation": "<p>Specifies a metric to minimize or maximize as the objective of a job. For , only <code>Accuracy</code> is supported.</p>",
+                    "documentation": "<p>Specifies a metric to minimize or maximize as the objective of a job. If not specified, the default objective metric depends on the problem type. For the list of default values per problem type, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AutoMLJobObjective.html\">AutoMLJobObjective</a>.</p> <note> <p>For tabular problem types, you must either provide both the <code>AutoMLJobObjective</code> and indicate the type of supervised learning problem in <code>AutoMLProblemTypeConfig</code> (<code>TabularJobConfig.ProblemType</code>), or none at all.</p> </note>",
                     "shape": "AutoMLJobObjective"
                 },
                 "AutoMLProblemTypeConfig": {
                     "documentation": "<p>Defines the configuration settings of one of the supported problem types.</p>",
                     "shape": "AutoMLProblemTypeConfig"
                 },
                 "DataSplitConfig": {
-                    "documentation": "<p>This structure specifies how to split the data into train and validation datasets.</p> <p>If you are using the V1 API (for example <code>CreateAutoMLJob</code>) or the V2 API for Natural Language Processing problems (for example <code>CreateAutoMLJobV2</code> with a <code>TextClassificationJobConfig</code> problem type), the validation and training datasets must contain the same headers. Also, for V1 API jobs, the validation dataset must be less than 2 GB in size.</p>",
+                    "documentation": "<p>This structure specifies how to split the data into train and validation datasets.</p> <p>The validation and training datasets must contain the same headers. For jobs created by calling <code>CreateAutoMLJob</code>, the validation dataset must be less than 2 GB in size.</p> <note> <p>This attribute must not be set for the time-series forecasting problem type, as Autopilot automatically splits the input dataset into training and validation sets.</p> </note>",
                     "shape": "AutoMLDataSplitConfig"
                 },
                 "ModelDeployConfig": {
                     "documentation": "<p>Specifies how to generate the endpoint name for an automatic one-click Autopilot model deployment.</p>",
                     "shape": "ModelDeployConfig"
                 },
                 "OutputDataConfig": {
@@ -9103,15 +9274,15 @@
                     "shape": "StoppingCondition"
                 },
                 "Tags": {
                     "documentation": "<p>An array of key-value pairs. You can use tags to categorize your Amazon Web Services resources in different ways, for example, by purpose, owner, or environment. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a>.</p>",
                     "shape": "TagList"
                 },
                 "VpcConfig": {
-                    "documentation": "<p>A <a>VpcConfig</a> object that specifies the VPC that you want your compilation job to connect to. Control access to your models by configuring the VPC. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/neo-vpc.html\">Protect Compilation Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
+                    "documentation": "<p>A <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_VpcConfig.html\">VpcConfig</a> object that specifies the VPC that you want your compilation job to connect to. Control access to your models by configuring the VPC. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/neo-vpc.html\">Protect Compilation Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
                     "shape": "NeoVpcConfig"
                 }
             },
             "required": [
                 "CompilationJobName",
                 "RoleArn",
                 "OutputConfig",
@@ -9272,15 +9443,15 @@
         "CreateDomainRequest": {
             "members": {
                 "AppNetworkAccessType": {
                     "documentation": "<p>Specifies the VPC used for non-EFS traffic. The default value is <code>PublicInternetOnly</code>.</p> <ul> <li> <p> <code>PublicInternetOnly</code> - Non-EFS traffic is through a VPC managed by Amazon SageMaker, which allows direct internet access</p> </li> <li> <p> <code>VpcOnly</code> - All Studio traffic is through the specified VPC and subnets</p> </li> </ul>",
                     "shape": "AppNetworkAccessType"
                 },
                 "AppSecurityGroupManagement": {
-                    "documentation": "<p>The entity that creates and manages the required security groups for inter-app communication in <code>VPCOnly</code> mode. Required when <code>CreateDomain.AppNetworkAccessType</code> is <code>VPCOnly</code> and <code>DomainSettings.RStudioServerProDomainSettings.DomainExecutionRoleArn</code> is provided.</p>",
+                    "documentation": "<p>The entity that creates and manages the required security groups for inter-app communication in <code>VPCOnly</code> mode. Required when <code>CreateDomain.AppNetworkAccessType</code> is <code>VPCOnly</code> and <code>DomainSettings.RStudioServerProDomainSettings.DomainExecutionRoleArn</code> is provided. If setting up the domain for use with RStudio, this value must be set to <code>Service</code>.</p>",
                     "shape": "AppSecurityGroupManagement"
                 },
                 "AuthMode": {
                     "documentation": "<p>The mode of authentication that members use to access the domain.</p>",
                     "shape": "AuthMode"
                 },
                 "DefaultSpaceSettings": {
@@ -9454,15 +9625,15 @@
                     "documentation": "<p>Specifies configuration for how an endpoint performs asynchronous inference. This is a required field in order for your Endpoint to be invoked using <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_runtime_InvokeEndpointAsync.html\">InvokeEndpointAsync</a>.</p>",
                     "shape": "AsyncInferenceConfig"
                 },
                 "DataCaptureConfig": {
                     "shape": "DataCaptureConfig"
                 },
                 "EndpointConfigName": {
-                    "documentation": "<p>The name of the endpoint configuration. You specify this name in a <a>CreateEndpoint</a> request. </p>",
+                    "documentation": "<p>The name of the endpoint configuration. You specify this name in a <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpoint.html\">CreateEndpoint</a> request. </p>",
                     "shape": "EndpointConfigName"
                 },
                 "ExplainerConfig": {
                     "documentation": "<p>A member of <code>CreateEndpointConfig</code> that enables explainers.</p>",
                     "shape": "ExplainerConfig"
                 },
                 "KmsKeyId": {
@@ -9502,19 +9673,19 @@
         },
         "CreateEndpointInput": {
             "members": {
                 "DeploymentConfig": {
                     "shape": "DeploymentConfig"
                 },
                 "EndpointConfigName": {
-                    "documentation": "<p>The name of an endpoint configuration. For more information, see <a>CreateEndpointConfig</a>. </p>",
+                    "documentation": "<p>The name of an endpoint configuration. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpointConfig.html\">CreateEndpointConfig</a>. </p>",
                     "shape": "EndpointConfigName"
                 },
                 "EndpointName": {
-                    "documentation": "<p>The name of the endpoint.The name must be unique within an Amazon Web Services Region in your Amazon Web Services account. The name is case-insensitive in <code>CreateEndpoint</code>, but the case is preserved and must be matched in .</p>",
+                    "documentation": "<p>The name of the endpoint.The name must be unique within an Amazon Web Services Region in your Amazon Web Services account. The name is case-insensitive in <code>CreateEndpoint</code>, but the case is preserved and must be matched in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_runtime_InvokeEndpoint.html\">InvokeEndpoint</a>.</p>",
                     "shape": "EndpointName"
                 },
                 "Tags": {
                     "documentation": "<p>An array of key-value pairs. You can use tags to categorize your Amazon Web Services resources in different ways, for example, by purpose, owner, or environment. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a>.</p>",
                     "shape": "TagList"
                 }
             },
@@ -9547,15 +9718,15 @@
                     "shape": "ExperimentEntityName"
                 },
                 "ExperimentName": {
                     "documentation": "<p>The name of the experiment. The name must be unique in your Amazon Web Services account and is not case-sensitive.</p>",
                     "shape": "ExperimentEntityName"
                 },
                 "Tags": {
-                    "documentation": "<p>A list of tags to associate with the experiment. You can use <a>Search</a> API to search on the tags.</p>",
+                    "documentation": "<p>A list of tags to associate with the experiment. You can use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API to search on the tags.</p>",
                     "shape": "TagList"
                 }
             },
             "required": [
                 "ExperimentName"
             ],
             "type": "structure"
@@ -9584,19 +9755,19 @@
                     "shape": "FeatureDefinitions"
                 },
                 "FeatureGroupName": {
                     "documentation": "<p>The name of the <code>FeatureGroup</code>. The name must be unique within an Amazon Web Services Region in an Amazon Web Services account. The name:</p> <ul> <li> <p>Must start and end with an alphanumeric character.</p> </li> <li> <p>Can only contain alphanumeric character and hyphens. Spaces are not allowed. </p> </li> </ul>",
                     "shape": "FeatureGroupName"
                 },
                 "OfflineStoreConfig": {
-                    "documentation": "<p>Use this to configure an <code>OfflineFeatureStore</code>. This parameter allows you to specify:</p> <ul> <li> <p>The Amazon Simple Storage Service (Amazon S3) location of an <code>OfflineStore</code>.</p> </li> <li> <p>A configuration for an Amazon Web Services Glue or Amazon Web Services Hive data catalog. </p> </li> <li> <p>An KMS encryption key to encrypt the Amazon S3 location used for <code>OfflineStore</code>. If KMS encryption key is not specified, by default we encrypt all data at rest using Amazon Web Services KMS key. By defining your <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucket-key.html\">bucket-level key</a> for SSE, you can reduce Amazon Web Services KMS requests costs by up to 99 percent.</p> </li> <li> <p>Format for the offline store table. Supported formats are Glue (Default) and <a href=\"https://iceberg.apache.org/\">Apache Iceberg</a>.</p> </li> </ul> <p>To learn more about this parameter, see <a>OfflineStoreConfig</a>.</p>",
+                    "documentation": "<p>Use this to configure an <code>OfflineFeatureStore</code>. This parameter allows you to specify:</p> <ul> <li> <p>The Amazon Simple Storage Service (Amazon S3) location of an <code>OfflineStore</code>.</p> </li> <li> <p>A configuration for an Amazon Web Services Glue or Amazon Web Services Hive data catalog. </p> </li> <li> <p>An KMS encryption key to encrypt the Amazon S3 location used for <code>OfflineStore</code>. If KMS encryption key is not specified, by default we encrypt all data at rest using Amazon Web Services KMS key. By defining your <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucket-key.html\">bucket-level key</a> for SSE, you can reduce Amazon Web Services KMS requests costs by up to 99 percent.</p> </li> <li> <p>Format for the offline store table. Supported formats are Glue (Default) and <a href=\"https://iceberg.apache.org/\">Apache Iceberg</a>.</p> </li> </ul> <p>To learn more about this parameter, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_OfflineStoreConfig.html\">OfflineStoreConfig</a>.</p>",
                     "shape": "OfflineStoreConfig"
                 },
                 "OnlineStoreConfig": {
-                    "documentation": "<p>You can turn the <code>OnlineStore</code> on or off by specifying <code>True</code> for the <code>EnableOnlineStore</code> flag in <code>OnlineStoreConfig</code>; the default value is <code>False</code>.</p> <p>You can also include an Amazon Web Services KMS key ID (<code>KMSKeyId</code>) for at-rest encryption of the <code>OnlineStore</code>.</p>",
+                    "documentation": "<p>You can turn the <code>OnlineStore</code> on or off by specifying <code>True</code> for the <code>EnableOnlineStore</code> flag in <code>OnlineStoreConfig</code>.</p> <p>You can also include an Amazon Web Services KMS key ID (<code>KMSKeyId</code>) for at-rest encryption of the <code>OnlineStore</code>.</p> <p>The default value is <code>False</code>.</p>",
                     "shape": "OnlineStoreConfig"
                 },
                 "RecordIdentifierFeatureName": {
                     "documentation": "<p>The name of the <code>Feature</code> whose value uniquely identifies a <code>Record</code> defined in the <code>FeatureStore</code>. Only the latest record per identifier value will be stored in the <code>OnlineStore</code>. <code>RecordIdentifierFeatureName</code> must be one of feature definitions' names.</p> <p>You use the <code>RecordIdentifierFeatureName</code> to access data in a <code>FeatureStore</code>.</p> <p>This name:</p> <ul> <li> <p>Must start and end with an alphanumeric character.</p> </li> <li> <p>Can only contains alphanumeric characters, hyphens, underscores. Spaces are not allowed. </p> </li> </ul>",
                     "shape": "FeatureName"
                 },
                 "RoleArn": {
@@ -9754,32 +9925,36 @@
             "required": [
                 "HumanTaskUiArn"
             ],
             "type": "structure"
         },
         "CreateHyperParameterTuningJobRequest": {
             "members": {
+                "Autotune": {
+                    "documentation": "<p>Configures SageMaker Automatic model tuning (AMT) to automatically find optimal parameters for the following fields:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobConfig.html#sagemaker-Type-HyperParameterTuningJobConfig-ParameterRanges\">ParameterRanges</a>: The names and ranges of parameters that a hyperparameter tuning job can optimize.</p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ResourceLimits.html\">ResourceLimits</a>: The maximum resources that can be used for a training job. These resources include the maximum number of training jobs, the maximum runtime of a tuning job, and the maximum number of training jobs to run at the same time.</p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobConfig.html#sagemaker-Type-HyperParameterTuningJobConfig-TrainingJobEarlyStoppingType\">TrainingJobEarlyStoppingType</a>: A flag that specifies whether or not to use early stopping for training jobs launched by a hyperparameter tuning job.</p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTrainingJobDefinition.html#sagemaker-Type-HyperParameterTrainingJobDefinition-RetryStrategy\">RetryStrategy</a>: The number of times to retry a training job.</p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobConfig.html\">Strategy</a>: Specifies how hyperparameter tuning chooses the combinations of hyperparameter values to use for the training jobs that it launches.</p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ConvergenceDetected.html\">ConvergenceDetected</a>: A flag to indicate that Automatic model tuning (AMT) has detected model convergence.</p> </li> </ul>",
+                    "shape": "Autotune"
+                },
                 "HyperParameterTuningJobConfig": {
-                    "documentation": "<p>The <a>HyperParameterTuningJobConfig</a> object that describes the tuning job, including the search strategy, the objective metric used to evaluate training jobs, ranges of parameters to search, and resource limits for the tuning job. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-how-it-works.html\">How Hyperparameter Tuning Works</a>.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobConfig.html\">HyperParameterTuningJobConfig</a> object that describes the tuning job, including the search strategy, the objective metric used to evaluate training jobs, ranges of parameters to search, and resource limits for the tuning job. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-how-it-works.html\">How Hyperparameter Tuning Works</a>.</p>",
                     "shape": "HyperParameterTuningJobConfig"
                 },
                 "HyperParameterTuningJobName": {
                     "documentation": "<p>The name of the tuning job. This name is the prefix for the names of all training jobs that this tuning job launches. The name must be unique within the same Amazon Web Services account and Amazon Web Services Region. The name must have 1 to 32 characters. Valid characters are a-z, A-Z, 0-9, and : + = @ _ % - (hyphen). The name is not case sensitive.</p>",
                     "shape": "HyperParameterTuningJobName"
                 },
                 "Tags": {
                     "documentation": "<p>An array of key-value pairs. You can use tags to categorize your Amazon Web Services resources in different ways, for example, by purpose, owner, or environment. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a>.</p> <p>Tags that you specify for the tuning job are also added to all training jobs that the tuning job launches.</p>",
                     "shape": "TagList"
                 },
                 "TrainingJobDefinition": {
-                    "documentation": "<p>The <a>HyperParameterTrainingJobDefinition</a> object that describes the training jobs that this tuning job launches, including static hyperparameters, input data configuration, output data configuration, resource configuration, and stopping condition.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTrainingJobDefinition.html\">HyperParameterTrainingJobDefinition</a> object that describes the training jobs that this tuning job launches, including static hyperparameters, input data configuration, output data configuration, resource configuration, and stopping condition.</p>",
                     "shape": "HyperParameterTrainingJobDefinition"
                 },
                 "TrainingJobDefinitions": {
-                    "documentation": "<p>A list of the <a>HyperParameterTrainingJobDefinition</a> objects launched for this tuning job.</p>",
+                    "documentation": "<p>A list of the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTrainingJobDefinition.html\">HyperParameterTrainingJobDefinition</a> objects launched for this tuning job.</p>",
                     "shape": "HyperParameterTrainingJobDefinitions"
                 },
                 "WarmStartConfig": {
                     "documentation": "<p>Specifies the configuration for starting the hyperparameter tuning job using one or more previous tuning jobs as a starting point. The results of previous tuning jobs are used to inform which combinations of hyperparameters to search over in the new tuning job.</p> <p>All training jobs launched by the new hyperparameter tuning job are evaluated by using the objective metric. If you specify <code>IDENTICAL_DATA_AND_ALGORITHM</code> as the <code>WarmStartType</code> value for the warm start configuration, the training job that performs the best in the new tuning job is compared to the best training jobs from the parent tuning jobs. From these, the training job that performs the best as measured by the objective metric is returned as the overall best training job.</p> <note> <p>All training jobs launched by parent hyperparameter tuning jobs and the new hyperparameter tuning jobs count against the limit of training jobs for the tuning job.</p> </note>",
                     "shape": "HyperParameterTuningJobWarmStartConfig"
                 }
             },
@@ -9979,15 +10154,15 @@
                     "shape": "RecommendationJobInputConfig"
                 },
                 "JobDescription": {
                     "documentation": "<p>Description of the recommendation job.</p>",
                     "shape": "RecommendationJobDescription"
                 },
                 "JobName": {
-                    "documentation": "<p>A name for the recommendation job. The name must be unique within the Amazon Web Services Region and within your Amazon Web Services account.</p>",
+                    "documentation": "<p>A name for the recommendation job. The name must be unique within the Amazon Web Services Region and within your Amazon Web Services account. The job name is passed down to the resources created by the recommendation job. The names of resources (such as the model, endpoint configuration, endpoint, and compilation) that are prefixed with the job name are truncated at 40 characters.</p>",
                     "shape": "RecommendationJobName"
                 },
                 "JobType": {
                     "documentation": "<p>Defines the type of recommendation job. Specify <code>Default</code> to initiate an instance recommendation and <code>Advanced</code> to initiate a load test. If left unspecified, Amazon SageMaker Inference Recommender will run an instance recommendation (<code>DEFAULT</code>) job.</p>",
                     "shape": "RecommendationJobType"
                 },
                 "OutputConfig": {
@@ -10191,15 +10366,15 @@
                 "ModelCardExportJobArn"
             ],
             "type": "structure"
         },
         "CreateModelCardRequest": {
             "members": {
                 "Content": {
-                    "documentation": "<p>The content of the model card. Content must be in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-cards-api-json-schema.html\">model card JSON schema</a> and provided as a string.</p>",
+                    "documentation": "<p>The content of the model card. Content must be in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-cards.html#model-cards-json-schema\">model card JSON schema</a> and provided as a string.</p>",
                     "shape": "ModelCardContent"
                 },
                 "ModelCardName": {
                     "documentation": "<p>The unique name of the model card.</p>",
                     "shape": "EntityName"
                 },
                 "ModelCardStatus": {
@@ -10323,15 +10498,15 @@
                     "shape": "ContainerDefinition"
                 },
                 "Tags": {
                     "documentation": "<p>An array of key-value pairs. You can use tags to categorize your Amazon Web Services resources in different ways, for example, by purpose, owner, or environment. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a>.</p>",
                     "shape": "TagList"
                 },
                 "VpcConfig": {
-                    "documentation": "<p>A <a>VpcConfig</a> object that specifies the VPC that you want your model to connect to. Control access to and from your model container by configuring the VPC. <code>VpcConfig</code> is used in hosting services and in batch transform. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/host-vpc.html\">Protect Endpoints by Using an Amazon Virtual Private Cloud</a> and <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/batch-vpc.html\">Protect Data in Batch Transform Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
+                    "documentation": "<p>A <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_VpcConfig.html\">VpcConfig</a> object that specifies the VPC that you want your model to connect to. Control access to and from your model container by configuring the VPC. <code>VpcConfig</code> is used in hosting services and in batch transform. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/host-vpc.html\">Protect Endpoints by Using an Amazon Virtual Private Cloud</a> and <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/batch-vpc.html\">Protect Data in Batch Transform Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
                     "shape": "VpcConfig"
                 }
             },
             "required": [
                 "ModelName",
                 "ExecutionRoleArn"
             ],
@@ -10685,15 +10860,15 @@
                     "shape": "IdempotencyToken"
                 },
                 "ParallelismConfiguration": {
                     "documentation": "<p>This is the configuration that controls the parallelism of the pipeline. If specified, it applies to all runs of this pipeline by default.</p>",
                     "shape": "ParallelismConfiguration"
                 },
                 "PipelineDefinition": {
-                    "documentation": "<p>The JSON pipeline definition of the pipeline.</p>",
+                    "documentation": "<p>The <a href=\"https://aws-sagemaker-mlops.github.io/sagemaker-model-building-pipeline-definition-JSON-schema/\">JSON pipeline definition</a> of the pipeline.</p>",
                     "shape": "PipelineDefinition"
                 },
                 "PipelineDefinitionS3Location": {
                     "documentation": "<p>The location of the pipeline definition stored in Amazon S3. If specified, SageMaker will retrieve the pipeline definition from this location.</p>",
                     "shape": "PipelineDefinitionS3Location"
                 },
                 "PipelineDescription": {
@@ -11010,15 +11185,15 @@
                     "shape": "ExperimentConfig"
                 },
                 "HyperParameters": {
                     "documentation": "<p>Algorithm-specific parameters that influence the quality of the model. You set hyperparameters before you start the learning process. For a list of hyperparameters for each training algorithm provided by SageMaker, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/algos.html\">Algorithms</a>. </p> <p>You can specify a maximum of 100 hyperparameters. Each hyperparameter is a key-value pair. Each key and value is limited to 256 characters, as specified by the <code>Length Constraint</code>. </p> <important> <p>Do not include any security-sensitive information including account access IDs, secrets or tokens in any hyperparameter field. If the use of security-sensitive credentials are detected, SageMaker will reject your training job request and return an exception error.</p> </important>",
                     "shape": "HyperParameters"
                 },
                 "InputDataConfig": {
-                    "documentation": "<p>An array of <code>Channel</code> objects. Each channel is a named input source. <code>InputDataConfig</code> describes the input data and its location. </p> <p>Algorithms can accept input data from one or more channels. For example, an algorithm might have two channels of input data, <code>training_data</code> and <code>validation_data</code>. The configuration for each channel provides the S3, EFS, or FSx location where the input data is stored. It also provides information about the stored data: the MIME type, compression method, and whether the data is wrapped in RecordIO format. </p> <p>Depending on the input mode that the algorithm supports, SageMaker either copies input data files from an S3 bucket to a local directory in the Docker container, or makes it available as input streams. For example, if you specify an EFS location, input data files are available as input streams. They do not need to be downloaded.</p>",
+                    "documentation": "<p>An array of <code>Channel</code> objects. Each channel is a named input source. <code>InputDataConfig</code> describes the input data and its location. </p> <p>Algorithms can accept input data from one or more channels. For example, an algorithm might have two channels of input data, <code>training_data</code> and <code>validation_data</code>. The configuration for each channel provides the S3, EFS, or FSx location where the input data is stored. It also provides information about the stored data: the MIME type, compression method, and whether the data is wrapped in RecordIO format. </p> <p>Depending on the input mode that the algorithm supports, SageMaker either copies input data files from an S3 bucket to a local directory in the Docker container, or makes it available as input streams. For example, if you specify an EFS location, input data files are available as input streams. They do not need to be downloaded.</p> <p>Your input must be in the same Amazon Web Services region as your training job.</p>",
                     "shape": "InputDataConfig"
                 },
                 "OutputDataConfig": {
                     "documentation": "<p>Specifies the path to the S3 location where you want to store model artifacts. SageMaker creates subfolders for the artifacts. </p>",
                     "shape": "OutputDataConfig"
                 },
                 "ProfilerConfig": {
@@ -11052,15 +11227,15 @@
                     "shape": "TensorBoardOutputConfig"
                 },
                 "TrainingJobName": {
                     "documentation": "<p>The name of the training job. The name must be unique within an Amazon Web Services Region in an Amazon Web Services account. </p>",
                     "shape": "TrainingJobName"
                 },
                 "VpcConfig": {
-                    "documentation": "<p>A <a>VpcConfig</a> object that specifies the VPC that you want your training job to connect to. Control access to and from your training container by configuring the VPC. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/train-vpc.html\">Protect Training Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
+                    "documentation": "<p>A <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_VpcConfig.html\">VpcConfig</a> object that specifies the VPC that you want your training job to connect to. Control access to and from your training container by configuring the VPC. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/train-vpc.html\">Protect Training Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
                     "shape": "VpcConfig"
                 }
             },
             "required": [
                 "TrainingJobName",
                 "AlgorithmSpecification",
                 "RoleArn",
@@ -11191,15 +11366,15 @@
                     "shape": "Timestamp"
                 },
                 "Status": {
                     "documentation": "<p>The status of the component. States include:</p> <ul> <li> <p>InProgress</p> </li> <li> <p>Completed</p> </li> <li> <p>Failed</p> </li> </ul>",
                     "shape": "TrialComponentStatus"
                 },
                 "Tags": {
-                    "documentation": "<p>A list of tags to associate with the component. You can use <a>Search</a> API to search on the tags.</p>",
+                    "documentation": "<p>A list of tags to associate with the component. You can use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API to search on the tags.</p>",
                     "shape": "TagList"
                 },
                 "TrialComponentName": {
                     "documentation": "<p>The name of the component. The name must be unique in your Amazon Web Services account and is not case-sensitive.</p>",
                     "shape": "ExperimentEntityName"
                 }
             },
@@ -11227,15 +11402,15 @@
                     "documentation": "<p>The name of the experiment to associate the trial with.</p>",
                     "shape": "ExperimentEntityName"
                 },
                 "MetadataProperties": {
                     "shape": "MetadataProperties"
                 },
                 "Tags": {
-                    "documentation": "<p>A list of tags to associate with the trial. You can use <a>Search</a> API to search on the tags.</p>",
+                    "documentation": "<p>A list of tags to associate with the trial. You can use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API to search on the tags.</p>",
                     "shape": "TagList"
                 },
                 "TrialName": {
                     "documentation": "<p>The name of the trial. The name must be unique in your Amazon Web Services account and is not case-sensitive.</p>",
                     "shape": "ExperimentEntityName"
                 }
             },
@@ -11800,25 +11975,25 @@
             "min": 0,
             "type": "integer"
         },
         "DefaultSpaceSettings": {
             "documentation": "<p>A collection of settings that apply to spaces created in the Domain.</p>",
             "members": {
                 "ExecutionRole": {
-                    "documentation": "<p>The execution role for the space.</p>",
+                    "documentation": "<p>The ARN of the execution role for the space.</p>",
                     "shape": "RoleArn"
                 },
                 "JupyterServerAppSettings": {
                     "shape": "JupyterServerAppSettings"
                 },
                 "KernelGatewayAppSettings": {
                     "shape": "KernelGatewayAppSettings"
                 },
                 "SecurityGroups": {
-                    "documentation": "<p>The security groups for the Amazon Virtual Private Cloud that the space uses for communication.</p>",
+                    "documentation": "<p>The security group IDs for the Amazon Virtual Private Cloud that the space uses for communication.</p>",
                     "shape": "SecurityGroupIds"
                 }
             },
             "type": "structure"
         },
         "DefaultUid": {
             "max": 65535,
@@ -12573,15 +12748,15 @@
         },
         "DependencyOriginPath": {
             "max": 1023,
             "pattern": ".*",
             "type": "string"
         },
         "DeployedImage": {
-            "documentation": "<p>Gets the Amazon EC2 Container Registry path of the docker image of the model that is hosted in this <a>ProductionVariant</a>.</p> <p>If you used the <code>registry/repository[:tag]</code> form to specify the image path of the primary container when you created the model hosted in this <code>ProductionVariant</code>, the path resolves to a path of the form <code>registry/repository[@digest]</code>. A digest is a hash value that identifies a specific version of an image. For information about Amazon ECR paths, see <a href=\"https://docs.aws.amazon.com/AmazonECR/latest/userguide/docker-pull-ecr-image.html\">Pulling an Image</a> in the <i>Amazon ECR User Guide</i>.</p>",
+            "documentation": "<p>Gets the Amazon EC2 Container Registry path of the docker image of the model that is hosted in this <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ProductionVariant.html\">ProductionVariant</a>.</p> <p>If you used the <code>registry/repository[:tag]</code> form to specify the image path of the primary container when you created the model hosted in this <code>ProductionVariant</code>, the path resolves to a path of the form <code>registry/repository[@digest]</code>. A digest is a hash value that identifies a specific version of an image. For information about Amazon ECR paths, see <a href=\"https://docs.aws.amazon.com/AmazonECR/latest/userguide/docker-pull-ecr-image.html\">Pulling an Image</a> in the <i>Amazon ECR User Guide</i>.</p>",
             "members": {
                 "ResolutionTime": {
                     "documentation": "<p>The date and time when the image path for the model resolved to the <code>ResolvedImage</code> </p>",
                     "shape": "Timestamp"
                 },
                 "ResolvedImage": {
                     "documentation": "<p>The specific digest path of the image hosted in this <code>ProductionVariant</code>.</p>",
@@ -12606,18 +12781,36 @@
                 "AutoRollbackConfiguration": {
                     "documentation": "<p>Automatic rollback configuration for handling endpoint deployment failures and recovery.</p>",
                     "shape": "AutoRollbackConfig"
                 },
                 "BlueGreenUpdatePolicy": {
                     "documentation": "<p>Update policy for a blue/green deployment. If this update policy is specified, SageMaker creates a new fleet during the deployment while maintaining the old fleet. SageMaker flips traffic to the new fleet according to the specified traffic routing configuration. Only one update policy should be used in the deployment configuration. If no update policy is specified, SageMaker uses a blue/green deployment strategy with all at once traffic shifting by default.</p>",
                     "shape": "BlueGreenUpdatePolicy"
+                },
+                "RollingUpdatePolicy": {
+                    "documentation": "<p>Specifies a rolling deployment strategy for updating a SageMaker endpoint.</p>",
+                    "shape": "RollingUpdatePolicy"
+                }
+            },
+            "type": "structure"
+        },
+        "DeploymentRecommendation": {
+            "documentation": "<p>A set of recommended deployment configurations for the model. To get more advanced recommendations, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateInferenceRecommendationsJob.html\">CreateInferenceRecommendationsJob</a> to create an inference recommendation job.</p>",
+            "members": {
+                "RealTimeInferenceRecommendations": {
+                    "documentation": "<p>A list of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_RealTimeInferenceRecommendation.html\">RealTimeInferenceRecommendation</a> items.</p>",
+                    "shape": "RealTimeInferenceRecommendations"
+                },
+                "RecommendationStatus": {
+                    "documentation": "<p>Status of the deployment recommendation. The status <code>NOT_APPLICABLE</code> means that SageMaker is unable to provide a default recommendation for the model using the information provided. If the deployment status is <code>IN_PROGRESS</code>, retry your API call after a few seconds to get a <code>COMPLETED</code> deployment recommendation.</p>",
+                    "shape": "RecommendationStatus"
                 }
             },
             "required": [
-                "BlueGreenUpdatePolicy"
+                "RecommendationStatus"
             ],
             "type": "structure"
         },
         "DeploymentStage": {
             "documentation": "<p>Contains information about a stage in an edge deployment plan.</p>",
             "members": {
                 "DeploymentConfig": {
@@ -13100,15 +13293,15 @@
                     "shape": "AutoMLPartialFailureReasons"
                 },
                 "ProblemType": {
                     "documentation": "<p>Returns the job's problem type.</p>",
                     "shape": "ProblemType"
                 },
                 "ResolvedAttributes": {
-                    "documentation": "<p>Contains <code>ProblemType</code>, <code>AutoMLJobObjective</code>, and <code>CompletionCriteria</code>. If you do not provide these values, they are auto-inferred. If you do provide them, the values used are the ones you provide.</p>",
+                    "documentation": "<p>Contains <code>ProblemType</code>, <code>AutoMLJobObjective</code>, and <code>CompletionCriteria</code>. If you do not provide these values, they are inferred.</p>",
                     "shape": "ResolvedAttributes"
                 },
                 "RoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Identity and Access Management (IAM) role that has read permission to the input data location and write permission to the output data location in Amazon S3.</p>",
                     "shape": "RoleArn"
                 }
             },
@@ -13124,71 +13317,78 @@
                 "AutoMLJobSecondaryStatus"
             ],
             "type": "structure"
         },
         "DescribeAutoMLJobV2Request": {
             "members": {
                 "AutoMLJobName": {
-                    "documentation": "<p>Requests information about an AutoML V2 job using its unique name.</p>",
+                    "documentation": "<p>Requests information about an AutoML job V2 using its unique name.</p>",
                     "shape": "AutoMLJobName"
                 }
             },
             "required": [
                 "AutoMLJobName"
             ],
             "type": "structure"
         },
         "DescribeAutoMLJobV2Response": {
             "members": {
                 "AutoMLJobArn": {
-                    "documentation": "<p>Returns the Amazon Resource Name (ARN) of the AutoML V2 job.</p>",
+                    "documentation": "<p>Returns the Amazon Resource Name (ARN) of the AutoML job V2.</p>",
                     "shape": "AutoMLJobArn"
                 },
+                "AutoMLJobArtifacts": {
+                    "shape": "AutoMLJobArtifacts"
+                },
                 "AutoMLJobInputDataConfig": {
                     "documentation": "<p>Returns an array of channel objects describing the input data and their location.</p>",
                     "shape": "AutoMLJobInputDataConfig"
                 },
                 "AutoMLJobName": {
-                    "documentation": "<p>Returns the name of the AutoML V2 job.</p>",
+                    "documentation": "<p>Returns the name of the AutoML job V2.</p>",
                     "shape": "AutoMLJobName"
                 },
                 "AutoMLJobObjective": {
                     "documentation": "<p>Returns the job's objective.</p>",
                     "shape": "AutoMLJobObjective"
                 },
                 "AutoMLJobSecondaryStatus": {
-                    "documentation": "<p>Returns the secondary status of the AutoML V2 job.</p>",
+                    "documentation": "<p>Returns the secondary status of the AutoML job V2.</p>",
                     "shape": "AutoMLJobSecondaryStatus"
                 },
                 "AutoMLJobStatus": {
-                    "documentation": "<p>Returns the status of the AutoML V2 job.</p>",
+                    "documentation": "<p>Returns the status of the AutoML job V2.</p>",
                     "shape": "AutoMLJobStatus"
                 },
                 "AutoMLProblemTypeConfig": {
-                    "documentation": "<p>Returns the configuration settings of the problem type set for the AutoML V2 job.</p>",
+                    "documentation": "<p>Returns the configuration settings of the problem type set for the AutoML job V2.</p>",
                     "shape": "AutoMLProblemTypeConfig"
                 },
+                "AutoMLProblemTypeConfigName": {
+                    "documentation": "<p>Returns the name of the problem type configuration set for the AutoML job V2.</p>",
+                    "shape": "AutoMLProblemTypeConfigName"
+                },
                 "BestCandidate": {
                     "documentation": "<p>Information about the candidate produced by an AutoML training job V2, including its status, steps, and other properties.</p>",
                     "shape": "AutoMLCandidate"
                 },
                 "CreationTime": {
-                    "documentation": "<p>Returns the creation time of the AutoML V2 job.</p>",
+                    "documentation": "<p>Returns the creation time of the AutoML job V2.</p>",
                     "shape": "Timestamp"
                 },
                 "DataSplitConfig": {
                     "documentation": "<p>Returns the configuration settings of how the data are split into train and validation datasets.</p>",
                     "shape": "AutoMLDataSplitConfig"
                 },
                 "EndTime": {
-                    "documentation": "<p>Returns the end time of the AutoML V2 job.</p>",
+                    "documentation": "<p>Returns the end time of the AutoML job V2.</p>",
                     "shape": "Timestamp"
                 },
                 "FailureReason": {
-                    "documentation": "<p>Returns the reason for the failure of the AutoML V2 job, when applicable.</p>",
+                    "documentation": "<p>Returns the reason for the failure of the AutoML job V2, when applicable.</p>",
                     "shape": "AutoMLFailureReason"
                 },
                 "LastModifiedTime": {
                     "documentation": "<p>Returns the job's last modified time.</p>",
                     "shape": "Timestamp"
                 },
                 "ModelDeployConfig": {
@@ -13200,17 +13400,21 @@
                     "shape": "ModelDeployResult"
                 },
                 "OutputDataConfig": {
                     "documentation": "<p>Returns the job's output data config.</p>",
                     "shape": "AutoMLOutputDataConfig"
                 },
                 "PartialFailureReasons": {
-                    "documentation": "<p>Returns a list of reasons for partial failures within an AutoML V2 job.</p>",
+                    "documentation": "<p>Returns a list of reasons for partial failures within an AutoML job V2.</p>",
                     "shape": "AutoMLPartialFailureReasons"
                 },
+                "ResolvedAttributes": {
+                    "documentation": "<p>Returns the resolved attributes used by the AutoML job V2.</p>",
+                    "shape": "AutoMLResolvedAttributes"
+                },
                 "RoleArn": {
                     "documentation": "<p>The ARN of the Identity and Access Management role that has read permission to the input data location and write permission to the output data location in Amazon S3.</p>",
                     "shape": "RoleArn"
                 },
                 "SecurityConfig": {
                     "documentation": "<p>Returns the security configuration for traffic encryption or Amazon VPC settings.</p>",
                     "shape": "AutoMLSecurityConfig"
@@ -13299,15 +13503,15 @@
                     "shape": "EntityName"
                 },
                 "CompilationJobStatus": {
                     "documentation": "<p>The status of the model compilation job.</p>",
                     "shape": "CompilationJobStatus"
                 },
                 "CompilationStartTime": {
-                    "documentation": "<p>The time when the model compilation job started the <code>CompilationJob</code> instances. </p> <p>You are billed for the time between this timestamp and the timestamp in the <a>DescribeCompilationJobResponse$CompilationEndTime</a> field. In Amazon CloudWatch Logs, the start time might be later than this time. That's because it takes time to download the compilation job, which depends on the size of the compilation job container. </p>",
+                    "documentation": "<p>The time when the model compilation job started the <code>CompilationJob</code> instances. </p> <p>You are billed for the time between this timestamp and the timestamp in the <code>CompilationEndTime</code> field. In Amazon CloudWatch Logs, the start time might be later than this time. That's because it takes time to download the compilation job, which depends on the size of the compilation job container. </p>",
                     "shape": "Timestamp"
                 },
                 "CreationTime": {
                     "documentation": "<p>The time that the model compilation job was created.</p>",
                     "shape": "CreationTime"
                 },
                 "FailureReason": {
@@ -13347,15 +13551,15 @@
                     "shape": "RoleArn"
                 },
                 "StoppingCondition": {
                     "documentation": "<p>Specifies a limit to how long a model compilation job can run. When the job reaches the time limit, Amazon SageMaker ends the compilation job. Use this API to cap model training costs.</p>",
                     "shape": "StoppingCondition"
                 },
                 "VpcConfig": {
-                    "documentation": "<p>A <a>VpcConfig</a> object that specifies the VPC that you want your compilation job to connect to. Control access to your models by configuring the VPC. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/neo-vpc.html\">Protect Compilation Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
+                    "documentation": "<p>A <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_VpcConfig.html\">VpcConfig</a> object that specifies the VPC that you want your compilation job to connect to. Control access to your models by configuring the VPC. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/neo-vpc.html\">Protect Compilation Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
                     "shape": "NeoVpcConfig"
                 }
             },
             "required": [
                 "CompilationJobName",
                 "CompilationJobArn",
                 "CompilationJobStatus",
@@ -13981,15 +14185,15 @@
                     "shape": "EndpointConfigName"
                 },
                 "EndpointName": {
                     "documentation": "<p>Name of the endpoint.</p>",
                     "shape": "EndpointName"
                 },
                 "EndpointStatus": {
-                    "documentation": "<p>The status of the endpoint.</p> <ul> <li> <p> <code>OutOfService</code>: Endpoint is not available to take incoming requests.</p> </li> <li> <p> <code>Creating</code>: <a>CreateEndpoint</a> is executing.</p> </li> <li> <p> <code>Updating</code>: <a>UpdateEndpoint</a> or <a>UpdateEndpointWeightsAndCapacities</a> is executing.</p> </li> <li> <p> <code>SystemUpdating</code>: Endpoint is undergoing maintenance and cannot be updated or deleted or re-scaled until it has completed. This maintenance operation does not change any customer-specified values such as VPC config, KMS encryption, model, instance type, or instance count.</p> </li> <li> <p> <code>RollingBack</code>: Endpoint fails to scale up or down or change its variant weight and is in the process of rolling back to its previous configuration. Once the rollback completes, endpoint returns to an <code>InService</code> status. This transitional status only applies to an endpoint that has autoscaling enabled and is undergoing variant weight or capacity changes as part of an <a>UpdateEndpointWeightsAndCapacities</a> call or when the <a>UpdateEndpointWeightsAndCapacities</a> operation is called explicitly.</p> </li> <li> <p> <code>InService</code>: Endpoint is available to process incoming requests.</p> </li> <li> <p> <code>Deleting</code>: <a>DeleteEndpoint</a> is executing.</p> </li> <li> <p> <code>Failed</code>: Endpoint could not be created, updated, or re-scaled. Use <a>DescribeEndpointOutput$FailureReason</a> for information about the failure. <a>DeleteEndpoint</a> is the only operation that can be performed on a failed endpoint.</p> </li> </ul>",
+                    "documentation": "<p>The status of the endpoint.</p> <ul> <li> <p> <code>OutOfService</code>: Endpoint is not available to take incoming requests.</p> </li> <li> <p> <code>Creating</code>: <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpoint.html\">CreateEndpoint</a> is executing.</p> </li> <li> <p> <code>Updating</code>: <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateEndpoint.html\">UpdateEndpoint</a> or <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateEndpointWeightsAndCapacities.html\">UpdateEndpointWeightsAndCapacities</a> is executing.</p> </li> <li> <p> <code>SystemUpdating</code>: Endpoint is undergoing maintenance and cannot be updated or deleted or re-scaled until it has completed. This maintenance operation does not change any customer-specified values such as VPC config, KMS encryption, model, instance type, or instance count.</p> </li> <li> <p> <code>RollingBack</code>: Endpoint fails to scale up or down or change its variant weight and is in the process of rolling back to its previous configuration. Once the rollback completes, endpoint returns to an <code>InService</code> status. This transitional status only applies to an endpoint that has autoscaling enabled and is undergoing variant weight or capacity changes as part of an <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateEndpointWeightsAndCapacities.html\">UpdateEndpointWeightsAndCapacities</a> call or when the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateEndpointWeightsAndCapacities.html\">UpdateEndpointWeightsAndCapacities</a> operation is called explicitly.</p> </li> <li> <p> <code>InService</code>: Endpoint is available to process incoming requests.</p> </li> <li> <p> <code>Deleting</code>: <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DeleteEndpoint.html\">DeleteEndpoint</a> is executing.</p> </li> <li> <p> <code>Failed</code>: Endpoint could not be created, updated, or re-scaled. Use the <code>FailureReason</code> value returned by <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeEndpoint.html\">DescribeEndpoint</a> for information about the failure. <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DeleteEndpoint.html\">DeleteEndpoint</a> is the only operation that can be performed on a failed endpoint.</p> </li> </ul>",
                     "shape": "EndpointStatus"
                 },
                 "ExplainerConfig": {
                     "documentation": "<p>The configuration parameters for an explainer.</p>",
                     "shape": "ExplainerConfig"
                 },
                 "FailureReason": {
@@ -14005,19 +14209,19 @@
                     "shape": "Timestamp"
                 },
                 "PendingDeploymentSummary": {
                     "documentation": "<p>Returns the summary of an in-progress deployment. This field is only returned when the endpoint is creating or updating with a new endpoint configuration.</p>",
                     "shape": "PendingDeploymentSummary"
                 },
                 "ProductionVariants": {
-                    "documentation": "<p>An array of <a>ProductionVariantSummary</a> objects, one for each model hosted behind this endpoint.</p>",
+                    "documentation": "<p>An array of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ProductionVariantSummary.html\">ProductionVariantSummary</a> objects, one for each model hosted behind this endpoint.</p>",
                     "shape": "ProductionVariantSummaryList"
                 },
                 "ShadowProductionVariants": {
-                    "documentation": "<p>An array of <a>ProductionVariantSummary</a> objects, one for each model that you want to host at this endpoint in shadow mode with production traffic replicated from the model specified on <code>ProductionVariants</code>.</p>",
+                    "documentation": "<p>An array of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ProductionVariantSummary.html\">ProductionVariantSummary</a> objects, one for each model that you want to host at this endpoint in shadow mode with production traffic replicated from the model specified on <code>ProductionVariants</code>.</p>",
                     "shape": "ProductionVariantSummaryList"
                 }
             },
             "required": [
                 "EndpointName",
                 "EndpointArn",
                 "EndpointConfigName",
@@ -14529,16 +14733,20 @@
             "required": [
                 "HyperParameterTuningJobName"
             ],
             "type": "structure"
         },
         "DescribeHyperParameterTuningJobResponse": {
             "members": {
+                "Autotune": {
+                    "documentation": "<p>A flag to indicate if autotune is enabled for the hyperparameter tuning job.</p>",
+                    "shape": "Autotune"
+                },
                 "BestTrainingJob": {
-                    "documentation": "<p>A <a>TrainingJobSummary</a> object that describes the training job that completed with the best current <a>HyperParameterTuningJobObjective</a>.</p>",
+                    "documentation": "<p>A <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_TrainingJobSummary.html\">TrainingJobSummary</a> object that describes the training job that completed with the best current <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobObjective.html\">HyperParameterTuningJobObjective</a>.</p>",
                     "shape": "HyperParameterTrainingJobSummary"
                 },
                 "ConsumedResources": {
                     "shape": "HyperParameterTuningJobConsumedResources"
                 },
                 "CreationTime": {
                     "documentation": "<p>The date and time that the tuning job started.</p>",
@@ -14553,47 +14761,47 @@
                     "shape": "Timestamp"
                 },
                 "HyperParameterTuningJobArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the tuning job.</p>",
                     "shape": "HyperParameterTuningJobArn"
                 },
                 "HyperParameterTuningJobConfig": {
-                    "documentation": "<p>The <a>HyperParameterTuningJobConfig</a> object that specifies the configuration of the tuning job.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobConfig.html\">HyperParameterTuningJobConfig</a> object that specifies the configuration of the tuning job.</p>",
                     "shape": "HyperParameterTuningJobConfig"
                 },
                 "HyperParameterTuningJobName": {
-                    "documentation": "<p>The name of the tuning job.</p>",
+                    "documentation": "<p>The name of the hyperparameter tuning job.</p>",
                     "shape": "HyperParameterTuningJobName"
                 },
                 "HyperParameterTuningJobStatus": {
                     "documentation": "<p>The status of the tuning job: InProgress, Completed, Failed, Stopping, or Stopped.</p>",
                     "shape": "HyperParameterTuningJobStatus"
                 },
                 "LastModifiedTime": {
                     "documentation": "<p>The date and time that the status of the tuning job was modified. </p>",
                     "shape": "Timestamp"
                 },
                 "ObjectiveStatusCounters": {
-                    "documentation": "<p>The <a>ObjectiveStatusCounters</a> object that specifies the number of training jobs, categorized by the status of their final objective metric, that this tuning job launched.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ObjectiveStatusCounters.html\">ObjectiveStatusCounters</a> object that specifies the number of training jobs, categorized by the status of their final objective metric, that this tuning job launched.</p>",
                     "shape": "ObjectiveStatusCounters"
                 },
                 "OverallBestTrainingJob": {
-                    "documentation": "<p>If the hyperparameter tuning job is an warm start tuning job with a <code>WarmStartType</code> of <code>IDENTICAL_DATA_AND_ALGORITHM</code>, this is the <a>TrainingJobSummary</a> for the training job with the best objective metric value of all training jobs launched by this tuning job and all parent jobs specified for the warm start tuning job.</p>",
+                    "documentation": "<p>If the hyperparameter tuning job is an warm start tuning job with a <code>WarmStartType</code> of <code>IDENTICAL_DATA_AND_ALGORITHM</code>, this is the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_TrainingJobSummary.html\">TrainingJobSummary</a> for the training job with the best objective metric value of all training jobs launched by this tuning job and all parent jobs specified for the warm start tuning job.</p>",
                     "shape": "HyperParameterTrainingJobSummary"
                 },
                 "TrainingJobDefinition": {
-                    "documentation": "<p>The <a>HyperParameterTrainingJobDefinition</a> object that specifies the definition of the training jobs that this tuning job launches.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTrainingJobDefinition.html\">HyperParameterTrainingJobDefinition</a> object that specifies the definition of the training jobs that this tuning job launches.</p>",
                     "shape": "HyperParameterTrainingJobDefinition"
                 },
                 "TrainingJobDefinitions": {
-                    "documentation": "<p>A list of the <a>HyperParameterTrainingJobDefinition</a> objects launched for this tuning job.</p>",
+                    "documentation": "<p>A list of the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTrainingJobDefinition.html\">HyperParameterTrainingJobDefinition</a> objects launched for this tuning job.</p>",
                     "shape": "HyperParameterTrainingJobDefinitions"
                 },
                 "TrainingJobStatusCounters": {
-                    "documentation": "<p>The <a>TrainingJobStatusCounters</a> object that specifies the number of training jobs, categorized by status, that this tuning job launched.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_TrainingJobStatusCounters.html\">TrainingJobStatusCounters</a> object that specifies the number of training jobs, categorized by status, that this tuning job launched.</p>",
                     "shape": "TrainingJobStatusCounters"
                 },
                 "TuningJobCompletionDetails": {
                     "documentation": "<p>Tuning job completion information returned as the response from a hyperparameter tuning job. This information tells if your tuning job has or has not converged. It also includes the number of training jobs that have not improved model performance as evaluated against the objective function.</p>",
                     "shape": "HyperParameterTuningJobCompletionDetails"
                 },
                 "WarmStartConfig": {
@@ -14789,15 +14997,15 @@
                     "shape": "InferenceExperimentDescription"
                 },
                 "EndpointMetadata": {
                     "documentation": "<p>The metadata of the endpoint on which the inference experiment ran.</p>",
                     "shape": "EndpointMetadata"
                 },
                 "KmsKey": {
-                    "documentation": "<p> The Amazon Web Services Key Management Service (Amazon Web Services KMS) key that Amazon SageMaker uses to encrypt data on the storage volume attached to the ML compute instance that hosts the endpoint. For more information, see <a>CreateInferenceExperimentRequest$KmsKey</a>. </p>",
+                    "documentation": "<p> The Amazon Web Services Key Management Service (Amazon Web Services KMS) key that Amazon SageMaker uses to encrypt data on the storage volume attached to the ML compute instance that hosts the endpoint. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateInferenceExperiment.html\">CreateInferenceExperiment</a>. </p>",
                     "shape": "KmsKeyId"
                 },
                 "LastModifiedTime": {
                     "documentation": "<p>The timestamp at which you last modified the inference experiment.</p>",
                     "shape": "Timestamp"
                 },
                 "ModelVariants": {
@@ -14817,19 +15025,19 @@
                     "shape": "InferenceExperimentSchedule"
                 },
                 "ShadowModeConfig": {
                     "documentation": "<p> The configuration of <code>ShadowMode</code> inference experiment type, which shows the production variant that takes all the inference requests, and the shadow variant to which Amazon SageMaker replicates a percentage of the inference requests. For the shadow variant it also shows the percentage of requests that Amazon SageMaker replicates. </p>",
                     "shape": "ShadowModeConfig"
                 },
                 "Status": {
-                    "documentation": "<p> The status of the inference experiment. The following are the possible statuses for an inference experiment: </p> <ul> <li> <p> <code>Creating</code> - Amazon SageMaker is creating your experiment. </p> </li> <li> <p> <code>Created</code> - Amazon SageMaker has finished the creation of your experiment and will begin the experiment at the scheduled time. </p> </li> <li> <p> <code>Updating</code> - When you make changes to your experiment, your experiment shows as updating. </p> </li> <li> <p> <code>Starting</code> - Amazon SageMaker is beginning your experiment. </p> </li> <li> <p> <code>Running</code> - Your experiment is in progress. </p> </li> <li> <p> <code>Stopping</code> - Amazon SageMaker is stopping your experiment. </p> </li> <li> <p> <code>Completed</code> - Your experiment has completed. </p> </li> <li> <p> <code>Cancelled</code> - When you conclude your experiment early using the <a>StopInferenceExperiment</a> API, or if any operation fails with an unexpected error, it shows as cancelled. </p> </li> </ul>",
+                    "documentation": "<p> The status of the inference experiment. The following are the possible statuses for an inference experiment: </p> <ul> <li> <p> <code>Creating</code> - Amazon SageMaker is creating your experiment. </p> </li> <li> <p> <code>Created</code> - Amazon SageMaker has finished the creation of your experiment and will begin the experiment at the scheduled time. </p> </li> <li> <p> <code>Updating</code> - When you make changes to your experiment, your experiment shows as updating. </p> </li> <li> <p> <code>Starting</code> - Amazon SageMaker is beginning your experiment. </p> </li> <li> <p> <code>Running</code> - Your experiment is in progress. </p> </li> <li> <p> <code>Stopping</code> - Amazon SageMaker is stopping your experiment. </p> </li> <li> <p> <code>Completed</code> - Your experiment has completed. </p> </li> <li> <p> <code>Cancelled</code> - When you conclude your experiment early using the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_StopInferenceExperiment.html\">StopInferenceExperiment</a> API, or if any operation fails with an unexpected error, it shows as cancelled. </p> </li> </ul>",
                     "shape": "InferenceExperimentStatus"
                 },
                 "StatusReason": {
-                    "documentation": "<p> The error message or client-specified <code>Reason</code> from the <a>StopInferenceExperiment</a> API, that explains the status of the inference experiment. </p>",
+                    "documentation": "<p> The error message or client-specified <code>Reason</code> from the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_StopInferenceExperiment.html\">StopInferenceExperiment</a> API, that explains the status of the inference experiment. </p>",
                     "shape": "InferenceExperimentStatusReason"
                 },
                 "Type": {
                     "documentation": "<p>The type of the inference experiment.</p>",
                     "shape": "InferenceExperimentType"
                 }
             },
@@ -15368,14 +15576,18 @@
                     "documentation": "<p>The containers in the inference pipeline.</p>",
                     "shape": "ContainerDefinitionList"
                 },
                 "CreationTime": {
                     "documentation": "<p>A timestamp that shows when the model was created.</p>",
                     "shape": "Timestamp"
                 },
+                "DeploymentRecommendation": {
+                    "documentation": "<p>A set of recommended deployment configurations for the model.</p>",
+                    "shape": "DeploymentRecommendation"
+                },
                 "EnableNetworkIsolation": {
                     "documentation": "<p>If <code>True</code>, no inbound or outbound network calls can be made to or from the model container.</p>",
                     "shape": "Boolean"
                 },
                 "ExecutionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that you specified for the model.</p>",
                     "shape": "RoleArn"
@@ -15393,15 +15605,15 @@
                     "shape": "ModelName"
                 },
                 "PrimaryContainer": {
                     "documentation": "<p>The location of the primary inference code, associated artifacts, and custom environment map that the inference code uses when it is deployed in production. </p>",
                     "shape": "ContainerDefinition"
                 },
                 "VpcConfig": {
-                    "documentation": "<p>A <a>VpcConfig</a> object that specifies the VPC that this model has access to. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/host-vpc.html\">Protect Endpoints by Using an Amazon Virtual Private Cloud</a> </p>",
+                    "documentation": "<p>A <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_VpcConfig.html\">VpcConfig</a> object that specifies the VPC that this model has access to. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/host-vpc.html\">Protect Endpoints by Using an Amazon Virtual Private Cloud</a> </p>",
                     "shape": "VpcConfig"
                 }
             },
             "required": [
                 "ModelName",
                 "ExecutionRoleArn",
                 "CreationTime",
@@ -15935,22 +16147,26 @@
                 },
                 "PipelineExecutionStatus": {
                     "documentation": "<p>The status of the pipeline execution.</p>",
                     "shape": "PipelineExecutionStatus"
                 },
                 "PipelineExperimentConfig": {
                     "shape": "PipelineExperimentConfig"
+                },
+                "SelectiveExecutionConfig": {
+                    "documentation": "<p>The selective execution configuration applied to the pipeline run.</p>",
+                    "shape": "SelectiveExecutionConfig"
                 }
             },
             "type": "structure"
         },
         "DescribePipelineRequest": {
             "members": {
                 "PipelineName": {
-                    "documentation": "<p>The name of the pipeline to describe.</p>",
+                    "documentation": "<p>The name or Amazon Resource Name (ARN) of the pipeline to describe.</p>",
                     "shape": "PipelineNameOrArn"
                 }
             },
             "required": [
                 "PipelineName"
             ],
             "type": "structure"
@@ -16428,15 +16644,15 @@
                     "shape": "RetryStrategy"
                 },
                 "RoleArn": {
                     "documentation": "<p>The Amazon Web Services Identity and Access Management (IAM) role configured for the training job. </p>",
                     "shape": "RoleArn"
                 },
                 "SecondaryStatus": {
-                    "documentation": "<p> Provides detailed information about the state of the training job. For detailed information on the secondary status of the training job, see <code>StatusMessage</code> under <a>SecondaryStatusTransition</a>.</p> <p>SageMaker provides primary statuses and secondary statuses that apply to each of them:</p> <dl> <dt>InProgress</dt> <dd> <ul> <li> <p> <code>Starting</code> - Starting the training job.</p> </li> <li> <p> <code>Downloading</code> - An optional stage for algorithms that support <code>File</code> training input mode. It indicates that data is being downloaded to the ML storage volumes.</p> </li> <li> <p> <code>Training</code> - Training is in progress.</p> </li> <li> <p> <code>Interrupted</code> - The job stopped because the managed spot training instances were interrupted. </p> </li> <li> <p> <code>Uploading</code> - Training is complete and the model artifacts are being uploaded to the S3 location.</p> </li> </ul> </dd> <dt>Completed</dt> <dd> <ul> <li> <p> <code>Completed</code> - The training job has completed.</p> </li> </ul> </dd> <dt>Failed</dt> <dd> <ul> <li> <p> <code>Failed</code> - The training job has failed. The reason for the failure is returned in the <code>FailureReason</code> field of <code>DescribeTrainingJobResponse</code>.</p> </li> </ul> </dd> <dt>Stopped</dt> <dd> <ul> <li> <p> <code>MaxRuntimeExceeded</code> - The job stopped because it exceeded the maximum allowed runtime.</p> </li> <li> <p> <code>MaxWaitTimeExceeded</code> - The job stopped because it exceeded the maximum allowed wait time.</p> </li> <li> <p> <code>Stopped</code> - The training job has stopped.</p> </li> </ul> </dd> <dt>Stopping</dt> <dd> <ul> <li> <p> <code>Stopping</code> - Stopping the training job.</p> </li> </ul> </dd> </dl> <important> <p>Valid values for <code>SecondaryStatus</code> are subject to change. </p> </important> <p>We no longer support the following secondary statuses:</p> <ul> <li> <p> <code>LaunchingMLInstances</code> </p> </li> <li> <p> <code>PreparingTraining</code> </p> </li> <li> <p> <code>DownloadingTrainingImage</code> </p> </li> </ul>",
+                    "documentation": "<p> Provides detailed information about the state of the training job. For detailed information on the secondary status of the training job, see <code>StatusMessage</code> under <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_SecondaryStatusTransition.html\">SecondaryStatusTransition</a>.</p> <p>SageMaker provides primary statuses and secondary statuses that apply to each of them:</p> <dl> <dt>InProgress</dt> <dd> <ul> <li> <p> <code>Starting</code> - Starting the training job.</p> </li> <li> <p> <code>Downloading</code> - An optional stage for algorithms that support <code>File</code> training input mode. It indicates that data is being downloaded to the ML storage volumes.</p> </li> <li> <p> <code>Training</code> - Training is in progress.</p> </li> <li> <p> <code>Interrupted</code> - The job stopped because the managed spot training instances were interrupted. </p> </li> <li> <p> <code>Uploading</code> - Training is complete and the model artifacts are being uploaded to the S3 location.</p> </li> </ul> </dd> <dt>Completed</dt> <dd> <ul> <li> <p> <code>Completed</code> - The training job has completed.</p> </li> </ul> </dd> <dt>Failed</dt> <dd> <ul> <li> <p> <code>Failed</code> - The training job has failed. The reason for the failure is returned in the <code>FailureReason</code> field of <code>DescribeTrainingJobResponse</code>.</p> </li> </ul> </dd> <dt>Stopped</dt> <dd> <ul> <li> <p> <code>MaxRuntimeExceeded</code> - The job stopped because it exceeded the maximum allowed runtime.</p> </li> <li> <p> <code>MaxWaitTimeExceeded</code> - The job stopped because it exceeded the maximum allowed wait time.</p> </li> <li> <p> <code>Stopped</code> - The training job has stopped.</p> </li> </ul> </dd> <dt>Stopping</dt> <dd> <ul> <li> <p> <code>Stopping</code> - Stopping the training job.</p> </li> </ul> </dd> </dl> <important> <p>Valid values for <code>SecondaryStatus</code> are subject to change. </p> </important> <p>We no longer support the following secondary statuses:</p> <ul> <li> <p> <code>LaunchingMLInstances</code> </p> </li> <li> <p> <code>PreparingTraining</code> </p> </li> <li> <p> <code>DownloadingTrainingImage</code> </p> </li> </ul>",
                     "shape": "SecondaryStatus"
                 },
                 "SecondaryStatusTransitions": {
                     "documentation": "<p>A history of all of the secondary statuses that the training job has transitioned through.</p>",
                     "shape": "SecondaryStatusTransitions"
                 },
                 "StoppingCondition": {
@@ -16471,15 +16687,15 @@
                     "shape": "TrainingTimeInSeconds"
                 },
                 "TuningJobArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the associated hyperparameter tuning job if the training job was launched by a hyperparameter tuning job.</p>",
                     "shape": "HyperParameterTuningJobArn"
                 },
                 "VpcConfig": {
-                    "documentation": "<p>A <a>VpcConfig</a> object that specifies the VPC that this training job has access to. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/train-vpc.html\">Protect Training Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
+                    "documentation": "<p>A <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_VpcConfig.html\">VpcConfig</a> object that specifies the VPC that this training job has access to. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/train-vpc.html\">Protect Training Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
                     "shape": "VpcConfig"
                 },
                 "WarmPoolStatus": {
                     "documentation": "<p>The status of the warm pool associated with the training job.</p>",
                     "shape": "WarmPoolStatus"
                 }
             },
@@ -16873,14 +17089,18 @@
                     "documentation": "<p>The variant's capacity.</p>",
                     "shape": "TaskCount"
                 },
                 "DesiredWeight": {
                     "documentation": "<p>The variant's weight.</p>",
                     "shape": "VariantWeight"
                 },
+                "ServerlessUpdateConfig": {
+                    "documentation": "<p>Specifies the serverless update concurrency configuration for an endpoint variant.</p>",
+                    "shape": "ProductionVariantServerlessUpdateConfig"
+                },
                 "VariantName": {
                     "documentation": "<p>The name of the variant to update.</p>",
                     "shape": "VariantName"
                 }
             },
             "required": [
                 "VariantName"
@@ -17354,15 +17574,15 @@
             "documentation": "<p>A collection of <code>Domain</code> configuration settings to update.</p>",
             "members": {
                 "ExecutionRoleIdentityConfig": {
                     "documentation": "<p>The configuration for attaching a SageMaker user profile name to the execution role as a <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_temp_control-access_monitor.html\">sts:SourceIdentity key</a>. This configuration can only be modified if there are no apps in the <code>InService</code> or <code>Pending</code> state.</p>",
                     "shape": "ExecutionRoleIdentityConfig"
                 },
                 "RStudioServerProDomainSettingsForUpdate": {
-                    "documentation": "<p>A collection of <code>RStudioServerPro</code> Domain-level app settings to update.</p>",
+                    "documentation": "<p>A collection of <code>RStudioServerPro</code> Domain-level app settings to update. A single <code>RStudioServerPro</code> application is created for a domain.</p>",
                     "shape": "RStudioServerProDomainSettingsForUpdate"
                 },
                 "SecurityGroupIds": {
                     "documentation": "<p>The security groups for the Amazon Virtual Private Cloud that the <code>Domain</code> uses for communication between Domain-level apps and user apps.</p>",
                     "shape": "DomainSecurityGroupIds"
                 }
             },
@@ -18093,19 +18313,19 @@
                 "InferenceSpecificationName": {
                     "documentation": "<p>The inference specification name in the model package version.</p>",
                     "shape": "InferenceSpecificationName"
                 },
                 "InstanceType": {
                     "documentation": "<p>The instance types to use for the load test.</p>",
                     "shape": "ProductionVariantInstanceType"
+                },
+                "ServerlessConfig": {
+                    "shape": "ProductionVariantServerlessConfig"
                 }
             },
-            "required": [
-                "InstanceType"
-            ],
             "type": "structure"
         },
         "EndpointInputConfigurations": {
             "max": 10,
             "member": {
                 "shape": "EndpointInputConfiguration"
             },
@@ -18120,15 +18340,15 @@
                     "shape": "EndpointConfigName"
                 },
                 "EndpointName": {
                     "documentation": "<p>The name of the endpoint.</p>",
                     "shape": "EndpointName"
                 },
                 "EndpointStatus": {
-                    "documentation": "<p> The status of the endpoint. For possible values of the status of an endpoint, see <a>EndpointSummary$EndpointStatus</a>. </p>",
+                    "documentation": "<p> The status of the endpoint. For possible values of the status of an endpoint, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_EndpointSummary.html\">EndpointSummary</a>. </p>",
                     "shape": "EndpointStatus"
                 },
                 "FailureReason": {
                     "documentation": "<p> If the status of the endpoint is <code>Failed</code>, or the status is <code>InService</code> but update operation fails, this provides the reason why it failed. </p>",
                     "shape": "FailureReason"
                 }
             },
@@ -18152,30 +18372,31 @@
             "members": {
                 "EndpointName": {
                     "documentation": "<p>The name of the endpoint made during a recommendation job.</p>",
                     "shape": "String"
                 },
                 "InitialInstanceCount": {
                     "documentation": "<p>The number of instances recommended to launch initially.</p>",
-                    "shape": "Integer"
+                    "shape": "InitialInstanceCount"
                 },
                 "InstanceType": {
                     "documentation": "<p>The instance type recommended by Amazon SageMaker Inference Recommender.</p>",
                     "shape": "ProductionVariantInstanceType"
                 },
+                "ServerlessConfig": {
+                    "shape": "ProductionVariantServerlessConfig"
+                },
                 "VariantName": {
                     "documentation": "<p>The name of the production variant (deployed model) made during a recommendation job.</p>",
                     "shape": "String"
                 }
             },
             "required": [
                 "EndpointName",
-                "VariantName",
-                "InstanceType",
-                "InitialInstanceCount"
+                "VariantName"
             ],
             "type": "structure"
         },
         "EndpointPerformance": {
             "documentation": "<p>The performance results from running an Inference Recommender job on an existing endpoint.</p>",
             "members": {
                 "EndpointInfo": {
@@ -18212,15 +18433,16 @@
                 "OutOfService",
                 "Creating",
                 "Updating",
                 "SystemUpdating",
                 "RollingBack",
                 "InService",
                 "Deleting",
-                "Failed"
+                "Failed",
+                "UpdateRollbackFailed"
             ],
             "type": "string"
         },
         "EndpointSummary": {
             "documentation": "<p>Provides summary information for an endpoint.</p>",
             "members": {
                 "CreationTime": {
@@ -18232,15 +18454,15 @@
                     "shape": "EndpointArn"
                 },
                 "EndpointName": {
                     "documentation": "<p>The name of the endpoint.</p>",
                     "shape": "EndpointName"
                 },
                 "EndpointStatus": {
-                    "documentation": "<p>The status of the endpoint.</p> <ul> <li> <p> <code>OutOfService</code>: Endpoint is not available to take incoming requests.</p> </li> <li> <p> <code>Creating</code>: <a>CreateEndpoint</a> is executing.</p> </li> <li> <p> <code>Updating</code>: <a>UpdateEndpoint</a> or <a>UpdateEndpointWeightsAndCapacities</a> is executing.</p> </li> <li> <p> <code>SystemUpdating</code>: Endpoint is undergoing maintenance and cannot be updated or deleted or re-scaled until it has completed. This maintenance operation does not change any customer-specified values such as VPC config, KMS encryption, model, instance type, or instance count.</p> </li> <li> <p> <code>RollingBack</code>: Endpoint fails to scale up or down or change its variant weight and is in the process of rolling back to its previous configuration. Once the rollback completes, endpoint returns to an <code>InService</code> status. This transitional status only applies to an endpoint that has autoscaling enabled and is undergoing variant weight or capacity changes as part of an <a>UpdateEndpointWeightsAndCapacities</a> call or when the <a>UpdateEndpointWeightsAndCapacities</a> operation is called explicitly.</p> </li> <li> <p> <code>InService</code>: Endpoint is available to process incoming requests.</p> </li> <li> <p> <code>Deleting</code>: <a>DeleteEndpoint</a> is executing.</p> </li> <li> <p> <code>Failed</code>: Endpoint could not be created, updated, or re-scaled. Use <a>DescribeEndpointOutput$FailureReason</a> for information about the failure. <a>DeleteEndpoint</a> is the only operation that can be performed on a failed endpoint.</p> </li> </ul> <p>To get a list of endpoints with a specified status, use the <a>ListEndpointsInput$StatusEquals</a> filter.</p>",
+                    "documentation": "<p>The status of the endpoint.</p> <ul> <li> <p> <code>OutOfService</code>: Endpoint is not available to take incoming requests.</p> </li> <li> <p> <code>Creating</code>: <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpoint.html\">CreateEndpoint</a> is executing.</p> </li> <li> <p> <code>Updating</code>: <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateEndpoint.html\">UpdateEndpoint</a> or <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateEndpointWeightsAndCapacities.html\">UpdateEndpointWeightsAndCapacities</a> is executing.</p> </li> <li> <p> <code>SystemUpdating</code>: Endpoint is undergoing maintenance and cannot be updated or deleted or re-scaled until it has completed. This maintenance operation does not change any customer-specified values such as VPC config, KMS encryption, model, instance type, or instance count.</p> </li> <li> <p> <code>RollingBack</code>: Endpoint fails to scale up or down or change its variant weight and is in the process of rolling back to its previous configuration. Once the rollback completes, endpoint returns to an <code>InService</code> status. This transitional status only applies to an endpoint that has autoscaling enabled and is undergoing variant weight or capacity changes as part of an <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateEndpointWeightsAndCapacities.html\">UpdateEndpointWeightsAndCapacities</a> call or when the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateEndpointWeightsAndCapacities.html\">UpdateEndpointWeightsAndCapacities</a> operation is called explicitly.</p> </li> <li> <p> <code>InService</code>: Endpoint is available to process incoming requests.</p> </li> <li> <p> <code>Deleting</code>: <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DeleteEndpoint.html\">DeleteEndpoint</a> is executing.</p> </li> <li> <p> <code>Failed</code>: Endpoint could not be created, updated, or re-scaled. Use <code>DescribeEndpointOutput$FailureReason</code> for information about the failure. <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DeleteEndpoint.html\">DeleteEndpoint</a> is the only operation that can be performed on a failed endpoint.</p> </li> </ul> <p>To get a list of endpoints with a specified status, use the <code>StatusEquals</code> filter with a call to <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ListEndpoints.html\">ListEndpoints</a>.</p>",
                     "shape": "EndpointStatus"
                 },
                 "LastModifiedTime": {
                     "documentation": "<p>A timestamp that shows when the endpoint was last modified.</p>",
                     "shape": "Timestamp"
                 }
             },
@@ -18359,15 +18581,15 @@
         },
         "ExitMessage": {
             "max": 1024,
             "pattern": "[\\S\\s]*",
             "type": "string"
         },
         "Experiment": {
-            "documentation": "<p>The properties of an experiment as returned by the <a>Search</a> API.</p>",
+            "documentation": "<p>The properties of an experiment as returned by the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API.</p>",
             "members": {
                 "CreatedBy": {
                     "documentation": "<p>Who created the experiment.</p>",
                     "shape": "UserContext"
                 },
                 "CreationTime": {
                     "documentation": "<p>When the experiment was created.</p>",
@@ -18396,27 +18618,27 @@
                     "documentation": "<p>When the experiment was last modified.</p>",
                     "shape": "Timestamp"
                 },
                 "Source": {
                     "shape": "ExperimentSource"
                 },
                 "Tags": {
-                    "documentation": "<p>The list of tags that are associated with the experiment. You can use <a>Search</a> API to search on the tags.</p>",
+                    "documentation": "<p>The list of tags that are associated with the experiment. You can use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API to search on the tags.</p>",
                     "shape": "TagList"
                 }
             },
             "type": "structure"
         },
         "ExperimentArn": {
             "max": 256,
             "pattern": "arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:experiment/.*",
             "type": "string"
         },
         "ExperimentConfig": {
-            "documentation": "<p>Associates a SageMaker job as a trial component with an experiment and trial. Specified when you call the following APIs:</p> <ul> <li> <p> <a>CreateProcessingJob</a> </p> </li> <li> <p> <a>CreateTrainingJob</a> </p> </li> <li> <p> <a>CreateTransformJob</a> </p> </li> </ul>",
+            "documentation": "<p>Associates a SageMaker job as a trial component with an experiment and trial. Specified when you call the following APIs:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateProcessingJob.html\">CreateProcessingJob</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateTrainingJob.html\">CreateTrainingJob</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateTransformJob.html\">CreateTransformJob</a> </p> </li> </ul>",
             "members": {
                 "ExperimentName": {
                     "documentation": "<p>The name of an existing experiment to associate with the trial component.</p>",
                     "shape": "ExperimentEntityName"
                 },
                 "RunName": {
                     "documentation": "<p>The name of the experiment run to associate with the trial component.</p>",
@@ -18475,15 +18697,15 @@
         "ExperimentSummaries": {
             "member": {
                 "shape": "ExperimentSummary"
             },
             "type": "list"
         },
         "ExperimentSummary": {
-            "documentation": "<p>A summary of the properties of an experiment. To get the complete set of properties, call the <a>DescribeExperiment</a> API and provide the <code>ExperimentName</code>.</p>",
+            "documentation": "<p>A summary of the properties of an experiment. To get the complete set of properties, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeExperiment.html\">DescribeExperiment</a> API and provide the <code>ExperimentName</code>.</p>",
             "members": {
                 "CreationTime": {
                     "documentation": "<p>When the experiment was created.</p>",
                     "shape": "Timestamp"
                 },
                 "DisplayName": {
                     "documentation": "<p>The name of the experiment as displayed. If <code>DisplayName</code> isn't specified, <code>ExperimentName</code> is displayed.</p>",
@@ -18935,19 +19157,60 @@
         "FileSystemType": {
             "enum": [
                 "EFS",
                 "FSxLustre"
             ],
             "type": "string"
         },
+        "FillingTransformationMap": {
+            "key": {
+                "shape": "FillingType"
+            },
+            "max": 6,
+            "min": 1,
+            "type": "map",
+            "value": {
+                "shape": "FillingTransformationValue"
+            }
+        },
+        "FillingTransformationValue": {
+            "max": 256,
+            "min": 1,
+            "pattern": "^[a-zA-Z0-9\\_\\-]+$",
+            "type": "string"
+        },
+        "FillingTransformations": {
+            "key": {
+                "shape": "TransformationAttributeName"
+            },
+            "max": 50,
+            "min": 1,
+            "type": "map",
+            "value": {
+                "shape": "FillingTransformationMap"
+            }
+        },
+        "FillingType": {
+            "enum": [
+                "frontfill",
+                "middlefill",
+                "backfill",
+                "futurefill",
+                "frontfill_value",
+                "middlefill_value",
+                "backfill_value",
+                "futurefill_value"
+            ],
+            "type": "string"
+        },
         "Filter": {
-            "documentation": "<p>A conditional statement for a search expression that includes a resource property, a Boolean operator, and a value. Resources that match the statement are returned in the results from the <a>Search</a> API.</p> <p>If you specify a <code>Value</code>, but not an <code>Operator</code>, SageMaker uses the equals operator.</p> <p>In search, there are several property types:</p> <dl> <dt>Metrics</dt> <dd> <p>To define a metric filter, enter a value using the form <code>\"Metrics.&lt;name&gt;\"</code>, where <code>&lt;name&gt;</code> is a metric name. For example, the following filter searches for training jobs with an <code>\"accuracy\"</code> metric greater than <code>\"0.9\"</code>:</p> <p> <code>{</code> </p> <p> <code>\"Name\": \"Metrics.accuracy\",</code> </p> <p> <code>\"Operator\": \"GreaterThan\",</code> </p> <p> <code>\"Value\": \"0.9\"</code> </p> <p> <code>}</code> </p> </dd> <dt>HyperParameters</dt> <dd> <p>To define a hyperparameter filter, enter a value with the form <code>\"HyperParameters.&lt;name&gt;\"</code>. Decimal hyperparameter values are treated as a decimal in a comparison if the specified <code>Value</code> is also a decimal value. If the specified <code>Value</code> is an integer, the decimal hyperparameter values are treated as integers. For example, the following filter is satisfied by training jobs with a <code>\"learning_rate\"</code> hyperparameter that is less than <code>\"0.5\"</code>:</p> <p> <code> {</code> </p> <p> <code> \"Name\": \"HyperParameters.learning_rate\",</code> </p> <p> <code> \"Operator\": \"LessThan\",</code> </p> <p> <code> \"Value\": \"0.5\"</code> </p> <p> <code> }</code> </p> </dd> <dt>Tags</dt> <dd> <p>To define a tag filter, enter a value with the form <code>Tags.&lt;key&gt;</code>.</p> </dd> </dl>",
+            "documentation": "<p>A conditional statement for a search expression that includes a resource property, a Boolean operator, and a value. Resources that match the statement are returned in the results from the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API.</p> <p>If you specify a <code>Value</code>, but not an <code>Operator</code>, SageMaker uses the equals operator.</p> <p>In search, there are several property types:</p> <dl> <dt>Metrics</dt> <dd> <p>To define a metric filter, enter a value using the form <code>\"Metrics.&lt;name&gt;\"</code>, where <code>&lt;name&gt;</code> is a metric name. For example, the following filter searches for training jobs with an <code>\"accuracy\"</code> metric greater than <code>\"0.9\"</code>:</p> <p> <code>{</code> </p> <p> <code>\"Name\": \"Metrics.accuracy\",</code> </p> <p> <code>\"Operator\": \"GreaterThan\",</code> </p> <p> <code>\"Value\": \"0.9\"</code> </p> <p> <code>}</code> </p> </dd> <dt>HyperParameters</dt> <dd> <p>To define a hyperparameter filter, enter a value with the form <code>\"HyperParameters.&lt;name&gt;\"</code>. Decimal hyperparameter values are treated as a decimal in a comparison if the specified <code>Value</code> is also a decimal value. If the specified <code>Value</code> is an integer, the decimal hyperparameter values are treated as integers. For example, the following filter is satisfied by training jobs with a <code>\"learning_rate\"</code> hyperparameter that is less than <code>\"0.5\"</code>:</p> <p> <code> {</code> </p> <p> <code> \"Name\": \"HyperParameters.learning_rate\",</code> </p> <p> <code> \"Operator\": \"LessThan\",</code> </p> <p> <code> \"Value\": \"0.5\"</code> </p> <p> <code> }</code> </p> </dd> <dt>Tags</dt> <dd> <p>To define a tag filter, enter a value with the form <code>Tags.&lt;key&gt;</code>.</p> </dd> </dl>",
             "members": {
                 "Name": {
-                    "documentation": "<p>A resource property name. For example, <code>TrainingJobName</code>. For valid property names, see <a>SearchRecord</a>. You must specify a valid property for the resource.</p>",
+                    "documentation": "<p>A resource property name. For example, <code>TrainingJobName</code>. For valid property names, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_SearchRecord.html\">SearchRecord</a>. You must specify a valid property for the resource.</p>",
                     "shape": "ResourcePropertyName"
                 },
                 "Operator": {
                     "documentation": "<p>A Boolean binary operator that is used to evaluate the filter. The operator field contains one of the following values:</p> <dl> <dt>Equals</dt> <dd> <p>The value of <code>Name</code> equals <code>Value</code>.</p> </dd> <dt>NotEquals</dt> <dd> <p>The value of <code>Name</code> doesn't equal <code>Value</code>.</p> </dd> <dt>Exists</dt> <dd> <p>The <code>Name</code> property exists.</p> </dd> <dt>NotExists</dt> <dd> <p>The <code>Name</code> property does not exist.</p> </dd> <dt>GreaterThan</dt> <dd> <p>The value of <code>Name</code> is greater than <code>Value</code>. Not supported for text properties.</p> </dd> <dt>GreaterThanOrEqualTo</dt> <dd> <p>The value of <code>Name</code> is greater than or equal to <code>Value</code>. Not supported for text properties.</p> </dd> <dt>LessThan</dt> <dd> <p>The value of <code>Name</code> is less than <code>Value</code>. Not supported for text properties.</p> </dd> <dt>LessThanOrEqualTo</dt> <dd> <p>The value of <code>Name</code> is less than or equal to <code>Value</code>. Not supported for text properties.</p> </dd> <dt>In</dt> <dd> <p>The value of <code>Name</code> is one of the comma delimited strings in <code>Value</code>. Only supported for text properties.</p> </dd> <dt>Contains</dt> <dd> <p>The value of <code>Name</code> contains the string <code>Value</code>. Only supported for text properties.</p> <p>A <code>SearchExpression</code> can include the <code>Contains</code> operator multiple times when the value of <code>Name</code> is one of the following:</p> <ul> <li> <p> <code>Experiment.DisplayName</code> </p> </li> <li> <p> <code>Experiment.ExperimentName</code> </p> </li> <li> <p> <code>Experiment.Tags</code> </p> </li> <li> <p> <code>Trial.DisplayName</code> </p> </li> <li> <p> <code>Trial.TrialName</code> </p> </li> <li> <p> <code>Trial.Tags</code> </p> </li> <li> <p> <code>TrialComponent.DisplayName</code> </p> </li> <li> <p> <code>TrialComponent.TrialComponentName</code> </p> </li> <li> <p> <code>TrialComponent.Tags</code> </p> </li> <li> <p> <code>TrialComponent.InputArtifacts</code> </p> </li> <li> <p> <code>TrialComponent.OutputArtifacts</code> </p> </li> </ul> <p>A <code>SearchExpression</code> can include only one <code>Contains</code> operator for all other values of <code>Name</code>. In these cases, if you include multiple <code>Contains</code> operators in the <code>SearchExpression</code>, the result is the following error message: \"<code>'CONTAINS' operator usage limit of 1 exceeded.</code>\"</p> </dd> </dl>",
                     "shape": "Operator"
                 },
                 "Value": {
@@ -18974,15 +19237,15 @@
             "pattern": ".+",
             "type": "string"
         },
         "FinalAutoMLJobObjectiveMetric": {
             "documentation": "<p>The best candidate result from an AutoML training job.</p>",
             "members": {
                 "MetricName": {
-                    "documentation": "<p>The name of the metric with the best result. For a description of the possible objective metrics, see <a>AutoMLJobObjective$MetricName</a>.</p>",
+                    "documentation": "<p>The name of the metric with the best result. For a description of the possible objective metrics, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AutoMLJobObjective.html\">AutoMLJobObjective$MetricName</a>.</p>",
                     "shape": "AutoMLMetricEnum"
                 },
                 "StandardMetricName": {
                     "documentation": "<p>The name of the standard metric. For a description of the standard metrics, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-metrics-validation.html#autopilot-metrics\">Autopilot candidate metrics</a>.</p>",
                     "shape": "AutoMLMetricEnum"
                 },
                 "Type": {
@@ -18997,15 +19260,15 @@
             "required": [
                 "MetricName",
                 "Value"
             ],
             "type": "structure"
         },
         "FinalHyperParameterTuningJobObjectiveMetric": {
-            "documentation": "<p>Shows the latest objective metric emitted by a training job that was launched by a hyperparameter tuning job. You define the objective metric in the <code>HyperParameterTuningJobObjective</code> parameter of <a>HyperParameterTuningJobConfig</a>.</p>",
+            "documentation": "<p>Shows the latest objective metric emitted by a training job that was launched by a hyperparameter tuning job. You define the objective metric in the <code>HyperParameterTuningJobObjective</code> parameter of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobConfig.html\">HyperParameterTuningJobConfig</a>.</p>",
             "members": {
                 "MetricName": {
                     "documentation": "<p>The name of the objective metric. For SageMaker built-in algorithms, metrics are defined per algorithm. See the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/xgboost-tuning.html\">metrics for XGBoost</a> as an example. You can also use a custom algorithm for training and define your own metrics. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-define-metrics-variables.html\">Define metrics and environment variables</a>.</p>",
                     "shape": "MetricName"
                 },
                 "Type": {
                     "documentation": "<p>Select if you want to minimize or maximize the objective metric during hyperparameter tuning. </p>",
@@ -19145,14 +19408,38 @@
         },
         "FlowDefinitionTaskTitle": {
             "max": 128,
             "min": 1,
             "pattern": "^[\\t\\n\\r -\\uD7FF\\uE000-\\uFFFD]*$",
             "type": "string"
         },
+        "ForecastFrequency": {
+            "max": 5,
+            "min": 1,
+            "pattern": "^1Y|Y|([1-9]|1[0-1])M|M|[1-4]W|W|[1-6]D|D|([1-9]|1[0-9]|2[0-3])H|H|([1-9]|[1-5][0-9])min$",
+            "type": "string"
+        },
+        "ForecastHorizon": {
+            "min": 1,
+            "type": "integer"
+        },
+        "ForecastQuantile": {
+            "max": 4,
+            "min": 2,
+            "pattern": "(^p[1-9]\\d?$)",
+            "type": "string"
+        },
+        "ForecastQuantiles": {
+            "max": 5,
+            "member": {
+                "shape": "ForecastQuantile"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "Framework": {
             "enum": [
                 "TENSORFLOW",
                 "KERAS",
                 "MXNET",
                 "ONNX",
                 "PYTORCH",
@@ -19349,14 +19636,27 @@
         },
         "Group": {
             "max": 63,
             "min": 1,
             "pattern": "[\\p{L}\\p{M}\\p{S}\\p{N}\\p{P}]+",
             "type": "string"
         },
+        "GroupingAttributeName": {
+            "max": 256,
+            "min": 1,
+            "type": "string"
+        },
+        "GroupingAttributeNames": {
+            "max": 5,
+            "member": {
+                "shape": "GroupingAttributeName"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "Groups": {
             "max": 10,
             "member": {
                 "shape": "Group"
             },
             "min": 1,
             "type": "list"
@@ -19640,15 +19940,15 @@
             "type": "string"
         },
         "HumanLoopActivationConditions": {
             "max": 10240,
             "type": "string"
         },
         "HumanLoopActivationConditionsConfig": {
-            "documentation": "<p>Defines under what conditions SageMaker creates a human loop. Used within . See for the required format of activation conditions.</p>",
+            "documentation": "<p>Defines under what conditions SageMaker creates a human loop. Used within <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateFlowDefinition.html\">CreateFlowDefinition</a>. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HumanLoopActivationConditionsConfig.html\">HumanLoopActivationConditionsConfig</a> for the required format of activation conditions.</p>",
             "members": {
                 "HumanLoopActivationConditions": {
                     "documentation": "<p>JSON expressing use-case specific conditions declaratively. If any condition is matched, atomic tasks are created against the configured work team. The set of conditions is different for Rekognition and Textract. For more information about how to structure the JSON, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/a2i-human-fallback-conditions-json-schema.html\">JSON Schema for Human Loop Activation Conditions in Amazon Augmented AI</a> in the <i>Amazon SageMaker Developer Guide</i>.</p>",
                     "jsonvalue": true,
                     "shape": "HumanLoopActivationConditions"
                 }
             },
@@ -19846,15 +20146,15 @@
             "documentation": "<p>Specifies which training algorithm to use for training jobs that a hyperparameter tuning job launches and the metrics to monitor.</p>",
             "members": {
                 "AlgorithmName": {
                     "documentation": "<p>The name of the resource algorithm to use for the hyperparameter tuning job. If you specify a value for this parameter, do not specify a value for <code>TrainingImage</code>.</p>",
                     "shape": "ArnOrName"
                 },
                 "MetricDefinitions": {
-                    "documentation": "<p>An array of <a>MetricDefinition</a> objects that specify the metrics that the algorithm emits.</p>",
+                    "documentation": "<p>An array of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_MetricDefinition.html\">MetricDefinition</a> objects that specify the metrics that the algorithm emits.</p>",
                     "shape": "MetricDefinitionList"
                 },
                 "TrainingImage": {
                     "documentation": "<p> The registry path of the Docker image that contains the training algorithm. For information about Docker registry paths for built-in algorithms, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-algo-docker-registry-paths.html\">Algorithms Provided by Amazon SageMaker: Common Parameters</a>. SageMaker supports both <code>registry/repository[:tag]</code> and <code>registry/repository[@digest]</code> image path formats. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/your-algorithms.html\">Using Your Own Algorithms with Amazon SageMaker</a>.</p>",
                     "shape": "AlgorithmImage"
                 },
                 "TrainingInputMode": {
@@ -19926,15 +20226,15 @@
             "min": 0,
             "type": "list"
         },
         "HyperParameterTrainingJobDefinition": {
             "documentation": "<p>Defines the training jobs launched by a hyperparameter tuning job.</p>",
             "members": {
                 "AlgorithmSpecification": {
-                    "documentation": "<p>The <a>HyperParameterAlgorithmSpecification</a> object that specifies the resource algorithm to use for the training jobs that the tuning job launches.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterAlgorithmSpecification.html\">HyperParameterAlgorithmSpecification</a> object that specifies the resource algorithm to use for the training jobs that the tuning job launches.</p>",
                     "shape": "HyperParameterAlgorithmSpecification"
                 },
                 "CheckpointConfig": {
                     "shape": "CheckpointConfig"
                 },
                 "DefinitionName": {
                     "documentation": "<p>The job definition name.</p>",
@@ -19949,26 +20249,26 @@
                     "shape": "Boolean"
                 },
                 "EnableNetworkIsolation": {
                     "documentation": "<p>Isolates the training container. No inbound or outbound network calls can be made, except for calls between peers within a training cluster for distributed training. If network isolation is used for training jobs that are configured to use a VPC, SageMaker downloads and uploads customer data and model artifacts through the specified VPC, but the training container does not have network access.</p>",
                     "shape": "Boolean"
                 },
                 "Environment": {
-                    "documentation": "<p>An environment variable that you can pass into the SageMaker <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateTrainingJob.html\">CreateTrainingJob</a> API. You can use an existing <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateTrainingJob.html#sagemaker-CreateTrainingJob-request-Environment\">environment variable from the training container</a> or use your own. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-define-metrics.html\">Define metrics and variables</a> for more information.</p> <note> <p>The maximum number of items specified for <code>Map Entries</code> refers to the maximum number of environment variables for each <code>TrainingJobDefinition</code> and also the maximum for the hyperparameter tuning job itself. That is, the sum of the number of environment variables for all the training job definitions can't exceed the maximum number specified.</p> </note>",
+                    "documentation": "<p>An environment variable that you can pass into the SageMaker <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateTrainingJob.html\">CreateTrainingJob</a> API. You can use an existing <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateTrainingJob.html#sagemaker-CreateTrainingJob-request-Environment\">environment variable from the training container</a> or use your own. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-define-metrics-variables.html\">Define metrics and variables</a> for more information.</p> <note> <p>The maximum number of items specified for <code>Map Entries</code> refers to the maximum number of environment variables for each <code>TrainingJobDefinition</code> and also the maximum for the hyperparameter tuning job itself. That is, the sum of the number of environment variables for all the training job definitions can't exceed the maximum number specified.</p> </note>",
                     "shape": "HyperParameterTrainingJobEnvironmentMap"
                 },
                 "HyperParameterRanges": {
                     "shape": "ParameterRanges"
                 },
                 "HyperParameterTuningResourceConfig": {
                     "documentation": "<p>The configuration for the hyperparameter tuning resources, including the compute instances and storage volumes, used for training jobs launched by the tuning job. By default, storage volumes hold model artifacts and incremental states. Choose <code>File</code> for <code>TrainingInputMode</code> in the <code>AlgorithmSpecification</code> parameter to additionally store training data in the storage volume (optional).</p>",
                     "shape": "HyperParameterTuningResourceConfig"
                 },
                 "InputDataConfig": {
-                    "documentation": "<p>An array of <a>Channel</a> objects that specify the input for the training jobs that the tuning job launches.</p>",
+                    "documentation": "<p>An array of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Channel.html\">Channel</a> objects that specify the input for the training jobs that the tuning job launches.</p>",
                     "shape": "InputDataConfig"
                 },
                 "OutputDataConfig": {
                     "documentation": "<p>Specifies the path to the Amazon S3 bucket where you store model artifacts from the training jobs that the tuning job launches.</p>",
                     "shape": "OutputDataConfig"
                 },
                 "ResourceConfig": {
@@ -19991,15 +20291,15 @@
                     "documentation": "<p>Specifies a limit to how long a model hyperparameter training job can run. It also specifies how long a managed spot training job has to complete. When the job reaches the time limit, SageMaker ends the training job. Use this API to cap model training costs.</p>",
                     "shape": "StoppingCondition"
                 },
                 "TuningObjective": {
                     "shape": "HyperParameterTuningJobObjective"
                 },
                 "VpcConfig": {
-                    "documentation": "<p>The <a>VpcConfig</a> object that specifies the VPC that you want the training jobs that this hyperparameter tuning job launches to connect to. Control access to and from your training container by configuring the VPC. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/train-vpc.html\">Protect Training Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_VpcConfig.html\">VpcConfig</a> object that specifies the VPC that you want the training jobs that this hyperparameter tuning job launches to connect to. Control access to and from your training container by configuring the VPC. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/train-vpc.html\">Protect Training Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
                     "shape": "VpcConfig"
                 }
             },
             "required": [
                 "AlgorithmSpecification",
                 "RoleArn",
                 "OutputDataConfig",
@@ -20055,15 +20355,15 @@
                     "shape": "Timestamp"
                 },
                 "FailureReason": {
                     "documentation": "<p>The reason that the training job failed. </p>",
                     "shape": "FailureReason"
                 },
                 "FinalHyperParameterTuningJobObjectiveMetric": {
-                    "documentation": "<p>The <a>FinalHyperParameterTuningJobObjectiveMetric</a> object that specifies the value of the objective metric of the tuning job that launched this training job.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_FinalHyperParameterTuningJobObjectiveMetric.html\">FinalHyperParameterTuningJobObjectiveMetric</a> object that specifies the value of the objective metric of the tuning job that launched this training job.</p>",
                     "shape": "FinalHyperParameterTuningJobObjectiveMetric"
                 },
                 "ObjectiveStatus": {
                     "documentation": "<p>The status of the objective metric for the training job:</p> <ul> <li> <p>Succeeded: The final objective metric for the training job was evaluated by the hyperparameter tuning job and used in the hyperparameter tuning process.</p> </li> </ul> <ul> <li> <p>Pending: The training job is in progress and evaluation of its final objective metric is pending.</p> </li> </ul> <ul> <li> <p>Failed: The final objective metric for the training job was not evaluated, and was not used in the hyperparameter tuning process. This typically occurs when the training job failed or did not emit an objective metric.</p> </li> </ul>",
                     "shape": "ObjectiveStatus"
                 },
                 "TrainingEndTime": {
@@ -20114,15 +20414,15 @@
             ],
             "type": "string"
         },
         "HyperParameterTuningInstanceConfig": {
             "documentation": "<p>The configuration for hyperparameter tuning resources for use in training jobs launched by the tuning job. These resources include compute instances and storage volumes. Specify one or more compute instance configurations and allocation strategies to select resources (optional).</p>",
             "members": {
                 "InstanceCount": {
-                    "documentation": "<p>The number of instances of the type specified by <code>InstanceType</code>. Choose an instance count larger than 1 for distributed training algorithms. See <a href=\"https://docs.aws.amazon.com/data-parallel-use-api.html\">SageMaker distributed training jobs</a> for more information.</p>",
+                    "documentation": "<p>The number of instances of the type specified by <code>InstanceType</code>. Choose an instance count larger than 1 for distributed training algorithms. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/data-parallel-use-api.html\">Step 2: Launch a SageMaker Distributed Training Job Using the SageMaker Python SDK</a> for more information.</p>",
                     "shape": "TrainingInstanceCount"
                 },
                 "InstanceType": {
                     "documentation": "<p>The instance type used for processing of hyperparameter optimization jobs. Choose from general purpose (no GPUs) instance types: ml.m5.xlarge, ml.m5.2xlarge, and ml.m5.4xlarge or compute optimized (no GPUs) instance types: ml.c5.xlarge and ml.c5.2xlarge. For more information about instance types, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-available-instance-types.html\">instance type descriptions</a>.</p>",
                     "shape": "TrainingInstanceType"
                 },
                 "VolumeSizeInGB": {
@@ -20164,27 +20464,27 @@
             },
             "type": "structure"
         },
         "HyperParameterTuningJobConfig": {
             "documentation": "<p>Configures a hyperparameter tuning job.</p>",
             "members": {
                 "HyperParameterTuningJobObjective": {
-                    "documentation": "<p>The <a>HyperParameterTuningJobObjective</a> specifies the objective metric used to evaluate the performance of training jobs launched by this tuning job.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobObjective.html\">HyperParameterTuningJobObjective</a> specifies the objective metric used to evaluate the performance of training jobs launched by this tuning job.</p>",
                     "shape": "HyperParameterTuningJobObjective"
                 },
                 "ParameterRanges": {
-                    "documentation": "<p>The <a>ParameterRanges</a> object that specifies the ranges of hyperparameters that this tuning job searches over to find the optimal configuration for the highest model performance against your chosen objective metric. </p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ParameterRanges.html\">ParameterRanges</a> object that specifies the ranges of hyperparameters that this tuning job searches over to find the optimal configuration for the highest model performance against your chosen objective metric. </p>",
                     "shape": "ParameterRanges"
                 },
                 "RandomSeed": {
                     "documentation": "<p>A value used to initialize a pseudo-random number generator. Setting a random seed and using the same seed later for the same tuning job will allow hyperparameter optimization to find more a consistent hyperparameter configuration between the two runs.</p>",
                     "shape": "RandomSeed"
                 },
                 "ResourceLimits": {
-                    "documentation": "<p>The <a>ResourceLimits</a> object that specifies the maximum number of training and parallel training jobs that can be used for this hyperparameter tuning job.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ResourceLimits.html\">ResourceLimits</a> object that specifies the maximum number of training and parallel training jobs that can be used for this hyperparameter tuning job.</p>",
                     "shape": "ResourceLimits"
                 },
                 "Strategy": {
                     "documentation": "<p>Specifies how hyperparameter tuning chooses the combinations of hyperparameter values to use for the training job it launches. For information about search strategies, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-how-it-works.html\">How Hyperparameter Tuning Works</a>.</p>",
                     "shape": "HyperParameterTuningJobStrategyType"
                 },
                 "StrategyConfig": {
@@ -20392,27 +20692,27 @@
                     "shape": "HyperParameterTuningJobStatus"
                 },
                 "LastModifiedTime": {
                     "documentation": "<p>The date and time that the tuning job was modified.</p>",
                     "shape": "Timestamp"
                 },
                 "ObjectiveStatusCounters": {
-                    "documentation": "<p>The <a>ObjectiveStatusCounters</a> object that specifies the numbers of training jobs, categorized by objective metric status, that this tuning job launched.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ObjectiveStatusCounters.html\">ObjectiveStatusCounters</a> object that specifies the numbers of training jobs, categorized by objective metric status, that this tuning job launched.</p>",
                     "shape": "ObjectiveStatusCounters"
                 },
                 "ResourceLimits": {
-                    "documentation": "<p>The <a>ResourceLimits</a> object that specifies the maximum number of training jobs and parallel training jobs allowed for this tuning job.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ResourceLimits.html\">ResourceLimits</a> object that specifies the maximum number of training jobs and parallel training jobs allowed for this tuning job.</p>",
                     "shape": "ResourceLimits"
                 },
                 "Strategy": {
                     "documentation": "<p>Specifies the search strategy hyperparameter tuning uses to choose which hyperparameters to evaluate at each iteration.</p>",
                     "shape": "HyperParameterTuningJobStrategyType"
                 },
                 "TrainingJobStatusCounters": {
-                    "documentation": "<p>The <a>TrainingJobStatusCounters</a> object that specifies the numbers of training jobs, categorized by status, that this tuning job launched.</p>",
+                    "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_TrainingJobStatusCounters.html\">TrainingJobStatusCounters</a> object that specifies the numbers of training jobs, categorized by status, that this tuning job launched.</p>",
                     "shape": "TrainingJobStatusCounters"
                 }
             },
             "required": [
                 "HyperParameterTuningJobName",
                 "HyperParameterTuningJobArn",
                 "HyperParameterTuningJobStatus",
@@ -20465,15 +20765,15 @@
                     "shape": "HyperParameterTuningInstanceConfigs"
                 },
                 "InstanceCount": {
                     "documentation": "<p>The number of compute instances of type <code>InstanceType</code> to use. For <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/data-parallel-use-api.html\">distributed training</a>, select a value greater than 1.</p>",
                     "shape": "TrainingInstanceCount"
                 },
                 "InstanceType": {
-                    "documentation": "<p>The instance type used to run hyperparameter optimization tuning jobs. See <a href=\"https://docs.aws.amazon.com/notebooks-available-instance-types.html\"> descriptions of instance types</a> for more information.</p>",
+                    "documentation": "<p>The instance type used to run hyperparameter optimization tuning jobs. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/notebooks-available-instance-types.html\"> descriptions of instance types</a> for more information.</p>",
                     "shape": "TrainingInstanceType"
                 },
                 "VolumeKmsKeyId": {
                     "documentation": "<p>A key used by Amazon Web Services Key Management Service to encrypt data on the storage volume attached to the compute instances used to run the training job. You can use either of the following formats to specify a key.</p> <p>KMS Key ID:</p> <p> <code>\"1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> <p>Amazon Resource Name (ARN) of a KMS key:</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> <p>Some instances use local storage, which use a <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ssd-instance-store.html\">hardware module to encrypt</a> storage volumes. If you choose one of these instance types, you cannot request a <code>VolumeKmsKeyId</code>. For a list of instance types that use local storage, see <a href=\"http://aws.amazon.com/releasenotes/host-instance-storage-volumes-table/\">instance store volumes</a>. For more information about Amazon Web Services Key Management Service, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/sms-security-kms-permissions.html\">KMS encryption</a> for more information.</p>",
                     "shape": "KmsKeyId"
                 },
                 "VolumeSizeInGB": {
@@ -20597,15 +20897,15 @@
         "ImageBaseImage": {
             "max": 255,
             "min": 1,
             "pattern": ".*",
             "type": "string"
         },
         "ImageClassificationJobConfig": {
-            "documentation": "<p>Stores the configuration information for the image classification problem of an AutoML job using the V2 API.</p>",
+            "documentation": "<p>Stores the configuration information for the image classification problem of an AutoML job V2.</p>",
             "members": {
                 "CompletionCriteria": {
                     "documentation": "<p>How long a job is allowed to run, or how many candidates a job is allowed to generate.</p>",
                     "shape": "AutoMLJobCompletionCriteria"
                 }
             },
             "type": "structure"
@@ -21051,14 +21351,22 @@
         "InferenceRecommendation": {
             "documentation": "<p>A list of recommendations made by Amazon SageMaker Inference Recommender.</p>",
             "members": {
                 "EndpointConfiguration": {
                     "documentation": "<p>Defines the endpoint configuration parameters.</p>",
                     "shape": "EndpointOutputConfiguration"
                 },
+                "InvocationEndTime": {
+                    "documentation": "<p>A timestamp that shows when the benchmark completed.</p>",
+                    "shape": "InvocationEndTime"
+                },
+                "InvocationStartTime": {
+                    "documentation": "<p>A timestamp that shows when the benchmark started.</p>",
+                    "shape": "InvocationStartTime"
+                },
                 "Metrics": {
                     "documentation": "<p>The metrics used to decide what recommendation to make.</p>",
                     "shape": "RecommendationMetrics"
                 },
                 "ModelConfiguration": {
                     "documentation": "<p>Defines the model configuration.</p>",
                     "shape": "ModelConfiguration"
@@ -21114,18 +21422,30 @@
                     "documentation": "<p>The recommendation job type.</p>",
                     "shape": "RecommendationJobType"
                 },
                 "LastModifiedTime": {
                     "documentation": "<p>A timestamp that shows when the job was last modified.</p>",
                     "shape": "LastModifiedTime"
                 },
+                "ModelName": {
+                    "documentation": "<p>The name of the created model.</p>",
+                    "shape": "ModelName"
+                },
+                "ModelPackageVersionArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of a versioned model package.</p>",
+                    "shape": "ModelPackageArn"
+                },
                 "RoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of an IAM role that enables Amazon SageMaker to perform tasks on your behalf.</p>",
                     "shape": "RoleArn"
                 },
+                "SamplePayloadUrl": {
+                    "documentation": "<p>The Amazon Simple Storage Service (Amazon S3) path where the sample payload is stored. This path must point to a single gzip compressed tar archive (.tar.gz suffix).</p>",
+                    "shape": "S3Uri"
+                },
                 "Status": {
                     "documentation": "<p>The status of the job.</p>",
                     "shape": "RecommendationJobStatus"
                 }
             },
             "required": [
                 "JobName",
@@ -21211,27 +21531,31 @@
         },
         "InferenceSpecificationName": {
             "max": 63,
             "min": 1,
             "pattern": "^[a-zA-Z0-9](-*[a-zA-Z0-9]){0,62}$",
             "type": "string"
         },
+        "InitialInstanceCount": {
+            "min": 1,
+            "type": "integer"
+        },
         "InitialNumberOfUsers": {
             "min": 1,
             "type": "integer"
         },
         "InitialTaskCount": {
             "min": 1,
             "type": "integer"
         },
         "InputConfig": {
             "documentation": "<p>Contains information about the location of input model artifacts, the name and shape of the expected data inputs, and the framework in which the model was trained.</p>",
             "members": {
                 "DataInputConfig": {
-                    "documentation": "<p>Specifies the name and shape of the expected data inputs for your trained model with a JSON dictionary form. The data inputs are <a>InputConfig$Framework</a> specific. </p> <ul> <li> <p> <code>TensorFlow</code>: You must specify the name and shape (NHWC format) of the expected data inputs using a dictionary format for your trained model. The dictionary formats required for the console and CLI are different.</p> <ul> <li> <p>Examples for one input:</p> <ul> <li> <p>If using the console, <code>{\"input\":[1,1024,1024,3]}</code> </p> </li> <li> <p>If using the CLI, <code>{\\\"input\\\":[1,1024,1024,3]}</code> </p> </li> </ul> </li> <li> <p>Examples for two inputs:</p> <ul> <li> <p>If using the console, <code>{\"data1\": [1,28,28,1], \"data2\":[1,28,28,1]}</code> </p> </li> <li> <p>If using the CLI, <code>{\\\"data1\\\": [1,28,28,1], \\\"data2\\\":[1,28,28,1]}</code> </p> </li> </ul> </li> </ul> </li> <li> <p> <code>KERAS</code>: You must specify the name and shape (NCHW format) of expected data inputs using a dictionary format for your trained model. Note that while Keras model artifacts should be uploaded in NHWC (channel-last) format, <code>DataInputConfig</code> should be specified in NCHW (channel-first) format. The dictionary formats required for the console and CLI are different.</p> <ul> <li> <p>Examples for one input:</p> <ul> <li> <p>If using the console, <code>{\"input_1\":[1,3,224,224]}</code> </p> </li> <li> <p>If using the CLI, <code>{\\\"input_1\\\":[1,3,224,224]}</code> </p> </li> </ul> </li> <li> <p>Examples for two inputs:</p> <ul> <li> <p>If using the console, <code>{\"input_1\": [1,3,224,224], \"input_2\":[1,3,224,224]} </code> </p> </li> <li> <p>If using the CLI, <code>{\\\"input_1\\\": [1,3,224,224], \\\"input_2\\\":[1,3,224,224]}</code> </p> </li> </ul> </li> </ul> </li> <li> <p> <code>MXNET/ONNX/DARKNET</code>: You must specify the name and shape (NCHW format) of the expected data inputs in order using a dictionary format for your trained model. The dictionary formats required for the console and CLI are different.</p> <ul> <li> <p>Examples for one input:</p> <ul> <li> <p>If using the console, <code>{\"data\":[1,3,1024,1024]}</code> </p> </li> <li> <p>If using the CLI, <code>{\\\"data\\\":[1,3,1024,1024]}</code> </p> </li> </ul> </li> <li> <p>Examples for two inputs:</p> <ul> <li> <p>If using the console, <code>{\"var1\": [1,1,28,28], \"var2\":[1,1,28,28]} </code> </p> </li> <li> <p>If using the CLI, <code>{\\\"var1\\\": [1,1,28,28], \\\"var2\\\":[1,1,28,28]}</code> </p> </li> </ul> </li> </ul> </li> <li> <p> <code>PyTorch</code>: You can either specify the name and shape (NCHW format) of expected data inputs in order using a dictionary format for your trained model or you can specify the shape only using a list format. The dictionary formats required for the console and CLI are different. The list formats for the console and CLI are the same.</p> <ul> <li> <p>Examples for one input in dictionary format:</p> <ul> <li> <p>If using the console, <code>{\"input0\":[1,3,224,224]}</code> </p> </li> <li> <p>If using the CLI, <code>{\\\"input0\\\":[1,3,224,224]}</code> </p> </li> </ul> </li> <li> <p>Example for one input in list format: <code>[[1,3,224,224]]</code> </p> </li> <li> <p>Examples for two inputs in dictionary format:</p> <ul> <li> <p>If using the console, <code>{\"input0\":[1,3,224,224], \"input1\":[1,3,224,224]}</code> </p> </li> <li> <p>If using the CLI, <code>{\\\"input0\\\":[1,3,224,224], \\\"input1\\\":[1,3,224,224]} </code> </p> </li> </ul> </li> <li> <p>Example for two inputs in list format: <code>[[1,3,224,224], [1,3,224,224]]</code> </p> </li> </ul> </li> <li> <p> <code>XGBOOST</code>: input data name and shape are not needed.</p> </li> </ul> <p> <code>DataInputConfig</code> supports the following parameters for <code>CoreML</code> <a>OutputConfig$TargetDevice</a> (ML Model format):</p> <ul> <li> <p> <code>shape</code>: Input shape, for example <code>{\"input_1\": {\"shape\": [1,224,224,3]}}</code>. In addition to static input shapes, CoreML converter supports Flexible input shapes:</p> <ul> <li> <p>Range Dimension. You can use the Range Dimension feature if you know the input shape will be within some specific interval in that dimension, for example: <code>{\"input_1\": {\"shape\": [\"1..10\", 224, 224, 3]}}</code> </p> </li> <li> <p>Enumerated shapes. Sometimes, the models are trained to work only on a select set of inputs. You can enumerate all supported input shapes, for example: <code>{\"input_1\": {\"shape\": [[1, 224, 224, 3], [1, 160, 160, 3]]}}</code> </p> </li> </ul> </li> <li> <p> <code>default_shape</code>: Default input shape. You can set a default shape during conversion for both Range Dimension and Enumerated Shapes. For example <code>{\"input_1\": {\"shape\": [\"1..10\", 224, 224, 3], \"default_shape\": [1, 224, 224, 3]}}</code> </p> </li> <li> <p> <code>type</code>: Input type. Allowed values: <code>Image</code> and <code>Tensor</code>. By default, the converter generates an ML Model with inputs of type Tensor (MultiArray). User can set input type to be Image. Image input type requires additional input parameters such as <code>bias</code> and <code>scale</code>.</p> </li> <li> <p> <code>bias</code>: If the input type is an Image, you need to provide the bias vector.</p> </li> <li> <p> <code>scale</code>: If the input type is an Image, you need to provide a scale factor.</p> </li> </ul> <p>CoreML <code>ClassifierConfig</code> parameters can be specified using <a>OutputConfig$CompilerOptions</a>. CoreML converter supports Tensorflow and PyTorch models. CoreML conversion examples:</p> <ul> <li> <p>Tensor type input:</p> <ul> <li> <p> <code>\"DataInputConfig\": {\"input_1\": {\"shape\": [[1,224,224,3], [1,160,160,3]], \"default_shape\": [1,224,224,3]}}</code> </p> </li> </ul> </li> <li> <p>Tensor type input without input name (PyTorch):</p> <ul> <li> <p> <code>\"DataInputConfig\": [{\"shape\": [[1,3,224,224], [1,3,160,160]], \"default_shape\": [1,3,224,224]}]</code> </p> </li> </ul> </li> <li> <p>Image type input:</p> <ul> <li> <p> <code>\"DataInputConfig\": {\"input_1\": {\"shape\": [[1,224,224,3], [1,160,160,3]], \"default_shape\": [1,224,224,3], \"type\": \"Image\", \"bias\": [-1,-1,-1], \"scale\": 0.007843137255}}</code> </p> </li> <li> <p> <code>\"CompilerOptions\": {\"class_labels\": \"imagenet_labels_1000.txt\"}</code> </p> </li> </ul> </li> <li> <p>Image type input without input name (PyTorch):</p> <ul> <li> <p> <code>\"DataInputConfig\": [{\"shape\": [[1,3,224,224], [1,3,160,160]], \"default_shape\": [1,3,224,224], \"type\": \"Image\", \"bias\": [-1,-1,-1], \"scale\": 0.007843137255}]</code> </p> </li> <li> <p> <code>\"CompilerOptions\": {\"class_labels\": \"imagenet_labels_1000.txt\"}</code> </p> </li> </ul> </li> </ul> <p>Depending on the model format, <code>DataInputConfig</code> requires the following parameters for <code>ml_eia2</code> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_OutputConfig.html#sagemaker-Type-OutputConfig-TargetDevice\">OutputConfig:TargetDevice</a>.</p> <ul> <li> <p>For TensorFlow models saved in the SavedModel format, specify the input names from <code>signature_def_key</code> and the input model shapes for <code>DataInputConfig</code>. Specify the <code>signature_def_key</code> in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_OutputConfig.html#sagemaker-Type-OutputConfig-CompilerOptions\"> <code>OutputConfig:CompilerOptions</code> </a> if the model does not use TensorFlow's default signature def key. For example:</p> <ul> <li> <p> <code>\"DataInputConfig\": {\"inputs\": [1, 224, 224, 3]}</code> </p> </li> <li> <p> <code>\"CompilerOptions\": {\"signature_def_key\": \"serving_custom\"}</code> </p> </li> </ul> </li> <li> <p>For TensorFlow models saved as a frozen graph, specify the input tensor names and shapes in <code>DataInputConfig</code> and the output tensor names for <code>output_names</code> in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_OutputConfig.html#sagemaker-Type-OutputConfig-CompilerOptions\"> <code>OutputConfig:CompilerOptions</code> </a>. For example:</p> <ul> <li> <p> <code>\"DataInputConfig\": {\"input_tensor:0\": [1, 224, 224, 3]}</code> </p> </li> <li> <p> <code>\"CompilerOptions\": {\"output_names\": [\"output_tensor:0\"]}</code> </p> </li> </ul> </li> </ul>",
+                    "documentation": "<p>Specifies the name and shape of the expected data inputs for your trained model with a JSON dictionary form. The data inputs are <code>Framework</code> specific. </p> <ul> <li> <p> <code>TensorFlow</code>: You must specify the name and shape (NHWC format) of the expected data inputs using a dictionary format for your trained model. The dictionary formats required for the console and CLI are different.</p> <ul> <li> <p>Examples for one input:</p> <ul> <li> <p>If using the console, <code>{\"input\":[1,1024,1024,3]}</code> </p> </li> <li> <p>If using the CLI, <code>{\\\"input\\\":[1,1024,1024,3]}</code> </p> </li> </ul> </li> <li> <p>Examples for two inputs:</p> <ul> <li> <p>If using the console, <code>{\"data1\": [1,28,28,1], \"data2\":[1,28,28,1]}</code> </p> </li> <li> <p>If using the CLI, <code>{\\\"data1\\\": [1,28,28,1], \\\"data2\\\":[1,28,28,1]}</code> </p> </li> </ul> </li> </ul> </li> <li> <p> <code>KERAS</code>: You must specify the name and shape (NCHW format) of expected data inputs using a dictionary format for your trained model. Note that while Keras model artifacts should be uploaded in NHWC (channel-last) format, <code>DataInputConfig</code> should be specified in NCHW (channel-first) format. The dictionary formats required for the console and CLI are different.</p> <ul> <li> <p>Examples for one input:</p> <ul> <li> <p>If using the console, <code>{\"input_1\":[1,3,224,224]}</code> </p> </li> <li> <p>If using the CLI, <code>{\\\"input_1\\\":[1,3,224,224]}</code> </p> </li> </ul> </li> <li> <p>Examples for two inputs:</p> <ul> <li> <p>If using the console, <code>{\"input_1\": [1,3,224,224], \"input_2\":[1,3,224,224]} </code> </p> </li> <li> <p>If using the CLI, <code>{\\\"input_1\\\": [1,3,224,224], \\\"input_2\\\":[1,3,224,224]}</code> </p> </li> </ul> </li> </ul> </li> <li> <p> <code>MXNET/ONNX/DARKNET</code>: You must specify the name and shape (NCHW format) of the expected data inputs in order using a dictionary format for your trained model. The dictionary formats required for the console and CLI are different.</p> <ul> <li> <p>Examples for one input:</p> <ul> <li> <p>If using the console, <code>{\"data\":[1,3,1024,1024]}</code> </p> </li> <li> <p>If using the CLI, <code>{\\\"data\\\":[1,3,1024,1024]}</code> </p> </li> </ul> </li> <li> <p>Examples for two inputs:</p> <ul> <li> <p>If using the console, <code>{\"var1\": [1,1,28,28], \"var2\":[1,1,28,28]} </code> </p> </li> <li> <p>If using the CLI, <code>{\\\"var1\\\": [1,1,28,28], \\\"var2\\\":[1,1,28,28]}</code> </p> </li> </ul> </li> </ul> </li> <li> <p> <code>PyTorch</code>: You can either specify the name and shape (NCHW format) of expected data inputs in order using a dictionary format for your trained model or you can specify the shape only using a list format. The dictionary formats required for the console and CLI are different. The list formats for the console and CLI are the same.</p> <ul> <li> <p>Examples for one input in dictionary format:</p> <ul> <li> <p>If using the console, <code>{\"input0\":[1,3,224,224]}</code> </p> </li> <li> <p>If using the CLI, <code>{\\\"input0\\\":[1,3,224,224]}</code> </p> </li> </ul> </li> <li> <p>Example for one input in list format: <code>[[1,3,224,224]]</code> </p> </li> <li> <p>Examples for two inputs in dictionary format:</p> <ul> <li> <p>If using the console, <code>{\"input0\":[1,3,224,224], \"input1\":[1,3,224,224]}</code> </p> </li> <li> <p>If using the CLI, <code>{\\\"input0\\\":[1,3,224,224], \\\"input1\\\":[1,3,224,224]} </code> </p> </li> </ul> </li> <li> <p>Example for two inputs in list format: <code>[[1,3,224,224], [1,3,224,224]]</code> </p> </li> </ul> </li> <li> <p> <code>XGBOOST</code>: input data name and shape are not needed.</p> </li> </ul> <p> <code>DataInputConfig</code> supports the following parameters for <code>CoreML</code> <code>TargetDevice</code> (ML Model format):</p> <ul> <li> <p> <code>shape</code>: Input shape, for example <code>{\"input_1\": {\"shape\": [1,224,224,3]}}</code>. In addition to static input shapes, CoreML converter supports Flexible input shapes:</p> <ul> <li> <p>Range Dimension. You can use the Range Dimension feature if you know the input shape will be within some specific interval in that dimension, for example: <code>{\"input_1\": {\"shape\": [\"1..10\", 224, 224, 3]}}</code> </p> </li> <li> <p>Enumerated shapes. Sometimes, the models are trained to work only on a select set of inputs. You can enumerate all supported input shapes, for example: <code>{\"input_1\": {\"shape\": [[1, 224, 224, 3], [1, 160, 160, 3]]}}</code> </p> </li> </ul> </li> <li> <p> <code>default_shape</code>: Default input shape. You can set a default shape during conversion for both Range Dimension and Enumerated Shapes. For example <code>{\"input_1\": {\"shape\": [\"1..10\", 224, 224, 3], \"default_shape\": [1, 224, 224, 3]}}</code> </p> </li> <li> <p> <code>type</code>: Input type. Allowed values: <code>Image</code> and <code>Tensor</code>. By default, the converter generates an ML Model with inputs of type Tensor (MultiArray). User can set input type to be Image. Image input type requires additional input parameters such as <code>bias</code> and <code>scale</code>.</p> </li> <li> <p> <code>bias</code>: If the input type is an Image, you need to provide the bias vector.</p> </li> <li> <p> <code>scale</code>: If the input type is an Image, you need to provide a scale factor.</p> </li> </ul> <p>CoreML <code>ClassifierConfig</code> parameters can be specified using <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_OutputConfig.html\">OutputConfig</a> <code>CompilerOptions</code>. CoreML converter supports Tensorflow and PyTorch models. CoreML conversion examples:</p> <ul> <li> <p>Tensor type input:</p> <ul> <li> <p> <code>\"DataInputConfig\": {\"input_1\": {\"shape\": [[1,224,224,3], [1,160,160,3]], \"default_shape\": [1,224,224,3]}}</code> </p> </li> </ul> </li> <li> <p>Tensor type input without input name (PyTorch):</p> <ul> <li> <p> <code>\"DataInputConfig\": [{\"shape\": [[1,3,224,224], [1,3,160,160]], \"default_shape\": [1,3,224,224]}]</code> </p> </li> </ul> </li> <li> <p>Image type input:</p> <ul> <li> <p> <code>\"DataInputConfig\": {\"input_1\": {\"shape\": [[1,224,224,3], [1,160,160,3]], \"default_shape\": [1,224,224,3], \"type\": \"Image\", \"bias\": [-1,-1,-1], \"scale\": 0.007843137255}}</code> </p> </li> <li> <p> <code>\"CompilerOptions\": {\"class_labels\": \"imagenet_labels_1000.txt\"}</code> </p> </li> </ul> </li> <li> <p>Image type input without input name (PyTorch):</p> <ul> <li> <p> <code>\"DataInputConfig\": [{\"shape\": [[1,3,224,224], [1,3,160,160]], \"default_shape\": [1,3,224,224], \"type\": \"Image\", \"bias\": [-1,-1,-1], \"scale\": 0.007843137255}]</code> </p> </li> <li> <p> <code>\"CompilerOptions\": {\"class_labels\": \"imagenet_labels_1000.txt\"}</code> </p> </li> </ul> </li> </ul> <p>Depending on the model format, <code>DataInputConfig</code> requires the following parameters for <code>ml_eia2</code> <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_OutputConfig.html#sagemaker-Type-OutputConfig-TargetDevice\">OutputConfig:TargetDevice</a>.</p> <ul> <li> <p>For TensorFlow models saved in the SavedModel format, specify the input names from <code>signature_def_key</code> and the input model shapes for <code>DataInputConfig</code>. Specify the <code>signature_def_key</code> in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_OutputConfig.html#sagemaker-Type-OutputConfig-CompilerOptions\"> <code>OutputConfig:CompilerOptions</code> </a> if the model does not use TensorFlow's default signature def key. For example:</p> <ul> <li> <p> <code>\"DataInputConfig\": {\"inputs\": [1, 224, 224, 3]}</code> </p> </li> <li> <p> <code>\"CompilerOptions\": {\"signature_def_key\": \"serving_custom\"}</code> </p> </li> </ul> </li> <li> <p>For TensorFlow models saved as a frozen graph, specify the input tensor names and shapes in <code>DataInputConfig</code> and the output tensor names for <code>output_names</code> in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_OutputConfig.html#sagemaker-Type-OutputConfig-CompilerOptions\"> <code>OutputConfig:CompilerOptions</code> </a>. For example:</p> <ul> <li> <p> <code>\"DataInputConfig\": {\"input_tensor:0\": [1, 224, 224, 3]}</code> </p> </li> <li> <p> <code>\"CompilerOptions\": {\"output_names\": [\"output_tensor:0\"]}</code> </p> </li> </ul> </li> </ul>",
                     "shape": "DataInputConfig"
                 },
                 "Framework": {
                     "documentation": "<p>Identifies the framework in which the model was trained. For example: TENSORFLOW.</p>",
                     "shape": "Framework"
                 },
                 "FrameworkVersion": {
@@ -21394,15 +21718,21 @@
                 "ml.g5.xlarge",
                 "ml.g5.2xlarge",
                 "ml.g5.4xlarge",
                 "ml.g5.8xlarge",
                 "ml.g5.16xlarge",
                 "ml.g5.12xlarge",
                 "ml.g5.24xlarge",
-                "ml.g5.48xlarge"
+                "ml.g5.48xlarge",
+                "ml.inf1.xlarge",
+                "ml.inf1.2xlarge",
+                "ml.inf1.6xlarge",
+                "ml.inf1.24xlarge",
+                "ml.p4d.24xlarge",
+                "ml.p4de.24xlarge"
             ],
             "type": "string"
         },
         "Integer": {
             "type": "integer"
         },
         "IntegerParameterRange": {
@@ -21457,28 +21787,39 @@
             },
             "min": 0,
             "type": "list"
         },
         "IntegerValue": {
             "type": "integer"
         },
+        "InvocationEndTime": {
+            "type": "timestamp"
+        },
+        "InvocationStartTime": {
+            "type": "timestamp"
+        },
         "InvocationsMaxRetries": {
             "max": 3,
             "min": 0,
             "type": "integer"
         },
         "InvocationsTimeoutInSeconds": {
             "max": 3600,
             "min": 1,
             "type": "integer"
         },
         "IotRoleAlias": {
             "pattern": "^arn:aws[a-z\\-]*:iam::\\d{12}:rolealias/?[a-zA-Z_0-9+=,.@\\-_/]+$",
             "type": "string"
         },
+        "ItemIdentifierAttributeName": {
+            "max": 256,
+            "min": 1,
+            "type": "string"
+        },
         "JobDurationInSeconds": {
             "min": 1,
             "type": "integer"
         },
         "JobReferenceCode": {
             "min": 1,
             "pattern": ".+",
@@ -22233,15 +22574,15 @@
                     "shape": "Timestamp"
                 },
                 "CreationTimeBefore": {
                     "documentation": "<p>A filter that returns only AppImageConfigs created on or before the specified time.</p>",
                     "shape": "Timestamp"
                 },
                 "MaxResults": {
-                    "documentation": "<p>The maximum number of AppImageConfigs to return in the response. The default value is 10. </p>",
+                    "documentation": "<p>The total number of items to return in the response. If the total number of items available is more than the value specified, a <code>NextToken</code> is provided in the response. To resume pagination, provide the <code>NextToken</code> value in the as part of a subsequent call. The default value is 10.</p>",
                     "shape": "MaxResults"
                 },
                 "ModifiedTimeAfter": {
                     "documentation": "<p>A filter that returns only AppImageConfigs modified on or after the specified time.</p>",
                     "shape": "Timestamp"
                 },
                 "ModifiedTimeBefore": {
@@ -22283,15 +22624,15 @@
         "ListAppsRequest": {
             "members": {
                 "DomainIdEquals": {
                     "documentation": "<p>A parameter to search for the domain ID.</p>",
                     "shape": "DomainId"
                 },
                 "MaxResults": {
-                    "documentation": "<p>Returns a list up to a specified limit.</p>",
+                    "documentation": "<p>The total number of items to return in the response. If the total number of items available is more than the value specified, a <code>NextToken</code> is provided in the response. To resume pagination, provide the <code>NextToken</code> value in the as part of a subsequent call. The default value is 10.</p>",
                     "shape": "MaxResults"
                 },
                 "NextToken": {
                     "documentation": "<p>If the previous response was truncated, you will receive this token. Use it in your next request to receive the next set of results.</p>",
                     "shape": "NextToken"
                 },
                 "SortBy": {
@@ -22646,24 +22987,24 @@
                     "shape": "ListCompilationJobsSortBy"
                 },
                 "SortOrder": {
                     "documentation": "<p>The sort order for results. The default is <code>Ascending</code>.</p>",
                     "shape": "SortOrder"
                 },
                 "StatusEquals": {
-                    "documentation": "<p>A filter that retrieves model compilation jobs with a specific <a>DescribeCompilationJobResponse$CompilationJobStatus</a> status.</p>",
+                    "documentation": "<p>A filter that retrieves model compilation jobs with a specific <code>CompilationJobStatus</code> status.</p>",
                     "shape": "CompilationJobStatus"
                 }
             },
             "type": "structure"
         },
         "ListCompilationJobsResponse": {
             "members": {
                 "CompilationJobSummaries": {
-                    "documentation": "<p>An array of <a>CompilationJobSummary</a> objects, each describing a model compilation job. </p>",
+                    "documentation": "<p>An array of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CompilationJobSummary.html\">CompilationJobSummary</a> objects, each describing a model compilation job. </p>",
                     "shape": "CompilationJobSummaries"
                 },
                 "NextToken": {
                     "documentation": "<p>If the response is truncated, Amazon SageMaker returns this <code>NextToken</code>. To retrieve the next set of model compilation jobs, use this token in the next request.</p>",
                     "shape": "NextToken"
                 }
             },
@@ -22890,15 +23231,15 @@
                 "DeviceSummaries"
             ],
             "type": "structure"
         },
         "ListDomainsRequest": {
             "members": {
                 "MaxResults": {
-                    "documentation": "<p>Returns a list up to a specified limit.</p>",
+                    "documentation": "<p>The total number of items to return in the response. If the total number of items available is more than the value specified, a <code>NextToken</code> is provided in the response. To resume pagination, provide the <code>NextToken</code> value in the as part of a subsequent call. The default value is 10.</p>",
                     "shape": "MaxResults"
                 },
                 "NextToken": {
                     "documentation": "<p>If the previous response was truncated, you will receive this token. Use it in your next request to receive the next set of results.</p>",
                     "shape": "NextToken"
                 }
             },
@@ -23595,15 +23936,15 @@
                 }
             },
             "type": "structure"
         },
         "ListHyperParameterTuningJobsResponse": {
             "members": {
                 "HyperParameterTuningJobSummaries": {
-                    "documentation": "<p>A list of <a>HyperParameterTuningJobSummary</a> objects that describe the tuning jobs that the <code>ListHyperParameterTuningJobs</code> request returned.</p>",
+                    "documentation": "<p>A list of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobSummary.html\">HyperParameterTuningJobSummary</a> objects that describe the tuning jobs that the <code>ListHyperParameterTuningJobs</code> request returned.</p>",
                     "shape": "HyperParameterTuningJobSummaries"
                 },
                 "NextToken": {
                     "documentation": "<p>If the result of this <code>ListHyperParameterTuningJobs</code> request was truncated, the response includes a <code>NextToken</code>. To retrieve the next set of tuning jobs, use the token in the next request.</p>",
                     "shape": "NextToken"
                 }
             },
@@ -23758,19 +24099,19 @@
                     "shape": "SortInferenceExperimentsBy"
                 },
                 "SortOrder": {
                     "documentation": "<p>The direction of sorting (ascending or descending).</p>",
                     "shape": "SortOrder"
                 },
                 "StatusEquals": {
-                    "documentation": "<p> Selects inference experiments which are in this status. For the possible statuses, see <a>DescribeInferenceExperimentResponse$Status</a>. </p>",
+                    "documentation": "<p> Selects inference experiments which are in this status. For the possible statuses, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeInferenceExperiment.html\">DescribeInferenceExperiment</a>. </p>",
                     "shape": "InferenceExperimentStatus"
                 },
                 "Type": {
-                    "documentation": "<p> Selects inference experiments of this type. For the possible types of inference experiments, see <a>CreateInferenceExperimentRequest$Type</a>. </p>",
+                    "documentation": "<p> Selects inference experiments of this type. For the possible types of inference experiments, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateInferenceExperiment.html\">CreateInferenceExperiment</a>. </p>",
                     "shape": "InferenceExperimentType"
                 }
             },
             "type": "structure"
         },
         "ListInferenceExperimentsResponse": {
             "members": {
@@ -23844,14 +24185,22 @@
                     "documentation": "<p>A filter that returns only jobs that were last modified before the specified time (timestamp).</p>",
                     "shape": "LastModifiedTime"
                 },
                 "MaxResults": {
                     "documentation": "<p>The maximum number of recommendations to return in the response.</p>",
                     "shape": "MaxResults"
                 },
+                "ModelNameEquals": {
+                    "documentation": "<p>A filter that returns only jobs that were created for this model.</p>",
+                    "shape": "ModelName"
+                },
+                "ModelPackageVersionArnEquals": {
+                    "documentation": "<p>A filter that returns only jobs that were created for this versioned model package.</p>",
+                    "shape": "ModelPackageArn"
+                },
                 "NameContains": {
                     "documentation": "<p>A string in the job name. This filter returns only recommendations whose name contains the specified string.</p>",
                     "shape": "NameContains"
                 },
                 "NextToken": {
                     "documentation": "<p>If the response to a previous <code>ListInferenceRecommendationsJobsRequest</code> request was truncated, the response includes a <code>NextToken</code>. To retrieve the next set of recommendations, use the token in the next request.</p>",
                     "shape": "NextToken"
@@ -25005,15 +25354,15 @@
                     "shape": "MaxResults"
                 },
                 "NextToken": {
                     "documentation": "<p>If the result of the previous <code>ListPipelineExecutions</code> request was truncated, the response includes a <code>NextToken</code>. To retrieve the next set of pipeline executions, use the token in the next request.</p>",
                     "shape": "NextToken"
                 },
                 "PipelineName": {
-                    "documentation": "<p>The name of the pipeline.</p>",
+                    "documentation": "<p>The name or Amazon Resource Name (ARN) of the pipeline.</p>",
                     "shape": "PipelineNameOrArn"
                 },
                 "SortBy": {
                     "documentation": "<p>The field by which to sort results. The default is <code>CreatedTime</code>.</p>",
                     "shape": "SortPipelineExecutionsBy"
                 },
                 "SortOrder": {
@@ -25232,15 +25581,15 @@
         "ListSpacesRequest": {
             "members": {
                 "DomainIdEquals": {
                     "documentation": "<p>A parameter to search for the Domain ID.</p>",
                     "shape": "DomainId"
                 },
                 "MaxResults": {
-                    "documentation": "<p>Returns a list up to a specified limit.</p>",
+                    "documentation": "<p>The total number of items to return in the response. If the total number of items available is more than the value specified, a <code>NextToken</code> is provided in the response. To resume pagination, provide the <code>NextToken</code> value in the as part of a subsequent call. The default value is 10.</p>",
                     "shape": "MaxResults"
                 },
                 "NextToken": {
                     "documentation": "<p>If the previous response was truncated, you will receive this token. Use it in your next request to receive the next set of results.</p>",
                     "shape": "NextToken"
                 },
                 "SortBy": {
@@ -25328,15 +25677,15 @@
                     "shape": "Timestamp"
                 },
                 "CreationTimeBefore": {
                     "documentation": "<p>A filter that returns only Lifecycle Configurations created on or before the specified time.</p>",
                     "shape": "Timestamp"
                 },
                 "MaxResults": {
-                    "documentation": "<p>The maximum number of Studio Lifecycle Configurations to return in the response. The default value is 10.</p>",
+                    "documentation": "<p>The total number of items to return in the response. If the total number of items available is more than the value specified, a <code>NextToken</code> is provided in the response. To resume pagination, provide the <code>NextToken</code> value in the as part of a subsequent call. The default value is 10.</p>",
                     "shape": "MaxResults"
                 },
                 "ModifiedTimeAfter": {
                     "documentation": "<p>A filter that returns only Lifecycle Configurations modified after the specified time.</p>",
                     "shape": "Timestamp"
                 },
                 "ModifiedTimeBefore": {
@@ -25361,15 +25710,15 @@
                 }
             },
             "type": "structure"
         },
         "ListStudioLifecycleConfigsResponse": {
             "members": {
                 "NextToken": {
-                    "documentation": "<p>A token for getting the next set of actions, if there are any.</p>",
+                    "documentation": "<p>If the previous response was truncated, you will receive this token. Use it in your next request to receive the next set of results.</p>",
                     "shape": "NextToken"
                 },
                 "StudioLifecycleConfigs": {
                     "documentation": "<p>A list of Lifecycle Configurations and their properties.</p>",
                     "shape": "StudioLifecycleConfigsList"
                 }
             },
@@ -25481,15 +25830,15 @@
         "ListTrainingJobsForHyperParameterTuningJobResponse": {
             "members": {
                 "NextToken": {
                     "documentation": "<p>If the result of this <code>ListTrainingJobsForHyperParameterTuningJob</code> request was truncated, the response includes a <code>NextToken</code>. To retrieve the next set of training jobs, use the token in the next request.</p>",
                     "shape": "NextToken"
                 },
                 "TrainingJobSummaries": {
-                    "documentation": "<p>A list of <a>TrainingJobSummary</a> objects that describe the training jobs that the <code>ListTrainingJobsForHyperParameterTuningJob</code> request returned.</p>",
+                    "documentation": "<p>A list of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_TrainingJobSummary.html\">TrainingJobSummary</a> objects that describe the training jobs that the <code>ListTrainingJobsForHyperParameterTuningJob</code> request returned.</p>",
                     "shape": "HyperParameterTrainingJobSummaries"
                 }
             },
             "required": [
                 "TrainingJobSummaries"
             ],
             "type": "structure"
@@ -25735,15 +26084,15 @@
         "ListUserProfilesRequest": {
             "members": {
                 "DomainIdEquals": {
                     "documentation": "<p>A parameter by which to filter the results.</p>",
                     "shape": "DomainId"
                 },
                 "MaxResults": {
-                    "documentation": "<p>Returns a list up to a specified limit.</p>",
+                    "documentation": "<p>The total number of items to return in the response. If the total number of items available is more than the value specified, a <code>NextToken</code> is provided in the response. To resume pagination, provide the <code>NextToken</code> value in the as part of a subsequent call. The default value is 10.</p>",
                     "shape": "MaxResults"
                 },
                 "NextToken": {
                     "documentation": "<p>If the previous response was truncated, you will receive this token. Use it in your next request to receive the next set of results.</p>",
                     "shape": "NextToken"
                 },
                 "SortBy": {
@@ -25955,15 +26304,15 @@
             "type": "integer"
         },
         "MaxWaitTimeInSeconds": {
             "min": 1,
             "type": "integer"
         },
         "MaximumExecutionTimeoutInSeconds": {
-            "max": 14400,
+            "max": 28800,
             "min": 600,
             "type": "integer"
         },
         "MaximumRetryAttempts": {
             "max": 30,
             "min": 1,
             "type": "integer"
@@ -26067,22 +26416,22 @@
                     "documentation": "<p>The value of the metric.</p>",
                     "shape": "Float"
                 }
             },
             "type": "structure"
         },
         "MetricDefinition": {
-            "documentation": "<p>Specifies a metric that the training algorithm writes to <code>stderr</code> or <code>stdout</code>. SageMakerhyperparameter tuning captures all defined metrics. You specify one metric that a hyperparameter tuning job uses as its objective metric to choose the best training job.</p>",
+            "documentation": "<p>Specifies a metric that the training algorithm writes to <code>stderr</code> or <code>stdout</code>. You can view these logs to understand how your training job performs and check for any errors encountered during training. SageMaker hyperparameter tuning captures all defined metrics. Specify one of the defined metrics to use as an objective metric using the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTrainingJobDefinition.html#sagemaker-Type-HyperParameterTrainingJobDefinition-TuningObjective\">TuningObjective</a> parameter in the <code>HyperParameterTrainingJobDefinition</code> API to evaluate job performance during hyperparameter tuning.</p>",
             "members": {
                 "Name": {
                     "documentation": "<p>The name of the metric.</p>",
                     "shape": "MetricName"
                 },
                 "Regex": {
-                    "documentation": "<p>A regular expression that searches the output of a training job and gets the value of the metric. For more information about using regular expressions to define metrics, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-define-metrics.html\">Defining Objective Metrics</a>.</p>",
+                    "documentation": "<p>A regular expression that searches the output of a training job and gets the value of the metric. For more information about using regular expressions to define metrics, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-define-metrics-variables.html\">Defining metrics and environment variables</a>.</p>",
                     "shape": "MetricRegex"
                 }
             },
             "required": [
                 "Name",
                 "Regex"
             ],
@@ -26143,24 +26492,28 @@
         },
         "MinimumInstanceMetadataServiceVersion": {
             "max": 1,
             "pattern": "1|2",
             "type": "string"
         },
         "Model": {
-            "documentation": "<p>The properties of a model as returned by the <a>Search</a> API.</p>",
+            "documentation": "<p>The properties of a model as returned by the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API.</p>",
             "members": {
                 "Containers": {
                     "documentation": "<p>The containers in the inference pipeline.</p>",
                     "shape": "ContainerDefinitionList"
                 },
                 "CreationTime": {
                     "documentation": "<p>A timestamp that indicates when the model was created.</p>",
                     "shape": "Timestamp"
                 },
+                "DeploymentRecommendation": {
+                    "documentation": "<p>A set of recommended deployment configurations for the model.</p>",
+                    "shape": "DeploymentRecommendation"
+                },
                 "EnableNetworkIsolation": {
                     "documentation": "<p>Isolates the model container. No inbound or outbound network calls can be made to or from the model container.</p>",
                     "shape": "Boolean"
                 },
                 "ExecutionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that you specified for the model.</p>",
                     "shape": "RoleArn"
@@ -26278,15 +26631,15 @@
             ],
             "type": "string"
         },
         "ModelCard": {
             "documentation": "<p>An Amazon SageMaker Model Card.</p>",
             "members": {
                 "Content": {
-                    "documentation": "<p>The content of the model card. Content uses the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-cards-api-json-schema.html\">model card JSON schema</a> and provided as a string.</p>",
+                    "documentation": "<p>The content of the model card. Content uses the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-cards.html#model-cards-json-schema\">model card JSON schema</a> and provided as a string.</p>",
                     "shape": "ModelCardContent"
                 },
                 "CreatedBy": {
                     "shape": "UserContext"
                 },
                 "CreationTime": {
                     "documentation": "<p>The date and time that the model card was created.</p>",
@@ -26315,14 +26668,18 @@
                     "documentation": "<p>The version of the model card.</p>",
                     "shape": "Integer"
                 },
                 "ModelId": {
                     "documentation": "<p>The unique name (ID) of the model.</p>",
                     "shape": "String"
                 },
+                "ModelPackageGroupName": {
+                    "documentation": "<p>The model package group that contains the model package. Only relevant for model cards created for model packages in the Amazon SageMaker Model Registry. </p>",
+                    "shape": "String"
+                },
                 "RiskRating": {
                     "documentation": "<p>The risk rating of the model. Different organizations might have different criteria for model card risk ratings. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-cards-risk-rating.html\">Risk ratings</a>.</p>",
                     "shape": "String"
                 },
                 "SecurityConfig": {
                     "documentation": "<p>The security configuration used to protect model card data.</p>",
                     "shape": "ModelCardSecurityConfig"
@@ -26591,14 +26948,21 @@
                 "InvocationsTimeoutInSeconds": {
                     "documentation": "<p>The timeout value in seconds for an invocation request. The default value is 600.</p>",
                     "shape": "InvocationsTimeoutInSeconds"
                 }
             },
             "type": "structure"
         },
+        "ModelCompressionType": {
+            "enum": [
+                "None",
+                "Gzip"
+            ],
+            "type": "string"
+        },
         "ModelConfiguration": {
             "documentation": "<p>Defines the model configuration. Includes the specification name and environment parameters.</p>",
             "members": {
                 "CompilationJobName": {
                     "documentation": "<p>The name of the compilation job used to create the recommended model artifacts.</p>",
                     "shape": "RecommendationJobCompilationJobName"
                 },
@@ -26803,14 +27167,27 @@
                 "Statistics": {
                     "documentation": "<p>Data quality statistics for a model.</p>",
                     "shape": "MetricsSource"
                 }
             },
             "type": "structure"
         },
+        "ModelDataSource": {
+            "documentation": "<p>Specifies the location of ML model data to deploy. If specified, you must specify one and only one of the available data sources.</p>",
+            "members": {
+                "S3DataSource": {
+                    "documentation": "<p>Specifies the S3 location of ML model data to deploy.</p>",
+                    "shape": "S3ModelDataSource"
+                }
+            },
+            "required": [
+                "S3DataSource"
+            ],
+            "type": "structure"
+        },
         "ModelDeployConfig": {
             "documentation": "<p>Specifies how to generate the endpoint name for an automatic one-click Autopilot model deployment.</p>",
             "members": {
                 "AutoGenerateEndpointName": {
                     "documentation": "<p>Set to <code>True</code> to automatically generate an endpoint name for a one-click Autopilot model deployment; set to <code>False</code> otherwise. The default value is <code>False</code>.</p> <note> <p>If you set <code>AutoGenerateEndpointName</code> to <code>True</code>, do not specify the <code>EndpointName</code>; otherwise a 400 error is thrown.</p> </note>",
                     "shape": "AutoGenerateEndpointName"
                 },
@@ -27607,14 +27984,32 @@
                 }
             },
             "required": [
                 "GroundTruthS3Input"
             ],
             "type": "structure"
         },
+        "ModelRegisterSettings": {
+            "documentation": "<p>The model registry settings for the SageMaker Canvas application.</p>",
+            "members": {
+                "CrossAccountModelRegisterRoleArn": {
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the SageMaker model registry account. Required only to register model versions created by a different SageMaker Canvas Amazon Web Services account than the Amazon Web Services account in which SageMaker model registry is set up.</p>",
+                    "shape": "RoleArn"
+                },
+                "Status": {
+                    "documentation": "<p>Describes whether the integration to the model registry is enabled or disabled in the Canvas application.</p>",
+                    "shape": "FeatureStatus"
+                }
+            },
+            "type": "structure"
+        },
+        "ModelSetupTime": {
+            "min": 0,
+            "type": "integer"
+        },
         "ModelSortKey": {
             "enum": [
                 "Name",
                 "CreationTime"
             ],
             "type": "string"
         },
@@ -28535,15 +28930,15 @@
         },
         "NameContains": {
             "max": 63,
             "pattern": "[a-zA-Z0-9\\-]+",
             "type": "string"
         },
         "NeoVpcConfig": {
-            "documentation": "<p>The <a>VpcConfig</a> configuration object that specifies the VPC that you want the compilation jobs to connect to. For more information on controlling access to your Amazon S3 buckets used for compilation job, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/neo-vpc.html\">Give Amazon SageMaker Compilation Jobs Access to Resources in Your Amazon VPC</a>.</p>",
+            "documentation": "<p>The <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_VpcConfig.html\">VpcConfig</a> configuration object that specifies the VPC that you want the compilation jobs to connect to. For more information on controlling access to your Amazon S3 buckets used for compilation job, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/neo-vpc.html\">Give Amazon SageMaker Compilation Jobs Access to Resources in Your Amazon VPC</a>.</p>",
             "members": {
                 "SecurityGroupIds": {
                     "documentation": "<p>The VPC security group IDs. IDs have the form of <code>sg-xxxxxxxx</code>. Specify the security groups for the VPC that is specified in the <code>Subnets</code> field.</p>",
                     "shape": "NeoVpcSecurityGroupIds"
                 },
                 "Subnets": {
                     "documentation": "<p>The ID of the subnets in the VPC that you want to connect the compilation job to for accessing the model in Amazon S3.</p>",
@@ -28579,15 +28974,15 @@
             "member": {
                 "shape": "NeoVpcSubnetId"
             },
             "min": 1,
             "type": "list"
         },
         "NestedFilters": {
-            "documentation": "<p>A list of nested <a>Filter</a> objects. A resource must satisfy the conditions of all filters to be included in the results returned from the <a>Search</a> API.</p> <p>For example, to filter on a training job's <code>InputDataConfig</code> property with a specific channel name and <code>S3Uri</code> prefix, define the following filters:</p> <ul> <li> <p> <code>'{Name:\"InputDataConfig.ChannelName\", \"Operator\":\"Equals\", \"Value\":\"train\"}',</code> </p> </li> <li> <p> <code>'{Name:\"InputDataConfig.DataSource.S3DataSource.S3Uri\", \"Operator\":\"Contains\", \"Value\":\"mybucket/catdata\"}'</code> </p> </li> </ul>",
+            "documentation": "<p>A list of nested <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Filter.html\">Filter</a> objects. A resource must satisfy the conditions of all filters to be included in the results returned from the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API.</p> <p>For example, to filter on a training job's <code>InputDataConfig</code> property with a specific channel name and <code>S3Uri</code> prefix, define the following filters:</p> <ul> <li> <p> <code>'{Name:\"InputDataConfig.ChannelName\", \"Operator\":\"Equals\", \"Value\":\"train\"}',</code> </p> </li> <li> <p> <code>'{Name:\"InputDataConfig.DataSource.S3DataSource.S3Uri\", \"Operator\":\"Contains\", \"Value\":\"mybucket/catdata\"}'</code> </p> </li> </ul>",
             "members": {
                 "Filters": {
                     "documentation": "<p>A list of filters. Each filter acts on a property. Filters must contain at least one <code>Filters</code> value. For example, a <code>NestedFilters</code> call might include a filter on the <code>PropertyName</code> parameter of the <code>InputDataConfig</code> property: <code>InputDataConfig.DataSource.S3DataSource.S3Uri</code>.</p>",
                     "shape": "FilterList"
                 },
                 "NestedPropertyName": {
                     "documentation": "<p>The name of the property to use in the nested filters. The value must match a listed property name, such as <code>InputDataConfig</code>.</p>",
@@ -28899,15 +29294,15 @@
             "documentation": "<p>The configuration of an <code>OfflineStore</code>.</p> <p>Provide an <code>OfflineStoreConfig</code> in a request to <code>CreateFeatureGroup</code> to create an <code>OfflineStore</code>.</p> <p>To encrypt an <code>OfflineStore</code> using at rest data encryption, specify Amazon Web Services Key Management Service (KMS) key ID, or <code>KMSKeyId</code>, in <code>S3StorageConfig</code>.</p>",
             "members": {
                 "DataCatalogConfig": {
                     "documentation": "<p>The meta data of the Glue table that is autogenerated when an <code>OfflineStore</code> is created. </p>",
                     "shape": "DataCatalogConfig"
                 },
                 "DisableGlueTableCreation": {
-                    "documentation": "<p>Set to <code>True</code> to disable the automatic creation of an Amazon Web Services Glue table when configuring an <code>OfflineStore</code>.</p>",
+                    "documentation": "<p>Set to <code>True</code> to disable the automatic creation of an Amazon Web Services Glue table when configuring an <code>OfflineStore</code>. If set to <code>False</code>, Feature Store will name the <code>OfflineStore</code> Glue table following <a href=\"https://docs.aws.amazon.com/athena/latest/ug/tables-databases-columns-names.html\">Athena's naming recommendations</a>.</p> <p>The default value is <code>False</code>.</p>",
                     "shape": "Boolean"
                 },
                 "S3StorageConfig": {
                     "documentation": "<p>The Amazon Simple Storage (Amazon S3) location of <code>OfflineStore</code>.</p>",
                     "shape": "S3StorageConfig"
                 },
                 "TableFormat": {
@@ -29042,23 +29437,37 @@
             },
             "required": [
                 "Groups"
             ],
             "type": "structure"
         },
         "OnlineStoreConfig": {
-            "documentation": "<p>Use this to specify the Amazon Web Services Key Management Service (KMS) Key ID, or <code>KMSKeyId</code>, for at rest data encryption. You can turn <code>OnlineStore</code> on or off by specifying the <code>EnableOnlineStore</code> flag at General Assembly; the default value is <code>False</code>.</p>",
+            "documentation": "<p>Use this to specify the Amazon Web Services Key Management Service (KMS) Key ID, or <code>KMSKeyId</code>, for at rest data encryption. You can turn <code>OnlineStore</code> on or off by specifying the <code>EnableOnlineStore</code> flag at General Assembly.</p> <p>The default value is <code>False</code>.</p>",
             "members": {
                 "EnableOnlineStore": {
                     "documentation": "<p>Turn <code>OnlineStore</code> off by specifying <code>False</code> for the <code>EnableOnlineStore</code> flag. Turn <code>OnlineStore</code> on by specifying <code>True</code> for the <code>EnableOnlineStore</code> flag. </p> <p>The default value is <code>False</code>.</p>",
                     "shape": "Boolean"
                 },
                 "SecurityConfig": {
                     "documentation": "<p>Use to specify KMS Key ID (<code>KMSKeyId</code>) for at-rest encryption of your <code>OnlineStore</code>.</p>",
                     "shape": "OnlineStoreSecurityConfig"
+                },
+                "TtlDuration": {
+                    "documentation": "<p>Time to live duration, where the record is hard deleted after the expiration time is reached; <code>ExpiresAt</code> = <code>EventTime</code> + <code>TtlDuration</code>. For information on HardDelete, see the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_feature_store_DeleteRecord.html\">DeleteRecord</a> API in the Amazon SageMaker API Reference guide.</p>",
+                    "shape": "TtlDuration"
+                }
+            },
+            "type": "structure"
+        },
+        "OnlineStoreConfigUpdate": {
+            "documentation": "<p>Updates the feature group online store configuration.</p>",
+            "members": {
+                "TtlDuration": {
+                    "documentation": "<p>Time to live duration, where the record is hard deleted after the expiration time is reached; <code>ExpiresAt</code> = <code>EventTime</code> + <code>TtlDuration</code>. For information on HardDelete, see the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_feature_store_DeleteRecord.html\">DeleteRecord</a> API in the Amazon SageMaker API Reference guide.</p>",
+                    "shape": "TtlDuration"
                 }
             },
             "type": "structure"
         },
         "OnlineStoreSecurityConfig": {
             "documentation": "<p>The security configuration for <code>OnlineStore</code>.</p>",
             "members": {
@@ -29100,31 +29509,38 @@
         "OrderKey": {
             "enum": [
                 "Ascending",
                 "Descending"
             ],
             "type": "string"
         },
+        "OutputCompressionType": {
+            "enum": [
+                "GZIP",
+                "NONE"
+            ],
+            "type": "string"
+        },
         "OutputConfig": {
             "documentation": "<p>Contains information about the output location for the compiled model and the target device that the model runs on. <code>TargetDevice</code> and <code>TargetPlatform</code> are mutually exclusive, so you need to choose one between the two to specify your target device or platform. If you cannot find your device you want to use from the <code>TargetDevice</code> list, use <code>TargetPlatform</code> to describe the platform of your edge device and <code>CompilerOptions</code> if there are specific settings that are required or recommended to use for particular TargetPlatform.</p>",
             "members": {
                 "CompilerOptions": {
-                    "documentation": "<p>Specifies additional parameters for compiler options in JSON format. The compiler options are <code>TargetPlatform</code> specific. It is required for NVIDIA accelerators and highly recommended for CPU compilations. For any other cases, it is optional to specify <code>CompilerOptions.</code> </p> <ul> <li> <p> <code>DTYPE</code>: Specifies the data type for the input. When compiling for <code>ml_*</code> (except for <code>ml_inf</code>) instances using PyTorch framework, provide the data type (dtype) of the model's input. <code>\"float32\"</code> is used if <code>\"DTYPE\"</code> is not specified. Options for data type are:</p> <ul> <li> <p>float32: Use either <code>\"float\"</code> or <code>\"float32\"</code>.</p> </li> <li> <p>int64: Use either <code>\"int64\"</code> or <code>\"long\"</code>.</p> </li> </ul> <p> For example, <code>{\"dtype\" : \"float32\"}</code>.</p> </li> <li> <p> <code>CPU</code>: Compilation for CPU supports the following compiler options.</p> <ul> <li> <p> <code>mcpu</code>: CPU micro-architecture. For example, <code>{'mcpu': 'skylake-avx512'}</code> </p> </li> <li> <p> <code>mattr</code>: CPU flags. For example, <code>{'mattr': ['+neon', '+vfpv4']}</code> </p> </li> </ul> </li> <li> <p> <code>ARM</code>: Details of ARM CPU compilations.</p> <ul> <li> <p> <code>NEON</code>: NEON is an implementation of the Advanced SIMD extension used in ARMv7 processors.</p> <p>For example, add <code>{'mattr': ['+neon']}</code> to the compiler options if compiling for ARM 32-bit platform with the NEON support.</p> </li> </ul> </li> <li> <p> <code>NVIDIA</code>: Compilation for NVIDIA GPU supports the following compiler options.</p> <ul> <li> <p> <code>gpu_code</code>: Specifies the targeted architecture.</p> </li> <li> <p> <code>trt-ver</code>: Specifies the TensorRT versions in x.y.z. format.</p> </li> <li> <p> <code>cuda-ver</code>: Specifies the CUDA version in x.y format.</p> </li> </ul> <p>For example, <code>{'gpu-code': 'sm_72', 'trt-ver': '6.0.1', 'cuda-ver': '10.1'}</code> </p> </li> <li> <p> <code>ANDROID</code>: Compilation for the Android OS supports the following compiler options:</p> <ul> <li> <p> <code>ANDROID_PLATFORM</code>: Specifies the Android API levels. Available levels range from 21 to 29. For example, <code>{'ANDROID_PLATFORM': 28}</code>.</p> </li> <li> <p> <code>mattr</code>: Add <code>{'mattr': ['+neon']}</code> to compiler options if compiling for ARM 32-bit platform with NEON support.</p> </li> </ul> </li> <li> <p> <code>INFERENTIA</code>: Compilation for target ml_inf1 uses compiler options passed in as a JSON string. For example, <code>\"CompilerOptions\": \"\\\"--verbose 1 --num-neuroncores 2 -O2\\\"\"</code>. </p> <p>For information about supported compiler options, see <a href=\"https://github.com/aws/aws-neuron-sdk/blob/master/docs/neuron-cc/command-line-reference.md\"> Neuron Compiler CLI</a>. </p> </li> <li> <p> <code>CoreML</code>: Compilation for the CoreML <a>OutputConfig$TargetDevice</a> supports the following compiler options:</p> <ul> <li> <p> <code>class_labels</code>: Specifies the classification labels file name inside input tar.gz file. For example, <code>{\"class_labels\": \"imagenet_labels_1000.txt\"}</code>. Labels inside the txt file should be separated by newlines.</p> </li> </ul> </li> <li> <p> <code>EIA</code>: Compilation for the Elastic Inference Accelerator supports the following compiler options:</p> <ul> <li> <p> <code>precision_mode</code>: Specifies the precision of compiled artifacts. Supported values are <code>\"FP16\"</code> and <code>\"FP32\"</code>. Default is <code>\"FP32\"</code>.</p> </li> <li> <p> <code>signature_def_key</code>: Specifies the signature to use for models in SavedModel format. Defaults is TensorFlow's default signature def key.</p> </li> <li> <p> <code>output_names</code>: Specifies a list of output tensor names for models in FrozenGraph format. Set at most one API field, either: <code>signature_def_key</code> or <code>output_names</code>.</p> </li> </ul> <p>For example: <code>{\"precision_mode\": \"FP32\", \"output_names\": [\"output:0\"]}</code> </p> </li> </ul>",
+                    "documentation": "<p>Specifies additional parameters for compiler options in JSON format. The compiler options are <code>TargetPlatform</code> specific. It is required for NVIDIA accelerators and highly recommended for CPU compilations. For any other cases, it is optional to specify <code>CompilerOptions.</code> </p> <ul> <li> <p> <code>DTYPE</code>: Specifies the data type for the input. When compiling for <code>ml_*</code> (except for <code>ml_inf</code>) instances using PyTorch framework, provide the data type (dtype) of the model's input. <code>\"float32\"</code> is used if <code>\"DTYPE\"</code> is not specified. Options for data type are:</p> <ul> <li> <p>float32: Use either <code>\"float\"</code> or <code>\"float32\"</code>.</p> </li> <li> <p>int64: Use either <code>\"int64\"</code> or <code>\"long\"</code>.</p> </li> </ul> <p> For example, <code>{\"dtype\" : \"float32\"}</code>.</p> </li> <li> <p> <code>CPU</code>: Compilation for CPU supports the following compiler options.</p> <ul> <li> <p> <code>mcpu</code>: CPU micro-architecture. For example, <code>{'mcpu': 'skylake-avx512'}</code> </p> </li> <li> <p> <code>mattr</code>: CPU flags. For example, <code>{'mattr': ['+neon', '+vfpv4']}</code> </p> </li> </ul> </li> <li> <p> <code>ARM</code>: Details of ARM CPU compilations.</p> <ul> <li> <p> <code>NEON</code>: NEON is an implementation of the Advanced SIMD extension used in ARMv7 processors.</p> <p>For example, add <code>{'mattr': ['+neon']}</code> to the compiler options if compiling for ARM 32-bit platform with the NEON support.</p> </li> </ul> </li> <li> <p> <code>NVIDIA</code>: Compilation for NVIDIA GPU supports the following compiler options.</p> <ul> <li> <p> <code>gpu_code</code>: Specifies the targeted architecture.</p> </li> <li> <p> <code>trt-ver</code>: Specifies the TensorRT versions in x.y.z. format.</p> </li> <li> <p> <code>cuda-ver</code>: Specifies the CUDA version in x.y format.</p> </li> </ul> <p>For example, <code>{'gpu-code': 'sm_72', 'trt-ver': '6.0.1', 'cuda-ver': '10.1'}</code> </p> </li> <li> <p> <code>ANDROID</code>: Compilation for the Android OS supports the following compiler options:</p> <ul> <li> <p> <code>ANDROID_PLATFORM</code>: Specifies the Android API levels. Available levels range from 21 to 29. For example, <code>{'ANDROID_PLATFORM': 28}</code>.</p> </li> <li> <p> <code>mattr</code>: Add <code>{'mattr': ['+neon']}</code> to compiler options if compiling for ARM 32-bit platform with NEON support.</p> </li> </ul> </li> <li> <p> <code>INFERENTIA</code>: Compilation for target ml_inf1 uses compiler options passed in as a JSON string. For example, <code>\"CompilerOptions\": \"\\\"--verbose 1 --num-neuroncores 2 -O2\\\"\"</code>. </p> <p>For information about supported compiler options, see <a href=\"https://github.com/aws/aws-neuron-sdk/blob/master/docs/neuron-cc/command-line-reference.md\"> Neuron Compiler CLI</a>. </p> </li> <li> <p> <code>CoreML</code>: Compilation for the CoreML <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_OutputConfig.html\">OutputConfig</a> <code>TargetDevice</code> supports the following compiler options:</p> <ul> <li> <p> <code>class_labels</code>: Specifies the classification labels file name inside input tar.gz file. For example, <code>{\"class_labels\": \"imagenet_labels_1000.txt\"}</code>. Labels inside the txt file should be separated by newlines.</p> </li> </ul> </li> <li> <p> <code>EIA</code>: Compilation for the Elastic Inference Accelerator supports the following compiler options:</p> <ul> <li> <p> <code>precision_mode</code>: Specifies the precision of compiled artifacts. Supported values are <code>\"FP16\"</code> and <code>\"FP32\"</code>. Default is <code>\"FP32\"</code>.</p> </li> <li> <p> <code>signature_def_key</code>: Specifies the signature to use for models in SavedModel format. Defaults is TensorFlow's default signature def key.</p> </li> <li> <p> <code>output_names</code>: Specifies a list of output tensor names for models in FrozenGraph format. Set at most one API field, either: <code>signature_def_key</code> or <code>output_names</code>.</p> </li> </ul> <p>For example: <code>{\"precision_mode\": \"FP32\", \"output_names\": [\"output:0\"]}</code> </p> </li> </ul>",
                     "shape": "CompilerOptions"
                 },
                 "KmsKeyId": {
                     "documentation": "<p>The Amazon Web Services Key Management Service key (Amazon Web Services KMS) that Amazon SageMaker uses to encrypt your output models with Amazon S3 server-side encryption after compilation job. If you don't provide a KMS key ID, Amazon SageMaker uses the default KMS key for Amazon S3 for your role's account. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingKMSEncryption.html\">KMS-Managed Encryption Keys</a> in the <i>Amazon Simple Storage Service Developer Guide.</i> </p> <p>The KmsKeyId can be any of the following formats: </p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias name ARN: <code>arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul>",
                     "shape": "KmsKeyId"
                 },
                 "S3OutputLocation": {
                     "documentation": "<p>Identifies the S3 bucket where you want Amazon SageMaker to store the model artifacts. For example, <code>s3://bucket-name/key-name-prefix</code>.</p>",
                     "shape": "S3Uri"
                 },
                 "TargetDevice": {
-                    "documentation": "<p>Identifies the target device or the machine learning instance that you want to run your model on after the compilation has completed. Alternatively, you can specify OS, architecture, and accelerator using <a>TargetPlatform</a> fields. It can be used instead of <code>TargetPlatform</code>.</p>",
+                    "documentation": "<p>Identifies the target device or the machine learning instance that you want to run your model on after the compilation has completed. Alternatively, you can specify OS, architecture, and accelerator using <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_TargetPlatform.html\">TargetPlatform</a> fields. It can be used instead of <code>TargetPlatform</code>.</p> <note> <p>Currently <code>ml_trn1</code> is available only in US East (N. Virginia) Region, and <code>ml_inf2</code> is available only in US East (Ohio) Region.</p> </note>",
                     "shape": "TargetDevice"
                 },
                 "TargetPlatform": {
                     "documentation": "<p>Contains information about a target platform that you want your model to run on, such as OS, architecture, and accelerators. It is an alternative of <code>TargetDevice</code>.</p> <p>The following examples show how to configure the <code>TargetPlatform</code> and <code>CompilerOptions</code> JSON strings for popular target platforms: </p> <ul> <li> <p>Raspberry Pi 3 Model B+</p> <p> <code>\"TargetPlatform\": {\"Os\": \"LINUX\", \"Arch\": \"ARM_EABIHF\"},</code> </p> <p> <code> \"CompilerOptions\": {'mattr': ['+neon']}</code> </p> </li> <li> <p>Jetson TX2</p> <p> <code>\"TargetPlatform\": {\"Os\": \"LINUX\", \"Arch\": \"ARM64\", \"Accelerator\": \"NVIDIA\"},</code> </p> <p> <code> \"CompilerOptions\": {'gpu-code': 'sm_62', 'trt-ver': '6.0.1', 'cuda-ver': '10.0'}</code> </p> </li> <li> <p>EC2 m5.2xlarge instance OS</p> <p> <code>\"TargetPlatform\": {\"Os\": \"LINUX\", \"Arch\": \"X86_64\", \"Accelerator\": \"NVIDIA\"},</code> </p> <p> <code> \"CompilerOptions\": {'mcpu': 'skylake-avx512'}</code> </p> </li> <li> <p>RK3399</p> <p> <code>\"TargetPlatform\": {\"Os\": \"LINUX\", \"Arch\": \"ARM64\", \"Accelerator\": \"MALI\"}</code> </p> </li> <li> <p>ARMv7 phone (CPU)</p> <p> <code>\"TargetPlatform\": {\"Os\": \"ANDROID\", \"Arch\": \"ARM_EABI\"},</code> </p> <p> <code> \"CompilerOptions\": {'ANDROID_PLATFORM': 25, 'mattr': ['+neon']}</code> </p> </li> <li> <p>ARMv8 phone (CPU)</p> <p> <code>\"TargetPlatform\": {\"Os\": \"ANDROID\", \"Arch\": \"ARM64\"},</code> </p> <p> <code> \"CompilerOptions\": {'ANDROID_PLATFORM': 29}</code> </p> </li> </ul>",
                     "shape": "TargetPlatform"
                 }
             },
@@ -29132,14 +29548,18 @@
                 "S3OutputLocation"
             ],
             "type": "structure"
         },
         "OutputDataConfig": {
             "documentation": "<p>Provides information about how to store model training results (model artifacts).</p>",
             "members": {
+                "CompressionType": {
+                    "documentation": "<p>The model output compression type. Select <code>None</code> to output an uncompressed model, recommended for large model outputs. Defaults to gzip.</p>",
+                    "shape": "OutputCompressionType"
+                },
                 "KmsKeyId": {
                     "documentation": "<p>The Amazon Web Services Key Management Service (Amazon Web Services KMS) key that SageMaker uses to encrypt the model artifacts at rest using Amazon S3 server-side encryption. The <code>KmsKeyId</code> can be any of the following formats: </p> <ul> <li> <p>// KMS Key ID</p> <p> <code>\"1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\"</code> </p> </li> <li> <p>// KMS Key Alias</p> <p> <code>\"alias/ExampleAlias\"</code> </p> </li> <li> <p>// Amazon Resource Name (ARN) of a KMS Key Alias</p> <p> <code>\"arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias\"</code> </p> </li> </ul> <p>If you use a KMS key ID or an alias of your KMS key, the SageMaker execution role must include permissions to call <code>kms:Encrypt</code>. If you don't provide a KMS key ID, SageMaker uses the default KMS key for Amazon S3 for your role's account. SageMaker uses server-side encryption with KMS-managed keys for <code>OutputDataConfig</code>. If you use a bucket policy with an <code>s3:PutObject</code> permission that only allows objects with server-side encryption, set the condition key of <code>s3:x-amz-server-side-encryption</code> to <code>\"aws:kms\"</code>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingKMSEncryption.html\">KMS-Managed Encryption Keys</a> in the <i>Amazon Simple Storage Service Developer Guide.</i> </p> <p>The KMS key policy must grant permission to the IAM role that you specify in your <code>CreateTrainingJob</code>, <code>CreateTransformJob</code>, or <code>CreateHyperParameterTuningJob</code> requests. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html\">Using Key Policies in Amazon Web Services KMS</a> in the <i>Amazon Web Services Key Management Service Developer Guide</i>.</p>",
                     "shape": "KmsKeyId"
                 },
                 "S3OutputPath": {
                     "documentation": "<p>Identifies the S3 path where you want SageMaker to store the model artifacts. For example, <code>s3://bucket-name/key-name-prefix</code>. </p>",
                     "shape": "S3Uri"
@@ -29247,24 +29667,28 @@
                 }
             },
             "type": "structure"
         },
         "ParameterRanges": {
             "documentation": "<p>Specifies ranges of integer, continuous, and categorical hyperparameters that a hyperparameter tuning job searches. The hyperparameter tuning job launches training jobs with hyperparameter values within these ranges to find the combination of values that result in the training job with the best performance as measured by the objective metric of the hyperparameter tuning job.</p> <note> <p>The maximum number of items specified for <code>Array Members</code> refers to the maximum number of hyperparameters for each range and also the maximum for the hyperparameter tuning job itself. That is, the sum of the number of hyperparameters for all the ranges can't exceed the maximum number specified.</p> </note>",
             "members": {
+                "AutoParameters": {
+                    "documentation": "<p>A list containing hyperparameter names and example values to be used by Autotune to determine optimal ranges for your tuning job.</p>",
+                    "shape": "AutoParameters"
+                },
                 "CategoricalParameterRanges": {
-                    "documentation": "<p>The array of <a>CategoricalParameterRange</a> objects that specify ranges of categorical hyperparameters that a hyperparameter tuning job searches.</p>",
+                    "documentation": "<p>The array of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CategoricalParameterRange.html\">CategoricalParameterRange</a> objects that specify ranges of categorical hyperparameters that a hyperparameter tuning job searches.</p>",
                     "shape": "CategoricalParameterRanges"
                 },
                 "ContinuousParameterRanges": {
-                    "documentation": "<p>The array of <a>ContinuousParameterRange</a> objects that specify ranges of continuous hyperparameters that a hyperparameter tuning job searches.</p>",
+                    "documentation": "<p>The array of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ContinuousParameterRange.html\">ContinuousParameterRange</a> objects that specify ranges of continuous hyperparameters that a hyperparameter tuning job searches.</p>",
                     "shape": "ContinuousParameterRanges"
                 },
                 "IntegerParameterRanges": {
-                    "documentation": "<p>The array of <a>IntegerParameterRange</a> objects that specify ranges of integer hyperparameters that a hyperparameter tuning job searches.</p>",
+                    "documentation": "<p>The array of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_IntegerParameterRange.html\">IntegerParameterRange</a> objects that specify ranges of integer hyperparameters that a hyperparameter tuning job searches.</p>",
                     "shape": "IntegerParameterRanges"
                 }
             },
             "type": "structure"
         },
         "ParameterType": {
             "enum": [
@@ -29330,33 +29754,33 @@
             "documentation": "<p>The summary of an in-progress deployment when an endpoint is creating or updating with a new endpoint configuration.</p>",
             "members": {
                 "EndpointConfigName": {
                     "documentation": "<p>The name of the endpoint configuration used in the deployment. </p>",
                     "shape": "EndpointConfigName"
                 },
                 "ProductionVariants": {
-                    "documentation": "<p>An array of <a>PendingProductionVariantSummary</a> objects, one for each model hosted behind this endpoint for the in-progress deployment.</p>",
+                    "documentation": "<p>An array of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_PendingProductionVariantSummary.html\">PendingProductionVariantSummary</a> objects, one for each model hosted behind this endpoint for the in-progress deployment.</p>",
                     "shape": "PendingProductionVariantSummaryList"
                 },
                 "ShadowProductionVariants": {
-                    "documentation": "<p>An array of <a>PendingProductionVariantSummary</a> objects, one for each model hosted behind this endpoint in shadow mode with production traffic replicated from the model specified on <code>ProductionVariants</code> for the in-progress deployment.</p>",
+                    "documentation": "<p>An array of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_PendingProductionVariantSummary.html\">PendingProductionVariantSummary</a> objects, one for each model hosted behind this endpoint in shadow mode with production traffic replicated from the model specified on <code>ProductionVariants</code> for the in-progress deployment.</p>",
                     "shape": "PendingProductionVariantSummaryList"
                 },
                 "StartTime": {
                     "documentation": "<p>The start time of the deployment.</p>",
                     "shape": "Timestamp"
                 }
             },
             "required": [
                 "EndpointConfigName"
             ],
             "type": "structure"
         },
         "PendingProductionVariantSummary": {
-            "documentation": "<p>The production variant summary for a deployment when an endpoint is creating or updating with the <code> <a>CreateEndpoint</a> </code> or <code> <a>UpdateEndpoint</a> </code> operations. Describes the <code>VariantStatus </code>, weight and capacity for a production variant associated with an endpoint. </p>",
+            "documentation": "<p>The production variant summary for a deployment when an endpoint is creating or updating with the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpoint.html\">CreateEndpoint</a> or <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateEndpoint.html\">UpdateEndpoint</a> operations. Describes the <code>VariantStatus </code>, weight and capacity for a production variant associated with an endpoint. </p>",
             "members": {
                 "AcceleratorType": {
                     "documentation": "<p>The size of the Elastic Inference (EI) instance to use for the production variant. EI instances provide on-demand GPU computing for inference. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/ei.html\">Using Elastic Inference in Amazon SageMaker</a>.</p>",
                     "shape": "ProductionVariantAcceleratorType"
                 },
                 "CurrentInstanceCount": {
                     "documentation": "<p>The number of instances associated with the variant.</p>",
@@ -29371,23 +29795,23 @@
                     "shape": "VariantWeight"
                 },
                 "DeployedImages": {
                     "documentation": "<p>An array of <code>DeployedImage</code> objects that specify the Amazon EC2 Container Registry paths of the inference images deployed on instances of this <code>ProductionVariant</code>.</p>",
                     "shape": "DeployedImages"
                 },
                 "DesiredInstanceCount": {
-                    "documentation": "<p>The number of instances requested in this deployment, as specified in the endpoint configuration for the endpoint. The value is taken from the request to the <code> <a>CreateEndpointConfig</a> </code> operation.</p>",
+                    "documentation": "<p>The number of instances requested in this deployment, as specified in the endpoint configuration for the endpoint. The value is taken from the request to the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpointConfig.html\">CreateEndpointConfig</a> operation.</p>",
                     "shape": "TaskCount"
                 },
                 "DesiredServerlessConfig": {
                     "documentation": "<p>The serverless configuration requested for this deployment, as specified in the endpoint configuration for the endpoint.</p>",
                     "shape": "ProductionVariantServerlessConfig"
                 },
                 "DesiredWeight": {
-                    "documentation": "<p>The requested weight for the variant in this deployment, as specified in the endpoint configuration for the endpoint. The value is taken from the request to the <code> <a>CreateEndpointConfig</a> </code> operation.</p>",
+                    "documentation": "<p>The requested weight for the variant in this deployment, as specified in the endpoint configuration for the endpoint. The value is taken from the request to the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpointConfig.html\">CreateEndpointConfig</a> operation.</p>",
                     "shape": "VariantWeight"
                 },
                 "InstanceType": {
                     "documentation": "<p>The type of instances associated with the variant.</p>",
                     "shape": "ProductionVariantInstanceType"
                 },
                 "VariantName": {
@@ -29582,14 +30006,18 @@
                 },
                 "PipelineExperimentConfig": {
                     "shape": "PipelineExperimentConfig"
                 },
                 "PipelineParameters": {
                     "documentation": "<p>Contains a list of pipeline parameters. This list can be empty. </p>",
                     "shape": "ParameterList"
+                },
+                "SelectiveExecutionConfig": {
+                    "documentation": "<p>The selective execution configuration applied to the pipeline run.</p>",
+                    "shape": "SelectiveExecutionConfig"
                 }
             },
             "type": "structure"
         },
         "PipelineExecutionArn": {
             "max": 256,
             "pattern": "^arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:pipeline\\/.*\\/execution\\/.*$",
@@ -29641,14 +30069,18 @@
                     "documentation": "<p>The reason why the step failed execution. This is only returned if the step failed its execution.</p>",
                     "shape": "FailureReason"
                 },
                 "Metadata": {
                     "documentation": "<p>Metadata to run the pipeline step.</p>",
                     "shape": "PipelineExecutionStepMetadata"
                 },
+                "SelectiveExecutionResult": {
+                    "documentation": "<p>The ARN from an execution of the current pipeline from which results are reused for this step.</p>",
+                    "shape": "SelectiveExecutionResult"
+                },
                 "StartTime": {
                     "documentation": "<p>The time that the step started executing.</p>",
                     "shape": "Timestamp"
                 },
                 "StepDescription": {
                     "documentation": "<p>The description of the step.</p>",
                     "shape": "StepDescription"
@@ -30631,15 +31063,21 @@
                 "ml.r6gd.large",
                 "ml.r6gd.xlarge",
                 "ml.r6gd.2xlarge",
                 "ml.r6gd.4xlarge",
                 "ml.r6gd.8xlarge",
                 "ml.r6gd.12xlarge",
                 "ml.r6gd.16xlarge",
-                "ml.p4de.24xlarge"
+                "ml.p4de.24xlarge",
+                "ml.trn1.2xlarge",
+                "ml.trn1.32xlarge",
+                "ml.inf2.xlarge",
+                "ml.inf2.8xlarge",
+                "ml.inf2.24xlarge",
+                "ml.inf2.48xlarge"
             ],
             "type": "string"
         },
         "ProductionVariantList": {
             "max": 10,
             "member": {
                 "shape": "ProductionVariant"
@@ -30661,22 +31099,40 @@
                 "MaxConcurrency": {
                     "documentation": "<p>The maximum number of concurrent invocations your serverless endpoint can process.</p>",
                     "shape": "ServerlessMaxConcurrency"
                 },
                 "MemorySizeInMB": {
                     "documentation": "<p>The memory size of your serverless endpoint. Valid values are in 1 GB increments: 1024 MB, 2048 MB, 3072 MB, 4096 MB, 5120 MB, or 6144 MB.</p>",
                     "shape": "ServerlessMemorySizeInMB"
+                },
+                "ProvisionedConcurrency": {
+                    "documentation": "<p>The amount of provisioned concurrency to allocate for the serverless endpoint. Should be less than or equal to <code>MaxConcurrency</code>.</p> <note> <p>This field is not supported for serverless endpoint recommendations for Inference Recommender jobs. For more information about creating an Inference Recommender job, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateInferenceRecommendationsJob.html\">CreateInferenceRecommendationsJobs</a>.</p> </note>",
+                    "shape": "ServerlessProvisionedConcurrency"
                 }
             },
             "required": [
                 "MemorySizeInMB",
                 "MaxConcurrency"
             ],
             "type": "structure"
         },
+        "ProductionVariantServerlessUpdateConfig": {
+            "documentation": "<p>Specifies the serverless update concurrency configuration for an endpoint variant.</p>",
+            "members": {
+                "MaxConcurrency": {
+                    "documentation": "<p>The updated maximum number of concurrent invocations your serverless endpoint can process.</p>",
+                    "shape": "ServerlessMaxConcurrency"
+                },
+                "ProvisionedConcurrency": {
+                    "documentation": "<p>The updated amount of provisioned concurrency to allocate for the serverless endpoint. Should be less than or equal to <code>MaxConcurrency</code>.</p>",
+                    "shape": "ServerlessProvisionedConcurrency"
+                }
+            },
+            "type": "structure"
+        },
         "ProductionVariantStatus": {
             "documentation": "<p>Describes the status of the production variant.</p>",
             "members": {
                 "StartTime": {
                     "documentation": "<p>The start time of the current status change.</p>",
                     "shape": "Timestamp"
                 },
@@ -31347,15 +31803,15 @@
             "enum": [
                 "ENABLED",
                 "DISABLED"
             ],
             "type": "string"
         },
         "RStudioServerProAppSettings": {
-            "documentation": "<p>A collection of settings that configure user interaction with the <code>RStudioServerPro</code> app. <code>RStudioServerProAppSettings</code> cannot be updated. The <code>RStudioServerPro</code> app must be deleted and a new one created to make any changes.</p>",
+            "documentation": "<p>A collection of settings that configure user interaction with the <code>RStudioServerPro</code> app.</p>",
             "members": {
                 "AccessStatus": {
                     "documentation": "<p>Indicates whether the current user has access to the <code>RStudioServerPro</code> app.</p>",
                     "shape": "RStudioServerProAccessStatus"
                 },
                 "UserGroup": {
                     "documentation": "<p>The level of permissions that the user has within the <code>RStudioServerPro</code> app. This value defaults to `User`. The `Admin` value allows the user access to the RStudio Administrative Dashboard.</p>",
@@ -31437,14 +31893,44 @@
             },
             "required": [
                 "InstanceType",
                 "InstanceCount"
             ],
             "type": "structure"
         },
+        "RealTimeInferenceRecommendation": {
+            "documentation": "<p>The recommended configuration to use for Real-Time Inference.</p>",
+            "members": {
+                "Environment": {
+                    "documentation": "<p>The recommended environment variables to set in the model container for Real-Time Inference.</p>",
+                    "shape": "EnvironmentMap"
+                },
+                "InstanceType": {
+                    "documentation": "<p>The recommended instance type for Real-Time Inference.</p>",
+                    "shape": "ProductionVariantInstanceType"
+                },
+                "RecommendationId": {
+                    "documentation": "<p>The recommendation ID which uniquely identifies each recommendation.</p>",
+                    "shape": "String"
+                }
+            },
+            "required": [
+                "RecommendationId",
+                "InstanceType"
+            ],
+            "type": "structure"
+        },
+        "RealTimeInferenceRecommendations": {
+            "max": 3,
+            "member": {
+                "shape": "RealTimeInferenceRecommendation"
+            },
+            "min": 0,
+            "type": "list"
+        },
         "RealtimeInferenceInstanceTypes": {
             "member": {
                 "shape": "ProductionVariantInstanceType"
             },
             "type": "list"
         },
         "RecommendationFailureReason": {
@@ -31494,14 +31980,18 @@
                     "documentation": "<p>The name of a pre-trained machine learning model benchmarked by Amazon SageMaker Inference Recommender that matches your model.</p> <p>Valid Values: <code>efficientnetb7 | unet | xgboost | faster-rcnn-resnet101 | nasnetlarge | vgg16 | inception-v3 | mask-rcnn | sagemaker-scikit-learn | densenet201-gluon | resnet18v2-gluon | xception | densenet201 | yolov4 | resnet152 | bert-base-cased | xceptionV1-keras | resnet50 | retinanet</code> </p>",
                     "shape": "String"
                 },
                 "PayloadConfig": {
                     "documentation": "<p>Specifies the <code>SamplePayloadUrl</code> and all other sample payload-related fields.</p>",
                     "shape": "RecommendationJobPayloadConfig"
                 },
+                "SupportedEndpointType": {
+                    "documentation": "<p>The endpoint type to receive recommendations for. By default this is null, and the results of the inference recommendation job return a combined list of both real-time and serverless benchmarks. By specifying a value for this field, you can receive a longer list of benchmarks for the desired endpoint type.</p>",
+                    "shape": "RecommendationJobSupportedEndpointType"
+                },
                 "SupportedInstanceTypes": {
                     "documentation": "<p>A list of the instance types that are used to generate inferences in real-time.</p>",
                     "shape": "RecommendationJobSupportedInstanceTypes"
                 },
                 "Task": {
                     "documentation": "<p>The machine learning task that the model accomplishes.</p> <p>Valid Values: <code>IMAGE_CLASSIFICATION | OBJECT_DETECTION | TEXT_GENERATION | IMAGE_SEGMENTATION | FILL_MASK | CLASSIFICATION | REGRESSION | OTHER</code> </p>",
                     "shape": "String"
@@ -31528,14 +32018,22 @@
                 "EndpointMetrics": {
                     "shape": "InferenceMetrics"
                 },
                 "FailureReason": {
                     "documentation": "<p>The reason why a benchmark failed.</p>",
                     "shape": "RecommendationFailureReason"
                 },
+                "InvocationEndTime": {
+                    "documentation": "<p>A timestamp that shows when the benchmark completed.</p>",
+                    "shape": "InvocationEndTime"
+                },
+                "InvocationStartTime": {
+                    "documentation": "<p>A timestamp that shows when the benchmark started.</p>",
+                    "shape": "InvocationStartTime"
+                },
                 "Metrics": {
                     "shape": "RecommendationMetrics"
                 },
                 "ModelConfiguration": {
                     "shape": "ModelConfiguration"
                 }
             },
@@ -31665,14 +32163,21 @@
         },
         "RecommendationJobSupportedContentTypes": {
             "member": {
                 "shape": "String"
             },
             "type": "list"
         },
+        "RecommendationJobSupportedEndpointType": {
+            "enum": [
+                "RealTime",
+                "Serverless"
+            ],
+            "type": "string"
+        },
         "RecommendationJobSupportedInstanceTypes": {
             "member": {
                 "shape": "String"
             },
             "type": "list"
         },
         "RecommendationJobType": {
@@ -31748,24 +32253,37 @@
                 "MemoryUtilization": {
                     "documentation": "<p>The expected memory utilization at maximum invocations per minute for the instance.</p> <p> <code>NaN</code> indicates that the value is not available.</p>",
                     "shape": "UtilizationMetric"
                 },
                 "ModelLatency": {
                     "documentation": "<p>The expected model latency at maximum invocation per minute for the instance.</p>",
                     "shape": "Integer"
+                },
+                "ModelSetupTime": {
+                    "documentation": "<p>The time it takes to launch new compute resources for a serverless endpoint. The time can vary depending on the model size, how long it takes to download the model, and the start-up time of the container.</p> <p> <code>NaN</code> indicates that the value is not available.</p>",
+                    "shape": "ModelSetupTime"
                 }
             },
             "required": [
                 "CostPerHour",
                 "CostPerInference",
                 "MaxInvocations",
                 "ModelLatency"
             ],
             "type": "structure"
         },
+        "RecommendationStatus": {
+            "enum": [
+                "IN_PROGRESS",
+                "COMPLETED",
+                "FAILED",
+                "NOT_APPLICABLE"
+            ],
+            "type": "string"
+        },
         "RecommendationStepType": {
             "enum": [
                 "BENCHMARK"
             ],
             "type": "string"
         },
         "RecordWrapper": {
@@ -31903,15 +32421,15 @@
             "min": 1,
             "pattern": ".*",
             "type": "string"
         },
         "RenderUiTemplateRequest": {
             "members": {
                 "HumanTaskUiArn": {
-                    "documentation": "<p>The <code>HumanTaskUiArn</code> of the worker UI that you want to render. Do not provide a <code>HumanTaskUiArn</code> if you use the <code>UiTemplate</code> parameter.</p> <p>See a list of available Human Ui Amazon Resource Names (ARNs) in <a>UiConfig</a>.</p>",
+                    "documentation": "<p>The <code>HumanTaskUiArn</code> of the worker UI that you want to render. Do not provide a <code>HumanTaskUiArn</code> if you use the <code>UiTemplate</code> parameter.</p> <p>See a list of available Human Ui Amazon Resource Names (ARNs) in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UiConfig.html\">UiConfig</a>.</p>",
                     "shape": "HumanTaskUiArn"
                 },
                 "RoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) that has access to the S3 objects that are used by the template.</p>",
                     "shape": "RoleArn"
                 },
                 "Task": {
@@ -32267,14 +32785,38 @@
         },
         "RoleArn": {
             "max": 2048,
             "min": 20,
             "pattern": "^arn:aws[a-z\\-]*:iam::\\d{12}:role/?[a-zA-Z_0-9+=,.@\\-_/]+$",
             "type": "string"
         },
+        "RollingUpdatePolicy": {
+            "documentation": "<p>Specifies a rolling deployment strategy for updating a SageMaker endpoint.</p>",
+            "members": {
+                "MaximumBatchSize": {
+                    "shape": "CapacitySize"
+                },
+                "MaximumExecutionTimeoutInSeconds": {
+                    "documentation": "<p>The time limit for the total deployment. Exceeding this limit causes a timeout.</p>",
+                    "shape": "MaximumExecutionTimeoutInSeconds"
+                },
+                "RollbackMaximumBatchSize": {
+                    "shape": "CapacitySize"
+                },
+                "WaitIntervalInSeconds": {
+                    "documentation": "<p>The length of the baking period, during which SageMaker monitors alarms for each batch on the new fleet.</p>",
+                    "shape": "WaitIntervalInSeconds"
+                }
+            },
+            "required": [
+                "MaximumBatchSize",
+                "WaitIntervalInSeconds"
+            ],
+            "type": "structure"
+        },
         "RootAccess": {
             "enum": [
                 "Enabled",
                 "Disabled"
             ],
             "type": "string"
         },
@@ -32310,15 +32852,15 @@
             "enum": [
                 "FullyReplicated",
                 "ShardedByS3Key"
             ],
             "type": "string"
         },
         "S3DataSource": {
-            "documentation": "<p>Describes the S3 data source.</p>",
+            "documentation": "<p>Describes the S3 data source.</p> <p>Your input bucket must be in the same Amazon Web Services region as your training job.</p>",
             "members": {
                 "AttributeNames": {
                     "documentation": "<p>A list of one or more attribute names to use that are found in a specified augmented manifest file.</p>",
                     "shape": "AttributeNames"
                 },
                 "InstanceGroupNames": {
                     "documentation": "<p>A list of names of instance groups that get data from the S3 data source.</p>",
@@ -32329,15 +32871,15 @@
                     "shape": "S3DataDistribution"
                 },
                 "S3DataType": {
                     "documentation": "<p>If you choose <code>S3Prefix</code>, <code>S3Uri</code> identifies a key name prefix. SageMaker uses all objects that match the specified key name prefix for model training. </p> <p>If you choose <code>ManifestFile</code>, <code>S3Uri</code> identifies an object that is a manifest file containing a list of object keys that you want SageMaker to use for model training. </p> <p>If you choose <code>AugmentedManifestFile</code>, S3Uri identifies an object that is an augmented manifest file in JSON lines format. This file contains the data you want to use for model training. <code>AugmentedManifestFile</code> can only be used if the Channel's input mode is <code>Pipe</code>.</p>",
                     "shape": "S3DataType"
                 },
                 "S3Uri": {
-                    "documentation": "<p>Depending on the value specified for the <code>S3DataType</code>, identifies either a key name prefix or a manifest. For example: </p> <ul> <li> <p> A key name prefix might look like this: <code>s3://bucketname/exampleprefix</code> </p> </li> <li> <p> A manifest might look like this: <code>s3://bucketname/example.manifest</code> </p> <p> A manifest is an S3 object which is a JSON file consisting of an array of elements. The first element is a prefix which is followed by one or more suffixes. SageMaker appends the suffix elements to the prefix to get a full set of <code>S3Uri</code>. Note that the prefix must be a valid non-empty <code>S3Uri</code> that precludes users from specifying a manifest whose individual <code>S3Uri</code> is sourced from different S3 buckets.</p> <p> The following code example shows a valid manifest format: </p> <p> <code>[ {\"prefix\": \"s3://customer_bucket/some/prefix/\"},</code> </p> <p> <code> \"relative/path/to/custdata-1\",</code> </p> <p> <code> \"relative/path/custdata-2\",</code> </p> <p> <code> ...</code> </p> <p> <code> \"relative/path/custdata-N\"</code> </p> <p> <code>]</code> </p> <p> This JSON is equivalent to the following <code>S3Uri</code> list:</p> <p> <code>s3://customer_bucket/some/prefix/relative/path/to/custdata-1</code> </p> <p> <code>s3://customer_bucket/some/prefix/relative/path/custdata-2</code> </p> <p> <code>...</code> </p> <p> <code>s3://customer_bucket/some/prefix/relative/path/custdata-N</code> </p> <p>The complete set of <code>S3Uri</code> in this manifest is the input data for the channel for this data source. The object that each <code>S3Uri</code> points to must be readable by the IAM role that SageMaker uses to perform tasks on your behalf. </p> </li> </ul>",
+                    "documentation": "<p>Depending on the value specified for the <code>S3DataType</code>, identifies either a key name prefix or a manifest. For example: </p> <ul> <li> <p> A key name prefix might look like this: <code>s3://bucketname/exampleprefix</code> </p> </li> <li> <p> A manifest might look like this: <code>s3://bucketname/example.manifest</code> </p> <p> A manifest is an S3 object which is a JSON file consisting of an array of elements. The first element is a prefix which is followed by one or more suffixes. SageMaker appends the suffix elements to the prefix to get a full set of <code>S3Uri</code>. Note that the prefix must be a valid non-empty <code>S3Uri</code> that precludes users from specifying a manifest whose individual <code>S3Uri</code> is sourced from different S3 buckets.</p> <p> The following code example shows a valid manifest format: </p> <p> <code>[ {\"prefix\": \"s3://customer_bucket/some/prefix/\"},</code> </p> <p> <code> \"relative/path/to/custdata-1\",</code> </p> <p> <code> \"relative/path/custdata-2\",</code> </p> <p> <code> ...</code> </p> <p> <code> \"relative/path/custdata-N\"</code> </p> <p> <code>]</code> </p> <p> This JSON is equivalent to the following <code>S3Uri</code> list:</p> <p> <code>s3://customer_bucket/some/prefix/relative/path/to/custdata-1</code> </p> <p> <code>s3://customer_bucket/some/prefix/relative/path/custdata-2</code> </p> <p> <code>...</code> </p> <p> <code>s3://customer_bucket/some/prefix/relative/path/custdata-N</code> </p> <p>The complete set of <code>S3Uri</code> in this manifest is the input data for the channel for this data source. The object that each <code>S3Uri</code> points to must be readable by the IAM role that SageMaker uses to perform tasks on your behalf. </p> </li> </ul> <p>Your input bucket must be located in same Amazon Web Services region as your training job.</p>",
                     "shape": "S3Uri"
                 }
             },
             "required": [
                 "S3DataType",
                 "S3Uri"
             ],
@@ -32347,14 +32889,49 @@
             "enum": [
                 "ManifestFile",
                 "S3Prefix",
                 "AugmentedManifestFile"
             ],
             "type": "string"
         },
+        "S3ModelDataSource": {
+            "documentation": "<p>Specifies the S3 location of ML model data to deploy.</p>",
+            "members": {
+                "CompressionType": {
+                    "documentation": "<p>Specifies how the ML model data is prepared.</p> <p>If you choose <code>Gzip</code> and choose <code>S3Object</code> as the value of <code>S3DataType</code>, <code>S3Uri</code> identifies an object that is a gzip-compressed TAR archive. SageMaker will attempt to decompress and untar the object during model deployment.</p> <p>If you choose <code>None</code> and chooose <code>S3Object</code> as the value of <code>S3DataType</code>, <code>S3Uri</code> identifies an object that represents an uncompressed ML model to deploy.</p> <p>If you choose None and choose <code>S3Prefix</code> as the value of <code>S3DataType</code>, <code>S3Uri</code> identifies a key name prefix, under which all objects represents the uncompressed ML model to deploy.</p> <p>If you choose None, then SageMaker will follow rules below when creating model data files under /opt/ml/model directory for use by your inference code:</p> <ul> <li> <p>If you choose <code>S3Object</code> as the value of <code>S3DataType</code>, then SageMaker will split the key of the S3 object referenced by <code>S3Uri</code> by slash (/), and use the last part as the filename of the file holding the content of the S3 object.</p> </li> <li> <p>If you choose <code>S3Prefix</code> as the value of <code>S3DataType</code>, then for each S3 object under the key name pefix referenced by <code>S3Uri</code>, SageMaker will trim its key by the prefix, and use the remainder as the path (relative to <code>/opt/ml/model</code>) of the file holding the content of the S3 object. SageMaker will split the remainder by slash (/), using intermediate parts as directory names and the last part as filename of the file holding the content of the S3 object.</p> </li> <li> <p>Do not use any of the following as file names or directory names:</p> <ul> <li> <p>An empty or blank string</p> </li> <li> <p>A string which contains null bytes</p> </li> <li> <p>A string longer than 255 bytes</p> </li> <li> <p>A single dot (<code>.</code>)</p> </li> <li> <p>A double dot (<code>..</code>)</p> </li> </ul> </li> <li> <p>Ambiguous file names will result in model deployment failure. For example, if your uncompressed ML model consists of two S3 objects <code>s3://mybucket/model/weights</code> and <code>s3://mybucket/model/weights/part1</code> and you specify <code>s3://mybucket/model/</code> as the value of <code>S3Uri</code> and <code>S3Prefix</code> as the value of <code>S3DataType</code>, then it will result in name clash between <code>/opt/ml/model/weights</code> (a regular file) and <code>/opt/ml/model/weights/</code> (a directory).</p> </li> <li> <p>Do not organize the model artifacts in <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/using-folders.html\">S3 console using folders</a>. When you create a folder in S3 console, S3 creates a 0-byte object with a key set to the folder name you provide. They key of the 0-byte object ends with a slash (/) which violates SageMaker restrictions on model artifact file names, leading to model deployment failure. </p> </li> </ul>",
+                    "shape": "ModelCompressionType"
+                },
+                "S3DataType": {
+                    "documentation": "<p>Specifies the type of ML model data to deploy.</p> <p>If you choose <code>S3Prefix</code>, <code>S3Uri</code> identifies a key name prefix. SageMaker uses all objects that match the specified key name prefix as part of the ML model data to deploy. A valid key name prefix identified by <code>S3Uri</code> always ends with a forward slash (/).</p> <p>If you choose <code>S3Object</code>, <code>S3Uri</code> identifies an object that is the ML model data to deploy.</p>",
+                    "shape": "S3ModelDataType"
+                },
+                "S3Uri": {
+                    "documentation": "<p>Specifies the S3 path of ML model data to deploy.</p>",
+                    "shape": "S3ModelUri"
+                }
+            },
+            "required": [
+                "S3Uri",
+                "S3DataType",
+                "CompressionType"
+            ],
+            "type": "structure"
+        },
+        "S3ModelDataType": {
+            "enum": [
+                "S3Prefix",
+                "S3Object"
+            ],
+            "type": "string"
+        },
+        "S3ModelUri": {
+            "max": 1024,
+            "pattern": "^(https|s3)://([^/]+)/?(.*)$",
+            "type": "string"
+        },
         "S3OutputPath": {
             "max": 1024,
             "pattern": "^(https|s3)://([^/]+)/?(.*)$",
             "type": "string"
         },
         "S3StorageConfig": {
             "documentation": "<p>The Amazon Simple Storage (Amazon S3) location and and security configuration for <code>OfflineStore</code>.</p>",
@@ -32397,14 +32974,20 @@
         "SagemakerServicecatalogStatus": {
             "enum": [
                 "Enabled",
                 "Disabled"
             ],
             "type": "string"
         },
+        "SampleWeightAttributeName": {
+            "max": 256,
+            "min": 1,
+            "pattern": "^[a-zA-Z0-9_-]+$",
+            "type": "string"
+        },
         "SamplingPercentage": {
             "max": 100,
             "min": 0,
             "type": "integer"
         },
         "ScheduleConfig": {
             "documentation": "<p>Configuration details about the monitoring schedule.</p>",
@@ -32460,15 +33043,15 @@
             "member": {
                 "shape": "SearchExpression"
             },
             "min": 1,
             "type": "list"
         },
         "SearchRecord": {
-            "documentation": "<p>A single resource returned as part of the <a>Search</a> API response.</p>",
+            "documentation": "<p>A single resource returned as part of the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API response.</p>",
             "members": {
                 "Endpoint": {
                     "shape": "Endpoint"
                 },
                 "Experiment": {
                     "documentation": "<p>The properties of an experiment.</p>",
                     "shape": "Experiment"
@@ -32599,30 +33182,30 @@
                 "MaxWaitTimeExceeded",
                 "Updating",
                 "Restarting"
             ],
             "type": "string"
         },
         "SecondaryStatusTransition": {
-            "documentation": "<p>An array element of <a>DescribeTrainingJobResponse$SecondaryStatusTransitions</a>. It provides additional details about a status that the training job has transitioned through. A training job can be in one of several states, for example, starting, downloading, training, or uploading. Within each state, there are a number of intermediate states. For example, within the starting state, SageMaker could be starting the training job or launching the ML instances. These transitional states are referred to as the job's secondary status. </p> <p/>",
+            "documentation": "<p>An array element of <code>SecondaryStatusTransitions</code> for <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeTrainingJob.html\">DescribeTrainingJob</a>. It provides additional details about a status that the training job has transitioned through. A training job can be in one of several states, for example, starting, downloading, training, or uploading. Within each state, there are a number of intermediate states. For example, within the starting state, SageMaker could be starting the training job or launching the ML instances. These transitional states are referred to as the job's secondary status. </p> <p/>",
             "members": {
                 "EndTime": {
                     "documentation": "<p>A timestamp that shows when the training job transitioned out of this secondary status state into another secondary status state or when the training job has ended.</p>",
                     "shape": "Timestamp"
                 },
                 "StartTime": {
                     "documentation": "<p>A timestamp that shows when the training job transitioned to the current secondary status state.</p>",
                     "shape": "Timestamp"
                 },
                 "Status": {
                     "documentation": "<p>Contains a secondary status information from a training job.</p> <p>Status might be one of the following secondary statuses:</p> <dl> <dt>InProgress</dt> <dd> <ul> <li> <p> <code>Starting</code> - Starting the training job.</p> </li> <li> <p> <code>Downloading</code> - An optional stage for algorithms that support <code>File</code> training input mode. It indicates that data is being downloaded to the ML storage volumes.</p> </li> <li> <p> <code>Training</code> - Training is in progress.</p> </li> <li> <p> <code>Uploading</code> - Training is complete and the model artifacts are being uploaded to the S3 location.</p> </li> </ul> </dd> <dt>Completed</dt> <dd> <ul> <li> <p> <code>Completed</code> - The training job has completed.</p> </li> </ul> </dd> <dt>Failed</dt> <dd> <ul> <li> <p> <code>Failed</code> - The training job has failed. The reason for the failure is returned in the <code>FailureReason</code> field of <code>DescribeTrainingJobResponse</code>.</p> </li> </ul> </dd> <dt>Stopped</dt> <dd> <ul> <li> <p> <code>MaxRuntimeExceeded</code> - The job stopped because it exceeded the maximum allowed runtime.</p> </li> <li> <p> <code>Stopped</code> - The training job has stopped.</p> </li> </ul> </dd> <dt>Stopping</dt> <dd> <ul> <li> <p> <code>Stopping</code> - Stopping the training job.</p> </li> </ul> </dd> </dl> <p>We no longer support the following secondary statuses:</p> <ul> <li> <p> <code>LaunchingMLInstances</code> </p> </li> <li> <p> <code>PreparingTrainingStack</code> </p> </li> <li> <p> <code>DownloadingTrainingImage</code> </p> </li> </ul>",
                     "shape": "SecondaryStatus"
                 },
                 "StatusMessage": {
-                    "documentation": "<p>A detailed description of the progress within a secondary status. </p> <p>SageMaker provides secondary statuses and status messages that apply to each of them:</p> <dl> <dt>Starting</dt> <dd> <ul> <li> <p>Starting the training job.</p> </li> <li> <p>Launching requested ML instances.</p> </li> <li> <p>Insufficient capacity error from EC2 while launching instances, retrying!</p> </li> <li> <p>Launched instance was unhealthy, replacing it!</p> </li> <li> <p>Preparing the instances for training.</p> </li> </ul> </dd> <dt>Training</dt> <dd> <ul> <li> <p>Downloading the training image.</p> </li> <li> <p>Training image download completed. Training in progress.</p> </li> </ul> </dd> </dl> <important> <p>Status messages are subject to change. Therefore, we recommend not including them in code that programmatically initiates actions. For examples, don't use status messages in if statements.</p> </important> <p>To have an overview of your training job's progress, view <code>TrainingJobStatus</code> and <code>SecondaryStatus</code> in <a>DescribeTrainingJob</a>, and <code>StatusMessage</code> together. For example, at the start of a training job, you might see the following:</p> <ul> <li> <p> <code>TrainingJobStatus</code> - InProgress</p> </li> <li> <p> <code>SecondaryStatus</code> - Training</p> </li> <li> <p> <code>StatusMessage</code> - Downloading the training image</p> </li> </ul>",
+                    "documentation": "<p>A detailed description of the progress within a secondary status. </p> <p>SageMaker provides secondary statuses and status messages that apply to each of them:</p> <dl> <dt>Starting</dt> <dd> <ul> <li> <p>Starting the training job.</p> </li> <li> <p>Launching requested ML instances.</p> </li> <li> <p>Insufficient capacity error from EC2 while launching instances, retrying!</p> </li> <li> <p>Launched instance was unhealthy, replacing it!</p> </li> <li> <p>Preparing the instances for training.</p> </li> </ul> </dd> <dt>Training</dt> <dd> <ul> <li> <p>Downloading the training image.</p> </li> <li> <p>Training image download completed. Training in progress.</p> </li> </ul> </dd> </dl> <important> <p>Status messages are subject to change. Therefore, we recommend not including them in code that programmatically initiates actions. For examples, don't use status messages in if statements.</p> </important> <p>To have an overview of your training job's progress, view <code>TrainingJobStatus</code> and <code>SecondaryStatus</code> in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeTrainingJob.html\">DescribeTrainingJob</a>, and <code>StatusMessage</code> together. For example, at the start of a training job, you might see the following:</p> <ul> <li> <p> <code>TrainingJobStatus</code> - InProgress</p> </li> <li> <p> <code>SecondaryStatus</code> - Training</p> </li> <li> <p> <code>StatusMessage</code> - Downloading the training image</p> </li> </ul>",
                     "shape": "StatusMessage"
                 }
             },
             "required": [
                 "Status",
                 "StartTime"
             ],
@@ -32651,14 +33234,63 @@
                 "shape": "SecurityGroupId"
             },
             "type": "list"
         },
         "Seed": {
             "type": "long"
         },
+        "SelectedStep": {
+            "documentation": "<p>A step selected to run in selective execution mode.</p>",
+            "members": {
+                "StepName": {
+                    "documentation": "<p>The name of the pipeline step.</p>",
+                    "shape": "String256"
+                }
+            },
+            "required": [
+                "StepName"
+            ],
+            "type": "structure"
+        },
+        "SelectedStepList": {
+            "max": 50,
+            "member": {
+                "shape": "SelectedStep"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "SelectiveExecutionConfig": {
+            "documentation": "<p>The selective execution configuration applied to the pipeline run.</p>",
+            "members": {
+                "SelectedSteps": {
+                    "documentation": "<p>A list of pipeline steps to run. All step(s) in all path(s) between two selected steps should be included.</p>",
+                    "shape": "SelectedStepList"
+                },
+                "SourcePipelineExecutionArn": {
+                    "documentation": "<p>The ARN from a reference execution of the current pipeline. Used to copy input collaterals needed for the selected steps to run. The execution status of the pipeline can be either <code>Failed</code> or <code>Success</code>.</p>",
+                    "shape": "PipelineExecutionArn"
+                }
+            },
+            "required": [
+                "SourcePipelineExecutionArn",
+                "SelectedSteps"
+            ],
+            "type": "structure"
+        },
+        "SelectiveExecutionResult": {
+            "documentation": "<p>The ARN from an execution of the current pipeline.</p>",
+            "members": {
+                "SourcePipelineExecutionArn": {
+                    "documentation": "<p>The ARN from an execution of the current pipeline.</p>",
+                    "shape": "PipelineExecutionArn"
+                }
+            },
+            "type": "structure"
+        },
         "SendPipelineExecutionStepFailureRequest": {
             "members": {
                 "CallbackToken": {
                     "documentation": "<p>The pipeline generated token from the Amazon SQS queue.</p>",
                     "shape": "CallbackToken"
                 },
                 "ClientRequestToken": {
@@ -32721,14 +33353,19 @@
             "type": "integer"
         },
         "ServerlessMemorySizeInMB": {
             "max": 6144,
             "min": 1024,
             "type": "integer"
         },
+        "ServerlessProvisionedConcurrency": {
+            "max": 200,
+            "min": 1,
+            "type": "integer"
+        },
         "ServiceCatalogEntityId": {
             "max": 100,
             "min": 1,
             "pattern": "^[a-zA-Z0-9_\\-]*",
             "type": "string"
         },
         "ServiceCatalogProvisionedProductDetails": {
@@ -32972,15 +33609,15 @@
             "documentation": "<p>Specifies an algorithm that was used to create the model package. The algorithm must be either an algorithm resource in your SageMaker account or an algorithm in Amazon Web Services Marketplace that you are subscribed to.</p>",
             "members": {
                 "AlgorithmName": {
                     "documentation": "<p>The name of an algorithm that was used to create the model package. The algorithm must be either an algorithm resource in your SageMaker account or an algorithm in Amazon Web Services Marketplace that you are subscribed to.</p>",
                     "shape": "ArnOrName"
                 },
                 "ModelDataUrl": {
-                    "documentation": "<p>The Amazon S3 path where the model artifacts, which result from model training, are stored. This path must point to a single <code>gzip</code> compressed tar archive (<code>.tar.gz</code> suffix).</p> <note> <p>The model artifacts must be in an S3 bucket that is in the same region as the algorithm.</p> </note>",
+                    "documentation": "<p>The Amazon S3 path where the model artifacts, which result from model training, are stored. This path must point to a single <code>gzip</code> compressed tar archive (<code>.tar.gz</code> suffix).</p> <note> <p>The model artifacts must be in an S3 bucket that is in the same Amazon Web Services region as the algorithm.</p> </note>",
                     "shape": "Url"
                 }
             },
             "required": [
                 "AlgorithmName"
             ],
             "type": "structure"
@@ -33208,20 +33845,24 @@
                     "shape": "PipelineExecutionDescription"
                 },
                 "PipelineExecutionDisplayName": {
                     "documentation": "<p>The display name of the pipeline execution.</p>",
                     "shape": "PipelineExecutionName"
                 },
                 "PipelineName": {
-                    "documentation": "<p>The name of the pipeline.</p>",
+                    "documentation": "<p>The name or Amazon Resource Name (ARN) of the pipeline.</p>",
                     "shape": "PipelineNameOrArn"
                 },
                 "PipelineParameters": {
                     "documentation": "<p>Contains a list of pipeline parameters. This list can be empty. </p>",
                     "shape": "ParameterList"
+                },
+                "SelectiveExecutionConfig": {
+                    "documentation": "<p>The selective execution configuration applied to the pipeline run.</p>",
+                    "shape": "SelectiveExecutionConfig"
                 }
             },
             "required": [
                 "PipelineName",
                 "ClientRequestToken"
             ],
             "type": "structure"
@@ -33659,15 +34300,15 @@
             },
             "type": "list"
         },
         "Success": {
             "type": "boolean"
         },
         "SuggestionQuery": {
-            "documentation": "<p>Specified in the <a>GetSearchSuggestions</a> request. Limits the property names that are included in the response.</p>",
+            "documentation": "<p>Specified in the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_GetSearchSuggestions.html\">GetSearchSuggestions</a> request. Limits the property names that are included in the response.</p>",
             "members": {
                 "PropertyNameQuery": {
                     "documentation": "<p>Defines a property name hint. Only property names that begin with the specified hint are included in the response.</p>",
                     "shape": "PropertyNameQuery"
                 }
             },
             "type": "structure"
@@ -33681,16 +34322,66 @@
         },
         "TableName": {
             "max": 255,
             "min": 1,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\t]*",
             "type": "string"
         },
+        "TabularJobConfig": {
+            "documentation": "<p>The collection of settings used by an AutoML job V2 for the <code>TABULAR</code> problem type.</p>",
+            "members": {
+                "CandidateGenerationConfig": {
+                    "documentation": "<p>The configuration information of how model candidates are generated.</p>",
+                    "shape": "CandidateGenerationConfig"
+                },
+                "CompletionCriteria": {
+                    "shape": "AutoMLJobCompletionCriteria"
+                },
+                "FeatureSpecificationS3Uri": {
+                    "documentation": "<p>A URL to the Amazon S3 data source containing selected features from the input data source to run an Autopilot job V2. You can input <code>FeatureAttributeNames</code> (optional) in JSON format as shown below: </p> <p> <code>{ \"FeatureAttributeNames\":[\"col1\", \"col2\", ...] }</code>.</p> <p>You can also specify the data type of the feature (optional) in the format shown below:</p> <p> <code>{ \"FeatureDataTypes\":{\"col1\":\"numeric\", \"col2\":\"categorical\" ... } }</code> </p> <note> <p>These column keys may not include the target column.</p> </note> <p>In ensembling mode, Autopilot only supports the following data types: <code>numeric</code>, <code>categorical</code>, <code>text</code>, and <code>datetime</code>. In HPO mode, Autopilot can support <code>numeric</code>, <code>categorical</code>, <code>text</code>, <code>datetime</code>, and <code>sequence</code>.</p> <p>If only <code>FeatureDataTypes</code> is provided, the column keys (<code>col1</code>, <code>col2</code>,..) should be a subset of the column names in the input data. </p> <p>If both <code>FeatureDataTypes</code> and <code>FeatureAttributeNames</code> are provided, then the column keys should be a subset of the column names provided in <code>FeatureAttributeNames</code>. </p> <p>The key name <code>FeatureAttributeNames</code> is fixed. The values listed in <code>[\"col1\", \"col2\", ...]</code> are case sensitive and should be a list of strings containing unique values that are a subset of the column names in the input data. The list of columns provided must not include the target column.</p>",
+                    "shape": "S3Uri"
+                },
+                "GenerateCandidateDefinitionsOnly": {
+                    "documentation": "<p>Generates possible candidates without training the models. A model candidate is a combination of data preprocessors, algorithms, and algorithm parameter settings.</p>",
+                    "shape": "GenerateCandidateDefinitionsOnly"
+                },
+                "Mode": {
+                    "documentation": "<p>The method that Autopilot uses to train the data. You can either specify the mode manually or let Autopilot choose for you based on the dataset size by selecting <code>AUTO</code>. In <code>AUTO</code> mode, Autopilot chooses <code>ENSEMBLING</code> for datasets smaller than 100 MB, and <code>HYPERPARAMETER_TUNING</code> for larger ones.</p> <p>The <code>ENSEMBLING</code> mode uses a multi-stack ensemble model to predict classification and regression tasks directly from your dataset. This machine learning mode combines several base models to produce an optimal predictive model. It then uses a stacking ensemble method to combine predictions from contributing members. A multi-stack ensemble model can provide better performance over a single model by combining the predictive capabilities of multiple models. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-model-support-validation.html#autopilot-algorithm-support\">Autopilot algorithm support</a> for a list of algorithms supported by <code>ENSEMBLING</code> mode.</p> <p>The <code>HYPERPARAMETER_TUNING</code> (HPO) mode uses the best hyperparameters to train the best version of a model. HPO automatically selects an algorithm for the type of problem you want to solve. Then HPO finds the best hyperparameters according to your objective metric. See <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-model-support-validation.html#autopilot-algorithm-support\">Autopilot algorithm support</a> for a list of algorithms supported by <code>HYPERPARAMETER_TUNING</code> mode.</p>",
+                    "shape": "AutoMLMode"
+                },
+                "ProblemType": {
+                    "documentation": "<p>The type of supervised learning problem available for the model candidates of the AutoML job V2. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-datasets-problem-types.html#autopilot-problem-types\"> Amazon SageMaker Autopilot problem types</a>.</p> <note> <p>You must either specify the type of supervised learning problem in <code>ProblemType</code> and provide the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJobV2.html#sagemaker-CreateAutoMLJobV2-request-AutoMLJobObjective\">AutoMLJobObjective</a> metric, or none at all.</p> </note>",
+                    "shape": "ProblemType"
+                },
+                "SampleWeightAttributeName": {
+                    "documentation": "<p>If specified, this column name indicates which column of the dataset should be treated as sample weights for use by the objective metric during the training, evaluation, and the selection of the best model. This column is not considered as a predictive feature. For more information on Autopilot metrics, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-metrics-validation.html\">Metrics and validation</a>.</p> <p>Sample weights should be numeric, non-negative, with larger values indicating which rows are more important than others. Data points that have invalid or no weight value are excluded.</p> <p>Support for sample weights is available in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AutoMLAlgorithmConfig.html\">Ensembling</a> mode only.</p>",
+                    "shape": "SampleWeightAttributeName"
+                },
+                "TargetAttributeName": {
+                    "documentation": "<p>The name of the target variable in supervised learning, usually represented by 'y'.</p>",
+                    "shape": "TargetAttributeName"
+                }
+            },
+            "required": [
+                "TargetAttributeName"
+            ],
+            "type": "structure"
+        },
+        "TabularResolvedAttributes": {
+            "documentation": "<p>The resolved attributes specific to the <code>TABULAR</code> problem type.</p>",
+            "members": {
+                "ProblemType": {
+                    "documentation": "<p>The type of supervised learning problem available for the model candidates of the AutoML job V2 (Binary Classification, Multiclass Classification, Regression). For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/autopilot-datasets-problem-types.html#autopilot-problem-types\"> Amazon SageMaker Autopilot problem types</a>.</p>",
+                    "shape": "ProblemType"
+                }
+            },
+            "type": "structure"
+        },
         "Tag": {
-            "documentation": "<p>A tag object that consists of a key and an optional value, used to manage metadata for SageMaker Amazon Web Services resources.</p> <p>You can add tags to notebook instances, training jobs, hyperparameter tuning jobs, batch transform jobs, models, labeling jobs, work teams, endpoint configurations, and endpoints. For more information on adding tags to SageMaker resources, see <a>AddTags</a>.</p> <p>For more information on adding metadata to your Amazon Web Services resources with tagging, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a>. For advice on best practices for managing Amazon Web Services resources with tagging, see <a href=\"https://d1.awsstatic.com/whitepapers/aws-tagging-best-practices.pdf\">Tagging Best Practices: Implement an Effective Amazon Web Services Resource Tagging Strategy</a>.</p>",
+            "documentation": "<p>A tag object that consists of a key and an optional value, used to manage metadata for SageMaker Amazon Web Services resources.</p> <p>You can add tags to notebook instances, training jobs, hyperparameter tuning jobs, batch transform jobs, models, labeling jobs, work teams, endpoint configurations, and endpoints. For more information on adding tags to SageMaker resources, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_AddTags.html\">AddTags</a>.</p> <p>For more information on adding metadata to your Amazon Web Services resources with tagging, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services resources</a>. For advice on best practices for managing Amazon Web Services resources with tagging, see <a href=\"https://d1.awsstatic.com/whitepapers/aws-tagging-best-practices.pdf\">Tagging Best Practices: Implement an Effective Amazon Web Services Resource Tagging Strategy</a>.</p>",
             "members": {
                 "Key": {
                     "documentation": "<p>The tag key. Tag keys must be unique per resource.</p>",
                     "shape": "TagKey"
                 },
                 "Value": {
                     "documentation": "<p>The tag value.</p>",
@@ -33742,14 +34433,16 @@
                 "ml_m5",
                 "ml_c4",
                 "ml_c5",
                 "ml_p2",
                 "ml_p3",
                 "ml_g4dn",
                 "ml_inf1",
+                "ml_inf2",
+                "ml_trn1",
                 "ml_eia2",
                 "jetson_tx1",
                 "jetson_tx2",
                 "jetson_nano",
                 "jetson_xavier",
                 "rasp3b",
                 "imx8qm",
@@ -33922,53 +34615,137 @@
         },
         "TerminationWaitInSeconds": {
             "max": 3600,
             "min": 0,
             "type": "integer"
         },
         "TextClassificationJobConfig": {
-            "documentation": "<p>Stores the configuration information for the text classification problem of an AutoML job using the V2 API.</p>",
+            "documentation": "<p>Stores the configuration information for the text classification problem of an AutoML job V2.</p>",
             "members": {
                 "CompletionCriteria": {
                     "documentation": "<p>How long a job is allowed to run, or how many candidates a job is allowed to generate.</p>",
                     "shape": "AutoMLJobCompletionCriteria"
                 },
                 "ContentColumn": {
-                    "documentation": "<p>The name of the column used to provide the sentences to be classified. It should not be the same as the target column.</p>",
+                    "documentation": "<p>The name of the column used to provide the sentences to be classified. It should not be the same as the target column (Required).</p>",
                     "shape": "ContentColumn"
                 },
                 "TargetLabelColumn": {
-                    "documentation": "<p>The name of the column used to provide the class labels. It should not be same as the content column.</p>",
+                    "documentation": "<p>The name of the column used to provide the class labels. It should not be same as the content column (Required).</p>",
                     "shape": "TargetLabelColumn"
                 }
             },
             "type": "structure"
         },
         "ThingName": {
             "max": 128,
             "pattern": "[a-zA-Z0-9:_-]+",
             "type": "string"
         },
+        "TimeSeriesConfig": {
+            "documentation": "<p>The collection of components that defines the time-series.</p>",
+            "members": {
+                "GroupingAttributeNames": {
+                    "documentation": "<p>A set of columns names that can be grouped with the item identifier column to create a composite key for which a target value is predicted.</p>",
+                    "shape": "GroupingAttributeNames"
+                },
+                "ItemIdentifierAttributeName": {
+                    "documentation": "<p>The name of the column that represents the set of item identifiers for which you want to predict the target value.</p>",
+                    "shape": "ItemIdentifierAttributeName"
+                },
+                "TargetAttributeName": {
+                    "documentation": "<p>The name of the column representing the target variable that you want to predict for each item in your dataset. The data type of the target variable must be numerical.</p>",
+                    "shape": "TargetAttributeName"
+                },
+                "TimestampAttributeName": {
+                    "documentation": "<p>The name of the column indicating a point in time at which the target value of a given item is recorded.</p>",
+                    "shape": "TimestampAttributeName"
+                }
+            },
+            "required": [
+                "TargetAttributeName",
+                "TimestampAttributeName",
+                "ItemIdentifierAttributeName"
+            ],
+            "type": "structure"
+        },
+        "TimeSeriesForecastingJobConfig": {
+            "documentation": "<p>The collection of settings used by an AutoML job V2 for the time-series forecasting problem type.</p> <note> <p>The <code>TimeSeriesForecastingJobConfig</code> problem type is only available in private beta. Contact Amazon Web Services Support or your account manager to learn more about access privileges.</p> </note>",
+            "members": {
+                "CompletionCriteria": {
+                    "shape": "AutoMLJobCompletionCriteria"
+                },
+                "FeatureSpecificationS3Uri": {
+                    "documentation": "<p>A URL to the Amazon S3 data source containing additional selected features that complement the target, itemID, timestamp, and grouped columns set in <code>TimeSeriesConfig</code>. When not provided, the AutoML job V2 includes all the columns from the original dataset that are not already declared in <code>TimeSeriesConfig</code>. If provided, the AutoML job V2 only considers these additional columns as a complement to the ones declared in <code>TimeSeriesConfig</code>.</p> <p> You can input <code>FeatureAttributeNames</code> (optional) in JSON format as shown below: </p> <p> <code>{ \"FeatureAttributeNames\":[\"col1\", \"col2\", ...] }</code>.</p> <p>You can also specify the data type of the feature (optional) in the format shown below:</p> <p> <code>{ \"FeatureDataTypes\":{\"col1\":\"numeric\", \"col2\":\"categorical\" ... } }</code> </p> <p>Autopilot supports the following data types: <code>numeric</code>, <code>categorical</code>, <code>text</code>, and <code>datetime</code>.</p> <note> <p>These column keys must not include any column set in <code>TimeSeriesConfig</code>.</p> </note> <p>When not provided, the AutoML job V2 includes all the columns from the original dataset that are not already declared in <code>TimeSeriesConfig</code>. If provided, the AutoML job V2 only considers these additional columns as a complement to the ones declared in <code>TimeSeriesConfig</code>.</p> <p>Autopilot supports the following data types: <code>numeric</code>, <code>categorical</code>, <code>text</code>, and <code>datetime</code>.</p>",
+                    "shape": "S3Uri"
+                },
+                "ForecastFrequency": {
+                    "documentation": "<p>The frequency of predictions in a forecast.</p> <p>Valid intervals are an integer followed by Y (Year), M (Month), W (Week), D (Day), H (Hour), and min (Minute). For example, <code>1D</code> indicates every day and <code>15min</code> indicates every 15 minutes. The value of a frequency must not overlap with the next larger frequency. For example, you must use a frequency of <code>1H</code> instead of <code>60min</code>.</p> <p>The valid values for each frequency are the following:</p> <ul> <li> <p>Minute - 1-59</p> </li> <li> <p>Hour - 1-23</p> </li> <li> <p>Day - 1-6</p> </li> <li> <p>Week - 1-4</p> </li> <li> <p>Month - 1-11</p> </li> <li> <p>Year - 1</p> </li> </ul>",
+                    "shape": "ForecastFrequency"
+                },
+                "ForecastHorizon": {
+                    "documentation": "<p>The number of time-steps that the model predicts. The forecast horizon is also called the prediction length. The maximum forecast horizon is the lesser of 500 time-steps or 1/4 of the time-steps in the dataset.</p>",
+                    "shape": "ForecastHorizon"
+                },
+                "ForecastQuantiles": {
+                    "documentation": "<p>The quantiles used to train the model for forecasts at a specified quantile. You can specify quantiles from <code>0.01</code> (p1) to <code>0.99</code> (p99), by increments of 0.01 or higher. Up to five forecast quantiles can be specified. When <code>ForecastQuantiles</code> is not provided, the AutoML job uses the quantiles p10, p50, and p90 as default.</p>",
+                    "shape": "ForecastQuantiles"
+                },
+                "TimeSeriesConfig": {
+                    "documentation": "<p>The collection of components that defines the time-series.</p>",
+                    "shape": "TimeSeriesConfig"
+                },
+                "Transformations": {
+                    "documentation": "<p>The transformations modifying specific attributes of the time-series, such as filling strategies for missing values.</p>",
+                    "shape": "TimeSeriesTransformations"
+                }
+            },
+            "required": [
+                "ForecastFrequency",
+                "ForecastHorizon",
+                "TimeSeriesConfig"
+            ],
+            "type": "structure"
+        },
         "TimeSeriesForecastingSettings": {
-            "documentation": "<p>Time series forecast settings for the SageMaker Canvas app.</p>",
+            "documentation": "<p>Time series forecast settings for the SageMaker Canvas application.</p>",
             "members": {
                 "AmazonForecastRoleArn": {
-                    "documentation": "<p>The IAM role that Canvas passes to Amazon Forecast for time series forecasting. By default, Canvas uses the execution role specified in the <code>UserProfile</code> that launches the Canvas app. If an execution role is not specified in the <code>UserProfile</code>, Canvas uses the execution role specified in the Domain that owns the <code>UserProfile</code>. To allow time series forecasting, this IAM role should have the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/security-iam-awsmanpol-canvas.html#security-iam-awsmanpol-AmazonSageMakerCanvasForecastAccess\"> AmazonSageMakerCanvasForecastAccess</a> policy attached and <code>forecast.amazonaws.com</code> added in the trust relationship as a service principal.</p>",
+                    "documentation": "<p>The IAM role that Canvas passes to Amazon Forecast for time series forecasting. By default, Canvas uses the execution role specified in the <code>UserProfile</code> that launches the Canvas application. If an execution role is not specified in the <code>UserProfile</code>, Canvas uses the execution role specified in the Domain that owns the <code>UserProfile</code>. To allow time series forecasting, this IAM role should have the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/security-iam-awsmanpol-canvas.html#security-iam-awsmanpol-AmazonSageMakerCanvasForecastAccess\"> AmazonSageMakerCanvasForecastAccess</a> policy attached and <code>forecast.amazonaws.com</code> added in the trust relationship as a service principal.</p>",
                     "shape": "RoleArn"
                 },
                 "Status": {
-                    "documentation": "<p>Describes whether time series forecasting is enabled or disabled in the Canvas app.</p>",
+                    "documentation": "<p>Describes whether time series forecasting is enabled or disabled in the Canvas application.</p>",
                     "shape": "FeatureStatus"
                 }
             },
             "type": "structure"
         },
+        "TimeSeriesTransformations": {
+            "documentation": "<p>Transformations allowed on the dataset. Supported transformations are <code>Filling</code> and <code>Aggregation</code>. <code>Filling</code> specifies how to add values to missing values in the dataset. <code>Aggregation</code> defines how to aggregate data that does not align with forecast frequency.</p>",
+            "members": {
+                "Aggregation": {
+                    "documentation": "<p>A key value pair defining the aggregation method for a column, where the key is the column name and the value is the aggregation method.</p> <p>The supported aggregation methods are <code>sum</code> (default), <code>avg</code>, <code>first</code>, <code>min</code>, <code>max</code>.</p> <note> <p>Aggregation is only supported for the target column.</p> </note>",
+                    "shape": "AggregationTransformations"
+                },
+                "Filling": {
+                    "documentation": "<p>A key value pair defining the filling method for a column, where the key is the column name and the value is an object which defines the filling logic. You can specify multiple filling methods for a single column.</p> <p>The supported filling methods and their corresponding options are:</p> <ul> <li> <p> <code>frontfill</code>: <code>none</code> (Supported only for target column)</p> </li> <li> <p> <code>middlefill</code>: <code>zero</code>, <code>value</code>, <code>median</code>, <code>mean</code>, <code>min</code>, <code>max</code> </p> </li> <li> <p> <code>backfill</code>: <code>zero</code>, <code>value</code>, <code>median</code>, <code>mean</code>, <code>min</code>, <code>max</code> </p> </li> <li> <p> <code>futurefill</code>: <code>zero</code>, <code>value</code>, <code>median</code>, <code>mean</code>, <code>min</code>, <code>max</code> </p> </li> </ul> <p>To set a filling method to a specific value, set the fill parameter to the chosen filling method value (for example <code>\"backfill\" : \"value\"</code>), and define the filling value in an additional parameter prefixed with \"_value\". For example, to set <code>backfill</code> to a value of <code>2</code>, you must include two parameters: <code>\"backfill\": \"value\"</code> and <code>\"backfill_value\":\"2\"</code>.</p>",
+                    "shape": "FillingTransformations"
+                }
+            },
+            "type": "structure"
+        },
         "Timestamp": {
             "type": "timestamp"
         },
+        "TimestampAttributeName": {
+            "max": 256,
+            "min": 1,
+            "type": "string"
+        },
         "TrafficDurationInSeconds": {
             "min": 1,
             "type": "integer"
         },
         "TrafficPattern": {
             "documentation": "<p>Defines the traffic pattern of the load test.</p>",
             "members": {
@@ -34145,15 +34922,16 @@
                 "ml.g5.4xlarge",
                 "ml.g5.8xlarge",
                 "ml.g5.16xlarge",
                 "ml.g5.12xlarge",
                 "ml.g5.24xlarge",
                 "ml.g5.48xlarge",
                 "ml.trn1.2xlarge",
-                "ml.trn1.32xlarge"
+                "ml.trn1.32xlarge",
+                "ml.trn1n.32xlarge"
             ],
             "type": "string"
         },
         "TrainingInstanceTypes": {
             "member": {
                 "shape": "TrainingInstanceType"
             },
@@ -34220,15 +34998,15 @@
                     "shape": "FinalMetricDataList"
                 },
                 "HyperParameters": {
                     "documentation": "<p>Algorithm-specific parameters.</p>",
                     "shape": "HyperParameters"
                 },
                 "InputDataConfig": {
-                    "documentation": "<p>An array of <code>Channel</code> objects that describes each data input channel.</p>",
+                    "documentation": "<p>An array of <code>Channel</code> objects that describes each data input channel.</p> <p>Your input must be in the same Amazon Web Services region as your training job.</p>",
                     "shape": "InputDataConfig"
                 },
                 "LabelingJobArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the labeling job.</p>",
                     "shape": "LabelingJobArn"
                 },
                 "LastModifiedTime": {
@@ -34252,15 +35030,15 @@
                     "shape": "RetryStrategy"
                 },
                 "RoleArn": {
                     "documentation": "<p>The Amazon Web Services Identity and Access Management (IAM) role configured for the training job.</p>",
                     "shape": "RoleArn"
                 },
                 "SecondaryStatus": {
-                    "documentation": "<p> Provides detailed information about the state of the training job. For detailed information about the secondary status of the training job, see <code>StatusMessage</code> under <a>SecondaryStatusTransition</a>.</p> <p>SageMaker provides primary statuses and secondary statuses that apply to each of them:</p> <dl> <dt>InProgress</dt> <dd> <ul> <li> <p> <code>Starting</code> - Starting the training job.</p> </li> <li> <p> <code>Downloading</code> - An optional stage for algorithms that support <code>File</code> training input mode. It indicates that data is being downloaded to the ML storage volumes.</p> </li> <li> <p> <code>Training</code> - Training is in progress.</p> </li> <li> <p> <code>Uploading</code> - Training is complete and the model artifacts are being uploaded to the S3 location.</p> </li> </ul> </dd> <dt>Completed</dt> <dd> <ul> <li> <p> <code>Completed</code> - The training job has completed.</p> </li> </ul> </dd> <dt>Failed</dt> <dd> <ul> <li> <p> <code>Failed</code> - The training job has failed. The reason for the failure is returned in the <code>FailureReason</code> field of <code>DescribeTrainingJobResponse</code>.</p> </li> </ul> </dd> <dt>Stopped</dt> <dd> <ul> <li> <p> <code>MaxRuntimeExceeded</code> - The job stopped because it exceeded the maximum allowed runtime.</p> </li> <li> <p> <code>Stopped</code> - The training job has stopped.</p> </li> </ul> </dd> <dt>Stopping</dt> <dd> <ul> <li> <p> <code>Stopping</code> - Stopping the training job.</p> </li> </ul> </dd> </dl> <important> <p>Valid values for <code>SecondaryStatus</code> are subject to change. </p> </important> <p>We no longer support the following secondary statuses:</p> <ul> <li> <p> <code>LaunchingMLInstances</code> </p> </li> <li> <p> <code>PreparingTrainingStack</code> </p> </li> <li> <p> <code>DownloadingTrainingImage</code> </p> </li> </ul>",
+                    "documentation": "<p> Provides detailed information about the state of the training job. For detailed information about the secondary status of the training job, see <code>StatusMessage</code> under <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_SecondaryStatusTransition.html\">SecondaryStatusTransition</a>.</p> <p>SageMaker provides primary statuses and secondary statuses that apply to each of them:</p> <dl> <dt>InProgress</dt> <dd> <ul> <li> <p> <code>Starting</code> - Starting the training job.</p> </li> <li> <p> <code>Downloading</code> - An optional stage for algorithms that support <code>File</code> training input mode. It indicates that data is being downloaded to the ML storage volumes.</p> </li> <li> <p> <code>Training</code> - Training is in progress.</p> </li> <li> <p> <code>Uploading</code> - Training is complete and the model artifacts are being uploaded to the S3 location.</p> </li> </ul> </dd> <dt>Completed</dt> <dd> <ul> <li> <p> <code>Completed</code> - The training job has completed.</p> </li> </ul> </dd> <dt>Failed</dt> <dd> <ul> <li> <p> <code>Failed</code> - The training job has failed. The reason for the failure is returned in the <code>FailureReason</code> field of <code>DescribeTrainingJobResponse</code>.</p> </li> </ul> </dd> <dt>Stopped</dt> <dd> <ul> <li> <p> <code>MaxRuntimeExceeded</code> - The job stopped because it exceeded the maximum allowed runtime.</p> </li> <li> <p> <code>Stopped</code> - The training job has stopped.</p> </li> </ul> </dd> <dt>Stopping</dt> <dd> <ul> <li> <p> <code>Stopping</code> - Stopping the training job.</p> </li> </ul> </dd> </dl> <important> <p>Valid values for <code>SecondaryStatus</code> are subject to change. </p> </important> <p>We no longer support the following secondary statuses:</p> <ul> <li> <p> <code>LaunchingMLInstances</code> </p> </li> <li> <p> <code>PreparingTrainingStack</code> </p> </li> <li> <p> <code>DownloadingTrainingImage</code> </p> </li> </ul>",
                     "shape": "SecondaryStatus"
                 },
                 "SecondaryStatusTransitions": {
                     "documentation": "<p>A history of all of the secondary statuses that the training job has transitioned through.</p>",
                     "shape": "SecondaryStatusTransitions"
                 },
                 "StoppingCondition": {
@@ -34299,15 +35077,15 @@
                     "shape": "TrainingTimeInSeconds"
                 },
                 "TuningJobArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the associated hyperparameter tuning job if the training job was launched by a hyperparameter tuning job.</p>",
                     "shape": "HyperParameterTuningJobArn"
                 },
                 "VpcConfig": {
-                    "documentation": "<p>A <a>VpcConfig</a> object that specifies the VPC that this training job has access to. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/train-vpc.html\">Protect Training Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
+                    "documentation": "<p>A <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_VpcConfig.html\">VpcConfig</a> object that specifies the VPC that this training job has access to. For more information, see <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/train-vpc.html\">Protect Training Jobs by Using an Amazon Virtual Private Cloud</a>.</p>",
                     "shape": "VpcConfig"
                 }
             },
             "type": "structure"
         },
         "TrainingJobArn": {
             "max": 256,
@@ -34804,15 +35582,15 @@
         "TransformJobSummaries": {
             "member": {
                 "shape": "TransformJobSummary"
             },
             "type": "list"
         },
         "TransformJobSummary": {
-            "documentation": "<p>Provides a summary of a transform job. Multiple <code>TransformJobSummary</code> objects are returned as a list after in response to a <a>ListTransformJobs</a> call.</p>",
+            "documentation": "<p>Provides a summary of a transform job. Multiple <code>TransformJobSummary</code> objects are returned as a list after in response to a <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ListTransformJobs.html\">ListTransformJobs</a> call.</p>",
             "members": {
                 "CreationTime": {
                     "documentation": "<p>A timestamp that shows when the transform Job was created.</p>",
                     "shape": "Timestamp"
                 },
                 "FailureReason": {
                     "documentation": "<p>If the transform job failed, the reason it failed.</p>",
@@ -34908,16 +35686,21 @@
             },
             "required": [
                 "S3DataType",
                 "S3Uri"
             ],
             "type": "structure"
         },
+        "TransformationAttributeName": {
+            "max": 256,
+            "min": 1,
+            "type": "string"
+        },
         "Trial": {
-            "documentation": "<p>The properties of a trial as returned by the <a>Search</a> API.</p>",
+            "documentation": "<p>The properties of a trial as returned by the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API.</p>",
             "members": {
                 "CreatedBy": {
                     "documentation": "<p>Who created the trial.</p>",
                     "shape": "UserContext"
                 },
                 "CreationTime": {
                     "documentation": "<p>When the trial was created.</p>",
@@ -34941,15 +35724,15 @@
                 "MetadataProperties": {
                     "shape": "MetadataProperties"
                 },
                 "Source": {
                     "shape": "TrialSource"
                 },
                 "Tags": {
-                    "documentation": "<p>The list of tags that are associated with the trial. You can use <a>Search</a> API to search on the tags.</p>",
+                    "documentation": "<p>The list of tags that are associated with the trial. You can use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API to search on the tags.</p>",
                     "shape": "TagList"
                 },
                 "TrialArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the trial.</p>",
                     "shape": "TrialArn"
                 },
                 "TrialComponentSummaries": {
@@ -34965,15 +35748,15 @@
         },
         "TrialArn": {
             "max": 256,
             "pattern": "arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:experiment-trial/.*",
             "type": "string"
         },
         "TrialComponent": {
-            "documentation": "<p>The properties of a trial component as returned by the <a>Search</a> API.</p>",
+            "documentation": "<p>The properties of a trial component as returned by the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API.</p>",
             "members": {
                 "CreatedBy": {
                     "documentation": "<p>Who created the trial component.</p>",
                     "shape": "UserContext"
                 },
                 "CreationTime": {
                     "documentation": "<p>When the component was created.</p>",
@@ -35037,15 +35820,15 @@
                     "documentation": "<p>When the component started.</p>",
                     "shape": "Timestamp"
                 },
                 "Status": {
                     "shape": "TrialComponentStatus"
                 },
                 "Tags": {
-                    "documentation": "<p>The list of tags that are associated with the component. You can use <a>Search</a> API to search on the tags.</p>",
+                    "documentation": "<p>The list of tags that are associated with the component. You can use <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_Search.html\">Search</a> API to search on the tags.</p>",
                     "shape": "TagList"
                 },
                 "TrialComponentArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the trial component.</p>",
                     "shape": "TrialComponentArn"
                 },
                 "TrialComponentName": {
@@ -35057,15 +35840,15 @@
         },
         "TrialComponentArn": {
             "max": 256,
             "pattern": "arn:aws[a-z\\-]*:sagemaker:[a-z0-9\\-]*:[0-9]{12}:experiment-trial-component/.*",
             "type": "string"
         },
         "TrialComponentArtifact": {
-            "documentation": "<p>Represents an input or output artifact of a trial component. You specify <code>TrialComponentArtifact</code> as part of the <code>InputArtifacts</code> and <code>OutputArtifacts</code> parameters in the <a>CreateTrialComponent</a> request.</p> <p>Examples of input artifacts are datasets, algorithms, hyperparameters, source code, and instance types. Examples of output artifacts are metrics, snapshots, logs, and images.</p>",
+            "documentation": "<p>Represents an input or output artifact of a trial component. You specify <code>TrialComponentArtifact</code> as part of the <code>InputArtifacts</code> and <code>OutputArtifacts</code> parameters in the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateTrialComponent.html\">CreateTrialComponent</a> request.</p> <p>Examples of input artifacts are datasets, algorithms, hyperparameters, source code, and instance types. Examples of output artifacts are metrics, snapshots, logs, and images.</p>",
             "members": {
                 "MediaType": {
                     "documentation": "<p>The media type of the artifact, which indicates the type of data in the artifact file. The media type consists of a <i>type</i> and a <i>subtype</i> concatenated with a slash (/) character, for example, text/csv, image/jpeg, and s3/uri. The type specifies the category of the media. The subtype specifies the kind of data.</p>",
                     "shape": "MediaType"
                 },
                 "Value": {
                     "documentation": "<p>The location of the artifact.</p>",
@@ -35147,15 +35930,15 @@
                     "documentation": "<p>When the metric was last updated.</p>",
                     "shape": "Timestamp"
                 }
             },
             "type": "structure"
         },
         "TrialComponentParameterValue": {
-            "documentation": "<p>The value of a hyperparameter. Only one of <code>NumberValue</code> or <code>StringValue</code> can be specified.</p> <p>This object is specified in the <a>CreateTrialComponent</a> request.</p>",
+            "documentation": "<p>The value of a hyperparameter. Only one of <code>NumberValue</code> or <code>StringValue</code> can be specified.</p> <p>This object is specified in the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateTrialComponent.html\">CreateTrialComponent</a> request.</p>",
             "members": {
                 "NumberValue": {
                     "documentation": "<p>The numeric value of a numeric hyperparameter. If you specify a value for this parameter, you can't specify the <code>StringValue</code> parameter.</p>",
                     "shape": "DoubleParameterValue"
                 },
                 "StringValue": {
                     "documentation": "<p>The string value of a categorical hyperparameter. If you specify a value for this parameter, you can't specify the <code>NumberValue</code> parameter.</p>",
@@ -35286,15 +36069,15 @@
         "TrialComponentSummaries": {
             "member": {
                 "shape": "TrialComponentSummary"
             },
             "type": "list"
         },
         "TrialComponentSummary": {
-            "documentation": "<p>A summary of the properties of a trial component. To get all the properties, call the <a>DescribeTrialComponent</a> API and provide the <code>TrialComponentName</code>.</p>",
+            "documentation": "<p>A summary of the properties of a trial component. To get all the properties, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeTrialComponent.html\">DescribeTrialComponent</a> API and provide the <code>TrialComponentName</code>.</p>",
             "members": {
                 "CreatedBy": {
                     "documentation": "<p>Who created the trial component.</p>",
                     "shape": "UserContext"
                 },
                 "CreationTime": {
                     "documentation": "<p>When the component was created.</p>",
@@ -35363,15 +36146,15 @@
         "TrialSummaries": {
             "member": {
                 "shape": "TrialSummary"
             },
             "type": "list"
         },
         "TrialSummary": {
-            "documentation": "<p>A summary of the properties of a trial. To get the complete set of properties, call the <a>DescribeTrial</a> API and provide the <code>TrialName</code>.</p>",
+            "documentation": "<p>A summary of the properties of a trial. To get the complete set of properties, call the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_DescribeTrial.html\">DescribeTrial</a> API and provide the <code>TrialName</code>.</p>",
             "members": {
                 "CreationTime": {
                     "documentation": "<p>When the trial was created.</p>",
                     "shape": "Timestamp"
                 },
                 "DisplayName": {
                     "documentation": "<p>The name of the trial as displayed. If <code>DisplayName</code> isn't specified, <code>TrialName</code> is displayed.</p>",
@@ -35391,14 +36174,42 @@
                 },
                 "TrialSource": {
                     "shape": "TrialSource"
                 }
             },
             "type": "structure"
         },
+        "TtlDuration": {
+            "documentation": "<p>Time to live duration, where the record is hard deleted after the expiration time is reached; <code>ExpiresAt</code> = <code>EventTime</code> + <code>TtlDuration</code>. For information on HardDelete, see the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_feature_store_DeleteRecord.html\">DeleteRecord</a> API in the Amazon SageMaker API Reference guide.</p>",
+            "members": {
+                "Unit": {
+                    "documentation": "<p> <code>TtlDuration</code> time unit.</p>",
+                    "shape": "TtlDurationUnit"
+                },
+                "Value": {
+                    "documentation": "<p> <code>TtlDuration</code> time value.</p>",
+                    "shape": "TtlDurationValue"
+                }
+            },
+            "type": "structure"
+        },
+        "TtlDurationUnit": {
+            "enum": [
+                "Seconds",
+                "Minutes",
+                "Hours",
+                "Days",
+                "Weeks"
+            ],
+            "type": "string"
+        },
+        "TtlDurationValue": {
+            "min": 1,
+            "type": "integer"
+        },
         "TuningJobCompletionCriteria": {
             "documentation": "<p>The job completion criteria.</p>",
             "members": {
                 "BestObjectiveNotImproving": {
                     "documentation": "<p>A flag to stop your hyperparameter tuning job if model performance fails to improve as evaluated against an objective function.</p>",
                     "shape": "BestObjectiveNotImproving"
                 },
@@ -35683,15 +36494,15 @@
                 "Devices"
             ],
             "type": "structure"
         },
         "UpdateDomainRequest": {
             "members": {
                 "AppSecurityGroupManagement": {
-                    "documentation": "<p>The entity that creates and manages the required security groups for inter-app communication in <code>VPCOnly</code> mode. Required when <code>CreateDomain.AppNetworkAccessType</code> is <code>VPCOnly</code> and <code>DomainSettings.RStudioServerProDomainSettings.DomainExecutionRoleArn</code> is provided.</p>",
+                    "documentation": "<p>The entity that creates and manages the required security groups for inter-app communication in <code>VPCOnly</code> mode. Required when <code>CreateDomain.AppNetworkAccessType</code> is <code>VPCOnly</code> and <code>DomainSettings.RStudioServerProDomainSettings.DomainExecutionRoleArn</code> is provided. If setting up the domain for use with RStudio, this value must be set to <code>Service</code>.</p>",
                     "shape": "AppSecurityGroupManagement"
                 },
                 "DefaultSpaceSettings": {
                     "documentation": "<p>The default settings used to create a space within the Domain.</p>",
                     "shape": "DefaultSpaceSettings"
                 },
                 "DefaultUserSettings": {
@@ -35732,15 +36543,15 @@
                     "shape": "EndpointConfigName"
                 },
                 "EndpointName": {
                     "documentation": "<p>The name of the endpoint whose configuration you want to update.</p>",
                     "shape": "EndpointName"
                 },
                 "ExcludeRetainedVariantProperties": {
-                    "documentation": "<p>When you are updating endpoint resources with <a>UpdateEndpointInput$RetainAllVariantProperties</a>, whose value is set to <code>true</code>, <code>ExcludeRetainedVariantProperties</code> specifies the list of type <a>VariantProperty</a> to override with the values provided by <code>EndpointConfig</code>. If you don't specify a value for <code>ExcludeRetainedVariantProperties</code>, no variant properties are overridden. </p>",
+                    "documentation": "<p>When you are updating endpoint resources with <code>RetainAllVariantProperties</code>, whose value is set to <code>true</code>, <code>ExcludeRetainedVariantProperties</code> specifies the list of type <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_VariantProperty.html\">VariantProperty</a> to override with the values provided by <code>EndpointConfig</code>. If you don't specify a value for <code>ExcludeRetainedVariantProperties</code>, no variant properties are overridden. </p>",
                     "shape": "VariantPropertyList"
                 },
                 "RetainAllVariantProperties": {
                     "documentation": "<p>When updating endpoint resources, enables or disables the retention of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_VariantProperty.html\">variant properties</a>, such as the instance count or the variant weight. To retain the variant properties of an endpoint when updating it, set <code>RetainAllVariantProperties</code> to <code>true</code>. To use the variant properties specified in a new <code>EndpointConfig</code> call when updating an endpoint, set <code>RetainAllVariantProperties</code> to <code>false</code>. The default is <code>false</code>.</p>",
                     "shape": "Boolean"
                 },
                 "RetainDeploymentConfig": {
@@ -35829,14 +36640,18 @@
                 "FeatureAdditions": {
                     "documentation": "<p>Updates the feature group. Updating a feature group is an asynchronous operation. When you get an HTTP 200 response, you've made a valid request. It takes some time after you've made a valid request for Feature Store to update the feature group.</p>",
                     "shape": "FeatureAdditions"
                 },
                 "FeatureGroupName": {
                     "documentation": "<p>The name of the feature group that you're updating.</p>",
                     "shape": "FeatureGroupName"
+                },
+                "OnlineStoreConfig": {
+                    "documentation": "<p>Updates the feature group online store configuration.</p>",
+                    "shape": "OnlineStoreConfigUpdate"
                 }
             },
             "required": [
                 "FeatureGroupName"
             ],
             "type": "structure"
         },
@@ -36062,15 +36877,15 @@
                 "InferenceExperimentArn"
             ],
             "type": "structure"
         },
         "UpdateModelCardRequest": {
             "members": {
                 "Content": {
-                    "documentation": "<p>The updated model card content. Content must be in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-cards-api-json-schema.html\">model card JSON schema</a> and provided as a string.</p> <p>When updating model card content, be sure to include the full content and not just updated content.</p>",
+                    "documentation": "<p>The updated model card content. Content must be in <a href=\"https://docs.aws.amazon.com/sagemaker/latest/dg/model-cards.html#model-cards-json-schema\">model card JSON schema</a> and provided as a string.</p> <p>When updating model card content, be sure to include the full content and not just updated content.</p>",
                     "shape": "ModelCardContent"
                 },
                 "ModelCardName": {
                     "documentation": "<p>The name of the model card to update.</p>",
                     "shape": "EntityName"
                 },
                 "ModelCardStatus": {
@@ -36606,15 +37421,15 @@
                     "shape": "OidcConfig"
                 },
                 "SourceIpConfig": {
                     "documentation": "<p>A list of one to ten worker IP address ranges (<a href=\"https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html\">CIDRs</a>) that can be used to access tasks assigned to this workforce.</p> <p>Maximum: Ten CIDR values</p>",
                     "shape": "SourceIpConfig"
                 },
                 "WorkforceName": {
-                    "documentation": "<p>The name of the private workforce that you want to update. You can find your workforce name by using the operation.</p>",
+                    "documentation": "<p>The name of the private workforce that you want to update. You can find your workforce name by using the <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_ListWorkforces.html\">ListWorkforces</a> operation.</p>",
                     "shape": "WorkforceName"
                 },
                 "WorkforceVpcConfig": {
                     "documentation": "<p>Use this parameter to update your VPC configuration for a workforce.</p>",
                     "shape": "WorkforceVpcConfigRequest"
                 }
             },
@@ -36783,15 +37598,15 @@
                     "shape": "RSessionAppSettings"
                 },
                 "RStudioServerProAppSettings": {
                     "documentation": "<p>A collection of settings that configure user interaction with the <code>RStudioServerPro</code> app.</p>",
                     "shape": "RStudioServerProAppSettings"
                 },
                 "SecurityGroups": {
-                    "documentation": "<p>The security groups for the Amazon Virtual Private Cloud (VPC) that Studio uses for communication.</p> <p>Optional when the <code>CreateDomain.AppNetworkAccessType</code> parameter is set to <code>PublicInternetOnly</code>.</p> <p>Required when the <code>CreateDomain.AppNetworkAccessType</code> parameter is set to <code>VpcOnly</code>.</p> <p>Amazon SageMaker adds a security group to allow NFS traffic from SageMaker Studio. Therefore, the number of security groups that you can specify is one less than the maximum number shown.</p>",
+                    "documentation": "<p>The security groups for the Amazon Virtual Private Cloud (VPC) that Studio uses for communication.</p> <p>Optional when the <code>CreateDomain.AppNetworkAccessType</code> parameter is set to <code>PublicInternetOnly</code>.</p> <p>Required when the <code>CreateDomain.AppNetworkAccessType</code> parameter is set to <code>VpcOnly</code>, unless specified as part of the <code>DefaultUserSettings</code> for the domain.</p> <p>Amazon SageMaker adds a security group to allow NFS traffic from SageMaker Studio. Therefore, the number of security groups that you can specify is one less than the maximum number shown.</p>",
                     "shape": "SecurityGroupIds"
                 },
                 "SharingSettings": {
                     "documentation": "<p>Specifies options for sharing SageMaker Studio notebooks.</p>",
                     "shape": "SharingSettings"
                 },
                 "TensorBoardAppSettings": {
@@ -36812,18 +37627,18 @@
         },
         "VariantName": {
             "max": 63,
             "pattern": "^[a-zA-Z0-9](-*[a-zA-Z0-9]){0,62}",
             "type": "string"
         },
         "VariantProperty": {
-            "documentation": "<p>Specifies a production variant property type for an Endpoint.</p> <p>If you are updating an endpoint with the <a>UpdateEndpointInput$RetainAllVariantProperties</a> option set to <code>true</code>, the <code>VariantProperty</code> objects listed in <a>UpdateEndpointInput$ExcludeRetainedVariantProperties</a> override the existing variant properties of the endpoint.</p>",
+            "documentation": "<p>Specifies a production variant property type for an Endpoint.</p> <p>If you are updating an endpoint with the <code>RetainAllVariantProperties</code> option of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateEndpoint.html\">UpdateEndpointInput</a> set to <code>true</code>, the <code>VariantProperty</code> objects listed in the <code>ExcludeRetainedVariantProperties</code> parameter of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateEndpoint.html\">UpdateEndpointInput</a> override the existing variant properties of the endpoint.</p>",
             "members": {
                 "VariantPropertyType": {
-                    "documentation": "<p>The type of variant property. The supported values are:</p> <ul> <li> <p> <code>DesiredInstanceCount</code>: Overrides the existing variant instance counts using the <a>ProductionVariant$InitialInstanceCount</a> values in the <a>CreateEndpointConfigInput$ProductionVariants</a>.</p> </li> <li> <p> <code>DesiredWeight</code>: Overrides the existing variant weights using the <a>ProductionVariant$InitialVariantWeight</a> values in the <a>CreateEndpointConfigInput$ProductionVariants</a>.</p> </li> <li> <p> <code>DataCaptureConfig</code>: (Not currently supported.)</p> </li> </ul>",
+                    "documentation": "<p>The type of variant property. The supported values are:</p> <ul> <li> <p> <code>DesiredInstanceCount</code>: Overrides the existing variant instance counts using the <code>InitialInstanceCount</code> values in the <code>ProductionVariants</code> of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpointConfig.html\">CreateEndpointConfig</a>.</p> </li> <li> <p> <code>DesiredWeight</code>: Overrides the existing variant weights using the <code>InitialVariantWeight</code> values in the <code>ProductionVariants</code> of <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateEndpointConfig.html\">CreateEndpointConfig</a>.</p> </li> <li> <p> <code>DataCaptureConfig</code>: (Not currently supported.)</p> </li> </ul>",
                     "shape": "VariantPropertyType"
                 }
             },
             "required": [
                 "VariantPropertyType"
             ],
             "type": "structure"
@@ -36989,15 +37804,15 @@
                     "shape": "Timestamp"
                 },
                 "FailureReason": {
                     "documentation": "<p>The reason your workforce failed.</p>",
                     "shape": "WorkforceFailureReason"
                 },
                 "LastUpdatedDate": {
-                    "documentation": "<p>The most recent date that was used to successfully add one or more IP address ranges (<a href=\"https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html\">CIDRs</a>) to a private workforce's allow list.</p>",
+                    "documentation": "<p>The most recent date that <a href=\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_UpdateWorkforce.html\">UpdateWorkforce</a> was used to successfully add one or more IP address ranges (<a href=\"https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html\">CIDRs</a>) to a private workforce's allow list.</p>",
                     "shape": "Timestamp"
                 },
                 "OidcConfig": {
                     "documentation": "<p>The configuration of an OIDC Identity Provider (IdP) private workforce.</p>",
                     "shape": "OidcConfigForResponse"
                 },
                 "SourceIpConfig": {
```

### Comparing `botocore-a-la-carte-sagemaker-1.29.99/botocore/data/sagemaker/2017-07-24/waiters-2.json` & `botocore-a-la-carte-sagemaker-1.30.0/botocore/data/sagemaker/2017-07-24/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-1.29.99/botocore_a_la_carte_sagemaker.egg-info/PKG-INFO` & `botocore-a-la-carte-sagemaker-1.30.0/botocore_a_la_carte_sagemaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sagemaker
-Version: 1.29.99
+Version: 1.30.0
 Summary: sagemaker data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sagemaker-1.29.99/setup.py` & `botocore-a-la-carte-sagemaker-1.30.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-sagemaker',
-    version="1.29.99",
+    version="1.30.0",
     description='sagemaker data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/sagemaker/*/*.json'],
```

