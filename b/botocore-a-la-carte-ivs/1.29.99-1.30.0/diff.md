# Comparing `tmp/botocore-a-la-carte-ivs-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-ivs-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ivs-1.29.99.tar", last modified: Sat Mar 25 01:22:45 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-ivs-1.30.0.tar", last modified: Tue Jul  4 01:44:36 2023, max compression
```

## Comparing `botocore-a-la-carte-ivs-1.29.99.tar` & `botocore-a-la-carte-ivs-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:45.735770 botocore-a-la-carte-ivs-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:22:45.000000 botocore-a-la-carte-ivs-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-25 01:22:45.731770 botocore-a-la-carte-ivs-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:45.731770 botocore-a-la-carte-ivs-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:45.731770 botocore-a-la-carte-ivs-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:45.731770 botocore-a-la-carte-ivs-1.29.99/botocore/data/ivs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:45.731770 botocore-a-la-carte-ivs-1.29.99/botocore/data/ivs/2020-07-14/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-03-25 01:22:12.000000 botocore-a-la-carte-ivs-1.29.99/botocore/data/ivs/2020-07-14/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-ivs-1.29.99/botocore/data/ivs/2020-07-14/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-25 01:22:12.000000 botocore-a-la-carte-ivs-1.29.99/botocore/data/ivs/2020-07-14/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    91277 2023-03-25 01:22:12.000000 botocore-a-la-carte-ivs-1.29.99/botocore/data/ivs/2020-07-14/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:22:45.731770 botocore-a-la-carte-ivs-1.29.99/botocore_a_la_carte_ivs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-25 01:22:45.000000 botocore-a-la-carte-ivs-1.29.99/botocore_a_la_carte_ivs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-25 01:22:45.000000 botocore-a-la-carte-ivs-1.29.99/botocore_a_la_carte_ivs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:22:45.000000 botocore-a-la-carte-ivs-1.29.99/botocore_a_la_carte_ivs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:22:45.000000 botocore-a-la-carte-ivs-1.29.99/botocore_a_la_carte_ivs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:22:45.735770 botocore-a-la-carte-ivs-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-25 01:22:45.000000 botocore-a-la-carte-ivs-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:36.538610 botocore-a-la-carte-ivs-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:36.000000 botocore-a-la-carte-ivs-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:44:36.538610 botocore-a-la-carte-ivs-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:36.538610 botocore-a-la-carte-ivs-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:36.538610 botocore-a-la-carte-ivs-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:36.538610 botocore-a-la-carte-ivs-1.30.0/botocore/data/ivs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:36.538610 botocore-a-la-carte-ivs-1.30.0/botocore/data/ivs/2020-07-14/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-04 01:44:02.000000 botocore-a-la-carte-ivs-1.30.0/botocore/data/ivs/2020-07-14/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-ivs-1.30.0/botocore/data/ivs/2020-07-14/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-04 01:44:02.000000 botocore-a-la-carte-ivs-1.30.0/botocore/data/ivs/2020-07-14/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   109098 2023-07-04 01:44:02.000000 botocore-a-la-carte-ivs-1.30.0/botocore/data/ivs/2020-07-14/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:36.538610 botocore-a-la-carte-ivs-1.30.0/botocore_a_la_carte_ivs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:44:36.000000 botocore-a-la-carte-ivs-1.30.0/botocore_a_la_carte_ivs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-04 01:44:36.000000 botocore-a-la-carte-ivs-1.30.0/botocore_a_la_carte_ivs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:36.000000 botocore-a-la-carte-ivs-1.30.0/botocore_a_la_carte_ivs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:36.000000 botocore-a-la-carte-ivs-1.30.0/botocore_a_la_carte_ivs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:36.538610 botocore-a-la-carte-ivs-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-04 01:44:36.000000 botocore-a-la-carte-ivs-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-ivs-1.29.99/LICENSE.txt` & `botocore-a-la-carte-ivs-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ivs-1.29.99/PKG-INFO` & `botocore-a-la-carte-ivs-1.30.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ivs
-Version: 1.29.99
+Version: 1.30.0
 Summary: ivs data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ivs-1.29.99/botocore/data/ivs/2020-07-14/endpoint-rule-set-1.json` & `botocore-a-la-carte-ivs-1.30.0/botocore/data/ivs/2020-07-14/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ivs-1.29.99/botocore/data/ivs/2020-07-14/paginators-1.json` & `botocore-a-la-carte-ivs-1.30.0/botocore/data/ivs/2020-07-14/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ivs-1.29.99/botocore/data/ivs/2020-07-14/service-2.json` & `botocore-a-la-carte-ivs-1.30.0/botocore/data/ivs/2020-07-14/service-2.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8850295854864875%*

 * *Differences: {"'documentation'": "'<p> <b>Introduction</b> </p> <p>The Amazon Interactive Video Service (IVS) "*

 * *                    'API is REST compatible, using a standard HTTP API and an Amazon Web Services '*

 * *                    'EventBridge event stream for responses. JSON is used for both requests and '*

 * *                    'responses, including errors.</p> <p>The API is an Amazon Web Services '*

 * *                    'regional service. For a list of supported regions and Amazon IVS HTTPS '*

 * *                    'service […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "documentation": "<p> <b>Introduction</b> </p> <p>The Amazon Interactive Video Service (IVS) API is REST compatible, using a standard HTTP API and an Amazon Web Services EventBridge event stream for responses. JSON is used for both requests and responses, including errors.</p> <p>The API is an Amazon Web Services regional service. For a list of supported regions and Amazon IVS HTTPS service endpoints, see the <a href=\"https://docs.aws.amazon.com/general/latest/gr/ivs.html\">Amazon IVS page</a> in the <i>Amazon Web Services General Reference</i>.</p> <p> <i> <b>All API request parameters and URLs are case sensitive. </b> </i> </p> <p>For a summary of notable documentation changes in each release, see <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/doc-history.html\"> Document History</a>.</p> <p> <b>Allowed Header Values</b> </p> <ul> <li> <p> <code> <b>Accept:</b> </code> application/json</p> </li> <li> <p> <code> <b>Accept-Encoding:</b> </code> gzip, deflate</p> </li> <li> <p> <code> <b>Content-Type:</b> </code>application/json</p> </li> </ul> <p> <b>Resources</b> </p> <p>The following resources contain information about your IVS live stream (see <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/getting-started.html\"> Getting Started with Amazon IVS</a>):</p> <ul> <li> <p>Channel \u2014 Stores configuration data related to your live stream. You first create a channel and then use the channel\u2019s stream key to start your live stream. See the Channel endpoints for more information. </p> </li> <li> <p>Stream key \u2014 An identifier assigned by Amazon IVS when you create a channel, which is then used to authorize streaming. See the StreamKey endpoints for more information. <i> <b>Treat the stream key like a secret, since it allows anyone to stream to the channel.</b> </i> </p> </li> <li> <p>Playback key pair \u2014 Video playback may be restricted using playback-authorization tokens, which use public-key encryption. A playback key pair is the public-private pair of keys used to sign and validate the playback-authorization token. See the PlaybackKeyPair endpoints for more information.</p> </li> <li> <p>Recording configuration \u2014 Stores configuration related to recording a live stream and where to store the recorded content. Multiple channels can reference the same recording configuration. See the Recording Configuration endpoints for more information.</p> </li> </ul> <p> <b>Tagging</b> </p> <p>A <i>tag</i> is a metadata label that you assign to an Amazon Web Services resource. A tag comprises a <i>key</i> and a <i>value</i>, both set by you. For example, you might set a tag as <code>topic:nature</code> to label a particular video category. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p> <p>Tags can help you identify and organize your Amazon Web Services resources. For example, you can use the same tag for different resources to indicate that they are related. You can also use tags to manage access (see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_tags.html\"> Access Tags</a>). </p> <p>The Amazon IVS API has these tag-related endpoints: <a>TagResource</a>, <a>UntagResource</a>, and <a>ListTagsForResource</a>. The following resources support tagging: Channels, Stream Keys, Playback Key Pairs, and Recording Configurations.</p> <p>At most 50 tags can be applied to a resource. </p> <p> <b>Authentication versus Authorization</b> </p> <p>Note the differences between these concepts:</p> <ul> <li> <p> <i>Authentication</i> is about verifying identity. You need to be authenticated to sign Amazon IVS API requests.</p> </li> <li> <p> <i>Authorization</i> is about granting permissions. Your IAM roles need to have permissions for Amazon IVS API requests. In addition, authorization is needed to view <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/private-channels.html\">Amazon IVS private channels</a>. (Private channels are channels that are enabled for \"playback authorization.\")</p> </li> </ul> <p> <b>Authentication</b> </p> <p>All Amazon IVS API requests must be authenticated with a signature. The Amazon Web Services Command-Line Interface (CLI) and Amazon IVS Player SDKs take care of signing the underlying API calls for you. However, if your application calls the Amazon IVS API directly, it\u2019s your responsibility to sign the requests.</p> <p>You generate a signature using valid Amazon Web Services credentials that have permission to perform the requested action. For example, you must sign PutMetadata requests with a signature generated from a user account that has the <code>ivs:PutMetadata</code> permission.</p> <p>For more information:</p> <ul> <li> <p>Authentication and generating signatures \u2014 See <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/sig-v4-authenticating-requests.html\">Authenticating Requests (Amazon Web Services Signature Version 4)</a> in the <i>Amazon Web Services General Reference</i>.</p> </li> <li> <p>Managing Amazon IVS permissions \u2014 See <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/security-iam.html\">Identity and Access Management</a> on the Security page of the <i>Amazon IVS User Guide</i>.</p> </li> </ul> <p> <b>Amazon Resource Names (ARNs)</b> </p> <p>ARNs uniquely identify AWS resources. An ARN is required when you need to specify a resource unambiguously across all of AWS, such as in IAM policies and API calls. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\">Amazon Resource Names</a> in the <i>AWS General Reference</i>.</p> <p> <b>Channel Endpoints</b> </p> <ul> <li> <p> <a>CreateChannel</a> \u2014 Creates a new channel and an associated stream key to start streaming.</p> </li> <li> <p> <a>GetChannel</a> \u2014 Gets the channel configuration for the specified channel ARN.</p> </li> <li> <p> <a>BatchGetChannel</a> \u2014 Performs <a>GetChannel</a> on multiple ARNs simultaneously.</p> </li> <li> <p> <a>ListChannels</a> \u2014 Gets summary information about all channels in your account, in the Amazon Web Services region where the API request is processed. This list can be filtered to match a specified name or recording-configuration ARN. Filters are mutually exclusive and cannot be used together. If you try to use both filters, you will get an error (409 Conflict Exception).</p> </li> <li> <p> <a>UpdateChannel</a> \u2014 Updates a channel's configuration. This does not affect an ongoing stream of this channel. You must stop and restart the stream for the changes to take effect.</p> </li> <li> <p> <a>DeleteChannel</a> \u2014 Deletes the specified channel.</p> </li> </ul> <p> <b>StreamKey Endpoints</b> </p> <ul> <li> <p> <a>CreateStreamKey</a> \u2014 Creates a stream key, used to initiate a stream, for the specified channel ARN.</p> </li> <li> <p> <a>GetStreamKey</a> \u2014 Gets stream key information for the specified ARN.</p> </li> <li> <p> <a>BatchGetStreamKey</a> \u2014 Performs <a>GetStreamKey</a> on multiple ARNs simultaneously.</p> </li> <li> <p> <a>ListStreamKeys</a> \u2014 Gets summary information about stream keys for the specified channel.</p> </li> <li> <p> <a>DeleteStreamKey</a> \u2014 Deletes the stream key for the specified ARN, so it can no longer be used to stream.</p> </li> </ul> <p> <b>Stream Endpoints</b> </p> <ul> <li> <p> <a>GetStream</a> \u2014 Gets information about the active (live) stream on a specified channel.</p> </li> <li> <p> <a>GetStreamSession</a> \u2014 Gets metadata on a specified stream.</p> </li> <li> <p> <a>ListStreams</a> \u2014 Gets summary information about live streams in your account, in the Amazon Web Services region where the API request is processed.</p> </li> <li> <p> <a>ListStreamSessions</a> \u2014 Gets a summary of current and previous streams for a specified channel in your account, in the AWS region where the API request is processed.</p> </li> <li> <p> <a>StopStream</a> \u2014 Disconnects the incoming RTMPS stream for the specified channel. Can be used in conjunction with <a>DeleteStreamKey</a> to prevent further streaming to a channel.</p> </li> <li> <p> <a>PutMetadata</a> \u2014 Inserts metadata into the active stream of the specified channel. At most 5 requests per second per channel are allowed, each with a maximum 1 KB payload. (If 5 TPS is not sufficient for your needs, we recommend batching your data into a single PutMetadata call.) At most 155 requests per second per account are allowed.</p> </li> </ul> <p> <b>PlaybackKeyPair Endpoints</b> </p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/private-channels.html\">Setting Up Private Channels</a> in the <i>Amazon IVS User Guide</i>.</p> <ul> <li> <p> <a>ImportPlaybackKeyPair</a> \u2014 Imports the public portion of a new key pair and returns its <code>arn</code> and <code>fingerprint</code>. The <code>privateKey</code> can then be used to generate viewer authorization tokens, to grant viewers access to private channels (channels enabled for playback authorization).</p> </li> <li> <p> <a>GetPlaybackKeyPair</a> \u2014 Gets a specified playback authorization key pair and returns the <code>arn</code> and <code>fingerprint</code>. The <code>privateKey</code> held by the caller can be used to generate viewer authorization tokens, to grant viewers access to private channels.</p> </li> <li> <p> <a>ListPlaybackKeyPairs</a> \u2014 Gets summary information about playback key pairs.</p> </li> <li> <p> <a>DeletePlaybackKeyPair</a> \u2014 Deletes a specified authorization key pair. This invalidates future viewer tokens generated using the key pair\u2019s <code>privateKey</code>.</p> </li> </ul> <p> <b>RecordingConfiguration Endpoints</b> </p> <ul> <li> <p> <a>CreateRecordingConfiguration</a> \u2014 Creates a new recording configuration, used to enable recording to Amazon S3.</p> </li> <li> <p> <a>GetRecordingConfiguration</a> \u2014 Gets the recording-configuration metadata for the specified ARN.</p> </li> <li> <p> <a>ListRecordingConfigurations</a> \u2014 Gets summary information about all recording configurations in your account, in the Amazon Web Services region where the API request is processed.</p> </li> <li> <p> <a>DeleteRecordingConfiguration</a> \u2014 Deletes the recording configuration for the specified ARN.</p> </li> </ul> <p> <b>Amazon Web Services Tags Endpoints</b> </p> <ul> <li> <p> <a>TagResource</a> \u2014 Adds or updates tags for the Amazon Web Services resource with the specified ARN.</p> </li> <li> <p> <a>UntagResource</a> \u2014 Removes tags from the resource with the specified ARN.</p> </li> <li> <p> <a>ListTagsForResource</a> \u2014 Gets information about Amazon Web Services tags for the specified ARN.</p> </li> </ul>",
+    "documentation": "<p> <b>Introduction</b> </p> <p>The Amazon Interactive Video Service (IVS) API is REST compatible, using a standard HTTP API and an Amazon Web Services EventBridge event stream for responses. JSON is used for both requests and responses, including errors.</p> <p>The API is an Amazon Web Services regional service. For a list of supported regions and Amazon IVS HTTPS service endpoints, see the <a href=\"https://docs.aws.amazon.com/general/latest/gr/ivs.html\">Amazon IVS page</a> in the <i>Amazon Web Services General Reference</i>.</p> <p> <i> <b>All API request parameters and URLs are case sensitive. </b> </i> </p> <p>For a summary of notable documentation changes in each release, see <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/doc-history.html\"> Document History</a>.</p> <p> <b>Allowed Header Values</b> </p> <ul> <li> <p> <code> <b>Accept:</b> </code> application/json</p> </li> <li> <p> <code> <b>Accept-Encoding:</b> </code> gzip, deflate</p> </li> <li> <p> <code> <b>Content-Type:</b> </code>application/json</p> </li> </ul> <p> <b>Resources</b> </p> <p>The following resources contain information about your IVS live stream (see <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/getting-started.html\"> Getting Started with Amazon IVS</a>):</p> <ul> <li> <p> <b>Channel</b> \u2014 Stores configuration data related to your live stream. You first create a channel and then use the channel\u2019s stream key to start your live stream. See the Channel endpoints for more information. </p> </li> <li> <p> <b>Stream key</b> \u2014 An identifier assigned by Amazon IVS when you create a channel, which is then used to authorize streaming. See the StreamKey endpoints for more information. <i> <b>Treat the stream key like a secret, since it allows anyone to stream to the channel.</b> </i> </p> </li> <li> <p> <b>Playback key pair</b> \u2014 Video playback may be restricted using playback-authorization tokens, which use public-key encryption. A playback key pair is the public-private pair of keys used to sign and validate the playback-authorization token. See the PlaybackKeyPair endpoints for more information.</p> </li> <li> <p> <b>Recording configuration</b> \u2014 Stores configuration related to recording a live stream and where to store the recorded content. Multiple channels can reference the same recording configuration. See the Recording Configuration endpoints for more information.</p> </li> </ul> <p> <b>Tagging</b> </p> <p>A <i>tag</i> is a metadata label that you assign to an Amazon Web Services resource. A tag comprises a <i>key</i> and a <i>value</i>, both set by you. For example, you might set a tag as <code>topic:nature</code> to label a particular video category. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p> <p>Tags can help you identify and organize your Amazon Web Services resources. For example, you can use the same tag for different resources to indicate that they are related. You can also use tags to manage access (see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_tags.html\"> Access Tags</a>). </p> <p>The Amazon IVS API has these tag-related endpoints: <a>TagResource</a>, <a>UntagResource</a>, and <a>ListTagsForResource</a>. The following resources support tagging: Channels, Stream Keys, Playback Key Pairs, and Recording Configurations.</p> <p>At most 50 tags can be applied to a resource. </p> <p> <b>Authentication versus Authorization</b> </p> <p>Note the differences between these concepts:</p> <ul> <li> <p> <i>Authentication</i> is about verifying identity. You need to be authenticated to sign Amazon IVS API requests.</p> </li> <li> <p> <i>Authorization</i> is about granting permissions. Your IAM roles need to have permissions for Amazon IVS API requests. In addition, authorization is needed to view <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/private-channels.html\">Amazon IVS private channels</a>. (Private channels are channels that are enabled for \"playback authorization.\")</p> </li> </ul> <p> <b>Authentication</b> </p> <p>All Amazon IVS API requests must be authenticated with a signature. The Amazon Web Services Command-Line Interface (CLI) and Amazon IVS Player SDKs take care of signing the underlying API calls for you. However, if your application calls the Amazon IVS API directly, it\u2019s your responsibility to sign the requests.</p> <p>You generate a signature using valid Amazon Web Services credentials that have permission to perform the requested action. For example, you must sign PutMetadata requests with a signature generated from a user account that has the <code>ivs:PutMetadata</code> permission.</p> <p>For more information:</p> <ul> <li> <p>Authentication and generating signatures \u2014 See <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/sig-v4-authenticating-requests.html\">Authenticating Requests (Amazon Web Services Signature Version 4)</a> in the <i>Amazon Web Services General Reference</i>.</p> </li> <li> <p>Managing Amazon IVS permissions \u2014 See <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/security-iam.html\">Identity and Access Management</a> on the Security page of the <i>Amazon IVS User Guide</i>.</p> </li> </ul> <p> <b>Amazon Resource Names (ARNs)</b> </p> <p>ARNs uniquely identify AWS resources. An ARN is required when you need to specify a resource unambiguously across all of AWS, such as in IAM policies and API calls. For more information, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\">Amazon Resource Names</a> in the <i>AWS General Reference</i>.</p> <p> <b>Channel Endpoints</b> </p> <ul> <li> <p> <a>CreateChannel</a> \u2014 Creates a new channel and an associated stream key to start streaming.</p> </li> <li> <p> <a>GetChannel</a> \u2014 Gets the channel configuration for the specified channel ARN.</p> </li> <li> <p> <a>BatchGetChannel</a> \u2014 Performs <a>GetChannel</a> on multiple ARNs simultaneously.</p> </li> <li> <p> <a>ListChannels</a> \u2014 Gets summary information about all channels in your account, in the Amazon Web Services region where the API request is processed. This list can be filtered to match a specified name or recording-configuration ARN. Filters are mutually exclusive and cannot be used together. If you try to use both filters, you will get an error (409 Conflict Exception).</p> </li> <li> <p> <a>UpdateChannel</a> \u2014 Updates a channel's configuration. This does not affect an ongoing stream of this channel. You must stop and restart the stream for the changes to take effect.</p> </li> <li> <p> <a>DeleteChannel</a> \u2014 Deletes the specified channel.</p> </li> </ul> <p> <b>StreamKey Endpoints</b> </p> <ul> <li> <p> <a>CreateStreamKey</a> \u2014 Creates a stream key, used to initiate a stream, for the specified channel ARN.</p> </li> <li> <p> <a>GetStreamKey</a> \u2014 Gets stream key information for the specified ARN.</p> </li> <li> <p> <a>BatchGetStreamKey</a> \u2014 Performs <a>GetStreamKey</a> on multiple ARNs simultaneously.</p> </li> <li> <p> <a>ListStreamKeys</a> \u2014 Gets summary information about stream keys for the specified channel.</p> </li> <li> <p> <a>DeleteStreamKey</a> \u2014 Deletes the stream key for the specified ARN, so it can no longer be used to stream.</p> </li> </ul> <p> <b>Stream Endpoints</b> </p> <ul> <li> <p> <a>GetStream</a> \u2014 Gets information about the active (live) stream on a specified channel.</p> </li> <li> <p> <a>GetStreamSession</a> \u2014 Gets metadata on a specified stream.</p> </li> <li> <p> <a>ListStreams</a> \u2014 Gets summary information about live streams in your account, in the Amazon Web Services region where the API request is processed.</p> </li> <li> <p> <a>ListStreamSessions</a> \u2014 Gets a summary of current and previous streams for a specified channel in your account, in the AWS region where the API request is processed.</p> </li> <li> <p> <a>StopStream</a> \u2014 Disconnects the incoming RTMPS stream for the specified channel. Can be used in conjunction with <a>DeleteStreamKey</a> to prevent further streaming to a channel.</p> </li> <li> <p> <a>PutMetadata</a> \u2014 Inserts metadata into the active stream of the specified channel. At most 5 requests per second per channel are allowed, each with a maximum 1 KB payload. (If 5 TPS is not sufficient for your needs, we recommend batching your data into a single PutMetadata call.) At most 155 requests per second per account are allowed.</p> </li> </ul> <p> <b>Private Channel Endpoints</b> </p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/private-channels.html\">Setting Up Private Channels</a> in the <i>Amazon IVS User Guide</i>.</p> <ul> <li> <p> <a>ImportPlaybackKeyPair</a> \u2014 Imports the public portion of a new key pair and returns its <code>arn</code> and <code>fingerprint</code>. The <code>privateKey</code> can then be used to generate viewer authorization tokens, to grant viewers access to private channels (channels enabled for playback authorization).</p> </li> <li> <p> <a>GetPlaybackKeyPair</a> \u2014 Gets a specified playback authorization key pair and returns the <code>arn</code> and <code>fingerprint</code>. The <code>privateKey</code> held by the caller can be used to generate viewer authorization tokens, to grant viewers access to private channels.</p> </li> <li> <p> <a>ListPlaybackKeyPairs</a> \u2014 Gets summary information about playback key pairs.</p> </li> <li> <p> <a>DeletePlaybackKeyPair</a> \u2014 Deletes a specified authorization key pair. This invalidates future viewer tokens generated using the key pair\u2019s <code>privateKey</code>.</p> </li> <li> <p> <a>StartViewerSessionRevocation</a> \u2014 Starts the process of revoking the viewer session associated with a specified channel ARN and viewer ID. Optionally, you can provide a version to revoke viewer sessions less than and including that version.</p> </li> <li> <p> <a>BatchStartViewerSessionRevocation</a> \u2014 Performs <a>StartViewerSessionRevocation</a> on multiple channel ARN and viewer ID pairs simultaneously.</p> </li> </ul> <p> <b>RecordingConfiguration Endpoints</b> </p> <ul> <li> <p> <a>CreateRecordingConfiguration</a> \u2014 Creates a new recording configuration, used to enable recording to Amazon S3.</p> </li> <li> <p> <a>GetRecordingConfiguration</a> \u2014 Gets the recording-configuration metadata for the specified ARN.</p> </li> <li> <p> <a>ListRecordingConfigurations</a> \u2014 Gets summary information about all recording configurations in your account, in the Amazon Web Services region where the API request is processed.</p> </li> <li> <p> <a>DeleteRecordingConfiguration</a> \u2014 Deletes the recording configuration for the specified ARN.</p> </li> </ul> <p> <b>Amazon Web Services Tags Endpoints</b> </p> <ul> <li> <p> <a>TagResource</a> \u2014 Adds or updates tags for the Amazon Web Services resource with the specified ARN.</p> </li> <li> <p> <a>UntagResource</a> \u2014 Removes tags from the resource with the specified ARN.</p> </li> <li> <p> <a>ListTagsForResource</a> \u2014 Gets information about Amazon Web Services tags for the specified ARN.</p> </li> </ul>",
     "metadata": {
         "apiVersion": "2020-07-14",
         "endpointPrefix": "ivs",
         "jsonVersion": "1.1",
         "protocol": "rest-json",
         "serviceAbbreviation": "Amazon IVS",
         "serviceFullName": "Amazon Interactive Video Service",
@@ -39,14 +39,34 @@
                 "shape": "BatchGetStreamKeyRequest"
             },
             "name": "BatchGetStreamKey",
             "output": {
                 "shape": "BatchGetStreamKeyResponse"
             }
         },
