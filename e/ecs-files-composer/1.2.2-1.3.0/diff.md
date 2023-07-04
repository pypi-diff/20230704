# Comparing `tmp/ecs_files_composer-1.2.2.tar.gz` & `tmp/ecs_files_composer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_files_composer-1.2.2.tar", max compression
+gzip compressed data, was "ecs_files_composer-1.3.0.tar", max compression
```

## Comparing `ecs_files_composer-1.2.2.tar` & `ecs_files_composer-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    16725 2022-03-23 11:16:37.079578 ecs_files_composer-1.2.2/LICENSE
--rw-r--r--   0        0        0     3280 2022-03-23 11:16:37.079578 ecs_files_composer-1.2.2/README.rst
--rw-r--r--   0        0        0      223 2023-04-03 09:10:16.022288 ecs_files_composer-1.2.2/ecs_files_composer/__init__.py
--rw-r--r--   0        0        0     7806 2022-10-15 07:41:13.975939 ecs_files_composer-1.2.2/ecs_files_composer/aws_mgmt.py
--rw-r--r--   0        0        0     1981 2023-02-28 08:48:00.274715 ecs_files_composer-1.2.2/ecs_files_composer/certbot_aws_store.py
--rw-r--r--   0        0        0     4698 2023-02-28 08:05:01.104212 ecs_files_composer-1.2.2/ecs_files_composer/certificates_mgmt.py
--rw-r--r--   0        0        0     3984 2022-07-28 09:26:42.121128 ecs_files_composer-1.2.2/ecs_files_composer/cli.py
--rw-r--r--   0        0        0     1646 2022-07-27 07:35:07.930636 ecs_files_composer-1.2.2/ecs_files_composer/common.py
--rw-r--r--   0        0        0     5018 2023-03-28 09:44:31.264626 ecs_files_composer-1.2.2/ecs_files_composer/ecs_files_composer.py
--rw-r--r--   0        0        0     1669 2022-07-27 07:35:08.374630 ecs_files_composer-1.2.2/ecs_files_composer/envsubst.py
--rw-r--r--   0        0        0    13358 2023-03-28 09:44:31.264626 ecs_files_composer-1.2.2/ecs_files_composer/files_mgmt.py
--rw-r--r--   0        0        0     8563 2023-04-03 09:06:06.422245 ecs_files_composer-1.2.2/ecs_files_composer/input.py
--rw-r--r--   0        0        0     6057 2023-04-03 09:05:54.690104 ecs_files_composer-1.2.2/ecs_files_composer/jinja2_filters/__init__.py
--rw-r--r--   0        0        0      697 2022-11-16 09:43:55.387189 ecs_files_composer-1.2.2/ecs_files_composer/jinja2_filters/aws_filters.py
--rw-r--r--   0        0        0     2941 2023-04-03 09:10:16.022288 ecs_files_composer-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     4570 1970-01-01 00:00:00.000000 ecs_files_composer-1.2.2/setup.py
--rw-r--r--   0        0        0     4881 1970-01-01 00:00:00.000000 ecs_files_composer-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2022-03-23 11:16:37.079578 ecs_files_composer-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3280 2022-03-23 11:16:37.079578 ecs_files_composer-1.3.0/README.rst
+-rw-r--r--   0        0        0      223 2023-07-04 12:20:07.188973 ecs_files_composer-1.3.0/ecs_files_composer/__init__.py
+-rw-r--r--   0        0        0     7806 2022-10-15 07:41:13.975939 ecs_files_composer-1.3.0/ecs_files_composer/aws_mgmt.py
+-rw-r--r--   0        0        0     1981 2023-02-28 08:48:00.274715 ecs_files_composer-1.3.0/ecs_files_composer/certbot_aws_store.py
+-rw-r--r--   0        0        0     4698 2023-02-28 08:05:01.104212 ecs_files_composer-1.3.0/ecs_files_composer/certificates_mgmt.py
+-rw-r--r--   0        0        0     3984 2022-07-28 09:26:42.121128 ecs_files_composer-1.3.0/ecs_files_composer/cli.py
+-rw-r--r--   0        0        0     1646 2022-07-27 07:35:07.930636 ecs_files_composer-1.3.0/ecs_files_composer/common.py
+-rw-r--r--   0        0        0     5018 2023-03-28 09:44:31.264626 ecs_files_composer-1.3.0/ecs_files_composer/ecs_files_composer.py
+-rw-r--r--   0        0        0     1669 2022-07-27 07:35:08.374630 ecs_files_composer-1.3.0/ecs_files_composer/envsubst.py
+-rw-r--r--   0        0        0    13235 2023-07-04 12:18:06.235641 ecs_files_composer-1.3.0/ecs_files_composer/files_mgmt.py
+-rw-r--r--   0        0        0     8488 2023-07-04 12:18:06.236641 ecs_files_composer-1.3.0/ecs_files_composer/input.py
+-rw-r--r--   0        0        0     6057 2023-07-03 22:27:33.182231 ecs_files_composer-1.3.0/ecs_files_composer/jinja2_filters/__init__.py
+-rw-r--r--   0        0        0      697 2022-11-16 09:43:55.387189 ecs_files_composer-1.3.0/ecs_files_composer/jinja2_filters/aws_filters.py
+-rw-r--r--   0        0        0     2945 2023-07-04 12:20:07.188973 ecs_files_composer-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4678 1970-01-01 00:00:00.000000 ecs_files_composer-1.3.0/PKG-INFO
```

### Comparing `ecs_files_composer-1.2.2/LICENSE` & `ecs_files_composer-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-1.2.2/README.rst` & `ecs_files_composer-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-1.2.2/ecs_files_composer/aws_mgmt.py` & `ecs_files_composer-1.3.0/ecs_files_composer/aws_mgmt.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-1.2.2/ecs_files_composer/certbot_aws_store.py` & `ecs_files_composer-1.3.0/ecs_files_composer/certbot_aws_store.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-1.2.2/ecs_files_composer/certificates_mgmt.py` & `ecs_files_composer-1.3.0/ecs_files_composer/certificates_mgmt.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-1.2.2/ecs_files_composer/cli.py` & `ecs_files_composer-1.3.0/ecs_files_composer/cli.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-1.2.2/ecs_files_composer/common.py` & `ecs_files_composer-1.3.0/ecs_files_composer/common.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-1.2.2/ecs_files_composer/ecs_files_composer.py` & `ecs_files_composer-1.3.0/ecs_files_composer/ecs_files_composer.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-1.2.2/ecs_files_composer/envsubst.py` & `ecs_files_composer-1.3.0/ecs_files_composer/envsubst.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-1.2.2/ecs_files_composer/files_mgmt.py` & `ecs_files_composer-1.3.0/ecs_files_composer/files_mgmt.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,41 +146,39 @@
         """
         Handles retrieving the content from S3
 
         :param ecs_files_composer.input.IamOverrideDef iam_override:
         :param boto3.session.Session session_override:
         :return: bool, result of the download from S3.
         """
