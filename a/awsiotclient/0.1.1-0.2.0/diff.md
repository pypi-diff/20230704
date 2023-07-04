# Comparing `tmp/awsiotclient-0.1.1.tar.gz` & `tmp/awsiotclient-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsiotclient-0.1.1.tar", max compression
+gzip compressed data, was "awsiotclient-0.2.0.tar", max compression
```

## Comparing `awsiotclient-0.1.1.tar` & `awsiotclient-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11342 2021-10-02 11:33:18.518084 awsiotclient-0.1.1/LICENSE
--rw-r--r--   0        0        0     2925 2021-10-02 11:33:18.518084 awsiotclient-0.1.1/README.md
--rw-r--r--   0        0        0      874 2021-10-02 11:53:35.078046 awsiotclient-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      439 2021-10-02 11:33:18.514084 awsiotclient-0.1.1/src/awsiotclient/__init__.py
--rw-r--r--   0        0        0    11094 2021-10-02 11:33:18.518084 awsiotclient-0.1.1/src/awsiotclient/classic_shadow.py
--rw-r--r--   0        0        0     1141 2021-10-02 11:33:18.514084 awsiotclient-0.1.1/src/awsiotclient/dictdiff.py
--rw-r--r--   0        0        0    10200 2021-10-02 11:33:18.518084 awsiotclient-0.1.1/src/awsiotclient/jobs.py
--rw-r--r--   0        0        0     4394 2021-10-02 11:33:18.514084 awsiotclient-0.1.1/src/awsiotclient/mqtt.py
--rw-r--r--   0        0        0    13000 2021-10-02 11:33:18.514084 awsiotclient-0.1.1/src/awsiotclient/named_shadow.py
--rw-r--r--   0        0        0     1630 2021-10-02 11:33:18.514084 awsiotclient-0.1.1/src/awsiotclient/pubsub.py
--rw-r--r--   0        0        0     3888 2021-10-02 11:53:50.812535 awsiotclient-0.1.1/setup.py
--rw-r--r--   0        0        0     3778 2021-10-02 11:53:50.812896 awsiotclient-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-05-30 05:39:59.830296 awsiotclient-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2927 2023-06-22 07:58:35.419314 awsiotclient-0.2.0/README.md
+-rw-r--r--   0        0        0      821 2023-07-04 10:16:41.362896 awsiotclient-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      439 2023-06-22 07:03:35.379170 awsiotclient-0.2.0/src/awsiotclient/__init__.py
+-rw-r--r--   0        0        0     4601 2023-07-04 10:16:41.362896 awsiotclient-0.2.0/src/awsiotclient/classic_shadow.py
+-rw-r--r--   0        0        0     1038 2023-06-22 07:57:13.420265 awsiotclient-0.2.0/src/awsiotclient/dictdiff.py
+-rw-r--r--   0        0        0    10351 2023-07-04 07:44:50.499287 awsiotclient-0.2.0/src/awsiotclient/jobs.py
+-rw-r--r--   0        0        0     4513 2023-06-22 08:04:01.999686 awsiotclient-0.2.0/src/awsiotclient/mqtt.py
+-rw-r--r--   0        0        0     4913 2023-07-04 10:16:41.362896 awsiotclient-0.2.0/src/awsiotclient/named_shadow.py
+-rw-r--r--   0        0        0     1865 2023-06-22 07:56:42.268632 awsiotclient-0.2.0/src/awsiotclient/pubsub.py
+-rw-r--r--   0        0        0     9444 2023-07-04 10:16:41.362896 awsiotclient-0.2.0/src/awsiotclient/shadow.py
+-rw-r--r--   0        0        0     3786 1970-01-01 00:00:00.000000 awsiotclient-0.2.0/PKG-INFO
```

### Comparing `awsiotclient-0.1.1/LICENSE` & `awsiotclient-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awsiotclient-0.1.1/README.md` & `awsiotclient-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 The AWS IoT Device Client provides device-side functionality for AWS IoT services such as jobs, device shadow, and simple pubsub.
 
 ## Installation
 
 ### Minimum Requirements
 
-- Python 3.6+
+- Python 3.7.1+
 
 ### Install from PyPI
 
 ```shell
 python3 -m pip install awsiotclient
 ```
```

### Comparing `awsiotclient-0.1.1/src/awsiotclient/dictdiff.py` & `awsiotclient-0.2.0/src/awsiotclient/dictdiff.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#!/usr/bin/env python3
+from copy import deepcopy
 from typing import Any, Dict, Optional
 
 from . import get_module_logger
 
 logger = get_module_logger(__name__)
 
 
-def dictdiff(s1: Optional[Dict[Any, Any]], s2: Optional[Dict[Any, Any]]) -> Optional[Dict[Any, Any]]:
+def dictdiff(
+    s1: Optional[Dict[Any, Any]], s2: Optional[Dict[Any, Any]]
+) -> Optional[Dict[Any, Any]]:
     if not s2 or s1 == s2:
         return None
     if not s1:
-        return s2  # s1 is empty.
+        return deepcopy(s2)  # s1 is empty.
 
     dst = dict()
     for k in s1.keys() | s2.keys():
         v1 = s1.get(k)
         v2 = s2.get(k)
         if v1 == v2:
             continue  # Not changed
+
         if v1 is None:
             logger.debug(f"Added Item ({k})  : None -> {v2}")
-            dst[k] = v2  # Added Item
+            dst[k] = deepcopy(v2)
             continue
+
         if v2 is None:
             logger.debug(f"Removed Item ({k}): {v1} -> None")
             dst[k] = None  # Removed Item
             continue
-        if type(v1) != type(v2):
-            dst[k] = v2  # Type changed. Override.
-            continue
 
-        # here, v1 != v2 and type(v1) == type(v2)
-        if isinstance(v1, dict):
+        if isinstance(v1, dict) and isinstance(v2, dict):
             dst[k] = dictdiff(v1, v2)
         else:
             logger.debug(f"Updated Item ({k}): {v1} -> {v2}")
-            dst[k] = v2  # Updated item
+            dst[k] = deepcopy(v2)  # Updated item
 
     return dst
```

### Comparing `awsiotclient-0.1.1/src/awsiotclient/jobs.py` & `awsiotclient-0.2.0/src/awsiotclient/jobs.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,70 +44,84 @@
         self.client = iotjobs.IotJobsClient(connection)
         self.thing_name = thing_name
         self.qos = qos
         self.locked_data = LockedData()
         self.job_func = job_func
 
         try:
