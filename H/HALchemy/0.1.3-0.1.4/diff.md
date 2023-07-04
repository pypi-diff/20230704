# Comparing `tmp/HALchemy-0.1.3-py3-none-any.whl.zip` & `tmp/HALchemy-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5070 bytes, number of entries: 7
+Zip file size: 5704 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Jul-04 01:21 halchemy/__init__.py
--rw-rw-rw-  2.0 fat     6851 b- defN 23-Jul-04 01:21 halchemy/api.py
+-rw-rw-rw-  2.0 fat     6873 b- defN 23-Jul-04 02:22 halchemy/api.py
 -rw-rw-rw-  2.0 fat     2548 b- defN 23-Jul-01 18:46 halchemy/requests_helper.py
--rw-rw-rw-  2.0 fat      669 b- defN 23-Jul-04 01:23 HALchemy-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 01:23 HALchemy-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-04 01:23 HALchemy-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      531 b- defN 23-Jul-04 01:23 HALchemy-0.1.3.dist-info/RECORD
-7 files, 10773 bytes uncompressed, 4128 bytes compressed:  61.7%
+-rw-rw-rw-  2.0 fat     2192 b- defN 23-Jul-04 02:57 HALchemy-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 02:57 HALchemy-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-04 02:57 HALchemy-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      532 b- defN 23-Jul-04 02:57 HALchemy-0.1.4.dist-info/RECORD
+7 files, 12319 bytes uncompressed, 4762 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: halchemy/api.py
 Comment: 
 
 Filename: halchemy/requests_helper.py
 Comment: 
 
-Filename: HALchemy-0.1.3.dist-info/METADATA
+Filename: HALchemy-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: HALchemy-0.1.3.dist-info/WHEEL
+Filename: HALchemy-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: HALchemy-0.1.3.dist-info/top_level.txt
+Filename: HALchemy-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: HALchemy-0.1.3.dist-info/RECORD
+Filename: HALchemy-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## halchemy/api.py

```diff
@@ -6,15 +6,15 @@
     the value of the Authorization: header
 
 Examples:
     api = Api('http://localhost:2112')
     people = api.get('/people')  # responds with collection whose members are in _items
     for person in people['_items']:
         print(f"{person['firstName']} {person['lastName']}")
-        cars = api.get_rel(person, 'cars')
+        cars = api.get_from_rel(person, 'cars')
         print(f" - has {len(cars['_items'])} cars")
 
 License:
     MIT License
 
     Copyright (c) 2023 Michael Ottoson
 
@@ -77,22 +77,22 @@
             return response.json()
         except:
             if response.status_code == 422:
                 issue = response.json().get('_issues', {}).get('name', '')
                 if 'is not unique' in issue:
                     new_data = json.loads(data)
                     new_data['name'] += ' ~'
-                    return self.post(url, new_data)
+                    return self._api.post(url, data=new_data)
             message = f'{response.status_code} {response.reason}'
             details = response.text
             raise RuntimeError(f'POST {url} - {message}\n{details}\n\n{data}')
 
     def post_to_rel(self, resource, rel, data, parameters={}, template={}):
         url = self.url_from_rel(resource, rel, parameters, template)
-        return self.post(url, data)
+        return self.post_to_url(url, data)
 
     def patch_resource(self, resource, data):
         if type(data) is not str:
             data = json.dumps(data)
         url = self.url_from_rel(resource, 'self')
         headers = {
             'If-Match': resource['_etag']
```

## Comparing `HALchemy-0.1.3.dist-info/RECORD` & `HALchemy-0.1.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 halchemy/__init__.py,sha256=uOY88fxo04Ofw2_FpvGJ6LziQpDTE2o6aWfNP5May5M,73
-halchemy/api.py,sha256=MtmtTdMHHxDNunTND_hh22W0I6jqIiRtHaDJ7gsZQhk,6851
+halchemy/api.py,sha256=R_Cweh-s_1-3jGtn_J7zsDW2z9fUwvM1WB9okUcJRsY,6873
 halchemy/requests_helper.py,sha256=7mV5ts4jN3viuvpTWoYogkap8v1HpYe0wIWxf9N0KMI,2548
-HALchemy-0.1.3.dist-info/METADATA,sha256=sdxUQdyPTk9sjQH8B2djniPfA672CfFXKMqqYuaJ058,669
-HALchemy-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-HALchemy-0.1.3.dist-info/top_level.txt,sha256=QDAX4T2q2TC09LWO_LgEyuEBr-lPTU86p48miwnpfzw,9
-HALchemy-0.1.3.dist-info/RECORD,,
+HALchemy-0.1.4.dist-info/METADATA,sha256=Tk97se30WMZ1K4wMIV68FBQrF-m-G6a14PAWOeKJROc,2192
+HALchemy-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+HALchemy-0.1.4.dist-info/top_level.txt,sha256=QDAX4T2q2TC09LWO_LgEyuEBr-lPTU86p48miwnpfzw,9
+HALchemy-0.1.4.dist-info/RECORD,,
```

