# Comparing `tmp/botocore-a-la-carte-ecs-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-ecs-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ecs-1.29.99.tar", last modified: Sat Mar 25 01:22:39 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-ecs-1.30.0.tar", last modified: Tue Jul  4 01:44:30 2023, max compression
```

## Comparing `botocore-a-la-carte-ecs-1.29.99.tar` & `botocore-a-la-carte-ecs-1.30.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:39.787383 botocore-a-la-carte-ecs-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:39.000000 botocore-a-la-carte-ecs-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-25 01:22:39.787383 botocore-a-la-carte-ecs-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:39.787383 botocore-a-la-carte-ecs-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:39.787383 botocore-a-la-carte-ecs-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:39.787383 botocore-a-la-carte-ecs-1.29.99/botocore/data/ecs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:39.787383 botocore-a-la-carte-ecs-1.29.99/botocore/data/ecs/2014-11-13/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-03-25 01:22:12.000000 botocore-a-la-carte-ecs-1.29.99/botocore/data/ecs/2014-11-13/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    36519 2023-03-25 01:22:12.000000 botocore-a-la-carte-ecs-1.29.99/botocore/data/ecs/2014-11-13/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-03-25 01:22:12.000000 botocore-a-la-carte-ecs-1.29.99/botocore/data/ecs/2014-11-13/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   524605 2023-03-25 01:22:12.000000 botocore-a-la-carte-ecs-1.29.99/botocore/data/ecs/2014-11-13/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-25 01:22:12.000000 botocore-a-la-carte-ecs-1.29.99/botocore/data/ecs/2014-11-13/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:39.787383 botocore-a-la-carte-ecs-1.29.99/botocore_a_la_carte_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-25 01:22:39.000000 botocore-a-la-carte-ecs-1.29.99/botocore_a_la_carte_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-25 01:22:39.000000 botocore-a-la-carte-ecs-1.29.99/botocore_a_la_carte_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:39.000000 botocore-a-la-carte-ecs-1.29.99/botocore_a_la_carte_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:39.000000 botocore-a-la-carte-ecs-1.29.99/botocore_a_la_carte_ecs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:39.787383 botocore-a-la-carte-ecs-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-25 01:22:39.000000 botocore-a-la-carte-ecs-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.566549 botocore-a-la-carte-ecs-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:30.000000 botocore-a-la-carte-ecs-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:44:30.566549 botocore-a-la-carte-ecs-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.562549 botocore-a-la-carte-ecs-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.562549 botocore-a-la-carte-ecs-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.562549 botocore-a-la-carte-ecs-1.30.0/botocore/data/ecs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.562549 botocore-a-la-carte-ecs-1.30.0/botocore/data/ecs/2014-11-13/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-04 01:44:02.000000 botocore-a-la-carte-ecs-1.30.0/botocore/data/ecs/2014-11-13/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36519 2023-07-04 01:44:02.000000 botocore-a-la-carte-ecs-1.30.0/botocore/data/ecs/2014-11-13/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-04 01:44:02.000000 botocore-a-la-carte-ecs-1.30.0/botocore/data/ecs/2014-11-13/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   532044 2023-07-04 01:44:02.000000 botocore-a-la-carte-ecs-1.30.0/botocore/data/ecs/2014-11-13/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-04 01:44:02.000000 botocore-a-la-carte-ecs-1.30.0/botocore/data/ecs/2014-11-13/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.566549 botocore-a-la-carte-ecs-1.30.0/botocore_a_la_carte_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:44:30.000000 botocore-a-la-carte-ecs-1.30.0/botocore_a_la_carte_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-04 01:44:30.000000 botocore-a-la-carte-ecs-1.30.0/botocore_a_la_carte_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:30.000000 botocore-a-la-carte-ecs-1.30.0/botocore_a_la_carte_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:30.000000 botocore-a-la-carte-ecs-1.30.0/botocore_a_la_carte_ecs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:30.566549 botocore-a-la-carte-ecs-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-04 01:44:30.000000 botocore-a-la-carte-ecs-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-ecs-1.29.99/LICENSE.txt` & `botocore-a-la-carte-ecs-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecs-1.29.99/PKG-INFO` & `botocore-a-la-carte-ecs-1.30.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ecs
-Version: 1.29.99
+Version: 1.30.0
 Summary: ecs data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ecs-1.29.99/botocore/data/ecs/2014-11-13/endpoint-rule-set-1.json` & `botocore-a-la-carte-ecs-1.30.0/botocore/data/ecs/2014-11-13/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecs-1.29.99/botocore/data/ecs/2014-11-13/examples-1.json` & `botocore-a-la-carte-ecs-1.30.0/botocore/data/ecs/2014-11-13/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecs-1.29.99/botocore/data/ecs/2014-11-13/paginators-1.json` & `botocore-a-la-carte-ecs-1.30.0/botocore/data/ecs/2014-11-13/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecs-1.29.99/botocore/data/ecs/2014-11-13/service-2.json` & `botocore-a-la-carte-ecs-1.30.0/botocore/data/ecs/2014-11-13/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999185761465251%*

 * *Differences: {"'operations'": "{'CreateCluster': {'errors': {insert: [(3, OrderedDict([('shape', "*

 * *                 "'NamespaceNotFoundException')]))]}}, 'CreateService': {'documentation': '<p>Runs "*

 * *                 'and maintains your desired number of tasks from a specified task definition. If '*

 * *                 'the number of tasks running in a service drops below the '*

 * *                 '<code>desiredCount</code>, Amazon ECS runs another copy of the task in the '*

 * *                 'specified cluster. To update an exi […]*

```diff
@@ -51,14 +51,17 @@
                     "shape": "ServerException"
                 },
                 {
                     "shape": "ClientException"
                 },
                 {
                     "shape": "InvalidParameterException"
+                },
+                {
+                    "shape": "NamespaceNotFoundException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -66,15 +69,15 @@
             },
             "name": "CreateCluster",
             "output": {
                 "shape": "CreateClusterResponse"
             }
         },
         "CreateService": {
-            "documentation": "<p>Runs and maintains your desired number of tasks from a specified task definition. If the number of tasks running in a service drops below the <code>desiredCount</code>, Amazon ECS runs another copy of the task in the specified cluster. To update an existing service, see the <a>UpdateService</a> action.</p> <p>In addition to maintaining the desired count of tasks in your service, you can optionally run your service behind one or more load balancers. The load balancers distribute traffic across the tasks that are associated with the service. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-load-balancing.html\">Service load balancing</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>Tasks for services that don't use a load balancer are considered healthy if they're in the <code>RUNNING</code> state. Tasks for services that use a load balancer are considered healthy if they're in the <code>RUNNING</code> state and are reported as healthy by the load balancer.</p> <p>There are two service scheduler strategies available:</p> <ul> <li> <p> <code>REPLICA</code> - The replica scheduling strategy places and maintains your desired number of tasks across your cluster. By default, the service scheduler spreads tasks across Availability Zones. You can use task placement strategies and constraints to customize task placement decisions. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html\">Service scheduler concepts</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </li> <li> <p> <code>DAEMON</code> - The daemon scheduling strategy deploys exactly one task on each active container instance that meets all of the task placement constraints that you specify in your cluster. The service scheduler also evaluates the task placement constraints for running tasks. It also stops tasks that don't meet the placement constraints. When using this strategy, you don't need to specify a desired number of tasks, a task placement strategy, or use Service Auto Scaling policies. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html\">Service scheduler concepts</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </li> </ul> <p>You can optionally specify a deployment configuration for your service. The deployment is initiated by changing properties. For example, the deployment might be initiated by the task definition or by your desired count of a service. This is done with an <a>UpdateService</a> operation. The default value for a replica service for <code>minimumHealthyPercent</code> is 100%. The default value for a daemon service for <code>minimumHealthyPercent</code> is 0%.</p> <p>If a service uses the <code>ECS</code> deployment controller, the minimum healthy percent represents a lower limit on the number of tasks in a service that must remain in the <code>RUNNING</code> state during a deployment. Specifically, it represents it as a percentage of your desired number of tasks (rounded up to the nearest integer). This happens when any of your container instances are in the <code>DRAINING</code> state if the service contains tasks using the EC2 launch type. Using this parameter, you can deploy without using additional cluster capacity. For example, if you set your service to have desired number of four tasks and a minimum healthy percent of 50%, the scheduler might stop two existing tasks to free up cluster capacity before starting two new tasks. If they're in the <code>RUNNING</code> state, tasks for services that don't use a load balancer are considered healthy . If they're in the <code>RUNNING</code> state and reported as healthy by the load balancer, tasks for services that <i>do</i> use a load balancer are considered healthy . The default value for minimum healthy percent is 100%.</p> <p>If a service uses the <code>ECS</code> deployment controller, the <b>maximum percent</b> parameter represents an upper limit on the number of tasks in a service that are allowed in the <code>RUNNING</code> or <code>PENDING</code> state during a deployment. Specifically, it represents it as a percentage of the desired number of tasks (rounded down to the nearest integer). This happens when any of your container instances are in the <code>DRAINING</code> state if the service contains tasks using the EC2 launch type. Using this parameter, you can define the deployment batch size. For example, if your service has a desired number of four tasks and a maximum percent value of 200%, the scheduler may start four new tasks before stopping the four older tasks (provided that the cluster resources required to do this are available). The default value for maximum percent is 200%.</p> <p>If a service uses either the <code>CODE_DEPLOY</code> or <code>EXTERNAL</code> deployment controller types and tasks that use the EC2 launch type, the <b>minimum healthy percent</b> and <b>maximum percent</b> values are used only to define the lower and upper limit on the number of the tasks in the service that remain in the <code>RUNNING</code> state. This is while the container instances are in the <code>DRAINING</code> state. If the tasks in the service use the Fargate launch type, the minimum healthy percent and maximum percent values aren't used. This is the case even if they're currently visible when describing your service.</p> <p>When creating a service that uses the <code>EXTERNAL</code> deployment controller, you can specify only parameters that aren't controlled at the task set level. The only required parameter is the service name. You control your services using the <a>CreateTaskSet</a> operation. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-types.html\">Amazon ECS deployment types</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>When the service scheduler launches new tasks, it determines task placement. For information about task placement and task placement strategies, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-placement.html\">Amazon ECS task placement</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+            "documentation": "<p>Runs and maintains your desired number of tasks from a specified task definition. If the number of tasks running in a service drops below the <code>desiredCount</code>, Amazon ECS runs another copy of the task in the specified cluster. To update an existing service, see the <a>UpdateService</a> action.</p> <note> <p>Starting April 15, 2023, Amazon Web Services will not onboard new customers to Amazon Elastic Inference (EI), and will help current customers migrate their workloads to options that offer better price and performance. After April 15, 2023, new customers will not be able to launch instances with Amazon EI accelerators in Amazon SageMaker, Amazon ECS, or Amazon EC2. However, customers who have used Amazon EI at least once during the past 30-day period are considered current customers and will be able to continue using the service. </p> </note> <p>In addition to maintaining the desired count of tasks in your service, you can optionally run your service behind one or more load balancers. The load balancers distribute traffic across the tasks that are associated with the service. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-load-balancing.html\">Service load balancing</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>Tasks for services that don't use a load balancer are considered healthy if they're in the <code>RUNNING</code> state. Tasks for services that use a load balancer are considered healthy if they're in the <code>RUNNING</code> state and are reported as healthy by the load balancer.</p> <p>There are two service scheduler strategies available:</p> <ul> <li> <p> <code>REPLICA</code> - The replica scheduling strategy places and maintains your desired number of tasks across your cluster. By default, the service scheduler spreads tasks across Availability Zones. You can use task placement strategies and constraints to customize task placement decisions. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html\">Service scheduler concepts</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </li> <li> <p> <code>DAEMON</code> - The daemon scheduling strategy deploys exactly one task on each active container instance that meets all of the task placement constraints that you specify in your cluster. The service scheduler also evaluates the task placement constraints for running tasks. It also stops tasks that don't meet the placement constraints. When using this strategy, you don't need to specify a desired number of tasks, a task placement strategy, or use Service Auto Scaling policies. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html\">Service scheduler concepts</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </li> </ul> <p>You can optionally specify a deployment configuration for your service. The deployment is initiated by changing properties. For example, the deployment might be initiated by the task definition or by your desired count of a service. This is done with an <a>UpdateService</a> operation. The default value for a replica service for <code>minimumHealthyPercent</code> is 100%. The default value for a daemon service for <code>minimumHealthyPercent</code> is 0%.</p> <p>If a service uses the <code>ECS</code> deployment controller, the minimum healthy percent represents a lower limit on the number of tasks in a service that must remain in the <code>RUNNING</code> state during a deployment. Specifically, it represents it as a percentage of your desired number of tasks (rounded up to the nearest integer). This happens when any of your container instances are in the <code>DRAINING</code> state if the service contains tasks using the EC2 launch type. Using this parameter, you can deploy without using additional cluster capacity. For example, if you set your service to have desired number of four tasks and a minimum healthy percent of 50%, the scheduler might stop two existing tasks to free up cluster capacity before starting two new tasks. If they're in the <code>RUNNING</code> state, tasks for services that don't use a load balancer are considered healthy . If they're in the <code>RUNNING</code> state and reported as healthy by the load balancer, tasks for services that <i>do</i> use a load balancer are considered healthy . The default value for minimum healthy percent is 100%.</p> <p>If a service uses the <code>ECS</code> deployment controller, the <b>maximum percent</b> parameter represents an upper limit on the number of tasks in a service that are allowed in the <code>RUNNING</code> or <code>PENDING</code> state during a deployment. Specifically, it represents it as a percentage of the desired number of tasks (rounded down to the nearest integer). This happens when any of your container instances are in the <code>DRAINING</code> state if the service contains tasks using the EC2 launch type. Using this parameter, you can define the deployment batch size. For example, if your service has a desired number of four tasks and a maximum percent value of 200%, the scheduler may start four new tasks before stopping the four older tasks (provided that the cluster resources required to do this are available). The default value for maximum percent is 200%.</p> <p>If a service uses either the <code>CODE_DEPLOY</code> or <code>EXTERNAL</code> deployment controller types and tasks that use the EC2 launch type, the <b>minimum healthy percent</b> and <b>maximum percent</b> values are used only to define the lower and upper limit on the number of the tasks in the service that remain in the <code>RUNNING</code> state. This is while the container instances are in the <code>DRAINING</code> state. If the tasks in the service use the Fargate launch type, the minimum healthy percent and maximum percent values aren't used. This is the case even if they're currently visible when describing your service.</p> <p>When creating a service that uses the <code>EXTERNAL</code> deployment controller, you can specify only parameters that aren't controlled at the task set level. The only required parameter is the service name. You control your services using the <a>CreateTaskSet</a> operation. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-types.html\">Amazon ECS deployment types</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>When the service scheduler launches new tasks, it determines task placement. For information about task placement and task placement strategies, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-placement.html\">Amazon ECS task placement</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "ServerException"
                 },
                 {
                     "shape": "ClientException"
                 },
@@ -304,15 +307,15 @@
             },
             "name": "DeleteService",
             "output": {
                 "shape": "DeleteServiceResponse"
             }
         },
         "DeleteTaskDefinitions": {
-            "documentation": "<p>Deletes one or more task definitions.</p> <p>You must deregister a task definition revision before you delete it. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_DeregisterTaskDefinition.html\">DeregisterTaskDefinition</a>.</p> <p>When you delete a task definition revision, it is immediately transitions from the <code>INACTIVE</code> to <code>DELETE_IN_PROGRESS</code>. Existing tasks and services that reference a <code>DELETE_IN_PROGRESS</code> task definition revision continue to run without disruption. Existing services that reference a <code>DELETE_IN_PROGRESS</code> task definition revision can still scale up or down by modifying the service's desired count.</p> <p>You can't use a <code>DELETE_IN_PROGRESS</code> task definition revision to run new tasks or create new services. You also can't update an existing service to reference a <code>DELETE_IN_PROGRESS</code> task definition revision.</p> <p> A task definition revision will stay in <code>DELETE_IN_PROGRESS</code> status until all the associated tasks and services have been terminated.</p>",
+            "documentation": "<p>Deletes one or more task definitions.</p> <p>You must deregister a task definition revision before you delete it. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_DeregisterTaskDefinition.html\">DeregisterTaskDefinition</a>.</p> <p>When you delete a task definition revision, it is immediately transitions from the <code>INACTIVE</code> to <code>DELETE_IN_PROGRESS</code>. Existing tasks and services that reference a <code>DELETE_IN_PROGRESS</code> task definition revision continue to run without disruption. Existing services that reference a <code>DELETE_IN_PROGRESS</code> task definition revision can still scale up or down by modifying the service's desired count.</p> <p>You can't use a <code>DELETE_IN_PROGRESS</code> task definition revision to run new tasks or create new services. You also can't update an existing service to reference a <code>DELETE_IN_PROGRESS</code> task definition revision.</p> <p> A task definition revision will stay in <code>DELETE_IN_PROGRESS</code> status until all the associated tasks and services have been terminated.</p> <p>When you delete all <code>INACTIVE</code> task definition revisions, the task definition name is not displayed in the console and not returned in the API. If a task definition revisions are in the <code>DELETE_IN_PROGRESS</code> state, the task definition name is displayed in the console and returned in the API. The task definition name is retained by Amazon ECS and the revision is incremented the next time you create a task definition with that name.</p>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "ClientException"
                 },
@@ -649,15 +652,15 @@
             },
             "name": "DiscoverPollEndpoint",
             "output": {
                 "shape": "DiscoverPollEndpointResponse"
             }
         },
         "ExecuteCommand": {
-            "documentation": "<p>Runs a command remotely on a container within a task.</p> <p>If you use a condition key in your IAM policy to refine the conditions for the policy statement, for example limit the actions to a specific cluster, you receive an <code>AccessDeniedException</code> when there is a mismatch between the condition key value and the corresponding parameter value.</p> <p>For information about required permissions and considerations, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-exec.htm\">Using Amazon ECS Exec for debugging</a> in the <i>Amazon ECS Developer Guide</i>. </p>",
+            "documentation": "<p>Runs a command remotely on a container within a task.</p> <p>If you use a condition key in your IAM policy to refine the conditions for the policy statement, for example limit the actions to a specific cluster, you receive an <code>AccessDeniedException</code> when there is a mismatch between the condition key value and the corresponding parameter value.</p> <p>For information about required permissions and considerations, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-exec.html\">Using Amazon ECS Exec for debugging</a> in the <i>Amazon ECS Developer Guide</i>. </p>",
             "errors": [
                 {
                     "shape": "ServerException"
                 },
                 {
                     "shape": "ClientException"
                 },
@@ -985,15 +988,15 @@
             },
             "name": "ListTasks",
             "output": {
                 "shape": "ListTasksResponse"
             }
         },
         "PutAccountSetting": {
-            "documentation": "<p>Modifies an account setting. Account settings are set on a per-Region basis.</p> <p>If you change the account setting for the root user, the default settings for all of the users and roles that no individual account setting was specified are reset for. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-account-settings.html\">Account Settings</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>When <code>serviceLongArnFormat</code>, <code>taskLongArnFormat</code>, or <code>containerInstanceLongArnFormat</code> are specified, the Amazon Resource Name (ARN) and resource ID format of the resource type for a specified user, role, or the root user for an account is affected. The opt-in and opt-out account setting must be set for each Amazon ECS resource separately. The ARN and resource ID format of a resource is defined by the opt-in status of the user or role that created the resource. You must turn on this setting to use Amazon ECS features such as resource tagging.</p> <p>When <code>awsvpcTrunking</code> is specified, the elastic network interface (ENI) limit for any new container instances that support the feature is changed. If <code>awsvpcTrunking</code> is enabled, any new container instances that support the feature are launched have the increased ENI limits available to them. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/container-instance-eni.html\">Elastic Network Interface Trunking</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>When <code>containerInsights</code> is specified, the default setting indicating whether CloudWatch Container Insights is enabled for your clusters is changed. If <code>containerInsights</code> is enabled, any new clusters that are created will have Container Insights enabled unless you disable it during cluster creation. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/cloudwatch-container-insights.html\">CloudWatch Container Insights</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+            "documentation": "<p>Modifies an account setting. Account settings are set on a per-Region basis.</p> <p>If you change the root user account setting, the default settings are reset for users and roles that do not have specified individual account settings. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-account-settings.html\">Account Settings</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>When <code>serviceLongArnFormat</code>, <code>taskLongArnFormat</code>, or <code>containerInstanceLongArnFormat</code> are specified, the Amazon Resource Name (ARN) and resource ID format of the resource type for a specified user, role, or the root user for an account is affected. The opt-in and opt-out account setting must be set for each Amazon ECS resource separately. The ARN and resource ID format of a resource is defined by the opt-in status of the user or role that created the resource. You must turn on this setting to use Amazon ECS features such as resource tagging.</p> <p>When <code>awsvpcTrunking</code> is specified, the elastic network interface (ENI) limit for any new container instances that support the feature is changed. If <code>awsvpcTrunking</code> is turned on, any new container instances that support the feature are launched have the increased ENI limits available to them. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/container-instance-eni.html\">Elastic Network Interface Trunking</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>When <code>containerInsights</code> is specified, the default setting indicating whether Amazon Web Services CloudWatch Container Insights is turned on for your clusters is changed. If <code>containerInsights</code> is turned on, any new clusters that are created will have Container Insights turned on unless you disable it during cluster creation. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/cloudwatch-container-insights.html\">CloudWatch Container Insights</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>Amazon ECS is introducing tagging authorization for resource creation. Users must have permissions for actions that create the resource, such as <code>ecsCreateCluster</code>. If tags are specified when you create a resource, Amazon Web Services performs additional authorization to verify if users or roles have permissions to create tags. Therefore, you must grant explicit permissions to use the <code>ecs:TagResource</code> action. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/supported-iam-actions-tagging.html\">Grant permission to tag resources on creation</a> in the <i>Amazon ECS Developer Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "ServerException"
                 },
                 {
                     "shape": "ClientException"
                 },
@@ -1147,15 +1150,15 @@
             },
             "name": "RegisterTaskDefinition",
             "output": {
                 "shape": "RegisterTaskDefinitionResponse"
             }
         },
         "RunTask": {
-            "documentation": "<p>Starts a new task using the specified task definition.</p> <p>You can allow Amazon ECS to place tasks for you, or you can customize how Amazon ECS places tasks using placement constraints and placement strategies. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/scheduling_tasks.html\">Scheduling Tasks</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>Alternatively, you can use <a>StartTask</a> to use your own scheduler or place tasks manually on specific container instances.</p> <p>The Amazon ECS API follows an eventual consistency model. This is because of the distributed nature of the system supporting the API. This means that the result of an API command you run that affects your Amazon ECS resources might not be immediately visible to all subsequent commands you run. Keep this in mind when you carry out an API command that immediately follows a previous API command.</p> <p>To manage eventual consistency, you can do the following:</p> <ul> <li> <p>Confirm the state of the resource before you run a command to modify it. Run the DescribeTasks command using an exponential backoff algorithm to ensure that you allow enough time for the previous command to propagate through the system. To do this, run the DescribeTasks command repeatedly, starting with a couple of seconds of wait time and increasing gradually up to five minutes of wait time.</p> </li> <li> <p>Add wait time between subsequent commands, even if the DescribeTasks command returns an accurate response. Apply an exponential backoff algorithm starting with a couple of seconds of wait time, and increase gradually up to about five minutes of wait time.</p> </li> </ul>",
+            "documentation": "<p>Starts a new task using the specified task definition.</p> <p>You can allow Amazon ECS to place tasks for you, or you can customize how Amazon ECS places tasks using placement constraints and placement strategies. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/scheduling_tasks.html\">Scheduling Tasks</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>Alternatively, you can use <a>StartTask</a> to use your own scheduler or place tasks manually on specific container instances.</p> <note> <p>Starting April 15, 2023, Amazon Web Services will not onboard new customers to Amazon Elastic Inference (EI), and will help current customers migrate their workloads to options that offer better price and performance. After April 15, 2023, new customers will not be able to launch instances with Amazon EI accelerators in Amazon SageMaker, Amazon ECS, or Amazon EC2. However, customers who have used Amazon EI at least once during the past 30-day period are considered current customers and will be able to continue using the service. </p> </note> <p>The Amazon ECS API follows an eventual consistency model. This is because of the distributed nature of the system supporting the API. This means that the result of an API command you run that affects your Amazon ECS resources might not be immediately visible to all subsequent commands you run. Keep this in mind when you carry out an API command that immediately follows a previous API command.</p> <p>To manage eventual consistency, you can do the following:</p> <ul> <li> <p>Confirm the state of the resource before you run a command to modify it. Run the DescribeTasks command using an exponential backoff algorithm to ensure that you allow enough time for the previous command to propagate through the system. To do this, run the DescribeTasks command repeatedly, starting with a couple of seconds of wait time and increasing gradually up to five minutes of wait time.</p> </li> <li> <p>Add wait time between subsequent commands, even if the DescribeTasks command returns an accurate response. Apply an exponential backoff algorithm starting with a couple of seconds of wait time, and increase gradually up to about five minutes of wait time.</p> </li> </ul>",
             "errors": [
                 {
                     "shape": "ServerException"
                 },
                 {
                     "shape": "ClientException"
                 },
@@ -1190,15 +1193,15 @@
             },
             "name": "RunTask",
             "output": {
                 "shape": "RunTaskResponse"
             }
         },
         "StartTask": {
-            "documentation": "<p>Starts a new task from the specified task definition on the specified container instance or instances.</p> <p>Alternatively, you can use <a>RunTask</a> to place tasks for you. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/scheduling_tasks.html\">Scheduling Tasks</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+            "documentation": "<p>Starts a new task from the specified task definition on the specified container instance or instances.</p> <note> <p>Starting April 15, 2023, Amazon Web Services will not onboard new customers to Amazon Elastic Inference (EI), and will help current customers migrate their workloads to options that offer better price and performance. After April 15, 2023, new customers will not be able to launch instances with Amazon EI accelerators in Amazon SageMaker, Amazon ECS, or Amazon EC2. However, customers who have used Amazon EI at least once during the past 30-day period are considered current customers and will be able to continue using the service. </p> </note> <p>Alternatively, you can use <a>RunTask</a> to place tasks for you. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/scheduling_tasks.html\">Scheduling Tasks</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "ServerException"
                 },
                 {
                     "shape": "ClientException"
                 },
@@ -1427,14 +1430,17 @@
                     "shape": "ClientException"
                 },
                 {
                     "shape": "ClusterNotFoundException"
                 },
                 {
                     "shape": "InvalidParameterException"
+                },
+                {
+                    "shape": "NamespaceNotFoundException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -1624,15 +1630,15 @@
             },
             "name": "UpdateServicePrimaryTaskSet",
             "output": {
                 "shape": "UpdateServicePrimaryTaskSetResponse"
             }
         },
         "UpdateTaskProtection": {
-            "documentation": "<p>Updates the protection status of a task. You can set <code>protectionEnabled</code> to <code>true</code> to protect your task from termination during scale-in events from <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-auto-scaling.html\">Service Autoscaling</a> or <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-types.html\">deployments</a>.</p> <p>Task-protection, by default, expires after 2 hours at which point Amazon ECS unsets the <code>protectionEnabled</code> property making the task eligible for termination by a subsequent scale-in event.</p> <p>You can specify a custom expiration period for task protection from 1 minute to up to 2,880 minutes (48 hours). To specify the custom expiration period, set the <code>expiresInMinutes</code> property. The <code>expiresInMinutes</code> property is always reset when you invoke this operation for a task that already has <code>protectionEnabled</code> set to <code>true</code>. You can keep extending the protection expiration period of a task by invoking this operation repeatedly.</p> <p>To learn more about Amazon ECS task protection, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-scale-in-protection.html\">Task scale-in protection</a> in the <i> <i>Amazon Elastic Container Service Developer Guide</i> </i>.</p> <note> <p>This operation is only supported for tasks belonging to an Amazon ECS service. Invoking this operation for a standalone task will result in an <code>TASK_NOT_VALID</code> failure. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/api_failures_messages.html\">API failure reasons</a>.</p> </note> <important> <p>If you prefer to set task protection from within the container, we recommend using the <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-scale-in-protection-endpoint.html\">Task scale-in protection endpoint</a>.</p> </important>",
+            "documentation": "<p>Updates the protection status of a task. You can set <code>protectionEnabled</code> to <code>true</code> to protect your task from termination during scale-in events from <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-auto-scaling.html\">Service Autoscaling</a> or <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-types.html\">deployments</a>.</p> <p>Task-protection, by default, expires after 2 hours at which point Amazon ECS clears the <code>protectionEnabled</code> property making the task eligible for termination by a subsequent scale-in event.</p> <p>You can specify a custom expiration period for task protection from 1 minute to up to 2,880 minutes (48 hours). To specify the custom expiration period, set the <code>expiresInMinutes</code> property. The <code>expiresInMinutes</code> property is always reset when you invoke this operation for a task that already has <code>protectionEnabled</code> set to <code>true</code>. You can keep extending the protection expiration period of a task by invoking this operation repeatedly.</p> <p>To learn more about Amazon ECS task protection, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-scale-in-protection.html\">Task scale-in protection</a> in the <i> <i>Amazon Elastic Container Service Developer Guide</i> </i>.</p> <note> <p>This operation is only supported for tasks belonging to an Amazon ECS service. Invoking this operation for a standalone task will result in an <code>TASK_NOT_VALID</code> failure. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/api_failures_messages.html\">API failure reasons</a>.</p> </note> <important> <p>If you prefer to set task protection from within the container, we recommend using the <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-scale-in-protection-endpoint.html\">Task scale-in protection endpoint</a>.</p> </important>",
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "ClientException"
                 },
@@ -1844,15 +1850,15 @@
                     "shape": "String"
                 },
                 "managedScaling": {
                     "documentation": "<p>The managed scaling settings for the Auto Scaling group capacity provider.</p>",
                     "shape": "ManagedScaling"
                 },
                 "managedTerminationProtection": {
-                    "documentation": "<p>The managed termination protection setting to use for the Auto Scaling group capacity provider. This determines whether the Auto Scaling group has managed termination protection. The default is off.</p> <important> <p>When using managed termination protection, managed scaling must also be used otherwise managed termination protection doesn't work.</p> </important> <p>When managed termination protection is on, Amazon ECS prevents the Amazon EC2 instances in an Auto Scaling group that contain tasks from being terminated during a scale-in action. The Auto Scaling group and each instance in the Auto Scaling group must have instance protection from scale-in actions enabled as well. For more information, see <a href=\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-instance-termination.html#instance-protection\">Instance Protection</a> in the <i>Auto Scaling User Guide</i>.</p> <p>When managed termination protection is off, your Amazon EC2 instances aren't protected from termination when the Auto Scaling group scales in.</p>",
+                    "documentation": "<p>The managed termination protection setting to use for the Auto Scaling group capacity provider. This determines whether the Auto Scaling group has managed termination protection. The default is off.</p> <important> <p>When using managed termination protection, managed scaling must also be used otherwise managed termination protection doesn't work.</p> </important> <p>When managed termination protection is on, Amazon ECS prevents the Amazon EC2 instances in an Auto Scaling group that contain tasks from being terminated during a scale-in action. The Auto Scaling group and each instance in the Auto Scaling group must have instance protection from scale-in actions on as well. For more information, see <a href=\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-instance-termination.html#instance-protection\">Instance Protection</a> in the <i>Auto Scaling User Guide</i>.</p> <p>When managed termination protection is off, your Amazon EC2 instances aren't protected from termination when the Auto Scaling group scales in.</p>",
                     "shape": "ManagedTerminationProtection"
                 }
             },
             "required": [
                 "autoScalingGroupArn"
             ],
             "type": "structure"
@@ -2163,32 +2169,32 @@
             },
             "type": "structure"
         },
         "ClusterServiceConnectDefaultsRequest": {
             "documentation": "<p>Use this parameter to set a default Service Connect namespace. After you set a default Service Connect namespace, any new services with Service Connect turned on that are created in the cluster are added as client services in the namespace. This setting only applies to new services that set the <code>enabled</code> parameter to <code>true</code> in the <code>ServiceConnectConfiguration</code>. You can set the namespace of each service individually in the <code>ServiceConnectConfiguration</code> to override this default parameter.</p> <p>Tasks that run in a namespace can use short names to connect to services in the namespace. Tasks can connect to services across all of the clusters in the namespace. Tasks connect through a managed proxy container that collects logs and metrics for increased visibility. Only the tasks that Amazon ECS services create are supported with Service Connect. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-connect.html\">Service Connect</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "members": {
                 "namespace": {
-                    "documentation": "<p>The namespace name or full Amazon Resource Name (ARN) of the Cloud Map namespace that's used when you create a service and don't specify a Service Connect configuration. The namespace name can include up to 1024 characters. The name is case-sensitive. The name can't include hyphens (-), tilde (~), greater than (&gt;), less than (&lt;), or slash (/).</p> <p>If you enter an existing namespace name or ARN, then that namespace will be used. Any namespace type is supported. The namespace must be in this account and this Amazon Web Services Region.</p> <p>If you enter a new name, a Cloud Map namespace will be created. Amazon ECS creates a Cloud Map namespace with the \"API calls\" method of instance discovery only. This instance discovery method is the \"HTTP\" namespace type in the Command Line Interface. Other types of instance discovery aren't used by Service Connect.</p> <p>If you update the service with an empty string <code>\"\"</code> for the namespace name, the cluster configuration for Service Connect is removed. Note that the namespace will remain in Cloud Map and must be deleted separately.</p> <p>For more information about Cloud Map, see <a href=\"https://docs.aws.amazon.com/\">Working with Services</a> in the <i>Cloud Map Developer Guide</i>.</p>",
+                    "documentation": "<p>The namespace name or full Amazon Resource Name (ARN) of the Cloud Map namespace that's used when you create a service and don't specify a Service Connect configuration. The namespace name can include up to 1024 characters. The name is case-sensitive. The name can't include hyphens (-), tilde (~), greater than (&gt;), less than (&lt;), or slash (/).</p> <p>If you enter an existing namespace name or ARN, then that namespace will be used. Any namespace type is supported. The namespace must be in this account and this Amazon Web Services Region.</p> <p>If you enter a new name, a Cloud Map namespace will be created. Amazon ECS creates a Cloud Map namespace with the \"API calls\" method of instance discovery only. This instance discovery method is the \"HTTP\" namespace type in the Command Line Interface. Other types of instance discovery aren't used by Service Connect.</p> <p>If you update the service with an empty string <code>\"\"</code> for the namespace name, the cluster configuration for Service Connect is removed. Note that the namespace will remain in Cloud Map and must be deleted separately.</p> <p>For more information about Cloud Map, see <a href=\"https://docs.aws.amazon.com/cloud-map/latest/dg/working-with-services.html\">Working with Services</a> in the <i>Cloud Map Developer Guide</i>.</p>",
                     "shape": "String"
                 }
             },
             "required": [
                 "namespace"
             ],
             "type": "structure"
         },
         "ClusterSetting": {
             "documentation": "<p>The settings to use when creating a cluster. This parameter is used to turn on CloudWatch Container Insights for a cluster.</p>",
             "members": {
                 "name": {
-                    "documentation": "<p>The name of the cluster setting. The only supported value is <code>containerInsights</code>.</p>",
+                    "documentation": "<p>The name of the cluster setting. The value is <code>containerInsights</code> .</p>",
                     "shape": "ClusterSettingName"
                 },
                 "value": {
-                    "documentation": "<p>The value to set for the cluster setting. The supported values are <code>enabled</code> and <code>disabled</code>. If <code>enabled</code> is specified, CloudWatch Container Insights will be enabled for the cluster, otherwise it will be off unless the <code>containerInsights</code> account setting is turned on. If a cluster value is specified, it will override the <code>containerInsights</code> value set with <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_PutAccountSetting.html\">PutAccountSetting</a> or <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_PutAccountSettingDefault.html\">PutAccountSettingDefault</a>.</p>",
+                    "documentation": "<p>The value to set for the cluster setting. The supported values are <code>enabled</code> and <code>disabled</code>. </p> <p>If you set <code>name</code> to <code>containerInsights</code> and <code>value</code> to <code>enabled</code>, CloudWatch Container Insights will be on for the cluster, otherwise it will be off unless the <code>containerInsights</code> account setting is turned on. If a cluster value is specified, it will override the <code>containerInsights</code> value set with <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_PutAccountSetting.html\">PutAccountSetting</a> or <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_PutAccountSettingDefault.html\">PutAccountSettingDefault</a>.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "ClusterSettingName": {
             "enum": [
@@ -2253,15 +2259,15 @@
                     "shape": "HealthStatus"
                 },
                 "image": {
                     "documentation": "<p>The image used for the container.</p>",
                     "shape": "String"
                 },
                 "imageDigest": {
-                    "documentation": "<p>The container image manifest digest.</p> <note> <p>The <code>imageDigest</code> is only returned if the container is using an image hosted in Amazon ECR, otherwise it is omitted.</p> </note>",
+                    "documentation": "<p>The container image manifest digest.</p>",
                     "shape": "String"
                 },
                 "lastStatus": {
                     "documentation": "<p>The last known status of the container.</p>",
                     "shape": "String"
                 },
                 "managedAgents": {
@@ -2319,14 +2325,18 @@
                     "documentation": "<p>The command that's passed to the container. This parameter maps to <code>Cmd</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>COMMAND</code> parameter to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>. For more information, see <a href=\"https://docs.docker.com/engine/reference/builder/#cmd\">https://docs.docker.com/engine/reference/builder/#cmd</a>. If there are multiple arguments, each argument is a separated string in the array.</p>",
                     "shape": "StringList"
                 },
                 "cpu": {
                     "documentation": "<p>The number of <code>cpu</code> units reserved for the container. This parameter maps to <code>CpuShares</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--cpu-shares</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>.</p> <p>This field is optional for tasks using the Fargate launch type, and the only requirement is that the total amount of CPU reserved for all containers within a task be lower than the task-level <code>cpu</code> value.</p> <note> <p>You can determine the number of CPU units that are available per EC2 instance type by multiplying the vCPUs listed for that instance type on the <a href=\"http://aws.amazon.com/ec2/instance-types/\">Amazon EC2 Instances</a> detail page by 1,024.</p> </note> <p>Linux containers share unallocated CPU units with other containers on the container instance with the same ratio as their allocated amount. For example, if you run a single-container task on a single-core instance type with 512 CPU units specified for that container, and that's the only task running on the container instance, that container could use the full 1,024 CPU unit share at any given time. However, if you launched another copy of the same task on that container instance, each task is guaranteed a minimum of 512 CPU units when needed. Moreover, each container could float to higher CPU usage if the other container was not using it. If both tasks were 100% active all of the time, they would be limited to 512 CPU units.</p> <p>On Linux container instances, the Docker daemon on the container instance uses the CPU value to calculate the relative CPU share ratios for running containers. For more information, see <a href=\"https://docs.docker.com/engine/reference/run/#cpu-share-constraint\">CPU share constraint</a> in the Docker documentation. The minimum valid CPU share value that the Linux kernel allows is 2. However, the CPU parameter isn't required, and you can use CPU values below 2 in your container definitions. For CPU values below 2 (including null), the behavior varies based on your Amazon ECS container agent version:</p> <ul> <li> <p> <b>Agent versions less than or equal to 1.1.0:</b> Null and zero CPU values are passed to Docker as 0, which Docker then converts to 1,024 CPU shares. CPU values of 1 are passed to Docker as 1, which the Linux kernel converts to two CPU shares.</p> </li> <li> <p> <b>Agent versions greater than or equal to 1.2.0:</b> Null, zero, and CPU values of 1 are passed to Docker as 2.</p> </li> </ul> <p>On Windows container instances, the CPU limit is enforced as an absolute limit, or a quota. Windows containers only have access to the specified amount of CPU that's described in the task definition. A null or zero CPU value is passed to Docker as <code>0</code>, which Windows interprets as 1% of one CPU.</p>",
                     "shape": "Integer"
                 },
+                "credentialSpecs": {
+                    "documentation": "<p>A list of ARNs in SSM or Amazon S3 to a credential spec (<code>credspec</code>code&gt;) file that configures a container for Active Directory authentication. This parameter is only used with domainless authentication.</p> <p>The format for each ARN is <code>credentialspecdomainless:MyARN</code>. Replace <code>MyARN</code> with the ARN in SSM or Amazon S3.</p> <p>The <code>credspec</code> must provide a ARN in Secrets Manager for a secret containing the username, password, and the domain to connect to. For better security, the instance isn't joined to the domain for domainless authentication. Other applications on the instance can't use the domainless credentials. You can use this parameter to run tasks on the same instance, even it the tasks need to join different domains. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/windows-gmsa.html\">Using gMSAs for Windows Containers</a> and <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/linux-gmsa.html\">Using gMSAs for Linux Containers</a>.</p>",
+                    "shape": "StringList"
+                },
                 "dependsOn": {
                     "documentation": "<p>The dependencies defined for container startup and shutdown. A container can contain multiple dependencies on other containers in a task definition. When a dependency is defined for container startup, for container shutdown it is reversed.</p> <p>For tasks using the EC2 launch type, the container instances require at least version 1.26.0 of the container agent to turn on container dependencies. However, we recommend using the latest container agent version. For information about checking your agent version and updating to the latest version, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-update.html\">Updating the Amazon ECS Container Agent</a> in the <i>Amazon Elastic Container Service Developer Guide</i>. If you're using an Amazon ECS-optimized Linux AMI, your instance needs at least version 1.26.0-1 of the <code>ecs-init</code> package. If your container instances are launched from version <code>20190301</code> or later, then they contain the required versions of the container agent and <code>ecs-init</code>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-optimized_AMI.html\">Amazon ECS-optimized Linux AMI</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>For tasks using the Fargate launch type, the task or service requires the following platforms:</p> <ul> <li> <p>Linux platform version <code>1.3.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul>",
                     "shape": "ContainerDependencies"
                 },
                 "disableNetworking": {
                     "documentation": "<p>When this parameter is true, networking is off within the container. This parameter maps to <code>NetworkDisabled</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a>.</p> <note> <p>This parameter is not supported for Windows containers.</p> </note>",
                     "shape": "BoxedBoolean"
@@ -2340,15 +2350,15 @@
                     "shape": "StringList"
                 },
                 "dockerLabels": {
                     "documentation": "<p>A key/value map of labels to add to the container. This parameter maps to <code>Labels</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--label</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>. This parameter requires version 1.18 of the Docker Remote API or greater on your container instance. To check the Docker Remote API version on your container instance, log in to your container instance and run the following command: <code>sudo docker version --format '{{.Server.APIVersion}}'</code> </p>",
                     "shape": "DockerLabelsMap"
                 },
                 "dockerSecurityOptions": {
-                    "documentation": "<p>A list of strings to provide custom labels for SELinux and AppArmor multi-level security systems. This field isn't valid for containers in tasks using the Fargate launch type.</p> <p>With Windows containers, this parameter can be used to reference a credential spec file when configuring a container for Active Directory authentication. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/windows-gmsa.html\">Using gMSAs for Windows Containers</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>This parameter maps to <code>SecurityOpt</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--security-opt</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>.</p> <note> <p>The Amazon ECS container agent running on a container instance must register with the <code>ECS_SELINUX_CAPABLE=true</code> or <code>ECS_APPARMOR_CAPABLE=true</code> environment variables before containers placed on that instance can use these security options. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-config.html\">Amazon ECS Container Agent Configuration</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </note> <p>For more information about valid values, see <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">Docker Run Security Configuration</a>. </p> <p>Valid values: \"no-new-privileges\" | \"apparmor:PROFILE\" | \"label:value\" | \"credentialspec:CredentialSpecFilePath\"</p>",
+                    "documentation": "<p>A list of strings to provide custom configuration for multiple security systems. For more information about valid values, see <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">Docker Run Security Configuration</a>. This field isn't valid for containers in tasks using the Fargate launch type.</p> <p>For Linux tasks on EC2, this parameter can be used to reference custom labels for SELinux and AppArmor multi-level security systems.</p> <p>For any tasks on EC2, this parameter can be used to reference a credential spec file that configures a container for Active Directory authentication. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/windows-gmsa.html\">Using gMSAs for Windows Containers</a> and <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/linux-gmsa.html\">Using gMSAs for Linux Containers</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>This parameter maps to <code>SecurityOpt</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--security-opt</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>.</p> <note> <p>The Amazon ECS container agent running on a container instance must register with the <code>ECS_SELINUX_CAPABLE=true</code> or <code>ECS_APPARMOR_CAPABLE=true</code> environment variables before containers placed on that instance can use these security options. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-config.html\">Amazon ECS Container Agent Configuration</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </note> <p>For more information about valid values, see <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">Docker Run Security Configuration</a>. </p> <p>Valid values: \"no-new-privileges\" | \"apparmor:PROFILE\" | \"label:value\" | \"credentialspec:CredentialSpecFilePath\"</p>",
                     "shape": "StringList"
                 },
                 "entryPoint": {
                     "documentation": "<important> <p>Early versions of the Amazon ECS container agent don't properly handle <code>entryPoint</code> parameters. If you have problems using <code>entryPoint</code>, update your container agent or enter your commands and arguments as <code>command</code> array items instead.</p> </important> <p>The entry point that's passed to the container. This parameter maps to <code>Entrypoint</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--entrypoint</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>. For more information, see <a href=\"https://docs.docker.com/engine/reference/builder/#entrypoint\">https://docs.docker.com/engine/reference/builder/#entrypoint</a>.</p>",
                     "shape": "StringList"
                 },
                 "environment": {
@@ -2806,23 +2816,23 @@
                     "shape": "DeploymentConfiguration"
                 },
                 "deploymentController": {
                     "documentation": "<p>The deployment controller to use for the service. If no deployment controller is specified, the default value of <code>ECS</code> is used.</p>",
                     "shape": "DeploymentController"
                 },
                 "desiredCount": {
-                    "documentation": "<p>The number of instantiations of the specified task definition to place and keep running on your cluster.</p> <p>This is required if <code>schedulingStrategy</code> is <code>REPLICA</code> or isn't specified. If <code>schedulingStrategy</code> is <code>DAEMON</code> then this isn't required.</p>",
+                    "documentation": "<p>The number of instantiations of the specified task definition to place and keep running in your service.</p> <p>This is required if <code>schedulingStrategy</code> is <code>REPLICA</code> or isn't specified. If <code>schedulingStrategy</code> is <code>DAEMON</code> then this isn't required.</p>",
                     "shape": "BoxedInteger"
                 },
                 "enableECSManagedTags": {
-                    "documentation": "<p>Specifies whether to turn on Amazon ECS managed tags for the tasks within the service. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-using-tags.html\">Tagging your Amazon ECS resources</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+                    "documentation": "<p>Specifies whether to turn on Amazon ECS managed tags for the tasks within the service. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-using-tags.html\">Tagging your Amazon ECS resources</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>When you use Amazon ECS managed tags, you need to set the <code>propagateTags</code> request parameter.</p>",
                     "shape": "Boolean"
                 },
                 "enableExecuteCommand": {
-                    "documentation": "<p>Determines whether the execute command functionality is enabled for the service. If <code>true</code>, this enables execute command functionality on all containers in the service tasks.</p>",
+                    "documentation": "<p>Determines whether the execute command functionality is turned on for the service. If <code>true</code>, this enables execute command functionality on all containers in the service tasks.</p>",
                     "shape": "Boolean"
                 },
                 "healthCheckGracePeriodSeconds": {
                     "documentation": "<p>The period of time, in seconds, that the Amazon ECS service scheduler ignores unhealthy Elastic Load Balancing target health checks after a task has first started. This is only used when your service is configured to use a load balancer. If your service has a load balancer defined and you don't specify a health check grace period value, the default value of <code>0</code> is used.</p> <p>If you do not use an Elastic Load Balancing, we recommend that you use the <code>startPeriod</code> in the task definition health check parameters. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_HealthCheck.html\">Health check</a>.</p> <p>If your service's tasks take a while to start and respond to Elastic Load Balancing health checks, you can specify a health check grace period of up to 2,147,483,647 seconds (about 69 years). During that time, the Amazon ECS service scheduler ignores health check status. This grace period can prevent the service scheduler from marking tasks as unhealthy and stopping them before they have time to come up.</p>",
                     "shape": "BoxedInteger"
                 },
                 "launchType": {
@@ -2846,15 +2856,15 @@
                     "shape": "PlacementStrategies"
                 },
                 "platformVersion": {
                     "documentation": "<p>The platform version that your tasks in the service are running on. A platform version is specified only for tasks using the Fargate launch type. If one isn't specified, the <code>LATEST</code> platform version is used. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html\">Fargate platform versions</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "String"
                 },
                 "propagateTags": {
-                    "documentation": "<p>Specifies whether to propagate the tags from the task definition to the task. If no value is specified, the tags aren't propagated. Tags can only be propagated to the task during task creation. To add tags to a task after task creation, use the <a>TagResource</a> API action.</p>",
+                    "documentation": "<p>Specifies whether to propagate the tags from the task definition to the task. If no value is specified, the tags aren't propagated. Tags can only be propagated to the task during task creation. To add tags to a task after task creation, use the <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_TagResource.html\">TagResource</a> API action.</p> <p>The default is <code>NONE</code>.</p>",
                     "shape": "PropagateTags"
                 },
                 "role": {
                     "documentation": "<p>The name or full Amazon Resource Name (ARN) of the IAM role that allows Amazon ECS to make calls to your load balancer on your behalf. This parameter is only permitted if you are using a load balancer with your service and your task definition doesn't use the <code>awsvpc</code> network mode. If you specify the <code>role</code> parameter, you must also specify a load balancer object with the <code>loadBalancers</code> parameter.</p> <important> <p>If your account has already created the Amazon ECS service-linked role, that role is used for your service unless you specify a role here. The service-linked role is required if your task definition uses the <code>awsvpc</code> network mode or if the service is configured to use service discovery, an external deployment controller, multiple target groups, or Elastic Inference accelerators in which case you don't specify a role here. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/using-service-linked-roles.html\">Using service-linked roles for Amazon ECS</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> </important> <p>If your specified role has a path other than <code>/</code>, then you must either specify the full role ARN (this is recommended) or prefix the role name with the path. For example, if a role with the name <code>bar</code> has a path of <code>/foo/</code> then you would specify <code>/foo/bar</code> as the role name. For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_identifiers.html#identifiers-friendly-names\">Friendly names and paths</a> in the <i>IAM User Guide</i>.</p>",
                     "shape": "String"
                 },
                 "schedulingStrategy": {
@@ -2874,15 +2884,15 @@
                     "shape": "ServiceRegistries"
                 },
                 "tags": {
                     "documentation": "<p>The metadata that you apply to the service to help you categorize and organize them. Each tag consists of a key and an optional value, both of which you define. When a service is deleted, the tags are deleted as well.</p> <p>The following basic restrictions apply to tags:</p> <ul> <li> <p>Maximum number of tags per resource - 50</p> </li> <li> <p>For each resource, each tag key must be unique, and each tag key can have only one value.</p> </li> <li> <p>Maximum key length - 128 Unicode characters in UTF-8</p> </li> <li> <p>Maximum value length - 256 Unicode characters in UTF-8</p> </li> <li> <p>If your tagging schema is used across multiple services and resources, remember that other services may have restrictions on allowed characters. Generally allowed characters are: letters, numbers, and spaces representable in UTF-8, and the following characters: + - = . _ : / @.</p> </li> <li> <p>Tag keys and values are case-sensitive.</p> </li> <li> <p>Do not use <code>aws:</code>, <code>AWS:</code>, or any upper or lowercase combination of such as a prefix for either keys or values as it is reserved for Amazon Web Services use. You cannot edit or delete tag keys or values with this prefix. Tags with this prefix do not count against your tags per resource limit.</p> </li> </ul>",
                     "shape": "Tags"
                 },
                 "taskDefinition": {
-                    "documentation": "<p>The <code>family</code> and <code>revision</code> (<code>family:revision</code>) or full ARN of the task definition to run in your service. If a <code>revision</code> isn't specified, the latest <code>ACTIVE</code> revision is used.</p> <p>A task definition must be specified if the service uses either the <code>ECS</code> or <code>CODE_DEPLOY</code> deployment controllers.</p>",
+                    "documentation": "<p>The <code>family</code> and <code>revision</code> (<code>family:revision</code>) or full ARN of the task definition to run in your service. If a <code>revision</code> isn't specified, the latest <code>ACTIVE</code> revision is used.</p> <p>A task definition must be specified if the service uses either the <code>ECS</code> or <code>CODE_DEPLOY</code> deployment controllers.</p> <p>For more information about deployment types, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-types.html\">Amazon ECS deployment types</a>.</p>",
                     "shape": "String"
                 }
             },
             "required": [
                 "serviceName"
             ],
             "type": "structure"
@@ -3188,15 +3198,15 @@
                     "shape": "String"
                 },
                 "platformVersion": {
                     "documentation": "<p>The platform version that your tasks in the service run on. A platform version is only specified for tasks using the Fargate launch type. If one isn't specified, the <code>LATEST</code> platform version is used. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html\">Fargate Platform Versions</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "String"
                 },
                 "rolloutState": {
-                    "documentation": "<note> <p>The <code>rolloutState</code> of a service is only returned for services that use the rolling update (<code>ECS</code>) deployment type that aren't behind a Classic Load Balancer.</p> </note> <p>The rollout state of the deployment. When a service deployment is started, it begins in an <code>IN_PROGRESS</code> state. When the service reaches a steady state, the deployment transitions to a <code>COMPLETED</code> state. If the service fails to reach a steady state and circuit breaker is enabled, the deployment transitions to a <code>FAILED</code> state. A deployment in <code>FAILED</code> state doesn't launch any new tasks. For more information, see <a>DeploymentCircuitBreaker</a>.</p>",
+                    "documentation": "<note> <p>The <code>rolloutState</code> of a service is only returned for services that use the rolling update (<code>ECS</code>) deployment type that aren't behind a Classic Load Balancer.</p> </note> <p>The rollout state of the deployment. When a service deployment is started, it begins in an <code>IN_PROGRESS</code> state. When the service reaches a steady state, the deployment transitions to a <code>COMPLETED</code> state. If the service fails to reach a steady state and circuit breaker is turned on, the deployment transitions to a <code>FAILED</code> state. A deployment in <code>FAILED</code> state doesn't launch any new tasks. For more information, see <a>DeploymentCircuitBreaker</a>.</p>",
                     "shape": "DeploymentRolloutState"
                 },
                 "rolloutStateReason": {
                     "documentation": "<p>A description of the rollout state of a deployment.</p>",
                     "shape": "String"
                 },
                 "runningCount": {
@@ -3246,15 +3256,15 @@
                 "alarmNames",
                 "enable",
                 "rollback"
             ],
             "type": "structure"
         },
         "DeploymentCircuitBreaker": {
-            "documentation": "<note> <p>The deployment circuit breaker can only be used for services using the rolling update (<code>ECS</code>) deployment type.</p> </note> <p>The <b>deployment circuit breaker</b> determines whether a service deployment will fail if the service can't reach a steady state. If enabled, a service deployment will transition to a failed state and stop launching new tasks. You can also configure Amazon ECS to roll back your service to the last completed deployment after a failure. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-type-ecs.html\">Rolling update</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+            "documentation": "<note> <p>The deployment circuit breaker can only be used for services using the rolling update (<code>ECS</code>) deployment type.</p> </note> <p>The <b>deployment circuit breaker</b> determines whether a service deployment will fail if the service can't reach a steady state. If it is turned on, a service deployment will transition to a failed state and stop launching new tasks. You can also configure Amazon ECS to roll back your service to the last completed deployment after a failure. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/deployment-type-ecs.html\">Rolling update</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "members": {
                 "enable": {
                     "documentation": "<p>Determines whether to use the deployment circuit breaker logic for the service.</p>",
                     "shape": "Boolean"
                 },
                 "rollback": {
                     "documentation": "<p>Determines whether to configure Amazon ECS to roll back the service if a service deployment fails. If rollback is on, when a service deployment fails, the service is rolled back to the last deployment that completed successfully.</p>",
@@ -3721,19 +3731,19 @@
         "Double": {
             "type": "double"
         },
         "EFSAuthorizationConfig": {
             "documentation": "<p>The authorization configuration details for the Amazon EFS file system.</p>",
             "members": {
                 "accessPointId": {
-                    "documentation": "<p>The Amazon EFS access point ID to use. If an access point is specified, the root directory value specified in the <code>EFSVolumeConfiguration</code> must either be omitted or set to <code>/</code> which will enforce the path set on the EFS access point. If an access point is used, transit encryption must be enabled in the <code>EFSVolumeConfiguration</code>. For more information, see <a href=\"https://docs.aws.amazon.com/efs/latest/ug/efs-access-points.html\">Working with Amazon EFS access points</a> in the <i>Amazon Elastic File System User Guide</i>.</p>",
+                    "documentation": "<p>The Amazon EFS access point ID to use. If an access point is specified, the root directory value specified in the <code>EFSVolumeConfiguration</code> must either be omitted or set to <code>/</code> which will enforce the path set on the EFS access point. If an access point is used, transit encryption must be on in the <code>EFSVolumeConfiguration</code>. For more information, see <a href=\"https://docs.aws.amazon.com/efs/latest/ug/efs-access-points.html\">Working with Amazon EFS access points</a> in the <i>Amazon Elastic File System User Guide</i>.</p>",
                     "shape": "String"
                 },
                 "iam": {
-                    "documentation": "<p>Determines whether to use the Amazon ECS task role defined in a task definition when mounting the Amazon EFS file system. If enabled, transit encryption must be enabled in the <code>EFSVolumeConfiguration</code>. If this parameter is omitted, the default value of <code>DISABLED</code> is used. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/efs-volumes.html#efs-volume-accesspoints\">Using Amazon EFS access points</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+                    "documentation": "<p>Determines whether to use the Amazon ECS task role defined in a task definition when mounting the Amazon EFS file system. If it is turned on, transit encryption must be turned on in the <code>EFSVolumeConfiguration</code>. If this parameter is omitted, the default value of <code>DISABLED</code> is used. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/efs-volumes.html#efs-volume-accesspoints\">Using Amazon EFS access points</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "EFSAuthorizationConfigIAM"
                 }
             },
             "type": "structure"
         },
         "EFSAuthorizationConfigIAM": {
             "enum": [
@@ -3761,15 +3771,15 @@
                     "shape": "String"
                 },
                 "rootDirectory": {
                     "documentation": "<p>The directory within the Amazon EFS file system to mount as the root directory inside the host. If this parameter is omitted, the root of the Amazon EFS volume will be used. Specifying <code>/</code> will have the same effect as omitting this parameter.</p> <important> <p>If an EFS access point is specified in the <code>authorizationConfig</code>, the root directory parameter must either be omitted or set to <code>/</code> which will enforce the path set on the EFS access point.</p> </important>",
                     "shape": "String"
                 },
                 "transitEncryption": {
-                    "documentation": "<p>Determines whether to use encryption for Amazon EFS data in transit between the Amazon ECS host and the Amazon EFS server. Transit encryption must be enabled if Amazon EFS IAM authorization is used. If this parameter is omitted, the default value of <code>DISABLED</code> is used. For more information, see <a href=\"https://docs.aws.amazon.com/efs/latest/ug/encryption-in-transit.html\">Encrypting data in transit</a> in the <i>Amazon Elastic File System User Guide</i>.</p>",
+                    "documentation": "<p>Determines whether to use encryption for Amazon EFS data in transit between the Amazon ECS host and the Amazon EFS server. Transit encryption must be turned on if Amazon EFS IAM authorization is used. If this parameter is omitted, the default value of <code>DISABLED</code> is used. For more information, see <a href=\"https://docs.aws.amazon.com/efs/latest/ug/encryption-in-transit.html\">Encrypting data in transit</a> in the <i>Amazon Elastic File System User Guide</i>.</p>",
                     "shape": "EFSTransitEncryption"
                 },
                 "transitEncryptionPort": {
                     "documentation": "<p>The port to use when sending encrypted data between the Amazon ECS host and the Amazon EFS server. If you do not specify a transit encryption port, it will use the port selection strategy that the Amazon EFS mount helper uses. For more information, see <a href=\"https://docs.aws.amazon.com/efs/latest/ug/efs-mount-helper.html\">EFS mount helper</a> in the <i>Amazon Elastic File System User Guide</i>.</p>",
                     "shape": "BoxedInteger"
                 }
             },
@@ -3811,15 +3821,15 @@
         "EnvironmentVariables": {
             "member": {
                 "shape": "KeyValuePair"
             },
             "type": "list"
         },
         "EphemeralStorage": {
-            "documentation": "<p>The amount of ephemeral storage to allocate for the task. This parameter is used to expand the total amount of ephemeral storage available, beyond the default amount, for tasks hosted on Fargate. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/userguide/using_data_volumes.html\">Fargate task storage</a> in the <i>Amazon ECS User Guide for Fargate</i>.</p> <note> <p>This parameter is only supported for tasks hosted on Fargate using Linux platform version <code>1.4.0</code> or later. This parameter is not supported for Windows containers on Fargate.</p> </note>",
+            "documentation": "<p>The amount of ephemeral storage to allocate for the task. This parameter is used to expand the total amount of ephemeral storage available, beyond the default amount, for tasks hosted on Fargate. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/userguide/using_data_volumes.html\">Fargate task storage</a> in the <i>Amazon ECS User Guide for Fargate</i>.</p> <note> <p>For tasks using the Fargate launch type, the task requires the following platforms:</p> <ul> <li> <p>Linux platform version <code>1.4.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul> </note>",
             "members": {
                 "sizeInGiB": {
                     "documentation": "<p>The total amount, in GiB, of ephemeral storage to set for the task. The minimum supported value is <code>21</code> GiB and the maximum supported value is <code>200</code> GiB.</p>",
                     "shape": "Integer"
                 }
             },
             "required": [
@@ -4055,28 +4065,28 @@
         "GetTaskProtectionResponse": {
             "members": {
                 "failures": {
                     "documentation": "<p>Any failures associated with the call.</p>",
                     "shape": "Failures"
                 },
                 "protectedTasks": {
-                    "documentation": "<p>A list of tasks with the following information.</p> <ul> <li> <p> <code>taskArn</code>: The task ARN.</p> </li> <li> <p> <code>protectionEnabled</code>: The protection status of the task. If scale-in protection is enabled for a task, the value is <code>true</code>. Otherwise, it is <code>false</code>.</p> </li> <li> <p> <code>expirationDate</code>: The epoch time when protection for the task will expire.</p> </li> </ul>",
+                    "documentation": "<p>A list of tasks with the following information.</p> <ul> <li> <p> <code>taskArn</code>: The task ARN.</p> </li> <li> <p> <code>protectionEnabled</code>: The protection status of the task. If scale-in protection is turned on for a task, the value is <code>true</code>. Otherwise, it is <code>false</code>.</p> </li> <li> <p> <code>expirationDate</code>: The epoch time when protection for the task will expire.</p> </li> </ul>",
                     "shape": "ProtectedTasks"
                 }
             },
             "type": "structure"
         },
         "GpuIds": {
             "member": {
                 "shape": "String"
             },
             "type": "list"
         },
         "HealthCheck": {
-            "documentation": "<p>An object representing a container health check. Health check parameters that are specified in a container definition override any Docker health checks that exist in the container image (such as those specified in a parent image or from the image's Dockerfile).</p> <note> <p>The Amazon ECS container agent only monitors and reports on the health checks specified in the task definition. Amazon ECS does not monitor Docker health checks that are embedded in a container image and not specified in the container definition. Health check parameters that are specified in a container definition override any Docker health checks that exist in the container image.</p> </note> <p>You can view the health status of both individual containers and a task with the DescribeTasks API operation or when viewing the task details in the console.</p> <p>The following describes the possible <code>healthStatus</code> values for a container:</p> <ul> <li> <p> <code>HEALTHY</code>-The container health check has passed successfully.</p> </li> <li> <p> <code>UNHEALTHY</code>-The container health check has failed.</p> </li> <li> <p> <code>UNKNOWN</code>-The container health check is being evaluated or there's no container health check defined.</p> </li> </ul> <p>The following describes the possible <code>healthStatus</code> values for a task. The container health check status of nonessential containers only affects the health status of a task if no essential containers have health checks defined.</p> <ul> <li> <p> <code>HEALTHY</code>-All essential containers within the task have passed their health checks.</p> </li> <li> <p> <code>UNHEALTHY</code>-One or more essential containers have failed their health check.</p> </li> <li> <p> <code>UNKNOWN</code>-The essential containers within the task are still having their health checks evaluated or there are only nonessential containers with health checks defined.</p> </li> </ul> <p>If a task is run manually, and not as part of a service, the task will continue its lifecycle regardless of its health status. For tasks that are part of a service, if the task reports as unhealthy then the task will be stopped and the service scheduler will replace it.</p> <important> <p>For tasks that are a part of a service and the service uses the <code>ECS</code> rolling deployment type, the deployment is paused while the new tasks have the <code>UNKNOWN</code> task health check status. For example, tasks that define health checks for nonessential containers when no essential containers have health checks will have the <code>UNKNOWN</code> health check status indefinitely which prevents the deployment from completing.</p> </important> <p>The following are notes about container health check support:</p> <ul> <li> <p>Container health checks require version 1.17.0 or greater of the Amazon ECS container agent. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-update.html\">Updating the Amazon ECS container agent</a>.</p> </li> <li> <p>Container health checks are supported for Fargate tasks if you're using platform version <code>1.1.0</code> or greater. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html\">Fargate platform versions</a>.</p> </li> <li> <p>Container health checks aren't supported for tasks that are part of a service that's configured to use a Classic Load Balancer.</p> </li> </ul>",
+            "documentation": "<p>An object representing a container health check. Health check parameters that are specified in a container definition override any Docker health checks that exist in the container image (such as those specified in a parent image or from the image's Dockerfile). This configuration maps to the <code>HEALTHCHECK</code> parameter of <a href=\"https://docs.docker.com/engine/reference/run/\">docker run</a>.</p> <note> <p>The Amazon ECS container agent only monitors and reports on the health checks specified in the task definition. Amazon ECS does not monitor Docker health checks that are embedded in a container image and not specified in the container definition. Health check parameters that are specified in a container definition override any Docker health checks that exist in the container image.</p> </note> <p>You can view the health status of both individual containers and a task with the DescribeTasks API operation or when viewing the task details in the console.</p> <p>The health check is designed to make sure that your containers survive agent restarts, upgrades, or temporary unavailability.</p> <p>The following describes the possible <code>healthStatus</code> values for a container:</p> <ul> <li> <p> <code>HEALTHY</code>-The container health check has passed successfully.</p> </li> <li> <p> <code>UNHEALTHY</code>-The container health check has failed.</p> </li> <li> <p> <code>UNKNOWN</code>-The container health check is being evaluated or there's no container health check defined.</p> </li> </ul> <p>The following describes the possible <code>healthStatus</code> values for a task. The container health check status of non-essential containers don't have an effect on the health status of a task.</p> <ul> <li> <p> <code>HEALTHY</code>-All essential containers within the task have passed their health checks.</p> </li> <li> <p> <code>UNHEALTHY</code>-One or more essential containers have failed their health check.</p> </li> <li> <p> <code>UNKNOWN</code>-The essential containers within the task are still having their health checks evaluated, there are only nonessential containers with health checks defined, or there are no container health checks defined.</p> </li> </ul> <p>If a task is run manually, and not as part of a service, the task will continue its lifecycle regardless of its health status. For tasks that are part of a service, if the task reports as unhealthy then the task will be stopped and the service scheduler will replace it.</p> <p>The following are notes about container health check support:</p> <ul> <li> <p>When the Amazon ECS agent cannot connect to the Amazon ECS service, the service reports the container as <code>UNHEALTHY</code>. </p> </li> <li> <p>The health check statuses are the \"last heard from\" response from the Amazon ECS agent. There are no assumptions made about the status of the container health checks.</p> </li> <li> <p>Container health checks require version 1.17.0 or greater of the Amazon ECS container agent. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-update.html\">Updating the Amazon ECS container agent</a>.</p> </li> <li> <p>Container health checks are supported for Fargate tasks if you're using platform version <code>1.1.0</code> or greater. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html\">Fargate platform versions</a>.</p> </li> <li> <p>Container health checks aren't supported for tasks that are part of a service that's configured to use a Classic Load Balancer.</p> </li> </ul>",
             "members": {
                 "command": {
                     "documentation": "<p>A string array representing the command that the container runs to determine if it is healthy. The string array must start with <code>CMD</code> to run the command arguments directly, or <code>CMD-SHELL</code> to run the command with the container's default shell. </p> <p> When you use the Amazon Web Services Management Console JSON panel, the Command Line Interface, or the APIs, enclose the list of commands in double quotes and brackets.</p> <p> <code>[ \"CMD-SHELL\", \"curl -f http://localhost/ || exit 1\" ]</code> </p> <p>You don't include the double quotes and brackets when you use the Amazon Web Services Management Console.</p> <p> <code> CMD-SHELL, curl -f http://localhost/ || exit 1</code> </p> <p>An exit code of 0 indicates success, and non-zero exit code indicates failure. For more information, see <code>HealthCheck</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a>.</p>",
                     "shape": "StringList"
                 },
                 "interval": {
                     "documentation": "<p>The time period in seconds between each health check execution. You may specify between 5 and 300 seconds. The default value is 30 seconds.</p>",
@@ -4142,15 +4152,15 @@
             },
             "type": "structure"
         },
         "InferenceAccelerator": {
             "documentation": "<p>Details on an Elastic Inference accelerator. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-inference.html\">Working with Amazon Elastic Inference on Amazon ECS</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "members": {
                 "deviceName": {
-                    "documentation": "<p>The Elastic Inference accelerator device name. The <code>deviceName</code> must also be referenced in a container definition as a <a>ResourceRequirement</a>.</p>",
+                    "documentation": "<p>The Elastic Inference accelerator device name. The <code>deviceName</code> must also be referenced in a container definition as a <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_ResourceRequirement.html\">ResourceRequirement</a>.</p>",
                     "shape": "String"
                 },
                 "deviceType": {
                     "documentation": "<p>The Elastic Inference accelerator type to use.</p>",
                     "shape": "String"
                 }
             },
@@ -4285,38 +4295,38 @@
         "LimitExceededException": {
             "documentation": "<p>The limit for the resource was exceeded.</p>",
             "exception": true,
             "members": {},
             "type": "structure"
         },
         "LinuxParameters": {
-            "documentation": "<p>Linux-specific options that are applied to the container, such as Linux <a>KernelCapabilities</a>.</p>",
+            "documentation": "<p>The Linux-specific options that are applied to the container, such as Linux <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_KernelCapabilities.html\">KernelCapabilities</a>.</p>",
             "members": {
                 "capabilities": {
                     "documentation": "<p>The Linux capabilities for the container that are added to or dropped from the default configuration provided by Docker.</p> <note> <p>For tasks that use the Fargate launch type, <code>capabilities</code> is supported for all platform versions but the <code>add</code> parameter is only supported if using platform version 1.4.0 or later.</p> </note>",
                     "shape": "KernelCapabilities"
                 },
                 "devices": {
                     "documentation": "<p>Any host devices to expose to the container. This parameter maps to <code>Devices</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--device</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>.</p> <note> <p>If you're using tasks that use the Fargate launch type, the <code>devices</code> parameter isn't supported.</p> </note>",
                     "shape": "DevicesList"
                 },
                 "initProcessEnabled": {
                     "documentation": "<p>Run an <code>init</code> process inside the container that forwards signals and reaps processes. This parameter maps to the <code>--init</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>. This parameter requires version 1.25 of the Docker Remote API or greater on your container instance. To check the Docker Remote API version on your container instance, log in to your container instance and run the following command: <code>sudo docker version --format '{{.Server.APIVersion}}'</code> </p>",
                     "shape": "BoxedBoolean"
                 },
                 "maxSwap": {
-                    "documentation": "<p>The total amount of swap memory (in MiB) a container can use. This parameter will be translated to the <code>--memory-swap</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a> where the value would be the sum of the container memory plus the <code>maxSwap</code> value.</p> <p>If a <code>maxSwap</code> value of <code>0</code> is specified, the container will not use swap. Accepted values are <code>0</code> or any positive integer. If the <code>maxSwap</code> parameter is omitted, the container will use the swap configuration for the container instance it is running on. A <code>maxSwap</code> value must be set for the <code>swappiness</code> parameter to be used.</p> <note> <p>If you're using tasks that use the Fargate launch type, the <code>maxSwap</code> parameter isn't supported.</p> </note>",
+                    "documentation": "<p>The total amount of swap memory (in MiB) a container can use. This parameter will be translated to the <code>--memory-swap</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a> where the value would be the sum of the container memory plus the <code>maxSwap</code> value.</p> <p>If a <code>maxSwap</code> value of <code>0</code> is specified, the container will not use swap. Accepted values are <code>0</code> or any positive integer. If the <code>maxSwap</code> parameter is omitted, the container will use the swap configuration for the container instance it is running on. A <code>maxSwap</code> value must be set for the <code>swappiness</code> parameter to be used.</p> <note> <p>If you're using tasks that use the Fargate launch type, the <code>maxSwap</code> parameter isn't supported.</p> <p>If you're using tasks on Amazon Linux 2023 the <code>swappiness</code> parameter isn't supported.</p> </note>",
                     "shape": "BoxedInteger"
                 },
                 "sharedMemorySize": {
                     "documentation": "<p>The value for the size (in MiB) of the <code>/dev/shm</code> volume. This parameter maps to the <code>--shm-size</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>.</p> <note> <p>If you are using tasks that use the Fargate launch type, the <code>sharedMemorySize</code> parameter is not supported.</p> </note>",
                     "shape": "BoxedInteger"
                 },
                 "swappiness": {
-                    "documentation": "<p>This allows you to tune a container's memory swappiness behavior. A <code>swappiness</code> value of <code>0</code> will cause swapping to not happen unless absolutely necessary. A <code>swappiness</code> value of <code>100</code> will cause pages to be swapped very aggressively. Accepted values are whole numbers between <code>0</code> and <code>100</code>. If the <code>swappiness</code> parameter is not specified, a default value of <code>60</code> is used. If a value is not specified for <code>maxSwap</code> then this parameter is ignored. This parameter maps to the <code>--memory-swappiness</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>.</p> <note> <p>If you're using tasks that use the Fargate launch type, the <code>swappiness</code> parameter isn't supported.</p> </note>",
+                    "documentation": "<p>This allows you to tune a container's memory swappiness behavior. A <code>swappiness</code> value of <code>0</code> will cause swapping to not happen unless absolutely necessary. A <code>swappiness</code> value of <code>100</code> will cause pages to be swapped very aggressively. Accepted values are whole numbers between <code>0</code> and <code>100</code>. If the <code>swappiness</code> parameter is not specified, a default value of <code>60</code> is used. If a value is not specified for <code>maxSwap</code> then this parameter is ignored. This parameter maps to the <code>--memory-swappiness</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>.</p> <note> <p>If you're using tasks that use the Fargate launch type, the <code>swappiness</code> parameter isn't supported.</p> <p>If you're using tasks on Amazon Linux 2023 the <code>swappiness</code> parameter isn't supported.</p> </note>",
                     "shape": "BoxedInteger"
                 },
                 "tmpfs": {
                     "documentation": "<p>The container path, mount options, and size (in MiB) of the tmpfs mount. This parameter maps to the <code>--tmpfs</code> option to <a href=\"https://docs.docker.com/engine/reference/run/#security-configuration\">docker run</a>.</p> <note> <p>If you're using tasks that use the Fargate launch type, the <code>tmpfs</code> parameter isn't supported.</p> </note>",
                     "shape": "TmpfsList"
                 }
             },
@@ -4688,15 +4698,15 @@
                     "documentation": "<p>The list of task ARN entries for the <code>ListTasks</code> request.</p>",
                     "shape": "StringList"
                 }
             },
             "type": "structure"
         },
         "LoadBalancer": {
-            "documentation": "<p>The load balancer configuration to use with a service or task set.</p> <p>For specific notes and restrictions regarding the use of load balancers with services and task sets, see the CreateService and CreateTaskSet actions.</p> <p>When you add, update, or remove a load balancer configuration, Amazon ECS starts a new deployment with the updated Elastic Load Balancing configuration. This causes tasks to register to and deregister from load balancers.</p> <p>We recommend that you verify this on a test environment before you update the Elastic Load Balancing configuration. </p> <p>A service-linked role is required for services that use multiple target groups. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/using-service-linked-roles.html\">Using service-linked roles</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+            "documentation": "<p>The load balancer configuration to use with a service or task set.</p> <p>When you add, update, or remove a load balancer configuration, Amazon ECS starts a new deployment with the updated Elastic Load Balancing configuration. This causes tasks to register to and deregister from load balancers.</p> <p>We recommend that you verify this on a test environment before you update the Elastic Load Balancing configuration. </p> <p>A service-linked role is required for services that use multiple target groups. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/using-service-linked-roles.html\">Using service-linked roles</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "members": {
                 "containerName": {
                     "documentation": "<p>The name of the container (as it appears in a container definition) to associate with the load balancer.</p>",
                     "shape": "String"
                 },
                 "containerPort": {
                     "documentation": "<p>The port on the container to associate with the load balancer. This port must correspond to a <code>containerPort</code> in the task definition the tasks in the service are using. For tasks that use the EC2 launch type, the container instance they're launched on must allow ingress traffic on the <code>hostPort</code> of the port mapping.</p>",
@@ -4773,15 +4783,15 @@
                     "shape": "Timestamp"
                 },
                 "lastStatus": {
                     "documentation": "<p>The last known status of the managed agent.</p>",
                     "shape": "String"
                 },
                 "name": {
-                    "documentation": "<p>The name of the managed agent. When the execute command feature is enabled, the managed agent name is <code>ExecuteCommandAgent</code>.</p>",
+                    "documentation": "<p>The name of the managed agent. When the execute command feature is turned on, the managed agent name is <code>ExecuteCommandAgent</code>.</p>",
                     "shape": "ManagedAgentName"
                 },
                 "reason": {
                     "documentation": "<p>The reason for why the managed agent is in the state it is in.</p>",
                     "shape": "String"
                 }
             },
@@ -4829,15 +4839,15 @@
         "ManagedAgents": {
             "member": {
                 "shape": "ManagedAgent"
             },
             "type": "list"
         },
         "ManagedScaling": {
-            "documentation": "<p>The managed scaling settings for the Auto Scaling group capacity provider.</p> <p>When managed scaling is enabled, Amazon ECS manages the scale-in and scale-out actions of the Auto Scaling group. Amazon ECS manages a target tracking scaling policy using an Amazon ECS managed CloudWatch metric with the specified <code>targetCapacity</code> value as the target value for the metric. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/asg-capacity-providers.html#asg-capacity-providers-managed-scaling\">Using managed scaling</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>If managed scaling is off, the user must manage the scaling of the Auto Scaling group.</p>",
+            "documentation": "<p>The managed scaling settings for the Auto Scaling group capacity provider.</p> <p>When managed scaling is turned on, Amazon ECS manages the scale-in and scale-out actions of the Auto Scaling group. Amazon ECS manages a target tracking scaling policy using an Amazon ECS managed CloudWatch metric with the specified <code>targetCapacity</code> value as the target value for the metric. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/asg-capacity-providers.html#asg-capacity-providers-managed-scaling\">Using managed scaling</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <p>If managed scaling is off, the user must manage the scaling of the Auto Scaling group.</p>",
             "members": {
                 "instanceWarmupPeriod": {
                     "documentation": "<p>The period of time, in seconds, after a newly launched Amazon EC2 instance can contribute to CloudWatch metrics for Auto Scaling group. If this parameter is omitted, the default value of <code>300</code> seconds is used.</p>",
                     "shape": "ManagedScalingInstanceWarmupPeriod"
                 },
                 "maximumScalingStepSize": {
                     "documentation": "<p>The maximum number of Amazon EC2 instances that Amazon ECS will scale out at one time. The scale in process is not affected by this parameter. If this parameter is omitted, the default value of <code>1</code> is used.</p>",
@@ -4848,15 +4858,15 @@
                     "shape": "ManagedScalingStepSize"
                 },
                 "status": {
                     "documentation": "<p>Determines whether to use managed scaling for the capacity provider.</p>",
                     "shape": "ManagedScalingStatus"
                 },
                 "targetCapacity": {
-                    "documentation": "<p>The target capacity value for the capacity provider. The specified value must be greater than <code>0</code> and less than or equal to <code>100</code>. A value of <code>100</code> results in the Amazon EC2 instances in your Auto Scaling group being completely used.</p>",
+                    "documentation": "<p>The target capacity utilization as a percentage for the capacity provider. The specified value must be greater than <code>0</code> and less than or equal to <code>100</code>. For example, if you want the capacity provider to maintain 10% spare capacity, then that means the utilization is 90%, so use a <code>targetCapacity</code> of <code>90</code>. The default value of <code>100</code> percent results in the Amazon EC2 instances in your Auto Scaling group being completely used.</p>",
                     "shape": "ManagedScalingTargetCapacity"
                 }
             },
             "type": "structure"
         },
         "ManagedScalingInstanceWarmupPeriod": {
             "max": 10000,
@@ -4890,15 +4900,15 @@
         "MissingVersionException": {
             "documentation": "<p>Amazon ECS can't determine the current version of the Amazon ECS container agent on the container instance and doesn't have enough information to proceed with an update. This could be because the agent running on the container instance is a previous or custom version that doesn't use our version information.</p>",
             "exception": true,
             "members": {},
             "type": "structure"
         },
         "MountPoint": {
-            "documentation": "<p>Details for a volume mount point that's used in a container definition.</p>",
+            "documentation": "<p>The details for a volume mount point that's used in a container definition.</p>",
             "members": {
                 "containerPath": {
                     "documentation": "<p>The path on the container to mount the host volume at.</p>",
                     "shape": "String"
                 },
                 "readOnly": {
                     "documentation": "<p>If this value is <code>true</code>, the container has read-only access to the volume. If this value is <code>false</code>, then the container can write to the volume. The default value is <code>false</code>.</p>",
@@ -5122,30 +5132,30 @@
         "PlatformUnknownException": {
             "documentation": "<p>The specified platform version doesn't exist.</p>",
             "exception": true,
             "members": {},
             "type": "structure"
         },
         "PortMapping": {
-            "documentation": "<p>Port mappings allow containers to access ports on the host container instance to send or receive traffic. Port mappings are specified as part of the container definition.</p> <p>If you use containers in a task with the <code>awsvpc</code> or <code>host</code> network mode, specify the exposed ports using <code>containerPort</code>. The <code>hostPort</code> can be left blank or it must be the same value as the <code>containerPort</code>.</p> <note> <p>You can't expose the same container port for multiple protocols. If you attempt this, an error is returned.</p> </note> <p>After a task reaches the <code>RUNNING</code> status, manual and automatic host and container port assignments are visible in the <code>networkBindings</code> section of <a>DescribeTasks</a> API responses.</p>",
+            "documentation": "<p>Port mappings allow containers to access ports on the host container instance to send or receive traffic. Port mappings are specified as part of the container definition.</p> <p>If you use containers in a task with the <code>awsvpc</code> or <code>host</code> network mode, specify the exposed ports using <code>containerPort</code>. The <code>hostPort</code> can be left blank or it must be the same value as the <code>containerPort</code>.</p> <p>Most fields of this parameter (<code>containerPort</code>, <code>hostPort</code>, <code>protocol</code>) maps to <code>PortBindings</code> in the <a href=\"https://docs.docker.com/engine/api/v1.35/#operation/ContainerCreate\">Create a container</a> section of the <a href=\"https://docs.docker.com/engine/api/v1.35/\">Docker Remote API</a> and the <code>--publish</code> option to <a href=\"https://docs.docker.com/engine/reference/commandline/run/\"> <code>docker run</code> </a>. If the network mode of a task definition is set to <code>host</code>, host ports must either be undefined or match the container port in the port mapping.</p> <note> <p>You can't expose the same container port for multiple protocols. If you attempt this, an error is returned.</p> </note> <p>After a task reaches the <code>RUNNING</code> status, manual and automatic host and container port assignments are visible in the <code>networkBindings</code> section of <a>DescribeTasks</a> API responses.</p>",
             "members": {
                 "appProtocol": {
                     "documentation": "<p>The application protocol that's used for the port mapping. This parameter only applies to Service Connect. We recommend that you set this parameter to be consistent with the protocol that your application uses. If you set this parameter, Amazon ECS adds protocol-specific connection handling to the Service Connect proxy. If you set this parameter, Amazon ECS adds protocol-specific telemetry in the Amazon ECS console and CloudWatch.</p> <p>If you don't set a value for this parameter, then TCP is used. However, Amazon ECS doesn't add protocol-specific telemetry for TCP.</p> <p>Tasks that run in a namespace can use short names to connect to services in the namespace. Tasks can connect to services across all of the clusters in the namespace. Tasks connect through a managed proxy container that collects logs and metrics for increased visibility. Only the tasks that Amazon ECS services create are supported with Service Connect. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-connect.html\">Service Connect</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "ApplicationProtocol"
                 },
                 "containerPort": {
                     "documentation": "<p>The port number on the container that's bound to the user-specified or automatically assigned host port.</p> <p>If you use containers in a task with the <code>awsvpc</code> or <code>host</code> network mode, specify the exposed ports using <code>containerPort</code>.</p> <p>If you use containers in a task with the <code>bridge</code> network mode and you specify a container port and not a host port, your container automatically receives a host port in the ephemeral port range. For more information, see <code>hostPort</code>. Port mappings that are automatically assigned in this way do not count toward the 100 reserved ports limit of a container instance.</p>",
                     "shape": "BoxedInteger"
                 },
                 "containerPortRange": {
                     "documentation": "<p>The port number range on the container that's bound to the dynamically mapped host port range. </p> <p>The following rules apply when you specify a <code>containerPortRange</code>:</p> <ul> <li> <p>You must use either the <code>bridge</code> network mode or the <code>awsvpc</code> network mode.</p> </li> <li> <p>This parameter is available for both the EC2 and Fargate launch types.</p> </li> <li> <p>This parameter is available for both the Linux and Windows operating systems.</p> </li> <li> <p>The container instance must have at least version 1.67.0 of the container agent and at least version 1.67.0-1 of the <code>ecs-init</code> package </p> </li> <li> <p>You can specify a maximum of 100 port ranges per container.</p> </li> <li> <p>You do not specify a <code>hostPortRange</code>. The value of the <code>hostPortRange</code> is set as follows:</p> <ul> <li> <p>For containers in a task with the <code>awsvpc</code> network mode, the <code>hostPort</code> is set to the same value as the <code>containerPort</code>. This is a static mapping strategy.</p> </li> <li> <p>For containers in a task with the <code>bridge</code> network mode, the Amazon ECS agent finds open host ports from the default ephemeral range and passes it to docker to bind them to the container ports.</p> </li> </ul> </li> <li> <p>The <code>containerPortRange</code> valid values are between 1 and 65535.</p> </li> <li> <p>A port can only be included in one port mapping per container.</p> </li> <li> <p>You cannot specify overlapping port ranges.</p> </li> <li> <p>The first port in the range must be less than last port in the range.</p> </li> <li> <p>Docker recommends that you turn off the docker-proxy in the Docker daemon config file when you have a large number of ports.</p> <p>For more information, see <a href=\"https://github.com/moby/moby/issues/11185\"> Issue #11185</a> on the Github website.</p> <p>For information about how to turn off the docker-proxy in the Docker daemon config file, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/bootstrap_container_instance.html#bootstrap_docker_daemon\">Docker daemon</a> in the <i>Amazon ECS Developer Guide</i>.</p> </li> </ul> <p>You can call <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_DescribeTasks.html\"> <code>DescribeTasks</code> </a> to view the <code>hostPortRange</code> which are the host ports that are bound to the container ports.</p>",
                     "shape": "String"
                 },
                 "hostPort": {
-                    "documentation": "<p>The port number on the container instance to reserve for your container.</p> <p>If you specify a <code>containerPortRange</code>, leave this field empty and the value of the <code>hostPort</code> is set as follows:</p> <ul> <li> <p>For containers in a task with the <code>awsvpc</code> network mode, the <code>hostPort</code> is set to the same value as the <code>containerPort</code>. This is a static mapping strategy.</p> </li> <li> <p>For containers in a task with the <code>bridge</code> network mode, the Amazon ECS agent finds open ports on the host and automaticaly binds them to the container ports. This is a dynamic mapping strategy.</p> </li> </ul> <p>If you use containers in a task with the <code>awsvpc</code> or <code>host</code> network mode, the <code>hostPort</code> can either be left blank or set to the same value as the <code>containerPort</code>.</p> <p>If you use containers in a task with the <code>bridge</code> network mode, you can specify a non-reserved host port for your container port mapping, or you can omit the <code>hostPort</code> (or set it to <code>0</code>) while specifying a <code>containerPort</code> and your container automatically receives a port in the ephemeral port range for your container instance operating system and Docker version.</p> <p>The default ephemeral port range for Docker version 1.6.0 and later is listed on the instance under <code>/proc/sys/net/ipv4/ip_local_port_range</code>. If this kernel parameter is unavailable, the default ephemeral port range from 49153 through 65535 is used. Do not attempt to specify a host port in the ephemeral port range as these are reserved for automatic assignment. In general, ports below 32768 are outside of the ephemeral port range.</p> <p>The default reserved ports are 22 for SSH, the Docker ports 2375 and 2376, and the Amazon ECS container agent ports 51678-51680. Any host port that was previously specified in a running task is also reserved while the task is running. That is, after a task stops, the host port is released. The current reserved ports are displayed in the <code>remainingResources</code> of <a>DescribeContainerInstances</a> output. A container instance can have up to 100 reserved ports at a time. This number includes the default reserved ports. Automatically assigned ports aren't included in the 100 reserved ports quota.</p>",
+                    "documentation": "<p>The port number on the container instance to reserve for your container.</p> <p>If you specify a <code>containerPortRange</code>, leave this field empty and the value of the <code>hostPort</code> is set as follows:</p> <ul> <li> <p>For containers in a task with the <code>awsvpc</code> network mode, the <code>hostPort</code> is set to the same value as the <code>containerPort</code>. This is a static mapping strategy.</p> </li> <li> <p>For containers in a task with the <code>bridge</code> network mode, the Amazon ECS agent finds open ports on the host and automatically binds them to the container ports. This is a dynamic mapping strategy.</p> </li> </ul> <p>If you use containers in a task with the <code>awsvpc</code> or <code>host</code> network mode, the <code>hostPort</code> can either be left blank or set to the same value as the <code>containerPort</code>.</p> <p>If you use containers in a task with the <code>bridge</code> network mode, you can specify a non-reserved host port for your container port mapping, or you can omit the <code>hostPort</code> (or set it to <code>0</code>) while specifying a <code>containerPort</code> and your container automatically receives a port in the ephemeral port range for your container instance operating system and Docker version.</p> <p>The default ephemeral port range for Docker version 1.6.0 and later is listed on the instance under <code>/proc/sys/net/ipv4/ip_local_port_range</code>. If this kernel parameter is unavailable, the default ephemeral port range from 49153 through 65535 is used. Do not attempt to specify a host port in the ephemeral port range as these are reserved for automatic assignment. In general, ports below 32768 are outside of the ephemeral port range.</p> <p>The default reserved ports are 22 for SSH, the Docker ports 2375 and 2376, and the Amazon ECS container agent ports 51678-51680. Any host port that was previously specified in a running task is also reserved while the task is running. That is, after a task stops, the host port is released. The current reserved ports are displayed in the <code>remainingResources</code> of <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_DescribeContainerInstances.html\">DescribeContainerInstances</a> output. A container instance can have up to 100 reserved ports at a time. This number includes the default reserved ports. Automatically assigned ports aren't included in the 100 reserved ports quota.</p>",
                     "shape": "BoxedInteger"
                 },
                 "name": {
                     "documentation": "<p>The name that's used for the port mapping. This parameter only applies to Service Connect. This parameter is the name that you use in the <code>serviceConnectConfiguration</code> of a service. The name can include up to 64 characters. The characters can include lowercase letters, numbers, underscores (_), and hyphens (-). The name can't start with a hyphen.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-connect.html\">Service Connect</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "String"
                 },
                 "protocol": {
@@ -5231,19 +5241,19 @@
                 "APPMESH"
             ],
             "type": "string"
         },
         "PutAccountSettingDefaultRequest": {
             "members": {
                 "name": {
-                    "documentation": "<p>The resource name for which to modify the account setting. If <code>serviceLongArnFormat</code> is specified, the ARN for your Amazon ECS services is affected. If <code>taskLongArnFormat</code> is specified, the ARN and resource ID for your Amazon ECS tasks is affected. If <code>containerInstanceLongArnFormat</code> is specified, the ARN and resource ID for your Amazon ECS container instances is affected. If <code>awsvpcTrunking</code> is specified, the ENI limit for your Amazon ECS container instances is affected. If <code>containerInsights</code> is specified, the default setting for CloudWatch Container Insights for your clusters is affected.</p> <p>Fargate is transitioning from task count-based quotas to vCPU-based quotas. You can set the name to <code>fargateVCPULimit</code> to opt in or opt out of the vCPU-based quotas. For information about the opt in timeline, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-account-settings.html#fargate-quota-timeline\">Fargate vCPU-based quotas timeline</a> in the <i>Amazon ECS Developer Guide</i>.</p>",
+                    "documentation": "<p>The resource name for which to modify the account setting. If <code>serviceLongArnFormat</code> is specified, the ARN for your Amazon ECS services is affected. If <code>taskLongArnFormat</code> is specified, the ARN and resource ID for your Amazon ECS tasks is affected. If <code>containerInstanceLongArnFormat</code> is specified, the ARN and resource ID for your Amazon ECS container instances is affected. If <code>awsvpcTrunking</code> is specified, the ENI limit for your Amazon ECS container instances is affected. If <code>containerInsights</code> is specified, the default setting for Amazon Web Services CloudWatch Container Insights for your clusters is affected. If <code>tagResourceAuthorization</code> is specified, the opt-in option for tagging resources on creation is affected. For information about the opt-in timeline, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-account-settings.html#tag-resources\">Tagging authorization timeline</a> in the <i>Amazon ECS Developer Guide</i>.</p> <p>When you specify <code>fargateFIPSMode</code> for the <code>name</code> and <code>enabled</code> for the <code>value</code>, Fargate uses FIPS-140 compliant cryptographic algorithms on your tasks. For more information about FIPS-140 compliance with Fargate, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-fips-compliance.html\"> Amazon Web Services Fargate Federal Information Processing Standard (FIPS) 140-2 compliance</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "SettingName"
                 },
                 "value": {
-                    "documentation": "<p>The account setting value for the specified principal ARN. Accepted values are <code>enabled</code> and <code>disabled</code>.</p>",
+                    "documentation": "<p>The account setting value for the specified principal ARN. Accepted values are <code>enabled</code>, <code>disabled</code>, <code>on</code>, and <code>off</code>.</p>",
                     "shape": "String"
                 }
             },
             "required": [
                 "name",
                 "value"
             ],
@@ -5257,23 +5267,23 @@
                 }
             },
             "type": "structure"
         },
         "PutAccountSettingRequest": {
             "members": {
                 "name": {
-                    "documentation": "<p>The Amazon ECS resource name for which to modify the account setting. If <code>serviceLongArnFormat</code> is specified, the ARN for your Amazon ECS services is affected. If <code>taskLongArnFormat</code> is specified, the ARN and resource ID for your Amazon ECS tasks is affected. If <code>containerInstanceLongArnFormat</code> is specified, the ARN and resource ID for your Amazon ECS container instances is affected. If <code>awsvpcTrunking</code> is specified, the elastic network interface (ENI) limit for your Amazon ECS container instances is affected. If <code>containerInsights</code> is specified, the default setting for CloudWatch Container Insights for your clusters is affected.</p>",
+                    "documentation": "<p>The Amazon ECS resource name for which to modify the account setting. If <code>serviceLongArnFormat</code> is specified, the ARN for your Amazon ECS services is affected. If <code>taskLongArnFormat</code> is specified, the ARN and resource ID for your Amazon ECS tasks is affected. If <code>containerInstanceLongArnFormat</code> is specified, the ARN and resource ID for your Amazon ECS container instances is affected. If <code>awsvpcTrunking</code> is specified, the elastic network interface (ENI) limit for your Amazon ECS container instances is affected. If <code>containerInsights</code> is specified, the default setting for Amazon Web Services CloudWatch Container Insights for your clusters is affected. If <code>fargateFIPSMode</code> is specified, Fargate FIPS 140 compliance is affected. If <code>tagResourceAuthorization</code> is specified, the opt-in option for tagging resources on creation is affected. For information about the opt-in timeline, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-account-settings.html#tag-resources\">Tagging authorization timeline</a> in the <i>Amazon ECS Developer Guide</i>.</p>",
                     "shape": "SettingName"
                 },
                 "principalArn": {
                     "documentation": "<p>The ARN of the principal, which can be a user, role, or the root user. If you specify the root user, it modifies the account setting for all users, roles, and the root user of the account unless a user or role explicitly overrides these settings. If this field is omitted, the setting is changed only for the authenticated user.</p> <note> <p>Federated users assume the account setting of the root user and can't have explicit account settings set for them.</p> </note>",
                     "shape": "String"
                 },
                 "value": {
-                    "documentation": "<p>The account setting value for the specified principal ARN. Accepted values are <code>enabled</code> and <code>disabled</code>.</p>",
+                    "documentation": "<p>The account setting value for the specified principal ARN. Accepted values are <code>enabled</code>, <code>disabled</code>, <code>on</code>, and <code>off</code>.</p>",
                     "shape": "String"
                 }
             },
             "required": [
                 "name",
                 "value"
             ],
@@ -5401,15 +5411,15 @@
                     "shape": "ContainerDefinitions"
                 },
                 "cpu": {
                     "documentation": "<p>The number of CPU units used by the task. It can be expressed as an integer using CPU units (for example, <code>1024</code>) or as a string using vCPUs (for example, <code>1 vCPU</code> or <code>1 vcpu</code>) in a task definition. String values are converted to an integer indicating the CPU units when the task definition is registered.</p> <note> <p>Task-level CPU and memory parameters are ignored for Windows containers. We recommend specifying container-level resources for Windows containers.</p> </note> <p>If you're using the EC2 launch type, this field is optional. Supported values are between <code>128</code> CPU units (<code>0.125</code> vCPUs) and <code>10240</code> CPU units (<code>10</code> vCPUs). If you do not specify a value, the parameter is ignored.</p> <p>If you're using the Fargate launch type, this field is required and you must use one of the following values, which determines your range of supported values for the <code>memory</code> parameter:</p> <p>The CPU units cannot be less than 1 vCPU when you use Windows containers on Fargate.</p> <ul> <li> <p>256 (.25 vCPU) - Available <code>memory</code> values: 512 (0.5 GB), 1024 (1 GB), 2048 (2 GB)</p> </li> <li> <p>512 (.5 vCPU) - Available <code>memory</code> values: 1024 (1 GB), 2048 (2 GB), 3072 (3 GB), 4096 (4 GB)</p> </li> <li> <p>1024 (1 vCPU) - Available <code>memory</code> values: 2048 (2 GB), 3072 (3 GB), 4096 (4 GB), 5120 (5 GB), 6144 (6 GB), 7168 (7 GB), 8192 (8 GB)</p> </li> <li> <p>2048 (2 vCPU) - Available <code>memory</code> values: 4096 (4 GB) and 16384 (16 GB) in increments of 1024 (1 GB)</p> </li> <li> <p>4096 (4 vCPU) - Available <code>memory</code> values: 8192 (8 GB) and 30720 (30 GB) in increments of 1024 (1 GB)</p> </li> <li> <p>8192 (8 vCPU) - Available <code>memory</code> values: 16 GB and 60 GB in 4 GB increments</p> <p>This option requires Linux platform <code>1.4.0</code> or later.</p> </li> <li> <p>16384 (16vCPU) - Available <code>memory</code> values: 32GB and 120 GB in 8 GB increments</p> <p>This option requires Linux platform <code>1.4.0</code> or later.</p> </li> </ul>",
                     "shape": "String"
                 },
                 "ephemeralStorage": {
-                    "documentation": "<p>The amount of ephemeral storage to allocate for the task. This parameter is used to expand the total amount of ephemeral storage available, beyond the default amount, for tasks hosted on Fargate. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/userguide/using_data_volumes.html\">Fargate task storage</a> in the <i>Amazon ECS User Guide for Fargate</i>.</p> <note> <p>This parameter is only supported for tasks hosted on Fargate using the following platform versions:</p> <ul> <li> <p>Linux platform version <code>1.4.0</code> or later.</p> </li> </ul> </note>",
+                    "documentation": "<p>The amount of ephemeral storage to allocate for the task. This parameter is used to expand the total amount of ephemeral storage available, beyond the default amount, for tasks hosted on Fargate. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/userguide/using_data_volumes.html\">Fargate task storage</a> in the <i>Amazon ECS User Guide for Fargate</i>.</p> <note> <p>For tasks using the Fargate launch type, the task requires the following platforms:</p> <ul> <li> <p>Linux platform version <code>1.4.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul> </note>",
                     "shape": "EphemeralStorage"
                 },
                 "executionRoleArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the task execution role that grants the Amazon ECS container agent permission to make Amazon Web Services API calls on your behalf. The task execution IAM role is required depending on the requirements of your task. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_execution_IAM_role.html\">Amazon ECS task execution IAM role</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "String"
                 },
                 "family": {
@@ -5549,15 +5559,15 @@
             "documentation": "<p>The type and amount of a resource to assign to a container. The supported resource types are GPUs and Elastic Inference accelerators. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-gpu.html\">Working with GPUs on Amazon ECS</a> or <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-inference.html\">Working with Amazon Elastic Inference on Amazon ECS</a> in the <i>Amazon Elastic Container Service Developer Guide</i> </p>",
             "members": {
                 "type": {
                     "documentation": "<p>The type of resource to assign to a container. The supported values are <code>GPU</code> or <code>InferenceAccelerator</code>.</p>",
                     "shape": "ResourceType"
                 },
                 "value": {
-                    "documentation": "<p>The value for the specified resource type.</p> <p>If the <code>GPU</code> type is used, the value is the number of physical <code>GPUs</code> the Amazon ECS container agent reserves for the container. The number of GPUs that's reserved for all containers in a task can't exceed the number of available GPUs on the container instance that the task is launched on.</p> <p>If the <code>InferenceAccelerator</code> type is used, the <code>value</code> matches the <code>deviceName</code> for an <a>InferenceAccelerator</a> specified in a task definition.</p>",
+                    "documentation": "<p>The value for the specified resource type.</p> <p>If the <code>GPU</code> type is used, the value is the number of physical <code>GPUs</code> the Amazon ECS container agent reserves for the container. The number of GPUs that's reserved for all containers in a task can't exceed the number of available GPUs on the container instance that the task is launched on.</p> <p>If the <code>InferenceAccelerator</code> type is used, the <code>value</code> matches the <code>deviceName</code> for an <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_InferenceAccelerator.html\">InferenceAccelerator</a> specified in a task definition.</p>",
                     "shape": "String"
                 }
             },
             "required": [
                 "value",
                 "type"
             ],
@@ -5755,15 +5765,15 @@
                 "message": {
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "Service": {
-            "documentation": "<p>Details on a service within a cluster</p>",
+            "documentation": "<p>Details on a service within a cluster.</p>",
             "members": {
                 "capacityProviderStrategy": {
                     "documentation": "<p>The capacity provider strategy the service uses. When using the DescribeServices API, this field is omitted if the service was created using a launch type.</p>",
                     "shape": "CapacityProviderStrategy"
                 },
                 "clusterArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the cluster that hosts the service.</p>",
@@ -5794,15 +5804,15 @@
                     "shape": "Integer"
                 },
                 "enableECSManagedTags": {
                     "documentation": "<p>Determines whether to use Amazon ECS managed tags for the tasks in the service. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-using-tags.html\">Tagging Your Amazon ECS Resources</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "Boolean"
                 },
                 "enableExecuteCommand": {
-                    "documentation": "<p>Determines whether the execute command functionality is enabled for the service. If <code>true</code>, the execute command functionality is enabled for all containers in tasks as part of the service.</p>",
+                    "documentation": "<p>Determines whether the execute command functionality is turned on for the service. If <code>true</code>, the execute command functionality is turned on for all containers in tasks as part of the service.</p>",
                     "shape": "Boolean"
                 },
                 "events": {
                     "documentation": "<p>The event stream for your service. A maximum of 100 of the latest events are displayed.</p>",
                     "shape": "ServiceEvents"
                 },
                 "healthCheckGracePeriodSeconds": {
@@ -5918,15 +5928,15 @@
                     "documentation": "<p>Specifies whether to use Service Connect with this service.</p>",
                     "shape": "Boolean"
                 },
                 "logConfiguration": {
                     "shape": "LogConfiguration"
                 },
                 "namespace": {
-                    "documentation": "<p>The namespace name or full Amazon Resource Name (ARN) of the Cloud Map namespace for use with Service Connect. The namespace must be in the same Amazon Web Services Region as the Amazon ECS service and cluster. The type of namespace doesn't affect Service Connect. For more information about Cloud Map, see <a href=\"https://docs.aws.amazon.com/\">Working with Services</a> in the <i>Cloud Map Developer Guide</i>.</p>",
+                    "documentation": "<p>The namespace name or full Amazon Resource Name (ARN) of the Cloud Map namespace for use with Service Connect. The namespace must be in the same Amazon Web Services Region as the Amazon ECS service and cluster. The type of namespace doesn't affect Service Connect. For more information about Cloud Map, see <a href=\"https://docs.aws.amazon.com/cloud-map/latest/dg/working-with-services.html\">Working with Services</a> in the <i>Cloud Map Developer Guide</i>.</p>",
                     "shape": "String"
                 },
                 "services": {
                     "documentation": "<p>The list of Service Connect service objects. These are names and aliases (also known as endpoints) that are used by other Amazon ECS services to connect to this service. </p> <p>This field is not required for a \"client\" Amazon ECS service that's a member of a namespace only to connect to other services within the namespace. An example of this would be a frontend application that accepts incoming requests from either a load balancer that's attached to the service or by other means.</p> <p>An object selects a port from the task definition, assigns a name for the Cloud Map service, and a list of aliases (endpoints) and ports for client applications to refer to this service.</p>",
                     "shape": "ServiceConnectServiceList"
                 }
             },
@@ -5939,15 +5949,15 @@
             "documentation": "<p>The Service Connect service object configuration. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/service-connect.html\">Service Connect</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "members": {
                 "clientAliases": {
                     "documentation": "<p>The list of client aliases for this Service Connect service. You use these to assign names that can be used by client applications. The maximum number of client aliases that you can have in this list is 1.</p> <p>Each alias (\"endpoint\") is a fully-qualified name and port number that other Amazon ECS tasks (\"clients\") can use to connect to this service.</p> <p>Each name and port mapping must be unique within the namespace.</p> <p>For each <code>ServiceConnectService</code>, you must provide at least one <code>clientAlias</code> with one <code>port</code>.</p>",
                     "shape": "ServiceConnectClientAliasList"
                 },
                 "discoveryName": {
-                    "documentation": "<p>The <code>discoveryName</code> is the name of the new Cloud Map service that Amazon ECS creates for this Amazon ECS service. This must be unique within the Cloud Map namespace. The name can contain up to 64 characters. The name can include lowercase letters, numbers, underscores (_), and hyphens (-). The name can't start with a hyphen.</p> <p>If this parameter isn't specified, the default value of <code>discoveryName.namespace</code> is used. If the <code>discoveryName</code> isn't specified, the port mapping name from the task definition is used in <code>portName.namespace</code>.</p>",
+                    "documentation": "<p>The <code>discoveryName</code> is the name of the new Cloud Map service that Amazon ECS creates for this Amazon ECS service. This must be unique within the Cloud Map namespace. The name can contain up to 64 characters. The name can include lowercase letters, numbers, underscores (_), and hyphens (-). The name can't start with a hyphen.</p> <p>If the <code>discoveryName</code> isn't specified, the port mapping name from the task definition is used in <code>portName.namespace</code>.</p>",
                     "shape": "String"
                 },
                 "ingressPortOverride": {
                     "documentation": "<p>The port number for the Service Connect proxy to listen on.</p> <p>Use the value of this field to bypass the proxy for traffic on the port number specified in the named <code>portMapping</code> in the task definition of this application, and then use it in your VPC security groups to allow traffic into the proxy for this Amazon ECS service.</p> <p>In <code>awsvpc</code> mode and Fargate, the default value is the container port number. The container port number is in the <code>portMapping</code> in the task definition. In bridge mode, the default value is the ephemeral port of the Service Connect proxy.</p>",
                     "shape": "PortNumber"
                 },
                 "portName": {
@@ -5970,15 +5980,15 @@
             "documentation": "<p>The Service Connect resource. Each configuration maps a discovery name to a Cloud Map service name. The data is stored in Cloud Map as part of the Service Connect configuration for each discovery name of this Amazon ECS service.</p> <p>A task can resolve the <code>dnsName</code> for each of the <code>clientAliases</code> of a service. However a task can't resolve the discovery names. If you want to connect to a service, refer to the <code>ServiceConnectConfiguration</code> of that service for the list of <code>clientAliases</code> that you can use.</p>",
             "members": {
                 "discoveryArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) for the namespace in Cloud Map that matches the discovery name for this Service Connect resource. You can use this ARN in other integrations with Cloud Map. However, Service Connect can't ensure connectivity outside of Amazon ECS.</p>",
                     "shape": "String"
                 },
                 "discoveryName": {
-                    "documentation": "<p>The discovery name of this Service Connect resource.</p> <p>The <code>discoveryName</code> is the name of the new Cloud Map service that Amazon ECS creates for this Amazon ECS service. This must be unique within the Cloud Map namespace. The name can contain up to 64 characters. The name can include lowercase letters, numbers, underscores (_), and hyphens (-). The name can't start with a hyphen.</p> <p>If this parameter isn't specified, the default value of <code>discoveryName.namespace</code> is used. If the <code>discoveryName</code> isn't specified, the port mapping name from the task definition is used in <code>portName.namespace</code>.</p>",
+                    "documentation": "<p>The discovery name of this Service Connect resource.</p> <p>The <code>discoveryName</code> is the name of the new Cloud Map service that Amazon ECS creates for this Amazon ECS service. This must be unique within the Cloud Map namespace. The name can contain up to 64 characters. The name can include lowercase letters, numbers, underscores (_), and hyphens (-). The name can't start with a hyphen.</p> <p>If the <code>discoveryName</code> isn't specified, the port mapping name from the task definition is used in <code>portName.namespace</code>.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "ServiceConnectServiceResourceList": {
             "member": {
@@ -6106,15 +6116,17 @@
         },
         "SettingName": {
             "enum": [
                 "serviceLongArnFormat",
                 "taskLongArnFormat",
                 "containerInstanceLongArnFormat",
                 "awsvpcTrunking",
-                "containerInsights"
+                "containerInsights",
+                "fargateFIPSMode",
+                "tagResourceAuthorization"
             ],
             "type": "string"
         },
         "Settings": {
             "member": {
                 "shape": "Setting"
             },
@@ -6145,15 +6157,15 @@
                     "shape": "StringList"
                 },
                 "enableECSManagedTags": {
                     "documentation": "<p>Specifies whether to use Amazon ECS managed tags for the task. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-using-tags.html\">Tagging Your Amazon ECS Resources</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "Boolean"
                 },
                 "enableExecuteCommand": {
-                    "documentation": "<p>Whether or not the execute command functionality is enabled for the task. If <code>true</code>, this enables execute command functionality on all containers in the task.</p>",
+                    "documentation": "<p>Whether or not the execute command functionality is turned on for the task. If <code>true</code>, this turns on the execute command functionality on all containers in the task.</p>",
                     "shape": "Boolean"
                 },
                 "group": {
                     "documentation": "<p>The name of the task group to associate with the task. The default value is the family name of the task definition (for example, family:my-family-name).</p>",
                     "shape": "String"
                 },
                 "networkConfiguration": {
@@ -6460,15 +6472,15 @@
             "member": {
                 "shape": "Tag"
             },
             "min": 0,
             "type": "list"
         },
         "TargetNotConnectedException": {
-            "documentation": "<p>The execute command cannot run. This error can be caused by any of the following configuration issues:</p> <ul> <li> <p>Incorrect IAM permissions</p> </li> <li> <p>The SSM agent is not installed or is not running</p> </li> <li> <p> There is an interface Amazon VPC endpoint for Amazon ECS, but there is not one for for Systems Manager Session Manager</p> </li> </ul> <p>For information about how to troubleshoot the issues, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-exec.html\">Troubleshooting issues with ECS Exec</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
+            "documentation": "<p>The execute command cannot run. This error can be caused by any of the following configuration issues:</p> <ul> <li> <p>Incorrect IAM permissions</p> </li> <li> <p>The SSM agent is not installed or is not running</p> </li> <li> <p> There is an interface Amazon VPC endpoint for Amazon ECS, but there is not one for Systems Manager Session Manager</p> </li> </ul> <p>For information about how to troubleshoot the issues, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-exec.html\">Troubleshooting issues with ECS Exec</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
             "exception": true,
             "members": {},
             "type": "structure"
         },
         "TargetNotFoundException": {
             "documentation": "<p>The specified target wasn't found. You can view your available container instances with <a>ListContainerInstances</a>. Amazon ECS container instances are cluster-specific and Region-specific.</p>",
             "exception": true,
@@ -6529,15 +6541,15 @@
                     "shape": "Timestamp"
                 },
                 "desiredStatus": {
                     "documentation": "<p>The desired status of the task. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-lifecycle.html\">Task Lifecycle</a>.</p>",
                     "shape": "String"
                 },
                 "enableExecuteCommand": {
-                    "documentation": "<p>Determines whether execute command functionality is enabled for this task. If <code>true</code>, execute command functionality is enabled on all the containers in the task.</p>",
+                    "documentation": "<p>Determines whether execute command functionality is turned on for this task. If <code>true</code>, execute command functionality is turned on all the containers in the task.</p>",
                     "shape": "Boolean"
                 },
                 "ephemeralStorage": {
                     "documentation": "<p>The ephemeral storage settings for the task.</p>",
                     "shape": "EphemeralStorage"
                 },
                 "executionStoppedAt": {
@@ -6699,15 +6711,15 @@
                     "shape": "String"
                 },
                 "requiresAttributes": {
                     "documentation": "<p>The container instance attributes required by your task. When an Amazon EC2 instance is registered to your cluster, the Amazon ECS container agent assigns some standard attributes to the instance. You can apply custom attributes. These are specified as key-value pairs using the Amazon ECS console or the <a>PutAttributes</a> API. These attributes are used when determining task placement for tasks hosted on Amazon EC2 instances. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-placement-constraints.html#attributes\">Attributes</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <note> <p>This parameter isn't supported for tasks run on Fargate.</p> </note>",
                     "shape": "RequiresAttributes"
                 },
                 "requiresCompatibilities": {
-                    "documentation": "<p>The task launch types the task definition was validated against. To determine which task launch types the task definition is validated for, see the <a>TaskDefinition$compatibilities</a> parameter.</p>",
+                    "documentation": "<p>The task launch types the task definition was validated against. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/launch_types.html\">Amazon ECS launch types</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "CompatibilityList"
                 },
                 "revision": {
                     "documentation": "<p>The revision of the task in a particular family. The revision is a version number of a task definition in a family. When you register a task definition for the first time, the revision is <code>1</code>. Each time that you register a new revision of a task definition in the same family, the revision value always increases by one. This is even if you deregistered previous revisions in this family.</p>",
                     "shape": "Integer"
                 },
                 "runtimePlatform": {
@@ -6756,15 +6768,15 @@
         "TaskDefinitionList": {
             "member": {
                 "shape": "TaskDefinition"
             },
             "type": "list"
         },
         "TaskDefinitionPlacementConstraint": {
-            "documentation": "<p>An object representing a constraint on task placement in the task definition. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-placement-constraints.html\">Task placement constraints</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <note> <p>Task placement constraints aren't supported for tasks run on Fargate.</p> </note>",
+            "documentation": "<p>The constraint on task placement in the task definition. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-placement-constraints.html\">Task placement constraints</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p> <note> <p>Task placement constraints aren't supported for tasks run on Fargate.</p> </note>",
             "members": {
                 "expression": {
                     "documentation": "<p>A cluster query language expression to apply to the constraint. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/cluster-query-language.html\">Cluster query language</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>",
                     "shape": "String"
                 },
                 "type": {
                     "documentation": "<p>The type of constraint. The <code>MemberOf</code> constraint restricts selection to be from a group of valid candidates.</p>",
@@ -7395,15 +7407,15 @@
         "UpdateTaskProtectionResponse": {
             "members": {
                 "failures": {
                     "documentation": "<p>Any failures associated with the call.</p>",
                     "shape": "Failures"
                 },
                 "protectedTasks": {
-                    "documentation": "<p>A list of tasks with the following information.</p> <ul> <li> <p> <code>taskArn</code>: The task ARN.</p> </li> <li> <p> <code>protectionEnabled</code>: The protection status of the task. If scale-in protection is enabled for a task, the value is <code>true</code>. Otherwise, it is <code>false</code>.</p> </li> <li> <p> <code>expirationDate</code>: The epoch time when protection for the task will expire.</p> </li> </ul>",
+                    "documentation": "<p>A list of tasks with the following information.</p> <ul> <li> <p> <code>taskArn</code>: The task ARN.</p> </li> <li> <p> <code>protectionEnabled</code>: The protection status of the task. If scale-in protection is turned on for a task, the value is <code>true</code>. Otherwise, it is <code>false</code>.</p> </li> <li> <p> <code>expirationDate</code>: The epoch time when protection for the task will expire.</p> </li> </ul>",
                     "shape": "ProtectedTasks"
                 }
             },
             "type": "structure"
         },
         "UpdateTaskSetRequest": {
             "members": {
```

### Comparing `botocore-a-la-carte-ecs-1.29.99/botocore/data/ecs/2014-11-13/waiters-2.json` & `botocore-a-la-carte-ecs-1.30.0/botocore/data/ecs/2014-11-13/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ecs-1.29.99/botocore_a_la_carte_ecs.egg-info/PKG-INFO` & `botocore-a-la-carte-ecs-1.30.0/botocore_a_la_carte_ecs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ecs
-Version: 1.29.99
+Version: 1.30.0
 Summary: ecs data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ecs-1.29.99/setup.py` & `botocore-a-la-carte-ecs-1.30.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ecs',
-    version="1.29.99",
+    version="1.30.0",
     description='ecs data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ecs/*/*.json'],
```