+        "BatchStartViewerSessionRevocation": {
+            "documentation": "<p>Performs <a>StartViewerSessionRevocation</a> on multiple channel ARN and viewer ID pairs simultaneously.</p>",
+            "errors": [
+                {
+                    "shape": "ValidationException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/BatchStartViewerSessionRevocation",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "BatchStartViewerSessionRevocationRequest"
+            },
+            "name": "BatchStartViewerSessionRevocation",
+            "output": {
+                "shape": "BatchStartViewerSessionRevocationResponse"
+            }
+        },
         "CreateChannel": {
             "documentation": "<p>Creates a new channel and an associated stream key to start streaming.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -218,15 +238,15 @@
                 {
                     "shape": "ConflictException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/DeleteRecordingConfiguration",
-                "responseCode": 200
+                "responseCode": 204
             },
             "input": {
                 "shape": "DeleteRecordingConfigurationRequest"
             },
             "name": "DeleteRecordingConfiguration"
         },
         "DeleteStreamKey": {
@@ -643,21 +663,50 @@
                 {
                     "shape": "ThrottlingException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/PutMetadata",
-                "responseCode": 200
+                "responseCode": 204
             },
             "input": {
                 "shape": "PutMetadataRequest"
             },
             "name": "PutMetadata"
         },
+        "StartViewerSessionRevocation": {
+            "documentation": "<p>Starts the process of revoking the viewer session associated with a specified channel ARN and viewer ID. Optionally, you can provide a version to revoke viewer sessions less than and including that version. For instructions on associating a viewer ID with a viewer session, see <a href=\"https://docs.aws.amazon.com/ivs/latest/userguide/private-channels.html\">Setting Up Private Channels</a>.</p>",
+            "errors": [
+                {
+                    "shape": "InternalServerException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/StartViewerSessionRevocation",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "StartViewerSessionRevocationRequest"
+            },
+            "name": "StartViewerSessionRevocation",
+            "output": {
+                "shape": "StartViewerSessionRevocationResponse"
+            }
+        },
         "StopStream": {
             "documentation": "<p>Disconnects the incoming RTMPS stream for the specified channel. Can be used in conjunction with <a>DeleteStreamKey</a> to prevent further streaming to a channel.</p> <note> <p>Many streaming client-software libraries automatically reconnect a dropped RTMPS session, so to stop the stream permanently, you may want to first revoke the <code>streamKey</code> attached to the channel.</p> </note>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
@@ -736,15 +785,15 @@
             },
             "name": "UntagResource",
             "output": {
                 "shape": "UntagResourceResponse"
             }
         },
         "UpdateChannel": {
-            "documentation": "<p>Updates a channel's configuration. This does not affect an ongoing stream of this channel. You must stop and restart the stream for the changes to take effect.</p>",
+            "documentation": "<p>Updates a channel's configuration. Live channels cannot be updated. You must stop the ongoing stream, update the channel, and restart the stream for the changes to take effect.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "AccessDeniedException"
                 },
@@ -880,14 +929,97 @@
                 "streamKeys": {
                     "documentation": "<p/>",
                     "shape": "StreamKeys"
                 }
             },
             "type": "structure"
         },
