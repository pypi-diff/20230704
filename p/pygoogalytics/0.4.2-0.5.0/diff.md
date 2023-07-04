# Comparing `tmp/pygoogalytics-0.4.2.tar.gz` & `tmp/pygoogalytics-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygoogalytics-0.4.2.tar", last modified: Wed Jun 21 15:32:22 2023, max compression
+gzip compressed data, was "pygoogalytics-0.5.0.tar", last modified: Tue Jul  4 11:40:18 2023, max compression
```

## Comparing `pygoogalytics-0.4.2.tar` & `pygoogalytics-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 15:32:22.869292 pygoogalytics-0.4.2/
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.4.2/LICENCE.txt
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.4.2/LICENSE
--rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-06-21 15:32:22.869171 pygoogalytics-0.4.2/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     5699 2023-05-10 09:11:02.000000 pygoogalytics-0.4.2/README.md
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 15:32:22.867430 pygoogalytics-0.4.2/pygoogalytics/
--rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-06-21 15:31:45.000000 pygoogalytics-0.4.2/pygoogalytics/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     3239 2023-06-21 13:16:26.000000 pygoogalytics-0.4.2/pygoogalytics/ads_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)     5678 2023-06-21 13:16:26.000000 pygoogalytics-0.4.2/pygoogalytics/client.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 15:32:22.868393 pygoogalytics-0.4.2/pygoogalytics/data/
--rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.4.2/pygoogalytics/data/country_iso_codes.csv
--rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.4.2/pygoogalytics/data/google_ads_location_ids.csv
--rw-r--r--   0 joshua     (501) staff       (20)    43521 2023-06-21 15:15:26.000000 pygoogalytics-0.4.2/pygoogalytics/googalytics_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)    39437 2023-06-21 15:15:26.000000 pygoogalytics-0.4.2/pygoogalytics/googlepandas.py
--rw-r--r--   0 joshua     (501) staff       (20)    42099 2023-05-09 12:29:00.000000 pygoogalytics-0.4.2/pygoogalytics/kwp_wrappers.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 15:32:22.868981 pygoogalytics-0.4.2/pygoogalytics/utils/
--rw-r--r--   0 joshua     (501) staff       (20)        0 2023-06-21 13:16:26.000000 pygoogalytics-0.4.2/pygoogalytics/utils/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     2804 2023-06-21 13:16:26.000000 pygoogalytics-0.4.2/pygoogalytics/utils/ads_reports_parsing.py
--rw-r--r--   0 joshua     (501) staff       (20)     1496 2023-06-21 15:15:26.000000 pygoogalytics-0.4.2/pygoogalytics/utils/ga4_parser.py
--rw-r--r--   0 joshua     (501) staff       (20)     2332 2023-06-21 13:42:17.000000 pygoogalytics-0.4.2/pygoogalytics/utils/general_utils.py
--rw-r--r--   0 joshua     (501) staff       (20)     2685 2023-06-21 13:16:26.000000 pygoogalytics-0.4.2/pygoogalytics/utils/resource_utils.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-06-21 15:32:22.868149 pygoogalytics-0.4.2/pygoogalytics.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-06-21 15:32:22.000000 pygoogalytics-0.4.2/pygoogalytics.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      670 2023-06-21 15:32:22.000000 pygoogalytics-0.4.2/pygoogalytics.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2023-06-21 15:32:22.000000 pygoogalytics-0.4.2/pygoogalytics.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)      113 2023-06-21 15:32:22.000000 pygoogalytics-0.4.2/pygoogalytics.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)       14 2023-06-21 15:32:22.000000 pygoogalytics-0.4.2/pygoogalytics.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2023-06-21 15:32:22.869328 pygoogalytics-0.4.2/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     1297 2023-06-21 15:31:45.000000 pygoogalytics-0.4.2/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-04 11:40:18.113817 pygoogalytics-0.5.0/
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.5.0/LICENCE.txt
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.5.0/LICENSE
+-rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-07-04 11:40:18.113672 pygoogalytics-0.5.0/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     5699 2023-05-10 09:11:02.000000 pygoogalytics-0.5.0/README.md
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-04 11:40:18.111213 pygoogalytics-0.5.0/pygoogalytics/
+-rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-07-04 11:40:14.000000 pygoogalytics-0.5.0/pygoogalytics/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3239 2023-06-21 13:16:26.000000 pygoogalytics-0.5.0/pygoogalytics/ads_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5678 2023-06-21 13:16:26.000000 pygoogalytics-0.5.0/pygoogalytics/client.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-04 11:40:18.112583 pygoogalytics-0.5.0/pygoogalytics/data/
+-rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.5.0/pygoogalytics/data/country_iso_codes.csv
+-rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.5.0/pygoogalytics/data/google_ads_location_ids.csv
+-rw-r--r--   0 joshua     (501) staff       (20)    40473 2023-07-04 11:40:14.000000 pygoogalytics-0.5.0/pygoogalytics/googalytics_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)    37705 2023-07-03 12:34:10.000000 pygoogalytics-0.5.0/pygoogalytics/googlepandas.py
+-rw-r--r--   0 joshua     (501) staff       (20)    42099 2023-05-09 12:29:00.000000 pygoogalytics-0.5.0/pygoogalytics/kwp_wrappers.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-04 11:40:18.113415 pygoogalytics-0.5.0/pygoogalytics/utils/
+-rw-r--r--   0 joshua     (501) staff       (20)        0 2023-06-21 13:16:26.000000 pygoogalytics-0.5.0/pygoogalytics/utils/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2804 2023-06-21 13:16:26.000000 pygoogalytics-0.5.0/pygoogalytics/utils/ads_reports_parsing.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3445 2023-07-03 12:25:40.000000 pygoogalytics-0.5.0/pygoogalytics/utils/ga4_parser.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3137 2023-06-29 09:27:17.000000 pygoogalytics-0.5.0/pygoogalytics/utils/general_utils.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2685 2023-06-21 13:16:26.000000 pygoogalytics-0.5.0/pygoogalytics/utils/resource_utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-04 11:40:18.112329 pygoogalytics-0.5.0/pygoogalytics.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     6443 2023-07-04 11:40:18.000000 pygoogalytics-0.5.0/pygoogalytics.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      670 2023-07-04 11:40:18.000000 pygoogalytics-0.5.0/pygoogalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2023-07-04 11:40:18.000000 pygoogalytics-0.5.0/pygoogalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)      113 2023-07-04 11:40:18.000000 pygoogalytics-0.5.0/pygoogalytics.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       14 2023-07-04 11:40:18.000000 pygoogalytics-0.5.0/pygoogalytics.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2023-07-04 11:40:18.113869 pygoogalytics-0.5.0/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     1297 2023-07-04 11:40:14.000000 pygoogalytics-0.5.0/setup.py
```

### Comparing `pygoogalytics-0.4.2/LICENCE.txt` & `pygoogalytics-0.5.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.2/LICENSE` & `pygoogalytics-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.2/PKG-INFO` & `pygoogalytics-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.4.2
+Version: 0.5.0
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.4.2/README.md` & `pygoogalytics-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.2/pygoogalytics/__init__.py` & `pygoogalytics-0.5.0/pygoogalytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   sc_domain='<search-console-domain>',
   view_id='<ga3-view-id>',
   ga4_property_id='<ga4-property-id>'
 )
 ```
 """
 
-__version__ = "0.4.2"
+__version__ = "0.5.0"
 __author__ = 'Joshua Prettyman'
 __credits__ = 'Blink SEO'
 
 import os
 import csv
 import logging
```

