# Comparing `tmp/mend_ignore_alerts-0.3-py3-none-any.whl.zip` & `tmp/mend_ignore_alerts-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11914 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 15:25 mend_ignore_alerts/__init__.py
--rw-r--r--  2.0 unx      105 b- defN 23-Jul-03 15:25 mend_ignore_alerts/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 15:25 mend_ignore_alerts/conftest.py
--rw-r--r--  2.0 unx     1554 b- defN 23-Jul-03 15:25 mend_ignore_alerts/const.py
--rw-r--r--  2.0 unx    10650 b- defN 23-Jul-03 15:25 mend_ignore_alerts/ignore_alerts.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-03 15:25 mend_ignore_alerts-0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     5028 b- defN 23-Jul-03 15:25 mend_ignore_alerts-0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 15:25 mend_ignore_alerts-0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jul-03 15:25 mend_ignore_alerts-0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-03 15:25 mend_ignore_alerts-0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 23-Jul-03 15:25 mend_ignore_alerts-0.3.dist-info/RECORD
-11 files, 29844 bytes uncompressed, 10246 bytes compressed:  65.7%
+Zip file size: 11964 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 07:27 mend_ignore_alerts/__init__.py
+-rw-r--r--  2.0 unx      107 b- defN 23-Jul-04 07:27 mend_ignore_alerts/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 07:27 mend_ignore_alerts/conftest.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Jul-04 07:27 mend_ignore_alerts/const.py
+-rw-r--r--  2.0 unx    10726 b- defN 23-Jul-04 07:27 mend_ignore_alerts/ignore_alerts.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-04 07:27 mend_ignore_alerts-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5030 b- defN 23-Jul-04 07:27 mend_ignore_alerts-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 07:27 mend_ignore_alerts-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-04 07:27 mend_ignore_alerts-0.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-04 07:27 mend_ignore_alerts-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      979 b- defN 23-Jul-04 07:27 mend_ignore_alerts-0.3.1.dist-info/RECORD
+11 files, 29936 bytes uncompressed, 10272 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: mend_ignore_alerts/const.py
 Comment: 
 
 Filename: mend_ignore_alerts/ignore_alerts.py
 Comment: 
 
-Filename: mend_ignore_alerts-0.3.dist-info/LICENSE
+Filename: mend_ignore_alerts-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: mend_ignore_alerts-0.3.dist-info/METADATA
+Filename: mend_ignore_alerts-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: mend_ignore_alerts-0.3.dist-info/WHEEL
+Filename: mend_ignore_alerts-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: mend_ignore_alerts-0.3.dist-info/entry_points.txt
+Filename: mend_ignore_alerts-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.3.dist-info/top_level.txt
+Filename: mend_ignore_alerts-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.3.dist-info/RECORD
+Filename: mend_ignore_alerts-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_ignore_alerts/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "0.3"
+__version__ = "0.3.1"
 __tool_name__ = "ignore_alerts"
 __description__ = "Parse yml file and update alerts"
```

## mend_ignore_alerts/ignore_alerts.py

```diff
@@ -225,15 +225,16 @@
         })
         return f"{json.loads(call_ws_api(data=data))['message']}. Alert UUID {alert_uuid}"
     except:
         return f"Failed Ignore operation for alert UUID {alert_uuid}"
 
 
 def exec_input_yaml(input_data):
-    for el_ in input_data:
+    input_data_ = [input_data] if type(input_data) is dict else input_data
+    for el_ in input_data_:
         prj_token = get_token_by_prj_name(el_["name"])
         if prj_token:
             #restore_alerts(project=prj_token)
             ignored_al = get_ingnored_alerts(project=prj_token)
             alerts = get_alerts_by_type(prj_token=prj_token, alert_type="SECURITY_VULNERABILITY")
             try:
                 for data_ in el_["vulns"]:
```

## Comparing `mend_ignore_alerts-0.3.dist-info/LICENSE` & `mend_ignore_alerts-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_ignore_alerts-0.3.dist-info/METADATA` & `mend_ignore_alerts-0.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-ignore-alerts
-Version: 0.3
+Version: 0.3.1
 Summary: Parse yml file and update alerts
 Home-page: https://github.com/mend-toolkit/ignore-alerts
 Author: Mend Professional Services
 Author-email: ps@mend.io
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `mend_ignore_alerts-0.3.dist-info/RECORD` & `mend_ignore_alerts-0.3.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mend_ignore_alerts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_ignore_alerts/_version.py,sha256=eE95Bz_WwRjC_Hyk6gSe4K-noTDQLb2KRWjPRJRtBnA,105
+mend_ignore_alerts/_version.py,sha256=WNW2ShReXUp0v-qHX3NDr0Bt3oMWEHOL4_sIB1__KnE,107
 mend_ignore_alerts/conftest.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mend_ignore_alerts/const.py,sha256=aRDadkUul_6NZB_LDIZTkGf5VkWTPqfnj6eap-1Y7As,1554
-mend_ignore_alerts/ignore_alerts.py,sha256=EAu7IK8LKB0Y5k_VEgTWHnhpbPwOfi4JQrUftUaR1_o,10650
-mend_ignore_alerts-0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mend_ignore_alerts-0.3.dist-info/METADATA,sha256=DAaWr86KpIQo_WkTG6iG5xSlnWOvfTecEaxQOTvRcTI,5028
-mend_ignore_alerts-0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mend_ignore_alerts-0.3.dist-info/entry_points.txt,sha256=b_q3jF-WbTVm6sR0BrVXts8u1OhXtD1aM2IZ5CfWmpE,72
-mend_ignore_alerts-0.3.dist-info/top_level.txt,sha256=ookvTXlTz4JKFzjrBd6U6MmV6RzYs9C8B2E2vMscaZ8,19
-mend_ignore_alerts-0.3.dist-info/RECORD,,
+mend_ignore_alerts/ignore_alerts.py,sha256=yOHiByN3TXMZ8bNdDi62CkKKIEvGXVXrUQOB-QtwFNk,10726
+mend_ignore_alerts-0.3.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mend_ignore_alerts-0.3.1.dist-info/METADATA,sha256=uCdMj7UiFYVPMtzuwcesbThGcbigDwQqk_uwde2O3sI,5030
+mend_ignore_alerts-0.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mend_ignore_alerts-0.3.1.dist-info/entry_points.txt,sha256=b_q3jF-WbTVm6sR0BrVXts8u1OhXtD1aM2IZ5CfWmpE,72
+mend_ignore_alerts-0.3.1.dist-info/top_level.txt,sha256=ookvTXlTz4JKFzjrBd6U6MmV6RzYs9C8B2E2vMscaZ8,19
+mend_ignore_alerts-0.3.1.dist-info/RECORD,,
```