-        from ecs_files_composer.input import S3Def1
+        from ecs_files_composer.input import S3Def
 
-        if not isinstance(self.source.s3.__root__, S3Def1):
-            raise TypeError(
-                "S3 source is not of type S3Def1", type(self.source.s3.__root__)
-            )
+        if not isinstance(self.source.s3, S3Def):
+            raise TypeError("S3 source is not of type S3Def", type(self.source.s3))
 
-        if self.source.s3.__root__.iam_override:
-            fetcher = S3Fetcher(iam_config_object=self.source.s3.__root__.iam_override)
+        if self.source.s3.iam_override:
+            fetcher = S3Fetcher(iam_config_object=self.source.s3.iam_override)
         elif iam_override:
             fetcher = S3Fetcher(iam_config_object=iam_override)
         elif session_override:
             fetcher = S3Fetcher(client_session_override=session_override)
         else:
             fetcher = S3Fetcher()
         try:
-            if self.source.s3.__root__.s3_uri:
+            if self.source.s3.s3_uri:
                 self.content = fetcher.get_content(
-                    s3_uri=self.source.s3.__root__.s3_uri.__root__,
+                    s3_uri=self.source.s3.s3_uri.__root__,
                 )
-            elif self.source.s3.__root__.compose_x_uri:
+            elif self.source.s3.compose_x_uri:
                 self.content = fetcher.get_content(
-                    composex_uri=self.source.s3.__root__.compose_x_uri.__root__,
+                    composex_uri=self.source.s3.compose_x_uri.__root__,
                 )
             else:
-                bucket_name = expandvars(self.source.s3.__root__.bucket_name)
-                key = expandvars(self.source.s3.__root__.key)
+                bucket_name = expandvars(self.source.s3.bucket_name)
+                key = expandvars(self.source.s3.key)
                 self.content = fetcher.get_content(
                     s3_bucket=bucket_name,
                     s3_key=key,
                 )
             return True
         except Exception as error:
             LOG.error("Failed to retrieve file from AWS S3")
```

### Comparing `ecs_files_composer-1.2.2/ecs_files_composer/input.py` & `ecs_files_composer-1.3.0/ecs_files_composer/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # generated by datamodel-codegen:
 #   filename:  ecs-files-input.json
-#   timestamp: 2023-04-03T09:06:05+00:00
+#   timestamp: 2023-07-03T22:45:29+00:00
 
 from __future__ import annotations
 
 from enum import Enum
-from typing import Any, Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Extra, Field, constr
 
 
 class S3Uri(BaseModel):
     __root__: str = Field(
         ...,
@@ -150,15 +150,15 @@
         None,
         alias="JsonKey",
         description="If the SecretString is a valid JSON, use the Key to map to the value stored in secret",
     )
     iam_override: Optional[IamOverrideDef] = Field(None, alias="IamOverride")
 
 