### Comparing `pygoogalytics-0.4.2/pygoogalytics/ads_wrapper.py` & `pygoogalytics-0.5.0/pygoogalytics/ads_wrapper.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.2/pygoogalytics/client.py` & `pygoogalytics-0.5.0/pygoogalytics/client.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.2/pygoogalytics/data/country_iso_codes.csv` & `pygoogalytics-0.5.0/pygoogalytics/data/country_iso_codes.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.2/pygoogalytics/data/google_ads_location_ids.csv` & `pygoogalytics-0.5.0/pygoogalytics/data/google_ads_location_ids.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.2/pygoogalytics/googalytics_wrapper.py` & `pygoogalytics-0.5.0/pygoogalytics/googalytics_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from googleapiclient.errors import HttpError as GoogleApiHttpError
 from google.api_core.exceptions import ResourceExhausted, InvalidArgument, PermissionDenied
 import google.analytics.data_v1beta.types as ga_data_types
 
 from . import googlepandas as gpd
 from .utils import general_utils
-from .utils.ga4_parser import parse_ga4_response
+from .utils.ga4_parser import parse_ga4_response, parse_ga3_response, join_ga4_responses
 from . import pga_logger
 
 
 class GoogalyticsWrapper:
     """
     The GoogalyticsWrapper requires the following arguments to access data:
     - for GSC data: sc_domain. This is the url-like string you see in the Google Search Console web application
@@ -240,109 +240,109 @@
                 print(f"{self.__class__.__name__}.get_gsc_response() :: empty gsc response")
             # raise EmptyResponseError("GSC", start_date=start_date, end_date=end_date)
             return None
 
         return gsc_response
 
     def get_ga3_response(self,
-                         start_date: Union[str, datetime.date],
-                         end_date: Optional[Union[str, datetime.date]] = None,
-                         ga_dimensions: Optional[Union[List[str], str]] = None,
-                         ga_metrics: Optional[Union[List[str], str]] = None,
-                         ga_filters: Optional[dict] = None,
+                         start_date: datetime.date,
+                         end_date: datetime.date,
+                         dimensions: list[str] | str | None = None,
+                         metrics: list[str] | str | None = None,
+                         ga_filters: dict | None = None,
                          raise_http_error: bool = False,
                          log_error: bool = True,
                          filter_google_organic: bool = False,
                          _print_log: bool = False) -> Optional[dict]:
 
+        if dimensions is None:
+            dimensions = ['productName']
+        elif isinstance(dimensions, str):
+            dimensions = dimensions.split('+')
+        dimensions = [re.sub(r"^ga:", "", _) for _ in dimensions]
+
+        if metrics is None:
+            metrics = ['itemRevenue']
+        elif isinstance(metrics, str):
+            metrics = [metrics]
+        metrics = [re.sub(r"^ga:", "", _) for _ in metrics]
+
+        ga_dimensions = ['ga:' + _s if not re.match(r'ga:', _s) else _s for _s in dimensions]
+        ga_metrics = ['ga:'+_s if not re.match(r'ga:', _s) else _s for _s in metrics]
+
         r = self._ga3_response_raw(
             start_date=start_date,
             end_date=end_date,
             ga_dimensions=ga_dimensions,
             ga_metrics=ga_metrics,
             ga_filters=ga_filters,
             filter_google_organic=filter_google_organic,
-            raise_http_error=raise_http_error,
-            log_error=log_error,
             page_token=None
         )
-        if r is None:
-            return None
 
         data = r.get('reports', [{}])[0].get('data', {}).get('rows', [])
         column_header = r.get('reports', [{}])[0].get('columnHeader')
         next_page_token = r.get('reports', [{}])[0].get('nextPageToken')
+        error = r.get('error', None)
+        error_type = r.get('error_type', None)
 
-        while next_page_token:
+        while next_page_token and not error:
             r = self._ga3_response_raw(
                 start_date=start_date,
                 end_date=end_date,
                 ga_dimensions=ga_dimensions,
                 ga_metrics=ga_metrics,
                 ga_filters=ga_filters,
                 filter_google_organic=filter_google_organic,
-                raise_http_error=raise_http_error,
                 page_token=next_page_token
             )
-            _d = r.get('reports', [{}])[0].get('data', {}).get('rows', [])
+            error = r.get('error', None)
+            error_type = r.get('error_type', None)
+            _d = r.get('reports', [dict()])[0].get('data', dict()).get('rows', [])
             data.extend(_d)
             next_page_token = r.get('reports', [{}])[0].get('nextPageToken')
 
-        synthetic_response = {
-            'reports': [
-                {
-                    'columnHeader': column_header,
-                    'data': {'rows': data}
-                }
-            ]
-        }
+        # print(f"\ndimensions: {ga_dimensions} \n"
+        #       f"metrics: {ga_metrics} \n "
+        #       f"data: len={len(data)}, \n"
+        #       f"error_type: {error_type} \n"
+        #       f"column_header: {column_header} \n")
 
-        return synthetic_response
+        response = parse_ga3_response(column_header=column_header, response_rows=data)
+
+        response['response_type'] = 'GA3'
+        response['start_date'] = start_date
+        response['end_date'] = end_date
+
+        response['error'] = error
+        response['error_type'] = error_type
+
+        return response
 
     def _ga3_response_raw(self,
-                          start_date: Union[str, datetime.date],
-                          end_date: Optional[Union[str, datetime.date]] = None,
-                          ga_dimensions: Optional[Union[List[str], str]] = None,
-                          ga_metrics: Optional[Union[List[str], str]] = None,
-                          ga_filters: Optional[dict] = None,
+                          start_date: datetime.date,
+                          end_date: datetime.date,
+                          ga_dimensions: list[str],
+                          ga_metrics: List[str],
+                          ga_filters: dict | None = None,
                           filter_google_organic: bool = False,
-                          raise_http_error: bool = False,
-                          log_error: bool = True,
                           return_raw_response: bool = False,
                           page_token: str = None,
                           _print_log: bool = False):
 
         if not self.view_id:
             # If there is no view_id we stop here and return None,
             # unless raise_http_error is True, in which case we continue to the execution and see what errors come up
             pga_logger.warning(f"{self.__class__.__name__}.get_ga3_response() :: view id is not set")
             if not raise_http_error:
                 return None
 
-        if end_date is None:
-            end_date = start_date
-
-        if isinstance(start_date, str):
-            start_date = datetime.datetime.strptime(start_date, "%Y-%m-%d").date()
-        if isinstance(end_date, str):
-            end_date = datetime.datetime.strptime(end_date, "%Y-%m-%d").date()
-
         start_date_string = start_date.strftime("%Y-%m-%d")
         end_date_string = end_date.strftime("%Y-%m-%d")
 
-        if ga_dimensions is None:
-            ga_dimensions = ['ga:productName']
-        elif isinstance(ga_dimensions, str):
-            ga_dimensions = ga_dimensions.split('+')
-
-        if ga_metrics is None:
-            ga_metrics = ['ga:itemRevenue']
-        elif isinstance(ga_metrics, str):
-            ga_metrics = [ga_metrics]
-
         _dfc = []  # dimension filter clauses
         _mfc = []  # metric filter clauses
         _orderby = []
 
         if ga_filters:
             for filter_dict in ga_filters:
                 if not isinstance(filter_dict.get('filters'), list):
@@ -376,147 +376,149 @@
             # 'dimensions': [{'name': 'ga:productName'}],
             # 'metrics': [{'expression': 'ga:itemRevenue'}]
             'dimensions': [{'name': _d} for _d in ga_dimensions],
             "dimensionFilterClauses": _dfc,
             "metricFilterClauses": _mfc,
             "orderBys": _orderby,
             'metrics': [{'expression': _m} for _m in ga_metrics],
-            'pageSize': 100000
+            'pageSize': 100_000
         }
 
         if page_token:
             _request_dict.update({'pageToken': page_token})
 
         ga3_request = {'reportRequests': [_request_dict]}
 
+        _error = None
+        _error_type = None
         try:
             ga3_response = self.ga3_resource.reports().batchGet(body=ga3_request).execute()
             if return_raw_response:
                 pga_logger.info(f"{self.__class__.__name__}.get_ga3_response() :: returning raw response")
                 return ga3_response
         except GoogleApiHttpError as http_error:
+            _error = http_error
             _msg = ''
             if re.match(".*user does not have sufficient permissions", repr(http_error).lower()):
+                _error_type = 'insufficient_permissions'
                 _msg = f"{self.__class__.__name__}.get_ga3_response() :: user does not have sufficient permissions"
             if re.match(".*viewid must be set", repr(http_error).lower()):
+                _error_type = 'missing_view_id'
                 _msg = f"{self.__class__.__name__}.get_ga3_response() :: view id is not set"
+            ga3_response = None
+        except Exception as _e:
+            _error = _e
+            _error_type = 'other'
+            ga3_response = None
 
-            if log_error and _msg:
-                pga_logger.error(_msg)
-
-            if raise_http_error:
-                raise http_error
-            else:
-                return None
+        if ga3_response is None:
+            ga3_response = dict()
+        else:
+            try:
+                _rows = ga3_response.get('reports', [])[0].get('data').get('rows', None)
+            except (AttributeError, KeyError) as _e:
+                _rows = None
+
+            if _rows is None:
+                _error = AttributeError('ga3_response in incorrect format.')
+                _error_type = 'empty_response'
+                pga_logger.debug(f"{self.__class__.__name__}.get_ga3_response() :: empty ga response")
+                # raise EmptyResponseError("GA3", start_date=start_date, end_date=end_date)
 
-        try:
-            _rows = ga3_response.get('reports', [])[0].get('data').get('rows', None)
-        except AttributeError:
-            _rows = None
-
-        if _rows is None:
-            pga_logger.debug(f"{self.__class__.__name__}.get_ga3_response() :: empty ga response")
-            # raise EmptyResponseError("GA3", start_date=start_date, end_date=end_date)
-            return None
+        ga3_response['error'] = _error
+        ga3_response['error_type'] = _error_type
 
         return ga3_response
 
     def _ga4_response_raw(self,
                          start_date: datetime.date,
                          end_date: datetime.date,
                          ga4_dimensions: list[ga_data_types.Dimension],
                          ga4_metrics: list[ga_data_types.Metric],
                          limit: int,
                          offset: int):
 
-        start_date_string = start_date.strftime("%Y-%m-%d")
-        end_date_string = end_date.strftime("%Y-%m-%d")
-
         request = ga_data_types.RunReportRequest(
             property=f"properties/{self.ga4_property_id}",
             dimensions=ga4_dimensions,
             metrics=ga4_metrics,
-            date_ranges=[ga_data_types.DateRange(start_date=start_date_string, end_date=end_date_string)],
+            date_ranges=[
+                ga_data_types.DateRange(
+                    start_date=start_date.strftime("%Y-%m-%d"),
+                    end_date=end_date.strftime("%Y-%m-%d")
+                )
+            ],
             limit=limit,
             offset=offset,
             return_property_quota=True
         )
         ga4_response = self.ga4_resource.run_report(request)
 
         return ga4_response
 
     def get_ga4_response(self,
-                         start_date: str | datetime.date,
-                         end_date: str | datetime.date | None = None,
-                         ga4_dimensions: list[str] | str | None = None,
-                         ga4_metrics: list[str] | str | None = None,
+                         start_date: datetime.date,
+                         end_date: datetime.date,
+                         ga_dimensions: list[str] | str | None = None,
+                         ga_metrics: list[str] | str | None = None,
                          filter_google_organic: bool = False,
                          raise_http_error: bool = False,
                          limit: int | None = None) -> (list, dict, Any):
 
         if not self.ga4_property_id:
             # If there is no view_id we stop here and return None,
             # unless raise_http_error is True, in which case we continue to the execution and see what errors come up
             pga_logger.warning(f"{self.__class__.__name__}.get_ga4_response() :: ga4_property_id is not set")
             if not raise_http_error:
                 return None
 
-        if end_date is None:
-            end_date = start_date
-
-        if isinstance(start_date, str):
-            start_date = datetime.datetime.strptime(start_date, "%Y-%m-%d").date()
-        if isinstance(end_date, str):
-            end_date = datetime.datetime.strptime(end_date, "%Y-%m-%d").date()
+        if ga_dimensions is None:
+            ga_dimensions = ["dateHour", "landingPage"]
+        elif isinstance(ga_dimensions, str):
+            ga_dimensions = [_.strip() for _ in ga_dimensions.split(',')]
 
-        if ga4_dimensions is None:
-            ga4_dimensions = ["dateHour", "landingPage"]
-        elif isinstance(ga4_dimensions, str):
-            ga4_dimensions = [_.strip() for _ in ga4_dimensions.split(',')]
-
-        if ga4_metrics is None:
-            ga4_metrics = ["totalUsers"]
-        elif isinstance(ga4_metrics, str):
-            ga4_metrics = [_.strip() for _ in ga4_metrics.split(',')]
+        if ga_metrics is None:
+            ga_metrics = ["totalUsers"]
+        elif isinstance(ga_metrics, str):
+            ga_metrics = [_.strip() for _ in ga_metrics.split(',')]
 
-        dimensions = [ga_data_types.Dimension(name=_) for _ in ga4_dimensions]
-        metrics = [ga_data_types.Metric(name=_) for _ in ga4_metrics]
+        dimensions = [ga_data_types.Dimension(name=_) for _ in ga_dimensions]
+        metrics = [ga_data_types.Metric(name=_) for _ in ga_metrics]
 
         request_limit = 100_000
         if limit is None:
             limit = 1_000_000_000
         elif limit < 100_000:
             request_limit = limit
 
         offset: int = 0
         complete: bool = False
         error_type: str | None = None
-        rows: list[dict] = []
-        metadata: list[dict] = []
+        responses: list[dict] = []
         error = None
 
         tokens_per_hour_consumed: int = 0
         tokens_per_day_consumed: int = 0
 
         while not complete:
             num_tries = 0
             success = False
-            _rows, _metadata = [], dict()
+            response = dict()
             while num_tries < 3 and not success:
                 error = None
                 try:
                     ga4_response = self._ga4_response_raw(
                         start_date=start_date,
                         end_date=end_date,
                         ga4_dimensions=dimensions,
                         ga4_metrics=metrics,
                         limit=request_limit,
                         offset=offset
                     )
-                    _rows, _metadata = parse_ga4_response(ga4_response)
+                    response = parse_ga4_response(ga4_response)
                     success = True
                 except PermissionDenied as _permission_denied_error:
                     complete = True
                     error_type = 'permission_denied'
                     error = _permission_denied_error
                     num_tries = 7
                 except ResourceExhausted as _resource_exhausted_error:
@@ -531,42 +533,44 @@
                     error = _invalid_argument_error
                     num_tries = 7
                 except Exception as _e:
                     error = _e
                     num_tries += 1
 
             if success:
-                rows_returned = len(_rows)
-                offset += rows_returned
+                offset += response.get('row_count', 0)
                 if offset >= limit:
                     complete = True
-                if rows_returned == 0 or offset >= _metadata.get('meta_row_count', 1_000_000_000):
+                if response.get('row_count', 0) == 0 or offset >= response.get('meta_row_count', 1_000_000_000):
                     complete = True
 
-                tokens_per_hour_consumed += _metadata.get('quota', dict()).get('tokens_per_hour', dict()).get('consumed', 0)
-                tokens_per_day_consumed += _metadata.get('quota', dict()).get('tokens_per_day', dict()).get('consumed', 0)
+                responses.append(response)
 
-                rows.extend(_rows)
-                metadata.append(_metadata)
-
-        response = dict()
-        if len(metadata) > 0:
-            response = metadata[-1]
-            response['quota']['tokens_per_hour']['consumed'] = tokens_per_hour_consumed
-            response['quota']['tokens_per_day']['consumed'] = tokens_per_day_consumed
+        if len(responses) > 1:
+            response = join_ga4_responses(responses)
+            if response.get('row_count', 0) == 0:
+                error = AttributeError("Empty response")
+                error_type = "empty_response"
+        elif len(responses) == 1:
+            response = responses[0]
+            if response.get('row_count', 0) == 0:
+                error = AttributeError("Empty response")
+                error_type = "empty_response"
         else:
-            response['response_type'] = 'GA4'
-            response['dimension_headers'] = ga4_dimensions
-            response['metric_headers'] = ga4_metrics
+            response = {
+                'response_type': 'GA4',
+                'dimension_headers': ga_dimensions,
+                'metric_headers': ga_metrics,
+                'rows': []
+            }
+
+
 
-        response['response_type'] = 'GA4'
         response['start_date'] = start_date
         response['end_date'] = end_date
-        response['total_rows'] = offset
-        response['rows'] = rows
 
         response['error'] = error
         response['error_type'] = error_type
 
         return response
 
     def get_dates(self,
@@ -631,15 +635,16 @@
                dimensions: Optional[Union[str, List[str]]] = None,
                metrics: Optional[Union[str, List[str]]] = None,
                row_limit: Optional[int] = None,
                url_list: Optional[Union[str, List[str]]] = None,
                filter_google_organic: bool = False,
                filters: List[dict] = None,
                add_boolean_metrics: bool = False,
-               _return_response: bool = False
+               _return_response: bool = False,
+               raise_errors: bool = True
                ) -> Union[gpd.GADataFrame, gpd.GSCDataFrame, pd.DataFrame]:
         """
         The `get_df` method accepts the following values for the `result` argument:
         - "GSC": for Google Search Console data
         - "GA3": for Google Analytics 3 (UA) data
         - "URL": for Google Search Console URL inspection data
         - "GA4": for Google Analytics 4 data (note, this is not yet available in production)
