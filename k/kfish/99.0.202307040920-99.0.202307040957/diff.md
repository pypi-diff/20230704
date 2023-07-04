# Comparing `tmp/kfish-99.0.202307040920-py3-none-any.whl.zip` & `tmp/kfish-99.0.202307040957-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7530 bytes, number of entries: 6
--rw-r--r--  2.0 unx     9748 b- defN 23-Jul-04 09:13 kfish/__init__.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Jul-04 09:20 kfish-99.0.202307040920.dist-info/LICENSE
--rw-r--r--  2.0 unx      302 b- defN 23-Jul-04 09:20 kfish-99.0.202307040920.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 09:20 kfish-99.0.202307040920.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-04 09:20 kfish-99.0.202307040920.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      509 b- defN 23-Jul-04 09:20 kfish-99.0.202307040920.dist-info/RECORD
-6 files, 22015 bytes uncompressed, 6600 bytes compressed:  70.0%
+Zip file size: 7507 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     9105 b- defN 23-Jul-04 09:51 kfish/__init__.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Jul-04 09:57 kfish-99.0.202307040957.dist-info/LICENSE
+-rw-r--r--  2.0 unx      302 b- defN 23-Jul-04 09:57 kfish-99.0.202307040957.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 09:57 kfish-99.0.202307040957.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-04 09:57 kfish-99.0.202307040957.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      509 b- defN 23-Jul-04 09:57 kfish-99.0.202307040957.dist-info/RECORD
+6 files, 21372 bytes uncompressed, 6577 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: kfish/__init__.py
 Comment: 
 
-Filename: kfish-99.0.202307040920.dist-info/LICENSE
+Filename: kfish-99.0.202307040957.dist-info/LICENSE
 Comment: 
 
-Filename: kfish-99.0.202307040920.dist-info/METADATA
+Filename: kfish-99.0.202307040957.dist-info/METADATA
 Comment: 
 
-Filename: kfish-99.0.202307040920.dist-info/WHEEL
+Filename: kfish-99.0.202307040957.dist-info/WHEEL
 Comment: 
 
-Filename: kfish-99.0.202307040920.dist-info/top_level.txt
+Filename: kfish-99.0.202307040957.dist-info/top_level.txt
 Comment: 
 
-Filename: kfish-99.0.202307040920.dist-info/RECORD
+Filename: kfish-99.0.202307040957.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kfish/__init__.py