-            changed_subscription_request = iotjobs.NextJobExecutionChangedSubscriptionRequest(thing_name=thing_name)
-            (subscribed_future, _,) = self.client.subscribe_to_next_job_execution_changed_events(
-                request=changed_subscription_request,
+            self.client.subscribe_to_next_job_execution_changed_events(
+                request=iotjobs.NextJobExecutionChangedSubscriptionRequest(
+                    thing_name=thing_name
+                ),
                 qos=qos,
                 callback=self.on_next_job_execution_changed,
-            )
+            )[0].result()
 
-            # Wait for subscription to succeed
-            subscribed_future.result()
+            self.__subscribe_start_next_pending_job()
+            self.__subscribe_update_job()
 
-            logger.debug("Subscribing to Start responses...")
-            start_subscription_request = iotjobs.StartNextPendingJobExecutionSubscriptionRequest(thing_name=thing_name)
-            (subscribed_accepted_future, _,) = self.client.subscribe_to_start_next_pending_job_execution_accepted(
-                request=start_subscription_request,
-                qos=qos,
-                callback=self.on_start_next_pending_job_execution_accepted,
-            )
+            # Make initial attempt to start next job. The service should reply with
+            # an "accepted" response, even if no jobs are pending. The response
+            # will contain data about the next job, if there is one.
+            self.try_start_next_job()
 
-            (subscribed_rejected_future, _,) = self.client.subscribe_to_start_next_pending_job_execution_rejected(
-                request=start_subscription_request,
-                qos=qos,
-                callback=self.on_start_next_pending_job_execution_rejected,
-            )
+        except Exception as e:
+            raise ExceptionAwsIotJobs(e)
 
-            # Wait for subscriptions to succeed
-            subscribed_accepted_future.result()
-            subscribed_rejected_future.result()
-
-            logger.debug("Subscribing to Update responses...")
-            # Note that we subscribe to "+", the MQTT wildcard, to receive
-            # responses about any job-ID.
-            update_subscription_request = iotjobs.UpdateJobExecutionSubscriptionRequest(thing_name=thing_name, job_id="+")
+    def __subscribe_start_next_pending_job(self) -> None:
+        logger.debug("Subscribing to Start responses...")
+        request = iotjobs.StartNextPendingJobExecutionSubscriptionRequest(
+            thing_name=self.thing_name
+        )
 
-            (subscribed_accepted_future, _,) = self.client.subscribe_to_update_job_execution_accepted(
-                request=update_subscription_request,
-                qos=qos,
-                callback=self.on_update_job_execution_accepted,
-            )
+        (
+            accepted_future,
+            _,
+        ) = self.client.subscribe_to_start_next_pending_job_execution_accepted(
+            request=request,
+            qos=self.qos,
+            callback=self.on_start_next_pending_job_execution_accepted,
+        )
 
-            (subscribed_rejected_future, _,) = self.client.subscribe_to_update_job_execution_rejected(
-                request=update_subscription_request,
-                qos=qos,
-                callback=self.on_update_job_execution_rejected,
-            )
+        (
+            rejected_future,
+            _,
+        ) = self.client.subscribe_to_start_next_pending_job_execution_rejected(
+            request=request,
+            qos=self.qos,
+            callback=self.on_start_next_pending_job_execution_rejected,
+        )
 
-            # Wait for subscriptions to succeed
-            subscribed_accepted_future.result()
-            subscribed_rejected_future.result()
+        # Wait for subscriptions to succeed
+        accepted_future.result()
+        rejected_future.result()
+
+    def __subscribe_update_job(self) -> None:
+        logger.debug("Subscribing to Update responses...")
+        # Note that we subscribe to "+", the MQTT wildcard, to receive
+        # responses about any job-ID.
+        request = iotjobs.UpdateJobExecutionSubscriptionRequest(
+            thing_name=self.thing_name, job_id="+"
+        )
 
-            # Make initial attempt to start next job. The service should reply with
-            # an "accepted" response, even if no jobs are pending. The response
-            # will contain data about the next job, if there is one.
-            self.try_start_next_job()
+        accepted_future, _ = self.client.subscribe_to_update_job_execution_accepted(
+            request=request,
+            qos=self.qos,
+            callback=self.on_update_job_execution_accepted,
+        )
 
-        except Exception as e:
-            raise (e)
+        rejected_future, _ = self.client.subscribe_to_update_job_execution_rejected(
+            request=request,
+            qos=self.qos,
+            callback=self.on_update_job_execution_rejected,
+        )
+
+        # Wait for subscriptions to succeed
+        accepted_future.result()
+        rejected_future.result()
 
     def try_start_next_job(self) -> None:
         logger.debug("Trying to start the next job...")
         with self.locked_data.lock:
             if self.locked_data.is_working_on_job:
                 logger.debug("Nevermind, already working on a job.")
                 return
@@ -116,99 +130,116 @@
                 logger.debug("Nevermind, sample is disconnecting.")
                 return
 
             self.locked_data.is_working_on_job = True
             self.locked_data.is_next_job_waiting = False
 
         logger.debug("Publishing request to start next job...")
-        request = iotjobs.StartNextPendingJobExecutionRequest(thing_name=self.thing_name)
-        publish_future = self.client.publish_start_next_pending_job_execution(request, self.qos)
-        publish_future.add_done_callback(self.on_publish_start_next_pending_job_execution)
+        request = iotjobs.StartNextPendingJobExecutionRequest(
+            thing_name=self.thing_name
+        )
+        publish_future = self.client.publish_start_next_pending_job_execution(
+            request, self.qos
+        )
+        publish_future.add_done_callback(
+            self.on_publish_start_next_pending_job_execution
+        )
 
     def done_working_on_job(self) -> None:
         with self.locked_data.lock:
             self.locked_data.is_working_on_job = False
             try_again = self.locked_data.is_next_job_waiting
 
         if try_again:
             self.try_start_next_job()
 
-    def on_next_job_execution_changed(self, event: iotjobs.NextJobExecutionChangedEvent) -> None:
+    def on_next_job_execution_changed(
+        self, event: iotjobs.NextJobExecutionChangedEvent
+    ) -> None:
         try:
             execution = event.execution
             if execution:
                 logger.debug(
                     "Received Next Job Execution Changed event. ",
-                    "job_id:{} job_document:{}".format(execution.job_id, execution.job_document),
+                    f"job_id:{execution.job_id} job_document:{execution.job_document}",
                 )
 
                 # Start job now, or remember to start it when current job is done
                 start_job_now = False
                 with self.locked_data.lock:
                     if self.locked_data.is_working_on_job:
                         self.locked_data.is_next_job_waiting = True
                     else:
                         start_job_now = True
 
                 if start_job_now:
                     self.try_start_next_job()
 
             else:
