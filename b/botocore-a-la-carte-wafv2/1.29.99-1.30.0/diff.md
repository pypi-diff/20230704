# Comparing `tmp/botocore-a-la-carte-wafv2-1.29.99.tar.gz` & `tmp/botocore-a-la-carte-wafv2-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-wafv2-1.29.99.tar", last modified: Sat Mar 25 01:23:14 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-wafv2-1.30.0.tar", last modified: Tue Jul  4 01:45:07 2023, max compression
```

## Comparing `botocore-a-la-carte-wafv2-1.29.99.tar` & `botocore-a-la-carte-wafv2-1.30.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:14.613284 botocore-a-la-carte-wafv2-1.29.99/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-25 01:23:14.000000 botocore-a-la-carte-wafv2-1.29.99/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-25 01:23:14.613284 botocore-a-la-carte-wafv2-1.29.99/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:14.613284 botocore-a-la-carte-wafv2-1.29.99/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:14.613284 botocore-a-la-carte-wafv2-1.29.99/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:14.613284 botocore-a-la-carte-wafv2-1.29.99/botocore/data/wafv2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:14.613284 botocore-a-la-carte-wafv2-1.29.99/botocore/data/wafv2/2019-07-29/
--rw-r--r--   0 runner    (1001) docker     (123)    47246 2023-03-25 01:22:12.000000 botocore-a-la-carte-wafv2-1.29.99/botocore/data/wafv2/2019-07-29/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-25 01:22:12.000000 botocore-a-la-carte-wafv2-1.29.99/botocore/data/wafv2/2019-07-29/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-25 01:22:12.000000 botocore-a-la-carte-wafv2-1.29.99/botocore/data/wafv2/2019-07-29/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   378414 2023-03-25 01:22:12.000000 botocore-a-la-carte-wafv2-1.29.99/botocore/data/wafv2/2019-07-29/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 01:23:14.613284 botocore-a-la-carte-wafv2-1.29.99/botocore_a_la_carte_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-25 01:23:14.000000 botocore-a-la-carte-wafv2-1.29.99/botocore_a_la_carte_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-25 01:23:14.000000 botocore-a-la-carte-wafv2-1.29.99/botocore_a_la_carte_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 01:23:14.000000 botocore-a-la-carte-wafv2-1.29.99/botocore_a_la_carte_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 01:23:14.000000 botocore-a-la-carte-wafv2-1.29.99/botocore_a_la_carte_wafv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 01:23:14.613284 botocore-a-la-carte-wafv2-1.29.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-25 01:23:14.000000 botocore-a-la-carte-wafv2-1.29.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:07.318892 botocore-a-la-carte-wafv2-1.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:45:07.000000 botocore-a-la-carte-wafv2-1.30.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-04 01:45:07.318892 botocore-a-la-carte-wafv2-1.30.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:07.314892 botocore-a-la-carte-wafv2-1.30.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:07.314892 botocore-a-la-carte-wafv2-1.30.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:07.314892 botocore-a-la-carte-wafv2-1.30.0/botocore/data/wafv2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:07.314892 botocore-a-la-carte-wafv2-1.30.0/botocore/data/wafv2/2019-07-29/
+-rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-07-04 01:44:02.000000 botocore-a-la-carte-wafv2-1.30.0/botocore/data/wafv2/2019-07-29/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-wafv2-1.30.0/botocore/data/wafv2/2019-07-29/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 01:44:02.000000 botocore-a-la-carte-wafv2-1.30.0/botocore/data/wafv2/2019-07-29/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   447635 2023-07-04 01:44:02.000000 botocore-a-la-carte-wafv2-1.30.0/botocore/data/wafv2/2019-07-29/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:07.318892 botocore-a-la-carte-wafv2-1.30.0/botocore_a_la_carte_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-04 01:45:07.000000 botocore-a-la-carte-wafv2-1.30.0/botocore_a_la_carte_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-04 01:45:07.000000 botocore-a-la-carte-wafv2-1.30.0/botocore_a_la_carte_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:45:07.000000 botocore-a-la-carte-wafv2-1.30.0/botocore_a_la_carte_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:45:07.000000 botocore-a-la-carte-wafv2-1.30.0/botocore_a_la_carte_wafv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:45:07.318892 botocore-a-la-carte-wafv2-1.30.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-04 01:45:07.000000 botocore-a-la-carte-wafv2-1.30.0/setup.py
```

### Comparing `botocore-a-la-carte-wafv2-1.29.99/LICENSE.txt` & `botocore-a-la-carte-wafv2-1.30.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-wafv2-1.29.99/PKG-INFO` & `botocore-a-la-carte-wafv2-1.30.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-wafv2
-Version: 1.29.99
+Version: 1.30.0
 Summary: wafv2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-wafv2-1.29.99/botocore/data/wafv2/2019-07-29/service-2.json` & `botocore-a-la-carte-wafv2-1.30.0/botocore/data/wafv2/2019-07-29/service-2.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8774416560518985%*

 * *Differences: {"'documentation'": "'<fullname>WAF</fullname> <note> <p>This is the latest version of the "*

 * *                    '<b>WAF</b> API, released in November, 2019. The names of the entities that '*

 * *                    'you use to access this API, like endpoints and namespaces, all have the '*

 * *                    'versioning information added, like "V2" or "v2", to distinguish from the '*

 * *                    'prior version. We recommend migrating your resources to this version, because '*

 * *                    'it has a […]*

```diff
@@ -1,24 +1,24 @@
 {
-    "documentation": "<fullname>WAF</fullname> <note> <p>This is the latest version of the <b>WAF</b> API, released in November, 2019. The names of the entities that you use to access this API, like endpoints and namespaces, all have the versioning information added, like \"V2\" or \"v2\", to distinguish from the prior version. We recommend migrating your resources to this version, because it has a number of significant improvements.</p> <p>If you used WAF prior to this release, you can't use this WAFV2 API to access any WAF resources that you created before. You can access your old rules, web ACLs, and other WAF resources only through the WAF Classic APIs. The WAF Classic APIs have retained the prior names, endpoints, and namespaces. </p> <p>For information, including how to migrate your WAF resources to this version, see the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p> </note> <p>WAF is a web application firewall that lets you monitor the HTTP and HTTPS requests that are forwarded to an Amazon CloudFront distribution, Amazon API Gateway REST API, Application Load Balancer, AppSync GraphQL API, Amazon Cognito user pool, or App Runner service. WAF also lets you control access to your content, to protect the Amazon Web Services resource that WAF is monitoring. Based on conditions that you specify, such as the IP addresses that requests originate from or the values of query strings, the protected resource responds to requests with either the requested content, an HTTP 403 status code (Forbidden), or with a custom response. </p> <p>This API guide is for developers who need detailed information about WAF API actions, data types, and errors. For detailed information about WAF features and guidance for configuring and using WAF, see the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/what-is-aws-waf.html\">WAF Developer Guide</a>.</p> <p>You can make calls using the endpoints listed in <a href=\"https://docs.aws.amazon.com/general/latest/gr/waf.html\">WAF endpoints and quotas</a>. </p> <ul> <li> <p>For regional applications, you can use any of the endpoints in the list. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> </li> <li> <p>For Amazon CloudFront applications, you must use the API endpoint listed for US East (N. Virginia): us-east-1.</p> </li> </ul> <p>Alternatively, you can use one of the Amazon Web Services SDKs to access an API that's tailored to the programming language or platform that you're using. For more information, see <a href=\"http://aws.amazon.com/tools/#SDKs\">Amazon Web Services SDKs</a>.</p> <p>We currently provide two versions of the WAF API: this API and the prior versions, the classic WAF APIs. This new API provides the same functionality as the older versions, with the following major improvements:</p> <ul> <li> <p>You use one API for both global and regional applications. Where you need to distinguish the scope, you specify a <code>Scope</code> parameter and set it to <code>CLOUDFRONT</code> or <code>REGIONAL</code>. </p> </li> <li> <p>You can define a web ACL or rule group with a single call, and update it with a single call. You define all rule specifications in JSON format, and pass them to your rule group or web ACL calls.</p> </li> <li> <p>The limits WAF places on the use of rules more closely reflects the cost of running each type of rule. Rule groups include capacity settings, so you know the maximum cost of a rule group when you use it.</p> </li> </ul>",
+    "documentation": "<fullname>WAF</fullname> <note> <p>This is the latest version of the <b>WAF</b> API, released in November, 2019. The names of the entities that you use to access this API, like endpoints and namespaces, all have the versioning information added, like \"V2\" or \"v2\", to distinguish from the prior version. We recommend migrating your resources to this version, because it has a number of significant improvements.</p> <p>If you used WAF prior to this release, you can't use this WAFV2 API to access any WAF resources that you created before. You can access your old rules, web ACLs, and other WAF resources only through the WAF Classic APIs. The WAF Classic APIs have retained the prior names, endpoints, and namespaces. </p> <p>For information, including how to migrate your WAF resources to this version, see the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p> </note> <p>WAF is a web application firewall that lets you monitor the HTTP and HTTPS requests that are forwarded to an Amazon CloudFront distribution, Amazon API Gateway REST API, Application Load Balancer, AppSync GraphQL API, Amazon Cognito user pool, App Runner service, or Amazon Web Services Verified Access instance. WAF also lets you control access to your content, to protect the Amazon Web Services resource that WAF is monitoring. Based on conditions that you specify, such as the IP addresses that requests originate from or the values of query strings, the protected resource responds to requests with either the requested content, an HTTP 403 status code (Forbidden), or with a custom response. </p> <p>This API guide is for developers who need detailed information about WAF API actions, data types, and errors. For detailed information about WAF features and guidance for configuring and using WAF, see the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/what-is-aws-waf.html\">WAF Developer Guide</a>.</p> <p>You can make calls using the endpoints listed in <a href=\"https://docs.aws.amazon.com/general/latest/gr/waf.html\">WAF endpoints and quotas</a>. </p> <ul> <li> <p>For regional applications, you can use any of the endpoints in the list. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> </li> <li> <p>For Amazon CloudFront applications, you must use the API endpoint listed for US East (N. Virginia): us-east-1.</p> </li> </ul> <p>Alternatively, you can use one of the Amazon Web Services SDKs to access an API that's tailored to the programming language or platform that you're using. For more information, see <a href=\"http://aws.amazon.com/tools/#SDKs\">Amazon Web Services SDKs</a>.</p> <p>We currently provide two versions of the WAF API: this API and the prior versions, the classic WAF APIs. This new API provides the same functionality as the older versions, with the following major improvements:</p> <ul> <li> <p>You use one API for both global and regional applications. Where you need to distinguish the scope, you specify a <code>Scope</code> parameter and set it to <code>CLOUDFRONT</code> or <code>REGIONAL</code>. </p> </li> <li> <p>You can define a web ACL or rule group with a single call, and update it with a single call. You define all rule specifications in JSON format, and pass them to your rule group or web ACL calls.</p> </li> <li> <p>The limits WAF places on the use of rules more closely reflects the cost of running each type of rule. Rule groups include capacity settings, so you know the maximum cost of a rule group when you use it.</p> </li> </ul>",
     "metadata": {
         "apiVersion": "2019-07-29",
         "endpointPrefix": "wafv2",
         "jsonVersion": "1.1",
         "protocol": "json",
         "serviceAbbreviation": "WAFV2",
         "serviceFullName": "AWS WAFV2",
         "serviceId": "WAFV2",
         "signatureVersion": "v4",
         "targetPrefix": "AWSWAF_20190729",
         "uid": "wafv2-2019-07-29"
     },
     "operations": {
         "AssociateWebACL": {
-            "documentation": "<p>Associates a web ACL with a regional application resource, to protect the resource. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>For Amazon CloudFront, don't use this call. Instead, use your CloudFront distribution configuration. To associate a web ACL, in the CloudFront call <code>UpdateDistribution</code>, set the web ACL ID to the Amazon Resource Name (ARN) of the web ACL. For information, see <a href=\"https://docs.aws.amazon.com/cloudfront/latest/APIReference/API_UpdateDistribution.html\">UpdateDistribution</a>.</p> <p>When you make changes to web ACLs or web ACL components, like rules and rule groups, WAF propagates the changes everywhere that the web ACL and its components are stored and used. Your changes are applied within seconds, but there might be a brief period of inconsistency when the changes have arrived in some places and not in others. So, for example, if you change a rule action setting, the action might be the old action in one area and the new action in another area. Or if you add an IP address to an IP set used in a blocking rule, the new address might briefly be blocked in one area while still allowed in another. This temporary inconsistency can occur when you first associate a web ACL with an Amazon Web Services resource and when you change a web ACL that is already associated with a resource. Generally, any inconsistencies of this type last only a few seconds.</p>",
+            "documentation": "<p>Associates a web ACL with a regional application resource, to protect the resource. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>For Amazon CloudFront, don't use this call. Instead, use your CloudFront distribution configuration. To associate a web ACL, in the CloudFront call <code>UpdateDistribution</code>, set the web ACL ID to the Amazon Resource Name (ARN) of the web ACL. For information, see <a href=\"https://docs.aws.amazon.com/cloudfront/latest/APIReference/API_UpdateDistribution.html\">UpdateDistribution</a> in the <i>Amazon CloudFront Developer Guide</i>. </p> <p>When you make changes to web ACLs or web ACL components, like rules and rule groups, WAF propagates the changes everywhere that the web ACL and its components are stored and used. Your changes are applied within seconds, but there might be a brief period of inconsistency when the changes have arrived in some places and not in others. So, for example, if you change a rule action setting, the action might be the old action in one area and the new action in another area. Or if you add an IP address to an IP set used in a blocking rule, the new address might briefly be blocked in one area while still allowed in another. This temporary inconsistency can occur when you first associate a web ACL with an Amazon Web Services resource and when you change a web ACL that is already associated with a resource. Generally, any inconsistencies of this type last only a few seconds.</p>",
             "errors": [
                 {
                     "shape": "WAFInternalErrorException"
                 },
                 {
                     "shape": "WAFInvalidParameterException"
                 },
@@ -41,15 +41,15 @@
             },
             "name": "AssociateWebACL",
             "output": {
                 "shape": "AssociateWebACLResponse"
             }
         },
         "CheckCapacity": {
-            "documentation": "<p>Returns the web ACL capacity unit (WCU) requirements for a specified scope and set of rules. You can use this to check the capacity requirements for the rules you want to use in a <a>RuleGroup</a> or <a>WebACL</a>. </p> <p>WAF uses WCUs to calculate and control the operating resources that are used to run your rules, rule groups, and web ACLs. WAF calculates capacity differently for each rule type, to reflect the relative cost of each rule. Simple rules that cost little to run use fewer WCUs than more complex rules that use more processing power. Rule group capacity is fixed at creation, which helps users plan their web ACL WCU usage when they use a rule group. The WCU limit for web ACLs is 1,500. </p>",
+            "documentation": "<p>Returns the web ACL capacity unit (WCU) requirements for a specified scope and set of rules. You can use this to check the capacity requirements for the rules you want to use in a <a>RuleGroup</a> or <a>WebACL</a>. </p> <p>WAF uses WCUs to calculate and control the operating resources that are used to run your rules, rule groups, and web ACLs. WAF calculates capacity differently for each rule type, to reflect the relative cost of each rule. Simple rules that cost little to run use fewer WCUs than more complex rules that use more processing power. Rule group capacity is fixed at creation, which helps users plan their web ACL WCU usage when they use a rule group. For more information, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/aws-waf-capacity-units.html\">WAF web ACL capacity units (WCU)</a> in the <i>WAF Developer Guide</i>. </p>",
             "errors": [
                 {
                     "shape": "WAFInternalErrorException"
                 },
                 {
                     "shape": "WAFInvalidParameterException"
                 },
@@ -83,14 +83,42 @@
                 "shape": "CheckCapacityRequest"
             },
             "name": "CheckCapacity",
             "output": {
                 "shape": "CheckCapacityResponse"
             }
         },
+        "CreateAPIKey": {
+            "documentation": "<p>Creates an API key that contains a set of token domains.</p> <p>API keys are required for the integration of the CAPTCHA API in your JavaScript client applications. The API lets you customize the placement and characteristics of the CAPTCHA puzzle for your end users. For more information about the CAPTCHA JavaScript integration, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-application-integration.html\">WAF client application integration</a> in the <i>WAF Developer Guide</i>.</p> <p>You can use a single key for up to 5 domains. After you generate a key, you can copy it for use in your JavaScript integration. </p>",
+            "errors": [
+                {
+                    "shape": "WAFInternalErrorException"
+                },
+                {
+                    "shape": "WAFInvalidParameterException"
+                },
+                {
+                    "shape": "WAFInvalidOperationException"
+                },
+                {
+                    "shape": "WAFLimitsExceededException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "CreateAPIKeyRequest"
+            },
+            "name": "CreateAPIKey",
+            "output": {
+                "shape": "CreateAPIKeyResponse"
+            }
+        },
         "CreateIPSet": {
             "documentation": "<p>Creates an <a>IPSet</a>, which you use to identify web requests that originate from specific IP addresses or ranges of IP addresses. For example, if you're receiving a lot of requests from a ranges of IP addresses, you can configure WAF to block them using an IPSet that lists those IP addresses. </p>",
             "errors": [
                 {
                     "shape": "WAFInternalErrorException"
                 },
                 {
@@ -213,15 +241,15 @@
             },
             "name": "CreateRuleGroup",
             "output": {
                 "shape": "CreateRuleGroupResponse"
             }
         },
         "CreateWebACL": {
-            "documentation": "<p>Creates a <a>WebACL</a> per the specifications provided.</p> <p> A web ACL defines a collection of rules to use to inspect and control web requests. Each rule has an action defined (allow, block, or count) for requests that match the statement of the rule. In the web ACL, you assign a default action to take (allow, block) for any request that does not match any of the rules. The rules in a web ACL can be a combination of the types <a>Rule</a>, <a>RuleGroup</a>, and managed rule group. You can associate a web ACL with one or more Amazon Web Services resources to protect. The resources can be an Amazon CloudFront distribution, an Amazon API Gateway REST API, an Application Load Balancer, an AppSync GraphQL API, Amazon Cognito user pool, or an App Runner service. </p>",
+            "documentation": "<p>Creates a <a>WebACL</a> per the specifications provided.</p> <p> A web ACL defines a collection of rules to use to inspect and control web requests. Each rule has an action defined (allow, block, or count) for requests that match the statement of the rule. In the web ACL, you assign a default action to take (allow, block) for any request that does not match any of the rules. The rules in a web ACL can be a combination of the types <a>Rule</a>, <a>RuleGroup</a>, and managed rule group. You can associate a web ACL with one or more Amazon Web Services resources to protect. The resources can be an Amazon CloudFront distribution, an Amazon API Gateway REST API, an Application Load Balancer, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p>",
             "errors": [
                 {
                     "shape": "WAFInternalErrorException"
                 },
                 {
                     "shape": "WAFInvalidParameterException"
                 },
@@ -478,15 +506,15 @@
             },
             "name": "DeleteRuleGroup",
             "output": {
                 "shape": "DeleteRuleGroupResponse"
             }
         },
         "DeleteWebACL": {
-            "documentation": "<p>Deletes the specified <a>WebACL</a>. </p> <p>You can only use this if <code>ManagedByFirewallManager</code> is false in the specified <a>WebACL</a>. </p> <note> <p>Before deleting any web ACL, first disassociate it from all resources.</p> <ul> <li> <p>To retrieve a list of the resources that are associated with a web ACL, use the following calls:</p> <ul> <li> <p>For regional resources, call <a>ListResourcesForWebACL</a>.</p> </li> <li> <p>For Amazon CloudFront distributions, use the CloudFront call <code>ListDistributionsByWebACLId</code>. For information, see <a href=\"https://docs.aws.amazon.com/cloudfront/latest/APIReference/API_ListDistributionsByWebACLId.html\">ListDistributionsByWebACLId</a>.</p> </li> </ul> </li> <li> <p>To disassociate a resource from a web ACL, use the following calls:</p> <ul> <li> <p>For regional resources, call <a>DisassociateWebACL</a>.</p> </li> <li> <p>For Amazon CloudFront distributions, provide an empty web ACL ID in the CloudFront call <code>UpdateDistribution</code>. For information, see <a href=\"https://docs.aws.amazon.com/cloudfront/latest/APIReference/API_UpdateDistribution.html\">UpdateDistribution</a>.</p> </li> </ul> </li> </ul> </note>",
+            "documentation": "<p>Deletes the specified <a>WebACL</a>. </p> <p>You can only use this if <code>ManagedByFirewallManager</code> is false in the specified <a>WebACL</a>. </p> <note> <p>Before deleting any web ACL, first disassociate it from all resources.</p> <ul> <li> <p>To retrieve a list of the resources that are associated with a web ACL, use the following calls:</p> <ul> <li> <p>For regional resources, call <a>ListResourcesForWebACL</a>.</p> </li> <li> <p>For Amazon CloudFront distributions, use the CloudFront call <code>ListDistributionsByWebACLId</code>. For information, see <a href=\"https://docs.aws.amazon.com/cloudfront/latest/APIReference/API_ListDistributionsByWebACLId.html\">ListDistributionsByWebACLId</a> in the <i>Amazon CloudFront API Reference</i>. </p> </li> </ul> </li> <li> <p>To disassociate a resource from a web ACL, use the following calls:</p> <ul> <li> <p>For regional resources, call <a>DisassociateWebACL</a>.</p> </li> <li> <p>For Amazon CloudFront distributions, provide an empty web ACL ID in the CloudFront call <code>UpdateDistribution</code>. For information, see <a href=\"https://docs.aws.amazon.com/cloudfront/latest/APIReference/API_UpdateDistribution.html\">UpdateDistribution</a> in the <i>Amazon CloudFront API Reference</i>. </p> </li> </ul> </li> </ul> </note>",
             "errors": [
                 {
                     "shape": "WAFInternalErrorException"
                 },
                 {
                     "shape": "WAFInvalidParameterException"
                 },
@@ -517,14 +545,61 @@
                 "shape": "DeleteWebACLRequest"
             },
             "name": "DeleteWebACL",
             "output": {
                 "shape": "DeleteWebACLResponse"
             }
         },
+        "DescribeAllManagedProducts": {
+            "documentation": "<p>Provides high-level information for the Amazon Web Services Managed Rules rule groups and Amazon Web Services Marketplace managed rule groups. </p>",
+            "errors": [
+                {
+                    "shape": "WAFInvalidOperationException"
+                },
+                {
+                    "shape": "WAFInternalErrorException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DescribeAllManagedProductsRequest"
+            },
+            "name": "DescribeAllManagedProducts",
+            "output": {
+                "shape": "DescribeAllManagedProductsResponse"
+            }
+        },
+        "DescribeManagedProductsByVendor": {
+            "documentation": "<p>Provides high-level information for the managed rule groups owned by a specific vendor. </p>",
+            "errors": [
+                {
+                    "shape": "WAFInvalidOperationException"
+                },
+                {
+                    "shape": "WAFInternalErrorException"
+                },
+                {
+                    "shape": "WAFInvalidParameterException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DescribeManagedProductsByVendorRequest"
+            },
+            "name": "DescribeManagedProductsByVendor",
+            "output": {
+                "shape": "DescribeManagedProductsByVendorResponse"
+            }
+        },
         "DescribeManagedRuleGroup": {
             "documentation": "<p>Provides high-level information for a managed rule group, including descriptions of the rules. </p>",
             "errors": [
                 {
                     "shape": "WAFInternalErrorException"
                 },
                 {
@@ -552,15 +627,15 @@
             },
             "name": "DescribeManagedRuleGroup",
             "output": {
                 "shape": "DescribeManagedRuleGroupResponse"
             }
         },
         "DisassociateWebACL": {
-            "documentation": "<p>Disassociates the specified regional application resource from any existing web ACL association. A resource can have at most one web ACL association. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>For Amazon CloudFront, don't use this call. Instead, use your CloudFront distribution configuration. To disassociate a web ACL, provide an empty web ACL ID in the CloudFront call <code>UpdateDistribution</code>. For information, see <a href=\"https://docs.aws.amazon.com/cloudfront/latest/APIReference/API_UpdateDistribution.html\">UpdateDistribution</a>.</p>",
+            "documentation": "<p>Disassociates the specified regional application resource from any existing web ACL association. A resource can have at most one web ACL association. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>For Amazon CloudFront, don't use this call. Instead, use your CloudFront distribution configuration. To disassociate a web ACL, provide an empty web ACL ID in the CloudFront call <code>UpdateDistribution</code>. For information, see <a href=\"https://docs.aws.amazon.com/cloudfront/latest/APIReference/API_UpdateDistribution.html\">UpdateDistribution</a> in the <i>Amazon CloudFront API Reference</i>. </p>",
             "errors": [
                 {
                     "shape": "WAFInternalErrorException"
                 },
                 {
                     "shape": "WAFInvalidParameterException"
                 },
@@ -607,14 +682,42 @@
                 "shape": "GenerateMobileSdkReleaseUrlRequest"
             },
             "name": "GenerateMobileSdkReleaseUrl",
             "output": {
                 "shape": "GenerateMobileSdkReleaseUrlResponse"
             }
         },
+        "GetDecryptedAPIKey": {
+            "documentation": "<p>Returns your API key in decrypted form. Use this to check the token domains that you have defined for the key. </p> <p>API keys are required for the integration of the CAPTCHA API in your JavaScript client applications. The API lets you customize the placement and characteristics of the CAPTCHA puzzle for your end users. For more information about the CAPTCHA JavaScript integration, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-application-integration.html\">WAF client application integration</a> in the <i>WAF Developer Guide</i>.</p>",
+            "errors": [
+                {
+                    "shape": "WAFInternalErrorException"
+                },
+                {
+                    "shape": "WAFInvalidParameterException"
+                },
+                {
+                    "shape": "WAFInvalidOperationException"
+                },
+                {
+                    "shape": "WAFInvalidResourceException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "GetDecryptedAPIKeyRequest"
+            },
+            "name": "GetDecryptedAPIKey",
+            "output": {
+                "shape": "GetDecryptedAPIKeyResponse"
+            }
+        },
         "GetIPSet": {
             "documentation": "<p>Retrieves the specified <a>IPSet</a>.</p>",
             "errors": [
                 {
                     "shape": "WAFInternalErrorException"
                 },
                 {
@@ -745,27 +848,30 @@
             },
             "name": "GetPermissionPolicy",
             "output": {
                 "shape": "GetPermissionPolicyResponse"
             }
         },
         "GetRateBasedStatementManagedKeys": {
-            "documentation": "<p>Retrieves the keys that are currently blocked by a rate-based rule instance. The maximum number of managed keys that can be blocked for a single rate-based rule instance is 10,000. If more than 10,000 addresses exceed the rate limit, those with the highest rates are blocked.</p> <p>For a rate-based rule that you've defined inside a rule group, provide the name of the rule group reference statement in your request, in addition to the rate-based rule name and the web ACL name. </p> <p>WAF monitors web requests and manages keys independently for each unique combination of web ACL, optional rule group, and rate-based rule. For example, if you define a rate-based rule inside a rule group, and then use the rule group in a web ACL, WAF monitors web requests and manages keys for that web ACL, rule group reference statement, and rate-based rule instance. If you use the same rule group in a second web ACL, WAF monitors web requests and manages keys for this second usage completely independent of your first. </p>",
+            "documentation": "<p>Retrieves the IP addresses that are currently blocked by a rate-based rule instance. This is only available for rate-based rules that aggregate solely on the IP address or on the forwarded IP address. </p> <p>The maximum number of addresses that can be blocked for a single rate-based rule instance is 10,000. If more than 10,000 addresses exceed the rate limit, those with the highest rates are blocked.</p> <p>For a rate-based rule that you've defined inside a rule group, provide the name of the rule group reference statement in your request, in addition to the rate-based rule name and the web ACL name. </p> <p>WAF monitors web requests and manages keys independently for each unique combination of web ACL, optional rule group, and rate-based rule. For example, if you define a rate-based rule inside a rule group, and then use the rule group in a web ACL, WAF monitors web requests and manages keys for that web ACL, rule group reference statement, and rate-based rule instance. If you use the same rule group in a second web ACL, WAF monitors web requests and manages keys for this second usage completely independent of your first. </p>",
             "errors": [
                 {
                     "shape": "WAFInternalErrorException"
                 },
                 {
                     "shape": "WAFInvalidParameterException"
                 },
                 {
                     "shape": "WAFNonexistentItemException"
                 },
                 {
                     "shape": "WAFInvalidOperationException"
+                },
+                {
+                    "shape": "WAFUnsupportedAggregateKeyTypeException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -912,14 +1018,42 @@
                 "shape": "GetWebACLForResourceRequest"
             },
             "name": "GetWebACLForResource",
             "output": {
                 "shape": "GetWebACLForResourceResponse"
             }
         },
+        "ListAPIKeys": {
+            "documentation": "<p>Retrieves a list of the API keys that you've defined for the specified scope. </p> <p>API keys are required for the integration of the CAPTCHA API in your JavaScript client applications. The API lets you customize the placement and characteristics of the CAPTCHA puzzle for your end users. For more information about the CAPTCHA JavaScript integration, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-application-integration.html\">WAF client application integration</a> in the <i>WAF Developer Guide</i>.</p>",
+            "errors": [
+                {
+                    "shape": "WAFInternalErrorException"
+                },
+                {
+                    "shape": "WAFInvalidParameterException"
+                },
+                {
+                    "shape": "WAFInvalidOperationException"
+                },
+                {
+                    "shape": "WAFInvalidResourceException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "ListAPIKeysRequest"
+            },
+            "name": "ListAPIKeys",
+            "output": {
+                "shape": "ListAPIKeysResponse"
+            }
+        },
         "ListAvailableManagedRuleGroupVersions": {
             "documentation": "<p>Returns a list of the available versions for the specified managed rule group. </p>",
             "errors": [
                 {
                     "shape": "WAFInternalErrorException"
                 },
                 {
@@ -1524,15 +1658,15 @@
             },
             "name": "UpdateRuleGroup",
             "output": {
                 "shape": "UpdateRuleGroupResponse"
             }
         },
         "UpdateWebACL": {
-            "documentation": "<p>Updates the specified <a>WebACL</a>. While updating a web ACL, WAF provides continuous coverage to the resources that you have associated with the web ACL. </p> <note> <p>This operation completely replaces the mutable specifications that you already have for the web ACL with the ones that you provide to this call. </p> <p>To modify a web ACL, do the following: </p> <ol> <li> <p>Retrieve it by calling <a>GetWebACL</a> </p> </li> <li> <p>Update its settings as needed</p> </li> <li> <p>Provide the complete web ACL specification to this call</p> </li> </ol> </note> <p>When you make changes to web ACLs or web ACL components, like rules and rule groups, WAF propagates the changes everywhere that the web ACL and its components are stored and used. Your changes are applied within seconds, but there might be a brief period of inconsistency when the changes have arrived in some places and not in others. So, for example, if you change a rule action setting, the action might be the old action in one area and the new action in another area. Or if you add an IP address to an IP set used in a blocking rule, the new address might briefly be blocked in one area while still allowed in another. This temporary inconsistency can occur when you first associate a web ACL with an Amazon Web Services resource and when you change a web ACL that is already associated with a resource. Generally, any inconsistencies of this type last only a few seconds.</p> <p> A web ACL defines a collection of rules to use to inspect and control web requests. Each rule has an action defined (allow, block, or count) for requests that match the statement of the rule. In the web ACL, you assign a default action to take (allow, block) for any request that does not match any of the rules. The rules in a web ACL can be a combination of the types <a>Rule</a>, <a>RuleGroup</a>, and managed rule group. You can associate a web ACL with one or more Amazon Web Services resources to protect. The resources can be an Amazon CloudFront distribution, an Amazon API Gateway REST API, an Application Load Balancer, an AppSync GraphQL API, Amazon Cognito user pool, or an App Runner service. </p>",
+            "documentation": "<p>Updates the specified <a>WebACL</a>. While updating a web ACL, WAF provides continuous coverage to the resources that you have associated with the web ACL. </p> <note> <p>This operation completely replaces the mutable specifications that you already have for the web ACL with the ones that you provide to this call. </p> <p>To modify a web ACL, do the following: </p> <ol> <li> <p>Retrieve it by calling <a>GetWebACL</a> </p> </li> <li> <p>Update its settings as needed</p> </li> <li> <p>Provide the complete web ACL specification to this call</p> </li> </ol> </note> <p>When you make changes to web ACLs or web ACL components, like rules and rule groups, WAF propagates the changes everywhere that the web ACL and its components are stored and used. Your changes are applied within seconds, but there might be a brief period of inconsistency when the changes have arrived in some places and not in others. So, for example, if you change a rule action setting, the action might be the old action in one area and the new action in another area. Or if you add an IP address to an IP set used in a blocking rule, the new address might briefly be blocked in one area while still allowed in another. This temporary inconsistency can occur when you first associate a web ACL with an Amazon Web Services resource and when you change a web ACL that is already associated with a resource. Generally, any inconsistencies of this type last only a few seconds.</p> <p> A web ACL defines a collection of rules to use to inspect and control web requests. Each rule has an action defined (allow, block, or count) for requests that match the statement of the rule. In the web ACL, you assign a default action to take (allow, block) for any request that does not match any of the rules. The rules in a web ACL can be a combination of the types <a>Rule</a>, <a>RuleGroup</a>, and managed rule group. You can associate a web ACL with one or more Amazon Web Services resources to protect. The resources can be an Amazon CloudFront distribution, an Amazon API Gateway REST API, an Application Load Balancer, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p>",
             "errors": [
                 {
                     "shape": "WAFInternalErrorException"
                 },
                 {
                     "shape": "WAFInvalidParameterException"
                 },
@@ -1577,40 +1711,120 @@
             "name": "UpdateWebACL",
             "output": {
                 "shape": "UpdateWebACLResponse"
             }
         }
     },
     "shapes": {
+        "APIKey": {
+            "max": 2048,
+            "min": 1,
+            "pattern": ".*\\S.*",
+            "type": "string"
+        },
+        "APIKeySummaries": {
+            "member": {
+                "shape": "APIKeySummary"
+            },
+            "type": "list"
+        },
+        "APIKeySummary": {
+            "documentation": "<p>Information for a single API key. </p> <p>API keys are required for the integration of the CAPTCHA API in your JavaScript client applications. The API lets you customize the placement and characteristics of the CAPTCHA puzzle for your end users. For more information about the CAPTCHA JavaScript integration, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-application-integration.html\">WAF client application integration</a> in the <i>WAF Developer Guide</i>.</p>",
+            "members": {
+                "APIKey": {
+                    "documentation": "<p>The generated, encrypted API key. You can copy this for use in your JavaScript CAPTCHA integration. </p>",
+                    "shape": "APIKey"
+                },
+                "CreationTimestamp": {
+                    "documentation": "<p>The date and time that the key was created. </p>",
+                    "shape": "Timestamp"
+                },
+                "TokenDomains": {
+                    "documentation": "<p>The token domains that are defined in this API key. </p>",
+                    "shape": "TokenDomains"
+                },
+                "Version": {
+                    "documentation": "<p>Internal value used by WAF to manage the key. </p>",
+                    "shape": "APIKeyVersion"
+                }
+            },
+            "type": "structure"
+        },
+        "APIKeyTokenDomains": {
+            "member": {
+                "shape": "TokenDomain"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "APIKeyVersion": {
+            "min": 0,
+            "type": "integer"
+        },
+        "AWSManagedRulesACFPRuleSet": {
+            "documentation": "<p>Details for your use of the account creation fraud prevention managed rule group, <code>AWSManagedRulesACFPRuleSet</code>. This configuration is used in <code>ManagedRuleGroupConfig</code>. </p>",
+            "members": {
+                "CreationPath": {
+                    "documentation": "<p>The path of the account creation endpoint for your application. This is the page on your website that accepts the completed registration form for a new user. This page must accept <code>POST</code> requests.</p> <p>For example, for the URL <code>https://example.com/web/signup</code>, you would provide the path <code>/web/signup</code>.</p>",
+                    "shape": "CreationPathString"
+                },
+                "EnableRegexInPath": {
+                    "documentation": "<p>Allow the use of regular expressions in the registration page path and the account creation path. </p>",
+                    "shape": "Boolean"
+                },
+                "RegistrationPagePath": {
+                    "documentation": "<p>The path of the account registration endpoint for your application. This is the page on your website that presents the registration form to new users. </p> <note> <p>This page must accept <code>GET</code> text/html requests.</p> </note> <p>For example, for the URL <code>https://example.com/web/register</code>, you would provide the path <code>/web/register</code>.</p>",
+                    "shape": "RegistrationPagePathString"
+                },
+                "RequestInspection": {
+                    "documentation": "<p>The criteria for inspecting account creation requests, used by the ACFP rule group to validate and track account creation attempts. </p>",
+                    "shape": "RequestInspectionACFP"
+                },
+                "ResponseInspection": {
+                    "documentation": "<p>The criteria for inspecting responses to account creation requests, used by the ACFP rule group to track account creation success rates. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note> <p>The ACFP rule group evaluates the responses that your protected resources send back to client account creation attempts, keeping count of successful and failed attempts from each IP address and client session. Using this information, the rule group labels and mitigates requests from client sessions and IP addresses that have had too many successful account creation attempts in a short amount of time. </p>",
+                    "shape": "ResponseInspection"
+                }
+            },
+            "required": [
+                "CreationPath",
+                "RegistrationPagePath",
+                "RequestInspection"
+            ],
+            "type": "structure"
+        },
         "AWSManagedRulesATPRuleSet": {
             "documentation": "<p>Details for your use of the account takeover prevention managed rule group, <code>AWSManagedRulesATPRuleSet</code>. This configuration is used in <code>ManagedRuleGroupConfig</code>. </p>",
             "members": {
+                "EnableRegexInPath": {
+                    "documentation": "<p>Allow the use of regular expressions in the login page path. </p>",
+                    "shape": "Boolean"
+                },
                 "LoginPath": {
                     "documentation": "<p>The path of the login endpoint for your application. For example, for the URL <code>https://example.com/web/login</code>, you would provide the path <code>/web/login</code>.</p> <p>The rule group inspects only HTTP <code>POST</code> requests to your specified login endpoint.</p>",
                     "shape": "String"
                 },
                 "RequestInspection": {
                     "documentation": "<p>The criteria for inspecting login requests, used by the ATP rule group to validate credentials usage. </p>",
                     "shape": "RequestInspection"
                 },
                 "ResponseInspection": {
-                    "documentation": "<p>The criteria for inspecting responses to login requests, used by the ATP rule group to track login failure rates. </p> <p>The ATP rule group evaluates the responses that your protected resources send back to client login attempts, keeping count of successful and failed attempts from each IP address and client session. Using this information, the rule group labels and mitigates requests from client sessions and IP addresses that submit too many failed login attempts in a short amount of time. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note>",
+                    "documentation": "<p>The criteria for inspecting responses to login requests, used by the ATP rule group to track login failure rates. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note> <p>The ATP rule group evaluates the responses that your protected resources send back to client login attempts, keeping count of successful and failed attempts for each IP address and client session. Using this information, the rule group labels and mitigates requests from client sessions and IP addresses that have had too many failed login attempts in a short amount of time. </p>",
                     "shape": "ResponseInspection"
                 }
             },
             "required": [
                 "LoginPath"
             ],
             "type": "structure"
         },
         "AWSManagedRulesBotControlRuleSet": {
             "documentation": "<p>Details for your use of the Bot Control managed rule group, <code>AWSManagedRulesBotControlRuleSet</code>. This configuration is used in <code>ManagedRuleGroupConfig</code>. </p>",
             "members": {
                 "InspectionLevel": {
-                    "documentation": "<p>The inspection level to use for the Bot Control rule group. The common level is the least expensive. The targeted level includes all common level rules and adds rules with more advanced inspection criteria. For details, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/aws-managed-rule-groups-bot.html\">WAF Bot Control rule group</a>.</p>",
+                    "documentation": "<p>The inspection level to use for the Bot Control rule group. The common level is the least expensive. The targeted level includes all common level rules and adds rules with more advanced inspection criteria. For details, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/aws-managed-rule-groups-bot.html\">WAF Bot Control rule group</a> in the <i>WAF Developer Guide</i>.</p>",
                     "shape": "InspectionLevel"
                 }
             },
             "required": [
                 "InspectionLevel"
             ],
             "type": "structure"
@@ -1638,29 +1852,48 @@
                 "COUNT",
                 "CAPTCHA",
                 "CHALLENGE",
                 "EXCLUDED_AS_COUNT"
             ],
             "type": "string"
         },
+        "AddressField": {
+            "documentation": "<p>The name of a field in the request payload that contains part or all of your customer's primary physical address. </p> <p>This data type is used in the <code>RequestInspectionACFP</code> data type. </p>",
+            "members": {
+                "Identifier": {
+                    "documentation": "<p>The name of a single primary address field. </p> <p>How you specify the address fields depends on the request inspection payload type.</p> <ul> <li> <p>For JSON payloads, specify the field identifiers in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"form\": { \"primaryaddressline1\": \"THE_ADDRESS1\", \"primaryaddressline2\": \"THE_ADDRESS2\", \"primaryaddressline3\": \"THE_ADDRESS3\" } }</code>, the address field idenfiers are <code>/form/primaryaddressline1</code>, <code>/form/primaryaddressline2</code>, and <code>/form/primaryaddressline3</code>.</p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with input elements named <code>primaryaddressline1</code>, <code>primaryaddressline2</code>, and <code>primaryaddressline3</code>, the address fields identifiers are <code>primaryaddressline1</code>, <code>primaryaddressline2</code>, and <code>primaryaddressline3</code>. </p> </li> </ul>",
+                    "shape": "FieldIdentifier"
+                }
+            },
+            "required": [
+                "Identifier"
+            ],
+            "type": "structure"
+        },
+        "AddressFields": {
+            "member": {
+                "shape": "AddressField"
+            },
+            "type": "list"
+        },
         "All": {
-            "documentation": "<p>Inspect all of the elements that WAF has parsed and extracted from the web request component that you've identified in your <a>FieldToMatch</a> specifications. </p> <p>This is used only in the <a>FieldToMatch</a> specification for some web request component types. </p> <p>JSON specification: <code>\"All\": {}</code> </p>",
+            "documentation": "<p>Inspect all of the elements that WAF has parsed and extracted from the web request component that you've identified in your <a>FieldToMatch</a> specifications. </p> <p>This is used in the <a>FieldToMatch</a> specification for some web request component types. </p> <p>JSON specification: <code>\"All\": {}</code> </p>",
             "members": {},
             "type": "structure"
         },
         "AllQueryArguments": {
-            "documentation": "<p>Inspect all query arguments of the web request. </p> <p>This is used only in the <a>FieldToMatch</a> specification for some web request component types. </p> <p>JSON specification: <code>\"AllQueryArguments\": {}</code> </p>",
+            "documentation": "<p>Inspect all query arguments of the web request. </p> <p>This is used in the <a>FieldToMatch</a> specification for some web request component types. </p> <p>JSON specification: <code>\"AllQueryArguments\": {}</code> </p>",
             "members": {},
             "type": "structure"
         },
         "AllowAction": {
             "documentation": "<p>Specifies that WAF should allow the request and optionally defines additional custom handling for the request.</p> <p>This is used in the context of other settings, for example to specify values for <a>RuleAction</a> and web ACL <a>DefaultAction</a>. </p>",
             "members": {
                 "CustomRequestHandling": {
-                    "documentation": "<p>Defines custom handling for the web request.</p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>Defines custom handling for the web request.</p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomRequestHandling"
                 }
             },
             "type": "structure"
         },
         "AndStatement": {
             "documentation": "<p>A logical rule statement used to combine other rule statements with AND logic. You provide more than one <a>Statement</a> within the <code>AndStatement</code>. </p>",
@@ -1674,15 +1907,15 @@
                 "Statements"
             ],
             "type": "structure"
         },
         "AssociateWebACLRequest": {
             "members": {
                 "ResourceArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the resource to associate with the web ACL. </p> <p>The ARN must be in one of the following formats:</p> <ul> <li> <p>For an Application Load Balancer: <code>arn:aws:elasticloadbalancing:<i>region</i>:<i>account-id</i>:loadbalancer/app/<i>load-balancer-name</i>/<i>load-balancer-id</i> </code> </p> </li> <li> <p>For an Amazon API Gateway REST API: <code>arn:aws:apigateway:<i>region</i>::/restapis/<i>api-id</i>/stages/<i>stage-name</i> </code> </p> </li> <li> <p>For an AppSync GraphQL API: <code>arn:aws:appsync:<i>region</i>:<i>account-id</i>:apis/<i>GraphQLApiId</i> </code> </p> </li> <li> <p>For an Amazon Cognito user pool: <code>arn:aws:cognito-idp:<i>region</i>:<i>account-id</i>:userpool/<i>user-pool-id</i> </code> </p> </li> <li> <p>For an App Runner service: <code>arn:aws:apprunner:<i>region</i>:<i>account-id</i>:service/<i>apprunner-service-name</i>/<i>apprunner-service-id</i> </code> </p> </li> </ul>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the resource to associate with the web ACL. </p> <p>The ARN must be in one of the following formats:</p> <ul> <li> <p>For an Application Load Balancer: <code>arn:<i>partition</i>:elasticloadbalancing:<i>region</i>:<i>account-id</i>:loadbalancer/app/<i>load-balancer-name</i>/<i>load-balancer-id</i> </code> </p> </li> <li> <p>For an Amazon API Gateway REST API: <code>arn:<i>partition</i>:apigateway:<i>region</i>::/restapis/<i>api-id</i>/stages/<i>stage-name</i> </code> </p> </li> <li> <p>For an AppSync GraphQL API: <code>arn:<i>partition</i>:appsync:<i>region</i>:<i>account-id</i>:apis/<i>GraphQLApiId</i> </code> </p> </li> <li> <p>For an Amazon Cognito user pool: <code>arn:<i>partition</i>:cognito-idp:<i>region</i>:<i>account-id</i>:userpool/<i>user-pool-id</i> </code> </p> </li> <li> <p>For an App Runner service: <code>arn:<i>partition</i>:apprunner:<i>region</i>:<i>account-id</i>:service/<i>apprunner-service-name</i>/<i>apprunner-service-id</i> </code> </p> </li> <li> <p>For an Amazon Web Services Verified Access instance: <code>arn:<i>partition</i>:ec2:<i>region</i>:<i>account-id</i>:verified-access-instance/<i>instance-id</i> </code> </p> </li> </ul>",
                     "shape": "ResourceArn"
                 },
                 "WebACLArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the web ACL that you want to associate with the resource.</p>",
                     "shape": "ResourceArn"
                 }
             },
@@ -1692,29 +1925,45 @@
             ],
             "type": "structure"
         },
         "AssociateWebACLResponse": {
             "members": {},
             "type": "structure"
         },
+        "AssociatedResourceType": {
+            "enum": [
+                "CLOUDFRONT"
+            ],
+            "type": "string"
+        },
+        "AssociationConfig": {
+            "documentation": "<p>Specifies custom configurations for the associations between the web ACL and protected resources. </p> <p>Use this to customize the maximum size of the request body that your protected CloudFront distributions forward to WAF for inspection. The default is 16 KB (16,384 kilobytes). </p> <note> <p>You are charged additional fees when your protected resources forward body sizes that are larger than the default. For more information, see <a href=\"http://aws.amazon.com/waf/pricing/\">WAF Pricing</a>.</p> </note>",
+            "members": {
+                "RequestBody": {
+                    "documentation": "<p>Customizes the maximum size of the request body that your protected CloudFront distributions forward to WAF for inspection. The default size is 16 KB (16,384 kilobytes). </p> <note> <p>You are charged additional fees when your protected resources forward body sizes that are larger than the default. For more information, see <a href=\"http://aws.amazon.com/waf/pricing/\">WAF Pricing</a>.</p> </note>",
+                    "shape": "RequestBody"
+                }
+            },
+            "type": "structure"
+        },
         "BlockAction": {
             "documentation": "<p>Specifies that WAF should block the request and optionally defines additional custom handling for the response to the web request.</p> <p>This is used in the context of other settings, for example to specify values for <a>RuleAction</a> and web ACL <a>DefaultAction</a>. </p>",
             "members": {
                 "CustomResponse": {
-                    "documentation": "<p>Defines a custom response for the web request.</p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>Defines a custom response for the web request.</p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomResponse"
                 }
             },
             "type": "structure"
         },
         "Body": {
             "documentation": "<p>Inspect the body of the web request. The body immediately follows the request headers.</p> <p>This is used to indicate the web request component to inspect, in the <a>FieldToMatch</a> specification. </p>",
             "members": {
                 "OversizeHandling": {
-                    "documentation": "<p>What WAF should do if the body is larger than WAF can inspect. WAF does not support inspecting the entire contents of the body of a web request when the body exceeds 8 KB (8192 bytes). Only the first 8 KB of the request body are forwarded to WAF by the underlying host service. </p> <p>The options for oversize handling are the following:</p> <ul> <li> <p> <code>CONTINUE</code> - Inspect the body normally, according to the rule inspection criteria. </p> </li> <li> <p> <code>MATCH</code> - Treat the web request as matching the rule statement. WAF applies the rule action to the request.</p> </li> <li> <p> <code>NO_MATCH</code> - Treat the web request as not matching the rule statement.</p> </li> </ul> <p>You can combine the <code>MATCH</code> or <code>NO_MATCH</code> settings for oversize handling with your rule and web ACL action settings, so that you block any request whose body is over 8 KB. </p> <p>Default: <code>CONTINUE</code> </p>",
+                    "documentation": "<p>What WAF should do if the body is larger than WAF can inspect. WAF does not support inspecting the entire contents of the web request body if the body exceeds the limit for the resource type. If the body is larger than the limit, the underlying host service only forwards the contents that are below the limit to WAF for inspection. </p> <p>The default limit is 8 KB (8,192 kilobytes) for regional resources and 16 KB (16,384 kilobytes) for CloudFront distributions. For CloudFront distributions, you can increase the limit in the web ACL <code>AssociationConfig</code>, for additional processing fees. </p> <p>The options for oversize handling are the following:</p> <ul> <li> <p> <code>CONTINUE</code> - Inspect the available body contents normally, according to the rule inspection criteria. </p> </li> <li> <p> <code>MATCH</code> - Treat the web request as matching the rule statement. WAF applies the rule action to the request.</p> </li> <li> <p> <code>NO_MATCH</code> - Treat the web request as not matching the rule statement.</p> </li> </ul> <p>You can combine the <code>MATCH</code> or <code>NO_MATCH</code> settings for oversize handling with your rule and web ACL action settings, so that you block any request whose body is over the limit. </p> <p>Default: <code>CONTINUE</code> </p>",
                     "shape": "OversizeHandling"
                 }
             },
             "type": "structure"
         },
         "BodyParsingFallbackBehavior": {
             "enum": [
@@ -1735,19 +1984,19 @@
                     "shape": "FieldToMatch"
                 },
                 "PositionalConstraint": {
                     "documentation": "<p>The area within the portion of the web request that you want WAF to search for <code>SearchString</code>. Valid values include the following:</p> <p> <b>CONTAINS</b> </p> <p>The specified part of the web request must include the value of <code>SearchString</code>, but the location doesn't matter.</p> <p> <b>CONTAINS_WORD</b> </p> <p>The specified part of the web request must include the value of <code>SearchString</code>, and <code>SearchString</code> must contain only alphanumeric characters or underscore (A-Z, a-z, 0-9, or _). In addition, <code>SearchString</code> must be a word, which means that both of the following are true:</p> <ul> <li> <p> <code>SearchString</code> is at the beginning of the specified part of the web request or is preceded by a character other than an alphanumeric character or underscore (_). Examples include the value of a header and <code>;BadBot</code>.</p> </li> <li> <p> <code>SearchString</code> is at the end of the specified part of the web request or is followed by a character other than an alphanumeric character or underscore (_), for example, <code>BadBot;</code> and <code>-BadBot;</code>.</p> </li> </ul> <p> <b>EXACTLY</b> </p> <p>The value of the specified part of the web request must exactly match the value of <code>SearchString</code>.</p> <p> <b>STARTS_WITH</b> </p> <p>The value of <code>SearchString</code> must appear at the beginning of the specified part of the web request.</p> <p> <b>ENDS_WITH</b> </p> <p>The value of <code>SearchString</code> must appear at the end of the specified part of the web request.</p>",
                     "shape": "PositionalConstraint"
                 },
                 "SearchString": {
-                    "documentation": "<p>A string value that you want WAF to search for. WAF searches only in the part of web requests that you designate for inspection in <a>FieldToMatch</a>. The maximum length of the value is 200 bytes.</p> <p>Valid values depend on the component that you specify for inspection in <code>FieldToMatch</code>:</p> <ul> <li> <p> <code>Method</code>: The HTTP method that you want WAF to search for. This indicates the type of operation specified in the request. </p> </li> <li> <p> <code>UriPath</code>: The value that you want WAF to search for in the URI path, for example, <code>/images/daily-ad.jpg</code>. </p> </li> </ul> <p>If <code>SearchString</code> includes alphabetic characters A-Z and a-z, note that the value is case sensitive.</p> <p> <b>If you're using the WAF API</b> </p> <p>Specify a base64-encoded version of the value. The maximum length of the value before you base64-encode it is 200 bytes.</p> <p>For example, suppose the value of <code>Type</code> is <code>HEADER</code> and the value of <code>Data</code> is <code>User-Agent</code>. If you want to search the <code>User-Agent</code> header for the value <code>BadBot</code>, you base64-encode <code>BadBot</code> using MIME base64-encoding and include the resulting value, <code>QmFkQm90</code>, in the value of <code>SearchString</code>.</p> <p> <b>If you're using the CLI or one of the Amazon Web Services SDKs</b> </p> <p>The value that you want WAF to search for. The SDK automatically base64 encodes the value.</p>",
+                    "documentation": "<p>A string value that you want WAF to search for. WAF searches only in the part of web requests that you designate for inspection in <a>FieldToMatch</a>. The maximum length of the value is 200 bytes.</p> <p>Valid values depend on the component that you specify for inspection in <code>FieldToMatch</code>:</p> <ul> <li> <p> <code>Method</code>: The HTTP method that you want WAF to search for. This indicates the type of operation specified in the request. </p> </li> <li> <p> <code>UriPath</code>: The value that you want WAF to search for in the URI path, for example, <code>/images/daily-ad.jpg</code>. </p> </li> <li> <p> <code>HeaderOrder</code>: The comma-separated list of header names to match for. WAF creates a string that contains the ordered list of header names, from the headers in the web request, and then matches against that string. </p> </li> </ul> <p>If <code>SearchString</code> includes alphabetic characters A-Z and a-z, note that the value is case sensitive.</p> <p> <b>If you're using the WAF API</b> </p> <p>Specify a base64-encoded version of the value. The maximum length of the value before you base64-encode it is 200 bytes.</p> <p>For example, suppose the value of <code>Type</code> is <code>HEADER</code> and the value of <code>Data</code> is <code>User-Agent</code>. If you want to search the <code>User-Agent</code> header for the value <code>BadBot</code>, you base64-encode <code>BadBot</code> using MIME base64-encoding and include the resulting value, <code>QmFkQm90</code>, in the value of <code>SearchString</code>.</p> <p> <b>If you're using the CLI or one of the Amazon Web Services SDKs</b> </p> <p>The value that you want WAF to search for. The SDK automatically base64 encodes the value.</p>",
                     "shape": "SearchString"
                 },
                 "TextTransformations": {
-                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. If you specify one or more transformations in a rule statement, WAF performs all transformations on the content of the request component identified by <code>FieldToMatch</code>, starting from the lowest priority setting, before inspecting the content for a match.</p>",
+                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. Text transformations are used in rule match statements, to transform the <code>FieldToMatch</code> request component before inspecting it, and they're used in rate-based rule statements, to transform request components before using them as custom aggregation keys. If you specify one or more transformations to apply, WAF performs all transformations on the specified content, starting from the lowest priority setting, and then uses the component contents. </p>",
                     "shape": "TextTransformations"
                 }
             },
             "required": [
                 "SearchString",
                 "FieldToMatch",
                 "TextTransformations",
@@ -1759,15 +2008,15 @@
             "min": 1,
             "type": "long"
         },
         "CaptchaAction": {
             "documentation": "<p>Specifies that WAF should run a <code>CAPTCHA</code> check against the request: </p> <ul> <li> <p>If the request includes a valid, unexpired <code>CAPTCHA</code> token, WAF applies any custom request handling and labels that you've configured and then allows the web request inspection to proceed to the next rule, similar to a <code>CountAction</code>. </p> </li> <li> <p>If the request doesn't include a valid, unexpired token, WAF discontinues the web ACL evaluation of the request and blocks it from going to its intended destination.</p> <p>WAF generates a response that it sends back to the client, which includes the following: </p> <ul> <li> <p>The header <code>x-amzn-waf-action</code> with a value of <code>captcha</code>. </p> </li> <li> <p>The HTTP status code <code>405 Method Not Allowed</code>. </p> </li> <li> <p>If the request contains an <code>Accept</code> header with a value of <code>text/html</code>, the response includes a <code>CAPTCHA</code> JavaScript page interstitial. </p> </li> </ul> </li> </ul> <p>You can configure the expiration time in the <code>CaptchaConfig</code> <code>ImmunityTimeProperty</code> setting at the rule and web ACL level. The rule setting overrides the web ACL setting. </p> <p>This action option is available for rules. It isn't available for web ACL default actions. </p>",
             "members": {
                 "CustomRequestHandling": {
-                    "documentation": "<p>Defines custom handling for the web request, used when the <code>CAPTCHA</code> inspection determines that the request's token is valid and unexpired.</p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>Defines custom handling for the web request, used when the <code>CAPTCHA</code> inspection determines that the request's token is valid and unexpired.</p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomRequestHandling"
                 }
             },
             "type": "structure"
         },
         "CaptchaConfig": {
             "documentation": "<p>Specifies how WAF should handle <code>CAPTCHA</code> evaluations. This is available at the web ACL level and in each rule. </p>",
@@ -1797,15 +2046,15 @@
             },
             "type": "structure"
         },
         "ChallengeAction": {
             "documentation": "<p>Specifies that WAF should run a <code>Challenge</code> check against the request to verify that the request is coming from a legitimate client session: </p> <ul> <li> <p>If the request includes a valid, unexpired challenge token, WAF applies any custom request handling and labels that you've configured and then allows the web request inspection to proceed to the next rule, similar to a <code>CountAction</code>. </p> </li> <li> <p>If the request doesn't include a valid, unexpired challenge token, WAF discontinues the web ACL evaluation of the request and blocks it from going to its intended destination.</p> <p>WAF then generates a challenge response that it sends back to the client, which includes the following: </p> <ul> <li> <p>The header <code>x-amzn-waf-action</code> with a value of <code>challenge</code>. </p> </li> <li> <p>The HTTP status code <code>202 Request Accepted</code>. </p> </li> <li> <p>If the request contains an <code>Accept</code> header with a value of <code>text/html</code>, the response includes a JavaScript page interstitial with a challenge script. </p> </li> </ul> <p>Challenges run silent browser interrogations in the background, and don't generally affect the end user experience. </p> <p>A challenge enforces token acquisition using an interstitial JavaScript challenge that inspects the client session for legitimate behavior. The challenge blocks bots or at least increases the cost of operating sophisticated bots. </p> <p>After the client session successfully responds to the challenge, it receives a new token from WAF, which the challenge script uses to resubmit the original request. </p> </li> </ul> <p>You can configure the expiration time in the <code>ChallengeConfig</code> <code>ImmunityTimeProperty</code> setting at the rule and web ACL level. The rule setting overrides the web ACL setting. </p> <p>This action option is available for rules. It isn't available for web ACL default actions. </p>",
             "members": {
                 "CustomRequestHandling": {
-                    "documentation": "<p>Defines custom handling for the web request, used when the challenge inspection determines that the request's token is valid and unexpired.</p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>Defines custom handling for the web request, used when the challenge inspection determines that the request's token is valid and unexpired.</p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomRequestHandling"
                 }
             },
             "type": "structure"
         },
         "ChallengeConfig": {
             "documentation": "<p>Specifies how WAF should handle <code>Challenge</code> evaluations. This is available at the web ACL level and in each rule. </p>",
@@ -1838,15 +2087,15 @@
         "CheckCapacityRequest": {
             "members": {
                 "Rules": {
                     "documentation": "<p>An array of <a>Rule</a> that you're configuring to use in a rule group or web ACL. </p>",
                     "shape": "Rules"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Scope",
                 "Rules"
             ],
@@ -1931,30 +2180,30 @@
                     "shape": "CookieMatchPattern"
                 },
                 "MatchScope": {
                     "documentation": "<p>The parts of the cookies to inspect with the rule inspection criteria. If you specify <code>All</code>, WAF inspects both keys and values. </p>",
                     "shape": "MapMatchScope"
                 },
                 "OversizeHandling": {
-                    "documentation": "<p>What WAF should do if the cookies of the request are larger than WAF can inspect. WAF does not support inspecting the entire contents of request cookies when they exceed 8 KB (8192 bytes) or 200 total cookies. The underlying host service forwards a maximum of 200 cookies and at most 8 KB of cookie contents to WAF. </p> <p>The options for oversize handling are the following:</p> <ul> <li> <p> <code>CONTINUE</code> - Inspect the cookies normally, according to the rule inspection criteria. </p> </li> <li> <p> <code>MATCH</code> - Treat the web request as matching the rule statement. WAF applies the rule action to the request.</p> </li> <li> <p> <code>NO_MATCH</code> - Treat the web request as not matching the rule statement.</p> </li> </ul>",
+                    "documentation": "<p>What WAF should do if the cookies of the request are more numerous or larger than WAF can inspect. WAF does not support inspecting the entire contents of request cookies when they exceed 8 KB (8192 bytes) or 200 total cookies. The underlying host service forwards a maximum of 200 cookies and at most 8 KB of cookie contents to WAF. </p> <p>The options for oversize handling are the following:</p> <ul> <li> <p> <code>CONTINUE</code> - Inspect the available cookies normally, according to the rule inspection criteria. </p> </li> <li> <p> <code>MATCH</code> - Treat the web request as matching the rule statement. WAF applies the rule action to the request.</p> </li> <li> <p> <code>NO_MATCH</code> - Treat the web request as not matching the rule statement.</p> </li> </ul>",
                     "shape": "OversizeHandling"
                 }
             },
             "required": [
                 "MatchPattern",
                 "MatchScope",
                 "OversizeHandling"
             ],
             "type": "structure"
         },
         "CountAction": {
             "documentation": "<p>Specifies that WAF should count the request. Optionally defines additional custom handling for the request.</p> <p>This is used in the context of other settings, for example to specify values for <a>RuleAction</a> and web ACL <a>DefaultAction</a>. </p>",
             "members": {
                 "CustomRequestHandling": {
-                    "documentation": "<p>Defines custom handling for the web request.</p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>Defines custom handling for the web request.</p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomRequestHandling"
                 }
             },
             "type": "structure"
         },
         "Country": {
             "type": "string"
@@ -2217,14 +2466,40 @@
         "CountryCodes": {
             "member": {
                 "shape": "CountryCode"
             },
             "min": 1,
             "type": "list"
         },
+        "CreateAPIKeyRequest": {
+            "members": {
+                "Scope": {
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "shape": "Scope"
+                },
+                "TokenDomains": {
+                    "documentation": "<p>The client application domains that you want to use this API key for. </p> <p>Example JSON: <code>\"TokenDomains\": [\"abc.com\", \"store.abc.com\"]</code> </p> <p>Public suffixes aren't allowed. For example, you can't use <code>usa.gov</code> or <code>co.uk</code> as token domains.</p>",
+                    "shape": "APIKeyTokenDomains"
+                }
+            },
+            "required": [
+                "Scope",
+                "TokenDomains"
+            ],
+            "type": "structure"
+        },
+        "CreateAPIKeyResponse": {
+            "members": {
+                "APIKey": {
+                    "documentation": "<p>The generated, encrypted API key. You can copy this for use in your JavaScript CAPTCHA integration. </p>",
+                    "shape": "APIKey"
+                }
+            },
+            "type": "structure"
+        },
         "CreateIPSetRequest": {
             "members": {
                 "Addresses": {
                     "documentation": "<p>Contains an array of strings that specifies zero or more IP addresses or blocks of IP addresses. All addresses must be specified using Classless Inter-Domain Routing (CIDR) notation. WAF supports all IPv4 and IPv6 CIDR ranges except for <code>/0</code>. </p> <p>Example address strings: </p> <ul> <li> <p>To configure WAF to allow, block, or count requests that originated from the IP address 192.0.2.44, specify <code>192.0.2.44/32</code>.</p> </li> <li> <p>To configure WAF to allow, block, or count requests that originated from IP addresses from 192.0.2.0 to 192.0.2.255, specify <code>192.0.2.0/24</code>.</p> </li> <li> <p>To configure WAF to allow, block, or count requests that originated from the IP address 1111:0000:0000:0000:0000:0000:0000:0111, specify <code>1111:0000:0000:0000:0000:0000:0000:0111/128</code>.</p> </li> <li> <p>To configure WAF to allow, block, or count requests that originated from IP addresses 1111:0000:0000:0000:0000:0000:0000:0000 to 1111:0000:0000:0000:ffff:ffff:ffff:ffff, specify <code>1111:0000:0000:0000:0000:0000:0000:0000/64</code>.</p> </li> </ul> <p>For more information about CIDR notation, see the Wikipedia entry <a href=\"https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing\">Classless Inter-Domain Routing</a>.</p> <p>Example JSON <code>Addresses</code> specifications: </p> <ul> <li> <p>Empty array: <code>\"Addresses\": []</code> </p> </li> <li> <p>Array with one address: <code>\"Addresses\": [\"192.0.2.44/32\"]</code> </p> </li> <li> <p>Array with three addresses: <code>\"Addresses\": [\"192.0.2.44/32\", \"192.0.2.0/24\", \"192.0.0.0/16\"]</code> </p> </li> <li> <p>INVALID specification: <code>\"Addresses\": [\"\"]</code> INVALID </p> </li> </ul>",
                     "shape": "IPAddresses"
                 },
                 "Description": {
@@ -2236,15 +2511,15 @@
                     "shape": "IPAddressVersion"
                 },
                 "Name": {
                     "documentation": "<p>The name of the IP set. You cannot change the name of an <code>IPSet</code> after you create it.</p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 },
                 "Tags": {
                     "documentation": "<p>An array of key:value pairs to associate with the resource.</p>",
                     "shape": "TagList"
                 }
             },
@@ -2276,15 +2551,15 @@
                     "shape": "EntityName"
                 },
                 "RegularExpressionList": {
                     "documentation": "<p>Array of regular expression strings. </p>",
                     "shape": "RegularExpressionList"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 },
                 "Tags": {
                     "documentation": "<p>An array of key:value pairs to associate with the resource.</p>",
                     "shape": "TagList"
                 }
             },
@@ -2303,19 +2578,19 @@
                 }
             },
             "type": "structure"
         },
         "CreateRuleGroupRequest": {
             "members": {
                 "Capacity": {
-                    "documentation": "<p>The web ACL capacity units (WCUs) required for this rule group.</p> <p>When you create your own rule group, you define this, and you cannot change it after creation. When you add or modify the rules in a rule group, WAF enforces this limit. You can check the capacity for a set of rules using <a>CheckCapacity</a>.</p> <p>WAF uses WCUs to calculate and control the operating resources that are used to run your rules, rule groups, and web ACLs. WAF calculates capacity differently for each rule type, to reflect the relative cost of each rule. Simple rules that cost little to run use fewer WCUs than more complex rules that use more processing power. Rule group capacity is fixed at creation, which helps users plan their web ACL WCU usage when they use a rule group. The WCU limit for web ACLs is 1,500. </p>",
+                    "documentation": "<p>The web ACL capacity units (WCUs) required for this rule group.</p> <p>When you create your own rule group, you define this, and you cannot change it after creation. When you add or modify the rules in a rule group, WAF enforces this limit. You can check the capacity for a set of rules using <a>CheckCapacity</a>.</p> <p>WAF uses WCUs to calculate and control the operating resources that are used to run your rules, rule groups, and web ACLs. WAF calculates capacity differently for each rule type, to reflect the relative cost of each rule. Simple rules that cost little to run use fewer WCUs than more complex rules that use more processing power. Rule group capacity is fixed at creation, which helps users plan their web ACL WCU usage when they use a rule group. For more information, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/aws-waf-capacity-units.html\">WAF web ACL capacity units (WCU)</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CapacityUnit"
                 },
                 "CustomResponseBodies": {
-                    "documentation": "<p>A map of custom response keys and content bodies. When you create a rule with a block action, you can send a custom response to the web request. You define these for the rule group, and then use them in the rules that you define in the rule group. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>A map of custom response keys and content bodies. When you create a rule with a block action, you can send a custom response to the web request. You define these for the rule group, and then use them in the rules that you define in the rule group. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomResponseBodies"
                 },
                 "Description": {
                     "documentation": "<p>A description of the rule group that helps with identification. </p>",
                     "shape": "EntityDescription"
                 },
                 "Name": {
@@ -2323,15 +2598,15 @@
                     "shape": "EntityName"
                 },
                 "Rules": {
                     "documentation": "<p>The <a>Rule</a> statements used to identify the web requests that you want to allow, block, or count. Each rule includes one top-level statement that WAF uses to identify matching web requests, and parameters that govern how WAF handles them. </p>",
                     "shape": "Rules"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 },
                 "Tags": {
                     "documentation": "<p>An array of key:value pairs to associate with the resource.</p>",
                     "shape": "TagList"
                 },
                 "VisibilityConfig": {
@@ -2354,24 +2629,28 @@
                     "shape": "RuleGroupSummary"
                 }
             },
             "type": "structure"
         },
         "CreateWebACLRequest": {
             "members": {
+                "AssociationConfig": {
+                    "documentation": "<p>Specifies custom configurations for the associations between the web ACL and protected resources. </p> <p>Use this to customize the maximum size of the request body that your protected CloudFront distributions forward to WAF for inspection. The default is 16 KB (16,384 kilobytes). </p> <note> <p>You are charged additional fees when your protected resources forward body sizes that are larger than the default. For more information, see <a href=\"http://aws.amazon.com/waf/pricing/\">WAF Pricing</a>.</p> </note>",
+                    "shape": "AssociationConfig"
+                },
                 "CaptchaConfig": {
                     "documentation": "<p>Specifies how WAF should handle <code>CAPTCHA</code> evaluations for rules that don't have their own <code>CaptchaConfig</code> settings. If you don't specify this, WAF uses its default settings for <code>CaptchaConfig</code>. </p>",
                     "shape": "CaptchaConfig"
                 },
                 "ChallengeConfig": {
                     "documentation": "<p>Specifies how WAF should handle challenge evaluations for rules that don't have their own <code>ChallengeConfig</code> settings. If you don't specify this, WAF uses its default settings for <code>ChallengeConfig</code>. </p>",
                     "shape": "ChallengeConfig"
                 },
                 "CustomResponseBodies": {
-                    "documentation": "<p>A map of custom response keys and content bodies. When you create a rule with a block action, you can send a custom response to the web request. You define these for the web ACL, and then use them in the rules and default actions that you define in the web ACL. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>A map of custom response keys and content bodies. When you create a rule with a block action, you can send a custom response to the web request. You define these for the web ACL, and then use them in the rules and default actions that you define in the web ACL. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomResponseBodies"
                 },
                 "DefaultAction": {
                     "documentation": "<p>The action to perform if none of the <code>Rules</code> contained in the <code>WebACL</code> match. </p>",
                     "shape": "DefaultAction"
                 },
                 "Description": {
@@ -2383,15 +2662,15 @@
                     "shape": "EntityName"
                 },
                 "Rules": {
                     "documentation": "<p>The <a>Rule</a> statements used to identify the web requests that you want to allow, block, or count. Each rule includes one top-level statement that WAF uses to identify matching web requests, and parameters that govern how WAF handles them. </p>",
                     "shape": "Rules"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 },
                 "Tags": {
                     "documentation": "<p>An array of key:value pairs to associate with the resource.</p>",
                     "shape": "TagList"
                 },
                 "TokenDomains": {
@@ -2416,14 +2695,20 @@
                 "Summary": {
                     "documentation": "<p>High-level information about a <a>WebACL</a>, returned by operations like create and list. This provides information like the ID, that you can use to retrieve and manage a <code>WebACL</code>, and the ARN, that you provide to operations like <a>AssociateWebACL</a>.</p>",
                     "shape": "WebACLSummary"
                 }
             },
             "type": "structure"
         },
+        "CreationPathString": {
+            "max": 256,
+            "min": 1,
+            "pattern": ".*\\S.*",
+            "type": "string"
+        },
         "CustomHTTPHeader": {
             "documentation": "<p>A custom header for custom request and response handling. This is used in <a>CustomResponse</a> and <a>CustomRequestHandling</a>.</p>",
             "members": {
                 "Name": {
                     "documentation": "<p>The name of the custom header. </p> <p>For custom request header insertion, when WAF inserts the header into the request, it prefixes this name <code>x-amzn-waf-</code>, to avoid confusion with the headers that are already in the request. For example, for the header name <code>sample</code>, WAF inserts the header <code>x-amzn-waf-sample</code>.</p>",
                     "shape": "CustomHTTPHeaderName"
                 },
@@ -2454,39 +2739,39 @@
             "member": {
                 "shape": "CustomHTTPHeader"
             },
             "min": 1,
             "type": "list"
         },
         "CustomRequestHandling": {
-            "documentation": "<p>Custom request handling behavior that inserts custom headers into a web request. You can add custom request handling for WAF to use when the rule action doesn't block the request. For example, <code>CaptchaAction</code> for requests with valid t okens, and <code>AllowAction</code>. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+            "documentation": "<p>Custom request handling behavior that inserts custom headers into a web request. You can add custom request handling for WAF to use when the rule action doesn't block the request. For example, <code>CaptchaAction</code> for requests with valid t okens, and <code>AllowAction</code>. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p>",
             "members": {
                 "InsertHeaders": {
-                    "documentation": "<p>The HTTP headers to insert into the request. Duplicate header names are not allowed. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>The HTTP headers to insert into the request. Duplicate header names are not allowed. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomHTTPHeaders"
                 }
             },
             "required": [
                 "InsertHeaders"
             ],
             "type": "structure"
         },
         "CustomResponse": {
-            "documentation": "<p>A custom response to send to the client. You can define a custom response for rule actions and default web ACL actions that are set to <a>BlockAction</a>. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+            "documentation": "<p>A custom response to send to the client. You can define a custom response for rule actions and default web ACL actions that are set to <a>BlockAction</a>. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p>",
             "members": {
                 "CustomResponseBodyKey": {
                     "documentation": "<p>References the response body that you want WAF to return to the web request client. You can define a custom response for a rule action or a default web ACL action that is set to block. To do this, you first define the response body key and value in the <code>CustomResponseBodies</code> setting for the <a>WebACL</a> or <a>RuleGroup</a> where you want to use it. Then, in the rule action or web ACL default action <code>BlockAction</code> setting, you reference the response body using this key. </p>",
                     "shape": "EntityName"
                 },
                 "ResponseCode": {
-                    "documentation": "<p>The HTTP status code to return to the client. </p> <p>For a list of status codes that you can use in your custom responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/customizing-the-response-status-codes.html\">Supported status codes for custom response</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>The HTTP status code to return to the client. </p> <p>For a list of status codes that you can use in your custom responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/customizing-the-response-status-codes.html\">Supported status codes for custom response</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "ResponseStatusCode"
                 },
                 "ResponseHeaders": {
-                    "documentation": "<p>The HTTP headers to use in the response. Duplicate header names are not allowed. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>The HTTP headers to use in the response. Duplicate header names are not allowed. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomHTTPHeaders"
                 }
             },
             "required": [
                 "ResponseCode"
             ],
             "type": "structure"
@@ -2501,15 +2786,15 @@
                 "shape": "CustomResponseBody"
             }
         },
         "CustomResponseBody": {
             "documentation": "<p>The response body to use in a custom response to a web request. This is referenced by key from <a>CustomResponse</a> <code>CustomResponseBodyKey</code>.</p>",
             "members": {
                 "Content": {
-                    "documentation": "<p>The payload of the custom response. </p> <p>You can use JSON escape strings in JSON content. To do this, you must specify JSON content in the <code>ContentType</code> setting. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>The payload of the custom response. </p> <p>You can use JSON escape strings in JSON content. To do this, you must specify JSON content in the <code>ContentType</code> setting. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "ResponseContent"
                 },
                 "ContentType": {
                     "documentation": "<p>The type of content in the payload that you are defining in the <code>Content</code> string.</p>",
                     "shape": "ResponseContentType"
                 }
             },
@@ -2570,15 +2855,15 @@
                     "shape": "LockToken"
                 },
                 "Name": {
                     "documentation": "<p>The name of the IP set. You cannot change the name of an <code>IPSet</code> after you create it.</p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Name",
                 "Scope",
                 "Id",
@@ -2633,15 +2918,15 @@
                     "shape": "LockToken"
                 },
                 "Name": {
                     "documentation": "<p>The name of the set. You cannot change the name after you create the set.</p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Name",
                 "Scope",
                 "Id",
@@ -2664,15 +2949,15 @@
                     "shape": "LockToken"
                 },
                 "Name": {
                     "documentation": "<p>The name of the rule group. You cannot change the name of a rule group after you create it.</p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Name",
                 "Scope",
                 "Id",
@@ -2695,15 +2980,15 @@
                     "shape": "LockToken"
                 },
                 "Name": {
                     "documentation": "<p>The name of the web ACL. You cannot change the name of a web ACL after you create it.</p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Name",
                 "Scope",
                 "Id",
@@ -2711,26 +2996,73 @@
             ],
             "type": "structure"
         },
         "DeleteWebACLResponse": {
             "members": {},
             "type": "structure"
         },
+        "DescribeAllManagedProductsRequest": {
+            "members": {
+                "Scope": {
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "shape": "Scope"
+                }
+            },
+            "required": [
+                "Scope"
+            ],
+            "type": "structure"
+        },
+        "DescribeAllManagedProductsResponse": {
+            "members": {
+                "ManagedProducts": {
+                    "documentation": "<p>High-level information for the Amazon Web Services Managed Rules rule groups and Amazon Web Services Marketplace managed rule groups. </p>",
+                    "shape": "ManagedProductDescriptors"
+                }
+            },
+            "type": "structure"
+        },
+        "DescribeManagedProductsByVendorRequest": {
+            "members": {
+                "Scope": {
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "shape": "Scope"
+                },
+                "VendorName": {
+                    "documentation": "<p>The name of the managed rule group vendor. You use this, along with the rule group name, to identify a rule group.</p>",
+                    "shape": "VendorName"
+                }
+            },
+            "required": [
+                "VendorName",
+                "Scope"
+            ],
+            "type": "structure"
+        },
+        "DescribeManagedProductsByVendorResponse": {
+            "members": {
+                "ManagedProducts": {
+                    "documentation": "<p>High-level information for the managed rule groups owned by the specified vendor. </p>",
+                    "shape": "ManagedProductDescriptors"
+                }
+            },
+            "type": "structure"
+        },
         "DescribeManagedRuleGroupRequest": {
             "members": {
                 "Name": {
                     "documentation": "<p>The name of the managed rule group. You use this, along with the vendor name, to identify the rule group.</p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 },
                 "VendorName": {
-                    "documentation": "<p>The name of the managed rule group vendor. You use this, along with the rule group name, to identify the rule group.</p>",
+                    "documentation": "<p>The name of the managed rule group vendor. You use this, along with the rule group name, to identify a rule group.</p>",
                     "shape": "VendorName"
                 },
                 "VersionName": {
                     "documentation": "<p>The version of the rule group. You can only use a version that is not scheduled for expiration. If you don't provide this, WAF uses the vendor's default version. </p>",
                     "shape": "VersionKeyString"
                 }
             },
@@ -2744,15 +3076,15 @@
         "DescribeManagedRuleGroupResponse": {
             "members": {
                 "AvailableLabels": {
                     "documentation": "<p>The labels that one or more rules in this rule group add to matching web requests. These labels are defined in the <code>RuleLabels</code> for a <a>Rule</a>.</p>",
                     "shape": "LabelSummaries"
                 },
                 "Capacity": {
-                    "documentation": "<p>The web ACL capacity units (WCUs) required for this rule group. WAF uses web ACL capacity units (WCU) to calculate and control the operating resources that are used to run your rules, rule groups, and web ACLs. WAF calculates capacity differently for each rule type, to reflect each rule's relative cost. Rule group capacity is fixed at creation, so users can plan their web ACL WCU usage when they use a rule group. The WCU limit for web ACLs is 1,500. </p>",
+                    "documentation": "<p>The web ACL capacity units (WCUs) required for this rule group.</p> <p>WAF uses WCUs to calculate and control the operating resources that are used to run your rules, rule groups, and web ACLs. WAF calculates capacity differently for each rule type, to reflect the relative cost of each rule. Simple rules that cost little to run use fewer WCUs than more complex rules that use more processing power. Rule group capacity is fixed at creation, which helps users plan their web ACL WCU usage when they use a rule group. For more information, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/aws-waf-capacity-units.html\">WAF web ACL capacity units (WCU)</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CapacityUnit"
                 },
                 "ConsumedLabels": {
                     "documentation": "<p>The labels that one or more rules in this rule group match against in label match statements. These labels are defined in a <code>LabelMatchStatement</code> specification, in the <a>Statement</a> definition of a rule. </p>",
                     "shape": "LabelSummaries"
                 },
                 "LabelNamespace": {
@@ -2760,28 +3092,28 @@
                     "shape": "LabelName"
                 },
                 "Rules": {
                     "documentation": "<p/>",
                     "shape": "RuleSummaries"
                 },
                 "SnsTopicArn": {
-                    "documentation": "<p>The Amazon resource name (ARN) of the Amazon Simple Notification Service SNS topic that's used to record changes to the managed rule group. You can subscribe to the SNS topic to receive notifications when the managed rule group is modified, such as for new versions and for version expiration. For more information, see the <a href=\"https://docs.aws.amazon.com/sns/latest/dg/welcome.html\">Amazon Simple Notification Service Developer Guide</a>.</p>",
+                    "documentation": "<p>The Amazon resource name (ARN) of the Amazon Simple Notification Service SNS topic that's used to provide notification of changes to the managed rule group. You can subscribe to the SNS topic to receive notifications when the managed rule group is modified, such as for new versions and for version expiration. For more information, see the <a href=\"https://docs.aws.amazon.com/sns/latest/dg/welcome.html\">Amazon Simple Notification Service Developer Guide</a>.</p>",
                     "shape": "ResourceArn"
                 },
                 "VersionName": {
                     "documentation": "<p>The managed rule group's version. </p>",
                     "shape": "VersionKeyString"
                 }
             },
             "type": "structure"
         },
         "DisassociateWebACLRequest": {
             "members": {
                 "ResourceArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the resource to disassociate from the web ACL. </p> <p>The ARN must be in one of the following formats:</p> <ul> <li> <p>For an Application Load Balancer: <code>arn:aws:elasticloadbalancing:<i>region</i>:<i>account-id</i>:loadbalancer/app/<i>load-balancer-name</i>/<i>load-balancer-id</i> </code> </p> </li> <li> <p>For an Amazon API Gateway REST API: <code>arn:aws:apigateway:<i>region</i>::/restapis/<i>api-id</i>/stages/<i>stage-name</i> </code> </p> </li> <li> <p>For an AppSync GraphQL API: <code>arn:aws:appsync:<i>region</i>:<i>account-id</i>:apis/<i>GraphQLApiId</i> </code> </p> </li> <li> <p>For an Amazon Cognito user pool: <code>arn:aws:cognito-idp:<i>region</i>:<i>account-id</i>:userpool/<i>user-pool-id</i> </code> </p> </li> <li> <p>For an App Runner service: <code>arn:aws:apprunner:<i>region</i>:<i>account-id</i>:service/<i>apprunner-service-name</i>/<i>apprunner-service-id</i> </code> </p> </li> </ul>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the resource to disassociate from the web ACL. </p> <p>The ARN must be in one of the following formats:</p> <ul> <li> <p>For an Application Load Balancer: <code>arn:<i>partition</i>:elasticloadbalancing:<i>region</i>:<i>account-id</i>:loadbalancer/app/<i>load-balancer-name</i>/<i>load-balancer-id</i> </code> </p> </li> <li> <p>For an Amazon API Gateway REST API: <code>arn:<i>partition</i>:apigateway:<i>region</i>::/restapis/<i>api-id</i>/stages/<i>stage-name</i> </code> </p> </li> <li> <p>For an AppSync GraphQL API: <code>arn:<i>partition</i>:appsync:<i>region</i>:<i>account-id</i>:apis/<i>GraphQLApiId</i> </code> </p> </li> <li> <p>For an Amazon Cognito user pool: <code>arn:<i>partition</i>:cognito-idp:<i>region</i>:<i>account-id</i>:userpool/<i>user-pool-id</i> </code> </p> </li> <li> <p>For an App Runner service: <code>arn:<i>partition</i>:apprunner:<i>region</i>:<i>account-id</i>:service/<i>apprunner-service-name</i>/<i>apprunner-service-id</i> </code> </p> </li> <li> <p>For an Amazon Web Services Verified Access instance: <code>arn:<i>partition</i>:ec2:<i>region</i>:<i>account-id</i>:verified-access-instance/<i>instance-id</i> </code> </p> </li> </ul>",
                     "shape": "ResourceArn"
                 }
             },
             "required": [
                 "ResourceArn"
             ],
             "type": "structure"
@@ -2789,14 +3121,27 @@
         "DisassociateWebACLResponse": {
             "members": {},
             "type": "structure"
         },
         "DownloadUrl": {
             "type": "string"
         },
+        "EmailField": {
+            "documentation": "<p>The name of the field in the request payload that contains your customer's email. </p> <p>This data type is used in the <code>RequestInspectionACFP</code> data type. </p>",
+            "members": {
+                "Identifier": {
+                    "documentation": "<p>The name of the email field. </p> <p>How you specify this depends on the request inspection payload type.</p> <ul> <li> <p>For JSON payloads, specify the field name in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"form\": { \"email\": \"THE_EMAIL\" } }</code>, the email field specification is <code>/form/email</code>.</p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with the input element named <code>email1</code>, the email field specification is <code>email1</code>.</p> </li> </ul>",
+                    "shape": "FieldIdentifier"
+                }
+            },
+            "required": [
+                "Identifier"
+            ],
+            "type": "structure"
+        },
         "EntityDescription": {
             "max": 256,
             "min": 1,
             "pattern": "^[\\w+=:#@/\\-,\\.][\\w+=:#@/\\-,\\.\\s]+[\\w+=:#@/\\-,\\.]$",
             "type": "string"
         },
         "EntityId": {
@@ -2874,27 +3219,31 @@
             "documentation": "<p>The part of the web request that you want WAF to inspect. Include the single <code>FieldToMatch</code> type that you want to inspect, with additional specifications as needed, according to the type. You specify a single request component in <code>FieldToMatch</code> for each rule statement that requires it. To inspect more than one component of the web request, create a separate rule statement for each component.</p> <p>Example JSON for a <code>QueryString</code> field to match: </p> <p> <code> \"FieldToMatch\": { \"QueryString\": {} }</code> </p> <p>Example JSON for a <code>Method</code> field to match specification:</p> <p> <code> \"FieldToMatch\": { \"Method\": { \"Name\": \"DELETE\" } }</code> </p>",
             "members": {
                 "AllQueryArguments": {
                     "documentation": "<p>Inspect all query arguments. </p>",
                     "shape": "AllQueryArguments"
                 },
                 "Body": {
-                    "documentation": "<p>Inspect the request body as plain text. The request body immediately follows the request headers. This is the part of a request that contains any additional data that you want to send to your web server as the HTTP request body, such as data from a form. </p> <p>Only the first 8 KB (8192 bytes) of the request body are forwarded to WAF for inspection by the underlying host service. For information about how to handle oversized request bodies, see the <code>Body</code> object configuration. </p>",
+                    "documentation": "<p>Inspect the request body as plain text. The request body immediately follows the request headers. This is the part of a request that contains any additional data that you want to send to your web server as the HTTP request body, such as data from a form. </p> <p>A limited amount of the request body is forwarded to WAF for inspection by the underlying host service. For regional resources, the limit is 8 KB (8,192 kilobytes) and for CloudFront distributions, the limit is 16 KB (16,384 kilobytes). For CloudFront distributions, you can increase the limit in the web ACL's <code>AssociationConfig</code>, for additional processing fees. </p> <p>For information about how to handle oversized request bodies, see the <code>Body</code> object configuration. </p>",
                     "shape": "Body"
                 },
                 "Cookies": {
                     "documentation": "<p>Inspect the request cookies. You must configure scope and pattern matching filters in the <code>Cookies</code> object, to define the set of cookies and the parts of the cookies that WAF inspects. </p> <p>Only the first 8 KB (8192 bytes) of a request's cookies and only the first 200 cookies are forwarded to WAF for inspection by the underlying host service. You must configure how to handle any oversize cookie content in the <code>Cookies</code> object. WAF applies the pattern matching filters to the cookies that it receives from the underlying host service. </p>",
                     "shape": "Cookies"
                 },
+                "HeaderOrder": {
+                    "documentation": "<p>Inspect a string containing the list of the request's header names, ordered as they appear in the web request that WAF receives for inspection. WAF generates the string and then uses that as the field to match component in its inspection. WAF separates the header names in the string using colons and no added spaces, for example <code>host:user-agent:accept:authorization:referer</code>.</p>",
+                    "shape": "HeaderOrder"
+                },
                 "Headers": {
                     "documentation": "<p>Inspect the request headers. You must configure scope and pattern matching filters in the <code>Headers</code> object, to define the set of headers to and the parts of the headers that WAF inspects. </p> <p>Only the first 8 KB (8192 bytes) of a request's headers and only the first 200 headers are forwarded to WAF for inspection by the underlying host service. You must configure how to handle any oversize header content in the <code>Headers</code> object. WAF applies the pattern matching filters to the headers that it receives from the underlying host service. </p>",
                     "shape": "Headers"
                 },
                 "JsonBody": {
-                    "documentation": "<p>Inspect the request body as JSON. The request body immediately follows the request headers. This is the part of a request that contains any additional data that you want to send to your web server as the HTTP request body, such as data from a form. </p> <p>Only the first 8 KB (8192 bytes) of the request body are forwarded to WAF for inspection by the underlying host service. For information about how to handle oversized request bodies, see the <code>JsonBody</code> object configuration. </p>",
+                    "documentation": "<p>Inspect the request body as JSON. The request body immediately follows the request headers. This is the part of a request that contains any additional data that you want to send to your web server as the HTTP request body, such as data from a form. </p> <p>A limited amount of the request body is forwarded to WAF for inspection by the underlying host service. For regional resources, the limit is 8 KB (8,192 kilobytes) and for CloudFront distributions, the limit is 16 KB (16,384 kilobytes). For CloudFront distributions, you can increase the limit in the web ACL's <code>AssociationConfig</code>, for additional processing fees. </p> <p>For information about how to handle oversized request bodies, see the <code>JsonBody</code> object configuration. </p>",
                     "shape": "JsonBody"
                 },
                 "Method": {
                     "documentation": "<p>Inspect the HTTP method. The method indicates the type of operation that the request is asking the origin to perform. </p>",
                     "shape": "Method"
                 },
                 "QueryString": {
@@ -3002,22 +3351,22 @@
         "FirewallManagerRuleGroups": {
             "member": {
                 "shape": "FirewallManagerRuleGroup"
             },
             "type": "list"
         },
         "FirewallManagerStatement": {
-            "documentation": "<p>The processing guidance for an Firewall Manager rule. This is like a regular rule <a>Statement</a>, but it can only contain a rule group reference.</p>",
+            "documentation": "<p>The processing guidance for an Firewall Manager rule. This is like a regular rule <a>Statement</a>, but it can only contain a single rule group reference.</p>",
             "members": {
                 "ManagedRuleGroupStatement": {
-                    "documentation": "<p>A rule statement used to run the rules that are defined in a managed rule group. To use this, provide the vendor name and the name of the rule group in this statement. You can retrieve the required names by calling <a>ListAvailableManagedRuleGroups</a>.</p> <p>You cannot nest a <code>ManagedRuleGroupStatement</code>, for example for use inside a <code>NotStatement</code> or <code>OrStatement</code>. It can only be referenced as a top-level statement within a rule.</p> <note> <p>You are charged additional fees when you use the WAF Bot Control managed rule group <code>AWSManagedRulesBotControlRuleSet</code> or the WAF Fraud Control account takeover prevention (ATP) managed rule group <code>AWSManagedRulesATPRuleSet</code>. For more information, see <a href=\"http://aws.amazon.com/waf/pricing/\">WAF Pricing</a>.</p> </note>",
+                    "documentation": "<p>A statement used by Firewall Manager to run the rules that are defined in a managed rule group. This is managed by Firewall Manager for an Firewall Manager WAF policy.</p>",
                     "shape": "ManagedRuleGroupStatement"
                 },
                 "RuleGroupReferenceStatement": {
-                    "documentation": "<p>A rule statement used to run the rules that are defined in a <a>RuleGroup</a>. To use this, create a rule group with your rules, then provide the ARN of the rule group in this statement.</p> <p>You cannot nest a <code>RuleGroupReferenceStatement</code>, for example for use inside a <code>NotStatement</code> or <code>OrStatement</code>. You can only use a rule group reference statement at the top level inside a web ACL. </p>",
+                    "documentation": "<p>A statement used by Firewall Manager to run the rules that are defined in a rule group. This is managed by Firewall Manager for an Firewall Manager WAF policy.</p>",
                     "shape": "RuleGroupReferenceStatement"
                 }
             },
             "type": "structure"
         },
         "ForwardedIPConfig": {
             "documentation": "<p>The configuration for inspecting IP addresses in an HTTP header that you specify, instead of using the IP address that's reported by the web request origin. Commonly, this is the X-Forwarded-For (XFF) header, but you can specify any header name. </p> <note> <p>If the specified header isn't present in the request, WAF doesn't apply the rule to the web request at all.</p> </note> <p>This configuration is used for <a>GeoMatchStatement</a> and <a>RateBasedStatement</a>. For <a>IPSetReferenceStatement</a>, use <a>IPSetForwardedIPConfig</a> instead. </p> <p>WAF only evaluates the first IP address found in the specified HTTP header. </p>",
@@ -3087,26 +3436,56 @@
                 "ForwardedIPConfig": {
                     "documentation": "<p>The configuration for inspecting IP addresses in an HTTP header that you specify, instead of using the IP address that's reported by the web request origin. Commonly, this is the X-Forwarded-For (XFF) header, but you can specify any header name. </p> <note> <p>If the specified header isn't present in the request, WAF doesn't apply the rule to the web request at all.</p> </note>",
                     "shape": "ForwardedIPConfig"
                 }
             },
             "type": "structure"
         },
+        "GetDecryptedAPIKeyRequest": {
+            "members": {
+                "APIKey": {
+                    "documentation": "<p>The encrypted API key. </p>",
+                    "shape": "APIKey"
+                },
+                "Scope": {
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "shape": "Scope"
+                }
+            },
+            "required": [
+                "Scope",
+                "APIKey"
+            ],
+            "type": "structure"
+        },
+        "GetDecryptedAPIKeyResponse": {
+            "members": {
+                "CreationTimestamp": {
+                    "documentation": "<p>The date and time that the key was created. </p>",
+                    "shape": "Timestamp"
+                },
+                "TokenDomains": {
+                    "documentation": "<p>The token domains that are defined in this API key. </p>",
+                    "shape": "TokenDomains"
+                }
+            },
+            "type": "structure"
+        },
         "GetIPSetRequest": {
             "members": {
                 "Id": {
                     "documentation": "<p>A unique identifier for the set. This ID is returned in the responses to create and list commands. You provide it to operations like update and delete.</p>",
                     "shape": "EntityId"
                 },
                 "Name": {
                     "documentation": "<p>The name of the IP set. You cannot change the name of an <code>IPSet</code> after you create it.</p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Name",
                 "Scope",
                 "Id"
@@ -3154,15 +3533,15 @@
                     "shape": "EntityId"
                 },
                 "Name": {
                     "documentation": "<p>The name of the managed rule set. You use this, along with the rule set ID, to identify the rule set.</p> <p>This name is assigned to the corresponding managed rule group, which your customers can access and use. </p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Name",
                 "Scope",
                 "Id"
@@ -3236,15 +3615,15 @@
                     "shape": "EntityName"
                 },
                 "RuleName": {
                     "documentation": "<p>The name of the rate-based rule to get the keys for. If you have the rule defined inside a rule group that you're using in your web ACL, also provide the name of the rule group reference statement in the request parameter <code>RuleGroupRuleName</code>.</p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 },
                 "WebACLId": {
                     "documentation": "<p>The unique identifier for the web ACL. This ID is returned in the responses to create and list commands. You provide it to operations like update and delete.</p>",
                     "shape": "EntityId"
                 },
                 "WebACLName": {
@@ -3280,15 +3659,15 @@
                     "shape": "EntityId"
                 },
                 "Name": {
                     "documentation": "<p>The name of the set. You cannot change the name after you create the set.</p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Name",
                 "Scope",
                 "Id"
@@ -3319,15 +3698,15 @@
                     "shape": "EntityId"
                 },
                 "Name": {
                     "documentation": "<p>The name of the rule group. You cannot change the name of a rule group after you create it.</p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "type": "structure"
         },
         "GetRuleGroupResponse": {
             "members": {
@@ -3349,15 +3728,15 @@
                     "shape": "ListMaxItems"
                 },
                 "RuleMetricName": {
                     "documentation": "<p>The metric name assigned to the <code>Rule</code> or <code>RuleGroup</code> dimension for which you want a sample of requests.</p>",
                     "shape": "MetricName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 },
                 "TimeWindow": {
                     "documentation": "<p>The start date and time and the end date and time of the range for which you want <code>GetSampledRequests</code> to return a sample of requests. You must specify the times in Coordinated Universal Time (UTC) format. UTC format includes the special designator, <code>Z</code>. For example, <code>\"2016-09-27T14:50Z\"</code>. You can specify any time range in the previous three hours. If you specify a start time that's earlier than three hours ago, WAF sets it to three hours ago.</p>",
                     "shape": "TimeWindow"
                 },
                 "WebAclArn": {
@@ -3390,15 +3769,15 @@
                 }
             },
             "type": "structure"
         },
         "GetWebACLForResourceRequest": {
             "members": {
                 "ResourceArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the resource whose web ACL you want to retrieve. </p> <p>The ARN must be in one of the following formats:</p> <ul> <li> <p>For an Application Load Balancer: <code>arn:aws:elasticloadbalancing:<i>region</i>:<i>account-id</i>:loadbalancer/app/<i>load-balancer-name</i>/<i>load-balancer-id</i> </code> </p> </li> <li> <p>For an Amazon API Gateway REST API: <code>arn:aws:apigateway:<i>region</i>::/restapis/<i>api-id</i>/stages/<i>stage-name</i> </code> </p> </li> <li> <p>For an AppSync GraphQL API: <code>arn:aws:appsync:<i>region</i>:<i>account-id</i>:apis/<i>GraphQLApiId</i> </code> </p> </li> <li> <p>For an Amazon Cognito user pool: <code>arn:aws:cognito-idp:<i>region</i>:<i>account-id</i>:userpool/<i>user-pool-id</i> </code> </p> </li> <li> <p>For an App Runner service: <code>arn:aws:apprunner:<i>region</i>:<i>account-id</i>:service/<i>apprunner-service-name</i>/<i>apprunner-service-id</i> </code> </p> </li> </ul>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the resource whose web ACL you want to retrieve. </p> <p>The ARN must be in one of the following formats:</p> <ul> <li> <p>For an Application Load Balancer: <code>arn:<i>partition</i>:elasticloadbalancing:<i>region</i>:<i>account-id</i>:loadbalancer/app/<i>load-balancer-name</i>/<i>load-balancer-id</i> </code> </p> </li> <li> <p>For an Amazon API Gateway REST API: <code>arn:<i>partition</i>:apigateway:<i>region</i>::/restapis/<i>api-id</i>/stages/<i>stage-name</i> </code> </p> </li> <li> <p>For an AppSync GraphQL API: <code>arn:<i>partition</i>:appsync:<i>region</i>:<i>account-id</i>:apis/<i>GraphQLApiId</i> </code> </p> </li> <li> <p>For an Amazon Cognito user pool: <code>arn:<i>partition</i>:cognito-idp:<i>region</i>:<i>account-id</i>:userpool/<i>user-pool-id</i> </code> </p> </li> <li> <p>For an App Runner service: <code>arn:<i>partition</i>:apprunner:<i>region</i>:<i>account-id</i>:service/<i>apprunner-service-name</i>/<i>apprunner-service-id</i> </code> </p> </li> <li> <p>For an Amazon Web Services Verified Access instance: <code>arn:<i>partition</i>:ec2:<i>region</i>:<i>account-id</i>:verified-access-instance/<i>instance-id</i> </code> </p> </li> </ul>",
                     "shape": "ResourceArn"
                 }
             },
             "required": [
                 "ResourceArn"
             ],
             "type": "structure"
@@ -3419,29 +3798,29 @@
                     "shape": "EntityId"
                 },
                 "Name": {
                     "documentation": "<p>The name of the web ACL. You cannot change the name of a web ACL after you create it.</p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Name",
                 "Scope",
                 "Id"
             ],
             "type": "structure"
         },
         "GetWebACLResponse": {
             "members": {
                 "ApplicationIntegrationURL": {
-                    "documentation": "<p>The URL to use in SDK integrations with Amazon Web Services managed rule groups. For example, you can use the integration SDKs with the account takeover prevention managed rule group <code>AWSManagedRulesATPRuleSet</code>. This is only populated if you are using a rule group in your web ACL that integrates with your applications in this way. For more information, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-application-integration.html\">WAF client application integration</a> in the <i>WAF Developer Guide</i>.</p>",
+                    "documentation": "<p>The URL to use in SDK integrations with Amazon Web Services managed rule groups. For example, you can use the integration SDKs with the account takeover prevention managed rule group <code>AWSManagedRulesATPRuleSet</code> and the account creation fraud prevention managed rule group <code>AWSManagedRulesACFPRuleSet</code>. This is only populated if you are using a rule group in your web ACL that integrates with your applications in this way. For more information, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-application-integration.html\">WAF client application integration</a> in the <i>WAF Developer Guide</i>.</p>",
                     "shape": "OutputUrl"
                 },
                 "LockToken": {
                     "documentation": "<p>A token used for optimistic locking. WAF returns a token to your <code>get</code> and <code>list</code> requests, to mark the state of the entity at the time of the request. To make changes to the entity associated with the token, you provide the token to operations like <code>update</code> and <code>delete</code>. WAF uses the token to ensure that no changes have been made to the entity since you last retrieved it. If a change has been made, the update fails with a <code>WAFOptimisticLockException</code>. If this happens, perform another <code>get</code>, and use the new token returned by that operation. </p>",
                     "shape": "LockToken"
                 },
                 "WebACL": {
@@ -3532,14 +3911,27 @@
             "max": 199,
             "member": {
                 "shape": "FieldToMatchData"
             },
             "min": 1,
             "type": "list"
         },
+        "HeaderOrder": {
+            "documentation": "<p>Inspect a string containing the list of the request's header names, ordered as they appear in the web request that WAF receives for inspection. WAF generates the string and then uses that as the field to match component in its inspection. WAF separates the header names in the string using colons and no added spaces, for example <code>host:user-agent:accept:authorization:referer</code>.</p>",
+            "members": {
+                "OversizeHandling": {
+                    "documentation": "<p>What WAF should do if the headers of the request are more numerous or larger than WAF can inspect. WAF does not support inspecting the entire contents of request headers when they exceed 8 KB (8192 bytes) or 200 total headers. The underlying host service forwards a maximum of 200 headers and at most 8 KB of header contents to WAF. </p> <p>The options for oversize handling are the following:</p> <ul> <li> <p> <code>CONTINUE</code> - Inspect the available headers normally, according to the rule inspection criteria. </p> </li> <li> <p> <code>MATCH</code> - Treat the web request as matching the rule statement. WAF applies the rule action to the request.</p> </li> <li> <p> <code>NO_MATCH</code> - Treat the web request as not matching the rule statement.</p> </li> </ul>",
+                    "shape": "OversizeHandling"
+                }
+            },
+            "required": [
+                "OversizeHandling"
+            ],
+            "type": "structure"
+        },
         "HeaderValue": {
             "type": "string"
         },
         "Headers": {
             "documentation": "<p>Inspect all headers in the web request. You can specify the parts of the headers to inspect and you can narrow the set of headers to inspect by including or excluding specific keys.</p> <p>This is used to indicate the web request component to inspect, in the <a>FieldToMatch</a> specification. </p> <p>If you want to inspect just the value of a single header, use the <code>SingleHeader</code> <code>FieldToMatch</code> setting instead.</p> <p>Example JSON: <code>\"Headers\": { \"MatchPattern\": { \"All\": {} }, \"MatchScope\": \"KEY\", \"OversizeHandling\": \"MATCH\" }</code> </p>",
             "members": {
                 "MatchPattern": {
@@ -3547,15 +3939,15 @@
                     "shape": "HeaderMatchPattern"
                 },
                 "MatchScope": {
                     "documentation": "<p>The parts of the headers to match with the rule inspection criteria. If you specify <code>All</code>, WAF inspects both keys and values. </p>",
                     "shape": "MapMatchScope"
                 },
                 "OversizeHandling": {
-                    "documentation": "<p>What WAF should do if the headers of the request are larger than WAF can inspect. WAF does not support inspecting the entire contents of request headers when they exceed 8 KB (8192 bytes) or 200 total headers. The underlying host service forwards a maximum of 200 headers and at most 8 KB of header contents to WAF. </p> <p>The options for oversize handling are the following:</p> <ul> <li> <p> <code>CONTINUE</code> - Inspect the headers normally, according to the rule inspection criteria. </p> </li> <li> <p> <code>MATCH</code> - Treat the web request as matching the rule statement. WAF applies the rule action to the request.</p> </li> <li> <p> <code>NO_MATCH</code> - Treat the web request as not matching the rule statement.</p> </li> </ul>",
+                    "documentation": "<p>What WAF should do if the headers of the request are more numerous or larger than WAF can inspect. WAF does not support inspecting the entire contents of request headers when they exceed 8 KB (8192 bytes) or 200 total headers. The underlying host service forwards a maximum of 200 headers and at most 8 KB of header contents to WAF. </p> <p>The options for oversize handling are the following:</p> <ul> <li> <p> <code>CONTINUE</code> - Inspect the available headers normally, according to the rule inspection criteria. </p> </li> <li> <p> <code>MATCH</code> - Treat the web request as matching the rule statement. WAF applies the rule action to the request.</p> </li> <li> <p> <code>NO_MATCH</code> - Treat the web request as not matching the rule statement.</p> </li> </ul>",
                     "shape": "OversizeHandling"
                 }
             },
             "required": [
                 "MatchPattern",
                 "MatchScope",
                 "OversizeHandling"
@@ -3725,15 +4117,15 @@
                     "shape": "JsonMatchPattern"
                 },
                 "MatchScope": {
                     "documentation": "<p>The parts of the JSON to match against using the <code>MatchPattern</code>. If you specify <code>All</code>, WAF matches against keys and values. </p>",
                     "shape": "JsonMatchScope"
                 },
                 "OversizeHandling": {
-                    "documentation": "<p>What WAF should do if the body is larger than WAF can inspect. WAF does not support inspecting the entire contents of the body of a web request when the body exceeds 8 KB (8192 bytes). Only the first 8 KB of the request body are forwarded to WAF by the underlying host service. </p> <p>The options for oversize handling are the following:</p> <ul> <li> <p> <code>CONTINUE</code> - Inspect the body normally, according to the rule inspection criteria. </p> </li> <li> <p> <code>MATCH</code> - Treat the web request as matching the rule statement. WAF applies the rule action to the request.</p> </li> <li> <p> <code>NO_MATCH</code> - Treat the web request as not matching the rule statement.</p> </li> </ul> <p>You can combine the <code>MATCH</code> or <code>NO_MATCH</code> settings for oversize handling with your rule and web ACL action settings, so that you block any request whose body is over 8 KB. </p> <p>Default: <code>CONTINUE</code> </p>",
+                    "documentation": "<p>What WAF should do if the body is larger than WAF can inspect. WAF does not support inspecting the entire contents of the web request body if the body exceeds the limit for the resource type. If the body is larger than the limit, the underlying host service only forwards the contents that are below the limit to WAF for inspection. </p> <p>The default limit is 8 KB (8,192 kilobytes) for regional resources and 16 KB (16,384 kilobytes) for CloudFront distributions. For CloudFront distributions, you can increase the limit in the web ACL <code>AssociationConfig</code>, for additional processing fees. </p> <p>The options for oversize handling are the following:</p> <ul> <li> <p> <code>CONTINUE</code> - Inspect the available body contents normally, according to the rule inspection criteria. </p> </li> <li> <p> <code>MATCH</code> - Treat the web request as matching the rule statement. WAF applies the rule action to the request.</p> </li> <li> <p> <code>NO_MATCH</code> - Treat the web request as not matching the rule statement.</p> </li> </ul> <p>You can combine the <code>MATCH</code> or <code>NO_MATCH</code> settings for oversize handling with your rule and web ACL action settings, so that you block any request whose body is over the limit. </p> <p>Default: <code>CONTINUE</code> </p>",
                     "shape": "OversizeHandling"
                 }
             },
             "required": [
                 "MatchPattern",
                 "MatchScope"
             ],
@@ -3833,14 +4225,20 @@
                 }
             },
             "required": [
                 "LabelName"
             ],
             "type": "structure"
         },
+        "LabelNamespace": {
+            "max": 1024,
+            "min": 1,
+            "pattern": "^[0-9A-Za-z_\\-:]+:$",
+            "type": "string"
+        },
         "LabelSummaries": {
             "member": {
                 "shape": "LabelSummary"
             },
             "type": "list"
         },
         "LabelSummary": {
@@ -3855,14 +4253,51 @@
         },
         "Labels": {
             "member": {
                 "shape": "Label"
             },
             "type": "list"
         },
+        "ListAPIKeysRequest": {
+            "members": {
+                "Limit": {
+                    "documentation": "<p>The maximum number of objects that you want WAF to return for this request. If more objects are available, in the response, WAF provides a <code>NextMarker</code> value that you can use in a subsequent call to get the next batch of objects.</p>",
+                    "shape": "PaginationLimit"
+                },
+                "NextMarker": {
+                    "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
+                    "shape": "NextMarker"
+                },
+                "Scope": {
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "shape": "Scope"
+                }
+            },
+            "required": [
+                "Scope"
+            ],
+            "type": "structure"
+        },
+        "ListAPIKeysResponse": {
+            "members": {
+                "APIKeySummaries": {
+                    "documentation": "<p>The array of key summaries. If you specified a <code>Limit</code> in your request, this might not be the full list. </p>",
+                    "shape": "APIKeySummaries"
+                },
+                "ApplicationIntegrationURL": {
+                    "documentation": "<p>The CAPTCHA application integration URL, for use in your JavaScript implementation. </p>",
+                    "shape": "OutputUrl"
+                },
+                "NextMarker": {
+                    "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
+                    "shape": "NextMarker"
+                }
+            },
+            "type": "structure"
+        },
         "ListAvailableManagedRuleGroupVersionsRequest": {
             "members": {
                 "Limit": {
                     "documentation": "<p>The maximum number of objects that you want WAF to return for this request. If more objects are available, in the response, WAF provides a <code>NextMarker</code> value that you can use in a subsequent call to get the next batch of objects.</p>",
                     "shape": "PaginationLimit"
                 },
                 "Name": {
@@ -3870,19 +4305,19 @@
                     "shape": "EntityName"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 },
                 "VendorName": {
-                    "documentation": "<p>The name of the managed rule group vendor. You use this, along with the rule group name, to identify the rule group.</p>",
+                    "documentation": "<p>The name of the managed rule group vendor. You use this, along with the rule group name, to identify a rule group.</p>",
                     "shape": "VendorName"
                 }
             },
             "required": [
                 "VendorName",
                 "Name",
                 "Scope"
@@ -3896,15 +4331,15 @@
                     "shape": "VersionKeyString"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "Versions": {
-                    "documentation": "<p>The versions that are currently available for the specified managed rule group. </p>",
+                    "documentation": "<p>The versions that are currently available for the specified managed rule group. If you specified a <code>Limit</code> in your request, this might not be the full list. </p>",
                     "shape": "ManagedRuleGroupVersions"
                 }
             },
             "type": "structure"
         },
         "ListAvailableManagedRuleGroupsRequest": {
             "members": {
@@ -3913,27 +4348,27 @@
                     "shape": "PaginationLimit"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Scope"
             ],
             "type": "structure"
         },
         "ListAvailableManagedRuleGroupsResponse": {
             "members": {
                 "ManagedRuleGroups": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Array of managed rule groups that you can use. If you specified a <code>Limit</code> in your request, this might not be the full list. </p>",
                     "shape": "ManagedRuleGroupSummaries"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 }
             },
@@ -3946,27 +4381,27 @@
                     "shape": "PaginationLimit"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Scope"
             ],
             "type": "structure"
         },
         "ListIPSetsResponse": {
             "members": {
                 "IPSets": {
-                    "documentation": "<p>Array of IPSets. This may not be the full list of IPSets that you have defined. See the <code>Limit</code> specification for this request.</p>",
+                    "documentation": "<p>Array of IPSets. If you specified a <code>Limit</code> in your request, this might not be the full list. </p>",
                     "shape": "IPSetSummaries"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 }
             },
@@ -3979,27 +4414,27 @@
                     "shape": "PaginationLimit"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Scope"
             ],
             "type": "structure"
         },
         "ListLoggingConfigurationsResponse": {
             "members": {
                 "LoggingConfigurations": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Array of logging configurations. If you specified a <code>Limit</code> in your request, this might not be the full list. </p>",
                     "shape": "LoggingConfigurations"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 }
             },
@@ -4012,27 +4447,27 @@
                     "shape": "PaginationLimit"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Scope"
             ],
             "type": "structure"
         },
         "ListManagedRuleSetsResponse": {
             "members": {
                 "ManagedRuleSets": {
-                    "documentation": "<p>Your managed rule sets. </p>",
+                    "documentation": "<p>Your managed rule sets. If you specified a <code>Limit</code> in your request, this might not be the full list. </p>",
                     "shape": "ManagedRuleSetSummaries"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 }
             },
@@ -4066,15 +4501,15 @@
         "ListMobileSdkReleasesResponse": {
             "members": {
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "ReleaseSummaries": {
-                    "documentation": "<p>High level information for the available SDK releases. </p>",
+                    "documentation": "<p>The high level information for the available SDK releases. If you specified a <code>Limit</code> in your request, this might not be the full list. </p>",
                     "shape": "ReleaseSummaries"
                 }
             },
             "type": "structure"
         },
         "ListRegexPatternSetsRequest": {
             "members": {
@@ -4083,15 +4518,15 @@
                     "shape": "PaginationLimit"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Scope"
             ],
             "type": "structure"
@@ -4099,24 +4534,24 @@
         "ListRegexPatternSetsResponse": {
             "members": {
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "RegexPatternSets": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Array of regex pattern sets. If you specified a <code>Limit</code> in your request, this might not be the full list. </p>",
                     "shape": "RegexPatternSetSummaries"
                 }
             },
             "type": "structure"
         },
         "ListResourcesForWebACLRequest": {
             "members": {
                 "ResourceType": {
-                    "documentation": "<p>Used for web ACLs that are scoped for regional applications. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <note> <p>If you don't provide a resource type, the call uses the resource type <code>APPLICATION_LOAD_BALANCER</code>. </p> </note> <p>Default: <code>APPLICATION_LOAD_BALANCER</code> </p>",
+                    "documentation": "<p>Used for web ACLs that are scoped for regional applications. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <note> <p>If you don't provide a resource type, the call uses the resource type <code>APPLICATION_LOAD_BALANCER</code>. </p> </note> <p>Default: <code>APPLICATION_LOAD_BALANCER</code> </p>",
                     "shape": "ResourceType"
                 },
                 "WebACLArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the web ACL.</p>",
                     "shape": "ResourceArn"
                 }
             },
@@ -4141,15 +4576,15 @@
                     "shape": "PaginationLimit"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Scope"
             ],
             "type": "structure"
@@ -4157,15 +4592,15 @@
         "ListRuleGroupsResponse": {
             "members": {
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "RuleGroups": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Array of rule groups. If you specified a <code>Limit</code> in your request, this might not be the full list. </p>",
                     "shape": "RuleGroupSummaries"
                 }
             },
             "type": "structure"
         },
         "ListTagsForResourceRequest": {
             "members": {
@@ -4190,15 +4625,15 @@
         "ListTagsForResourceResponse": {
             "members": {
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "TagInfoForResource": {
-                    "documentation": "<p>The collection of tagging definitions for the resource. </p>",
+                    "documentation": "<p>The collection of tagging definitions for the resource. If you specified a <code>Limit</code> in your request, this might not be the full list. </p>",
                     "shape": "TagInfoForResource"
                 }
             },
             "type": "structure"
         },
         "ListWebACLsRequest": {
             "members": {
@@ -4207,15 +4642,15 @@
                     "shape": "PaginationLimit"
                 },
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Scope"
             ],
             "type": "structure"
@@ -4223,15 +4658,15 @@
         "ListWebACLsResponse": {
             "members": {
                 "NextMarker": {
                     "documentation": "<p>When you request a list of objects with a <code>Limit</code> setting, if the number of objects that are still available for retrieval exceeds the limit, WAF returns a <code>NextMarker</code> value in the response. To retrieve the next batch of objects, provide the marker from the prior call in your next request.</p>",
                     "shape": "NextMarker"
                 },
                 "WebACLs": {
-                    "documentation": "<p/>",
+                    "documentation": "<p>Array of web ACLs. If you specified a <code>Limit</code> in your request, this might not be the full list. </p>",
                     "shape": "WebACLSummaries"
                 }
             },
             "type": "structure"
         },
         "LockToken": {
             "max": 36,
@@ -4259,15 +4694,15 @@
                     "shape": "LoggingFilter"
                 },
                 "ManagedByFirewallManager": {
                     "documentation": "<p>Indicates whether the logging configuration was created by Firewall Manager, as part of an WAF policy configuration. If true, only Firewall Manager can modify or delete the configuration. </p>",
                     "shape": "Boolean"
                 },
                 "RedactedFields": {
-                    "documentation": "<p>The parts of the request that you want to keep out of the logs. For example, if you redact the <code>SingleHeader</code> field, the <code>HEADER</code> field in the logs will be <code>REDACTED</code>. </p> <note> <p>You can specify only the following fields for redaction: <code>UriPath</code>, <code>QueryString</code>, <code>SingleHeader</code>, <code>Method</code>, and <code>JsonBody</code>.</p> </note>",
+                    "documentation": "<p>The parts of the request that you want to keep out of the logs.</p> <p>For example, if you redact the <code>SingleHeader</code> field, the <code>HEADER</code> field in the logs will be <code>REDACTED</code> for all rules that use the <code>SingleHeader</code> <code>FieldToMatch</code> setting. </p> <p>Redaction applies only to the component that's specified in the rule's <code>FieldToMatch</code> setting, so the <code>SingleHeader</code> redaction doesn't apply to rules that use the <code>Headers</code> <code>FieldToMatch</code>.</p> <note> <p>You can specify only the following fields for redaction: <code>UriPath</code>, <code>QueryString</code>, <code>SingleHeader</code>, and <code>Method</code>.</p> </note>",
                     "shape": "RedactedFields"
                 },
                 "ResourceArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the web ACL that you want to associate with <code>LogDestinationConfigs</code>.</p>",
                     "shape": "ResourceArn"
                 }
             },
@@ -4303,17 +4738,69 @@
         },
         "LoginPathString": {
             "max": 256,
             "min": 1,
             "pattern": ".*\\S.*",
             "type": "string"
         },
+        "ManagedProductDescriptor": {
+            "documentation": "<p>The properties of a managed product, such as an Amazon Web Services Managed Rules rule group or an Amazon Web Services Marketplace managed rule group. </p>",
+            "members": {
+                "IsAdvancedManagedRuleSet": {
+                    "documentation": "<p>Indicates whether the rule group provides an advanced set of protections, such as the the Amazon Web Services Managed Rules rule groups that are used for WAF intelligent threat mitigation. </p>",
+                    "shape": "Boolean"
+                },
+                "IsVersioningSupported": {
+                    "documentation": "<p>Indicates whether the rule group is versioned. </p>",
+                    "shape": "Boolean"
+                },
+                "ManagedRuleSetName": {
+                    "documentation": "<p>The name of the managed rule group. For example, <code>AWSManagedRulesAnonymousIpList</code> or <code>AWSManagedRulesATPRuleSet</code>.</p>",
+                    "shape": "EntityName"
+                },
+                "ProductDescription": {
+                    "documentation": "<p>A short description of the managed rule group.</p>",
+                    "shape": "ProductDescription"
+                },
+                "ProductId": {
+                    "documentation": "<p>A unique identifier for the rule group. This ID is returned in the responses to create and list commands. You provide it to operations like update and delete.</p>",
+                    "shape": "ProductId"
+                },
+                "ProductLink": {
+                    "documentation": "<p>For Amazon Web Services Marketplace managed rule groups only, the link to the rule group product page. </p>",
+                    "shape": "ProductLink"
+                },
+                "ProductTitle": {
+                    "documentation": "<p>The display name for the managed rule group. For example, <code>Anonymous IP list</code> or <code>Account takeover prevention</code>.</p>",
+                    "shape": "ProductTitle"
+                },
+                "SnsTopicArn": {
+                    "documentation": "<p>The Amazon resource name (ARN) of the Amazon Simple Notification Service SNS topic that's used to provide notification of changes to the managed rule group. You can subscribe to the SNS topic to receive notifications when the managed rule group is modified, such as for new versions and for version expiration. For more information, see the <a href=\"https://docs.aws.amazon.com/sns/latest/dg/welcome.html\">Amazon Simple Notification Service Developer Guide</a>.</p>",
+                    "shape": "ResourceArn"
+                },
+                "VendorName": {
+                    "documentation": "<p>The name of the managed rule group vendor. You use this, along with the rule group name, to identify a rule group.</p>",
+                    "shape": "VendorName"
+                }
+            },
+            "type": "structure"
+        },
+        "ManagedProductDescriptors": {
+            "member": {
+                "shape": "ManagedProductDescriptor"
+            },
+            "type": "list"
+        },
         "ManagedRuleGroupConfig": {
-            "documentation": "<p>Additional information that's used by a managed rule group. Many managed rule groups don't require this.</p> <p>Use the <code>AWSManagedRulesATPRuleSet</code> configuration object for the account takeover prevention managed rule group, to provide information such as the sign-in page of your application and the type of content to accept or reject from the client. </p> <p>Use the <code>AWSManagedRulesBotControlRuleSet</code> configuration object to configure the protection level that you want the Bot Control rule group to use. </p> <p>For example specifications, see the examples section of <a>CreateWebACL</a>.</p>",
+            "documentation": "<p>Additional information that's used by a managed rule group. Many managed rule groups don't require this.</p> <p>The rule groups used for intelligent threat mitigation require additional configuration: </p> <ul> <li> <p>Use the <code>AWSManagedRulesACFPRuleSet</code> configuration object to configure the account creation fraud prevention managed rule group. The configuration includes the registration and sign-up pages of your application and the locations in the account creation request payload of data, such as the user email and phone number fields. </p> </li> <li> <p>Use the <code>AWSManagedRulesATPRuleSet</code> configuration object to configure the account takeover prevention managed rule group. The configuration includes the sign-in page of your application and the locations in the login request payload of data such as the username and password. </p> </li> <li> <p>Use the <code>AWSManagedRulesBotControlRuleSet</code> configuration object to configure the protection level that you want the Bot Control rule group to use. </p> </li> </ul> <p>For example specifications, see the examples section of <a>CreateWebACL</a>.</p>",
             "members": {
+                "AWSManagedRulesACFPRuleSet": {
+                    "documentation": "<p>Additional configuration for using the account creation fraud prevention (ACFP) managed rule group, <code>AWSManagedRulesACFPRuleSet</code>. Use this to provide account creation request information to the rule group. For web ACLs that protect CloudFront distributions, use this to also provide the information about how your distribution responds to account creation requests. </p> <p>For information about using the ACFP managed rule group, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/aws-managed-rule-groups-acfp.html\">WAF Fraud Control account creation fraud prevention (ACFP) rule group</a> and <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-acfp.html\">WAF Fraud Control account creation fraud prevention (ACFP)</a> in the <i>WAF Developer Guide</i>.</p>",
+                    "shape": "AWSManagedRulesACFPRuleSet"
+                },
                 "AWSManagedRulesATPRuleSet": {
                     "documentation": "<p>Additional configuration for using the account takeover prevention (ATP) managed rule group, <code>AWSManagedRulesATPRuleSet</code>. Use this to provide login request information to the rule group. For web ACLs that protect CloudFront distributions, use this to also provide the information about how your distribution responds to login requests. </p> <p>This configuration replaces the individual configuration fields in <code>ManagedRuleGroupConfig</code> and provides additional feature configuration. </p> <p>For information about using the ATP managed rule group, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/aws-managed-rule-groups-atp.html\">WAF Fraud Control account takeover prevention (ATP) rule group</a> and <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-atp.html\">WAF Fraud Control account takeover prevention (ATP)</a> in the <i>WAF Developer Guide</i>.</p>",
                     "shape": "AWSManagedRulesATPRuleSet"
                 },
                 "AWSManagedRulesBotControlRuleSet": {
                     "documentation": "<p>Additional configuration for using the Bot Control managed rule group. Use this to specify the inspection level that you want to use. For information about using the Bot Control managed rule group, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/aws-managed-rule-groups-bot.html\">WAF Bot Control rule group</a> and <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-bot-control.html\">WAF Bot Control</a> in the <i>WAF Developer Guide</i>.</p>",
                     "shape": "AWSManagedRulesBotControlRuleSet"
@@ -4323,47 +4810,47 @@
                     "deprecatedMessage": "Deprecated. Use AWSManagedRulesATPRuleSet LoginPath",
                     "documentation": "<note> <p>Instead of this setting, provide your configuration under <code>AWSManagedRulesATPRuleSet</code>. </p> </note>",
                     "shape": "LoginPathString"
                 },
                 "PasswordField": {
                     "deprecated": true,
                     "deprecatedMessage": "Deprecated. Use AWSManagedRulesATPRuleSet RequestInspection PasswordField",
-                    "documentation": "<note> <p>Instead of this setting, provide your configuration under <code>AWSManagedRulesATPRuleSet</code> <code>RequestInspection</code>. </p> </note>",
+                    "documentation": "<note> <p>Instead of this setting, provide your configuration under the request inspection configuration for <code>AWSManagedRulesATPRuleSet</code> or <code>AWSManagedRulesACFPRuleSet</code>. </p> </note>",
                     "shape": "PasswordField"
                 },
                 "PayloadType": {
                     "deprecated": true,
                     "deprecatedMessage": "Deprecated. Use AWSManagedRulesATPRuleSet RequestInspection PayloadType",
-                    "documentation": "<note> <p>Instead of this setting, provide your configuration under <code>AWSManagedRulesATPRuleSet</code> <code>RequestInspection</code>. </p> </note>",
+                    "documentation": "<note> <p>Instead of this setting, provide your configuration under the request inspection configuration for <code>AWSManagedRulesATPRuleSet</code> or <code>AWSManagedRulesACFPRuleSet</code>. </p> </note>",
                     "shape": "PayloadType"
                 },
                 "UsernameField": {
                     "deprecated": true,
                     "deprecatedMessage": "Deprecated. Use AWSManagedRulesATPRuleSet RequestInspection UsernameField",
-                    "documentation": "<note> <p>Instead of this setting, provide your configuration under <code>AWSManagedRulesATPRuleSet</code> <code>RequestInspection</code>. </p> </note>",
+                    "documentation": "<note> <p>Instead of this setting, provide your configuration under the request inspection configuration for <code>AWSManagedRulesATPRuleSet</code> or <code>AWSManagedRulesACFPRuleSet</code>. </p> </note>",
                     "shape": "UsernameField"
                 }
             },
             "type": "structure"
         },
         "ManagedRuleGroupConfigs": {
             "member": {
                 "shape": "ManagedRuleGroupConfig"
             },
             "type": "list"
         },
         "ManagedRuleGroupStatement": {
-            "documentation": "<p>A rule statement used to run the rules that are defined in a managed rule group. To use this, provide the vendor name and the name of the rule group in this statement. You can retrieve the required names by calling <a>ListAvailableManagedRuleGroups</a>.</p> <p>You cannot nest a <code>ManagedRuleGroupStatement</code>, for example for use inside a <code>NotStatement</code> or <code>OrStatement</code>. It can only be referenced as a top-level statement within a rule.</p> <note> <p>You are charged additional fees when you use the WAF Bot Control managed rule group <code>AWSManagedRulesBotControlRuleSet</code> or the WAF Fraud Control account takeover prevention (ATP) managed rule group <code>AWSManagedRulesATPRuleSet</code>. For more information, see <a href=\"http://aws.amazon.com/waf/pricing/\">WAF Pricing</a>.</p> </note>",
+            "documentation": "<p>A rule statement used to run the rules that are defined in a managed rule group. To use this, provide the vendor name and the name of the rule group in this statement. You can retrieve the required names by calling <a>ListAvailableManagedRuleGroups</a>.</p> <p>You cannot nest a <code>ManagedRuleGroupStatement</code>, for example for use inside a <code>NotStatement</code> or <code>OrStatement</code>. It can only be referenced as a top-level statement within a rule.</p> <note> <p>You are charged additional fees when you use the WAF Bot Control managed rule group <code>AWSManagedRulesBotControlRuleSet</code>, the WAF Fraud Control account takeover prevention (ATP) managed rule group <code>AWSManagedRulesATPRuleSet</code>, or the WAF Fraud Control account creation fraud prevention (ACFP) managed rule group <code>AWSManagedRulesACFPRuleSet</code>. For more information, see <a href=\"http://aws.amazon.com/waf/pricing/\">WAF Pricing</a>.</p> </note>",
             "members": {
                 "ExcludedRules": {
                     "documentation": "<p>Rules in the referenced rule group whose actions are set to <code>Count</code>. </p> <note> <p>Instead of this option, use <code>RuleActionOverrides</code>. It accepts any valid action setting, including <code>Count</code>.</p> </note>",
                     "shape": "ExcludedRules"
                 },
                 "ManagedRuleGroupConfigs": {
-                    "documentation": "<p>Additional information that's used by a managed rule group. Many managed rule groups don't require this.</p> <p>Use the <code>AWSManagedRulesATPRuleSet</code> configuration object for the account takeover prevention managed rule group, to provide information such as the sign-in page of your application and the type of content to accept or reject from the client. </p> <p>Use the <code>AWSManagedRulesBotControlRuleSet</code> configuration object to configure the protection level that you want the Bot Control rule group to use. </p>",
+                    "documentation": "<p>Additional information that's used by a managed rule group. Many managed rule groups don't require this.</p> <p>The rule groups used for intelligent threat mitigation require additional configuration: </p> <ul> <li> <p>Use the <code>AWSManagedRulesACFPRuleSet</code> configuration object to configure the account creation fraud prevention managed rule group. The configuration includes the registration and sign-up pages of your application and the locations in the account creation request payload of data, such as the user email and phone number fields. </p> </li> <li> <p>Use the <code>AWSManagedRulesATPRuleSet</code> configuration object to configure the account takeover prevention managed rule group. The configuration includes the sign-in page of your application and the locations in the login request payload of data such as the username and password. </p> </li> <li> <p>Use the <code>AWSManagedRulesBotControlRuleSet</code> configuration object to configure the protection level that you want the Bot Control rule group to use. </p> </li> </ul>",
                     "shape": "ManagedRuleGroupConfigs"
                 },
                 "Name": {
                     "documentation": "<p>The name of the managed rule group. You use this, along with the vendor name, to identify the rule group.</p>",
                     "shape": "EntityName"
                 },
                 "RuleActionOverrides": {
@@ -4371,15 +4858,15 @@
                     "shape": "RuleActionOverrides"
                 },
                 "ScopeDownStatement": {
                     "documentation": "<p>An optional nested statement that narrows the scope of the web requests that are evaluated by the managed rule group. Requests are only evaluated by the rule group if they match the scope-down statement. You can use any nestable <a>Statement</a> in the scope-down statement, and you can nest statements at any level, the same as you can for a rule statement. </p>",
                     "shape": "Statement"
                 },
                 "VendorName": {
-                    "documentation": "<p>The name of the managed rule group vendor. You use this, along with the rule group name, to identify the rule group.</p>",
+                    "documentation": "<p>The name of the managed rule group vendor. You use this, along with the rule group name, to identify a rule group.</p>",
                     "shape": "VendorName"
                 },
                 "Version": {
                     "documentation": "<p>The version of the managed rule group to use. If you specify this, the version setting is fixed until you change it. If you don't specify this, WAF uses the vendor's default version, and then keeps the version at the vendor's default when the vendor updates the managed rule group settings. </p>",
                     "shape": "VersionKeyString"
                 }
             },
@@ -4392,26 +4879,26 @@
         "ManagedRuleGroupSummaries": {
             "member": {
                 "shape": "ManagedRuleGroupSummary"
             },
             "type": "list"
         },
         "ManagedRuleGroupSummary": {
-            "documentation": "<p>High-level information about a managed rule group, returned by <a>ListAvailableManagedRuleGroups</a>. This provides information like the name and vendor name, that you provide when you add a <a>ManagedRuleGroupStatement</a> to a web ACL. Managed rule groups include Amazon Web Services Managed Rules rule groups, which are free of charge to WAF customers, and Amazon Web Services Marketplace managed rule groups, which you can subscribe to through Amazon Web Services Marketplace. </p>",
+            "documentation": "<p>High-level information about a managed rule group, returned by <a>ListAvailableManagedRuleGroups</a>. This provides information like the name and vendor name, that you provide when you add a <a>ManagedRuleGroupStatement</a> to a web ACL. Managed rule groups include Amazon Web Services Managed Rules rule groups and Amazon Web Services Marketplace managed rule groups. To use any Amazon Web Services Marketplace managed rule group, first subscribe to the rule group through Amazon Web Services Marketplace. </p>",
             "members": {
                 "Description": {
                     "documentation": "<p>The description of the managed rule group, provided by Amazon Web Services Managed Rules or the Amazon Web Services Marketplace seller who manages it.</p>",
                     "shape": "EntityDescription"
                 },
                 "Name": {
                     "documentation": "<p>The name of the managed rule group. You use this, along with the vendor name, to identify the rule group.</p>",
                     "shape": "EntityName"
                 },
                 "VendorName": {
-                    "documentation": "<p>The name of the managed rule group vendor. You use this, along with the rule group name, to identify the rule group.</p>",
+                    "documentation": "<p>The name of the managed rule group vendor. You use this, along with the rule group name, to identify a rule group.</p>",
                     "shape": "VendorName"
                 },
                 "VersioningSupported": {
                     "documentation": "<p>Indicates whether the managed rule group is versioned. If it is, you can retrieve the versions list by calling <a>ListAvailableManagedRuleGroupVersions</a>. </p>",
                     "shape": "Boolean"
                 }
             },
@@ -4516,15 +5003,15 @@
             "documentation": "<p>Information for a single version of a managed rule set. </p> <note> <p>This is intended for use only by vendors of managed rule sets. Vendors are Amazon Web Services and Amazon Web Services Marketplace sellers. </p> <p>Vendors, you can use the managed rule set APIs to provide controlled rollout of your versioned managed rule group offerings for your customers. The APIs are <code>ListManagedRuleSets</code>, <code>GetManagedRuleSet</code>, <code>PutManagedRuleSetVersions</code>, and <code>UpdateManagedRuleSetVersionExpiryDate</code>.</p> </note>",
             "members": {
                 "AssociatedRuleGroupArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the vendor rule group that's used to define the published version of your managed rule group. </p>",
                     "shape": "ResourceArn"
                 },
                 "Capacity": {
-                    "documentation": "<p>The web ACL capacity units (WCUs) required for this rule group.</p> <p>WAF uses WCUs to calculate and control the operating resources that are used to run your rules, rule groups, and web ACLs. WAF calculates capacity differently for each rule type, to reflect the relative cost of each rule. Simple rules that cost little to run use fewer WCUs than more complex rules that use more processing power. Rule group capacity is fixed at creation, which helps users plan their web ACL WCU usage when they use a rule group. The WCU limit for web ACLs is 1,500. </p>",
+                    "documentation": "<p>The web ACL capacity units (WCUs) required for this rule group.</p> <p>WAF uses WCUs to calculate and control the operating resources that are used to run your rules, rule groups, and web ACLs. WAF calculates capacity differently for each rule type, to reflect the relative cost of each rule. Simple rules that cost little to run use fewer WCUs than more complex rules that use more processing power. Rule group capacity is fixed at creation, which helps users plan their web ACL WCU usage when they use a rule group. For more information, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/aws-waf-capacity-units.html\">WAF web ACL capacity units (WCU)</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CapacityUnit"
                 },
                 "ExpiryTimestamp": {
                     "documentation": "<p>The time that this version is set to expire.</p> <p>Times are in Coordinated Universal Time (UTC) format. UTC format includes the special designator, Z. For example, \"2016-09-27T14:50Z\". </p>",
                     "shape": "Timestamp"
                 },
                 "ForecastedLifetime": {
@@ -4547,15 +5034,15 @@
                 "ALL",
                 "KEY",
                 "VALUE"
             ],
             "type": "string"
         },
         "Method": {
-            "documentation": "<p>Inspect the HTTP method of the web request. The method indicates the type of operation that the request is asking the origin to perform. </p> <p>This is used only in the <a>FieldToMatch</a> specification for some web request component types. </p> <p>JSON specification: <code>\"Method\": {}</code> </p>",
+            "documentation": "<p>Inspect the HTTP method of the web request. The method indicates the type of operation that the request is asking the origin to perform. </p> <p>This is used in the <a>FieldToMatch</a> specification for some web request component types. </p> <p>JSON specification: <code>\"Method\": {}</code> </p>",
             "members": {},
             "type": "structure"
         },
         "MetricName": {
             "max": 255,
             "min": 1,
             "pattern": "^[\\w#:\\.\\-/]+$",
@@ -4713,27 +5200,31 @@
                 "PAYLOAD_TYPE",
                 "HEADER_MATCH_PATTERN",
                 "COOKIE_MATCH_PATTERN",
                 "MAP_MATCH_SCOPE",
                 "OVERSIZE_HANDLING",
                 "CHALLENGE_CONFIG",
                 "TOKEN_DOMAIN",
-                "ATP_RULE_SET_RESPONSE_INSPECTION"
+                "ATP_RULE_SET_RESPONSE_INSPECTION",
+                "ASSOCIATED_RESOURCE_TYPE",
+                "SCOPE_DOWN",
+                "CUSTOM_KEYS",
+                "ACP_RULE_SET_RESPONSE_INSPECTION"
             ],
             "type": "string"
         },
         "ParameterExceptionParameter": {
             "min": 1,
             "type": "string"
         },
         "PasswordField": {
-            "documentation": "<p>Details about your login page password field for request inspection, used in the <code>AWSManagedRulesATPRuleSet</code> <code>RequestInspection</code> configuration.</p>",
+            "documentation": "<p>The name of the field in the request payload that contains your customer's password. </p> <p>This data type is used in the <code>RequestInspection</code> and <code>RequestInspectionACFP</code> data types. </p>",
             "members": {
                 "Identifier": {
-                    "documentation": "<p>The name of the password field. For example <code>/form/password</code>.</p>",
+                    "documentation": "<p>The name of the password field. </p> <p>How you specify this depends on the request inspection payload type.</p> <ul> <li> <p>For JSON payloads, specify the field name in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"form\": { \"password\": \"THE_PASSWORD\" } }</code>, the password field specification is <code>/form/password</code>.</p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with the input element named <code>password1</code>, the password field specification is <code>password1</code>.</p> </li> </ul>",
                     "shape": "FieldIdentifier"
                 }
             },
             "required": [
                 "Identifier"
             ],
             "type": "structure"
@@ -4741,14 +5232,33 @@
         "PayloadType": {
             "enum": [
                 "JSON",
                 "FORM_ENCODED"
             ],
             "type": "string"
         },
+        "PhoneNumberField": {
+            "documentation": "<p>The name of a field in the request payload that contains part or all of your customer's primary phone number. </p> <p>This data type is used in the <code>RequestInspectionACFP</code> data type. </p>",
+            "members": {
+                "Identifier": {
+                    "documentation": "<p>The name of a single primary phone number field. </p> <p>How you specify the phone number fields depends on the request inspection payload type.</p> <ul> <li> <p>For JSON payloads, specify the field identifiers in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"form\": { \"primaryphoneline1\": \"THE_PHONE1\", \"primaryphoneline2\": \"THE_PHONE2\", \"primaryphoneline3\": \"THE_PHONE3\" } }</code>, the phone number field identifiers are <code>/form/primaryphoneline1</code>, <code>/form/primaryphoneline2</code>, and <code>/form/primaryphoneline3</code>.</p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with input elements named <code>primaryphoneline1</code>, <code>primaryphoneline2</code>, and <code>primaryphoneline3</code>, the phone number field identifiers are <code>primaryphoneline1</code>, <code>primaryphoneline2</code>, and <code>primaryphoneline3</code>. </p> </li> </ul>",
+                    "shape": "FieldIdentifier"
+                }
+            },
+            "required": [
+                "Identifier"
+            ],
+            "type": "structure"
+        },
+        "PhoneNumberFields": {
+            "member": {
+                "shape": "PhoneNumberField"
+            },
+            "type": "list"
+        },
         "Platform": {
             "enum": [
                 "IOS",
                 "ANDROID"
             ],
             "type": "string"
         },
@@ -4767,14 +5277,36 @@
                 "STARTS_WITH",
                 "ENDS_WITH",
                 "CONTAINS",
                 "CONTAINS_WORD"
             ],
             "type": "string"
         },
+        "ProductDescription": {
+            "min": 1,
+            "pattern": ".*\\S.*",
+            "type": "string"
+        },
+        "ProductId": {
+            "max": 128,
+            "min": 1,
+            "pattern": ".*\\S.*",
+            "type": "string"
+        },
+        "ProductLink": {
+            "max": 2048,
+            "min": 1,
+            "pattern": ".*\\S.*",
+            "type": "string"
+        },
+        "ProductTitle": {
+            "min": 1,
+            "pattern": ".*\\S.*",
+            "type": "string"
+        },
         "PublishedVersions": {
             "key": {
                 "shape": "VersionKeyString"
             },
             "type": "map",
             "value": {
                 "shape": "ManagedRuleSetVersion"
@@ -4816,15 +5348,15 @@
                     "shape": "EntityName"
                 },
                 "RecommendedVersion": {
                     "documentation": "<p>The version of the named managed rule group that you'd like your customers to choose, from among your version offerings. </p>",
                     "shape": "VersionKeyString"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 },
                 "VersionsToPublish": {
                     "documentation": "<p>The versions of the named managed rule group that you want to offer to your customers. </p>",
                     "shape": "VersionsToPublish"
                 }
             },
@@ -4844,15 +5376,15 @@
                 }
             },
             "type": "structure"
         },
         "PutPermissionPolicyRequest": {
             "members": {
                 "Policy": {
-                    "documentation": "<p>The policy to attach to the specified rule group. </p> <p>The policy specifications must conform to the following:</p> <ul> <li> <p>The policy must be composed using IAM Policy version 2012-10-17 or version 2015-01-01.</p> </li> <li> <p>The policy must include specifications for <code>Effect</code>, <code>Action</code>, and <code>Principal</code>.</p> </li> <li> <p> <code>Effect</code> must specify <code>Allow</code>.</p> </li> <li> <p> <code>Action</code> must specify <code>wafv2:CreateWebACL</code>, <code>wafv2:UpdateWebACL</code>, and <code>wafv2:PutFirewallManagerRuleGroups</code> and may optionally specify <code>wafv2:GetRuleGroup</code>. WAF rejects any extra actions or wildcard actions in the policy.</p> </li> <li> <p>The policy must not include a <code>Resource</code> parameter.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html\">IAM Policies</a>. </p>",
+                    "documentation": "<p>The policy to attach to the specified rule group. </p> <p>The policy specifications must conform to the following:</p> <ul> <li> <p>The policy must be composed using IAM Policy version 2012-10-17.</p> </li> <li> <p>The policy must include specifications for <code>Effect</code>, <code>Action</code>, and <code>Principal</code>.</p> </li> <li> <p> <code>Effect</code> must specify <code>Allow</code>.</p> </li> <li> <p> <code>Action</code> must specify <code>wafv2:CreateWebACL</code>, <code>wafv2:UpdateWebACL</code>, and <code>wafv2:PutFirewallManagerRuleGroups</code> and may optionally specify <code>wafv2:GetRuleGroup</code>. WAF rejects any extra actions or wildcard actions in the policy.</p> </li> <li> <p>The policy must not include a <code>Resource</code> parameter.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html\">IAM Policies</a>. </p>",
                     "shape": "PolicyString"
                 },
                 "ResourceArn": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the <a>RuleGroup</a> to which you want to attach the policy.</p>",
                     "shape": "ResourceArn"
                 }
             },
@@ -4863,53 +5395,105 @@
             "type": "structure"
         },
         "PutPermissionPolicyResponse": {
             "members": {},
             "type": "structure"
         },
         "QueryString": {
-            "documentation": "<p>Inspect the query string of the web request. This is the part of a URL that appears after a <code>?</code> character, if any.</p> <p>This is used only in the <a>FieldToMatch</a> specification for some web request component types. </p> <p>JSON specification: <code>\"QueryString\": {}</code> </p>",
+            "documentation": "<p>Inspect the query string of the web request. This is the part of a URL that appears after a <code>?</code> character, if any.</p> <p>This is used in the <a>FieldToMatch</a> specification for some web request component types. </p> <p>JSON specification: <code>\"QueryString\": {}</code> </p>",
             "members": {},
             "type": "structure"
         },
         "RateBasedStatement": {
-            "documentation": "<p>A rate-based rule tracks the rate of requests for each originating IP address, and triggers the rule action when the rate exceeds a limit that you specify on the number of requests in any 5-minute time span. You can use this to put a temporary block on requests from an IP address that is sending excessive requests. </p> <p>WAF tracks and manages web requests separately for each instance of a rate-based rule that you use. For example, if you provide the same rate-based rule settings in two web ACLs, each of the two rule statements represents a separate instance of the rate-based rule and gets its own tracking and management by WAF. If you define a rate-based rule inside a rule group, and then use that rule group in multiple places, each use creates a separate instance of the rate-based rule that gets its own tracking and management by WAF. </p> <p>When the rule action triggers, WAF blocks additional requests from the IP address until the request rate falls below the limit.</p> <p>You can optionally nest another statement inside the rate-based statement, to narrow the scope of the rule so that it only counts requests that match the nested statement. For example, based on recent requests that you have seen from an attacker, you might create a rate-based rule with a nested AND rule statement that contains the following nested statements:</p> <ul> <li> <p>An IP match statement with an IP set that specifies the address 192.0.2.44.</p> </li> <li> <p>A string match statement that searches in the User-Agent header for the string BadBot.</p> </li> </ul> <p>In this rate-based rule, you also define a rate limit. For this example, the rate limit is 1,000. Requests that meet the criteria of both of the nested statements are counted. If the count exceeds 1,000 requests per five minutes, the rule action triggers. Requests that do not meet the criteria of both of the nested statements are not counted towards the rate limit and are not affected by this rule.</p> <p>You cannot nest a <code>RateBasedStatement</code> inside another statement, for example inside a <code>NotStatement</code> or <code>OrStatement</code>. You can define a <code>RateBasedStatement</code> inside a web ACL and inside a rule group. </p>",
+            "documentation": "<p>A rate-based rule counts incoming requests and rate limits requests when they are coming at too fast a rate. The rule categorizes requests according to your aggregation criteria, collects them into aggregation instances, and counts and rate limits the requests for each instance. </p> <p>You can specify individual aggregation keys, like IP address or HTTP method. You can also specify aggregation key combinations, like IP address and HTTP method, or HTTP method, query argument, and cookie. </p> <p>Each unique set of values for the aggregation keys that you specify is a separate aggregation instance, with the value from each key contributing to the aggregation instance definition. </p> <p>For example, assume the rule evaluates web requests with the following IP address and HTTP method values: </p> <ul> <li> <p>IP address 10.1.1.1, HTTP method POST</p> </li> <li> <p>IP address 10.1.1.1, HTTP method GET</p> </li> <li> <p>IP address 127.0.0.0, HTTP method POST</p> </li> <li> <p>IP address 10.1.1.1, HTTP method GET</p> </li> </ul> <p>The rule would create different aggregation instances according to your aggregation criteria, for example: </p> <ul> <li> <p>If the aggregation criteria is just the IP address, then each individual address is an aggregation instance, and WAF counts requests separately for each. The aggregation instances and request counts for our example would be the following: </p> <ul> <li> <p>IP address 10.1.1.1: count 3</p> </li> <li> <p>IP address 127.0.0.0: count 1</p> </li> </ul> </li> <li> <p>If the aggregation criteria is HTTP method, then each individual HTTP method is an aggregation instance. The aggregation instances and request counts for our example would be the following: </p> <ul> <li> <p>HTTP method POST: count 2</p> </li> <li> <p>HTTP method GET: count 2</p> </li> </ul> </li> <li> <p>If the aggregation criteria is IP address and HTTP method, then each IP address and each HTTP method would contribute to the combined aggregation instance. The aggregation instances and request counts for our example would be the following: </p> <ul> <li> <p>IP address 10.1.1.1, HTTP method POST: count 1</p> </li> <li> <p>IP address 10.1.1.1, HTTP method GET: count 2</p> </li> <li> <p>IP address 127.0.0.0, HTTP method POST: count 1</p> </li> </ul> </li> </ul> <p>For any n-tuple of aggregation keys, each unique combination of values for the keys defines a separate aggregation instance, which WAF counts and rate-limits individually. </p> <p>You can optionally nest another statement inside the rate-based statement, to narrow the scope of the rule so that it only counts and rate limits requests that match the nested statement. You can use this nested scope-down statement in conjunction with your aggregation key specifications or you can just count and rate limit all requests that match the scope-down statement, without additional aggregation. When you choose to just manage all requests that match a scope-down statement, the aggregation instance is singular for the rule. </p> <p>You cannot nest a <code>RateBasedStatement</code> inside another statement, for example inside a <code>NotStatement</code> or <code>OrStatement</code>. You can define a <code>RateBasedStatement</code> inside a web ACL and inside a rule group. </p> <p>For additional information about the options, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-rate-based-rules.html\">Rate limiting web requests using rate-based rules</a> in the <i>WAF Developer Guide</i>. </p> <p>If you only aggregate on the individual IP address or forwarded IP address, you can retrieve the list of IP addresses that WAF is currently rate limiting for a rule through the API call <code>GetRateBasedStatementManagedKeys</code>. This option is not available for other aggregation configurations.</p> <p>WAF tracks and manages web requests separately for each instance of a rate-based rule that you use. For example, if you provide the same rate-based rule settings in two web ACLs, each of the two rule statements represents a separate instance of the rate-based rule and gets its own tracking and management by WAF. If you define a rate-based rule inside a rule group, and then use that rule group in multiple places, each use creates a separate instance of the rate-based rule that gets its own tracking and management by WAF. </p>",
             "members": {
                 "AggregateKeyType": {
-                    "documentation": "<p>Setting that indicates how to aggregate the request counts. The options are the following:</p> <ul> <li> <p>IP - Aggregate the request counts on the IP address from the web request origin.</p> </li> <li> <p>FORWARDED_IP - Aggregate the request counts on the first IP address in an HTTP header. If you use this, configure the <code>ForwardedIPConfig</code>, to specify the header to use. </p> </li> </ul>",
+                    "documentation": "<p>Setting that indicates how to aggregate the request counts. </p> <note> <p>Web requests that are missing any of the components specified in the aggregation keys are omitted from the rate-based rule evaluation and handling. </p> </note> <ul> <li> <p> <code>CONSTANT</code> - Count and limit the requests that match the rate-based rule's scope-down statement. With this option, the counted requests aren't further aggregated. The scope-down statement is the only specification used. When the count of all requests that satisfy the scope-down statement goes over the limit, WAF applies the rule action to all requests that satisfy the scope-down statement. </p> <p>With this option, you must configure the <code>ScopeDownStatement</code> property. </p> </li> <li> <p> <code>CUSTOM_KEYS</code> - Aggregate the request counts using one or more web request components as the aggregate keys.</p> <p>With this option, you must specify the aggregate keys in the <code>CustomKeys</code> property. </p> <p>To aggregate on only the IP address or only the forwarded IP address, don't use custom keys. Instead, set the aggregate key type to <code>IP</code> or <code>FORWARDED_IP</code>.</p> </li> <li> <p> <code>FORWARDED_IP</code> - Aggregate the request counts on the first IP address in an HTTP header. </p> <p>With this option, you must specify the header to use in the <code>ForwardedIPConfig</code> property. </p> <p>To aggregate on a combination of the forwarded IP address with other aggregate keys, use <code>CUSTOM_KEYS</code>. </p> </li> <li> <p> <code>IP</code> - Aggregate the request counts on the IP address from the web request origin.</p> <p>To aggregate on a combination of the IP address with other aggregate keys, use <code>CUSTOM_KEYS</code>. </p> </li> </ul>",
                     "shape": "RateBasedStatementAggregateKeyType"
                 },
+                "CustomKeys": {
+                    "documentation": "<p>Specifies the aggregate keys to use in a rate-base rule. </p>",
+                    "shape": "RateBasedStatementCustomKeys"
+                },
                 "ForwardedIPConfig": {
-                    "documentation": "<p>The configuration for inspecting IP addresses in an HTTP header that you specify, instead of using the IP address that's reported by the web request origin. Commonly, this is the X-Forwarded-For (XFF) header, but you can specify any header name. </p> <note> <p>If the specified header isn't present in the request, WAF doesn't apply the rule to the web request at all.</p> </note> <p>This is required if <code>AggregateKeyType</code> is set to <code>FORWARDED_IP</code>.</p>",
+                    "documentation": "<p>The configuration for inspecting IP addresses in an HTTP header that you specify, instead of using the IP address that's reported by the web request origin. Commonly, this is the X-Forwarded-For (XFF) header, but you can specify any header name. </p> <note> <p>If the specified header isn't present in the request, WAF doesn't apply the rule to the web request at all.</p> </note> <p>This is required if you specify a forwarded IP in the rule's aggregate key settings. </p>",
                     "shape": "ForwardedIPConfig"
                 },
                 "Limit": {
-                    "documentation": "<p>The limit on requests per 5-minute period for a single originating IP address. If the statement includes a <code>ScopeDownStatement</code>, this limit is applied only to the requests that match the statement.</p>",
+                    "documentation": "<p>The limit on requests per 5-minute period for a single aggregation instance for the rate-based rule. If the rate-based statement includes a <code>ScopeDownStatement</code>, this limit is applied only to the requests that match the statement.</p> <p>Examples: </p> <ul> <li> <p>If you aggregate on just the IP address, this is the limit on requests from any single IP address. </p> </li> <li> <p>If you aggregate on the HTTP method and the query argument name \"city\", then this is the limit on requests for any single method, city pair. </p> </li> </ul>",
                     "shape": "RateLimit"
                 },
                 "ScopeDownStatement": {
-                    "documentation": "<p>An optional nested statement that narrows the scope of the web requests that are evaluated by the rate-based statement. Requests are only tracked by the rate-based statement if they match the scope-down statement. You can use any nestable <a>Statement</a> in the scope-down statement, and you can nest statements at any level, the same as you can for a rule statement. </p>",
+                    "documentation": "<p>An optional nested statement that narrows the scope of the web requests that are evaluated and managed by the rate-based statement. When you use a scope-down statement, the rate-based rule only tracks and rate limits requests that match the scope-down statement. You can use any nestable <a>Statement</a> in the scope-down statement, and you can nest statements at any level, the same as you can for a rule statement. </p>",
                     "shape": "Statement"
                 }
             },
             "required": [
                 "Limit",
                 "AggregateKeyType"
             ],
             "type": "structure"
         },
         "RateBasedStatementAggregateKeyType": {
             "enum": [
                 "IP",
-                "FORWARDED_IP"
+                "FORWARDED_IP",
+                "CUSTOM_KEYS",
+                "CONSTANT"
             ],
             "type": "string"
         },
+        "RateBasedStatementCustomKey": {
+            "documentation": "<p>Specifies a single custom aggregate key for a rate-base rule. </p> <note> <p>Web requests that are missing any of the components specified in the aggregation keys are omitted from the rate-based rule evaluation and handling. </p> </note>",
+            "members": {
+                "Cookie": {
+                    "documentation": "<p>Use the value of a cookie in the request as an aggregate key. Each distinct value in the cookie contributes to the aggregation instance. If you use a single cookie as your custom key, then each value fully defines an aggregation instance. </p>",
+                    "shape": "RateLimitCookie"
+                },
+                "ForwardedIP": {
+                    "documentation": "<p>Use the first IP address in an HTTP header as an aggregate key. Each distinct forwarded IP address contributes to the aggregation instance.</p> <p>When you specify an IP or forwarded IP in the custom key settings, you must also specify at least one other key to use. You can aggregate on only the forwarded IP address by specifying <code>FORWARDED_IP</code> in your rate-based statement's <code>AggregateKeyType</code>. </p> <p>With this option, you must specify the header to use in the rate-based rule's <code>ForwardedIPConfig</code> property. </p>",
+                    "shape": "RateLimitForwardedIP"
+                },
+                "HTTPMethod": {
+                    "documentation": "<p>Use the request's HTTP method as an aggregate key. Each distinct HTTP method contributes to the aggregation instance. If you use just the HTTP method as your custom key, then each method fully defines an aggregation instance. </p>",
+                    "shape": "RateLimitHTTPMethod"
+                },
+                "Header": {
+                    "documentation": "<p>Use the value of a header in the request as an aggregate key. Each distinct value in the header contributes to the aggregation instance. If you use a single header as your custom key, then each value fully defines an aggregation instance. </p>",
+                    "shape": "RateLimitHeader"
+                },
+                "IP": {
+                    "documentation": "<p>Use the request's originating IP address as an aggregate key. Each distinct IP address contributes to the aggregation instance.</p> <p>When you specify an IP or forwarded IP in the custom key settings, you must also specify at least one other key to use. You can aggregate on only the IP address by specifying <code>IP</code> in your rate-based statement's <code>AggregateKeyType</code>. </p>",
+                    "shape": "RateLimitIP"
+                },
+                "LabelNamespace": {
+                    "documentation": "<p>Use the specified label namespace as an aggregate key. Each distinct fully qualified label name that has the specified label namespace contributes to the aggregation instance. If you use just one label namespace as your custom key, then each label name fully defines an aggregation instance. </p> <p>This uses only labels that have been added to the request by rules that are evaluated before this rate-based rule in the web ACL. </p> <p>For information about label namespaces and names, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-rule-label-requirements.html\">Label syntax and naming requirements</a> in the <i>WAF Developer Guide</i>.</p>",
+                    "shape": "RateLimitLabelNamespace"
+                },
+                "QueryArgument": {
+                    "documentation": "<p>Use the specified query argument as an aggregate key. Each distinct value for the named query argument contributes to the aggregation instance. If you use a single query argument as your custom key, then each value fully defines an aggregation instance. </p>",
+                    "shape": "RateLimitQueryArgument"
+                },
+                "QueryString": {
+                    "documentation": "<p>Use the request's query string as an aggregate key. Each distinct string contributes to the aggregation instance. If you use just the query string as your custom key, then each string fully defines an aggregation instance. </p>",
+                    "shape": "RateLimitQueryString"
+                }
+            },
+            "type": "structure"
+        },
+        "RateBasedStatementCustomKeys": {
+            "max": 5,
+            "member": {
+                "shape": "RateBasedStatementCustomKey"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "RateBasedStatementManagedKeysIPSet": {
-            "documentation": "<p>The set of IP addresses that are currently blocked for a <a>RateBasedStatement</a>.</p>",
+            "documentation": "<p>The set of IP addresses that are currently blocked for a <a>RateBasedStatement</a>. This is only available for rate-based rules that aggregate on just the IP address, with the <code>AggregateKeyType</code> set to <code>IP</code> or <code>FORWARDED_IP</code>.</p> <p>A rate-based rule applies its rule action to requests from IP addresses that are in the rule's managed keys list and that match the rule's scope-down statement. When a rule has no scope-down statement, it applies the action to all requests from the IP addresses that are in the list. The rule applies its rule action to rate limit the matching requests. The action is usually Block but it can be any valid rule action except for Allow. </p> <p>The maximum number of IP addresses that can be rate limited by a single rate-based rule instance is 10,000. If more than 10,000 addresses exceed the rate limit, WAF limits those with the highest rates. </p>",
             "members": {
                 "Addresses": {
                     "documentation": "<p>The IP addresses that are currently blocked.</p>",
                     "shape": "IPAddresses"
                 },
                 "IPAddressVersion": {
                     "documentation": "<p>The version of the IP addresses, either <code>IPV4</code> or <code>IPV6</code>. </p>",
@@ -4919,14 +5503,109 @@
             "type": "structure"
         },
         "RateLimit": {
             "max": 2000000000,
             "min": 100,
             "type": "long"
         },
+        "RateLimitCookie": {
+            "documentation": "<p>Specifies a cookie as an aggregate key for a rate-based rule. Each distinct value in the cookie contributes to the aggregation instance. If you use a single cookie as your custom key, then each value fully defines an aggregation instance. </p>",
+            "members": {
+                "Name": {
+                    "documentation": "<p>The name of the cookie to use. </p>",
+                    "shape": "FieldToMatchData"
+                },
+                "TextTransformations": {
+                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. Text transformations are used in rule match statements, to transform the <code>FieldToMatch</code> request component before inspecting it, and they're used in rate-based rule statements, to transform request components before using them as custom aggregation keys. If you specify one or more transformations to apply, WAF performs all transformations on the specified content, starting from the lowest priority setting, and then uses the component contents. </p>",
+                    "shape": "TextTransformations"
+                }
+            },
+            "required": [
+                "Name",
+                "TextTransformations"
+            ],
+            "type": "structure"
+        },
+        "RateLimitForwardedIP": {
+            "documentation": "<p>Specifies the first IP address in an HTTP header as an aggregate key for a rate-based rule. Each distinct forwarded IP address contributes to the aggregation instance.</p> <p>This setting is used only in the <code>RateBasedStatementCustomKey</code> specification of a rate-based rule statement. When you specify an IP or forwarded IP in the custom key settings, you must also specify at least one other key to use. You can aggregate on only the forwarded IP address by specifying <code>FORWARDED_IP</code> in your rate-based statement's <code>AggregateKeyType</code>. </p> <p>This data type supports using the forwarded IP address in the web request aggregation for a rate-based rule, in <code>RateBasedStatementCustomKey</code>. The JSON specification for using the forwarded IP address doesn't explicitly use this data type. </p> <p>JSON specification: <code>\"ForwardedIP\": {}</code> </p> <p>When you use this specification, you must also configure the forwarded IP address in the rate-based statement's <code>ForwardedIPConfig</code>. </p>",
+            "members": {},
+            "type": "structure"
+        },
+        "RateLimitHTTPMethod": {
+            "documentation": "<p>Specifies the request's HTTP method as an aggregate key for a rate-based rule. Each distinct HTTP method contributes to the aggregation instance. If you use just the HTTP method as your custom key, then each method fully defines an aggregation instance. </p> <p>JSON specification: <code>\"RateLimitHTTPMethod\": {}</code> </p>",
+            "members": {},
+            "type": "structure"
+        },
+        "RateLimitHeader": {
+            "documentation": "<p>Specifies a header as an aggregate key for a rate-based rule. Each distinct value in the header contributes to the aggregation instance. If you use a single header as your custom key, then each value fully defines an aggregation instance. </p>",
+            "members": {
+                "Name": {
+                    "documentation": "<p>The name of the header to use. </p>",
+                    "shape": "FieldToMatchData"
+                },
+                "TextTransformations": {
+                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. Text transformations are used in rule match statements, to transform the <code>FieldToMatch</code> request component before inspecting it, and they're used in rate-based rule statements, to transform request components before using them as custom aggregation keys. If you specify one or more transformations to apply, WAF performs all transformations on the specified content, starting from the lowest priority setting, and then uses the component contents. </p>",
+                    "shape": "TextTransformations"
+                }
+            },
+            "required": [
+                "Name",
+                "TextTransformations"
+            ],
+            "type": "structure"
+        },
+        "RateLimitIP": {
+            "documentation": "<p>Specifies the IP address in the web request as an aggregate key for a rate-based rule. Each distinct IP address contributes to the aggregation instance. </p> <p>This setting is used only in the <code>RateBasedStatementCustomKey</code> specification of a rate-based rule statement. To use this in the custom key settings, you must specify at least one other key to use, along with the IP address. To aggregate on only the IP address, in your rate-based statement's <code>AggregateKeyType</code>, specify <code>IP</code>.</p> <p>JSON specification: <code>\"RateLimitIP\": {}</code> </p>",
+            "members": {},
+            "type": "structure"
+        },
+        "RateLimitLabelNamespace": {
+            "documentation": "<p>Specifies a label namespace to use as an aggregate key for a rate-based rule. Each distinct fully qualified label name that has the specified label namespace contributes to the aggregation instance. If you use just one label namespace as your custom key, then each label name fully defines an aggregation instance. </p> <p>This uses only labels that have been added to the request by rules that are evaluated before this rate-based rule in the web ACL. </p> <p>For information about label namespaces and names, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-rule-label-requirements.html\">Label syntax and naming requirements</a> in the <i>WAF Developer Guide</i>.</p>",
+            "members": {
+                "Namespace": {
+                    "documentation": "<p>The namespace to use for aggregation. </p>",
+                    "shape": "LabelNamespace"
+                }
+            },
+            "required": [
+                "Namespace"
+            ],
+            "type": "structure"
+        },
+        "RateLimitQueryArgument": {
+            "documentation": "<p>Specifies a query argument in the request as an aggregate key for a rate-based rule. Each distinct value for the named query argument contributes to the aggregation instance. If you use a single query argument as your custom key, then each value fully defines an aggregation instance. </p>",
+            "members": {
+                "Name": {
+                    "documentation": "<p>The name of the query argument to use. </p>",
+                    "shape": "FieldToMatchData"
+                },
+                "TextTransformations": {
+                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. Text transformations are used in rule match statements, to transform the <code>FieldToMatch</code> request component before inspecting it, and they're used in rate-based rule statements, to transform request components before using them as custom aggregation keys. If you specify one or more transformations to apply, WAF performs all transformations on the specified content, starting from the lowest priority setting, and then uses the component contents. </p>",
+                    "shape": "TextTransformations"
+                }
+            },
+            "required": [
+                "Name",
+                "TextTransformations"
+            ],
+            "type": "structure"
+        },
+        "RateLimitQueryString": {
+            "documentation": "<p>Specifies the request's query string as an aggregate key for a rate-based rule. Each distinct string contributes to the aggregation instance. If you use just the query string as your custom key, then each string fully defines an aggregation instance. </p>",
+            "members": {
+                "TextTransformations": {
+                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. Text transformations are used in rule match statements, to transform the <code>FieldToMatch</code> request component before inspecting it, and they're used in rate-based rule statements, to transform request components before using them as custom aggregation keys. If you specify one or more transformations to apply, WAF performs all transformations on the specified content, starting from the lowest priority setting, and then uses the component contents. </p>",
+                    "shape": "TextTransformations"
+                }
+            },
+            "required": [
+                "TextTransformations"
+            ],
+            "type": "structure"
+        },
         "RedactedFields": {
             "max": 100,
             "member": {
                 "shape": "FieldToMatch"
             },
             "type": "list"
         },
@@ -4948,15 +5627,15 @@
                     "shape": "FieldToMatch"
                 },
                 "RegexString": {
                     "documentation": "<p>The string representing the regular expression.</p>",
                     "shape": "RegexPatternString"
                 },
                 "TextTransformations": {
-                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. If you specify one or more transformations in a rule statement, WAF performs all transformations on the content of the request component identified by <code>FieldToMatch</code>, starting from the lowest priority setting, before inspecting the content for a match.</p>",
+                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. Text transformations are used in rule match statements, to transform the <code>FieldToMatch</code> request component before inspecting it, and they're used in rate-based rule statements, to transform request components before using them as custom aggregation keys. If you specify one or more transformations to apply, WAF performs all transformations on the specified content, starting from the lowest priority setting, and then uses the component contents. </p>",
                     "shape": "TextTransformations"
                 }
             },
             "required": [
                 "RegexString",
                 "FieldToMatch",
                 "TextTransformations"
@@ -4997,15 +5676,15 @@
                     "shape": "ResourceArn"
                 },
                 "FieldToMatch": {
                     "documentation": "<p>The part of the web request that you want WAF to inspect. </p>",
                     "shape": "FieldToMatch"
                 },
                 "TextTransformations": {
-                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. If you specify one or more transformations in a rule statement, WAF performs all transformations on the content of the request component identified by <code>FieldToMatch</code>, starting from the lowest priority setting, before inspecting the content for a match.</p>",
+                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. Text transformations are used in rule match statements, to transform the <code>FieldToMatch</code> request component before inspecting it, and they're used in rate-based rule statements, to transform request components before using them as custom aggregation keys. If you specify one or more transformations to apply, WAF performs all transformations on the specified content, starting from the lowest priority setting, and then uses the component contents. </p>",
                     "shape": "TextTransformations"
                 }
             },
             "required": [
                 "ARN",
                 "FieldToMatch",
                 "TextTransformations"
@@ -5046,14 +5725,20 @@
         },
         "RegexPatternString": {
             "max": 512,
             "min": 1,
             "pattern": ".*",
             "type": "string"
         },
+        "RegistrationPagePathString": {
+            "max": 256,
+            "min": 1,
+            "pattern": ".*\\S.*",
+            "type": "string"
+        },
         "RegularExpressionList": {
             "member": {
                 "shape": "Regex"
             },
             "type": "list"
         },
         "ReleaseNotes": {
@@ -5075,37 +5760,92 @@
                 "Timestamp": {
                     "documentation": "<p>The timestamp of the release. </p>",
                     "shape": "Timestamp"
                 }
             },
             "type": "structure"
         },
+        "RequestBody": {
+            "key": {
+                "shape": "AssociatedResourceType"
+            },
+            "type": "map",
+            "value": {
+                "shape": "RequestBodyAssociatedResourceTypeConfig"
+            }
+        },
+        "RequestBodyAssociatedResourceTypeConfig": {
+            "documentation": "<p>Customizes the maximum size of the request body that your protected CloudFront distributions forward to WAF for inspection. The default size is 16 KB (16,384 kilobytes). </p> <note> <p>You are charged additional fees when your protected resources forward body sizes that are larger than the default. For more information, see <a href=\"http://aws.amazon.com/waf/pricing/\">WAF Pricing</a>.</p> </note> <p>This is used in the <code>AssociationConfig</code> of the web ACL. </p>",
+            "members": {
+                "DefaultSizeInspectionLimit": {
+                    "documentation": "<p>Specifies the maximum size of the web request body component that an associated CloudFront distribution should send to WAF for inspection. This applies to statements in the web ACL that inspect the body or JSON body. </p> <p>Default: <code>16 KB (16,384 kilobytes)</code> </p>",
+                    "shape": "SizeInspectionLimit"
+                }
+            },
+            "required": [
+                "DefaultSizeInspectionLimit"
+            ],
+            "type": "structure"
+        },
         "RequestInspection": {
             "documentation": "<p>The criteria for inspecting login requests, used by the ATP rule group to validate credentials usage. </p> <p>This is part of the <code>AWSManagedRulesATPRuleSet</code> configuration in <code>ManagedRuleGroupConfig</code>.</p> <p>In these settings, you specify how your application accepts login attempts by providing the request payload type and the names of the fields within the request body where the username and password are provided. </p>",
             "members": {
                 "PasswordField": {
-                    "documentation": "<p>Details about your login page password field. </p> <p>How you specify this depends on the payload type.</p> <ul> <li> <p>For JSON payloads, specify the field name in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"login\": { \"username\": \"THE_USERNAME\", \"password\": \"THE_PASSWORD\" } }</code>, the username field specification is <code>/login/username</code> and the password field specification is <code>/login/password</code>.</p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with input elements named <code>username1</code> and <code>password1</code>, the username field specification is <code>username1</code> and the password field specification is <code>password1</code>.</p> </li> </ul>",
+                    "documentation": "<p>The name of the field in the request payload that contains your customer's password. </p> <p>How you specify this depends on the request inspection payload type.</p> <ul> <li> <p>For JSON payloads, specify the field name in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"form\": { \"password\": \"THE_PASSWORD\" } }</code>, the password field specification is <code>/form/password</code>.</p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with the input element named <code>password1</code>, the password field specification is <code>password1</code>.</p> </li> </ul>",
                     "shape": "PasswordField"
                 },
                 "PayloadType": {
                     "documentation": "<p>The payload type for your login endpoint, either JSON or form encoded.</p>",
                     "shape": "PayloadType"
                 },
                 "UsernameField": {
-                    "documentation": "<p>Details about your login page username field. </p> <p>How you specify this depends on the payload type.</p> <ul> <li> <p>For JSON payloads, specify the field name in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"login\": { \"username\": \"THE_USERNAME\", \"password\": \"THE_PASSWORD\" } }</code>, the username field specification is <code>/login/username</code> and the password field specification is <code>/login/password</code>.</p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with input elements named <code>username1</code> and <code>password1</code>, the username field specification is <code>username1</code> and the password field specification is <code>password1</code>.</p> </li> </ul>",
+                    "documentation": "<p>The name of the field in the request payload that contains your customer's username. </p> <p>How you specify this depends on the request inspection payload type.</p> <ul> <li> <p>For JSON payloads, specify the field name in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"form\": { \"username\": \"THE_USERNAME\" } }</code>, the username field specification is <code>/form/username</code>. </p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with the input element named <code>username1</code>, the username field specification is <code>username1</code> </p> </li> </ul>",
                     "shape": "UsernameField"
                 }
             },
             "required": [
                 "PayloadType",
                 "UsernameField",
                 "PasswordField"
             ],
             "type": "structure"
         },
+        "RequestInspectionACFP": {
+            "documentation": "<p>The criteria for inspecting account creation requests, used by the ACFP rule group to validate and track account creation attempts. </p> <p>This is part of the <code>AWSManagedRulesACFPRuleSet</code> configuration in <code>ManagedRuleGroupConfig</code>.</p> <p>In these settings, you specify how your application accepts account creation attempts by providing the request payload type and the names of the fields within the request body where the username, password, email, and primary address and phone number fields are provided. </p>",
+            "members": {
+                "AddressFields": {
+                    "documentation": "<p>The names of the fields in the request payload that contain your customer's primary physical address. </p> <p>Order the address fields in the array exactly as they are ordered in the request payload. </p> <p>How you specify the address fields depends on the request inspection payload type.</p> <ul> <li> <p>For JSON payloads, specify the field identifiers in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"form\": { \"primaryaddressline1\": \"THE_ADDRESS1\", \"primaryaddressline2\": \"THE_ADDRESS2\", \"primaryaddressline3\": \"THE_ADDRESS3\" } }</code>, the address field idenfiers are <code>/form/primaryaddressline1</code>, <code>/form/primaryaddressline2</code>, and <code>/form/primaryaddressline3</code>.</p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with input elements named <code>primaryaddressline1</code>, <code>primaryaddressline2</code>, and <code>primaryaddressline3</code>, the address fields identifiers are <code>primaryaddressline1</code>, <code>primaryaddressline2</code>, and <code>primaryaddressline3</code>. </p> </li> </ul>",
+                    "shape": "AddressFields"
+                },
+                "EmailField": {
+                    "documentation": "<p>The name of the field in the request payload that contains your customer's email. </p> <p>How you specify this depends on the request inspection payload type.</p> <ul> <li> <p>For JSON payloads, specify the field name in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"form\": { \"email\": \"THE_EMAIL\" } }</code>, the email field specification is <code>/form/email</code>.</p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with the input element named <code>email1</code>, the email field specification is <code>email1</code>.</p> </li> </ul>",
+                    "shape": "EmailField"
+                },
+                "PasswordField": {
+                    "documentation": "<p>The name of the field in the request payload that contains your customer's password. </p> <p>How you specify this depends on the request inspection payload type.</p> <ul> <li> <p>For JSON payloads, specify the field name in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"form\": { \"password\": \"THE_PASSWORD\" } }</code>, the password field specification is <code>/form/password</code>.</p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with the input element named <code>password1</code>, the password field specification is <code>password1</code>.</p> </li> </ul>",
+                    "shape": "PasswordField"
+                },
+                "PayloadType": {
+                    "documentation": "<p>The payload type for your account creation endpoint, either JSON or form encoded.</p>",
+                    "shape": "PayloadType"
+                },
+                "PhoneNumberFields": {
+                    "documentation": "<p>The names of the fields in the request payload that contain your customer's primary phone number. </p> <p>Order the phone number fields in the array exactly as they are ordered in the request payload. </p> <p>How you specify the phone number fields depends on the request inspection payload type.</p> <ul> <li> <p>For JSON payloads, specify the field identifiers in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"form\": { \"primaryphoneline1\": \"THE_PHONE1\", \"primaryphoneline2\": \"THE_PHONE2\", \"primaryphoneline3\": \"THE_PHONE3\" } }</code>, the phone number field identifiers are <code>/form/primaryphoneline1</code>, <code>/form/primaryphoneline2</code>, and <code>/form/primaryphoneline3</code>.</p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with input elements named <code>primaryphoneline1</code>, <code>primaryphoneline2</code>, and <code>primaryphoneline3</code>, the phone number field identifiers are <code>primaryphoneline1</code>, <code>primaryphoneline2</code>, and <code>primaryphoneline3</code>. </p> </li> </ul>",
+                    "shape": "PhoneNumberFields"
+                },
+                "UsernameField": {
+                    "documentation": "<p>The name of the field in the request payload that contains your customer's username. </p> <p>How you specify this depends on the request inspection payload type.</p> <ul> <li> <p>For JSON payloads, specify the field name in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"form\": { \"username\": \"THE_USERNAME\" } }</code>, the username field specification is <code>/form/username</code>. </p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with the input element named <code>username1</code>, the username field specification is <code>username1</code> </p> </li> </ul>",
+                    "shape": "UsernameField"
+                }
+            },
+            "required": [
+                "PayloadType"
+            ],
+            "type": "structure"
+        },
         "ResourceArn": {
             "max": 2048,
             "min": 20,
             "pattern": ".*\\S.*",
             "type": "string"
         },
         "ResourceArns": {
@@ -5116,15 +5856,16 @@
         },
         "ResourceType": {
             "enum": [
                 "APPLICATION_LOAD_BALANCER",
                 "API_GATEWAY",
                 "APPSYNC",
                 "COGNITO_USER_POOL",
-                "APP_RUNNER_SERVICE"
+                "APP_RUNNER_SERVICE",
+                "VERIFIED_ACCESS_INSTANCE"
             ],
             "type": "string"
         },
         "ResponseCode": {
             "type": "integer"
         },
         "ResponseContent": {
@@ -5138,44 +5879,44 @@
                 "TEXT_PLAIN",
                 "TEXT_HTML",
                 "APPLICATION_JSON"
             ],
             "type": "string"
         },
         "ResponseInspection": {
-            "documentation": "<p>The criteria for inspecting responses to login requests, used by the ATP rule group to track login failure rates. </p> <p>The ATP rule group evaluates the responses that your protected resources send back to client login attempts, keeping count of successful and failed attempts from each IP address and client session. Using this information, the rule group labels and mitigates requests from client sessions and IP addresses that submit too many failed login attempts in a short amount of time. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note> <p>This is part of the <code>AWSManagedRulesATPRuleSet</code> configuration in <code>ManagedRuleGroupConfig</code>.</p> <p>Enable login response inspection by configuring exactly one component of the response to inspect. You can't configure more than one. If you don't configure any of the response inspection options, response inspection is disabled. </p>",
+            "documentation": "<p>The criteria for inspecting responses to login requests and account creation requests, used by the ATP and ACFP rule groups to track login and account creation success and failure rates. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note> <p>The rule groups evaluates the responses that your protected resources send back to client login and account creation attempts, keeping count of successful and failed attempts from each IP address and client session. Using this information, the rule group labels and mitigates requests from client sessions and IP addresses with too much suspicious activity in a short amount of time. </p> <p>This is part of the <code>AWSManagedRulesATPRuleSet</code> and <code>AWSManagedRulesACFPRuleSet</code> configurations in <code>ManagedRuleGroupConfig</code>.</p> <p>Enable response inspection by configuring exactly one component of the response to inspect, for example, <code>Header</code> or <code>StatusCode</code>. You can't configure more than one component for inspection. If you don't configure any of the response inspection options, response inspection is disabled. </p>",
             "members": {
                 "BodyContains": {
-                    "documentation": "<p>Configures inspection of the response body. WAF can inspect the first 65,536 bytes (64 KB) of the response body. </p>",
+                    "documentation": "<p>Configures inspection of the response body for success and failure indicators. WAF can inspect the first 65,536 bytes (64 KB) of the response body. </p>",
                     "shape": "ResponseInspectionBodyContains"
                 },
                 "Header": {
-                    "documentation": "<p>Configures inspection of the response header. </p>",
+                    "documentation": "<p>Configures inspection of the response header for success and failure indicators. </p>",
                     "shape": "ResponseInspectionHeader"
                 },
                 "Json": {
-                    "documentation": "<p>Configures inspection of the response JSON. WAF can inspect the first 65,536 bytes (64 KB) of the response JSON. </p>",
+                    "documentation": "<p>Configures inspection of the response JSON for success and failure indicators. WAF can inspect the first 65,536 bytes (64 KB) of the response JSON. </p>",
                     "shape": "ResponseInspectionJson"
                 },
                 "StatusCode": {
-                    "documentation": "<p>Configures inspection of the response status code. </p>",
+                    "documentation": "<p>Configures inspection of the response status code for success and failure indicators. </p>",
                     "shape": "ResponseInspectionStatusCode"
                 }
             },
             "type": "structure"
         },
         "ResponseInspectionBodyContains": {
-            "documentation": "<p>Configures inspection of the response body. WAF can inspect the first 65,536 bytes (64 KB) of the response body. This is part of the <code>ResponseInspection</code> configuration for <code>AWSManagedRulesATPRuleSet</code>. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note>",
+            "documentation": "<p>Configures inspection of the response body. WAF can inspect the first 65,536 bytes (64 KB) of the response body. This is part of the <code>ResponseInspection</code> configuration for <code>AWSManagedRulesATPRuleSet</code> and <code>AWSManagedRulesACFPRuleSet</code>. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note>",
             "members": {
                 "FailureStrings": {
-                    "documentation": "<p>Strings in the body of the response that indicate a failed login attempt. To be counted as a failed login, the string can be anywhere in the body and must be an exact match, including case. Each string must be unique among the success and failure strings. </p> <p>JSON example: <code>\"FailureStrings\": [ \"Login failed\" ]</code> </p>",
+                    "documentation": "<p>Strings in the body of the response that indicate a failed login or account creation attempt. To be counted as a failure, the string can be anywhere in the body and must be an exact match, including case. Each string must be unique among the success and failure strings. </p> <p>JSON example: <code>\"FailureStrings\": [ \"Request failed\" ]</code> </p>",
                     "shape": "ResponseInspectionBodyContainsFailureStrings"
                 },
                 "SuccessStrings": {
-                    "documentation": "<p>Strings in the body of the response that indicate a successful login attempt. To be counted as a successful login, the string can be anywhere in the body and must be an exact match, including case. Each string must be unique among the success and failure strings. </p> <p>JSON example: <code>\"SuccessStrings\": [ \"Login successful\", \"Welcome to our site!\" ]</code> </p>",
+                    "documentation": "<p>Strings in the body of the response that indicate a successful login or account creation attempt. To be counted as a success, the string can be anywhere in the body and must be an exact match, including case. Each string must be unique among the success and failure strings. </p> <p>JSON examples: <code>\"SuccessStrings\": [ \"Login successful\" ]</code> and <code>\"SuccessStrings\": [ \"Account creation successful\", \"Welcome to our site!\" ]</code> </p>",
                     "shape": "ResponseInspectionBodyContainsSuccessStrings"
                 }
             },
             "required": [
                 "SuccessStrings",
                 "FailureStrings"
             ],
@@ -5194,26 +5935,26 @@
             "member": {
                 "shape": "SuccessValue"
             },
             "min": 1,
             "type": "list"
         },
         "ResponseInspectionHeader": {
-            "documentation": "<p>Configures inspection of the response header. This is part of the <code>ResponseInspection</code> configuration for <code>AWSManagedRulesATPRuleSet</code>. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note>",
+            "documentation": "<p>Configures inspection of the response header. This is part of the <code>ResponseInspection</code> configuration for <code>AWSManagedRulesATPRuleSet</code> and <code>AWSManagedRulesACFPRuleSet</code>. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note>",
             "members": {
                 "FailureValues": {
-                    "documentation": "<p>Values in the response header with the specified name that indicate a failed login attempt. To be counted as a failed login, the value must be an exact match, including case. Each value must be unique among the success and failure values. </p> <p>JSON example: <code>\"FailureValues\": [ \"LoginFailed\", \"Failed login\" ]</code> </p>",
+                    "documentation": "<p>Values in the response header with the specified name that indicate a failed login or account creation attempt. To be counted as a failure, the value must be an exact match, including case. Each value must be unique among the success and failure values. </p> <p>JSON examples: <code>\"FailureValues\": [ \"LoginFailed\", \"Failed login\" ]</code> and <code>\"FailureValues\": [ \"AccountCreationFailed\" ]</code> </p>",
                     "shape": "ResponseInspectionHeaderFailureValues"
                 },
                 "Name": {
-                    "documentation": "<p>The name of the header to match against. The name must be an exact match, including case.</p> <p>JSON example: <code>\"Name\": [ \"LoginResult\" ]</code> </p>",
+                    "documentation": "<p>The name of the header to match against. The name must be an exact match, including case.</p> <p>JSON example: <code>\"Name\": [ \"RequestResult\" ]</code> </p>",
                     "shape": "ResponseInspectionHeaderName"
                 },
                 "SuccessValues": {
-                    "documentation": "<p>Values in the response header with the specified name that indicate a successful login attempt. To be counted as a successful login, the value must be an exact match, including case. Each value must be unique among the success and failure values. </p> <p>JSON example: <code>\"SuccessValues\": [ \"LoginPassed\", \"Successful login\" ]</code> </p>",
+                    "documentation": "<p>Values in the response header with the specified name that indicate a successful login or account creation attempt. To be counted as a success, the value must be an exact match, including case. Each value must be unique among the success and failure values. </p> <p>JSON examples: <code>\"SuccessValues\": [ \"LoginPassed\", \"Successful login\" ]</code> and <code>\"SuccessValues\": [ \"AccountCreated\", \"Successful account creation\" ]</code> </p>",
                     "shape": "ResponseInspectionHeaderSuccessValues"
                 }
             },
             "required": [
                 "Name",
                 "SuccessValues",
                 "FailureValues"
@@ -5239,26 +5980,26 @@
             "member": {
                 "shape": "SuccessValue"
             },
             "min": 1,
             "type": "list"
         },
         "ResponseInspectionJson": {
-            "documentation": "<p>Configures inspection of the response JSON. WAF can inspect the first 65,536 bytes (64 KB) of the response JSON. This is part of the <code>ResponseInspection</code> configuration for <code>AWSManagedRulesATPRuleSet</code>. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note>",
+            "documentation": "<p>Configures inspection of the response JSON. WAF can inspect the first 65,536 bytes (64 KB) of the response JSON. This is part of the <code>ResponseInspection</code> configuration for <code>AWSManagedRulesATPRuleSet</code> and <code>AWSManagedRulesACFPRuleSet</code>. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note>",
             "members": {
                 "FailureValues": {
-                    "documentation": "<p>Values for the specified identifier in the response JSON that indicate a failed login attempt. To be counted as a failed login, the value must be an exact match, including case. Each value must be unique among the success and failure values. </p> <p>JSON example: <code>\"FailureValues\": [ \"False\", \"Failed\" ]</code> </p>",
+                    "documentation": "<p>Values for the specified identifier in the response JSON that indicate a failed login or account creation attempt. To be counted as a failure, the value must be an exact match, including case. Each value must be unique among the success and failure values. </p> <p>JSON example: <code>\"FailureValues\": [ \"False\", \"Failed\" ]</code> </p>",
                     "shape": "ResponseInspectionJsonFailureValues"
                 },
                 "Identifier": {
-                    "documentation": "<p>The identifier for the value to match against in the JSON. The identifier must be an exact match, including case.</p> <p>JSON example: <code>\"Identifier\": [ \"/login/success\" ]</code> </p>",
+                    "documentation": "<p>The identifier for the value to match against in the JSON. The identifier must be an exact match, including case.</p> <p>JSON examples: <code>\"Identifier\": [ \"/login/success\" ]</code> and <code>\"Identifier\": [ \"/sign-up/success\" ]</code> </p>",
                     "shape": "FieldIdentifier"
                 },
                 "SuccessValues": {
-                    "documentation": "<p>Values for the specified identifier in the response JSON that indicate a successful login attempt. To be counted as a successful login, the value must be an exact match, including case. Each value must be unique among the success and failure values. </p> <p>JSON example: <code>\"SuccessValues\": [ \"True\", \"Succeeded\" ]</code> </p>",
+                    "documentation": "<p>Values for the specified identifier in the response JSON that indicate a successful login or account creation attempt. To be counted as a success, the value must be an exact match, including case. Each value must be unique among the success and failure values. </p> <p>JSON example: <code>\"SuccessValues\": [ \"True\", \"Succeeded\" ]</code> </p>",
                     "shape": "ResponseInspectionJsonSuccessValues"
                 }
             },
             "required": [
                 "Identifier",
                 "SuccessValues",
                 "FailureValues"
@@ -5278,22 +6019,22 @@
             "member": {
                 "shape": "SuccessValue"
             },
             "min": 1,
             "type": "list"
         },
         "ResponseInspectionStatusCode": {
-            "documentation": "<p>Configures inspection of the response status code. This is part of the <code>ResponseInspection</code> configuration for <code>AWSManagedRulesATPRuleSet</code>. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note>",
+            "documentation": "<p>Configures inspection of the response status code. This is part of the <code>ResponseInspection</code> configuration for <code>AWSManagedRulesATPRuleSet</code> and <code>AWSManagedRulesACFPRuleSet</code>. </p> <note> <p>Response inspection is available only in web ACLs that protect Amazon CloudFront distributions.</p> </note>",
             "members": {
                 "FailureCodes": {
-                    "documentation": "<p>Status codes in the response that indicate a failed login attempt. To be counted as a failed login, the response status code must match one of these. Each code must be unique among the success and failure status codes. </p> <p>JSON example: <code>\"FailureCodes\": [ 400, 404 ]</code> </p>",
+                    "documentation": "<p>Status codes in the response that indicate a failed login or account creation attempt. To be counted as a failure, the response status code must match one of these. Each code must be unique among the success and failure status codes. </p> <p>JSON example: <code>\"FailureCodes\": [ 400, 404 ]</code> </p>",
                     "shape": "ResponseInspectionStatusCodeFailureCodes"
                 },
                 "SuccessCodes": {
-                    "documentation": "<p>Status codes in the response that indicate a successful login attempt. To be counted as a successful login, the response status code must match one of these. Each code must be unique among the success and failure status codes. </p> <p>JSON example: <code>\"SuccessCodes\": [ 200, 201 ]</code> </p>",
+                    "documentation": "<p>Status codes in the response that indicate a successful login or account creation attempt. To be counted as a success, the response status code must match one of these. Each code must be unique among the success and failure status codes. </p> <p>JSON example: <code>\"SuccessCodes\": [ 200, 201 ]</code> </p>",
                     "shape": "ResponseInspectionStatusCodeSuccessCodes"
                 }
             },
             "required": [
                 "SuccessCodes",
                 "FailureCodes"
             ],
@@ -5428,23 +6169,23 @@
                     "shape": "ResourceArn"
                 },
                 "AvailableLabels": {
                     "documentation": "<p>The labels that one or more rules in this rule group add to matching web requests. These labels are defined in the <code>RuleLabels</code> for a <a>Rule</a>.</p>",
                     "shape": "LabelSummaries"
                 },
                 "Capacity": {
-                    "documentation": "<p>The web ACL capacity units (WCUs) required for this rule group.</p> <p>When you create your own rule group, you define this, and you cannot change it after creation. When you add or modify the rules in a rule group, WAF enforces this limit. You can check the capacity for a set of rules using <a>CheckCapacity</a>.</p> <p>WAF uses WCUs to calculate and control the operating resources that are used to run your rules, rule groups, and web ACLs. WAF calculates capacity differently for each rule type, to reflect the relative cost of each rule. Simple rules that cost little to run use fewer WCUs than more complex rules that use more processing power. Rule group capacity is fixed at creation, which helps users plan their web ACL WCU usage when they use a rule group. The WCU limit for web ACLs is 1,500. </p>",
+                    "documentation": "<p>The web ACL capacity units (WCUs) required for this rule group.</p> <p>When you create your own rule group, you define this, and you cannot change it after creation. When you add or modify the rules in a rule group, WAF enforces this limit. You can check the capacity for a set of rules using <a>CheckCapacity</a>.</p> <p>WAF uses WCUs to calculate and control the operating resources that are used to run your rules, rule groups, and web ACLs. WAF calculates capacity differently for each rule type, to reflect the relative cost of each rule. Simple rules that cost little to run use fewer WCUs than more complex rules that use more processing power. Rule group capacity is fixed at creation, which helps users plan their web ACL WCU usage when they use a rule group. For more information, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/aws-waf-capacity-units.html\">WAF web ACL capacity units (WCU)</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CapacityUnit"
                 },
                 "ConsumedLabels": {
                     "documentation": "<p>The labels that one or more rules in this rule group match against in label match statements. These labels are defined in a <code>LabelMatchStatement</code> specification, in the <a>Statement</a> definition of a rule. </p>",
                     "shape": "LabelSummaries"
                 },
                 "CustomResponseBodies": {
-                    "documentation": "<p>A map of custom response keys and content bodies. When you create a rule with a block action, you can send a custom response to the web request. You define these for the rule group, and then use them in the rules that you define in the rule group. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>A map of custom response keys and content bodies. When you create a rule with a block action, you can send a custom response to the web request. You define these for the rule group, and then use them in the rules that you define in the rule group. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomResponseBodies"
                 },
                 "Description": {
                     "documentation": "<p>A description of the rule group that helps with identification. </p>",
                     "shape": "EntityDescription"
                 },
                 "Id": {
@@ -5675,41 +6416,50 @@
         },
         "Size": {
             "max": 21474836480,
             "min": 0,
             "type": "long"
         },
         "SizeConstraintStatement": {
-            "documentation": "<p>A rule statement that compares a number of bytes against the size of a request component, using a comparison operator, such as greater than (&gt;) or less than (&lt;). For example, you can use a size constraint statement to look for query strings that are longer than 100 bytes. </p> <p>If you configure WAF to inspect the request body, WAF inspects only the first 8192 bytes (8 KB). If the request body for your web requests never exceeds 8192 bytes, you could use a size constraint statement to block requests that have a request body greater than 8192 bytes.</p> <p>If you choose URI for the value of Part of the request to filter on, the slash (/) in the URI counts as one character. For example, the URI <code>/logo.jpg</code> is nine characters long.</p>",
+            "documentation": "<p>A rule statement that compares a number of bytes against the size of a request component, using a comparison operator, such as greater than (&gt;) or less than (&lt;). For example, you can use a size constraint statement to look for query strings that are longer than 100 bytes. </p> <p>If you configure WAF to inspect the request body, WAF inspects only the number of bytes of the body up to the limit for the web ACL. By default, for regional web ACLs, this limit is 8 KB (8,192 kilobytes) and for CloudFront web ACLs, this limit is 16 KB (16,384 kilobytes). For CloudFront web ACLs, you can increase the limit in the web ACL <code>AssociationConfig</code>, for additional fees. If you know that the request body for your web requests should never exceed the inspection limit, you could use a size constraint statement to block requests that have a larger request body size.</p> <p>If you choose URI for the value of Part of the request to filter on, the slash (/) in the URI counts as one character. For example, the URI <code>/logo.jpg</code> is nine characters long.</p>",
             "members": {
                 "ComparisonOperator": {
                     "documentation": "<p>The operator to use to compare the request part to the size setting. </p>",
                     "shape": "ComparisonOperator"
                 },
                 "FieldToMatch": {
                     "documentation": "<p>The part of the web request that you want WAF to inspect. </p>",
                     "shape": "FieldToMatch"
                 },
                 "Size": {
                     "documentation": "<p>The size, in byte, to compare to the request part, after any transformations.</p>",
                     "shape": "Size"
                 },
                 "TextTransformations": {
-                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. If you specify one or more transformations in a rule statement, WAF performs all transformations on the content of the request component identified by <code>FieldToMatch</code>, starting from the lowest priority setting, before inspecting the content for a match.</p>",
+                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. Text transformations are used in rule match statements, to transform the <code>FieldToMatch</code> request component before inspecting it, and they're used in rate-based rule statements, to transform request components before using them as custom aggregation keys. If you specify one or more transformations to apply, WAF performs all transformations on the specified content, starting from the lowest priority setting, and then uses the component contents. </p>",
                     "shape": "TextTransformations"
                 }
             },
             "required": [
                 "FieldToMatch",
                 "ComparisonOperator",
                 "Size",
                 "TextTransformations"
             ],
             "type": "structure"
         },
+        "SizeInspectionLimit": {
+            "enum": [
+                "KB_16",
+                "KB_32",
+                "KB_48",
+                "KB_64"
+            ],
+            "type": "string"
+        },
         "SolveTimestamp": {
             "type": "long"
         },
         "SqliMatchStatement": {
             "documentation": "<p>A rule statement that inspects for malicious SQL code. Attackers insert malicious SQL code into web requests to do things like modify your database or extract data from it. </p>",
             "members": {
                 "FieldToMatch": {
@@ -5717,15 +6467,15 @@
                     "shape": "FieldToMatch"
                 },
                 "SensitivityLevel": {
                     "documentation": "<p>The sensitivity that you want WAF to use to inspect for SQL injection attacks. </p> <p> <code>HIGH</code> detects more attacks, but might generate more false positives, especially if your web requests frequently contain unusual strings. For information about identifying and mitigating false positives, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/web-acl-testing.html\">Testing and tuning</a> in the <i>WAF Developer Guide</i>.</p> <p> <code>LOW</code> is generally a better choice for resources that already have other protections against SQL injection attacks or that have a low tolerance for false positives. </p> <p>Default: <code>LOW</code> </p>",
                     "shape": "SensitivityLevel"
                 },
                 "TextTransformations": {
-                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. If you specify one or more transformations in a rule statement, WAF performs all transformations on the content of the request component identified by <code>FieldToMatch</code>, starting from the lowest priority setting, before inspecting the content for a match.</p>",
+                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. Text transformations are used in rule match statements, to transform the <code>FieldToMatch</code> request component before inspecting it, and they're used in rate-based rule statements, to transform request components before using them as custom aggregation keys. If you specify one or more transformations to apply, WAF performs all transformations on the specified content, starting from the lowest priority setting, and then uses the component contents. </p>",
                     "shape": "TextTransformations"
                 }
             },
             "required": [
                 "FieldToMatch",
                 "TextTransformations"
             ],
@@ -5751,27 +6501,27 @@
                     "shape": "IPSetReferenceStatement"
                 },
                 "LabelMatchStatement": {
                     "documentation": "<p>A rule statement to match against labels that have been added to the web request by rules that have already run in the web ACL. </p> <p>The label match statement provides the label or namespace string to search for. The label string can represent a part or all of the fully qualified label name that had been added to the web request. Fully qualified labels have a prefix, optional namespaces, and label name. The prefix identifies the rule group or web ACL context of the rule that added the label. If you do not provide the fully qualified name in your label match string, WAF performs the search for labels that were added in the same context as the label match statement. </p>",
                     "shape": "LabelMatchStatement"
                 },
                 "ManagedRuleGroupStatement": {
-                    "documentation": "<p>A rule statement used to run the rules that are defined in a managed rule group. To use this, provide the vendor name and the name of the rule group in this statement. You can retrieve the required names by calling <a>ListAvailableManagedRuleGroups</a>.</p> <p>You cannot nest a <code>ManagedRuleGroupStatement</code>, for example for use inside a <code>NotStatement</code> or <code>OrStatement</code>. It can only be referenced as a top-level statement within a rule.</p> <note> <p>You are charged additional fees when you use the WAF Bot Control managed rule group <code>AWSManagedRulesBotControlRuleSet</code> or the WAF Fraud Control account takeover prevention (ATP) managed rule group <code>AWSManagedRulesATPRuleSet</code>. For more information, see <a href=\"http://aws.amazon.com/waf/pricing/\">WAF Pricing</a>.</p> </note>",
+                    "documentation": "<p>A rule statement used to run the rules that are defined in a managed rule group. To use this, provide the vendor name and the name of the rule group in this statement. You can retrieve the required names by calling <a>ListAvailableManagedRuleGroups</a>.</p> <p>You cannot nest a <code>ManagedRuleGroupStatement</code>, for example for use inside a <code>NotStatement</code> or <code>OrStatement</code>. It can only be referenced as a top-level statement within a rule.</p> <note> <p>You are charged additional fees when you use the WAF Bot Control managed rule group <code>AWSManagedRulesBotControlRuleSet</code>, the WAF Fraud Control account takeover prevention (ATP) managed rule group <code>AWSManagedRulesATPRuleSet</code>, or the WAF Fraud Control account creation fraud prevention (ACFP) managed rule group <code>AWSManagedRulesACFPRuleSet</code>. For more information, see <a href=\"http://aws.amazon.com/waf/pricing/\">WAF Pricing</a>.</p> </note>",
                     "shape": "ManagedRuleGroupStatement"
                 },
                 "NotStatement": {
                     "documentation": "<p>A logical rule statement used to negate the results of another rule statement. You provide one <a>Statement</a> within the <code>NotStatement</code>.</p>",
                     "shape": "NotStatement"
                 },
                 "OrStatement": {
                     "documentation": "<p>A logical rule statement used to combine other rule statements with OR logic. You provide more than one <a>Statement</a> within the <code>OrStatement</code>. </p>",
                     "shape": "OrStatement"
                 },
                 "RateBasedStatement": {
-                    "documentation": "<p>A rate-based rule tracks the rate of requests for each originating IP address, and triggers the rule action when the rate exceeds a limit that you specify on the number of requests in any 5-minute time span. You can use this to put a temporary block on requests from an IP address that is sending excessive requests. </p> <p>WAF tracks and manages web requests separately for each instance of a rate-based rule that you use. For example, if you provide the same rate-based rule settings in two web ACLs, each of the two rule statements represents a separate instance of the rate-based rule and gets its own tracking and management by WAF. If you define a rate-based rule inside a rule group, and then use that rule group in multiple places, each use creates a separate instance of the rate-based rule that gets its own tracking and management by WAF. </p> <p>When the rule action triggers, WAF blocks additional requests from the IP address until the request rate falls below the limit.</p> <p>You can optionally nest another statement inside the rate-based statement, to narrow the scope of the rule so that it only counts requests that match the nested statement. For example, based on recent requests that you have seen from an attacker, you might create a rate-based rule with a nested AND rule statement that contains the following nested statements:</p> <ul> <li> <p>An IP match statement with an IP set that specifies the address 192.0.2.44.</p> </li> <li> <p>A string match statement that searches in the User-Agent header for the string BadBot.</p> </li> </ul> <p>In this rate-based rule, you also define a rate limit. For this example, the rate limit is 1,000. Requests that meet the criteria of both of the nested statements are counted. If the count exceeds 1,000 requests per five minutes, the rule action triggers. Requests that do not meet the criteria of both of the nested statements are not counted towards the rate limit and are not affected by this rule.</p> <p>You cannot nest a <code>RateBasedStatement</code> inside another statement, for example inside a <code>NotStatement</code> or <code>OrStatement</code>. You can define a <code>RateBasedStatement</code> inside a web ACL and inside a rule group. </p>",
+                    "documentation": "<p>A rate-based rule counts incoming requests and rate limits requests when they are coming at too fast a rate. The rule categorizes requests according to your aggregation criteria, collects them into aggregation instances, and counts and rate limits the requests for each instance. </p> <p>You can specify individual aggregation keys, like IP address or HTTP method. You can also specify aggregation key combinations, like IP address and HTTP method, or HTTP method, query argument, and cookie. </p> <p>Each unique set of values for the aggregation keys that you specify is a separate aggregation instance, with the value from each key contributing to the aggregation instance definition. </p> <p>For example, assume the rule evaluates web requests with the following IP address and HTTP method values: </p> <ul> <li> <p>IP address 10.1.1.1, HTTP method POST</p> </li> <li> <p>IP address 10.1.1.1, HTTP method GET</p> </li> <li> <p>IP address 127.0.0.0, HTTP method POST</p> </li> <li> <p>IP address 10.1.1.1, HTTP method GET</p> </li> </ul> <p>The rule would create different aggregation instances according to your aggregation criteria, for example: </p> <ul> <li> <p>If the aggregation criteria is just the IP address, then each individual address is an aggregation instance, and WAF counts requests separately for each. The aggregation instances and request counts for our example would be the following: </p> <ul> <li> <p>IP address 10.1.1.1: count 3</p> </li> <li> <p>IP address 127.0.0.0: count 1</p> </li> </ul> </li> <li> <p>If the aggregation criteria is HTTP method, then each individual HTTP method is an aggregation instance. The aggregation instances and request counts for our example would be the following: </p> <ul> <li> <p>HTTP method POST: count 2</p> </li> <li> <p>HTTP method GET: count 2</p> </li> </ul> </li> <li> <p>If the aggregation criteria is IP address and HTTP method, then each IP address and each HTTP method would contribute to the combined aggregation instance. The aggregation instances and request counts for our example would be the following: </p> <ul> <li> <p>IP address 10.1.1.1, HTTP method POST: count 1</p> </li> <li> <p>IP address 10.1.1.1, HTTP method GET: count 2</p> </li> <li> <p>IP address 127.0.0.0, HTTP method POST: count 1</p> </li> </ul> </li> </ul> <p>For any n-tuple of aggregation keys, each unique combination of values for the keys defines a separate aggregation instance, which WAF counts and rate-limits individually. </p> <p>You can optionally nest another statement inside the rate-based statement, to narrow the scope of the rule so that it only counts and rate limits requests that match the nested statement. You can use this nested scope-down statement in conjunction with your aggregation key specifications or you can just count and rate limit all requests that match the scope-down statement, without additional aggregation. When you choose to just manage all requests that match a scope-down statement, the aggregation instance is singular for the rule. </p> <p>You cannot nest a <code>RateBasedStatement</code> inside another statement, for example inside a <code>NotStatement</code> or <code>OrStatement</code>. You can define a <code>RateBasedStatement</code> inside a web ACL and inside a rule group. </p> <p>For additional information about the options, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-rate-based-rules.html\">Rate limiting web requests using rate-based rules</a> in the <i>WAF Developer Guide</i>. </p> <p>If you only aggregate on the individual IP address or forwarded IP address, you can retrieve the list of IP addresses that WAF is currently rate limiting for a rule through the API call <code>GetRateBasedStatementManagedKeys</code>. This option is not available for other aggregation configurations.</p> <p>WAF tracks and manages web requests separately for each instance of a rate-based rule that you use. For example, if you provide the same rate-based rule settings in two web ACLs, each of the two rule statements represents a separate instance of the rate-based rule and gets its own tracking and management by WAF. If you define a rate-based rule inside a rule group, and then use that rule group in multiple places, each use creates a separate instance of the rate-based rule that gets its own tracking and management by WAF. </p>",
                     "shape": "RateBasedStatement"
                 },
                 "RegexMatchStatement": {
                     "documentation": "<p>A rule statement used to search web request components for a match against a single regular expression. </p>",
                     "shape": "RegexMatchStatement"
                 },
                 "RegexPatternSetReferenceStatement": {
@@ -5779,15 +6529,15 @@
                     "shape": "RegexPatternSetReferenceStatement"
                 },
                 "RuleGroupReferenceStatement": {
                     "documentation": "<p>A rule statement used to run the rules that are defined in a <a>RuleGroup</a>. To use this, create a rule group with your rules, then provide the ARN of the rule group in this statement.</p> <p>You cannot nest a <code>RuleGroupReferenceStatement</code>, for example for use inside a <code>NotStatement</code> or <code>OrStatement</code>. You can only use a rule group reference statement at the top level inside a web ACL. </p>",
                     "shape": "RuleGroupReferenceStatement"
                 },
                 "SizeConstraintStatement": {
-                    "documentation": "<p>A rule statement that compares a number of bytes against the size of a request component, using a comparison operator, such as greater than (&gt;) or less than (&lt;). For example, you can use a size constraint statement to look for query strings that are longer than 100 bytes. </p> <p>If you configure WAF to inspect the request body, WAF inspects only the first 8192 bytes (8 KB). If the request body for your web requests never exceeds 8192 bytes, you could use a size constraint statement to block requests that have a request body greater than 8192 bytes.</p> <p>If you choose URI for the value of Part of the request to filter on, the slash (/) in the URI counts as one character. For example, the URI <code>/logo.jpg</code> is nine characters long.</p>",
+                    "documentation": "<p>A rule statement that compares a number of bytes against the size of a request component, using a comparison operator, such as greater than (&gt;) or less than (&lt;). For example, you can use a size constraint statement to look for query strings that are longer than 100 bytes. </p> <p>If you configure WAF to inspect the request body, WAF inspects only the number of bytes of the body up to the limit for the web ACL. By default, for regional web ACLs, this limit is 8 KB (8,192 kilobytes) and for CloudFront web ACLs, this limit is 16 KB (16,384 kilobytes). For CloudFront web ACLs, you can increase the limit in the web ACL <code>AssociationConfig</code>, for additional fees. If you know that the request body for your web requests should never exceed the inspection limit, you could use a size constraint statement to block requests that have a larger request body size.</p> <p>If you choose URI for the value of Part of the request to filter on, the slash (/) in the URI counts as one character. For example, the URI <code>/logo.jpg</code> is nine characters long.</p>",
                     "shape": "SizeConstraintStatement"
                 },
                 "SqliMatchStatement": {
                     "documentation": "<p>A rule statement that inspects for malicious SQL code. Attackers insert malicious SQL code into web requests to do things like modify your database or extract data from it. </p>",
                     "shape": "SqliMatchStatement"
                 },
                 "XssMatchStatement": {
@@ -5896,15 +6646,15 @@
             "pattern": "^([\\p{L}\\p{Z}\\p{N}_.:/=+\\-@]*)$",
             "type": "string"
         },
         "TextTransformation": {
             "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. </p>",
             "members": {
                 "Priority": {
-                    "documentation": "<p>Sets the relative processing order for multiple transformations that are defined for a rule statement. WAF processes all transformations, from lowest priority to highest, before inspecting the transformed content. The priorities don't need to be consecutive, but they must all be different. </p>",
+                    "documentation": "<p>Sets the relative processing order for multiple transformations. WAF processes all transformations, from lowest priority to highest, before inspecting the transformed content. The priorities don't need to be consecutive, but they must all be different. </p>",
                     "shape": "TextTransformationPriority"
                 },
                 "Type": {
                     "documentation": "<p>You can specify the following transformation types:</p> <p> <b>BASE64_DECODE</b> - Decode a <code>Base64</code>-encoded string.</p> <p> <b>BASE64_DECODE_EXT</b> - Decode a <code>Base64</code>-encoded string, but use a forgiving implementation that ignores characters that aren't valid.</p> <p> <b>CMD_LINE</b> - Command-line transformations. These are helpful in reducing effectiveness of attackers who inject an operating system command-line command and use unusual formatting to disguise some or all of the command. </p> <ul> <li> <p>Delete the following characters: <code>\\ \" ' ^</code> </p> </li> <li> <p>Delete spaces before the following characters: <code>/ (</code> </p> </li> <li> <p>Replace the following characters with a space: <code>, ;</code> </p> </li> <li> <p>Replace multiple spaces with one space</p> </li> <li> <p>Convert uppercase letters (A-Z) to lowercase (a-z)</p> </li> </ul> <p> <b>COMPRESS_WHITE_SPACE</b> - Replace these characters with a space character (decimal 32): </p> <ul> <li> <p> <code>\\f</code>, formfeed, decimal 12</p> </li> <li> <p> <code>\\t</code>, tab, decimal 9</p> </li> <li> <p> <code>\\n</code>, newline, decimal 10</p> </li> <li> <p> <code>\\r</code>, carriage return, decimal 13</p> </li> <li> <p> <code>\\v</code>, vertical tab, decimal 11</p> </li> <li> <p>Non-breaking space, decimal 160</p> </li> </ul> <p> <code>COMPRESS_WHITE_SPACE</code> also replaces multiple spaces with one space.</p> <p> <b>CSS_DECODE</b> - Decode characters that were encoded using CSS 2.x escape rules <code>syndata.html#characters</code>. This function uses up to two bytes in the decoding process, so it can help to uncover ASCII characters that were encoded using CSS encoding that wouldn\u2019t typically be encoded. It's also useful in countering evasion, which is a combination of a backslash and non-hexadecimal characters. For example, <code>ja\\vascript</code> for javascript. </p> <p> <b>ESCAPE_SEQ_DECODE</b> - Decode the following ANSI C escape sequences: <code>\\a</code>, <code>\\b</code>, <code>\\f</code>, <code>\\n</code>, <code>\\r</code>, <code>\\t</code>, <code>\\v</code>, <code>\\\\</code>, <code>\\?</code>, <code>\\'</code>, <code>\\\"</code>, <code>\\xHH</code> (hexadecimal), <code>\\0OOO</code> (octal). Encodings that aren't valid remain in the output. </p> <p> <b>HEX_DECODE</b> - Decode a string of hexadecimal characters into a binary.</p> <p> <b>HTML_ENTITY_DECODE</b> - Replace HTML-encoded characters with unencoded characters. <code>HTML_ENTITY_DECODE</code> performs these operations: </p> <ul> <li> <p>Replaces <code>(ampersand)quot;</code> with <code>\"</code> </p> </li> <li> <p>Replaces <code>(ampersand)nbsp;</code> with a non-breaking space, decimal 160</p> </li> <li> <p>Replaces <code>(ampersand)lt;</code> with a \"less than\" symbol</p> </li> <li> <p>Replaces <code>(ampersand)gt;</code> with <code>&gt;</code> </p> </li> <li> <p>Replaces characters that are represented in hexadecimal format, <code>(ampersand)#xhhhh;</code>, with the corresponding characters</p> </li> <li> <p>Replaces characters that are represented in decimal format, <code>(ampersand)#nnnn;</code>, with the corresponding characters</p> </li> </ul> <p> <b>JS_DECODE</b> - Decode JavaScript escape sequences. If a <code>\\</code> <code>u</code> <code>HHHH</code> code is in the full-width ASCII code range of <code>FF01-FF5E</code>, then the higher byte is used to detect and adjust the lower byte. If not, only the lower byte is used and the higher byte is zeroed, causing a possible loss of information. </p> <p> <b>LOWERCASE</b> - Convert uppercase letters (A-Z) to lowercase (a-z). </p> <p> <b>MD5</b> - Calculate an MD5 hash from the data in the input. The computed hash is in a raw binary form. </p> <p> <b>NONE</b> - Specify <code>NONE</code> if you don't want any text transformations. </p> <p> <b>NORMALIZE_PATH</b> - Remove multiple slashes, directory self-references, and directory back-references that are not at the beginning of the input from an input string. </p> <p> <b>NORMALIZE_PATH_WIN</b> - This is the same as <code>NORMALIZE_PATH</code>, but first converts backslash characters to forward slashes. </p> <p> <b>REMOVE_NULLS</b> - Remove all <code>NULL</code> bytes from the input. </p> <p> <b>REPLACE_COMMENTS</b> - Replace each occurrence of a C-style comment (<code>/* ... */</code>) with a single space. Multiple consecutive occurrences are not compressed. Unterminated comments are also replaced with a space (ASCII 0x20). However, a standalone termination of a comment (<code>*/</code>) is not acted upon. </p> <p> <b>REPLACE_NULLS</b> - Replace NULL bytes in the input with space characters (ASCII <code>0x20</code>). </p> <p> <b>SQL_HEX_DECODE</b> - Decode SQL hex data. Example (<code>0x414243</code>) will be decoded to (<code>ABC</code>).</p> <p> <b>URL_DECODE</b> - Decode a URL-encoded value. </p> <p> <b>URL_DECODE_UNI</b> - Like <code>URL_DECODE</code>, but with support for Microsoft-specific <code>%u</code> encoding. If the code is in the full-width ASCII code range of <code>FF01-FF5E</code>, the higher byte is used to detect and adjust the lower byte. Otherwise, only the lower byte is used and the higher byte is zeroed. </p> <p> <b>UTF8_TO_UNICODE</b> - Convert all UTF-8 character sequences to Unicode. This helps input normalization, and minimizing false-positives and false-negatives for non-English languages.</p>",
                     "shape": "TextTransformationType"
                 }
             },
@@ -6036,15 +6786,15 @@
                     "shape": "LockToken"
                 },
                 "Name": {
                     "documentation": "<p>The name of the IP set. You cannot change the name of an <code>IPSet</code> after you create it.</p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Name",
                 "Scope",
                 "Id",
@@ -6077,15 +6827,15 @@
                     "shape": "LockToken"
                 },
                 "Name": {
                     "documentation": "<p>The name of the managed rule set. You use this, along with the rule set ID, to identify the rule set.</p> <p>This name is assigned to the corresponding managed rule group, which your customers can access and use. </p>",
                     "shape": "EntityName"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 },
                 "VersionToExpire": {
                     "documentation": "<p>The version that you want to remove from your list of offerings for the named managed rule group. </p>",
                     "shape": "VersionKeyString"
                 }
             },
@@ -6135,15 +6885,15 @@
                     "shape": "EntityName"
                 },
                 "RegularExpressionList": {
                     "documentation": "<p/>",
                     "shape": "RegularExpressionList"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 }
             },
             "required": [
                 "Name",
                 "Scope",
                 "Id",
@@ -6160,15 +6910,15 @@
                 }
             },
             "type": "structure"
         },
         "UpdateRuleGroupRequest": {
             "members": {
                 "CustomResponseBodies": {
-                    "documentation": "<p>A map of custom response keys and content bodies. When you create a rule with a block action, you can send a custom response to the web request. You define these for the rule group, and then use them in the rules that you define in the rule group. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>A map of custom response keys and content bodies. When you create a rule with a block action, you can send a custom response to the web request. You define these for the rule group, and then use them in the rules that you define in the rule group. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomResponseBodies"
                 },
                 "Description": {
                     "documentation": "<p>A description of the rule group that helps with identification. </p>",
                     "shape": "EntityDescription"
                 },
                 "Id": {
@@ -6184,15 +6934,15 @@
                     "shape": "EntityName"
                 },
                 "Rules": {
                     "documentation": "<p>The <a>Rule</a> statements used to identify the web requests that you want to allow, block, or count. Each rule includes one top-level statement that WAF uses to identify matching web requests, and parameters that govern how WAF handles them. </p>",
                     "shape": "Rules"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 },
                 "VisibilityConfig": {
                     "documentation": "<p>Defines and enables Amazon CloudWatch metrics and web request sample collection. </p>",
                     "shape": "VisibilityConfig"
                 }
             },
@@ -6212,24 +6962,28 @@
                     "shape": "LockToken"
                 }
             },
             "type": "structure"
         },
         "UpdateWebACLRequest": {
             "members": {
+                "AssociationConfig": {
+                    "documentation": "<p>Specifies custom configurations for the associations between the web ACL and protected resources. </p> <p>Use this to customize the maximum size of the request body that your protected CloudFront distributions forward to WAF for inspection. The default is 16 KB (16,384 kilobytes). </p> <note> <p>You are charged additional fees when your protected resources forward body sizes that are larger than the default. For more information, see <a href=\"http://aws.amazon.com/waf/pricing/\">WAF Pricing</a>.</p> </note>",
+                    "shape": "AssociationConfig"
+                },
                 "CaptchaConfig": {
                     "documentation": "<p>Specifies how WAF should handle <code>CAPTCHA</code> evaluations for rules that don't have their own <code>CaptchaConfig</code> settings. If you don't specify this, WAF uses its default settings for <code>CaptchaConfig</code>. </p>",
                     "shape": "CaptchaConfig"
                 },
                 "ChallengeConfig": {
                     "documentation": "<p>Specifies how WAF should handle challenge evaluations for rules that don't have their own <code>ChallengeConfig</code> settings. If you don't specify this, WAF uses its default settings for <code>ChallengeConfig</code>. </p>",
                     "shape": "ChallengeConfig"
                 },
                 "CustomResponseBodies": {
-                    "documentation": "<p>A map of custom response keys and content bodies. When you create a rule with a block action, you can send a custom response to the web request. You define these for the web ACL, and then use them in the rules and default actions that you define in the web ACL. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>A map of custom response keys and content bodies. When you create a rule with a block action, you can send a custom response to the web request. You define these for the web ACL, and then use them in the rules and default actions that you define in the web ACL. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomResponseBodies"
                 },
                 "DefaultAction": {
                     "documentation": "<p>The action to perform if none of the <code>Rules</code> contained in the <code>WebACL</code> match. </p>",
                     "shape": "DefaultAction"
                 },
                 "Description": {
@@ -6249,15 +7003,15 @@
                     "shape": "EntityName"
                 },
                 "Rules": {
                     "documentation": "<p>The <a>Rule</a> statements used to identify the web requests that you want to allow, block, or count. Each rule includes one top-level statement that WAF uses to identify matching web requests, and parameters that govern how WAF handles them. </p>",
                     "shape": "Rules"
                 },
                 "Scope": {
-                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, a Amazon Cognito user pool, or an App Runner service. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
+                    "documentation": "<p>Specifies whether this is for an Amazon CloudFront distribution or for a regional application. A regional application can be an Application Load Balancer (ALB), an Amazon API Gateway REST API, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p> <p>To work with CloudFront, you must also specify the Region US East (N. Virginia) as follows: </p> <ul> <li> <p>CLI - Specify the Region when you use the CloudFront scope: <code>--scope=CLOUDFRONT --region=us-east-1</code>. </p> </li> <li> <p>API and SDKs - For all calls, use the Region endpoint us-east-1. </p> </li> </ul>",
                     "shape": "Scope"
                 },
                 "TokenDomains": {
                     "documentation": "<p>Specifies the domains that WAF should accept in a web request token. This enables the use of tokens across multiple protected websites. When WAF provides a token, it uses the domain of the Amazon Web Services resource that the web ACL is protecting. If you don't specify a list of token domains, WAF accepts tokens only for the domain of the protected resource. With a token domain list, WAF accepts the resource's host domain plus all domains in the token domain list, including their prefixed subdomains.</p> <p>Example JSON: <code>\"TokenDomains\": { \"mywebsite.com\", \"myotherwebsite.com\" }</code> </p> <p>Public suffixes aren't allowed. For example, you can't use <code>usa.gov</code> or <code>co.uk</code> as token domains.</p>",
                     "shape": "TokenDomains"
                 },
                 "VisibilityConfig": {
@@ -6281,23 +7035,23 @@
                     "documentation": "<p>A token used for optimistic locking. WAF returns this token to your <code>update</code> requests. You use <code>NextLockToken</code> in the same manner as you use <code>LockToken</code>. </p>",
                     "shape": "LockToken"
                 }
             },
             "type": "structure"
         },
         "UriPath": {
-            "documentation": "<p>Inspect the path component of the URI of the web request. This is the part of the web request that identifies a resource. For example, <code>/images/daily-ad.jpg</code>.</p> <p>This is used only in the <a>FieldToMatch</a> specification for some web request component types. </p> <p>JSON specification: <code>\"UriPath\": {}</code> </p>",
+            "documentation": "<p>Inspect the path component of the URI of the web request. This is the part of the web request that identifies a resource. For example, <code>/images/daily-ad.jpg</code>.</p> <p>This is used in the <a>FieldToMatch</a> specification for some web request component types. </p> <p>JSON specification: <code>\"UriPath\": {}</code> </p>",
             "members": {},
             "type": "structure"
         },
         "UsernameField": {
-            "documentation": "<p>Details about your login page username field for request inspection, used in the <code>AWSManagedRulesATPRuleSet</code> <code>RequestInspection</code> configuration.</p>",
+            "documentation": "<p>The name of the field in the request payload that contains your customer's username. </p> <p>This data type is used in the <code>RequestInspection</code> and <code>RequestInspectionACFP</code> data types. </p>",
             "members": {
                 "Identifier": {
-                    "documentation": "<p>The name of the username field. For example <code>/form/username</code>.</p>",
+                    "documentation": "<p>The name of the username field. </p> <p>How you specify this depends on the request inspection payload type.</p> <ul> <li> <p>For JSON payloads, specify the field name in JSON pointer syntax. For information about the JSON Pointer syntax, see the Internet Engineering Task Force (IETF) documentation <a href=\"https://tools.ietf.org/html/rfc6901\">JavaScript Object Notation (JSON) Pointer</a>. </p> <p>For example, for the JSON payload <code>{ \"form\": { \"username\": \"THE_USERNAME\" } }</code>, the username field specification is <code>/form/username</code>. </p> </li> <li> <p>For form encoded payload types, use the HTML form names.</p> <p>For example, for an HTML form with the input element named <code>username1</code>, the username field specification is <code>username1</code> </p> </li> </ul>",
                     "shape": "FieldIdentifier"
                 }
             },
             "required": [
                 "Identifier"
             ],
             "type": "structure"
@@ -6337,23 +7091,23 @@
                 "shape": "VersionToPublish"
             }
         },
         "VisibilityConfig": {
             "documentation": "<p>Defines and enables Amazon CloudWatch metrics and web request sample collection. </p>",
             "members": {
                 "CloudWatchMetricsEnabled": {
-                    "documentation": "<p>A boolean indicating whether the associated resource sends metrics to Amazon CloudWatch. For the list of available metrics, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/monitoring-cloudwatch.html#waf-metrics\">WAF Metrics</a>.</p>",
+                    "documentation": "<p>Indicates whether the associated resource sends metrics to Amazon CloudWatch. For the list of available metrics, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/monitoring-cloudwatch.html#waf-metrics\">WAF Metrics</a> in the <i>WAF Developer Guide</i>.</p> <p>For web ACLs, the metrics are for web requests that have the web ACL default action applied. WAF applies the default action to web requests that pass the inspection of all rules in the web ACL without being either allowed or blocked. For more information, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/web-acl-default-action.html\">The web ACL default action</a> in the <i>WAF Developer Guide</i>.</p>",
                     "shape": "Boolean"
                 },
                 "MetricName": {
                     "documentation": "<p>A name of the Amazon CloudWatch metric dimension. The name can contain only the characters: A-Z, a-z, 0-9, - (hyphen), and _ (underscore). The name can be from one to 128 characters long. It can't contain whitespace or metric names that are reserved for WAF, for example <code>All</code> and <code>Default_Action</code>. </p>",
                     "shape": "MetricName"
                 },
                 "SampledRequestsEnabled": {
-                    "documentation": "<p>A boolean indicating whether WAF should store a sampling of the web requests that match the rules. You can view the sampled requests through the WAF console. </p>",
+                    "documentation": "<p>Indicates whether WAF should store a sampling of the web requests that match the rules. You can view the sampled requests through the WAF console. </p>",
                     "shape": "Boolean"
                 }
             },
             "required": [
                 "SampledRequestsEnabled",
                 "CloudWatchMetricsEnabled",
                 "MetricName"
@@ -6440,15 +7194,15 @@
                 "message": {
                     "shape": "ErrorMessage"
                 }
             },
             "type": "structure"
         },
         "WAFInvalidPermissionPolicyException": {
-            "documentation": "<p>The operation failed because the specified policy isn't in the proper format. </p> <p>The policy specifications must conform to the following:</p> <ul> <li> <p>The policy must be composed using IAM Policy version 2012-10-17 or version 2015-01-01.</p> </li> <li> <p>The policy must include specifications for <code>Effect</code>, <code>Action</code>, and <code>Principal</code>.</p> </li> <li> <p> <code>Effect</code> must specify <code>Allow</code>.</p> </li> <li> <p> <code>Action</code> must specify <code>wafv2:CreateWebACL</code>, <code>wafv2:UpdateWebACL</code>, and <code>wafv2:PutFirewallManagerRuleGroups</code> and may optionally specify <code>wafv2:GetRuleGroup</code>. WAF rejects any extra actions or wildcard actions in the policy.</p> </li> <li> <p>The policy must not include a <code>Resource</code> parameter.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html\">IAM Policies</a>. </p>",
+            "documentation": "<p>The operation failed because the specified policy isn't in the proper format. </p> <p>The policy specifications must conform to the following:</p> <ul> <li> <p>The policy must be composed using IAM Policy version 2012-10-17.</p> </li> <li> <p>The policy must include specifications for <code>Effect</code>, <code>Action</code>, and <code>Principal</code>.</p> </li> <li> <p> <code>Effect</code> must specify <code>Allow</code>.</p> </li> <li> <p> <code>Action</code> must specify <code>wafv2:CreateWebACL</code>, <code>wafv2:UpdateWebACL</code>, and <code>wafv2:PutFirewallManagerRuleGroups</code> and may optionally specify <code>wafv2:GetRuleGroup</code>. WAF rejects any extra actions or wildcard actions in the policy.</p> </li> <li> <p>The policy must not include a <code>Resource</code> parameter.</p> </li> </ul> <p>For more information, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html\">IAM Policies</a>. </p>",
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "ErrorMessage"
                 }
             },
             "type": "structure"
@@ -6550,35 +7304,49 @@
             "members": {
                 "Message": {
                     "shape": "ErrorMessage"
                 }
             },
             "type": "structure"
         },
+        "WAFUnsupportedAggregateKeyTypeException": {
+            "documentation": "<p>The rule that you've named doesn't aggregate solely on the IP address or solely on the forwarded IP address. This call is only available for rate-based rules with an <code>AggregateKeyType</code> setting of <code>IP</code> or <code>FORWARDED_IP</code>.</p>",
+            "exception": true,
+            "members": {
+                "Message": {
+                    "shape": "ErrorMessage"
+                }
+            },
+            "type": "structure"
+        },
         "WebACL": {
-            "documentation": "<p> A web ACL defines a collection of rules to use to inspect and control web requests. Each rule has an action defined (allow, block, or count) for requests that match the statement of the rule. In the web ACL, you assign a default action to take (allow, block) for any request that does not match any of the rules. The rules in a web ACL can be a combination of the types <a>Rule</a>, <a>RuleGroup</a>, and managed rule group. You can associate a web ACL with one or more Amazon Web Services resources to protect. The resources can be an Amazon CloudFront distribution, an Amazon API Gateway REST API, an Application Load Balancer, an AppSync GraphQL API, Amazon Cognito user pool, or an App Runner service. </p>",
+            "documentation": "<p> A web ACL defines a collection of rules to use to inspect and control web requests. Each rule has an action defined (allow, block, or count) for requests that match the statement of the rule. In the web ACL, you assign a default action to take (allow, block) for any request that does not match any of the rules. The rules in a web ACL can be a combination of the types <a>Rule</a>, <a>RuleGroup</a>, and managed rule group. You can associate a web ACL with one or more Amazon Web Services resources to protect. The resources can be an Amazon CloudFront distribution, an Amazon API Gateway REST API, an Application Load Balancer, an AppSync GraphQL API, an Amazon Cognito user pool, an App Runner service, or an Amazon Web Services Verified Access instance. </p>",
             "members": {
                 "ARN": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the web ACL that you want to associate with the resource.</p>",
                     "shape": "ResourceArn"
                 },
+                "AssociationConfig": {
+                    "documentation": "<p>Specifies custom configurations for the associations between the web ACL and protected resources. </p> <p>Use this to customize the maximum size of the request body that your protected CloudFront distributions forward to WAF for inspection. The default is 16 KB (16,384 kilobytes). </p> <note> <p>You are charged additional fees when your protected resources forward body sizes that are larger than the default. For more information, see <a href=\"http://aws.amazon.com/waf/pricing/\">WAF Pricing</a>.</p> </note>",
+                    "shape": "AssociationConfig"
+                },
                 "Capacity": {
-                    "documentation": "<p>The web ACL capacity units (WCUs) currently being used by this web ACL. </p> <p>WAF uses WCUs to calculate and control the operating resources that are used to run your rules, rule groups, and web ACLs. WAF calculates capacity differently for each rule type, to reflect the relative cost of each rule. Simple rules that cost little to run use fewer WCUs than more complex rules that use more processing power. Rule group capacity is fixed at creation, which helps users plan their web ACL WCU usage when they use a rule group. The WCU limit for web ACLs is 1,500. </p>",
+                    "documentation": "<p>The web ACL capacity units (WCUs) currently being used by this web ACL. </p> <p>WAF uses WCUs to calculate and control the operating resources that are used to run your rules, rule groups, and web ACLs. WAF calculates capacity differently for each rule type, to reflect the relative cost of each rule. Simple rules that cost little to run use fewer WCUs than more complex rules that use more processing power. Rule group capacity is fixed at creation, which helps users plan their web ACL WCU usage when they use a rule group. For more information, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/aws-waf-capacity-units.html\">WAF web ACL capacity units (WCU)</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "ConsumedCapacity"
                 },
                 "CaptchaConfig": {
                     "documentation": "<p>Specifies how WAF should handle <code>CAPTCHA</code> evaluations for rules that don't have their own <code>CaptchaConfig</code> settings. If you don't specify this, WAF uses its default settings for <code>CaptchaConfig</code>. </p>",
                     "shape": "CaptchaConfig"
                 },
                 "ChallengeConfig": {
                     "documentation": "<p>Specifies how WAF should handle challenge evaluations for rules that don't have their own <code>ChallengeConfig</code> settings. If you don't specify this, WAF uses its default settings for <code>ChallengeConfig</code>. </p>",
                     "shape": "ChallengeConfig"
                 },
                 "CustomResponseBodies": {
-                    "documentation": "<p>A map of custom response keys and content bodies. When you create a rule with a block action, you can send a custom response to the web request. You define these for the web ACL, and then use them in the rules and default actions that you define in the web ACL. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html\">WAF Developer Guide</a>. </p>",
+                    "documentation": "<p>A map of custom response keys and content bodies. When you create a rule with a block action, you can send a custom response to the web request. You define these for the web ACL, and then use them in the rules and default actions that you define in the web ACL. </p> <p>For information about customizing web requests and responses, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/waf-custom-request-response.html\">Customizing web requests and responses in WAF</a> in the <i>WAF Developer Guide</i>. </p> <p>For information about the limits on count and size for custom request and response settings, see <a href=\"https://docs.aws.amazon.com/waf/latest/developerguide/limits.html\">WAF quotas</a> in the <i>WAF Developer Guide</i>. </p>",
                     "shape": "CustomResponseBodies"
                 },
                 "DefaultAction": {
                     "documentation": "<p>The action to perform if none of the <code>Rules</code> contained in the <code>WebACL</code> match. </p>",
                     "shape": "DefaultAction"
                 },
                 "Description": {
@@ -6667,15 +7435,15 @@
             "documentation": "<p>A rule statement that inspects for cross-site scripting (XSS) attacks. In XSS attacks, the attacker uses vulnerabilities in a benign website as a vehicle to inject malicious client-site scripts into other legitimate web browsers. </p>",
             "members": {
                 "FieldToMatch": {
                     "documentation": "<p>The part of the web request that you want WAF to inspect. </p>",
                     "shape": "FieldToMatch"
                 },
                 "TextTransformations": {
-                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. If you specify one or more transformations in a rule statement, WAF performs all transformations on the content of the request component identified by <code>FieldToMatch</code>, starting from the lowest priority setting, before inspecting the content for a match.</p>",
+                    "documentation": "<p>Text transformations eliminate some of the unusual formatting that attackers use in web requests in an effort to bypass detection. Text transformations are used in rule match statements, to transform the <code>FieldToMatch</code> request component before inspecting it, and they're used in rate-based rule statements, to transform request components before using them as custom aggregation keys. If you specify one or more transformations to apply, WAF performs all transformations on the specified content, starting from the lowest priority setting, and then uses the component contents. </p>",
                     "shape": "TextTransformations"
                 }
             },
             "required": [
                 "FieldToMatch",
                 "TextTransformations"
             ],
```

### Comparing `botocore-a-la-carte-wafv2-1.29.99/botocore_a_la_carte_wafv2.egg-info/PKG-INFO` & `botocore-a-la-carte-wafv2-1.30.0/botocore_a_la_carte_wafv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-wafv2
-Version: 1.29.99
+Version: 1.30.0
 Summary: wafv2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-wafv2-1.29.99/setup.py` & `botocore-a-la-carte-wafv2-1.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-wafv2',
-    version="1.29.99",
+    version="1.30.0",
     description='wafv2 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/wafv2/*/*.json'],
```