+        "BatchStartViewerSessionRevocationError": {
+            "documentation": "<p>Error for a request in the batch for BatchStartViewerSessionRevocation. Each error is related to a specific channel-ARN and viewer-ID pair.</p>",
+            "members": {
+                "channelArn": {
+                    "documentation": "<p>Channel ARN.</p>",
+                    "shape": "ChannelArn"
+                },
+                "code": {
+                    "documentation": "<p>Error code.</p>",
+                    "shape": "errorCode"
+                },
+                "message": {
+                    "documentation": "<p>Error message, determined by the application.</p>",
+                    "shape": "errorMessage"
+                },
+                "viewerId": {
+                    "documentation": "<p>The ID of the viewer session to revoke.</p>",
+                    "shape": "ViewerId"
+                }
+            },
+            "required": [
+                "channelArn",
+                "viewerId"
+            ],
+            "type": "structure"
+        },
+        "BatchStartViewerSessionRevocationErrors": {
+            "member": {
+                "shape": "BatchStartViewerSessionRevocationError"
+            },
+            "type": "list"
+        },
+        "BatchStartViewerSessionRevocationRequest": {
+            "members": {
+                "viewerSessions": {
+                    "documentation": "<p>Array of viewer sessions, one per channel-ARN and viewer-ID pair.</p>",
+                    "shape": "BatchStartViewerSessionRevocationViewerSessionList"
+                }
+            },
+            "required": [
+                "viewerSessions"
+            ],
+            "type": "structure"
+        },
+        "BatchStartViewerSessionRevocationResponse": {
+            "members": {
+                "errors": {
+                    "documentation": "<p>Each error object is related to a specific <code>channelArn</code> and <code>viewerId</code> pair in the request.</p>",
+                    "shape": "BatchStartViewerSessionRevocationErrors"
+                }
+            },
+            "type": "structure"
+        },
+        "BatchStartViewerSessionRevocationViewerSession": {
+            "documentation": "<p>A viewer session to revoke in the call to <a>BatchStartViewerSessionRevocation</a>.</p>",
+            "members": {
+                "channelArn": {
+                    "documentation": "<p>The ARN of the channel associated with the viewer session to revoke.</p>",
+                    "shape": "ChannelArn"
+                },
+                "viewerId": {
+                    "documentation": "<p>The ID of the viewer associated with the viewer session to revoke. Do not use this field for personally identifying, confidential, or sensitive information.</p>",
+                    "shape": "ViewerId"
+                },
+                "viewerSessionVersionsLessThanOrEqualTo": {
+                    "documentation": "<p>An optional filter on which versions of the viewer session to revoke. All versions less than or equal to the specified version will be revoked. Default: 0.</p>",
+                    "shape": "ViewerSessionVersion"
+                }
+            },
+            "required": [
+                "channelArn",
+                "viewerId"
+            ],
+            "type": "structure"
+        },
+        "BatchStartViewerSessionRevocationViewerSessionList": {
+            "max": 20,
+            "member": {
+                "shape": "BatchStartViewerSessionRevocationViewerSession"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "Boolean": {
             "type": "boolean"
         },
         "Channel": {
             "documentation": "<p>Object specifying a channel.</p>",
             "members": {
                 "arn": {
@@ -898,36 +1030,44 @@
                     "documentation": "<p>Whether the channel is private (enabled for playback authorization). Default: <code>false</code>.</p>",
                     "shape": "IsAuthorized"
                 },
                 "ingestEndpoint": {
                     "documentation": "<p>Channel ingest endpoint, part of the definition of an ingest server, used when you set up streaming software.</p>",
                     "shape": "IngestEndpoint"
                 },
+                "insecureIngest": {
+                    "documentation": "<p>Whether the channel allows insecure RTMP ingest. Default: <code>false</code>.</p>",
+                    "shape": "InsecureIngest"
+                },
                 "latencyMode": {
                     "documentation": "<p>Channel latency mode. Use <code>NORMAL</code> to broadcast and deliver live video up to Full HD. Use <code>LOW</code> for near-real-time interaction with viewers. Default: <code>LOW</code>. (Note: In the Amazon IVS console, <code>LOW</code> and <code>NORMAL</code> correspond to Ultra-low and Standard, respectively.)</p>",
                     "shape": "ChannelLatencyMode"
                 },
                 "name": {
                     "documentation": "<p>Channel name.</p>",
                     "shape": "ChannelName"
                 },
                 "playbackUrl": {
                     "documentation": "<p>Channel playback URL.</p>",
                     "shape": "PlaybackURL"
                 },
+                "preset": {
+                    "documentation": "<p>Optional transcode preset for the channel. This is selectable only for <code>ADVANCED_HD</code> and <code>ADVANCED_SD</code> channel types. For those channel types, the default <code>preset</code> is <code>HIGHER_BANDWIDTH_DELIVERY</code>. For other channel types (<code>BASIC</code> and <code>STANDARD</code>), <code>preset</code> is the empty string (<code>\"\"</code>).</p>",
+                    "shape": "TranscodePreset"
+                },
                 "recordingConfigurationArn": {
                     "documentation": "<p>Recording-configuration ARN. A value other than an empty string indicates that recording is enabled. Default: \"\" (empty string, recording is disabled).</p>",
                     "shape": "ChannelRecordingConfigurationArn"
                 },
                 "tags": {
                     "documentation": "<p>Tags attached to the resource. Array of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p>",
                     "shape": "Tags"
                 },
                 "type": {
-                    "documentation": "<p>Channel type, which determines the allowable resolution and bitrate. <i>If you exceed the allowable resolution or bitrate, the stream probably will disconnect immediately.</i> Default: <code>STANDARD</code>. Valid values:</p> <ul> <li> <p> <code>STANDARD</code>: Video is transcoded: multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Transcoding allows higher playback quality across a range of download speeds. Resolution can be up to 1080p and bitrate can be up to 8.5 Mbps. Audio is transcoded only for renditions 360p and below; above that, audio is passed through. This is the default.</p> </li> <li> <p> <code>BASIC</code>: Video is transmuxed: Amazon IVS delivers the original input to viewers. The viewer\u2019s video-quality choice is limited to the original input. Resolution can be up to 1080p and bitrate can be up to 1.5 Mbps for 480p and up to 3.5 Mbps for resolutions between 480p and 1080p.</p> </li> </ul>",
+                    "documentation": "<p>Channel type, which determines the allowable resolution and bitrate. <i>If you exceed the allowable input resolution or bitrate, the stream probably will disconnect immediately.</i> Some types generate multiple qualities (renditions) from the original input; this automatically gives viewers the best experience for their devices and network conditions. Some types provide transcoded video; transcoding allows higher playback quality across a range of download speeds. Default: <code>STANDARD</code>. Valid values:</p> <ul> <li> <p> <code>BASIC</code>: Video is transmuxed: Amazon IVS delivers the original input quality to viewers. The viewer\u2019s video-quality choice is limited to the original input. Input resolution can be up to 1080p and bitrate can be up to 1.5 Mbps for 480p and up to 3.5 Mbps for resolutions between 480p and 1080p. Original audio is passed through.</p> </li> <li> <p> <code>STANDARD</code>: Video is transcoded: multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Transcoding allows higher playback quality across a range of download speeds. Resolution can be up to 1080p and bitrate can be up to 8.5 Mbps. Audio is transcoded only for renditions 360p and below; above that, audio is passed through. This is the default when you create a channel.</p> </li> <li> <p> <code>ADVANCED_SD</code>: Video is transcoded; multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Input resolution can be up to 1080p and bitrate can be up to 8.5 Mbps; output is capped at SD quality (480p). You can select an optional transcode preset (see below). Audio for all renditions is transcoded, and an audio-only rendition is available.</p> </li> <li> <p> <code>ADVANCED_HD</code>: Video is transcoded; multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Input resolution can be up to 1080p and bitrate can be up to 8.5 Mbps; output is capped at HD quality (720p). You can select an optional transcode preset (see below). Audio for all renditions is transcoded, and an audio-only rendition is available.</p> </li> </ul> <p>Optional <i>transcode presets</i> (available for the <code>ADVANCED</code> types) allow you to trade off available download bandwidth and video quality, to optimize the viewing experience. There are two presets:</p> <ul> <li> <p> <i>Constrained bandwidth delivery</i> uses a lower bitrate for each quality level. Use it if you have low download bandwidth and/or simple video content (e.g., talking heads)</p> </li> <li> <p> <i>Higher bandwidth delivery</i> uses a higher bitrate for each quality level. Use it if you have high download bandwidth and/or complex video content (e.g., flashes and quick scene changes).</p> </li> </ul>",
                     "shape": "ChannelType"
                 }
             },
             "type": "structure"
         },
         "ChannelArn": {
             "max": 128,
@@ -990,37 +1130,51 @@
                     "documentation": "<p>Channel ARN.</p>",
                     "shape": "ChannelArn"
                 },
                 "authorized": {
                     "documentation": "<p>Whether the channel is private (enabled for playback authorization). Default: <code>false</code>.</p>",
                     "shape": "IsAuthorized"
                 },
+                "insecureIngest": {
+                    "documentation": "<p>Whether the channel allows insecure RTMP ingest. Default: <code>false</code>.</p>",
+                    "shape": "InsecureIngest"
+                },
                 "latencyMode": {
                     "documentation": "<p>Channel latency mode. Use <code>NORMAL</code> to broadcast and deliver live video up to Full HD. Use <code>LOW</code> for near-real-time interaction with viewers. Default: <code>LOW</code>. (Note: In the Amazon IVS console, <code>LOW</code> and <code>NORMAL</code> correspond to Ultra-low and Standard, respectively.)</p>",
                     "shape": "ChannelLatencyMode"
                 },
                 "name": {
                     "documentation": "<p>Channel name.</p>",
                     "shape": "ChannelName"
                 },
+                "preset": {
+                    "documentation": "<p>Optional transcode preset for the channel. This is selectable only for <code>ADVANCED_HD</code> and <code>ADVANCED_SD</code> channel types. For those channel types, the default <code>preset</code> is <code>HIGHER_BANDWIDTH_DELIVERY</code>. For other channel types (<code>BASIC</code> and <code>STANDARD</code>), <code>preset</code> is the empty string (<code>\"\"</code>).</p>",
+                    "shape": "TranscodePreset"
+                },
                 "recordingConfigurationArn": {
                     "documentation": "<p>Recording-configuration ARN. A value other than an empty string indicates that recording is enabled. Default: \"\" (empty string, recording is disabled).</p>",
                     "shape": "ChannelRecordingConfigurationArn"
                 },
                 "tags": {
                     "documentation": "<p>Tags attached to the resource. Array of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p>",
                     "shape": "Tags"
+                },
+                "type": {
+                    "documentation": "<p>Channel type, which determines the allowable resolution and bitrate. <i>If you exceed the allowable input resolution or bitrate, the stream probably will disconnect immediately.</i> Some types generate multiple qualities (renditions) from the original input; this automatically gives viewers the best experience for their devices and network conditions. Some types provide transcoded video; transcoding allows higher playback quality across a range of download speeds. Default: <code>STANDARD</code>. Valid values:</p> <ul> <li> <p> <code>BASIC</code>: Video is transmuxed: Amazon IVS delivers the original input quality to viewers. The viewer\u2019s video-quality choice is limited to the original input. Input resolution can be up to 1080p and bitrate can be up to 1.5 Mbps for 480p and up to 3.5 Mbps for resolutions between 480p and 1080p. Original audio is passed through.</p> </li> <li> <p> <code>STANDARD</code>: Video is transcoded: multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Transcoding allows higher playback quality across a range of download speeds. Resolution can be up to 1080p and bitrate can be up to 8.5 Mbps. Audio is transcoded only for renditions 360p and below; above that, audio is passed through. This is the default when you create a channel.</p> </li> <li> <p> <code>ADVANCED_SD</code>: Video is transcoded; multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Input resolution can be up to 1080p and bitrate can be up to 8.5 Mbps; output is capped at SD quality (480p). You can select an optional transcode preset (see below). Audio for all renditions is transcoded, and an audio-only rendition is available.</p> </li> <li> <p> <code>ADVANCED_HD</code>: Video is transcoded; multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Input resolution can be up to 1080p and bitrate can be up to 8.5 Mbps; output is capped at HD quality (720p). You can select an optional transcode preset (see below). Audio for all renditions is transcoded, and an audio-only rendition is available.</p> </li> </ul> <p>Optional <i>transcode presets</i> (available for the <code>ADVANCED</code> types) allow you to trade off available download bandwidth and video quality, to optimize the viewing experience. There are two presets:</p> <ul> <li> <p> <i>Constrained bandwidth delivery</i> uses a lower bitrate for each quality level. Use it if you have low download bandwidth and/or simple video content (e.g., talking heads)</p> </li> <li> <p> <i>Higher bandwidth delivery</i> uses a higher bitrate for each quality level. Use it if you have high download bandwidth and/or complex video content (e.g., flashes and quick scene changes).</p> </li> </ul>",
+                    "shape": "ChannelType"
                 }
             },
             "type": "structure"
         },
         "ChannelType": {
             "enum": [
                 "BASIC",
-                "STANDARD"
+                "STANDARD",
+                "ADVANCED_SD",
+                "ADVANCED_HD"
             ],
             "type": "string"
         },
         "Channels": {
             "member": {
                 "shape": "Channel"
             },
@@ -1043,32 +1197,40 @@
         },
         "CreateChannelRequest": {
             "members": {
                 "authorized": {
                     "documentation": "<p>Whether the channel is private (enabled for playback authorization). Default: <code>false</code>.</p>",
                     "shape": "Boolean"
                 },
+                "insecureIngest": {
+                    "documentation": "<p>Whether the channel allows insecure RTMP ingest. Default: <code>false</code>.</p>",
+                    "shape": "Boolean"
+                },
                 "latencyMode": {
                     "documentation": "<p>Channel latency mode. Use <code>NORMAL</code> to broadcast and deliver live video up to Full HD. Use <code>LOW</code> for near-real-time interaction with viewers. (Note: In the Amazon IVS console, <code>LOW</code> and <code>NORMAL</code> correspond to Ultra-low and Standard, respectively.) Default: <code>LOW</code>.</p>",
                     "shape": "ChannelLatencyMode"
                 },
                 "name": {
                     "documentation": "<p>Channel name.</p>",
                     "shape": "ChannelName"
                 },
+                "preset": {
+                    "documentation": "<p>Optional transcode preset for the channel. This is selectable only for <code>ADVANCED_HD</code> and <code>ADVANCED_SD</code> channel types. For those channel types, the default <code>preset</code> is <code>HIGHER_BANDWIDTH_DELIVERY</code>. For other channel types (<code>BASIC</code> and <code>STANDARD</code>), <code>preset</code> is the empty string (<code>\"\"</code>).</p>",
+                    "shape": "TranscodePreset"
+                },
                 "recordingConfigurationArn": {
                     "documentation": "<p>Recording-configuration ARN. Default: \"\" (empty string, recording is disabled).</p>",
                     "shape": "ChannelRecordingConfigurationArn"
                 },
                 "tags": {
                     "documentation": "<p>Array of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \"Tag naming limits and requirements\"; Amazon IVS has no service-specific constraints beyond what is documented there.</p>",
                     "shape": "Tags"
                 },
                 "type": {
-                    "documentation": "<p>Channel type, which determines the allowable resolution and bitrate. <i>If you exceed the allowable resolution or bitrate, the stream probably will disconnect immediately.</i> Default: <code>STANDARD</code>. Valid values:</p> <ul> <li> <p> <code>STANDARD</code>: Video is transcoded: multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Transcoding allows higher playback quality across a range of download speeds. Resolution can be up to 1080p and bitrate can be up to 8.5 Mbps. Audio is transcoded only for renditions 360p and below; above that, audio is passed through. This is the default.</p> </li> <li> <p> <code>BASIC</code>: Video is transmuxed: Amazon IVS delivers the original input to viewers. The viewer\u2019s video-quality choice is limited to the original input. Resolution can be up to 1080p and bitrate can be up to 1.5 Mbps for 480p and up to 3.5 Mbps for resolutions between 480p and 1080p.</p> </li> </ul>",
+                    "documentation": "<p>Channel type, which determines the allowable resolution and bitrate. <i>If you exceed the allowable input resolution or bitrate, the stream probably will disconnect immediately.</i> Some types generate multiple qualities (renditions) from the original input; this automatically gives viewers the best experience for their devices and network conditions. Some types provide transcoded video; transcoding allows higher playback quality across a range of download speeds. Default: <code>STANDARD</code>. Valid values:</p> <ul> <li> <p> <code>BASIC</code>: Video is transmuxed: Amazon IVS delivers the original input quality to viewers. The viewer\u2019s video-quality choice is limited to the original input. Input resolution can be up to 1080p and bitrate can be up to 1.5 Mbps for 480p and up to 3.5 Mbps for resolutions between 480p and 1080p. Original audio is passed through.</p> </li> <li> <p> <code>STANDARD</code>: Video is transcoded: multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Transcoding allows higher playback quality across a range of download speeds. Resolution can be up to 1080p and bitrate can be up to 8.5 Mbps. Audio is transcoded only for renditions 360p and below; above that, audio is passed through. This is the default when you create a channel.</p> </li> <li> <p> <code>ADVANCED_SD</code>: Video is transcoded; multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Input resolution can be up to 1080p and bitrate can be up to 8.5 Mbps; output is capped at SD quality (480p). You can select an optional transcode preset (see below). Audio for all renditions is transcoded, and an audio-only rendition is available.</p> </li> <li> <p> <code>ADVANCED_HD</code>: Video is transcoded; multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Input resolution can be up to 1080p and bitrate can be up to 8.5 Mbps; output is capped at HD quality (720p). You can select an optional transcode preset (see below). Audio for all renditions is transcoded, and an audio-only rendition is available.</p> </li> </ul> <p>Optional <i>transcode presets</i> (available for the <code>ADVANCED</code> types) allow you to trade off available download bandwidth and video quality, to optimize the viewing experience. There are two presets:</p> <ul> <li> <p> <i>Constrained bandwidth delivery</i> uses a lower bitrate for each quality level. Use it if you have low download bandwidth and/or simple video content (e.g., talking heads)</p> </li> <li> <p> <i>Higher bandwidth delivery</i> uses a higher bitrate for each quality level. Use it if you have high download bandwidth and/or complex video content (e.g., flashes and quick scene changes).</p> </li> </ul>",
                     "shape": "ChannelType"
                 }
             },
             "type": "structure"
         },
         "CreateChannelResponse": {
             "members": {
@@ -1379,14 +1541,17 @@
                 }
             },
             "type": "structure"
         },
         "IngestEndpoint": {
             "type": "string"
         },
