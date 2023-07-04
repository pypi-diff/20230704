# Comparing `tmp/mesh_sandbox-1.0.4-py3-none-any.whl.zip` & `tmp/mesh_sandbox-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 78309 bytes, number of entries: 76
+Zip file size: 78308 bytes, number of entries: 76
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 mesh_sandbox/__init__.py
 -rw-r--r--  2.0 unx     3925 b- defN 80-Jan-01 00:00 mesh_sandbox/api.py
 -rw-r--r--  2.0 unx     3403 b- defN 80-Jan-01 00:00 mesh_sandbox/common/__init__.py
 -rw-r--r--  2.0 unx     6504 b- defN 80-Jan-01 00:00 mesh_sandbox/common/constants.py
 -rw-r--r--  2.0 unx     1481 b- defN 80-Jan-01 00:00 mesh_sandbox/common/exceptions.py
 -rw-r--r--  2.0 unx      551 b- defN 80-Jan-01 00:00 mesh_sandbox/common/fernet.py
 -rw-r--r--  2.0 unx      392 b- defN 80-Jan-01 00:00 mesh_sandbox/common/handler_helpers.py
@@ -48,15 +48,15 @@
 -rw-r--r--  2.0 unx     1643 b- defN 80-Jan-01 00:00 mesh_sandbox/store/memory_store.py
 -rw-r--r--  2.0 unx     3615 b- defN 80-Jan-01 00:00 mesh_sandbox/store/serialisation.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mesh_sandbox/test_plugin/__init__.py
 -rw-r--r--  2.0 unx      967 b- defN 80-Jan-01 00:00 mesh_sandbox/test_plugin/example_plugin.py
 -rw-r--r--  2.0 unx       24 b- defN 80-Jan-01 00:00 mesh_sandbox/test_plugin/example_plugin.txt
 -rw-r--r--  2.0 unx      106 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/__init__.py
 -rw-r--r--  2.0 unx    14549 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/admin.py
--rw-r--r--  2.0 unx     1584 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/docker_tests.py
+-rw-r--r--  2.0 unx     1598 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/docker_tests.py
 -rw-r--r--  2.0 unx      740 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/exceptions.py
 -rw-r--r--  2.0 unx     6259 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/handshake.py
 -rw-r--r--  2.0 unx     6885 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/helpers.py
 -rw-r--r--  2.0 unx    10412 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/inbox.py
 -rw-r--r--  2.0 unx     6547 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/java_client_tests.py
 -rw-r--r--  2.0 unx     2768 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/lookup.py
 -rw-r--r--  2.0 unx     3901 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/mesh_api_helpers.py
@@ -67,12 +67,12 @@
 -rw-r--r--  2.0 unx     1237 b- defN 80-Jan-01 00:00 mesh_sandbox/views/__init__.py
 -rw-r--r--  2.0 unx     1315 b- defN 80-Jan-01 00:00 mesh_sandbox/views/admin.py
 -rw-r--r--  2.0 unx     3885 b- defN 80-Jan-01 00:00 mesh_sandbox/views/error.py
 -rw-r--r--  2.0 unx     5662 b- defN 80-Jan-01 00:00 mesh_sandbox/views/inbox.py
 -rw-r--r--  2.0 unx     2775 b- defN 80-Jan-01 00:00 mesh_sandbox/views/lookup.py
 -rw-r--r--  2.0 unx     4932 b- defN 80-Jan-01 00:00 mesh_sandbox/views/outbox.py
 -rw-r--r--  2.0 unx     8918 b- defN 80-Jan-01 00:00 mesh_sandbox/views/tracking.py
--rw-r--r--  2.0 unx     2428 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx     1051 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     6901 b- defN 16-Jan-01 00:00 mesh_sandbox-1.0.4.dist-info/RECORD
-76 files, 259441 bytes uncompressed, 67191 bytes compressed:  74.1%
+-rw-r--r--  2.0 unx     1051 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2388 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     6901 b- defN 16-Jan-01 00:00 mesh_sandbox-1.0.5.dist-info/RECORD
+76 files, 259415 bytes uncompressed, 67190 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -210,20 +210,20 @@
 
 Filename: mesh_sandbox/views/outbox.py
 Comment: 
 
 Filename: mesh_sandbox/views/tracking.py
 Comment: 
 
