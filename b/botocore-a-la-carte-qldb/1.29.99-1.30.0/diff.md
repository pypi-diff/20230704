# Comparing `tmp/botocore-a-la-carte-qldb-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-qldb-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-qldb-1.29.99.tar", last modified: Sat Mar 25 01:23:01 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-qldb-1.30.0.tar", last modified: Tue Jul  4 01:44:53 2023, max compression
```

## Comparing `botocore-a-la-carte-qldb-1.29.99.tar` & `botocore-a-la-carte-qldb-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:01.344663 botocore-a-la-carte-qldb-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:01.000000 botocore-a-la-carte-qldb-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-25 01:23:01.344663 botocore-a-la-carte-qldb-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:01.344663 botocore-a-la-carte-qldb-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:01.344663 botocore-a-la-carte-qldb-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:01.344663 botocore-a-la-carte-qldb-1.29.99/botocore/data/qldb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:01.344663 botocore-a-la-carte-qldb-1.29.99/botocore/data/qldb/2019-01-02/
--rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-03-25 01:22:12.000000 botocore-a-la-carte-qldb-1.29.99/botocore/data/qldb/2019-01-02/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-qldb-1.29.99/botocore/data/qldb/2019-01-02/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-25 01:22:12.000000 botocore-a-la-carte-qldb-1.29.99/botocore/data/qldb/2019-01-02/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    74293 2023-03-25 01:22:12.000000 botocore-a-la-carte-qldb-1.29.99/botocore/data/qldb/2019-01-02/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:01.344663 botocore-a-la-carte-qldb-1.29.99/botocore_a_la_carte_qldb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-25 01:23:01.000000 botocore-a-la-carte-qldb-1.29.99/botocore_a_la_carte_qldb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-25 01:23:01.000000 botocore-a-la-carte-qldb-1.29.99/botocore_a_la_carte_qldb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:01.000000 botocore-a-la-carte-qldb-1.29.99/botocore_a_la_carte_qldb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:01.000000 botocore-a-la-carte-qldb-1.29.99/botocore_a_la_carte_qldb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:01.344663 botocore-a-la-carte-qldb-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-25 01:23:01.000000 botocore-a-la-carte-qldb-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:53.306766 botocore-a-la-carte-qldb-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:53.000000 botocore-a-la-carte-qldb-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-04 01:44:53.306766 botocore-a-la-carte-qldb-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:53.306766 botocore-a-la-carte-qldb-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:53.306766 botocore-a-la-carte-qldb-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:53.306766 botocore-a-la-carte-qldb-1.30.0/botocore/data/qldb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:53.306766 botocore-a-la-carte-qldb-1.30.0/botocore/data/qldb/2019-01-02/
+-rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-07-04 01:44:02.000000 botocore-a-la-carte-qldb-1.30.0/botocore/data/qldb/2019-01-02/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-qldb-1.30.0/botocore/data/qldb/2019-01-02/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 01:44:02.000000 botocore-a-la-carte-qldb-1.30.0/botocore/data/qldb/2019-01-02/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    74308 2023-07-04 01:44:02.000000 botocore-a-la-carte-qldb-1.30.0/botocore/data/qldb/2019-01-02/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:53.306766 botocore-a-la-carte-qldb-1.30.0/botocore_a_la_carte_qldb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-04 01:44:53.000000 botocore-a-la-carte-qldb-1.30.0/botocore_a_la_carte_qldb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-04 01:44:53.000000 botocore-a-la-carte-qldb-1.30.0/botocore_a_la_carte_qldb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:53.000000 botocore-a-la-carte-qldb-1.30.0/botocore_a_la_carte_qldb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:53.000000 botocore-a-la-carte-qldb-1.30.0/botocore_a_la_carte_qldb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:53.306766 botocore-a-la-carte-qldb-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-04 01:44:53.000000 botocore-a-la-carte-qldb-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-qldb-1.29.99/LICENSE.txt` & `botocore-a-la-carte-qldb-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-qldb-1.29.99/PKG-INFO` & `botocore-a-la-carte-qldb-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-qldb
-Version: 1.29.99
+Version: 1.30.0
 Summary: qldb data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-qldb-1.29.99/botocore/data/qldb/2019-01-02/service-2.json` & `botocore-a-la-carte-qldb-1.30.0/botocore/data/qldb/2019-01-02/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8985127353266888%*

 * *Differences: {"'documentation'": "'<p>The resource management API for Amazon QLDB</p>'",*

 * * "'operations'": "{'DeleteLedger': {'documentation': '<p>Deletes a ledger and all of its contents. "*

 * *                 'This action is irreversible.</p> <p>If deletion protection is enabled, you must '*

 * *                 'first disable it before you can delete the ledger. You can disable it by calling '*

 * *                 'the <code>UpdateLedger</code> operation to set this parameter to '*

 * *                 "<code>false</code>.</p>'}, 'Exp […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "documentation": "<p>The control plane for Amazon QLDB</p>",
+    "documentation": "<p>The resource management API for Amazon QLDB</p>",
     "metadata": {
         "apiVersion": "2019-01-02",
         "endpointPrefix": "qldb",
         "jsonVersion": "1.0",
         "protocol": "rest-json",
         "serviceAbbreviation": "QLDB",
         "serviceFullName": "Amazon QLDB",
@@ -63,15 +63,15 @@
             },
             "name": "CreateLedger",
             "output": {
                 "shape": "CreateLedgerResponse"
             }
         },
         "DeleteLedger": {
-            "documentation": "<p>Deletes a ledger and all of its contents. This action is irreversible.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set the flag to <code>false</code>.</p>",
+            "documentation": "<p>Deletes a ledger and all of its contents. This action is irreversible.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set this parameter to <code>false</code>.</p>",
             "errors": [
                 {
                     "shape": "InvalidParameterException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -154,15 +154,15 @@
             },
             "name": "DescribeLedger",
             "output": {
                 "shape": "DescribeLedgerResponse"
             }
         },
         "ExportJournalToS3": {
-            "documentation": "<p>Exports journal contents within a date and time range from a ledger into a specified Amazon Simple Storage Service (Amazon S3) bucket. A journal export job can write the data objects in either the text or binary representation of Amazon Ion format, or in <i>JSON Lines</i> text format.</p> <p>In JSON Lines format, each journal block in the exported data object is a valid JSON object that is delimited by a newline. You can use this format to easily integrate JSON exports with analytics tools such as Glue and Amazon Athena because these services can parse newline-delimited JSON automatically. For more information about the format, see <a href=\"https://jsonlines.org/\">JSON Lines</a>.</p> <p>If the ledger with the given <code>Name</code> doesn't exist, then throws <code>ResourceNotFoundException</code>.</p> <p>If the ledger with the given <code>Name</code> is in <code>CREATING</code> status, then throws <code>ResourcePreconditionNotMetException</code>.</p> <p>You can initiate up to two concurrent journal export requests for each ledger. Beyond this limit, journal export requests throw <code>LimitExceededException</code>.</p>",
+            "documentation": "<p>Exports journal contents within a date and time range from a ledger into a specified Amazon Simple Storage Service (Amazon S3) bucket. A journal export job can write the data objects in either the text or binary representation of Amazon Ion format, or in <i>JSON Lines</i> text format.</p> <p>If the ledger with the given <code>Name</code> doesn't exist, then throws <code>ResourceNotFoundException</code>.</p> <p>If the ledger with the given <code>Name</code> is in <code>CREATING</code> status, then throws <code>ResourcePreconditionNotMetException</code>.</p> <p>You can initiate up to two concurrent journal export requests for each ledger. Beyond this limit, journal export requests throw <code>LimitExceededException</code>.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "ResourcePreconditionNotMetException"
                 }
@@ -251,15 +251,15 @@
             },
             "name": "GetRevision",
             "output": {
                 "shape": "GetRevisionResponse"
             }
         },
         "ListJournalKinesisStreamsForLedger": {
-            "documentation": "<p>Returns an array of all Amazon QLDB journal stream descriptors for a given ledger. The output of each stream descriptor includes the same details that are returned by <code>DescribeJournalKinesisStream</code>.</p> <p>This action does not return any expired journal streams. For more information, see <a href=\"https://docs.aws.amazon.com/qldb/latest/developerguide/streams.create.html#streams.create.states.expiration\">Expiration for terminal streams</a> in the <i>Amazon QLDB Developer Guide</i>.</p> <p>This action returns a maximum of <code>MaxResults</code> items. It is paginated so that you can retrieve all the items by calling <code>ListJournalKinesisStreamsForLedger</code> multiple times.</p>",
+            "documentation": "<p>Returns all Amazon QLDB journal streams for a given ledger.</p> <p>This action does not return any expired journal streams. For more information, see <a href=\"https://docs.aws.amazon.com/qldb/latest/developerguide/streams.create.html#streams.create.states.expiration\">Expiration for terminal streams</a> in the <i>Amazon QLDB Developer Guide</i>.</p> <p>This action returns a maximum of <code>MaxResults</code> items. It is paginated so that you can retrieve all the items by calling <code>ListJournalKinesisStreamsForLedger</code> multiple times.</p>",
             "errors": [
                 {
                     "shape": "InvalidParameterException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -276,43 +276,43 @@
             },
             "name": "ListJournalKinesisStreamsForLedger",
             "output": {
                 "shape": "ListJournalKinesisStreamsForLedgerResponse"
             }
         },
         "ListJournalS3Exports": {
-            "documentation": "<p>Returns an array of journal export job descriptions for all ledgers that are associated with the current Amazon Web Services account and Region.</p> <p>This action returns a maximum of <code>MaxResults</code> items, and is paginated so that you can retrieve all the items by calling <code>ListJournalS3Exports</code> multiple times.</p> <p>This action does not return any expired export jobs. For more information, see <a href=\"https://docs.aws.amazon.com/qldb/latest/developerguide/export-journal.request.html#export-journal.request.expiration\">Export job expiration</a> in the <i>Amazon QLDB Developer Guide</i>.</p>",
+            "documentation": "<p>Returns all journal export jobs for all ledgers that are associated with the current Amazon Web Services account and Region.</p> <p>This action returns a maximum of <code>MaxResults</code> items, and is paginated so that you can retrieve all the items by calling <code>ListJournalS3Exports</code> multiple times.</p> <p>This action does not return any expired export jobs. For more information, see <a href=\"https://docs.aws.amazon.com/qldb/latest/developerguide/export-journal.request.html#export-journal.request.expiration\">Export job expiration</a> in the <i>Amazon QLDB Developer Guide</i>.</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/journal-s3-exports"
             },
             "input": {
                 "shape": "ListJournalS3ExportsRequest"
             },
             "name": "ListJournalS3Exports",
             "output": {
                 "shape": "ListJournalS3ExportsResponse"
             }
         },
         "ListJournalS3ExportsForLedger": {
-            "documentation": "<p>Returns an array of journal export job descriptions for a specified ledger.</p> <p>This action returns a maximum of <code>MaxResults</code> items, and is paginated so that you can retrieve all the items by calling <code>ListJournalS3ExportsForLedger</code> multiple times.</p> <p>This action does not return any expired export jobs. For more information, see <a href=\"https://docs.aws.amazon.com/qldb/latest/developerguide/export-journal.request.html#export-journal.request.expiration\">Export job expiration</a> in the <i>Amazon QLDB Developer Guide</i>.</p>",
+            "documentation": "<p>Returns all journal export jobs for a specified ledger.</p> <p>This action returns a maximum of <code>MaxResults</code> items, and is paginated so that you can retrieve all the items by calling <code>ListJournalS3ExportsForLedger</code> multiple times.</p> <p>This action does not return any expired export jobs. For more information, see <a href=\"https://docs.aws.amazon.com/qldb/latest/developerguide/export-journal.request.html#export-journal.request.expiration\">Export job expiration</a> in the <i>Amazon QLDB Developer Guide</i>.</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/ledgers/{name}/journal-s3-exports"
             },
             "input": {
                 "shape": "ListJournalS3ExportsForLedgerRequest"
             },
             "name": "ListJournalS3ExportsForLedger",
             "output": {
                 "shape": "ListJournalS3ExportsForLedgerResponse"
             }
         },
         "ListLedgers": {
-            "documentation": "<p>Returns an array of ledger summaries that are associated with the current Amazon Web Services account and Region.</p> <p>This action returns a maximum of 100 items and is paginated so that you can retrieve all the items by calling <code>ListLedgers</code> multiple times.</p>",
+            "documentation": "<p>Returns all ledgers that are associated with the current Amazon Web Services account and Region.</p> <p>This action returns a maximum of <code>MaxResults</code> items and is paginated so that you can retrieve all the items by calling <code>ListLedgers</code> multiple times.</p>",
             "http": {
                 "method": "GET",
                 "requestUri": "/ledgers"
             },
             "input": {
                 "shape": "ListLedgersRequest"
             },
@@ -495,19 +495,19 @@
                 }
             },
             "type": "structure"
         },
         "CreateLedgerRequest": {
             "members": {
                 "DeletionProtection": {
-                    "documentation": "<p>The flag that prevents a ledger from being deleted by any user. If not provided on ledger creation, this feature is enabled (<code>true</code>) by default.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set the flag to <code>false</code>.</p>",
+                    "documentation": "<p>Specifies whether the ledger is protected from being deleted by any user. If not defined during ledger creation, this feature is enabled (<code>true</code>) by default.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set this parameter to <code>false</code>.</p>",
                     "shape": "DeletionProtection"
                 },
                 "KmsKey": {
-                    "documentation": "<p>The key in Key Management Service (KMS) to use for encryption of data at rest in the ledger. For more information, see <a href=\"https://docs.aws.amazon.com/qldb/latest/developerguide/encryption-at-rest.html\">Encryption at rest</a> in the <i>Amazon QLDB Developer Guide</i>.</p> <p>Use one of the following options to specify this parameter:</p> <ul> <li> <p> <code>AWS_OWNED_KMS_KEY</code>: Use an KMS key that is owned and managed by Amazon Web Services on your behalf.</p> </li> <li> <p> <b>Undefined</b>: By default, use an Amazon Web Services owned KMS key.</p> </li> <li> <p> <b>A valid symmetric customer managed KMS key</b>: Use the specified KMS key in your account that you create, own, and manage.</p> <p>Amazon QLDB does not support asymmetric keys. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/symmetric-asymmetric.html\">Using symmetric and asymmetric keys</a> in the <i>Key Management Service Developer Guide</i>.</p> </li> </ul> <p>To specify a customer managed KMS key, you can use its key ID, Amazon Resource Name (ARN), alias name, or alias ARN. When using an alias name, prefix it with <code>\"alias/\"</code>. To specify a key in a different Amazon Web Services account, you must use the key ARN or alias ARN.</p> <p>For example:</p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-east-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias ARN: <code>arn:aws:kms:us-east-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#key-id\">Key identifiers (KeyId)</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "documentation": "<p>The key in Key Management Service (KMS) to use for encryption of data at rest in the ledger. For more information, see <a href=\"https://docs.aws.amazon.com/qldb/latest/developerguide/encryption-at-rest.html\">Encryption at rest</a> in the <i>Amazon QLDB Developer Guide</i>.</p> <p>Use one of the following options to specify this parameter:</p> <ul> <li> <p> <code>AWS_OWNED_KMS_KEY</code>: Use an KMS key that is owned and managed by Amazon Web Services on your behalf.</p> </li> <li> <p> <b>Undefined</b>: By default, use an Amazon Web Services owned KMS key.</p> </li> <li> <p> <b>A valid symmetric customer managed KMS key</b>: Use the specified symmetric encryption KMS key in your account that you create, own, and manage.</p> <p>Amazon QLDB does not support asymmetric keys. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/symmetric-asymmetric.html\">Using symmetric and asymmetric keys</a> in the <i>Key Management Service Developer Guide</i>.</p> </li> </ul> <p>To specify a customer managed KMS key, you can use its key ID, Amazon Resource Name (ARN), alias name, or alias ARN. When using an alias name, prefix it with <code>\"alias/\"</code>. To specify a key in a different Amazon Web Services account, you must use the key ARN or alias ARN.</p> <p>For example:</p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-east-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias ARN: <code>arn:aws:kms:us-east-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#key-id\">Key identifiers (KeyId)</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "KmsKey"
                 },
                 "Name": {
                     "documentation": "<p>The name of the ledger that you want to create. The name must be unique among all of the ledgers in your Amazon Web Services account in the current Region.</p> <p>Naming constraints for ledger names are defined in <a href=\"https://docs.aws.amazon.com/qldb/latest/developerguide/limits.html#limits.naming\">Quotas in Amazon QLDB</a> in the <i>Amazon QLDB Developer Guide</i>.</p>",
                     "shape": "LedgerName"
                 },
                 "PermissionsMode": {
@@ -532,15 +532,15 @@
                     "shape": "Arn"
                 },
                 "CreationDateTime": {
                     "documentation": "<p>The date and time, in epoch time format, when the ledger was created. (Epoch time format is the number of seconds elapsed since 12:00:00 AM January 1, 1970 UTC.)</p>",
                     "shape": "Timestamp"
                 },
                 "DeletionProtection": {
-                    "documentation": "<p>The flag that prevents a ledger from being deleted by any user. If not provided on ledger creation, this feature is enabled (<code>true</code>) by default.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set the flag to <code>false</code>.</p>",
+                    "documentation": "<p>Specifies whether the ledger is protected from being deleted by any user. If not defined during ledger creation, this feature is enabled (<code>true</code>) by default.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set this parameter to <code>false</code>.</p>",
                     "shape": "DeletionProtection"
                 },
                 "KmsKeyArn": {
                     "documentation": "<p>The ARN of the customer managed KMS key that the ledger uses for encryption at rest. If this parameter is undefined, the ledger uses an Amazon Web Services owned KMS key for encryption.</p>",
                     "shape": "Arn"
                 },
                 "Name": {
@@ -659,15 +659,15 @@
                     "shape": "Arn"
                 },
                 "CreationDateTime": {
                     "documentation": "<p>The date and time, in epoch time format, when the ledger was created. (Epoch time format is the number of seconds elapsed since 12:00:00 AM January 1, 1970 UTC.)</p>",
                     "shape": "Timestamp"
                 },
                 "DeletionProtection": {
-                    "documentation": "<p>The flag that prevents a ledger from being deleted by any user. If not provided on ledger creation, this feature is enabled (<code>true</code>) by default.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set the flag to <code>false</code>.</p>",
+                    "documentation": "<p>Specifies whether the ledger is protected from being deleted by any user. If not defined during ledger creation, this feature is enabled (<code>true</code>) by default.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set this parameter to <code>false</code>.</p>",
                     "shape": "DeletionProtection"
                 },
                 "EncryptionDescription": {
                     "documentation": "<p>Information about the encryption of data at rest in the ledger. This includes the current status, the KMS key, and when the key became inaccessible (in the case of an error).</p>",
                     "shape": "LedgerEncryptionDescription"
                 },
                 "Name": {
@@ -721,19 +721,19 @@
                 "Name": {
                     "documentation": "<p>The name of the ledger.</p>",
                     "location": "uri",
                     "locationName": "name",
                     "shape": "LedgerName"
                 },
                 "OutputFormat": {
-                    "documentation": "<p>The output format of your exported journal data. If this parameter is not specified, the exported data defaults to <code>ION_TEXT</code> format.</p>",
+                    "documentation": "<p>The output format of your exported journal data. A journal export job can write the data objects in either the text or binary representation of <a href=\"https://docs.aws.amazon.com/qldb/latest/developerguide/ion.html\">Amazon Ion</a> format, or in <a href=\"https://jsonlines.org/\">JSON Lines</a> text format.</p> <p>Default: <code>ION_TEXT</code> </p> <p>In JSON Lines format, each journal block in an exported data object is a valid JSON object that is delimited by a newline. You can use this format to directly integrate JSON exports with analytics tools such as Amazon Athena and Glue because these services can parse newline-delimited JSON automatically.</p>",
                     "shape": "OutputFormat"
                 },
                 "RoleArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that grants QLDB permissions for a journal export job to do the following:</p> <ul> <li> <p>Write objects into your Amazon Simple Storage Service (Amazon S3) bucket.</p> </li> <li> <p>(Optional) Use your customer managed key in Key Management Service (KMS) for server-side encryption of your exported data.</p> </li> </ul> <p>To pass a role to QLDB when requesting a journal export, you must have permissions to perform the <code>iam:PassRole</code> action on the IAM role resource. This is required for all journal export requests.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the IAM role that grants QLDB permissions for a journal export job to do the following:</p> <ul> <li> <p>Write objects into your Amazon S3 bucket.</p> </li> <li> <p>(Optional) Use your customer managed key in Key Management Service (KMS) for server-side encryption of your exported data.</p> </li> </ul> <p>To pass a role to QLDB when requesting a journal export, you must have permissions to perform the <code>iam:PassRole</code> action on the IAM role resource. This is required for all journal export requests.</p>",
                     "shape": "Arn"
                 },
                 "S3ExportConfiguration": {
                     "documentation": "<p>The configuration settings of the Amazon S3 bucket destination for your export request.</p>",
                     "shape": "S3ExportConfiguration"
                 }
             },
@@ -1024,15 +1024,15 @@
             },
             "type": "list"
         },
         "KinesisConfiguration": {
             "documentation": "<p>The configuration settings of the Amazon Kinesis Data Streams destination for an Amazon QLDB journal stream.</p>",
             "members": {
                 "AggregationEnabled": {
-                    "documentation": "<p>Enables QLDB to publish multiple data records in a single Kinesis Data Streams record, increasing the number of records sent per API call.</p> <p> <i>This option is enabled by default.</i> Record aggregation has important implications for processing records and requires de-aggregation in your stream consumer. To learn more, see <a href=\"https://docs.aws.amazon.com/streams/latest/dev/kinesis-kpl-concepts.html\">KPL Key Concepts</a> and <a href=\"https://docs.aws.amazon.com/streams/latest/dev/kinesis-kpl-consumer-deaggregation.html\">Consumer De-aggregation</a> in the <i>Amazon Kinesis Data Streams Developer Guide</i>.</p>",
+                    "documentation": "<p>Enables QLDB to publish multiple data records in a single Kinesis Data Streams record, increasing the number of records sent per API call.</p> <p>Default: <code>True</code> </p> <important> <p>Record aggregation has important implications for processing records and requires de-aggregation in your stream consumer. To learn more, see <a href=\"https://docs.aws.amazon.com/streams/latest/dev/kinesis-kpl-concepts.html\">KPL Key Concepts</a> and <a href=\"https://docs.aws.amazon.com/streams/latest/dev/kinesis-kpl-consumer-deaggregation.html\">Consumer De-aggregation</a> in the <i>Amazon Kinesis Data Streams Developer Guide</i>.</p> </important>",
                     "shape": "Boolean"
                 },
                 "StreamArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Kinesis Data Streams resource.</p>",
                     "shape": "Arn"
                 }
             },