+        "InsecureIngest": {
+            "type": "boolean"
+        },
         "Integer": {
             "type": "long"
         },
         "InternalServerException": {
             "documentation": "<p/>",
             "error": {
                 "httpStatusCode": 500
@@ -1919,14 +2084,39 @@
                 "exceptionMessage": {
                     "documentation": "<p>Request would cause a service quota to be exceeded.</p>",
                     "shape": "errorMessage"
                 }
             },
             "type": "structure"
         },
+        "StartViewerSessionRevocationRequest": {
+            "members": {
+                "channelArn": {
+                    "documentation": "<p>The ARN of the channel associated with the viewer session to revoke.</p>",
+                    "shape": "ChannelArn"
+                },
+                "viewerId": {
+                    "documentation": "<p>The ID of the viewer associated with the viewer session to revoke. Do not use this field for personally identifying, confidential, or sensitive information.</p>",
+                    "shape": "ViewerId"
+                },
+                "viewerSessionVersionsLessThanOrEqualTo": {
+                    "documentation": "<p>An optional filter on which versions of the viewer session to revoke. All versions less than or equal to the specified version will be revoked. Default: 0.</p>",
+                    "shape": "ViewerSessionVersion"
+                }
+            },
+            "required": [
+                "channelArn",
+                "viewerId"
+            ],
+            "type": "structure"
+        },
+        "StartViewerSessionRevocationResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "StopStreamRequest": {
             "members": {
                 "channelArn": {
                     "documentation": "<p>ARN of the channel for which the stream is to be stopped.</p>",
                     "shape": "ChannelArn"
                 }
             },
