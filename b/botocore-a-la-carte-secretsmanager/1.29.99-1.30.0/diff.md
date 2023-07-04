# Comparing `tmp/botocore-a-la-carte-secretsmanager-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-secretsmanager-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-secretsmanager-1.29.99.tar", last modified: Sat Mar 25 01:23:14 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-secretsmanager-1.30.0.tar", last modified: Tue Jul  4 01:45:06 2023, max compression
```

## Comparing `botocore-a-la-carte-secretsmanager-1.29.99.tar` & `botocore-a-la-carte-secretsmanager-1.30.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:14.301266 botocore-a-la-carte-secretsmanager-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:14.000000 botocore-a-la-carte-secretsmanager-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-25 01:23:14.301266 botocore-a-la-carte-secretsmanager-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:14.301266 botocore-a-la-carte-secretsmanager-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:14.301266 botocore-a-la-carte-secretsmanager-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:14.301266 botocore-a-la-carte-secretsmanager-1.29.99/botocore/data/secretsmanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:14.301266 botocore-a-la-carte-secretsmanager-1.29.99/botocore/data/secretsmanager/2017-10-17/
--rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-03-25 01:22:12.000000 botocore-a-la-carte-secretsmanager-1.29.99/botocore/data/secretsmanager/2017-10-17/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-03-25 01:22:12.000000 botocore-a-la-carte-secretsmanager-1.29.99/botocore/data/secretsmanager/2017-10-17/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-25 01:22:12.000000 botocore-a-la-carte-secretsmanager-1.29.99/botocore/data/secretsmanager/2017-10-17/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   131111 2023-03-25 01:22:12.000000 botocore-a-la-carte-secretsmanager-1.29.99/botocore/data/secretsmanager/2017-10-17/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-25 01:22:12.000000 botocore-a-la-carte-secretsmanager-1.29.99/botocore/data/secretsmanager/2017-10-17/service-2.sdk-extras.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:14.301266 botocore-a-la-carte-secretsmanager-1.29.99/botocore_a_la_carte_secretsmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-25 01:23:14.000000 botocore-a-la-carte-secretsmanager-1.29.99/botocore_a_la_carte_secretsmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-25 01:23:14.000000 botocore-a-la-carte-secretsmanager-1.29.99/botocore_a_la_carte_secretsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:14.000000 botocore-a-la-carte-secretsmanager-1.29.99/botocore_a_la_carte_secretsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:14.000000 botocore-a-la-carte-secretsmanager-1.29.99/botocore_a_la_carte_secretsmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:14.301266 botocore-a-la-carte-secretsmanager-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-25 01:23:14.000000 botocore-a-la-carte-secretsmanager-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:06.722887 botocore-a-la-carte-secretsmanager-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:45:06.000000 botocore-a-la-carte-secretsmanager-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-04 01:45:06.722887 botocore-a-la-carte-secretsmanager-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:06.722887 botocore-a-la-carte-secretsmanager-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:06.722887 botocore-a-la-carte-secretsmanager-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:06.722887 botocore-a-la-carte-secretsmanager-1.30.0/botocore/data/secretsmanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:06.722887 botocore-a-la-carte-secretsmanager-1.30.0/botocore/data/secretsmanager/2017-10-17/
+-rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-07-04 01:44:02.000000 botocore-a-la-carte-secretsmanager-1.30.0/botocore/data/secretsmanager/2017-10-17/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-07-04 01:44:02.000000 botocore-a-la-carte-secretsmanager-1.30.0/botocore/data/secretsmanager/2017-10-17/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 01:44:02.000000 botocore-a-la-carte-secretsmanager-1.30.0/botocore/data/secretsmanager/2017-10-17/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   131455 2023-07-04 01:44:02.000000 botocore-a-la-carte-secretsmanager-1.30.0/botocore/data/secretsmanager/2017-10-17/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 01:44:02.000000 botocore-a-la-carte-secretsmanager-1.30.0/botocore/data/secretsmanager/2017-10-17/service-2.sdk-extras.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:06.722887 botocore-a-la-carte-secretsmanager-1.30.0/botocore_a_la_carte_secretsmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-04 01:45:06.000000 botocore-a-la-carte-secretsmanager-1.30.0/botocore_a_la_carte_secretsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-04 01:45:06.000000 botocore-a-la-carte-secretsmanager-1.30.0/botocore_a_la_carte_secretsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:45:06.000000 botocore-a-la-carte-secretsmanager-1.30.0/botocore_a_la_carte_secretsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:45:06.000000 botocore-a-la-carte-secretsmanager-1.30.0/botocore_a_la_carte_secretsmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:45:06.722887 botocore-a-la-carte-secretsmanager-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-04 01:45:06.000000 botocore-a-la-carte-secretsmanager-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-secretsmanager-1.29.99/LICENSE.txt` & `botocore-a-la-carte-secretsmanager-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-secretsmanager-1.29.99/PKG-INFO` & `botocore-a-la-carte-secretsmanager-1.30.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-secretsmanager
-Version: 1.29.99
+Version: 1.30.0
 Summary: secretsmanager data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-secretsmanager-1.29.99/botocore/data/secretsmanager/2017-10-17/endpoint-rule-set-1.json` & `botocore-a-la-carte-secretsmanager-1.30.0/botocore/data/secretsmanager/2017-10-17/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-secretsmanager-1.29.99/botocore/data/secretsmanager/2017-10-17/examples-1.json` & `botocore-a-la-carte-secretsmanager-1.30.0/botocore/data/secretsmanager/2017-10-17/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-secretsmanager-1.29.99/botocore/data/secretsmanager/2017-10-17/service-2.json` & `botocore-a-la-carte-secretsmanager-1.30.0/botocore/data/secretsmanager/2017-10-17/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999795757923971%*

 * *Differences: {"'operations'": "{'ValidateResourcePolicy': {'documentation': '<p>Validates that a resource "*

 * *                 'policy does not grant a wide range of principals access to your secret. A '*

 * *                 'resource-based policy is optional for secrets.</p> <p>The API performs three '*

 * *                 'checks when validating the policy:</p> <ul> <li> <p>Sends a call to <a '*

 * *                 'href="https://aws.amazon.com/blogs/security/protect-sensitive-data-in-the-cloud-with-automated-reasoning-zelkova/">Ze […]*

```diff
@@ -643,15 +643,15 @@
             },
             "name": "UpdateSecretVersionStage",
             "output": {
                 "shape": "UpdateSecretVersionStageResponse"
             }
         },
         "ValidateResourcePolicy": {
-            "documentation": "<p>Validates that a resource policy does not grant a wide range of principals access to your secret. A resource-based policy is optional for secrets.</p> <p>The API performs three checks when validating the policy:</p> <ul> <li> <p>Sends a call to <a href=\"https://aws.amazon.com/blogs/security/protect-sensitive-data-in-the-cloud-with-automated-reasoning-zelkova/\">Zelkova</a>, an automated reasoning engine, to ensure your resource policy does not allow broad access to your secret, for example policies that use a wildcard for the principal.</p> </li> <li> <p>Checks for correct syntax in a policy.</p> </li> <li> <p>Verifies the policy does not lock out a caller.</p> </li> </ul> <p>Secrets Manager generates a CloudTrail log entry when you call this action. Do not include sensitive information in request parameters because it might be logged. For more information, see <a href=\"https://docs.aws.amazon.com/secretsmanager/latest/userguide/retrieve-ct-entries.html\">Logging Secrets Manager events with CloudTrail</a>.</p> <p> <b>Required permissions: </b> <code>secretsmanager:ValidateResourcePolicy</code>. For more information, see <a href=\"https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#reference_iam-permissions_actions\"> IAM policy actions for Secrets Manager</a> and <a href=\"https://docs.aws.amazon.com/secretsmanager/latest/userguide/auth-and-access.html\">Authentication and access control in Secrets Manager</a>. </p>",
+            "documentation": "<p>Validates that a resource policy does not grant a wide range of principals access to your secret. A resource-based policy is optional for secrets.</p> <p>The API performs three checks when validating the policy:</p> <ul> <li> <p>Sends a call to <a href=\"https://aws.amazon.com/blogs/security/protect-sensitive-data-in-the-cloud-with-automated-reasoning-zelkova/\">Zelkova</a>, an automated reasoning engine, to ensure your resource policy does not allow broad access to your secret, for example policies that use a wildcard for the principal.</p> </li> <li> <p>Checks for correct syntax in a policy.</p> </li> <li> <p>Verifies the policy does not lock out a caller.</p> </li> </ul> <p>Secrets Manager generates a CloudTrail log entry when you call this action. Do not include sensitive information in request parameters because it might be logged. For more information, see <a href=\"https://docs.aws.amazon.com/secretsmanager/latest/userguide/retrieve-ct-entries.html\">Logging Secrets Manager events with CloudTrail</a>.</p> <p> <b>Required permissions: </b> <code>secretsmanager:ValidateResourcePolicy</code> and <code>secretsmanager:PutResourcePolicy</code>. For more information, see <a href=\"https://docs.aws.amazon.com/secretsmanager/latest/userguide/reference_iam-permissions.html#reference_iam-permissions_actions\"> IAM policy actions for Secrets Manager</a> and <a href=\"https://docs.aws.amazon.com/secretsmanager/latest/userguide/auth-and-access.html\">Authentication and access control in Secrets Manager</a>. </p>",
             "errors": [
                 {
                     "shape": "MalformedPolicyDocumentException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -740,15 +740,15 @@
                     "shape": "ClientRequestTokenType"
                 },
                 "Description": {
                     "documentation": "<p>The description of the secret.</p>",
                     "shape": "DescriptionType"
                 },
                 "ForceOverwriteReplicaSecret": {
-                    "documentation": "<p>Specifies whether to overwrite a secret with the same name in the destination Region.</p>",
+                    "documentation": "<p>Specifies whether to overwrite a secret with the same name in the destination Region. By default, secrets aren't overwritten.</p>",
                     "shape": "BooleanType"
                 },
                 "KmsKeyId": {
                     "documentation": "<p>The ARN, key ID, or alias of the KMS key that Secrets Manager uses to encrypt the secret value in the secret. An alias is always prefixed by <code>alias/</code>, for example <code>alias/aws/secretsmanager</code>. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/alias-about.html\">About aliases</a>.</p> <p>To use a KMS key in a different account, use the key ARN or the alias ARN.</p> <p>If you don't specify this value, then Secrets Manager uses the key <code>aws/secretsmanager</code>. If that key doesn't yet exist, then Secrets Manager creates it for you automatically the first time it encrypts the secret value.</p> <p>If the secret is in a different Amazon Web Services account from the credentials calling the API, then you can't use <code>aws/secretsmanager</code> to encrypt the secret, and you must create and use a customer managed KMS key. </p>",
                     "shape": "KmsKeyIdType"
                 },
                 "Name": {
@@ -832,20 +832,20 @@
             },
             "type": "structure"
         },
         "DeleteSecretRequest": {
             "members": {
                 "ForceDeleteWithoutRecovery": {
                     "box": true,
-                    "documentation": "<p>Specifies whether to delete the secret without any recovery window. You can't use both this parameter and <code>RecoveryWindowInDays</code> in the same call. If you don't use either, then Secrets Manager defaults to a 30 day recovery window.</p> <p>Secrets Manager performs the actual deletion with an asynchronous background process, so there might be a short delay before the secret is permanently deleted. If you delete a secret and then immediately create a secret with the same name, use appropriate back off and retry logic.</p> <important> <p>Use this parameter with caution. This parameter causes the operation to skip the normal recovery window before the permanent deletion that Secrets Manager would normally impose with the <code>RecoveryWindowInDays</code> parameter. If you delete a secret with the <code>ForceDeleteWithoutRecovery</code> parameter, then you have no opportunity to recover the secret. You lose the secret permanently.</p> </important>",
+                    "documentation": "<p>Specifies whether to delete the secret without any recovery window. You can't use both this parameter and <code>RecoveryWindowInDays</code> in the same call. If you don't use either, then by default Secrets Manager uses a 30 day recovery window.</p> <p>Secrets Manager performs the actual deletion with an asynchronous background process, so there might be a short delay before the secret is permanently deleted. If you delete a secret and then immediately create a secret with the same name, use appropriate back off and retry logic.</p> <p>If you forcibly delete an already deleted or nonexistent secret, the operation does not return <code>ResourceNotFoundException</code>.</p> <important> <p>Use this parameter with caution. This parameter causes the operation to skip the normal recovery window before the permanent deletion that Secrets Manager would normally impose with the <code>RecoveryWindowInDays</code> parameter. If you delete a secret with the <code>ForceDeleteWithoutRecovery</code> parameter, then you have no opportunity to recover the secret. You lose the secret permanently.</p> </important>",
                     "shape": "BooleanType"
                 },
                 "RecoveryWindowInDays": {
                     "box": true,
-                    "documentation": "<p>The number of days from 7 to 30 that Secrets Manager waits before permanently deleting the secret. You can't use both this parameter and <code>ForceDeleteWithoutRecovery</code> in the same call. If you don't use either, then Secrets Manager defaults to a 30 day recovery window.</p>",
+                    "documentation": "<p>The number of days from 7 to 30 that Secrets Manager waits before permanently deleting the secret. You can't use both this parameter and <code>ForceDeleteWithoutRecovery</code> in the same call. If you don't use either, then by default Secrets Manager uses a 30 day recovery window.</p>",
                     "shape": "RecoveryWindowInDaysType"
                 },
                 "SecretId": {
                     "documentation": "<p>The ARN or name of the secret to delete.</p> <p>For an ARN, we recommend that you specify a complete ARN rather than a partial ARN. See <a href=\"https://docs.aws.amazon.com/secretsmanager/latest/userguide/troubleshoot.html#ARN_secretnamehyphen\">Finding a secret from a partial ARN</a>.</p>",
                     "shape": "SecretIdType"
                 }
             },
@@ -930,15 +930,15 @@
                     "shape": "LastRotatedDateType"
                 },
                 "Name": {
                     "documentation": "<p>The name of the secret.</p>",
                     "shape": "SecretNameType"
                 },
                 "NextRotationDate": {
-                    "documentation": "<p>The next date and time that Secrets Manager will rotate the secret, rounded to the nearest hour. If the secret isn't configured for rotation, Secrets Manager returns null.</p>",
+                    "documentation": "<p>The next rotation is scheduled to occur on or before this date. If the secret isn't configured for rotation, Secrets Manager returns null.</p>",
                     "shape": "NextRotationDateType"
                 },
                 "OwningService": {
                     "documentation": "<p>The ID of the service that created this secret. For more information, see <a href=\"https://docs.aws.amazon.com/secretsmanager/latest/userguide/service-linked-secrets.html\">Secrets managed by other Amazon Web Services services</a>.</p>",
                     "shape": "OwningServiceType"
                 },
                 "PrimaryRegion": {
@@ -1269,15 +1269,15 @@
             },
             "type": "structure"
         },
         "ListSecretVersionIdsRequest": {
             "members": {
                 "IncludeDeprecated": {
                     "box": true,
-                    "documentation": "<p>Specifies whether to include versions of secrets that don't have any staging labels attached to them. Versions without staging labels are considered deprecated and are subject to deletion by Secrets Manager.</p>",
+                    "documentation": "<p>Specifies whether to include versions of secrets that don't have any staging labels attached to them. Versions without staging labels are considered deprecated and are subject to deletion by Secrets Manager. By default, versions without staging labels aren't included.</p>",
                     "shape": "BooleanType"
                 },
                 "MaxResults": {
                     "box": true,
                     "documentation": "<p>The number of results to include in the response.</p> <p>If there are more results available, in the response, Secrets Manager includes <code>NextToken</code>. To get the next results, call <code>ListSecretVersionIds</code> again with the value from <code>NextToken</code>. </p>",
                     "shape": "MaxResultsType"
                 },
@@ -1320,15 +1320,15 @@
             "members": {
                 "Filters": {
                     "documentation": "<p>The filters to apply to the list of secrets.</p>",
                     "shape": "FiltersListType"
                 },
                 "IncludePlannedDeletion": {
                     "box": true,
-                    "documentation": "<p>Specifies whether to include secrets scheduled for deletion.</p>",
+                    "documentation": "<p>Specifies whether to include secrets scheduled for deletion. By default, secrets scheduled for deletion aren't included.</p>",
                     "shape": "BooleanType"
                 },
                 "MaxResults": {
                     "box": true,
                     "documentation": "<p>The number of results to include in the response.</p> <p>If there are more results available, in the response, Secrets Manager includes <code>NextToken</code>. To get the next results, call <code>ListSecrets</code> again with the value from <code>NextToken</code>.</p>",
                     "shape": "MaxResultsType"
                 },
@@ -1419,15 +1419,15 @@
             },
             "type": "structure"
         },
         "PutResourcePolicyRequest": {
             "members": {
                 "BlockPublicPolicy": {
                     "box": true,
-                    "documentation": "<p>Specifies whether to block resource-based policies that allow broad access to the secret, for example those that use a wildcard for the principal.</p>",
+                    "documentation": "<p>Specifies whether to block resource-based policies that allow broad access to the secret, for example those that use a wildcard for the principal. By default, public policies aren't blocked.</p>",
                     "shape": "BooleanType"
                 },
                 "ResourcePolicy": {
                     "documentation": "<p>A JSON-formatted string for an Amazon Web Services resource-based policy. For example policies, see <a href=\"https://docs.aws.amazon.com/secretsmanager/latest/userguide/auth-and-access_examples.html\">Permissions policy examples</a>.</p>",
                     "shape": "NonEmptyResourcePolicyType"
                 },
                 "SecretId": {
@@ -1573,15 +1573,15 @@
         "ReplicateSecretToRegionsRequest": {
             "members": {
                 "AddReplicaRegions": {
                     "documentation": "<p>A list of Regions in which to replicate the secret.</p>",
                     "shape": "AddReplicaRegionListType"
                 },
                 "ForceOverwriteReplicaSecret": {
-                    "documentation": "<p>Specifies whether to overwrite a secret with the same name in the destination Region.</p>",
+                    "documentation": "<p>Specifies whether to overwrite a secret with the same name in the destination Region. By default, secrets aren't overwritten.</p>",
                     "shape": "BooleanType"
                 },
                 "SecretId": {
                     "documentation": "<p>The ARN or name of the secret to replicate.</p>",
                     "shape": "SecretIdType"
                 }
             },
@@ -1689,15 +1689,15 @@
                 "ClientRequestToken": {
                     "documentation": "<p>A unique identifier for the new version of the secret that helps ensure idempotency. Secrets Manager uses this value to prevent the accidental creation of duplicate versions if there are failures and retries during rotation. This value becomes the <code>VersionId</code> of the new version.</p> <p>If you use the Amazon Web Services CLI or one of the Amazon Web Services SDK to call this operation, then you can leave this parameter empty. The CLI or SDK generates a random UUID for you and includes that in the request for this parameter. If you don't use the SDK and instead generate a raw HTTP request to the Secrets Manager service endpoint, then you must generate a <code>ClientRequestToken</code> yourself for new versions and include that value in the request.</p> <p>You only need to specify this value if you implement your own retry logic and you want to ensure that Secrets Manager doesn't attempt to create a secret version twice. We recommend that you generate a <a href=\"https://wikipedia.org/wiki/Universally_unique_identifier\">UUID-type</a> value to ensure uniqueness within the specified secret. </p>",
                     "idempotencyToken": true,
                     "shape": "ClientRequestTokenType"
                 },
                 "RotateImmediately": {
                     "box": true,
-                    "documentation": "<p>Specifies whether to rotate the secret immediately or wait until the next scheduled rotation window. The rotation schedule is defined in <a>RotateSecretRequest$RotationRules</a>.</p> <p>For secrets that use a Lambda rotation function to rotate, if you don't immediately rotate the secret, Secrets Manager tests the rotation configuration by running the <a href=\"https://docs.aws.amazon.com/secretsmanager/latest/userguide/rotate-secrets_how.html\"> <code>testSecret</code> step</a> of the Lambda rotation function. The test creates an <code>AWSPENDING</code> version of the secret and then removes it.</p> <p>If you don't specify this value, then by default, Secrets Manager rotates the secret immediately.</p>",
+                    "documentation": "<p>Specifies whether to rotate the secret immediately or wait until the next scheduled rotation window. The rotation schedule is defined in <a>RotateSecretRequest$RotationRules</a>.</p> <p>For secrets that use a Lambda rotation function to rotate, if you don't immediately rotate the secret, Secrets Manager tests the rotation configuration by running the <a href=\"https://docs.aws.amazon.com/secretsmanager/latest/userguide/rotate-secrets_how.html\"> <code>testSecret</code> step</a> of the Lambda rotation function. The test creates an <code>AWSPENDING</code> version of the secret and then removes it.</p> <p>By default, Secrets Manager rotates the secret immediately.</p>",
                     "shape": "BooleanType"
                 },
                 "RotationLambdaARN": {
                     "documentation": "<p>For secrets that use a Lambda rotation function to rotate, the ARN of the Lambda rotation function. </p> <p>For secrets that use <i>managed rotation</i>, omit this field. For more information, see <a href=\"https://docs.aws.amazon.com/secretsmanager/latest/userguide/rotate-secrets_managed.html\">Managed rotation</a> in the <i>Secrets Manager User Guide</i>.</p>",
                     "shape": "RotationLambdaARNType"
                 },
                 "RotationRules": {
@@ -1821,15 +1821,15 @@
                     "shape": "LastRotatedDateType"
                 },
                 "Name": {
                     "documentation": "<p>The friendly name of the secret. You can use forward slashes in the name to represent a path hierarchy. For example, <code>/prod/databases/dbserver1</code> could represent the secret for a server named <code>dbserver1</code> in the folder <code>databases</code> in the folder <code>prod</code>. </p>",
                     "shape": "SecretNameType"
                 },
                 "NextRotationDate": {
-                    "documentation": "<p>The next date and time that Secrets Manager will attempt to rotate the secret, rounded to the nearest hour. This value is null if the secret is not set up for rotation.</p>",
+                    "documentation": "<p>The next rotation is scheduled to occur on or before this date. If the secret isn't configured for rotation, Secrets Manager returns null.</p>",
                     "shape": "NextRotationDateType"
                 },
                 "OwningService": {
                     "documentation": "<p>Returns the name of the service that created the secret.</p>",
                     "shape": "OwningServiceType"
                 },
                 "PrimaryRegion": {
```

### Comparing `botocore-a-la-carte-secretsmanager-1.29.99/botocore_a_la_carte_secretsmanager.egg-info/PKG-INFO` & `botocore-a-la-carte-secretsmanager-1.30.0/botocore_a_la_carte_secretsmanager.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-secretsmanager
-Version: 1.29.99
+Version: 1.30.0
 Summary: secretsmanager data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-secretsmanager-1.29.99/botocore_a_la_carte_secretsmanager.egg-info/SOURCES.txt` & `botocore-a-la-carte-secretsmanager-1.30.0/botocore_a_la_carte_secretsmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-secretsmanager-1.29.99/setup.py` & `botocore-a-la-carte-secretsmanager-1.30.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-secretsmanager',
-    version="1.29.99",
+    version="1.30.0",
     description='secretsmanager data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/secretsmanager/*/*.json'],
```