@@ -1152,15 +1152,15 @@
         "ListJournalKinesisStreamsForLedgerResponse": {
             "members": {
                 "NextToken": {
                     "documentation": "<ul> <li> <p>If <code>NextToken</code> is empty, the last page of results has been processed and there are no more results to be retrieved.</p> </li> <li> <p>If <code>NextToken</code> is <i>not</i> empty, more results are available. To retrieve the next page of results, use the value of <code>NextToken</code> in a subsequent <code>ListJournalKinesisStreamsForLedger</code> call.</p> </li> </ul>",
                     "shape": "NextToken"
                 },
                 "Streams": {
-                    "documentation": "<p>The array of QLDB journal stream descriptors that are associated with the given ledger.</p>",
+                    "documentation": "<p>The QLDB journal streams that are currently associated with the given ledger.</p>",
                     "shape": "JournalKinesisStreamDescriptionList"
                 }
             },
             "type": "structure"
         },
         "ListJournalS3ExportsForLedgerRequest": {
             "members": {
@@ -1187,15 +1187,15 @@
                 "Name"
             ],
             "type": "structure"
         },
         "ListJournalS3ExportsForLedgerResponse": {
             "members": {
                 "JournalS3Exports": {
-                    "documentation": "<p>The array of journal export job descriptions that are associated with the specified ledger.</p>",
+                    "documentation": "<p>The journal export jobs that are currently associated with the specified ledger.</p>",
                     "shape": "JournalS3ExportList"
                 },
                 "NextToken": {
                     "documentation": "<ul> <li> <p>If <code>NextToken</code> is empty, then the last page of results has been processed and there are no more results to be retrieved.</p> </li> <li> <p>If <code>NextToken</code> is <i>not</i> empty, then there are more results available. To retrieve the next page of results, use the value of <code>NextToken</code> in a subsequent <code>ListJournalS3ExportsForLedger</code> call.</p> </li> </ul>",
                     "shape": "NextToken"
                 }
             },
@@ -1217,15 +1217,15 @@
                 }
             },
             "type": "structure"
         },
         "ListJournalS3ExportsResponse": {
             "members": {
                 "JournalS3Exports": {
-                    "documentation": "<p>The array of journal export job descriptions for all ledgers that are associated with the current Amazon Web Services account and Region.</p>",
+                    "documentation": "<p>The journal export jobs for all ledgers that are associated with the current Amazon Web Services account and Region.</p>",
                     "shape": "JournalS3ExportList"
                 },
                 "NextToken": {
                     "documentation": "<ul> <li> <p>If <code>NextToken</code> is empty, then the last page of results has been processed and there are no more results to be retrieved.</p> </li> <li> <p>If <code>NextToken</code> is <i>not</i> empty, then there are more results available. To retrieve the next page of results, use the value of <code>NextToken</code> in a subsequent <code>ListJournalS3Exports</code> call.</p> </li> </ul>",
                     "shape": "NextToken"
                 }
             },
@@ -1247,15 +1247,15 @@
                 }
             },
             "type": "structure"
         },
         "ListLedgersResponse": {
             "members": {
                 "Ledgers": {
-                    "documentation": "<p>The array of ledger summaries that are associated with the current Amazon Web Services account and Region.</p>",
+                    "documentation": "<p>The ledgers that are associated with the current Amazon Web Services account and Region.</p>",
                     "shape": "LedgerList"
                 },
                 "NextToken": {
                     "documentation": "<p>A pagination token, indicating whether there are more results available:</p> <ul> <li> <p>If <code>NextToken</code> is empty, then the last page of results has been processed and there are no more results to be retrieved.</p> </li> <li> <p>If <code>NextToken</code> is <i>not</i> empty, then there are more results available. To retrieve the next page of results, use the value of <code>NextToken</code> in a subsequent <code>ListLedgers</code> call.</p> </li> </ul>",
                     "shape": "NextToken"
                 }
             },
@@ -1409,15 +1409,15 @@
             "pattern": "^[A-Za-z-0-9-_.]+$",
             "type": "string"
         },
         "S3EncryptionConfiguration": {
             "documentation": "<p>The encryption settings that are used by a journal export job to write data in an Amazon Simple Storage Service (Amazon S3) bucket.</p>",
             "members": {
                 "KmsKeyArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of a symmetric key in Key Management Service (KMS). Amazon S3 does not support asymmetric KMS keys.</p> <p>You must provide a <code>KmsKeyArn</code> if you specify <code>SSE_KMS</code> as the <code>ObjectEncryptionType</code>.</p> <p> <code>KmsKeyArn</code> is not required if you specify <code>SSE_S3</code> as the <code>ObjectEncryptionType</code>.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of a symmetric encryption key in Key Management Service (KMS). Amazon S3 does not support asymmetric KMS keys.</p> <p>You must provide a <code>KmsKeyArn</code> if you specify <code>SSE_KMS</code> as the <code>ObjectEncryptionType</code>.</p> <p> <code>KmsKeyArn</code> is not required if you specify <code>SSE_S3</code> as the <code>ObjectEncryptionType</code>.</p>",
                     "shape": "Arn"
                 },
                 "ObjectEncryptionType": {
                     "documentation": "<p>The Amazon S3 object encryption type.</p> <p>To learn more about server-side encryption options in Amazon S3, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/serv-side-encryption.html\">Protecting Data Using Server-Side Encryption</a> in the <i>Amazon S3 Developer Guide</i>.</p>",
                     "shape": "S3ObjectEncryptionType"
                 }
             },