-class S3Def1(BaseModel):
+class S3Def(BaseModel):
     s3_uri: Optional[S3Uri] = Field(None, alias="S3Uri")
     compose_x_uri: Optional[ComposeXUri] = Field(None, alias="ComposeXUri")
     bucket_name: Optional[str] = Field(
         None, alias="BucketName", description="Name of the S3 Bucket"
     )
     bucket_region: Optional[str] = Field(
         None,
@@ -167,18 +167,14 @@
     )
     key: Optional[str] = Field(
         None, alias="Key", description="Full path to the file to retrieve"
     )
     iam_override: Optional[IamOverrideDef] = Field(None, alias="IamOverride")
 
 
-class S3Def(BaseModel):
-    __root__: Union[S3Def1, Any, Any, Any]
-
-
 class X509CertDef(BaseModel):
     class Config:
         extra = Extra.allow
 
     dir_path: Optional[str] = None
     email_address: Optional[EmailStr] = Field(
         "files-composer@compose-x.tld", alias="emailAddress"
```

### Comparing `ecs_files_composer-1.2.2/ecs_files_composer/jinja2_filters/__init__.py` & `ecs_files_composer-1.3.0/ecs_files_composer/jinja2_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-1.2.2/ecs_files_composer/jinja2_filters/aws_filters.py` & `ecs_files_composer-1.3.0/ecs_files_composer/jinja2_filters/aws_filters.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-1.2.2/pyproject.toml` & `ecs_files_composer-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecs_files_composer"
-version = "1.2.2"
+version = "1.3.0"
 description = "Files and configuration handler to inject configuration files into volumes for ECS containers"
 authors = ["John Preston <john@compose-x.io>"]
 license = "MPL-2.0"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
@@ -17,38 +17,39 @@
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)"
 ]
 readme = "README.rst"
 keywords=["aws", "ecs", "k8s", "secrets"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-boto3 = "^1.26"
-pydantic = {extras = ["email"], version = "^1.9.0"}
+boto3 = ">=1.27,<2.0"
+pydantic = {extras = ["email"], version = "^1.9"}
 pyOpenSSL = "^22"
 requests = "^2.27.1"
 PyYAML = "^6.0"
 Jinja2 = "^3.1.2"
 jsonschema = "^4.17"
 compose-x-common = "^1.2"
 flatdict = "^4.0.1"
 pyjks = "^20.0.0"
 certbot-aws-store = "^0.4.2.post0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 placebo = "^0.10"
-datamodel-code-generator = {extras = ["http"], version = "^0.15"}
+datamodel-code-generator = {extras = ["http"], version = "^0.21"}
 black = "^23.1"
 isort = "^5.10.1"
 coverage = "^7.1"
 behave = "^1.2.6"
 pytest = "^7"
 watchdog = "^3.0"
-pre-commit = "^3.0"
+pre-commit = "^3.3"
 tbump = "^6.9.0"
 
+
 [tool.poetry.scripts]
 files_composer = "ecs_files_composer.cli:main"
 ecs_files_composer = "ecs_files_composer.cli:main"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.3.0"
 sphinx-material = "^0.0.35"
@@ -89,15 +90,15 @@
 
 omit = ["ecs_files_composer/cli.py"]
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/ecs-files-composer"
 
 [tool.tbump.version]
-current = "1.2.2"
+current = "1.3.0"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
@@ -113,9 +114,9 @@
 # tbump.toml location.
 [[tool.tbump.file]]
 src = "pyproject.toml"
 
 [[tool.tbump.file]]
 src = "ecs_files_composer/__init__.py"
 [build-system]
-requires = ["poetry-core>=1.2.1"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ecs_files_composer-1.2.2/PKG-INFO` & `ecs_files_composer-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs-files-composer
-Version: 1.2.2
+Version: 1.3.0
 Summary: Files and configuration handler to inject configuration files into volumes for ECS containers
 License: MPL-2.0
 Keywords: aws,ecs,k8s,secrets
 Author: John Preston
 Author-email: john@compose-x.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,27 +15,23 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: boto3 (>=1.26,<2.0)
+Requires-Dist: boto3 (>=1.27,<2.0)
 Requires-Dist: certbot-aws-store (>=0.4.2.post0,<0.5.0)
 Requires-Dist: compose-x-common (>=1.2,<2.0)
 Requires-Dist: flatdict (>=4.0.1,<5.0.0)
 Requires-Dist: jsonschema (>=4.17,<5.0)
 Requires-Dist: pyOpenSSL (>=22,<23)
-Requires-Dist: pydantic[email] (>=1.9.0,<2.0.0)
+Requires-Dist: pydantic[email] (>=1.9,<2.0)
 Requires-Dist: pyjks (>=20.0.0,<21.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Description-Content-Type: text/x-rst
 
 .. meta::
     :description: ECS Files Composer input config
     :keywords: AWS, AWS ECS, Docker, Compose, docker-compose, AWS S3, AWS SSM, Secrets, Configuration
```