```diff
@@ -1,233 +1,221 @@
 from urllib.parse import urlparse
 from urllib.request import urlopen, Request
 import base64
 import json
+import os
 import ssl
+import re
 import sys
 from uuid import UUID
 
 
 def valid_uuid(uuid):
     try:
         UUID(uuid)
         return True
     except:
         return False
 
 
-def virtual(url):
-    p = urlparse(url)
-    if not p.path.startswith('/redfish/v1/Systems'):
-        return False
-    path = p.path.replace('/redfish/v1/Systems/', '')
-    return valid_uuid(path) or len(path.split('/')) == 2
+def get_info(url, user, password):
+    match = re.match('.*/redfish/v1/Systems/(.*)', url)
+    if '/redfish/v1/Systems' in url and\
+       (valid_uuid(os.path.basename(url)) or (match is not None and len(match.group(1).split('/')) == 2)):
+        model = 'virtual'
+        if user is None:
+            user = 'fake'
+        if password is None:
+            password = 'fake'
+        return model, url, user, password
+    oem_url = f"https://{url}" if '://' not in url else url
+    p = urlparse(oem_url)
+    headers = {'Accept': 'application/json'}
+    request = Request(f"https://{p.netloc}/redfish/v1", headers=headers)
+    oem = json.loads(urlopen(request).read())['Oem']
+    model = "dell" if 'Dell' in oem else "hp" if 'Hpe' in oem else 'supermicro' if 'Supermicro' in oem else 'N/A'
+    if '://' not in url:
+        if model in ['hp', 'supermicro']:
+            url = f"https://{url}/redfish/v1/Systems/1"
+        elif model == 'dell':
+            url = f"https://{url}/redfish/v1/Systems/System.Embedded.1"
+            if user is None:
+                user = 'root'
+            if password is None:
+                password = 'calvin'
+        else:
+            print(f"Invalid url {url}")
+            sys.exit(0)
+    return model, url, user, password
 
 
 class Redfish(object):
     def __init__(self, url, user='root', password='calvin', insecure=True, debug=False, model=None):
         self.debug = debug
         self.headers = {'Content-Type': 'application/json', 'Accept': 'application/json'}
-        self.context = ssl.create_default_context()
         if insecure:
-            self.context.check_hostname = False
-            self.context.verify_mode = ssl.CERT_NONE
+            ssl._create_default_https_context = ssl._create_unverified_context
         url = url.replace('idrac-virtualmedia', 'https').replace('ilo5-virtualmedia', 'https')
-        if virtual(url):
-            self.model = 'fake'
-            if user is None or password is None:
-                user, password = 'fake', 'fake'
-        else:
-            self.model = model or self.get_model(url)
-        if '://' not in url:
-            if self.model in ['hp', 'hpe', 'supermicro']:
-                url = f"https://{url}/redfish/v1/Systems/1"
-            elif self.model == 'dell':
-                url = f"https://{url}/redfish/v1/Systems/System.Embedded.1"
-                if user is None or password is None:
-                    user, password = 'root', 'calvin'
-            else:
-                print(f"Invalid url {url}")
-                sys.exit(0)
-        self.url = url
+        self.model, self.url, self.user, self.password = get_info(url, user, password)
         if self.debug:
             print(f"Using base url {self.url}")
         p = urlparse(url)
         self.baseurl = f"{p.scheme}://{p.netloc}"
-        self.user = user
-        self.password = password
-        credentials = base64.b64encode(bytes(f'{user}:{password}', 'ascii')).decode('utf-8')
+        credentials = base64.b64encode(bytes(f'{self.user}:{self.password}', 'ascii')).decode('utf-8')
         self.headers["Authorization"] = f"Basic {credentials}"
         self.manager_url = None
 
-    def get_model(self, url):
-        if '://' not in url:
-            url = f"https://{url}"
-        p = urlparse(url)
-        headers = {'Accept': 'application/json'}
-        request = Request(f"https://{p.netloc}/redfish/v1", headers=headers)
-        oem = json.loads(urlopen(request, context=self.context).read())['Oem']
-        if 'Dell' in oem:
-            model = "dell"
-        elif 'Hpe' in oem:
-            model = "hpe"
-        elif 'Supermicro' in oem:
-            model = "supermicro"
-        else:
-            model = 'N/A'
-        return model
-
     def get_manager_url(self):
         request = Request(self.url, headers=self.headers)
-        response = json.loads(urlopen(request, context=self.context).read())
+        response = json.loads(urlopen(request).read())
         return f"{self.baseurl}{response['Links']['ManagedBy'][0]['@odata.id']}"
 
     def get_iso_url(self):
         manager_url = self.get_manager_url()
         request = Request(f'{manager_url}', headers=self.headers)
-        results = json.loads(urlopen(request, context=self.context).read())
+        results = json.loads(urlopen(request).read())
         if 'VirtualMedia' in results:
             virtual_media_url = results['VirtualMedia']['@odata.id']
         else:
             virtual_media_url = results['Status']['VirtualMedia']['@odata.id']
         request = Request(f'{self.baseurl}{virtual_media_url}', headers=self.headers)
-        results = json.loads(urlopen(request, context=self.context).read())
+        results = json.loads(urlopen(request).read())
         if 'Oem' in results:
             odata = results['Oem']['Supermicro']['VirtualMediaConfig']['@odata.id']
         else:
             for member in results['Members']:
                 odata = member['@odata.id']
                 if odata.endswith('CD') or odata.endswith('Cd') or odata.endswith('2'):
                     break
         return f'{self.baseurl}{odata}'
 
     def get_iso_status(self):
         iso_url = self.get_iso_url()
         if self.debug:
             print(f"Getting {iso_url}")
         request = Request(iso_url, headers=self.headers)
-        response = json.loads(urlopen(request, context=self.context).read())
+        response = json.loads(urlopen(request).read())
         return f"{response['Image']}"
 
     def get_iso_eject_url(self):
         iso_url = self.get_iso_url()
         request = Request(iso_url, headers=self.headers)
-        actions = json.loads(urlopen(request, context=self.context).read())['Actions']
+        actions = json.loads(urlopen(request).read())['Actions']
         target = '#IsoConfig.UnMount' if self.model == 'supermicro' else '#VirtualMedia.EjectMedia'
         t = actions[target]['target']
         return f"{self.baseurl}{t}"
 
     def get_iso_insert_url(self):
         iso_url = self.get_iso_url()
         request = Request(iso_url, headers=self.headers)
-        actions = json.loads(urlopen(request, context=self.context).read())['Actions']
+        actions = json.loads(urlopen(request).read())['Actions']
         target = '#IsoConfig.Mount' if self.model == 'supermicro' else '#VirtualMedia.InsertMedia'
         t = actions[target]['target']
         return f"{self.baseurl}{t}"
 
     def eject_iso(self):
         headers = self.headers.copy()
         data = json.dumps({}).encode('utf-8')
         if self.model == 'supermicro':
             headers['Content-Length'] = 0
             # data = {}
         eject_url = self.get_iso_eject_url()
         if self.debug:
             print(f"Sending POST to {eject_url} with empty data")
         request = Request(eject_url, headers=headers, method='POST', data=data)
-        urlopen(request, context=self.context)
+        urlopen(request)
 
     def insert_iso(self, iso_url):
         headers = self.headers.copy()
         if self.model == 'supermicro':
             p = urlparse(iso_url)
             data = {"Host": f"{p.scheme}://{p.netloc}", "Path": p.path}
             manager_url = self.get_manager_url()
             cd_url = f"{manager_url}/VM1/CfgCD"
             if self.debug:
                 print(f"Sending PATCH to {cd_url} with data {data}")
             data = json.dumps(data).encode('utf-8')
             request = Request(cd_url, data=data, headers=self.headers, method='PATCH')
-            urlopen(request, context=self.context)
+            urlopen(request)
             headers['Content-Length'] = 0
         data = {"Image": iso_url, "Inserted": True}
         insert_url = self.get_iso_insert_url()
         if self.debug:
             print(f"Sending POST to {insert_url} with data {data}")
         data = json.dumps(data).encode('utf-8')
         request = Request(insert_url, data=data, headers=headers)
-        urlopen(request, context=self.context)
+        urlopen(request)
 
     def set_iso_once(self):
         request = Request(self.url, headers=self.headers)
-        response = json.loads(urlopen(request, context=self.context).read())
+        response = json.loads(urlopen(request).read())
         currentboot = response['Boot']
         newboot = {}
         if currentboot['BootSourceOverrideEnabled'] != 'Once':
             newboot['BootSourceOverrideEnabled'] = 'Once'
         if currentboot['BootSourceOverrideTarget'] != 'Cd':
             newboot['BootSourceOverrideTarget'] = 'Cd'
         if 'BootSourceOverrideMode' not in currentboot or currentboot['BootSourceOverrideMode'] != 'UEFI':
             newboot['BootSourceOverrideMode'] = 'UEFI'
         data = {"Boot": newboot}
         if self.debug:
             print(f"Sending PATCH to {self.url} with data {data}")
         data = json.dumps(data).encode('utf-8')
         request = Request(self.url, data=data, headers=self.headers, method='PATCH')
-        urlopen(request, context=self.context)
+        urlopen(request)
 
     def restart(self):
         request = Request(self.url, headers=self.headers)
-        response = json.loads(urlopen(request, context=self.context).read())
+        response = json.loads(urlopen(request).read())
         reset_type = 'On' if response['PowerState'] == 'Off' else 'ForceRestart'
         data = {"ResetType": reset_type}
         reset_url = f"{self.url}/Actions/ComputerSystem.Reset"
         if self.debug:
             print(f"Sending POST to {reset_url} with data {data}")
         data = json.dumps(data).encode('utf-8')
         request = Request(reset_url, data=data, headers=self.headers)
-        urlopen(request, context=self.context)
+        urlopen(request)
 
     def stop(self):
         data = {"ResetType": "ForceOff"}
         reset_url = f"{self.url}/Actions/ComputerSystem.Reset"
         if self.debug:
             print(f"Sending POST to {reset_url} with data {data}")
         data = json.dumps(data).encode('utf-8')
         request = Request(reset_url, data=data, headers=self.headers)
-        urlopen(request, context=self.context)
+        urlopen(request)
 
     def start(self):
         data = {"ResetType": "On"}
         reset_url = f"{self.url}/Actions/ComputerSystem.Reset"
         if self.debug:
             print(f"Sending POST to {reset_url} with {data}")
         data = json.dumps(data).encode('utf-8')
         request = Request(reset_url, data=data, headers=self.headers)
-        urlopen(request, context=self.context)
+        urlopen(request)
 
     def status(self):
         request = Request(self.url, headers=self.headers)
-        response = json.loads(urlopen(request, context=self.context).read())
+        response = json.loads(urlopen(request).read())
         return response['PowerState']
 
     def info(self):
         request = Request(self.url, headers=self.headers)
-        response = json.loads(urlopen(request, context=self.context).read())
+        response = json.loads(urlopen(request).read())
         return response
 
     def reset(self):
         manager_url = self.get_manager_url()
         reset_url = f"{manager_url}/Actions/Manager.Reset"
         data = {"ResetType": "GracefulRestart"}
         if self.debug:
             print(f"Sending POST to {reset_url} with data {data}")
         data = json.dumps(data).encode('utf-8')
         request = Request(reset_url, headers=self.headers, method='POST', data=data)
-        urlopen(request, context=self.context)
+        urlopen(request)
 
     def set_iso(self, iso_url):
         try:
             self.eject_iso()
         except:
             pass
         self.insert_iso(iso_url)
```

## Comparing `kfish-99.0.202307040920.dist-info/LICENSE` & `kfish-99.0.202307040957.dist-info/LICENSE`

 * *Files identical despite different names*