-                logger.debug("Received Next Job Execution Changed event: ", "None. Waiting for further jobs...")
+                logger.debug(
+                    "Received Next Job Execution Changed event: ",
+                    "None. Waiting for further jobs...",
+                )
 
         except Exception as e:
-            raise (e)
+            raise ExceptionAwsIotJobs(e)
 
     def on_publish_start_next_pending_job_execution(self, future: Future) -> None:  # type: ignore
         try:
             future.result()  # raises exception if publish failed
 
             logger.debug("Published request to start the next job.")
 
         except Exception as e:
-            raise (e)
+            raise ExceptionAwsIotJobs(e)
 
-    def on_start_next_pending_job_execution_accepted(self, response):
-        # type: (iotjobs.StartNextJobExecutionResponse) -> None
+    def on_start_next_pending_job_execution_accepted(
+        self, response: iotjobs.StartNextJobExecutionResponse
+    ):
         try:
             if response.execution:
                 execution = response.execution
                 logger.debug(
-                    "Request to start next job was accepted. job_id:{} job_document:{}".format(
-                        execution.job_id, execution.job_document
-                    )
+                    f"Request to start next job was accepted. job_id:{execution.job_id} job_document:{execution.job_document}"
                 )
 
                 # To emulate working on a job, spawn a thread that sleeps for a few seconds
                 job_thread = threading.Thread(
-                    target=lambda: self.job_thread_fn(execution.job_id, execution.job_document),
+                    target=lambda: self.job_thread_fn(
+                        execution.job_id, execution.job_document
+                    ),
                     name="job_thread",
                 )
                 job_thread.start()
             else:
                 logger.debug(
-                    "Request to start next job was accepted, but there are no jobs to be done.", " Waiting for further jobs..."
+                    "Request to start next job was accepted, but there are no jobs to be done.",
+                    " Waiting for further jobs...",
                 )
                 self.done_working_on_job()
 
         except Exception as e:
-            raise (e)
+            raise ExceptionAwsIotJobs(e)
 
-    def on_start_next_pending_job_execution_rejected(self, rejected: iotjobs.RejectedError) -> None:
+    def on_start_next_pending_job_execution_rejected(
+        self, rejected: iotjobs.RejectedError
+    ) -> None:
         raise ExceptionAwsIotJobs(
-            "Request to start next pending job rejected with code:'{}' message:'{}'".format(rejected.code, rejected.message)
+            f"Request to start next pending job rejected with code:'{rejected.code}' message:'{rejected.message}'"
         )
 
     def job_thread_fn(self, job_id: str, job_document: JobDocument) -> None:
         try:
             logger.debug("Starting local work on job...")
             self.job_func(job_id, job_document)
             logger.debug("Done working on job.")
         except ExceptionAwsIotJobsUserDefinedFailure as e:
-            logger.debug("Report that job excecution failed due to user-defined reason...")
+            logger.debug(
+                "Report that job excecution failed due to user-defined reason..."
+            )
             request = iotjobs.UpdateJobExecutionRequest(
                 thing_name=self.thing_name,
                 job_id=job_id,
                 status_details=dict(failure_type="user_defined", failure_detail=str(e)),
                 status=iotjobs.JobStatus.FAILED,
             )
         except Exception as e:
@@ -232,20 +263,22 @@
 
     def on_publish_update_job_execution(self, future: Future) -> None:  # type: ignore
         try:
             future.result()  # raises exception if publish failed
             logger.debug("Published request to update job.")
 
         except Exception as e:
-            raise (e)
+            raise ExceptionAwsIotJobs(e)
 
-    def on_update_job_execution_accepted(self, response: iotjobs.UpdateJobExecutionResponse) -> None:
+    def on_update_job_execution_accepted(
+        self, response: iotjobs.UpdateJobExecutionResponse
+    ) -> None:
         try:
             logger.debug("Request to update job was accepted.")
             self.done_working_on_job()
         except Exception as e:
-            raise (e)
+            raise ExceptionAwsIotJobs(e)
 
     def on_update_job_execution_rejected(self, rejected: iotjobs.RejectedError) -> None:
         raise ExceptionAwsIotJobs(
-            "Request to update job status was rejected. code:'{}' message:'{}'.".format(rejected.code, rejected.message)
+            f"Request to update job status was rejected. code:'{rejected.code}' message:'{rejected.message}'."
         )
```

### Comparing `awsiotclient-0.1.1/src/awsiotclient/mqtt.py` & `awsiotclient-0.2.0/src/awsiotclient/mqtt.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,29 @@
 
 
 class ExceptionAwsIotMqtt(ExceptionAwsIotClient):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
-def on_connection_interrupted(connection: mqtt.Connection, error: exceptions.AwsCrtError, **kwargs: KwArgs) -> None:
+def on_connection_interrupted(
+    connection: mqtt.Connection, error: exceptions.AwsCrtError, **kwargs: KwArgs
+) -> None:
     logger.debug(f"Connection interrupted. error: {error}")
 
 
 def on_connection_resumed(
-    connection: mqtt.Connection, return_code: mqtt.ConnectReturnCode, session_present: bool, **kwargs: KwArgs
+    connection: mqtt.Connection,
+    return_code: mqtt.ConnectReturnCode,
+    session_present: bool,
+    **kwargs: KwArgs,
 ) -> None:
-    logger.debug(f"Connection resumed. return_code: {return_code} session_present: {session_present}")
+    logger.debug(
+        f"Connection resumed. return_code: {return_code} session_present: {session_present}"
+    )
 
     if return_code == mqtt.ConnectReturnCode.ACCEPTED and not session_present:
         logger.debug("Session did not persist. Resubscribing to existing topics...")
         resubscribe_future, _ = connection.resubscribe_existing_topics()
 
         # Cannot synchronously wait for resubscribe result
         # because we're on the connection's event-loop thread,