-Filename: mesh_sandbox-1.0.4.dist-info/METADATA
+Filename: mesh_sandbox-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: mesh_sandbox-1.0.4.dist-info/LICENSE
+Filename: mesh_sandbox-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: mesh_sandbox-1.0.4.dist-info/WHEEL
+Filename: mesh_sandbox-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: mesh_sandbox-1.0.4.dist-info/RECORD
+Filename: mesh_sandbox-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mesh_sandbox/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.4"
+__version__ = "1.0.5"
```

## mesh_sandbox/tests/docker_tests.py

```diff
@@ -28,15 +28,15 @@
         sent_payload = b"a" * 1000
 
         message_id = sender.send_message(_CANNED_MAILBOX2, sent_payload, workflow_id=workflow_id, subject="change me")
 
         assert message_id
 
         with MeshClient(
-            url=base_uri, mailbox=recipient_mailbox_id, password=_PASSWORD, shared_key=_SHARED_KEY
+            url=base_uri, mailbox=recipient_mailbox_id, password=_PASSWORD, shared_key=_SHARED_KEY, verify=False
         ) as recipient:
             message_ids = recipient.list_messages()
             assert message_ids == [message_id]
             message = recipient.retrieve_message(message_id)
             assert message.workflow_id == workflow_id  # pylint: disable=no-member
             received_payload = message.read()
             assert received_payload == sent_payload
```

## Comparing `mesh_sandbox-1.0.4.dist-info/METADATA` & `mesh_sandbox-1.0.5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: mesh-sandbox
-Version: 1.0.4
+Version: 1.0.5
 Summary: NHSDigital mesh sandbox, a locally testable version of the MESH api
 License: MIT
 Author: spinecore
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=39.0.1,<42.0.0)
-Requires-Dist: fastapi (>=0.94,<0.96)
+Requires-Dist: fastapi (>=0.94,<0.99)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
-Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: types-python-dateutil (>=2.8.9,<3.0.0)
 Requires-Dist: uvicorn (>=0.21,<0.23)
 Description-Content-Type: text/markdown
 
 MESH Sandbox
 ===========
@@ -46,15 +45,15 @@
 version: '3.9'
 
 
 services:
 
   mesh_sandbox:
     build: 
-      context: https://github.com/NHSDigital/mesh-sandbox.git#develop
+      context: https://github.com/NHSDigital/mesh-sandbox.git#refs/tags/v1.0.4
     ports:
       - "8700:80"
     deploy:
       restart_policy:
         condition: on-failure
         max_attempts: 3
     healthcheck:
```

## Comparing `mesh_sandbox-1.0.4.dist-info/LICENSE` & `mesh_sandbox-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mesh_sandbox-1.0.4.dist-info/RECORD` & `mesh_sandbox-1.0.5.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-mesh_sandbox/__init__.py,sha256=acuR_XSJzp4OrQ5T8-Ac5gYe48mUwObuwjRmisFmZ7k,22
+mesh_sandbox/__init__.py,sha256=B9kKWJLln1i8LjtkcYecvNWGLTrez4gCUOHtnPlInFo,22
 mesh_sandbox/api.py,sha256=F2KUKENAsSe6NAGG0wzHA2jebGF6mWFgta1q55oqacU,3925
 mesh_sandbox/common/__init__.py,sha256=MwKS4FixADUGgN49MQJI7vW0Wx6mnf9SBOPbgE4RddM,3403
 mesh_sandbox/common/constants.py,sha256=_hnaHDkAQGHWLF7n_WfC5ZHIY5D-fUbOdpSqLusUMNY,6504
 mesh_sandbox/common/exceptions.py,sha256=YQII8w6DQQoKuW0cukEr6PIE9j0rwrqDpCn5lapgmkQ,1481
 mesh_sandbox/common/fernet.py,sha256=f8yygkVnK1cmQLBgcPifoB4PwGpgiOrG8Yk-6OMDy8o,551
 mesh_sandbox/common/handler_helpers.py,sha256=Eg00Tide2mL87EoMFw83fDuxiTL5DgIwxHs2RaJasgE,392
 mesh_sandbox/common/messaging.py,sha256=xZbNpWQLhfjI4wiBG3PpIkEy2WbvwxqaWSR90sSb4hk,14664