@@ -1650,19 +1650,19 @@
                 }
             },
             "type": "structure"
         },
         "UpdateLedgerRequest": {
             "members": {
                 "DeletionProtection": {
-                    "documentation": "<p>The flag that prevents a ledger from being deleted by any user. If not provided on ledger creation, this feature is enabled (<code>true</code>) by default.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set the flag to <code>false</code>.</p>",
+                    "documentation": "<p>Specifies whether the ledger is protected from being deleted by any user. If not defined during ledger creation, this feature is enabled (<code>true</code>) by default.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set this parameter to <code>false</code>.</p>",
                     "shape": "DeletionProtection"
                 },
                 "KmsKey": {
-                    "documentation": "<p>The key in Key Management Service (KMS) to use for encryption of data at rest in the ledger. For more information, see <a href=\"https://docs.aws.amazon.com/qldb/latest/developerguide/encryption-at-rest.html\">Encryption at rest</a> in the <i>Amazon QLDB Developer Guide</i>.</p> <p>Use one of the following options to specify this parameter:</p> <ul> <li> <p> <code>AWS_OWNED_KMS_KEY</code>: Use an KMS key that is owned and managed by Amazon Web Services on your behalf.</p> </li> <li> <p> <b>Undefined</b>: Make no changes to the KMS key of the ledger.</p> </li> <li> <p> <b>A valid symmetric customer managed KMS key</b>: Use the specified KMS key in your account that you create, own, and manage.</p> <p>Amazon QLDB does not support asymmetric keys. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/symmetric-asymmetric.html\">Using symmetric and asymmetric keys</a> in the <i>Key Management Service Developer Guide</i>.</p> </li> </ul> <p>To specify a customer managed KMS key, you can use its key ID, Amazon Resource Name (ARN), alias name, or alias ARN. When using an alias name, prefix it with <code>\"alias/\"</code>. To specify a key in a different Amazon Web Services account, you must use the key ARN or alias ARN.</p> <p>For example:</p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-east-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias ARN: <code>arn:aws:kms:us-east-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#key-id\">Key identifiers (KeyId)</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "documentation": "<p>The key in Key Management Service (KMS) to use for encryption of data at rest in the ledger. For more information, see <a href=\"https://docs.aws.amazon.com/qldb/latest/developerguide/encryption-at-rest.html\">Encryption at rest</a> in the <i>Amazon QLDB Developer Guide</i>.</p> <p>Use one of the following options to specify this parameter:</p> <ul> <li> <p> <code>AWS_OWNED_KMS_KEY</code>: Use an KMS key that is owned and managed by Amazon Web Services on your behalf.</p> </li> <li> <p> <b>Undefined</b>: Make no changes to the KMS key of the ledger.</p> </li> <li> <p> <b>A valid symmetric customer managed KMS key</b>: Use the specified symmetric encryption KMS key in your account that you create, own, and manage.</p> <p>Amazon QLDB does not support asymmetric keys. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/symmetric-asymmetric.html\">Using symmetric and asymmetric keys</a> in the <i>Key Management Service Developer Guide</i>.</p> </li> </ul> <p>To specify a customer managed KMS key, you can use its key ID, Amazon Resource Name (ARN), alias name, or alias ARN. When using an alias name, prefix it with <code>\"alias/\"</code>. To specify a key in a different Amazon Web Services account, you must use the key ARN or alias ARN.</p> <p>For example:</p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-east-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias ARN: <code>arn:aws:kms:us-east-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#key-id\">Key identifiers (KeyId)</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "KmsKey"
                 },
                 "Name": {
                     "documentation": "<p>The name of the ledger.</p>",
                     "location": "uri",
                     "locationName": "name",
                     "shape": "LedgerName"
@@ -1680,15 +1680,15 @@
                     "shape": "Arn"
                 },
                 "CreationDateTime": {
                     "documentation": "<p>The date and time, in epoch time format, when the ledger was created. (Epoch time format is the number of seconds elapsed since 12:00:00 AM January 1, 1970 UTC.)</p>",
                     "shape": "Timestamp"
                 },
                 "DeletionProtection": {
-                    "documentation": "<p>The flag that prevents a ledger from being deleted by any user. If not provided on ledger creation, this feature is enabled (<code>true</code>) by default.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set the flag to <code>false</code>.</p>",
+                    "documentation": "<p>Specifies whether the ledger is protected from being deleted by any user. If not defined during ledger creation, this feature is enabled (<code>true</code>) by default.</p> <p>If deletion protection is enabled, you must first disable it before you can delete the ledger. You can disable it by calling the <code>UpdateLedger</code> operation to set this parameter to <code>false</code>.</p>",
                     "shape": "DeletionProtection"
                 },
                 "EncryptionDescription": {
                     "documentation": "<p>Information about the encryption of data at rest in the ledger. This includes the current status, the KMS key, and when the key became inaccessible (in the case of an error).</p>",
                     "shape": "LedgerEncryptionDescription"
                 },
                 "Name": {
```

### Comparing `botocore-a-la-carte-qldb-1.29.99/botocore_a_la_carte_qldb.egg-info/PKG-INFO` & `botocore-a-la-carte-qldb-1.30.0/botocore_a_la_carte_qldb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-qldb
-Version: 1.29.99
+Version: 1.30.0
 Summary: qldb data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-qldb-1.29.99/setup.py` & `botocore-a-la-carte-qldb-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-qldb',
-    version="1.29.99",
+    version="1.30.0",
     description='qldb data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/qldb/*/*.json'],
```