@@ -38,15 +45,17 @@
 
 def on_resubscribe_complete(resubscribe_future: Future) -> None:  # type: ignore
     resubscribe_results = resubscribe_future.result()
     logger.debug(f"Resubscribe results: {resubscribe_results}")
 
     for topic, qos in resubscribe_results["topics"]:
         if qos is None:
-            raise (ExceptionAwsIotMqtt(f"Server rejected resubscribe to topic: {topic}"))
+            raise (
+                ExceptionAwsIotMqtt(f"Server rejected resubscribe to topic: {topic}")
+            )
 
 
 class ConnectionParams:
     def __init__(
         self,
         endpoint: str = "",
         signing_region: str = "ap-northeast-1",
@@ -74,17 +83,21 @@
     event_loop_group = io.EventLoopGroup(1)
     host_resolver = io.DefaultHostResolver(event_loop_group)
     client_bootstrap = io.ClientBootstrap(event_loop_group, host_resolver)
 
     if params.use_websocket:
         proxy_options = None
         if params.proxy_host:
-            proxy_options = http.HttpProxyOptions(host_name=params.proxy_host, port=params.proxy_port)
+            proxy_options = http.HttpProxyOptions(
+                host_name=params.proxy_host, port=params.proxy_port
+            )
 
-        credentials_provider = auth.AwsCredentialsProvider.new_default_chain(client_bootstrap=client_bootstrap)
+        credentials_provider = auth.AwsCredentialsProvider.new_default_chain(
+            client_bootstrap=client_bootstrap
+        )
         mqtt_connection = mqtt_connection_builder.websockets_with_default_aws_signing(
             endpoint=params.endpoint,
             client_bootstrap=client_bootstrap,
             region=params.signing_region,
             credentials_provider=credentials_provider,
             websocket_proxy_options=proxy_options,
             ca_filepath=params.root_ca,
@@ -105,10 +118,12 @@
             on_connection_interrupted=on_connection_interrupted,
             on_connection_resumed=on_connection_resumed,
             client_id=params.client_id,
             clean_session=False,
             keep_alive_secs=6,
         )
 
-    logger.debug("Connecting to {} with client ID '{}'...".format(params.endpoint, params.client_id))
+    logger.debug(
+        f"Connecting to {params.endpoint} with client ID '{params.client_id}'..."
+    )
 
     return mqtt_connection
```

### Comparing `awsiotclient-0.1.1/src/awsiotclient/named_shadow.py` & `awsiotclient-0.2.0/src/awsiotclient/shadow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,298 +1,267 @@
-import threading
+from abc import ABC, abstractmethod
 from concurrent.futures import Future
+from dataclasses import dataclass
+from threading import Lock
 from traceback import format_exc
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 from awscrt import mqtt
 from awsiot import iotshadow
 
 from . import ExceptionAwsIotClient, dictdiff, get_module_logger
 
 logger = get_module_logger(__name__)
 ShadowDocument = Optional[Dict[str, Any]]
+SHADOW_VALUE_DEFAULT = None
 
 
-class ExceptionAwsIotNamedShadow(ExceptionAwsIotClient):
+class ExceptionAwsIotShadow(ExceptionAwsIotClient):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
-class ExceptionAwsIotNamedShadowInvalidDelta(ExceptionAwsIotNamedShadow):
+class ExceptionAwsIotShadowInvalidDelta(ExceptionAwsIotShadow):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
-def empty_func(thing_name: str, shadow_name: str, value: Dict[str, Any]) -> None:
-    logger.debug(f"empty func. thing_name: {thing_name}, shadow_name: {shadow_name}, value: {value}")
+def done_future() -> "Future[None]":
+    future: "Future[None]" = Future()
+    future.set_result(None)
+    return future
 
 
-SHADOW_VALUE_DEFAULT = None
+@dataclass
+class DocumentTracker:
+    _current: ShadowDocument = None
+
+    def get(self) -> ShadowDocument:
+        return self._current
+
+    def set(self, value: ShadowDocument) -> None:
+        self._current = value
+
+    def update(self, new: ShadowDocument, diff_only: bool) -> ShadowDocument:
+        if self._current == new:
+            logger.debug(f"Shadow value is already '{new}'.")
+            return None
+
+        if diff_only:
+            value = dictdiff.dictdiff(self._current, new)
+        else:
+            value = new
+
+        logger.debug(f"Shadow value changes to '{new}'.")
+        self.set(new)
+        return value
+
 
+@dataclass
+class ShadowData:
+    _lock: Lock = Lock()
+    _desired_value: DocumentTracker = DocumentTracker()
+    _reported_value: DocumentTracker = DocumentTracker()
 
-class LockedData:
-    def __init__(self) -> None:
-        self.lock: threading.Lock = threading.Lock()
-        self.reported_value: ShadowDocument = None
-        self.desired_value: ShadowDocument = None
-        self.disconnect_called: bool = False
+    def get_desired_value(self) -> ShadowDocument:
+        with self._lock:
+            return self._desired_value.get()
+
+    def set_desired_value(self, value: ShadowDocument) -> None:
+        with self._lock:
+            self._desired_value.set(value)
+
+    def update_desired_value(
+        self, value: ShadowDocument, publish_full_doc: bool
+    ) -> ShadowDocument:
+        with self._lock:
+            return self._desired_value.update(value, not publish_full_doc)
 
+    def get_reported_value(self) -> ShadowDocument:
+        with self._lock:
+            return self._reported_value.get()
+
+    def set_reported_value(self, value: ShadowDocument) -> None:
+        with self._lock:
+            self._reported_value.set(value)
+
+    def update_reported_value(
+        self, value: ShadowDocument, publish_full_doc: bool
+    ) -> ShadowDocument:
+        with self._lock:
+            return self._reported_value.update(value, not publish_full_doc)
+
+    def update_both_values(
+        self,
+        desired_value: ShadowDocument,
+        reported_value: ShadowDocument,
+        publish_full_doc: bool,
+    ) -> Tuple[ShadowDocument, ShadowDocument]:
+        with self._lock:
+            desired = self._desired_value.update(desired_value, not publish_full_doc)
+            reported = self._reported_value.update(reported_value, not publish_full_doc)
+            return desired, reported
+
+
+class ShadowClientCommon(ABC):
+    client: iotshadow.IotShadowClient
+    thing_name: str
+    property_name: Optional[str]
+    locked_data = ShadowData()
+    qos: mqtt.QoS
+    publish_full_doc: bool
 
-class client:
     def __init__(
         self,
         connection: mqtt.Connection,
         thing_name: str,
-        shadow_name: str,
-        qos: mqtt.QoS = mqtt.QoS.AT_LEAST_ONCE,
-        delta_func: Callable[[str, str, Dict[str, Any]], None] = empty_func,
-        publish_full_doc: bool = False,
+        property_name: Optional[str],
+        qos: mqtt.QoS,
+        delta_func: Callable[[str, str, ShadowDocument], None],
+        desired_func: Callable[[str, str, ShadowDocument], None],
+        publish_full_doc: bool,
     ) -> None:
         self.client = iotshadow.IotShadowClient(connection)
         self.thing_name = thing_name
-        self.shadow_name = shadow_name
-        self.locked_data = LockedData()
-        self.delta_func = delta_func
+        self.property_name = property_name
         self.qos = qos
+        self.delta_func = delta_func
+        self.desired_func = desired_func
         self.publish_full_doc = publish_full_doc
-        try:
-            # Subscribe to necessary topics.
-            # Note that **is** important to wait for "accepted/rejected" subscriptions
-            # to succeed before publishing the corresponding "request".
-            logger.debug("Subscribing to Delta events...")
-            (delta_subscribed_future, _,) = self.client.subscribe_to_named_shadow_delta_updated_events(
-                request=iotshadow.NamedShadowDeltaUpdatedSubscriptionRequest(thing_name=thing_name, shadow_name=shadow_name),
-                qos=qos,
-                callback=self.on_named_shadow_delta_updated,
-            )
-
-            # Wait for subscription to succeed
-            delta_subscribed_future.result()
 
-            logger.debug("Subscribing to Update responses...")
-            (update_accepted_subscribed_future, _,) = self.client.subscribe_to_update_named_shadow_accepted(
-                request=iotshadow.UpdateNamedShadowSubscriptionRequest(thing_name=thing_name, shadow_name=shadow_name),
-                qos=qos,
-                callback=self.on_update_named_shadow_accepted,
-            )
-
-            (update_rejected_subscribed_future, _,) = self.client.subscribe_to_update_named_shadow_rejected(
-                request=iotshadow.UpdateNamedShadowSubscriptionRequest(thing_name=thing_name, shadow_name=shadow_name),
-                qos=qos,
-                callback=self.on_update_named_shadow_rejected,
-            )
-
-            # Wait for subscriptions to succeed
-            update_accepted_subscribed_future.result()
-            update_rejected_subscribed_future.result()
-
-            logger.debug("Subscribing to Get responses...")
-            (get_accepted_subscribed_future, _,) = self.client.subscribe_to_get_named_shadow_accepted(
-                request=iotshadow.GetNamedShadowSubscriptionRequest(thing_name=thing_name, shadow_name=shadow_name),
-                qos=qos,
-                callback=self.on_get_named_shadow_accepted,
-            )
-
-            (get_rejected_subscribed_future, _,) = self.client.subscribe_to_get_named_shadow_rejected(
-                request=iotshadow.GetNamedShadowSubscriptionRequest(thing_name=thing_name, shadow_name=shadow_name),
-                qos=qos,
-                callback=self.on_get_named_shadow_rejected,
-            )
-
-            # Wait for subscriptions to succeed
-            get_accepted_subscribed_future.result()
-            get_rejected_subscribed_future.result()
-
-            # The rest of the sample runs asyncronously.
-
-            # Issue request for shadow's current state.
-            # The response will be received by the on_get_accepted() callback
-            logger.debug("Requesting current shadow state...")
-            publish_get_future = self.client.publish_get_named_shadow(
-                request=iotshadow.GetNamedShadowRequest(thing_name=thing_name, shadow_name=shadow_name),
-                qos=qos,
-            )
+    def __filter_property(self, v: ShadowDocument) -> ShadowDocument:
+        if self.property_name is None:
+            return v
+        return v.get(self.property_name)
+
+    def label(self) -> str:
+        return self.property_name
+
+    def on_shadow_delta_updated(self, delta: iotshadow.ShadowDeltaUpdatedEvent) -> None:
+        logger.debug("Received shadow delta event.")
+        if not delta.state:
+            logger.debug(f"  Delta did not report a change in '{self.label()}'")
+            return
 
-            # Ensure that publish succeeds
-            publish_get_future.result()
+        value = self.__filter_property(delta.state)
 
+        try:
+            if value is None:
+                logger.debug(
+                    f"  Delta reports that '{self.label()}' was deleted. Resetting defaults..."
+                )
+                self.change_reported_value(SHADOW_VALUE_DEFAULT)
+                return
+            else:
+                logger.debug(
+                    f"  Delta reports that desired value is '{value}'. Invoke delta func..."
+                )
+                try:
+                    self.delta_func(self.thing_name, self.label(), value)
+                except ExceptionAwsIotShadowInvalidDelta:
+                    logger.debug(
+                        f"  Delta reports invalid request in {self.label()}. Resetting defaults..."
+                    )
+                    self.change_desired_value(SHADOW_VALUE_DEFAULT)
         except Exception as e:
             logger.error(format_exc())
             raise (e)
 
-    def on_get_named_shadow_accepted(self, response):
-        # type: (iotshadow.GetNamedShadowResponse) -> None
-        try:
-            logger.debug("Finished getting initial shadow state.")
-            with self.locked_data.lock:
-                if self.locked_data.reported_value is not None:
-                    logger.debug("  Ignoring initial query because a delta event has already been received.")
-                    return
+    def on_get_shadow_accepted(self, response: iotshadow.GetShadowResponse) -> None:
+        logger.debug("Finished getting initial shadow state.")
+        if self.locked_data.get_reported_value() is not None:
+            logger.debug(
+                "  Ignoring initial query because a delta event has already been received."
+            )
+            return
 
+        try:
             if response.state:
                 if response.state.delta:
-                    value = response.state.delta
+                    value = self.__filter_property(response.state.delta)
                     if value:
-                        logger.debug("  Named Shadow contains delta value '{}'.".format(value))
+                        logger.debug(f"  Shadow contains delta value '{value}'.")
                         return
 
                 if response.state.reported:
-                    value = response.state.reported
+                    value = self.__filter_property(response.state.reported)
                     if value:
-                        logger.debug("  Named Shadow contains reported value '{}'.".format(value))
-                        self.set_local_value_due_to_initial_query(response.state.reported)
+                        logger.debug(f"  Shadow contains reported value '{value}'.")
+                        self.locked_data.set_reported_value(value)
                         return
 
-            logger.debug("  Named Shadow document lacks '{}' state. Setting defaults...".format(self.shadow_name))
+            logger.debug(
+                f"  Shadow document lacks '{self.label()}' property. Setting defaults..."
+            )
             self.change_reported_value(SHADOW_VALUE_DEFAULT)
-            return
 
         except Exception as e:
             logger.error(format_exc())
             raise (e)
 
-    def on_get_named_shadow_rejected(self, error):
-        # type: (iotshadow.ErrorResponse) -> None
+    def on_get_shadow_rejected(self, error: iotshadow.ErrorResponse) -> None:
         if error.code == 404:
             logger.debug("Thing has no shadow document. Creating with defaults...")
             self.change_reported_value(SHADOW_VALUE_DEFAULT)
         else:
-            raise ExceptionAwsIotNamedShadow("Get request was rejected. code:{} message:'{}'".format(error.code, error.message))
+            raise ExceptionAwsIotClient(error)
 
-    def on_named_shadow_delta_updated(self, delta):
-        # type: (iotshadow.NamedShadowDeltaUpdatedEvent) -> None
+    def on_update_shadow_accepted(
+        self, response: iotshadow.UpdateShadowResponse
+    ) -> None:
         try:
-            logger.debug("Received shadow delta event.")
-            if delta.state:
-                value = delta.state
-                if value is None:
-                    logger.debug("  Delta reports that '{}' was deleted. Resetting defaults...".format(self.shadow_name))
-                    self.change_reported_value(SHADOW_VALUE_DEFAULT)
-                    return
-                else:
-                    logger.debug("  Delta reports that desired value is '{}'. Invoke delta func...".format(value))
-                    try:
-                        self.delta_func(self.thing_name, self.shadow_name, value)
-                    except ExceptionAwsIotNamedShadowInvalidDelta:
-                        logger.debug(f"  Delta reports invalid request in {self.shadow_name}. Resetting defaults...")
-                        for key in value:
-                            value[key] = None
-                        self.change_desired_value(value)
-
-            else:
-                logger.debug("  Delta did not report a change in '{}'".format(self.shadow_name))
-
+            if response.state.reported:
+                logger.debug(
+                    f"Finished updating reported shadow value to '{response.state.reported}'."
+                )
+            if response.state.desired:
+                logger.debug(
+                    f"Finished updating desired shadow value to '{response.state.desired}'."
+                )
+                self.locked_data.set_desired_value(response.state.desired)
+                self.desired_func(self.thing_name, self.label(), response.state.desired)
         except Exception as e:
             logger.error(format_exc())
+            logger.error("Updated shadow is missing the target property.")
             raise (e)
 
-    def on_publish_update_named_shadow(self, future: Future) -> None:  # type: ignore
+    def on_update_shadow_rejected(self, error: iotshadow.ErrorResponse) -> None:
+        logger.error(
+            f"Update request was rejected. code:{error.code} message:'{error.message}'"
+        )
+        raise ExceptionAwsIotClient(error)
+
+    def on_publish_update_shadow(self, future: Future) -> None:
         try:
             future.result()
             logger.debug("Update request published.")
         except Exception as e:
             logger.error(format_exc())
-            logger.error("Failed to publish update request.")
+            logger.debug("Failed to publish update request.")
             raise (e)
 
-    def on_update_named_shadow_accepted(self, response):
-        # type: (iotshadow.UpdateNamedShadowResponse) -> None
-        try:
-            if response.state.reported:
-                logger.debug("Finished updating reported shadow value to '{}'.".format(response.state.reported))
-            if response.state.desired:
-                logger.debug("Finished updating desired shadow value to '{}'.".format(response.state.desired))
-        except Exception as e:
-            logger.error(format_exc())
-            logger.error("Updated shadow is missing the target property.")
-            raise (e)
-
-    def on_update_named_shadow_rejected(self, error):
-        # type: (iotshadow.ErrorResponse) -> None
-        errstr = "Update request was rejected. code:{} message:'{}'".format(error.code, error.message)
-        logger.error(errstr)
-        raise ExceptionAwsIotNamedShadow(errstr)
-
-    def set_local_value_due_to_initial_query(self, reported_value: ShadowDocument) -> None:
-        with self.locked_data.lock:
-            self.locked_data.reported_value = reported_value
-
-    def change_reported_value(self, value: ShadowDocument) -> None:
-        with self.locked_data.lock:
-            if self.locked_data.reported_value == value:
-                logger.debug("Local value is already '{}'.".format(value))
-                return
-
-            if self.publish_full_doc:
-                reported = value
-            else:
-                reported = dictdiff.dictdiff(self.locked_data.reported_value, value)
-            logger.debug("Changed local shadow value to '{}'.".format(value))
-            self.locked_data.reported_value = value
-
-        logger.debug("Updating reported shadow value to '{}'...".format(reported))
-        request = iotshadow.UpdateNamedShadowRequest(
-            thing_name=self.thing_name,
-            shadow_name=self.shadow_name,
-            state=iotshadow.ShadowState(
-                reported=reported,
-            ),
+    @abstractmethod
+    def update_shadow_request(
+        self, desired: ShadowDocument, reported: ShadowDocument
+    ) -> "Future[None]":
+        pass
+
+    def change_reported_value(self, value: ShadowDocument) -> "Future[None]":
+        reported = self.locked_data.update_reported_value(value, self.publish_full_doc)
+
+        logger.debug(f"Updating reported shadow value to '{reported}'...")
+        return self.update_shadow_request(reported=reported, desired=None)
+
+    def change_desired_value(self, value: ShadowDocument) -> "Future[None]":
+        desired = self.locked_data.update_desired_value(value, self.publish_full_doc)
+
+        logger.debug(f"Updating desired shadow value to '{desired}'...")
+        return self.update_shadow_request(reported=None, desired=desired)
+
+    def change_both_values(
+        self, desired_value: ShadowDocument, reported_value: ShadowDocument
+    ) -> "Future[None]":
+        desired, reported = self.locked_data.update_both_values(
+            desired_value, reported_value, self.publish_full_doc
         )
-        future = self.client.publish_update_named_shadow(request, self.qos)
-        future.add_done_callback(self.on_publish_update_named_shadow)
 
-    def change_desired_value(self, value: ShadowDocument) -> None:
-        with self.locked_data.lock:
-            if self.locked_data.desired_value == value:
-                logger.debug("Local desired value is already '{}'.".format(value))
-                return
-            if self.publish_full_doc:
-                desired = value
-            else:
-                desired = dictdiff.dictdiff(self.locked_data.desired_value, value)
-            logger.debug("Changed local desired value to '{}'.".format(value))
-            self.locked_data.desired_value = value
-
-        logger.debug("Updating desired shadow value to '{}'...".format(desired))
-        request = iotshadow.UpdateNamedShadowRequest(
-            thing_name=self.thing_name,
-            shadow_name=self.shadow_name,
-            state=iotshadow.ShadowState(
-                desired=desired,
-            ),
-        )
-        future = self.client.publish_update_named_shadow(request, self.qos)
-        future.add_done_callback(self.on_publish_update_named_shadow)
-
-    def change_both_values(self, desired_value: ShadowDocument, reported_value: ShadowDocument) -> None:
-        with self.locked_data.lock:
-            if self.locked_data.desired_value == desired_value and self.locked_data.reported_value == reported_value:
-                logger.debug("Both of desired and reported values are unchanged.")
-                return
-            if self.publish_full_doc:
-                desired = desired_value
-                reported = reported_value
-            else:
-                desired = dictdiff.dictdiff(self.locked_data.desired_value, desired_value)
-                reported = dictdiff.dictdiff(self.locked_data.reported_value, reported_value)
-            logger.debug("Changed local desired value to '{}'.".format(desired_value))
-            self.locked_data.desired_value = desired_value
-            logger.debug("Changed local reported value to '{}'.".format(reported_value))
-            self.locked_data.reported_value = reported_value
-
-        logger.debug("Updating desired shadow value to '{}'...".format(desired))
-        request = iotshadow.UpdateNamedShadowRequest(
-            thing_name=self.thing_name,
-            shadow_name=self.shadow_name,
-            state=iotshadow.ShadowState(
-                desired=desired,
-                reported=reported,
-            ),
-        )
-        future = self.client.publish_update_named_shadow(request, self.qos)
-        future.add_done_callback(self.on_publish_update_named_shadow)
-
-    def get_reported_value(self) -> ShadowDocument:
-        return self.locked_data.reported_value
-
-    def get_desired_value(self) -> ShadowDocument:
-        return self.locked_data.desired_value
+        return self.update_shadow_request(desired=desired, reported=reported)
```

### Comparing `awsiotclient-0.1.1/src/awsiotclient/pubsub.py` & `awsiotclient-0.2.0/src/awsiotclient/pubsub.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,62 @@
 import json
+from concurrent.futures import Future
 from typing import Any, Callable, Dict, Optional
 
 from awscrt import mqtt
-from awsiotclient import get_module_logger
+
+from . import get_module_logger
 
 logger = get_module_logger(__name__)
 
 
-def empty_func(topic: str, payload: Optional[Dict[str, Any]], **kwargs: Optional[Dict[str, Any]]) -> None:
+def empty_func(
+    topic: str, payload: Optional[Dict[str, Any]], **kwargs: Optional[Dict[str, Any]]
+) -> None:
     logger.debug(f"empty_func: {topic}, {payload}")
 
 
 class Subscriber:
     def __init__(
         self,
         connection: mqtt.Connection,
         topic: str,
         qos: mqtt.QoS = mqtt.QoS.AT_LEAST_ONCE,
         callback: Callable[[str, Optional[Dict[str, Any]]], None] = empty_func,
     ):
         self.callback = callback
-        self.future, self.packet_id = connection.subscribe(topic=topic, qos=qos, callback=self.on_message_received)
+        self.future, self.packet_id = connection.subscribe(
+            topic=topic, qos=qos, callback=self.on_message_received
+        )
 
         self.result = self.future.result()
         logger.debug(f"Subscribed with {str(self.result['qos'])}")
 
     def on_message_received(self, topic: str, payload: bytes) -> None:
         packet = json.loads(payload)
         self.callback(topic, packet)
         logger.debug(f"Received message from topic '{topic}': {packet}")
 
 
 class Publisher:
-    def __init__(self, connection: mqtt.Connection, topic: str, qos: mqtt.QoS = mqtt.QoS.AT_LEAST_ONCE):
+    def __init__(
+        self,
+        connection: mqtt.Connection,
+        topic: str,
+        qos: mqtt.QoS = mqtt.QoS.AT_LEAST_ONCE,
+    ):
         self.connection = connection
         self.topic = topic
         self.qos = qos
 
-    def publish(self, payload: Optional[Dict[str, Any]]) -> None:
+    def publish(self, payload: Optional[Dict[str, Any]]) -> "Future[Any]":
         if payload:
             logger.debug(f"Publishing message to topic '{self.topic}': {payload}")
-            self.connection.publish(topic=self.topic, payload=json.dumps(payload), qos=self.qos)
+            future, _ = self.connection.publish(
+                topic=self.topic, payload=json.dumps(payload), qos=self.qos
+            )
         else:
             logger.debug(f"Empty payload. Nothing will be publshed to '{self.topic}'")
+            future = Future()
+            future.set_result(None)
+
+        return future
```

### Comparing `awsiotclient-0.1.1/setup.py` & `awsiotclient-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,137 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: awsiotclient
+Version: 0.2.0
+Summary: The AWS IoT Device Client provides device-side functionality for AWS IoT services such as jobs, device shadow, and simple pubsub.
+Home-page: https://github.com/whill-labs/aws-iot-device-client-python
+License: Apache-2.0
+Author: Seiya Shimizu
+Author-email: seiya.shimizu@gmail.com
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: awsiotsdk (>=1.5.11,<2.0.0)
+Project-URL: Repository, https://github.com/whill-labs/aws-iot-device-client-python
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# aws-iot-device-client-python
 
-packages = \
-['awsiotclient']
+The AWS IoT Device Client provides device-side functionality for AWS IoT services such as jobs, device shadow, and simple pubsub.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['awsiotsdk>=1.5.11,<2.0.0']
-
-setup_kwargs = {
-    'name': 'awsiotclient',
-    'version': '0.1.1',
-    'description': 'The AWS IoT Device Client provides device-side functionality for AWS IoT services such as jobs, device shadow, and simple pubsub.',
-    'long_description': '# aws-iot-device-client-python\n\nThe AWS IoT Device Client provides device-side functionality for AWS IoT services such as jobs, device shadow, and simple pubsub.\n\n## Installation\n\n### Minimum Requirements\n\n- Python 3.6+\n\n### Install from PyPI\n\n```shell\npython3 -m pip install awsiotclient\n```\n\n### Install from source\n\n```shell\ngit clone https://github.com/whill-labs/aws-iot-device-client-python\npython3 -m pip install ./aws-iot-device-client-python\n```\n\n## Usage\n\n### Create MQTT connection\n\n```python\nfrom awsiotclient import mqtt\n\n# Construct connection parameters\nconn_params = mqtt.ConnectionParams()\n\n# Required params\nconn_params.endpoint = <your_endpoint_url>\nconn_params.cert = <path_to_your_certificate>\nconn_params.key = <path_to_your_private_key>\nconn_params.root_ca = <path_to_your_root_ca>\n\n# Optional params\nconn_params.client_id = <client_id> # default "mqtt-" + uuid4()\nconn_params.signing_region = <signing_region> # default "ap-northeast-1" (Tokyo Region)\nconn_params.use_websocket = <True/False> # default False\n\n# Initialize connection\nmqtt_connection = mqtt.init(conn_params)\nconnect_future = mqtt_connection.connect()\nconnect_future.result()\n```\n\n### Use AWS IoT named shadow\n\nNote that usage of classic shadow client is similar to named shadow client.\n\n#### without delta (one-way communication from device to cloud)\n\n```python\nfrom awsiotclient import mqtt, named_shadow\n\n# <create mqtt connection here as described above>\nmy_client = named_shadow.client(\n    mqtt_connection,\n    thing_name="my_thing",\n    shadow_name="my_shadow"\n)\n\nmy_value = dict(foo="var")\nmy_clinet.change_reported_value(my_value)\n```\n\n#### with delta (two-way communication from/to device and cloud)\n\n```python\nfrom awsiotclient import mqtt, named_shadow\n\ndef my_delta_func(thing_name: str, shadow_name: str, value: Dict[str, Any]) -> None:\n    print("my_client invokes this callback when it receives delta message")\n    print(f"thing_name: {thing_name}, shadow_name: {shadow_name}, value: {value}")\n\n# <create mqtt connection here as described above>\nmy_client = named_shadow.client(\n    mqtt_connection,\n    thing_name="my_thing",\n    shadow_name="my_shadow",\n    delta_func=my_delta_func,\n)\n\nmy_value = dict(foo="var")\nmy_client.change_reported_value(my_value)\n# <wait until the client receives delta>\n```\n\n### Use AWS IoT jobs\n\n```python\nfrom awsiotclient import mqtt, named_shadow\n\ndef job_runner(id: str, document: dict):\n    print("my_client invokes this callback when it receives job document")\n    print(f"job id: {id}, document: {document}")\n\n# <create mqtt connection here as described above\njob_client = jobs.client(\n    mqtt_connection,\n    thing_name="my_thing",\n    job_func=job_runner\n)\n# <wait until the client receives job>\n```\n\n## License\n\nThis library is licensed under the Apache 2.0 License.\n\n## Acknowledgments\n\n- [AWS IoT Device SDK v2 for Python](https://github.com/aws/aws-iot-device-sdk-python-v2)\n',
-    'author': 'Seiya Shimizu',
-    'author_email': 'seiya.shimizu@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/whill-labs/aws-iot-device-client-python',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
+## Installation
 
+### Minimum Requirements
+
+- Python 3.7.1+
+
+### Install from PyPI
+
+```shell
+python3 -m pip install awsiotclient
+```
+
+### Install from source
+
+```shell
+git clone https://github.com/whill-labs/aws-iot-device-client-python
+python3 -m pip install ./aws-iot-device-client-python
+```
+
+## Usage
+
+### Create MQTT connection
+
+```python
+from awsiotclient import mqtt
+
+# Construct connection parameters
+conn_params = mqtt.ConnectionParams()
+
+# Required params
+conn_params.endpoint = <your_endpoint_url>
+conn_params.cert = <path_to_your_certificate>
+conn_params.key = <path_to_your_private_key>
+conn_params.root_ca = <path_to_your_root_ca>
+
+# Optional params
+conn_params.client_id = <client_id> # default "mqtt-" + uuid4()
+conn_params.signing_region = <signing_region> # default "ap-northeast-1" (Tokyo Region)
+conn_params.use_websocket = <True/False> # default False
+
+# Initialize connection
+mqtt_connection = mqtt.init(conn_params)
+connect_future = mqtt_connection.connect()
+connect_future.result()
+```
+
+### Use AWS IoT named shadow
+
+Note that usage of classic shadow client is similar to named shadow client.
+
+#### without delta (one-way communication from device to cloud)
+
+```python
+from awsiotclient import mqtt, named_shadow
+
+# <create mqtt connection here as described above>
+my_client = named_shadow.client(
+    mqtt_connection,
+    thing_name="my_thing",
+    shadow_name="my_shadow"
+)
+
+my_value = dict(foo="var")
+my_clinet.change_reported_value(my_value)
+```
+
+#### with delta (two-way communication from/to device and cloud)
+
+```python
+from awsiotclient import mqtt, named_shadow
+
+def my_delta_func(thing_name: str, shadow_name: str, value: Dict[str, Any]) -> None:
+    print("my_client invokes this callback when it receives delta message")
+    print(f"thing_name: {thing_name}, shadow_name: {shadow_name}, value: {value}")
+
+# <create mqtt connection here as described above>
+my_client = named_shadow.client(
+    mqtt_connection,
+    thing_name="my_thing",
+    shadow_name="my_shadow",
+    delta_func=my_delta_func,
+)
+
+my_value = dict(foo="var")
+my_client.change_reported_value(my_value)
+# <wait until the client receives delta>
+```
+
+### Use AWS IoT jobs
+
+```python
+from awsiotclient import mqtt, named_shadow
+
+def job_runner(id: str, document: dict):
+    print("my_client invokes this callback when it receives job document")
+    print(f"job id: {id}, document: {document}")
+
+# <create mqtt connection here as described above
+job_client = jobs.client(
+    mqtt_connection,
+    thing_name="my_thing",
+    job_func=job_runner
+)
+# <wait until the client receives job>
+```
+
+## License
+
+This library is licensed under the Apache 2.0 License.
+
+## Acknowledgments
+
+- [AWS IoT Device SDK v2 for Python](https://github.com/aws/aws-iot-device-sdk-python-v2)
 
-setup(**setup_kwargs)
```