@@ -663,31 +668,38 @@
             dimensions = [dimensions]
         if isinstance(metrics, str):
             metrics = [metrics]
         if isinstance(url_list, str):
             url_list = [url_list]
 
         if re.match(r"GA4", result):
-            return self._get_ga4_df(start_date=start_date,
-                                    end_date=end_date,
-                                    ga_dimensions=dimensions,
-                                    ga_metrics=metrics,
-                                    add_boolean_metrics=add_boolean_metrics,
-                                    filter_google_organic=filter_google_organic,
-                                    limit=row_limit,
-                                    filters=filters,
-                                    return_response=_return_response)
+            return self._get_analytics_df(
+                response_type='GA4',
+                start_date=start_date,
+                end_date=end_date,
+                ga_dimensions=dimensions,
+                ga_metrics=metrics,
+                add_boolean_metrics=add_boolean_metrics,
+                limit=row_limit,
+                filters=filters,
+                return_response=_return_response,
+                raise_errors=raise_errors
+            )
         elif re.match(r"GA3", result):
-            return self._get_ga3_df(start_date=start_date,
-                                    end_date=end_date,
-                                    ga_dimensions=dimensions,
-                                    ga_metrics=metrics,
-                                    add_boolean_metrics=add_boolean_metrics,
-                                    filter_google_organic=filter_google_organic,
-                                    filters=filters)
+            return self._get_analytics_df(
+                response_type='GA3',
+                start_date=start_date,
+                end_date=end_date,
+                ga_dimensions=dimensions,
+                ga_metrics=metrics,
+                filters=filters,
+                add_boolean_metrics=add_boolean_metrics,
+                raise_errors=raise_errors,
+                return_response=_return_response
+            )
         elif re.match(r"GSC", result) and result != "GSCQ":
             if row_limit is None:
                 row_limit = 100000
             return self._get_gsc_df(start_date=start_date,
                                     end_date=end_date,
                                     gsc_dimensions=dimensions,
                                     row_limit=row_limit,
@@ -778,48 +790,73 @@
         if add_boolean_metrics:
             gsc_df.add_question_column()
             gsc_df.add_transactional_column()
             gsc_df.add_investigation_column()
 
         return gsc_df
 
-    def _get_ga4_df(self,
-                    start_date: datetime.date,
-                    end_date: datetime.date,
+    def _get_analytics_df(self,
+                    response_type: str,
+                    start_date: datetime.date | str,
+                    end_date: datetime.date | str | None = None,
                     ga_dimensions: Optional[List[str]] = None,
                     ga_metrics: list[str] | list[list[str]] = None,
                     add_boolean_metrics: bool = True,
                     filters: Optional[dict] = None,
                     limit: int | None = 100_000_000,
                     return_response: bool = False,
-                    raise_errors: bool = False,
-                    filter_google_organic: bool = False) -> gpd.GADataFrame:
+                    raise_errors: bool = True) -> gpd.GADataFrame:
+
+        if not end_date:
+            end_date = start_date
+        if isinstance(start_date, str):
+            start_date = general_utils.parse_date(start_date)
+        if isinstance(end_date, str):
+            end_date = general_utils.parse_date(end_date)
+        if end_date < start_date:
+            raise ValueError("date range incompatible: end_date < start_date")
+        if start_date > datetime.date.today():
+            raise ValueError("date range incompatible: start_date in the future")
 
         if all(isinstance(_, str) for _ in ga_metrics):
             ga_metrics = [ga_metrics]
 
         metrics_list: list[list[str]] = []
         for _list in ga_metrics:
             metrics_list.extend([_list[10 * i:10 * i + 10] for i in range((len(_list) - 1) // 10 + 1)])
 
         responses: list = []
         breaking_error: bool = False
         breaking_error_type: str | None = None
         for _ga_metrics in metrics_list:
-            _r = self.get_ga4_response(
-                            start_date=start_date,
-                            end_date=end_date,
-                            ga4_dimensions=ga_dimensions,
-                            ga4_metrics=_ga_metrics,
-                            limit=limit,
-                        )
+            if response_type == 'GA3':
+                _r = self.get_ga3_response(
+                    start_date=start_date,
+                    end_date=end_date,
+                    dimensions=ga_dimensions,
+                    ga_filters=filters,
+                    metrics=_ga_metrics,
+                    raise_http_error=False
+                )
+            elif response_type == 'GA4':
+                _r = self.get_ga4_response(
+                    start_date=start_date,
+                    end_date=end_date,
+                    ga_dimensions=ga_dimensions,
+                    ga_metrics=_ga_metrics,
+                    raise_http_error=False,
+                    limit=limit
+                )
+            else:
+                raise KeyError("response_type not recognised")
+
             responses.append(_r)
-            if _t := _r.get('error_type') is not None:
+            if _r.get('error_type') is not None:
                 breaking_error = True
-                breaking_error_type = _t
+                breaking_error_type = _r.get('error_type')
                 break
 
         if return_response:
             return responses
 
         if raise_errors:
             _errors = [_r.get('error') for _r in responses if _r.get('error') is not None]
@@ -827,139 +864,51 @@
                 raise _errors[0]
 
         if breaking_error:
             frames = []
         else:
             frames = [gpd.from_response(response=_r) for _r in responses]
 
+        # if len(frames)>0:
+        #     return frames
+
         if len(frames) == 0:
-            ga4_df = gpd.GADataFrame(df_input=None,
+            dataframe = gpd.GADataFrame(df_input=None,
                                      dimensions=ga_dimensions,
-                                     metrics=ga_metrics,
+                                     metrics=general_utils.expand_list(ga_metrics),
                                      start_date=start_date,
                                      end_date=end_date,
                                      error = breaking_error_type)
 
         elif all(len(_frame) == 0 for _frame in frames):
-            ga4_df = gpd.GADataFrame(df_input=None,
+            dataframe = gpd.GADataFrame(df_input=None,
                                      dimensions=ga_dimensions,
-                                     metrics=ga_metrics,
+                                     metrics=general_utils.expand_list(ga_metrics),
                                      start_date=start_date,
-                                     end_date=end_date)
+                                     end_date=end_date,
+                                        error = breaking_error_type)
         elif len(frames) == 1:
-            ga4_df = frames[0]
+            dataframe = frames[0]
         else:
-            ga4_df = frames[0]
+            dataframe = frames[0]
             for i in range(1, len(frames)):
-                ga4_df = ga4_df.join_on_dimensions(frames[i], how="outer")
+                dataframe = dataframe.join_on_dimensions(frames[i], how="outer")
 
         if add_boolean_metrics:
-            ga4_df.add_google_organic_column()
-            ga4_df.add_has_item_column()
-            ga4_df.add_new_user_column()
-            ga4_df.add_shopping_stage_all_column()
-            ga4_df.add_has_site_search_column()
+            dataframe.add_google_organic_column()
+            dataframe.add_has_item_column()
+            dataframe.add_new_user_column()
+            dataframe.add_shopping_stage_all_column()
+            dataframe.add_has_site_search_column()
 
-        ga4_df.fill_nan_with_zeros()
+        dataframe.fill_nan_with_zeros()
 
-        return ga4_df
+        return dataframe
 
 
-    def _get_ga3_df(self,
-                    start_date: datetime.date,
-                    end_date: datetime.date,
-                    ga_dimensions: list[str] | None = None,
-                    ga_metrics: list[str] | None = None,
-                    add_boolean_metrics: bool = True,
-                    filters: dict | None = None,
-                    filter_google_organic: bool = False) -> Optional[gpd.GADataFrame]:
-
-        if ga_dimensions is None:
-            ga_dimensions = ['ga:date',
-                             'ga:landingPagePath',
-                             'ga:productName',
-                             'ga:source',
-                             'ga:medium']
-
-        if ga_metrics is None:
-            ga_metrics = ['ga:itemRevenue',
-                          'ga:itemQuantity',
-                          'ga:users',
-                          'ga:newUsers',
-                          'ga:sessions',
-                          'ga:sessionDuration']
-        else:
-            ga_metrics = list(ga_metrics)
-
-        metrics_list = [ga_metrics[10 * i:10 * i + 10] for i in range((len(ga_metrics) - 1) // 10 + 1)]
-
-        frames = []
-        for metrics in metrics_list:
-            ga3_response = self.get_ga3_response(
-                start_date=start_date,
-                end_date=end_date,
-                ga_dimensions=ga_dimensions,
-                ga_metrics=metrics,
-                ga_filters=filters,
-                filter_google_organic=filter_google_organic
-            )
-
-            if ga3_response is not None:
-                # Make a dataframe of the ga response
-                ga3_df = gpd.from_response(response=ga3_response,
-                                           response_type="GA3",
-                                           start_date=start_date,
-                                           end_date=end_date)
-            else:
-                ga3_df = gpd.GADataFrame(df_input=None,
-                                         response_type='GA3',
-                                         dimensions=ga_dimensions,
-                                         metrics=metrics,
-                                         start_date=start_date,
-                                         end_date=end_date)
-            frames.append(ga3_df)
-
-        if all(len(_frame) == 0 for _frame in frames):
-            ga3_df = gpd.GADataFrame(df_input=None,
-                                     response_type='GA3',
-                                     dimensions=ga_dimensions,
-                                     metrics=ga_metrics,
-                                     start_date=start_date,
-                                     end_date=end_date)
-        else:
-            join_dimensions = frames[0].join_dimensions
-            if not all(set(_df.join_dimensions) == set(join_dimensions) for _df in frames):
-                print(f"{start_date} - {end_date}:")
-                for _i, _df in enumerate(frames):
-                    print(f"\t{_i} :")
-                    print(f"\t\tlength:     {len(_df)}")
-                    print(f"\t\tmetrics:    {_df.metrics}")
-                    print(f"\t\tdimensions: {_df.join_dimensions}")
-                raise AssertionError("unmatched join dimensions")
-            ga3_df = frames[0]
-            for i in range(1, len(frames)):
-                ga3_df = pd.merge(ga3_df, frames[i], how="outer", on=join_dimensions)
-            ga3_df = gpd.GADataFrame(df_input=ga3_df,
-                                     response_type='GA3',
-                                     dimensions=ga_dimensions,
-                                     metrics=ga_metrics,
-                                     from_ga_response=False,
-                                     join_dimensions=join_dimensions,
-                                     start_date=start_date,
-                                     end_date=end_date)
-
-        if add_boolean_metrics:
-            ga3_df.add_google_organic_column()
-            ga3_df.add_has_item_column()
-            ga3_df.add_new_user_column()
-            ga3_df.add_shopping_stage_all_column()
-            ga3_df.add_has_site_search_column()
-
-        return ga3_df
-
     def urlinspection_dict(self, url: str, inspection_index: int = None) -> dict:
         _now = datetime.datetime.utcnow()
         _d = {"record_date": _now.date(),
               "record_time": _now.time(),
               "url": url}
 
         try:
@@ -1009,7 +958,9 @@
             url_list = [url_list]
         pga_logger.info(f"{self.__class__.__name__}.get_urlinspection_df() :: "
                         f"requesting url inspection for {len(url_list)} urls")
         _frames = []
         for _i, url in enumerate(url_list):
             _frames.append(self.urlinspection_dict(url, inspection_index=_i))
         return pd.DataFrame(_frames)
+
+
```

### Comparing `pygoogalytics-0.4.2/pygoogalytics/googlepandas.py` & `pygoogalytics-0.5.0/pygoogalytics/googlepandas.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,61 +7,61 @@
 import datetime
 
 from google.analytics.data_v1beta.types.analytics_data_api import RunReportResponse
 
 from typing import List, Optional, Union, Pattern
 
 from .utils import general_utils
-from .utils.ga4_parser import parse_ga4_response
+from .utils.ga4_parser import parse_ga4_response, parse_ga3_response
 
 gpd_logger = logging.getLogger("googlepandas")
 
 
 def camel_to_snake(string: str):
     return general_utils.RE_C2S.sub('_', string).lower()
 
 
 GA_Types = {
-    'ga:date': str,
-    'ga:dateHourMinute': str,
-    'ga:landingPagePath': str,
-    'ga:pagePath': str,
-    'ga:productName': str,
-    'ga:productSku': str,
-    'ga:productListName': str,
-    'ga:productListPosition': str,
-    'ga:source': str,
-    'ga:medium': str,
-    'ga:sourceMedium': str,
-    'ga:channelGrouping': str,
-    'ga:referralPath': str,
-    'ga:campaign': str,
-    'ga:keyword': str,
-    'ga:deviceCategory': str,
-    'ga:countryIsoCode': str,
-    'ga:itemRevenue': float,
-    'ga:itemQuantity': float,
-    'ga:users': int,
-    'ga:timeOnPage': float,
-    'ga:newUsers': int,
-    'ga:sessions': int,
-    'ga:sessionDuration': float,
-    'ga:transactionsPerSession': float,  # i.e. conversion_rate
-    'ga:bounceRate': float,
-    'ga:transactions': float,
-    'ga:transactionRevenue': float,
-    'ga:pageViews': float,
-    'ga:pageviewsPerSession': float,
-    'ga:avgTimeOnPage': float,
-    'ga:avgPageLoadTime': float,
-    'ga:exits': int,
-    'ga:productDetailViews': float,
-    'ga:productListCTR': float,
-    'ga:productListClicks': float,
-    'ga:productListViews': float
+    'date': str,
+    'dateHourMinute': str,
+    'landingPagePath': str,
+    'pagePath': str,
+    'productName': str,
+    'productSku': str,
+    'productListName': str,
+    'productListPosition': str,
+    'source': str,
+    'medium': str,
+    'sourceMedium': str,
+    'channelGrouping': str,
+    'referralPath': str,
+    'campaign': str,
+    'keyword': str,
+    'deviceCategory': str,
+    'countryIsoCode': str,
+    'itemRevenue': float,
+    'itemQuantity': float,
+    'users': int,
+    'timeOnPage': float,
+    'newUsers': int,
+    'sessions': int,
+    'sessionDuration': float,
+    'transactionsPerSession': float,  # i.e. conversion_rate
+    'bounceRate': float,
+    'transactions': float,
+    'transactionRevenue': float,
+    'pageViews': float,
+    'pageviewsPerSession': float,
+    'avgTimeOnPage': float,
+    'avgPageLoadTime': float,
+    'exits': int,
+    'productDetailViews': float,
+    'productListCTR': float,
+    'productListClicks': float,
+    'productListViews': float
 }
 
 
 def from_response(response: dict | RunReportResponse,
                   response_type: str = None,
                   report_index: int = 0,
                   gsc_dimensions: Optional[List[str]] = None,
@@ -69,64 +69,52 @@
                   end_date: datetime.date = None):
     # We're going to what kind of response this is by making assumptions about what the responses will look like.
     # If the response dictionary includes a 'report' key, we assume it is a GA response.
     # If the response dictionary includes a 'rows' key with returns
     if response_type is None:
         response_type = get_response_type(response)
 
-    if response_type == 'GA3':
-        rows = response.get('reports', [])[report_index]['data']['rows']
-        dimensions = response.get('reports')[report_index].get('columnHeader').get('dimensions')
-        _metric_header_entries = response.get('reports')[report_index] \
-            .get('columnHeader') \
-            .get('metricHeader') \
-            .get('metricHeaderEntries')
-        metrics = [_d['name'] for _d in _metric_header_entries]
-        gpd_logger.debug(f"from_response: creating GADataFrame. dimensions = [{dimensions}], metrics = [{metrics}]")
-        return GADataFrame(df_input=rows,
-                           response_type='GA3',
-                           dimensions=dimensions, metrics=metrics,
-                           start_date=start_date, end_date=end_date,
-                           from_ga_response=True)
-    elif response_type == 'GA4':
+    if response_type == 'GA3' or response_type == 'GA4':
         if isinstance(response, RunReportResponse):
-            rows, metadata = parse_ga4_response(response)
-            return GADataFrame(df_input=rows,
-                               response_type='GA4',
-                               dimensions=metadata.get('dimension_headers'),
-                               metrics=metadata.get('metric_headers'),
-                               row_count=metadata.get('row_count'),
-                               start_date=start_date, end_date=end_date,
-                               from_ga_response=True)
-        else:
-            rows = response.get('rows')
-            from_ga_response = True
-            if len(rows) == 0:
-                rows = None
-                from_ga_response = False
-            return GADataFrame(df_input=rows,
-                               response_type='GA4',
-                               dimensions=response.get('dimension_headers'),
-                               metrics=response.get('metric_headers'),
-                               row_count=response.get('total_row_count'),
-                               start_date=response.get('start_date'),
-                               end_date=response.get('end_date'),
-                               error=response.get('error_type'),
-                               from_ga_response=from_ga_response)
+            response = parse_ga4_response(response)
+        elif response.get('reports', None):
+            response = parse_ga3_response(response)
+        return from_standard_analytics_response(response, start_date=start_date, end_date=end_date)
 
     elif response_type == 'GSC':
         rows = response.get('rows', [])
         response_aggregation = response.get('responseAggregationType', None)
         gpd_logger.debug("from_response: creating GSCDataFrame")
         _gsc_df = GSCDataFrame(df_input=rows,
                                gsc_dimensions=gsc_dimensions,
                                from_gsc_response=True)
         _gsc_df.response_aggregation = response_aggregation
         return _gsc_df
 
+def from_standard_analytics_response(response: dict, start_date: datetime.date=None, end_date: datetime.date=None):
+    rows = response.get('rows')
+    from_ga_response = True
+    if len(rows) == 0:
+        rows = None
+        from_ga_response = False
+
+    if response.get('start_date'):
+        start_date = response.get('start_date')
+    if response.get('end_date'):
+        end_date = response.get('end_date')
+
+    return GADataFrame(df_input=rows,
+                       response_type='GA4',
+                       dimensions=response.get('dimension_headers'),
+                       metrics=response.get('metric_headers'),
+                       row_count=response.get('row_count'),
+                       start_date=start_date,
+                       end_date=end_date,
+                       error=response.get('error_type'),
+                       from_ga_response=from_ga_response)
 
 def from_csv(csv_file_path):
     pandas_df = pd.read_csv(csv_file_path)
     r_type = response_type_from_file(csv_file_path)
     if r_type == 'GA':
         gpd_logger.debug("creating GADataFrame from csv")
         return GADataFrame(df_input=pandas_df,
@@ -139,16 +127,14 @@
 
 class GADataFrame(pd.DataFrame):
     """
     Subclass of pandas.DataFrame specifically for use with Google Analytics responses.
     The subclass must be initialized with a GA response object and will create a dataframe
     from the report indexed by `report_index` (default 0).
 
-    The DataFrame column headings are the same as the GA dimensions and metrics but without the 'ga:' prefix
-
     In addition to pandas DataFrame functionality, the GADataFrame has additional metadata attributes:
         dimensions:      list of the GA dimensions returned in the response
         metrics:         list of the GA metrics returned in the response
         brand_regex_dict:     dictionary of regex patterns supplied to __init__()
         category_regex_dict: dictionary of regex patterns supplied to __init__()
     """
 
@@ -198,16 +184,16 @@
 
         if start_date and end_date:
             self.date_range_days = (end_date - start_date).days + 1
         else:
             self.date_range_days = None
 
         if df_input is None:
-            self.join_dimensions = [strip_ga_prefix(_) for _ in self.dimensions]
-            super().__init__(None, columns=[strip_ga_prefix(_) for _ in dimensions + metrics])
+            self.join_dimensions = self.dimensions
+            super().__init__(None, columns=dimensions + metrics)
 
             if 'landingPagePlusQueryString' in self.columns:
                 self.rename(columns={'landingPagePlusQueryString': 'landingPagePath'}, inplace=True)
                 self.remove_join_dimensions('landingPagePlusQueryString')
                 self.add_join_dimensions('landingPagePath')
 
             if 'landingPagePath' in self.columns:
@@ -215,18 +201,23 @@
                 # 'landingPage' and 'landingPageParameter'
                 self.rename(columns={'landingPagePath': 'landingPageFull'}, inplace=True)
                 self['landingPage'] = None
                 self['landingPageParameter'] = None
                 self.remove_join_dimensions('landingPagePath')
                 self.add_join_dimensions(['landingPage', 'landingPageFull', 'landingPageParameter'])
 
+            if 'countryId' in self.columns:
+                self.rename(columns={'countryId': 'countryIsoCode'}, inplace=True)
+                self.remove_join_dimensions('countryId')
+                self.add_join_dimensions('countryIsoCode')
+
             if 'deviceCategory' in self.columns:
                 self.rename(columns={'deviceCategory': 'device'}, inplace=True)
                 self.remove_join_dimensions('deviceCategory')
-                self.add_join_dimensions(['device'])
+                self.add_join_dimensions('device')
 
             if 'sourceMedium' in self.columns:
                 self['source'] = None
                 self['medium'] = None
                 self.drop(columns='sourceMedium', inplace=True)
                 self.remove_join_dimensions('sourceMedium')
                 self.add_join_dimensions(['source', 'medium'])
@@ -239,14 +230,16 @@
                 self.add_join_dimensions(['source', 'medium'])
 
             if 'transactionsPerSession' in self.columns:
                 self.rename(columns={'transactionsPerSession': 'conversionRate'}, inplace=True)
 
             if 'itemPurchaseQuantity' in self.columns:
                 self.rename(columns={'itemPurchaseQuantity': 'itemQuantity'}, inplace=True)
+                self.metrics = remove_list_item(self.metrics, 'itemPurchaseQuantity')
+                self.metrics.append('itemQuantity')
 
             if 'date' in self.columns:
                 self.rename(columns={'date': 'recordDate'}, inplace=True)
                 self.remove_join_dimensions('date')
                 self.add_join_dimensions(['recordDate'])
 
             if 'dateHourMinute' in self.columns:
@@ -265,30 +258,14 @@
 
             self.snake_case_join_dimensions()
 
         else:
             super().__init__(df_input)
 
         if from_ga_response:
-            if response_type == 'GA3':
-                for _i in range(len(self.metrics) - 1, -1, -1):
-                    self.insert(loc=0, column=strip_ga_prefix(self.metrics[_i]),
-                                value=self['metrics'].apply(lambda x: x[0].get('values')[_i]
-                                                            ).astype(GA_Types.get(self.metrics[_i], str))
-                                )
-                self.drop(columns='metrics', inplace=True)
-
-                for _i in range(len(self.dimensions) - 1, -1, -1):
-                    self.insert(loc=0, column=strip_ga_prefix(self.dimensions[_i]),
-                                value=self['dimensions'].apply(lambda x: x[_i]
-                                                               ).astype(GA_Types.get(self.dimensions[_i], str))
-                                )
-                self.drop(columns='dimensions', inplace=True)
-                self.join_dimensions = [strip_ga_prefix(_) for _ in self.dimensions]
-
             if 'productName' in self.columns:
                 self['productName'] = self['productName'].apply(lambda s: s.strip().lower()
                                                                 .replace('-', ' ')
                                                                 .replace('_', ' ')
                                                                 .replace('&amp;', '&')
                                                                 )
                 self['productName'] = self['productName'].apply(lambda s: re.sub(r"\\u[a-f\d]{4}", " ", s))
@@ -297,14 +274,16 @@
             if 'landingPagePlusQueryString' in self.columns:
                 self.rename(columns={'landingPagePlusQueryString': 'landingPagePath'}, inplace=True)
                 self.remove_join_dimensions('landingPagePlusQueryString')
                 self.add_join_dimensions('landingPagePath')
 
             if 'itemPurchaseQuantity' in self.columns:
                 self.rename(columns={'itemPurchaseQuantity': 'itemQuantity'}, inplace=True)
+                self.metrics = remove_list_item(self.metrics, 'itemPurchaseQuantity')
+                self.metrics.append('itemQuantity')
 
             if 'landingPagePath' in self.columns:
                 self['landingPagePath'] = self['landingPagePath'].apply(general_utils.url_strip_domain)
                 self['landingPage'] = self['landingPagePath'].apply(lambda _u: _u.split('?')[0])
                 self['landingPageParameter'] = self['landingPagePath'].apply(general_utils.url_extract_parameter)
                 self.rename(columns={'landingPagePath': 'landingPageFull'}, inplace=True)
 
@@ -364,23 +343,22 @@
                 date_time_series = pd.to_datetime(self['dateHour'], format="%Y%m%d%H")
                 self['recordDate'] = date_time_series.apply(lambda date_time: datetime.datetime.date(date_time))
                 self['recordTime'] = date_time_series.apply(lambda date_time: date_time.time())
                 self.drop(columns='dateHour', inplace=True)
                 self.remove_join_dimensions('dateHour')
                 self.add_join_dimensions(['recordDate', 'recordTime'])
 
-            if 'countryIsoCode' in self.columns:
-                self.countryIsoCode = self.countryIsoCode.apply(iso_code_2_to_3)
-
             if 'countryId' in self.columns:
-                self['countryIsoCode'] = self['countryId'].apply(iso_code_2_to_3)
-                self.drop(columns='countryId', inplace=True)
+                self.rename(columns={'countryId': 'countryIsoCode'}, inplace=True)
                 self.remove_join_dimensions('countryId')
                 self.add_join_dimensions(['countryIsoCode'])
 
+            if 'countryIsoCode' in self.columns:
+                self.countryIsoCode = self.countryIsoCode.apply(iso_code_2_to_3)
+
             self.snake_case_join_dimensions()
 
         self.snake_case_columns()
 
         if "record_date" not in self.columns:
             if start_date and end_date:
                 self.insert(loc=0, column="record_date", value=end_date)
@@ -567,37 +545,46 @@
         values = {_col: 0 for _col, _type in self.dtypes.items() if _type == 'float' or _type == 'int'}
         self.fillna(value=values, inplace=True)
 
     def join_on_dimensions(self, dataframe, how: str = "outer"):
         if not set(self.join_dimensions) == set(dataframe.join_dimensions):
             raise ValueError("Input dataframe must have same join_dimensions")
 
+        if self.error:
+            _e = self.error
+        else:
+            _e = dataframe.error
+
         _out = GADataFrame(
             df_input=pd.merge(self, dataframe, how=how, on=self.join_dimensions),
             response_type=self.response_type,
             dimensions=list(set(self.dimensions + dataframe.dimensions)),
             metrics=list(set(self.metrics + dataframe.metrics)),
             from_ga_response=False,
             join_dimensions=self.join_dimensions,
             start_date=min(self.date_range.get('start'), dataframe.date_range.get('start')),
-            end_date=max(self.date_range.get('end'), dataframe.date_range.get('end'))
+            end_date=max(self.date_range.get('end'), dataframe.date_range.get('end')),
+            error=_e
         )
 
         return _out
 
+    def add_row_id(self):
+        self.reset_index(drop=True, inplace=True)
+        self.reset_index(drop=False, inplace=True)
+        self.rename(columns={'index': 'row_id'}, inplace=True)
+
 
 class GSCDataFrame(pd.DataFrame):
     """
     Subclass of pandas.DataFrame specifically for use with Google Search Console responses.
     The subclass must be initialized with a GSC response object and will create a dataframe
     from the report.
 
-    The DataFrame column headings are the same as the GA dimensions and metrics but without the 'ga:' prefix
-
-    In addition to pandas DataFrame functionality, the GADataFrame has additional metadata attributes:
+    In addition to pandas DataFrame functionality, the GSCDataFrame has additional metadata attributes:
         dimensions: list of the GSC dimensions
     """
 
     _metadata = ["dimensions",
                  "metrics",
                  "response_aggregation",
                  "date_range"]
@@ -619,15 +606,15 @@
         if gsc_dimensions is None:
             gsc_dimensions = ['country', 'device', 'page', 'query']
 
         self.dimensions = gsc_dimensions
 
         if df_input is None:
             self.metrics = ['clicks', 'impressions', 'ctr', 'position']
-            super().__init__(None, columns=[strip_ga_prefix(_) for _ in self.dimensions + self.metrics])
+            super().__init__(None, columns=self.dimensions + self.metrics)
             if 'date' in self.columns:
                 self.rename(columns={'date': 'record_date'}, inplace=True)
             if 'page' in self.columns:
                 self.rename(columns={'page': 'landing_page'}, inplace=True)
         else:
             super().__init__(df_input)
 
@@ -840,23 +827,14 @@
     subcat_dict = categories_dict.get('subcategories')
     for sub_cat in subcat_dict.keys():
         if re.match(subcat_dict.get(sub_cat), product_name.lower()):
             return sub_cat
     return 'other'
 
 
-def strip_ga_prefix(s: str) -> str:
-    if len(s) < 3:
-        return s
-    elif s[:3] == 'ga:':
-        return s[3:]
-    else:
-        return s
-
-
 def get_response_type(response: dict | RunReportResponse):
     if isinstance(response, RunReportResponse):
         return 'GA4'
 
     if _t := response.get('response_type'):
         return _t
```

### Comparing `pygoogalytics-0.4.2/pygoogalytics/kwp_wrappers.py` & `pygoogalytics-0.5.0/pygoogalytics/kwp_wrappers.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.2/pygoogalytics/utils/ads_reports_parsing.py` & `pygoogalytics-0.5.0/pygoogalytics/utils/ads_reports_parsing.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.2/pygoogalytics/utils/general_utils.py` & `pygoogalytics-0.5.0/pygoogalytics/utils/general_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -73,8 +73,30 @@
 
 def dict_merge(dict1, dict2):
     d = dict()
     for k, v in dict1.items():
         d[k] = v
     for k, v in dict2.items():
         d[k] = v
-    return d
+    return d
+
+
+def expand_list(list_of_lists: list[list]) -> list:
+    while any(isinstance(_l, list) for _l in list_of_lists):
+        _new_list = []
+        for _item in list_of_lists:
+            if isinstance(_item, list):
+                _new_list.extend(_item)
+            else:
+                _new_list.append(_item)
+        list_of_lists = _new_list
+    return list_of_lists
+
+def parse_date(d):
+    if m:=re.match(r"\d{8}", d):
+        return datetime.datetime.strptime(m.group(0), "%Y%m%d").date()
+    elif m:=re.match(r"\d{4}-\d{2}-\d{2}", d):
+        return datetime.datetime.strptime(m.group(0), "%Y-%m-%d").date()
+    elif m:=re.match(r"\d{4} \d{2} \d{2}", d):
+        return datetime.datetime.strptime(m.group(0), "%Y %m %d").date()
+    else:
+        raise ValueError(f"Cannot parse date string '{d}'")
```

### Comparing `pygoogalytics-0.4.2/pygoogalytics/utils/resource_utils.py` & `pygoogalytics-0.5.0/pygoogalytics/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.2/pygoogalytics.egg-info/PKG-INFO` & `pygoogalytics-0.5.0/pygoogalytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.4.2
+Version: 0.5.0
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.4.2/pygoogalytics.egg-info/SOURCES.txt` & `pygoogalytics-0.5.0/pygoogalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.4.2/setup.py` & `pygoogalytics-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # twine upload dist/*
 
 _desc = """PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 in the form of a pandas dataframe."""
 
 setup(
     name='pygoogalytics',
-    version='0.4.2',
+    version='0.5.0',
     description=_desc,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Blink-SEO/pygoogalytics',
     author='Joshua Prettyman',
     author_email='joshua@blinkseo.co.uk',
     license='MIT',
```