@@ -47,15 +47,15 @@
 mesh_sandbox/store/memory_store.py,sha256=VJTsPAnwvPAVFTEo-mO2A__lcc7jMnyqiq0JerYmrKY,1643
 mesh_sandbox/store/serialisation.py,sha256=pMYZ704GP74aCDRX9Nu1r4B1XA4BPJXYY-RKLFJJfUg,3615
 mesh_sandbox/test_plugin/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mesh_sandbox/test_plugin/example_plugin.py,sha256=MnNpyyWKziqvOr89LeIxOwqskwHcrSsh_te67SeNJr4,967
 mesh_sandbox/test_plugin/example_plugin.txt,sha256=aUePU6UUVhpxeP37Pdz5Zxyn_nxI6HCY3qtQBo1iUEI,24
 mesh_sandbox/tests/__init__.py,sha256=wPjH0Ka1334a0OR9VMUfeYxsr03JqWjHTBnAH_1SB7I,106
 mesh_sandbox/tests/admin.py,sha256=Y_nzBhqSGPCTjG3EczSHClA-mVALGNBd-iOShoYh8WU,14549
-mesh_sandbox/tests/docker_tests.py,sha256=SJuuquoQA7_fP49--89mrIZmY_4KRO7fiFkOcZeR4AU,1584
+mesh_sandbox/tests/docker_tests.py,sha256=-dLCnAdgZkpU6tkgO4FwO7Sjvt5zZe45ewBSXo5afT0,1598
 mesh_sandbox/tests/exceptions.py,sha256=j_jKskVzLAYpyu4qNAEY5ahkbk8Uh2Nc_CGpnpdXjnI,740
 mesh_sandbox/tests/handshake.py,sha256=X-fCbwaEAc8cAvvnniCvt4W4DAV9ItPq7tpIpZkfj6M,6259
 mesh_sandbox/tests/helpers.py,sha256=wRC1t8mj4FKChebvwfcJWpxqK_nmE1NBUHgfCA2rBsk,6885
 mesh_sandbox/tests/inbox.py,sha256=GLqOC6qlivKpp7qEtcGqv_nECkf2MhP4XwRWbIPC_ks,10412
 mesh_sandbox/tests/java_client_tests.py,sha256=NYvNH1LxJc0SmHQ3q6mSvEd6Wuv2r_xMqAXW28sT2Pw,6547
 mesh_sandbox/tests/lookup.py,sha256=wY8x0F415y2um48Lw5kyD4ugMo1vBGKB7cqPdHEaVO4,2768
 mesh_sandbox/tests/mesh_api_helpers.py,sha256=ZedDWMHO88j4Zxw3hsK5vmvivy3UhdzbzHle0g9GJXA,3901
@@ -66,11 +66,11 @@
 mesh_sandbox/views/__init__.py,sha256=nZkb6_1S8jz8Xl_AayfwjgEZG0JD2dfulfGxjJ5W9Ec,1237
 mesh_sandbox/views/admin.py,sha256=2YGslfDyC0QKoq3WTGXBicqrOMR9UmQYocP3R0qTbAY,1315
 mesh_sandbox/views/error.py,sha256=9lnUr3P93Vm-nOrBTEuAD6nrSBUvpI6-XqXzILWjgGk,3885
 mesh_sandbox/views/inbox.py,sha256=gnaD9Csx5BqilVRefQQ_tXmeq80lwcLJfepW005GrkU,5662
 mesh_sandbox/views/lookup.py,sha256=HHUqZ-Iy22ysC3qaO8Bl5GBQqf_7IiBbe5acyxqS78M,2775
 mesh_sandbox/views/outbox.py,sha256=jxYiHylEdpljZ6Wl45Ke3aaH5rEKb-kzUuCNEKDS3So,4932
 mesh_sandbox/views/tracking.py,sha256=1H7Ghcvqkmx__KS1Y-lm105EVx_Z1eJo3oMDh8pzRMQ,8918
-mesh_sandbox-1.0.4.dist-info/METADATA,sha256=Wh9gYotOc1wzMnqO-Kf-WUzTFko6JEQyM1sXnttQ72g,2428
-mesh_sandbox-1.0.4.dist-info/LICENSE,sha256=usgzIvDUpVX5pYZepJTRXQJqIaz0mdd32GuS5a3PFlY,1051
-mesh_sandbox-1.0.4.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-mesh_sandbox-1.0.4.dist-info/RECORD,,
+mesh_sandbox-1.0.5.dist-info/LICENSE,sha256=usgzIvDUpVX5pYZepJTRXQJqIaz0mdd32GuS5a3PFlY,1051
+mesh_sandbox-1.0.5.dist-info/METADATA,sha256=yP1kTIaacLRi87NEWBDfZKAM_dENdkCnBobL57T2QWE,2388
+mesh_sandbox-1.0.5.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+mesh_sandbox-1.0.5.dist-info/RECORD,,
```