@@ -2278,15 +2468,15 @@
             "type": "map",
             "value": {
                 "shape": "TagValue"
             }
         },
         "TargetIntervalSeconds": {
             "max": 60,
-            "min": 5,
+            "min": 1,
             "type": "long"
         },
         "ThrottlingException": {
             "documentation": "<p/>",
             "error": {
                 "httpStatusCode": 429,
                 "senderFault": true
@@ -2314,14 +2504,21 @@
             },
             "type": "structure"
         },
         "Time": {
             "timestampFormat": "iso8601",
             "type": "timestamp"
         },
+        "TranscodePreset": {
+            "enum": [
+                "HIGHER_BANDWIDTH_DELIVERY",
+                "CONSTRAINED_BANDWIDTH_DELIVERY"
+            ],
+            "type": "string"
+        },
         "UntagResourceRequest": {
             "members": {
                 "resourceArn": {
                     "documentation": "<p>ARN of the resource for which tags are to be removed. The ARN must be URL-encoded.</p>",
                     "location": "uri",
                     "locationName": "resourceArn",
                     "shape": "ResourceArn"
@@ -2349,28 +2546,36 @@
                     "documentation": "<p>ARN of the channel to be updated.</p>",
                     "shape": "ChannelArn"
                 },
                 "authorized": {
                     "documentation": "<p>Whether the channel is private (enabled for playback authorization).</p>",
                     "shape": "Boolean"
                 },
+                "insecureIngest": {
+                    "documentation": "<p>Whether the channel allows insecure RTMP ingest. Default: <code>false</code>.</p>",
+                    "shape": "Boolean"
+                },
                 "latencyMode": {
                     "documentation": "<p>Channel latency mode. Use <code>NORMAL</code> to broadcast and deliver live video up to Full HD. Use <code>LOW</code> for near-real-time interaction with viewers. (Note: In the Amazon IVS console, <code>LOW</code> and <code>NORMAL</code> correspond to Ultra-low and Standard, respectively.)</p>",
                     "shape": "ChannelLatencyMode"
                 },
                 "name": {
                     "documentation": "<p>Channel name.</p>",
                     "shape": "ChannelName"
                 },
+                "preset": {
+                    "documentation": "<p>Optional transcode preset for the channel. This is selectable only for <code>ADVANCED_HD</code> and <code>ADVANCED_SD</code> channel types. For those channel types, the default <code>preset</code> is <code>HIGHER_BANDWIDTH_DELIVERY</code>. For other channel types (<code>BASIC</code> and <code>STANDARD</code>), <code>preset</code> is the empty string (<code>\"\"</code>).</p>",
+                    "shape": "TranscodePreset"
+                },
                 "recordingConfigurationArn": {
                     "documentation": "<p>Recording-configuration ARN. If this is set to an empty string, recording is disabled. A value other than an empty string indicates that recording is enabled</p>",
                     "shape": "ChannelRecordingConfigurationArn"
                 },
                 "type": {
-                    "documentation": "<p>Channel type, which determines the allowable resolution and bitrate. <i>If you exceed the allowable resolution or bitrate, the stream probably will disconnect immediately</i>. Valid values:</p> <ul> <li> <p> <code>STANDARD</code>: Video is transcoded: multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Transcoding allows higher playback quality across a range of download speeds. Resolution can be up to 1080p and bitrate can be up to 8.5 Mbps. Audio is transcoded only for renditions 360p and below; above that, audio is passed through. This is the default.</p> </li> <li> <p> <code>BASIC</code>: Video is transmuxed: Amazon IVS delivers the original input to viewers. The viewer\u2019s video-quality choice is limited to the original input. Resolution can be up to 1080p and bitrate can be up to 1.5 Mbps for 480p and up to 3.5 Mbps for resolutions between 480p and 1080p.</p> </li> </ul>",
+                    "documentation": "<p>Channel type, which determines the allowable resolution and bitrate. <i>If you exceed the allowable input resolution or bitrate, the stream probably will disconnect immediately.</i> Some types generate multiple qualities (renditions) from the original input; this automatically gives viewers the best experience for their devices and network conditions. Some types provide transcoded video; transcoding allows higher playback quality across a range of download speeds. Default: <code>STANDARD</code>. Valid values:</p> <ul> <li> <p> <code>BASIC</code>: Video is transmuxed: Amazon IVS delivers the original input quality to viewers. The viewer\u2019s video-quality choice is limited to the original input. Input resolution can be up to 1080p and bitrate can be up to 1.5 Mbps for 480p and up to 3.5 Mbps for resolutions between 480p and 1080p. Original audio is passed through.</p> </li> <li> <p> <code>STANDARD</code>: Video is transcoded: multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Transcoding allows higher playback quality across a range of download speeds. Resolution can be up to 1080p and bitrate can be up to 8.5 Mbps. Audio is transcoded only for renditions 360p and below; above that, audio is passed through. This is the default when you create a channel.</p> </li> <li> <p> <code>ADVANCED_SD</code>: Video is transcoded; multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Input resolution can be up to 1080p and bitrate can be up to 8.5 Mbps; output is capped at SD quality (480p). You can select an optional transcode preset (see below). Audio for all renditions is transcoded, and an audio-only rendition is available.</p> </li> <li> <p> <code>ADVANCED_HD</code>: Video is transcoded; multiple qualities are generated from the original input, to automatically give viewers the best experience for their devices and network conditions. Input resolution can be up to 1080p and bitrate can be up to 8.5 Mbps; output is capped at HD quality (720p). You can select an optional transcode preset (see below). Audio for all renditions is transcoded, and an audio-only rendition is available.</p> </li> </ul> <p>Optional <i>transcode presets</i> (available for the <code>ADVANCED</code> types) allow you to trade off available download bandwidth and video quality, to optimize the viewing experience. There are two presets:</p> <ul> <li> <p> <i>Constrained bandwidth delivery</i> uses a lower bitrate for each quality level. Use it if you have low download bandwidth and/or simple video content (e.g., talking heads)</p> </li> <li> <p> <i>Higher bandwidth delivery</i> uses a higher bitrate for each quality level. Use it if you have high download bandwidth and/or complex video content (e.g., flashes and quick scene changes).</p> </li> </ul>",
                     "shape": "ChannelType"
                 }
             },
             "required": [
                 "arn"
             ],
             "type": "structure"
@@ -2432,14 +2637,23 @@
                 "videoWidth": {
                     "documentation": "<p>Video-resolution width in pixels.</p>",
                     "shape": "Integer"
                 }
             },
             "type": "structure"
         },
+        "ViewerId": {
+            "max": 40,
+            "min": 1,
+            "type": "string"
+        },
+        "ViewerSessionVersion": {
+            "min": 0,
+            "type": "integer"
+        },
         "errorCode": {
             "type": "string"
         },
         "errorMessage": {
             "type": "string"
         }
     },
```

### Comparing `botocore-a-la-carte-ivs-1.29.99/botocore_a_la_carte_ivs.egg-info/PKG-INFO` & `botocore-a-la-carte-ivs-1.30.0/botocore_a_la_carte_ivs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ivs
-Version: 1.29.99
+Version: 1.30.0
 Summary: ivs data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ivs-1.29.99/setup.py` & `botocore-a-la-carte-ivs-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ivs',
-    version="1.29.99",
+    version="1.30.0",
     description='ivs data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ivs/*/*.json'],
```

