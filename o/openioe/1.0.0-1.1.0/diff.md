# Comparing `tmp/openioe-1.0.0.tar.gz` & `tmp/openioe-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openioe-1.0.0.tar", last modified: Mon Jul  3 10:51:17 2023, max compression
+gzip compressed data, was "openioe-1.1.0.tar", last modified: Tue Jul  4 10:00:53 2023, max compression
```

## Comparing `openioe-1.0.0.tar` & `openioe-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 10:51:17.344422 openioe-1.0.0/
--rw-rw-rw-   0        0        0     1091 2020-04-05 22:23:47.000000 openioe-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     9082 2023-07-03 10:51:17.344422 openioe-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8664 2023-07-03 10:43:13.000000 openioe-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 10:51:17.324428 openioe-1.0.0/openioe/
--rw-rw-rw-   0        0        0      100 2022-09-04 08:32:51.000000 openioe-1.0.0/openioe/__init__.py
--rw-rw-rw-   0        0        0     4747 2023-07-03 09:27:22.000000 openioe-1.0.0/openioe/openioe_apis.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:51:17.344422 openioe-1.0.0/openioe.egg-info/
--rw-rw-rw-   0        0        0     9082 2023-07-03 10:51:17.000000 openioe-1.0.0/openioe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-07-03 10:51:17.000000 openioe-1.0.0/openioe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 10:51:17.000000 openioe-1.0.0/openioe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 10:51:17.000000 openioe-1.0.0/openioe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 10:51:17.344422 openioe-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-07-03 10:51:01.000000 openioe-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:00:53.551106 openioe-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2020-04-05 22:23:47.000000 openioe-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     8582 2023-07-04 10:00:53.551106 openioe-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8164 2023-07-04 09:54:10.000000 openioe-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 10:00:53.531104 openioe-1.1.0/openioe/
+-rw-rw-rw-   0        0        0      100 2022-09-04 08:32:51.000000 openioe-1.1.0/openioe/__init__.py
+-rw-rw-rw-   0        0        0     6025 2023-07-04 08:05:38.000000 openioe-1.1.0/openioe/openioe_apis.py
+drwxrwxrwx   0        0        0        0 2023-07-04 10:00:53.551106 openioe-1.1.0/openioe.egg-info/
+-rw-rw-rw-   0        0        0     8582 2023-07-04 10:00:53.000000 openioe-1.1.0/openioe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-07-04 10:00:53.000000 openioe-1.1.0/openioe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 10:00:53.000000 openioe-1.1.0/openioe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-04 10:00:53.000000 openioe-1.1.0/openioe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 10:00:53.551106 openioe-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-07-04 10:00:35.000000 openioe-1.1.0/setup.py
```

### Comparing `openioe-1.0.0/LICENSE` & `openioe-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openioe-1.0.0/PKG-INFO` & `openioe-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,140 +1,162 @@
 Metadata-Version: 2.1
 Name: openioe
-Version: 1.0.0
+Version: 1.1.0
 Summary: Open IoE
 Home-page: https://openioe.gnanodaya.org/
 Author: Venkataswamy R
 Author-email: opensourceioe@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
+ 
 ## Open IoE
 
-
 Open IoE is a simple IoT platform to operate IoT devices.
 
 There are two options available,
 
-1. Python Library (Client) 
+1. Python Library (Client)
+
 2. Web services (REST APIs)
+
 ---
 
 ### 1\. Python Library
 
 Users are expected to take these steps,
-1. Install Python Library
 
-    `pip install openioe`
+1. Install Python Library
+	`pip install openioe`
 
 2. Write the client code using the following methods
 
+ 
 #### Method List:
-<table><tbody><tr><td><strong>No</strong></td><td><strong>Method</strong></td><td><strong>Description</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>ReadValue</td><td>To read the sensor data from single nodes. Type of data is "Numeric/String"</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+
+<table><tbody><tr><td><strong>No</strong></td><td><strong>Method</strong></td><td><strong>Description</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>ReadValue</td><td>To read the sensor data from single nodes. Type of data is "Numeric/String"</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.DeviceID=xx
 oi.DevicePin=xxx
 SensorData,ResposeCode=oi.ReadValue()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
-<tr><td>2</td><td>WriteValue</td><td>To modify the control signal at single nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+<tr><td>2</td><td>WriteValue</td><td>To modify the control signal at single nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.DeviceID=xx
 oi.DevicePin=xx
 oi.Data=10
 SensorData,ResposeCode=oi.WriteValue()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
-<tr><td>3</td><td>ReadJSON</td><td>To read the sensor data from single nodes. Type of data is "JSON".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+<tr><td>3</td><td>ReadJSON</td><td>To read the sensor data from single nodes. Type of data is "JSON".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.DeviceID=xx
 oi.DevicePin=xxx
 SensorData,ResposeCode=oi.ReadJSON()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
-<tr><td>4</td><td>WriteJSON</td><td>To modify the control signal at single nodes. Type of data is "JSON".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+<tr><td>4</td><td>WriteJSON</td><td>To modify the control signal at single nodes. Type of data is "JSON".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.DeviceID=xx
 oi.DevicePin=xxx
 oi.DataJSON={'Value': '10'}
 SensorData,ResposeCode=oi.WriteJSON()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
-<tr><td>5</td><td>ReadXML</td><td>To read the sensor data from single nodes. Type of data is "XML".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+<tr><td>5</td><td>ReadXML</td><td>To read the sensor data from single nodes. Type of data is "XML".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.DeviceID=xx
 oi.DevicePin=xxx
 SensorData,ResposeCode=oi.ReadXML()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
-<tr><td>6</td><td>WriteXML</td><td>To modify the control signal at single nodes. Type of data is "XML".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+<tr><td>6</td><td>WriteXML</td><td>To modify the control signal at single nodes. Type of data is "XML".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.DeviceID=xx
 oi.DevicePin=xxx
 oi.DataXML='<Name>OpenIoE</Name>'
 SensorData,ResposeCode=oi.WriteXML()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
-<tr><td>7</td><td>Read</td><td>To read the sensor data from multiple nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+<tr><td>7</td><td>Read</td><td>To read the sensor data from multiple nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.UserIDPinAPIKeys=[[xx, xxx], [x, xxx]]
 SensorData,ResposeCode=oi.Read()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
 <tr><td>8</td><td>Write</td><td>To modify the control signal at multiple nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.UserIDPinAPIKeys=[[xx, xxx], [xx, xxx]]
 oi.Data=[xx,xx]
 Confirmation,ResposeCode=oi.ReadAPI()
 print(Confirmation)
-print(ResposeCode)</code></pre></td></tr><tr><td>3</td><td>Developer</td><td>To display the developer information</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>9</td><td>Generate API Key</td><td>To generate new API key for a given email and password.</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
+oi.UserEmail='xxxxxxxxxx'
+oi.UserPassword='xxxxxxxxxxx'
+ResponseJson,ResponseCode=oi.GenerateAPIKey()
+print(ResponseJson['User ID'])
+print(ResponseJson['API Key'])
+print(ResponseJson['Message'])
+print(ResponseCode)</code></pre></td></tr>
+<tr><td>10</td><td>Create New Device</td><td>To add new IoT device for a given API key, name, cryptotype and data format.</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
+oi.APIKey='pnHEmHgjFl0PT247Eae9'
+oi.DeviceName='Test000'
+oi.CryptoName='None'
+oi.DataFormat='Value' # 'XML' or 'JSON'
+ResponseTest,ResponseCode=oi.CreateDevice()
+print(ResponseTest)
+print(ResponseCode)</code></pre></td></tr>
+<tr><td>11</td><td>Developer</td><td>To display the developer information</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.Developer()</code></pre></td></tr></tbody></table>
 
-  
-
----
+---  
 
 ### 2\. Web Services
 
 Users are expected to take these steps,
-
 1. Register and login to OpenIoE- [Register/Login](https://openioe.gnanodaya.org/)
-
 2. Create API Key/ Get API Key from OpenIoE.
-
 3. Embed the API Key, Device ID and Pin into the client code.
 
- 
 #### Visit the OpenIoE 3.0 web portal at [https://openioe.gnanodaya.org](https://openioe.gnanodaya.org)
 
+
 #### Visit the OpenIoE 3.0 Help Portal at [https://openioedoc.gnanodaya.org](https://openioedoc.gnanodaya.org)
-  
 
+ 
 #### API List:
 
-<table><tbody><tr><td><strong>No</strong></td><td><strong>API</strong></td><td><strong>Description</strong></td><td><strong>Type</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>showdevicevalue</td><td>To get hardware value from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicevalue/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>2</td><td>updatedevicevalue</td><td>Update the hardware value passed as a parameter</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevievalue/&lt;apikey&gt;/2/433/2</code></pre></td></tr><tr><td>3</td><td>showdevicejson</td><td>To get hardware JSON from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicejson/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>4</td><td>updatedevicejson</td><td>Update the hardware JSON passed as parameter</td><td>http post</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevicejson/&lt;apikey&gt;/2/433 &lt;Data&gt;</code></pre></td></tr><tr><td>5</td><td>showdevicexml</td><td>To get hardware XML file from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicexml/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>6</td><td>updatedevicexml</td><td>Update the hardware XML passed as parameter</td><td>http post</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevicexml/&lt;apikey&gt;/2/433 &lt;Data&gt;</code></pre></td></tr></tbody></table>
-
-  
+<table><tbody><tr><td><strong>No</strong></td><td><strong>API</strong></td><td><strong>Description</strong></td><td><strong>Type</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>showdevicevalue</td><td>To get hardware value from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicevalue/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>2</td><td>updatedevicevalue</td><td>Update the hardware value passed as a parameter</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevievalue/&lt;apikey&gt;/2/433/2</code></pre></td></tr><tr><td>3</td><td>showdevicejson</td><td>To get hardware JSON from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicejson/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>4</td><td>updatedevicejson</td><td>Update the hardware JSON passed as parameter</td><td>http post</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevicejson/&lt;apikey&gt;/2/433 &lt;Data&gt;</code></pre></td></tr><tr><td>5</td><td>showdevicexml</td><td>To get hardware XML file from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicexml/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>6</td><td>updatedevicexml</td><td>Update the hardware XML passed as parameter</td><td>http post</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevicexml/&lt;apikey&gt;/2/433 &lt;Data&gt;</code></pre></td></tr>
+<tr><td>7</td><td>generateapikey</td><td>Generate new API Key by providing user creds</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/generateapikey/&lt;emailid&gt;/&lt;password&gt;</code></pre></td></tr>
+<tr><td>8</td><td>createuserdevice</td><td>Add new IoT device to your account</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/createuserdevice/&lt;APIKey&gt;/&lt;DeviceName&gt;/&lt;CryptoName&gt;/&lt;DataFormat&gt;</code></pre></td></tr>
+</tbody></table>
 
 ---
 
- 
-### Developers
-
+### Developers 
 <p>
 <img  src="https://venkataswamy.in/images/img1.jpg"  alt="Dr. Venkataswamy R"  width="100"/>
 </p>
-<div><div  dir="ltr"><div  style="font-size:small"><i><font  face="times new roman, serif">Thanks and Regards</font><font  face="arial">,</font></i></div><div  style="font-family:arial"><b><font  size="2"  color="#0000ff"><span></span>Venkataswamy R</font><font  size="2"><span></span></font></b></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>Assistant Professor,</b></font></span></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>Department of Electrical and Electronics Engineering,</b></font></span></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>School of Engineering and Technology,<br></b></font></span></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>Christ (Deemed to be University),</b></font></span></div><div  style="font-size:small"><span  style="color:rgb(56,118,29)"><font  face="trebuchet ms, sans-serif"><b><span  style="color:rgb(0,0,0)">Bengaluru-560074, India</span><br><br></b></font></span></div><div  style="font-family:arial;font-size:small"><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i><img  src="https://ci4.googleusercontent.com/proxy/JGrPNyQPabY_rra4ygFQhpV3cMA7ITqb5WxBKVcm5J7nUXsWZgk4oUuqR-1Dso97mGx5TF4OvAWyEvAm6fA0h9EhgVZcO6VnO77JetkXhoxX6-7YrakgsA=s0-d-e1-ft#https://openclipart.org/image/2400px/svg_to_png/262221/phone25.png"  alt="Image result for phone icon"  style="margin-top:0px"  width="17"  height="14"> 080-4012-9961 (O)</i></b><font  face="trebuchet ms, sans-serif"  color="#073763"><b><i>&nbsp;&nbsp;  </i></b></font><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i><img  src="https://ci4.googleusercontent.com/proxy/xDyzoCUBYbAyKgjwt27Jl4lkN_6MrkWuk-4BQ2IgMCZEuCMwJLtZjRYqLSrgS6SGWQcpQOVuNmBzqrKJpes9riut82x8hJ1GJVKL=s0-d-e1-ft#http://simpleicon.com/wp-content/uploads/mobile-1.png"  style="margin-top:0px"  alt="Image result for mobile icon"  width="21"  height="21">+91-7829222446</i></b><i><b>&nbsp;  </b></i><img  src="https://lh4.googleusercontent.com/-FqpLVHU8eMw/AAAAAAAAAAI/AAAAAAAAABM/ivbX55TtoV4/photo.jpg"  alt="Related image"  style="margin-top:0px"  width="21"  height="21"><span><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i>  <a  href="http://venkataswamy.in"  target="_blank">venkatswamy.in</a><br><br><br></i></b></span></div></div></div>
+<div>Thanks and Regards</div>
+<div><strong>Venkataswamy R</strong></div>
+<div>Assistant Professor</div>
+<div>Department of Electrical and Electronics Engineering,</div>
+<div>School of Engineering and Technology</div>
+<div>Christ (Deemed to be University)</div>
+<div>Bengaluru-560074, India</div>
+<br>
+<img  src="https://lh4.googleusercontent.com/-FqpLVHU8eMw/AAAAAAAAAAI/AAAAAAAAABM/ivbX55TtoV4/photo.jpg"  alt="Related image"  style="margin-top:0px"  width="21"  height="21"> <span><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i>  <a  href="http://venkataswamy.in"  target="_blank">venkatswamy.in</a><br><br><br></i></b></span></div></div></div>
```

#### html2text {}

```diff
@@ -1,93 +1,104 @@
-Metadata-Version: 2.1 Name: openioe Version: 1.0.0 Summary: Open IoE Home-page:
+Metadata-Version: 2.1 Name: openioe Version: 1.1.0 Summary: Open IoE Home-page:
 https://openioe.gnanodaya.org/ Author: Venkataswamy R Author-email:
 opensourceioe@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE ## Open IoE Open IoE is a simple IoT platform to
 operate IoT devices. There are two options available, 1. Python Library
 (Client) 2. Web services (REST APIs) --- ### 1\. Python Library Users are
 expected to take these steps, 1. Install Python Library `pip install openioe`
 2. Write the client code using the following methods #### Method List:
-No Method     Description                  Example
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-              To read the sensor data from oi.DeviceID=xx
-1  ReadValue  single nodes. Type of data   oi.DevicePin=xxx
-              is "Numeric/String"          SensorData,ResposeCode=oi.ReadValue
-                                           ()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-              To modify the control signal oi.DeviceID=xx
-2  WriteValue at single nodes. Type of     oi.DevicePin=xx
-              data is "Numeric/String".    oi.Data=10
-                                           SensorData,ResposeCode=oi.WriteValue
-                                           ()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-              To read the sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-3  ReadJSON   single nodes. Type of data   oi.DeviceID=xx
-              is "JSON".                   oi.DevicePin=xxx
-                                           SensorData,ResposeCode=oi.ReadJSON()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-              To modify the control signal oi.DeviceID=xx
-4  WriteJSON  at single nodes. Type of     oi.DevicePin=xxx
-              data is "JSON".              oi.DataJSON={'Value': '10'}
-                                           SensorData,ResposeCode=oi.WriteJSON
-                                           ()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-              To read the sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-5  ReadXML    single nodes. Type of data   oi.DeviceID=xx
-              is "XML".                    oi.DevicePin=xxx
-                                           SensorData,ResposeCode=oi.ReadXML()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-              To modify the control signal oi.DeviceID=xx
-6  WriteXML   at single nodes. Type of     oi.DevicePin=xxx
-              data is "XML".               oi.DataXML='OpenIoE'
-                                           SensorData,ResposeCode=oi.WriteXML()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-              To read the sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-7  Read       multiple nodes. Type of data oi.UserIDPinAPIKeys=[[xx, xxx], [x,
-              is "Numeric/String".         xxx]]
-                                           SensorData,ResposeCode=oi.Read()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from openioe.openioe_apis import *
-                                           oi=openioe_apis()
-                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-              To modify the control signal oi.UserIDPinAPIKeys=[[xx, xxx], [xx,
-8  Write      at multiple nodes. Type of   xxx]]
-              data is "Numeric/String".    oi.Data=[xx,xx]
-                                           Confirmation,ResposeCode=oi.ReadAPI
-                                           ()
-                                           print(Confirmation)
-                                           print(ResposeCode)
-              To display the developer     from openioe.openioe_apis import *
-3  Developer  information                  oi=openioe_apis()
-                                           oi.Developer()
+No Method       Description      Example
+                                 from openioe.openioe_apis import *
+                To read the      oi=openioe_apis()
+                sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+1  ReadValue    single nodes.    oi.DeviceID=xx
+                Type of data is  oi.DevicePin=xxx
+                "Numeric/String" SensorData,ResposeCode=oi.ReadValue()
+                                 print(SensorData)
+                                 print(ResposeCode)
+                                 from openioe.openioe_apis import *
+                To modify the    oi=openioe_apis()
+                control signal   oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+                at single nodes. oi.DeviceID=xx
+2  WriteValue   Type of data is  oi.DevicePin=xx
+                "Numeric/        oi.Data=10
+                String".         SensorData,ResposeCode=oi.WriteValue()
+                                 print(SensorData)
+                                 print(ResposeCode)
+                                 from openioe.openioe_apis import *
+                To read the      oi=openioe_apis()
+                sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+3  ReadJSON     single nodes.    oi.DeviceID=xx
+                Type of data is  oi.DevicePin=xxx
+                "JSON".          SensorData,ResposeCode=oi.ReadJSON()
+                                 print(SensorData)
+                                 print(ResposeCode)
+                                 from openioe.openioe_apis import *
+                                 oi=openioe_apis()
+                To modify the    oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+                control signal   oi.DeviceID=xx
+4  WriteJSON    at single nodes. oi.DevicePin=xxx
+                Type of data is  oi.DataJSON={'Value': '10'}
+                "JSON".          SensorData,ResposeCode=oi.WriteJSON()
+                                 print(SensorData)
+                                 print(ResposeCode)
+                                 from openioe.openioe_apis import *
+                To read the      oi=openioe_apis()
+                sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+5  ReadXML      single nodes.    oi.DeviceID=xx
+                Type of data is  oi.DevicePin=xxx
+                "XML".           SensorData,ResposeCode=oi.ReadXML()
+                                 print(SensorData)
+                                 print(ResposeCode)
+                                 from openioe.openioe_apis import *
+                                 oi=openioe_apis()
+                To modify the    oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+                control signal   oi.DeviceID=xx
+6  WriteXML     at single nodes. oi.DevicePin=xxx
+                Type of data is  oi.DataXML='OpenIoE'
+                "XML".           SensorData,ResposeCode=oi.WriteXML()
+                                 print(SensorData)
+                                 print(ResposeCode)
+                To read the      from openioe.openioe_apis import *
+                sensor data from oi=openioe_apis()
+                multiple nodes.  oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+7  Read         Type of data is  oi.UserIDPinAPIKeys=[[xx, xxx], [x, xxx]]
+                "Numeric/        SensorData,ResposeCode=oi.Read()
+                String".         print(SensorData)
+                                 print(ResposeCode)
+                To modify the    from openioe.openioe_apis import *
+                control signal   oi=openioe_apis()
+                at multiple      oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+8  Write        nodes. Type of   oi.UserIDPinAPIKeys=[[xx, xxx], [xx, xxx]]
+                data is          oi.Data=[xx,xx]
+                "Numeric/        Confirmation,ResposeCode=oi.ReadAPI()
+                String".         print(Confirmation)
+                                 print(ResposeCode)
+                                 from openioe.openioe_apis import *
+                                 oi.UserEmail='xxxxxxxxxx'
+                To generate new  oi.UserPassword='xxxxxxxxxxx'
+   Generate API API key for a    ResponseJson,ResponseCode=oi.GenerateAPIKey
+9  Key          given email and  ()
+                password.        print(ResponseJson['User ID'])
+                                 print(ResponseJson['API Key'])
+                                 print(ResponseJson['Message'])
+                                 print(ResponseCode)
+                                 from openioe.openioe_apis import *
+                To add new IoT   oi.APIKey='pnHEmHgjFl0PT247Eae9'
+                device for a     oi.DeviceName='Test000'
+10 Create New   given API key,   oi.CryptoName='None'
+   Device       name, cryptotype oi.DataFormat='Value' # 'XML' or 'JSON'
+                and data format. ResponseTest,ResponseCode=oi.CreateDevice()
+                                 print(ResponseTest)
+                                 print(ResponseCode)
+                To display the   from openioe.openioe_apis import *
+11 Developer    developer        oi=openioe_apis()
+                information      oi.Developer()
 --- ### 2\. Web Services Users are expected to take these steps, 1. Register
 and login to OpenIoE- [Register/Login](https://openioe.gnanodaya.org/) 2.
 Create API Key/ Get API Key from OpenIoE. 3. Embed the API Key, Device ID and
 Pin into the client code. #### Visit the OpenIoE 3.0 web portal at [https://
 openioe.gnanodaya.org](https://openioe.gnanodaya.org) #### Visit the OpenIoE
 3.0 Help Portal at [https://openioedoc.gnanodaya.org](https://
 openioedoc.gnanodaya.org) #### API List:
@@ -106,21 +117,28 @@
                      parameter                         <apikey>/2/433 <Data>
                      To get hardware XML               <endpoint>/
 5  showdevicexml     file from web service.  http get  showdevicexml/<apikey>/
                                                        2/433
                      Update the hardware XML           <endpoint>/
 6  updatedevicexml   passed as parameter     http post updatedevicexml/
                                                        <apikey>/2/433 <Data>
+                     Generate new API Key by           <endpoint>/
+7  generateapikey    providing user creds    http get  generateapikey/
+                                                       <emailid>/<password>
+                                                       <endpoint>/
+                     Add new IoT device to             createuserdevice/
+8  createuserdevice  your account            http get  <APIKey>/<DeviceName>/
+                                                       <CryptoName>/
+                                                       <DataFormat>
 --- ### Developers
 [Dr. Venkataswamy R]
-Thanks and Regards,
+Thanks and Regards
 Venkataswamy R
-Assistant Professor,
+Assistant Professor
 Department of Electrical and Electronics Engineering,
-School of Engineering and Technology,
-Christ (Deemed to be University),
+School of Engineering and Technology
+Christ (Deemed to be University)
 Bengaluru-560074, India
 
-[Image result for phone icon] 080-4012-9961 (O)  [Image result for mobile
-icon]+91-7829222446 [Related image]venkatswamy.in
+[Related image] venkatswamy.in
```

### Comparing `openioe-1.0.0/README.md` & `openioe-1.1.0/openioe.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,126 +1,162 @@
+Metadata-Version: 2.1
+Name: openioe
+Version: 1.1.0
+Summary: Open IoE
+Home-page: https://openioe.gnanodaya.org/
+Author: Venkataswamy R
+Author-email: opensourceioe@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
+ 
 ## Open IoE
 
-
 Open IoE is a simple IoT platform to operate IoT devices.
 
 There are two options available,
 
-1. Python Library (Client) 
+1. Python Library (Client)
+
 2. Web services (REST APIs)
+
 ---
 
 ### 1\. Python Library
 
 Users are expected to take these steps,
-1. Install Python Library
 
-    `pip install openioe`
+1. Install Python Library
+	`pip install openioe`
 
 2. Write the client code using the following methods
 
+ 
 #### Method List:
-<table><tbody><tr><td><strong>No</strong></td><td><strong>Method</strong></td><td><strong>Description</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>ReadValue</td><td>To read the sensor data from single nodes. Type of data is "Numeric/String"</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+
+<table><tbody><tr><td><strong>No</strong></td><td><strong>Method</strong></td><td><strong>Description</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>ReadValue</td><td>To read the sensor data from single nodes. Type of data is "Numeric/String"</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.DeviceID=xx
 oi.DevicePin=xxx
 SensorData,ResposeCode=oi.ReadValue()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
-<tr><td>2</td><td>WriteValue</td><td>To modify the control signal at single nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+<tr><td>2</td><td>WriteValue</td><td>To modify the control signal at single nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.DeviceID=xx
 oi.DevicePin=xx
 oi.Data=10
 SensorData,ResposeCode=oi.WriteValue()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
-<tr><td>3</td><td>ReadJSON</td><td>To read the sensor data from single nodes. Type of data is "JSON".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+<tr><td>3</td><td>ReadJSON</td><td>To read the sensor data from single nodes. Type of data is "JSON".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.DeviceID=xx
 oi.DevicePin=xxx
 SensorData,ResposeCode=oi.ReadJSON()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
-<tr><td>4</td><td>WriteJSON</td><td>To modify the control signal at single nodes. Type of data is "JSON".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+<tr><td>4</td><td>WriteJSON</td><td>To modify the control signal at single nodes. Type of data is "JSON".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.DeviceID=xx
 oi.DevicePin=xxx
 oi.DataJSON={'Value': '10'}
 SensorData,ResposeCode=oi.WriteJSON()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
-<tr><td>5</td><td>ReadXML</td><td>To read the sensor data from single nodes. Type of data is "XML".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+<tr><td>5</td><td>ReadXML</td><td>To read the sensor data from single nodes. Type of data is "XML".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.DeviceID=xx
 oi.DevicePin=xxx
 SensorData,ResposeCode=oi.ReadXML()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
-<tr><td>6</td><td>WriteXML</td><td>To modify the control signal at single nodes. Type of data is "XML".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+<tr><td>6</td><td>WriteXML</td><td>To modify the control signal at single nodes. Type of data is "XML".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.DeviceID=xx
 oi.DevicePin=xxx
 oi.DataXML='<Name>OpenIoE</Name>'
 SensorData,ResposeCode=oi.WriteXML()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
-<tr><td>7</td><td>Read</td><td>To read the sensor data from multiple nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from  openioe.openioe_apis  import *
+<tr><td>7</td><td>Read</td><td>To read the sensor data from multiple nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.UserIDPinAPIKeys=[[xx, xxx], [x, xxx]]
 SensorData,ResposeCode=oi.Read()
 print(SensorData)
 print(ResposeCode)</code></pre></td></tr>
 <tr><td>8</td><td>Write</td><td>To modify the control signal at multiple nodes. Type of data is "Numeric/String".</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
 oi.UserIDPinAPIKeys=[[xx, xxx], [xx, xxx]]
 oi.Data=[xx,xx]
 Confirmation,ResposeCode=oi.ReadAPI()
 print(Confirmation)
-print(ResposeCode)</code></pre></td></tr><tr><td>3</td><td>Developer</td><td>To display the developer information</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
+print(ResposeCode)</code></pre></td></tr>
+<tr><td>9</td><td>Generate API Key</td><td>To generate new API key for a given email and password.</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
+oi.UserEmail='xxxxxxxxxx'
+oi.UserPassword='xxxxxxxxxxx'
+ResponseJson,ResponseCode=oi.GenerateAPIKey()
+print(ResponseJson['User ID'])
+print(ResponseJson['API Key'])
+print(ResponseJson['Message'])
+print(ResponseCode)</code></pre></td></tr>
+<tr><td>10</td><td>Create New Device</td><td>To add new IoT device for a given API key, name, cryptotype and data format.</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
+oi.APIKey='pnHEmHgjFl0PT247Eae9'
+oi.DeviceName='Test000'
+oi.CryptoName='None'
+oi.DataFormat='Value' # 'XML' or 'JSON'
+ResponseTest,ResponseCode=oi.CreateDevice()
+print(ResponseTest)
+print(ResponseCode)</code></pre></td></tr>
+<tr><td>11</td><td>Developer</td><td>To display the developer information</td><td><pre><code  class="language-python">from openioe.openioe_apis import *
 oi=openioe_apis()
 oi.Developer()</code></pre></td></tr></tbody></table>
 
-  
-
----
+---  
 
 ### 2\. Web Services
 
 Users are expected to take these steps,
-
 1. Register and login to OpenIoE- [Register/Login](https://openioe.gnanodaya.org/)
-
 2. Create API Key/ Get API Key from OpenIoE.
-
 3. Embed the API Key, Device ID and Pin into the client code.
 
- 
 #### Visit the OpenIoE 3.0 web portal at [https://openioe.gnanodaya.org](https://openioe.gnanodaya.org)
 
+
 #### Visit the OpenIoE 3.0 Help Portal at [https://openioedoc.gnanodaya.org](https://openioedoc.gnanodaya.org)
-  
 
+ 
 #### API List:
 
-<table><tbody><tr><td><strong>No</strong></td><td><strong>API</strong></td><td><strong>Description</strong></td><td><strong>Type</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>showdevicevalue</td><td>To get hardware value from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicevalue/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>2</td><td>updatedevicevalue</td><td>Update the hardware value passed as a parameter</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevievalue/&lt;apikey&gt;/2/433/2</code></pre></td></tr><tr><td>3</td><td>showdevicejson</td><td>To get hardware JSON from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicejson/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>4</td><td>updatedevicejson</td><td>Update the hardware JSON passed as parameter</td><td>http post</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevicejson/&lt;apikey&gt;/2/433 &lt;Data&gt;</code></pre></td></tr><tr><td>5</td><td>showdevicexml</td><td>To get hardware XML file from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicexml/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>6</td><td>updatedevicexml</td><td>Update the hardware XML passed as parameter</td><td>http post</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevicexml/&lt;apikey&gt;/2/433 &lt;Data&gt;</code></pre></td></tr></tbody></table>
-
-  
+<table><tbody><tr><td><strong>No</strong></td><td><strong>API</strong></td><td><strong>Description</strong></td><td><strong>Type</strong></td><td><strong>Example</strong></td></tr><tr><td>1</td><td>showdevicevalue</td><td>To get hardware value from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicevalue/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>2</td><td>updatedevicevalue</td><td>Update the hardware value passed as a parameter</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevievalue/&lt;apikey&gt;/2/433/2</code></pre></td></tr><tr><td>3</td><td>showdevicejson</td><td>To get hardware JSON from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicejson/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>4</td><td>updatedevicejson</td><td>Update the hardware JSON passed as parameter</td><td>http post</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevicejson/&lt;apikey&gt;/2/433 &lt;Data&gt;</code></pre></td></tr><tr><td>5</td><td>showdevicexml</td><td>To get hardware XML file from web service.</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/showdevicexml/&lt;apikey&gt;/2/433</code></pre></td></tr><tr><td>6</td><td>updatedevicexml</td><td>Update the hardware XML passed as parameter</td><td>http post</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/updatedevicexml/&lt;apikey&gt;/2/433 &lt;Data&gt;</code></pre></td></tr>
+<tr><td>7</td><td>generateapikey</td><td>Generate new API Key by providing user creds</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/generateapikey/&lt;emailid&gt;/&lt;password&gt;</code></pre></td></tr>
+<tr><td>8</td><td>createuserdevice</td><td>Add new IoT device to your account</td><td>http get</td><td><pre><code  class="language-plaintext">&lt;endpoint&gt;/createuserdevice/&lt;APIKey&gt;/&lt;DeviceName&gt;/&lt;CryptoName&gt;/&lt;DataFormat&gt;</code></pre></td></tr>
+</tbody></table>
 
 ---
 
- 
-### Developers
-
+### Developers 
 <p>
 <img  src="https://venkataswamy.in/images/img1.jpg"  alt="Dr. Venkataswamy R"  width="100"/>
 </p>
-<div><div  dir="ltr"><div  style="font-size:small"><i><font  face="times new roman, serif">Thanks and Regards</font><font  face="arial">,</font></i></div><div  style="font-family:arial"><b><font  size="2"  color="#0000ff"><span></span>Venkataswamy R</font><font  size="2"><span></span></font></b></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>Assistant Professor,</b></font></span></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>Department of Electrical and Electronics Engineering,</b></font></span></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>School of Engineering and Technology,<br></b></font></span></div><div  style="font-size:small"><span  style="color:rgb(0,0,0)"><font  face="trebuchet ms, sans-serif"><b>Christ (Deemed to be University),</b></font></span></div><div  style="font-size:small"><span  style="color:rgb(56,118,29)"><font  face="trebuchet ms, sans-serif"><b><span  style="color:rgb(0,0,0)">Bengaluru-560074, India</span><br><br></b></font></span></div><div  style="font-family:arial;font-size:small"><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i><img  src="https://ci4.googleusercontent.com/proxy/JGrPNyQPabY_rra4ygFQhpV3cMA7ITqb5WxBKVcm5J7nUXsWZgk4oUuqR-1Dso97mGx5TF4OvAWyEvAm6fA0h9EhgVZcO6VnO77JetkXhoxX6-7YrakgsA=s0-d-e1-ft#https://openclipart.org/image/2400px/svg_to_png/262221/phone25.png"  alt="Image result for phone icon"  style="margin-top:0px"  width="17"  height="14"> 080-4012-9961 (O)</i></b><font  face="trebuchet ms, sans-serif"  color="#073763"><b><i>&nbsp;&nbsp;  </i></b></font><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i><img  src="https://ci4.googleusercontent.com/proxy/xDyzoCUBYbAyKgjwt27Jl4lkN_6MrkWuk-4BQ2IgMCZEuCMwJLtZjRYqLSrgS6SGWQcpQOVuNmBzqrKJpes9riut82x8hJ1GJVKL=s0-d-e1-ft#http://simpleicon.com/wp-content/uploads/mobile-1.png"  style="margin-top:0px"  alt="Image result for mobile icon"  width="21"  height="21">+91-7829222446</i></b><i><b>&nbsp;  </b></i><img  src="https://lh4.googleusercontent.com/-FqpLVHU8eMw/AAAAAAAAAAI/AAAAAAAAABM/ivbX55TtoV4/photo.jpg"  alt="Related image"  style="margin-top:0px"  width="21"  height="21"><span><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i>  <a  href="http://venkataswamy.in"  target="_blank">venkatswamy.in</a><br><br><br></i></b></span></div></div></div>
+<div>Thanks and Regards</div>
+<div><strong>Venkataswamy R</strong></div>
+<div>Assistant Professor</div>
+<div>Department of Electrical and Electronics Engineering,</div>
+<div>School of Engineering and Technology</div>
+<div>Christ (Deemed to be University)</div>
+<div>Bengaluru-560074, India</div>
+<br>
+<img  src="https://lh4.googleusercontent.com/-FqpLVHU8eMw/AAAAAAAAAAI/AAAAAAAAABM/ivbX55TtoV4/photo.jpg"  alt="Related image"  style="margin-top:0px"  width="21"  height="21"> <span><b  style="color:rgb(7,55,99);font-family:'trebuchet ms',sans-serif"><i>  <a  href="http://venkataswamy.in"  target="_blank">venkatswamy.in</a><br><br><br></i></b></span></div></div></div>
```

#### html2text {}

```diff
@@ -1,88 +1,104 @@
- ## Open IoE Open IoE is a simple IoT platform to operate IoT devices. There
-are two options available, 1. Python Library (Client) 2. Web services (REST
-APIs) --- ### 1\. Python Library Users are expected to take these steps, 1.
-Install Python Library `pip install openioe` 2. Write the client code using the
-following methods #### Method List:
-No Method     Description                  Example
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-              To read the sensor data from oi.DeviceID=xx
-1  ReadValue  single nodes. Type of data   oi.DevicePin=xxx
-              is "Numeric/String"          SensorData,ResposeCode=oi.ReadValue
-                                           ()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-              To modify the control signal oi.DeviceID=xx
-2  WriteValue at single nodes. Type of     oi.DevicePin=xx
-              data is "Numeric/String".    oi.Data=10
-                                           SensorData,ResposeCode=oi.WriteValue
-                                           ()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-              To read the sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-3  ReadJSON   single nodes. Type of data   oi.DeviceID=xx
-              is "JSON".                   oi.DevicePin=xxx
-                                           SensorData,ResposeCode=oi.ReadJSON()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-              To modify the control signal oi.DeviceID=xx
-4  WriteJSON  at single nodes. Type of     oi.DevicePin=xxx
-              data is "JSON".              oi.DataJSON={'Value': '10'}
-                                           SensorData,ResposeCode=oi.WriteJSON
-                                           ()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-              To read the sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-5  ReadXML    single nodes. Type of data   oi.DeviceID=xx
-              is "XML".                    oi.DevicePin=xxx
-                                           SensorData,ResposeCode=oi.ReadXML()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-              To modify the control signal oi.DeviceID=xx
-6  WriteXML   at single nodes. Type of     oi.DevicePin=xxx
-              data is "XML".               oi.DataXML='OpenIoE'
-                                           SensorData,ResposeCode=oi.WriteXML()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from  openioe.openioe_apis  import *
-                                           oi=openioe_apis()
-              To read the sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-7  Read       multiple nodes. Type of data oi.UserIDPinAPIKeys=[[xx, xxx], [x,
-              is "Numeric/String".         xxx]]
-                                           SensorData,ResposeCode=oi.Read()
-                                           print(SensorData)
-                                           print(ResposeCode)
-                                           from openioe.openioe_apis import *
-                                           oi=openioe_apis()
-                                           oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
-              To modify the control signal oi.UserIDPinAPIKeys=[[xx, xxx], [xx,
-8  Write      at multiple nodes. Type of   xxx]]
-              data is "Numeric/String".    oi.Data=[xx,xx]
-                                           Confirmation,ResposeCode=oi.ReadAPI
-                                           ()
-                                           print(Confirmation)
-                                           print(ResposeCode)
-              To display the developer     from openioe.openioe_apis import *
-3  Developer  information                  oi=openioe_apis()
-                                           oi.Developer()
+Metadata-Version: 2.1 Name: openioe Version: 1.1.0 Summary: Open IoE Home-page:
+https://openioe.gnanodaya.org/ Author: Venkataswamy R Author-email:
+opensourceioe@gmail.com Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE ## Open IoE Open IoE is a simple IoT platform to
+operate IoT devices. There are two options available, 1. Python Library
+(Client) 2. Web services (REST APIs) --- ### 1\. Python Library Users are
+expected to take these steps, 1. Install Python Library `pip install openioe`
+2. Write the client code using the following methods #### Method List:
+No Method       Description      Example
+                                 from openioe.openioe_apis import *
+                To read the      oi=openioe_apis()
+                sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+1  ReadValue    single nodes.    oi.DeviceID=xx
+                Type of data is  oi.DevicePin=xxx
+                "Numeric/String" SensorData,ResposeCode=oi.ReadValue()
+                                 print(SensorData)
+                                 print(ResposeCode)
+                                 from openioe.openioe_apis import *
+                To modify the    oi=openioe_apis()
+                control signal   oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+                at single nodes. oi.DeviceID=xx
+2  WriteValue   Type of data is  oi.DevicePin=xx
+                "Numeric/        oi.Data=10
+                String".         SensorData,ResposeCode=oi.WriteValue()
+                                 print(SensorData)
+                                 print(ResposeCode)
+                                 from openioe.openioe_apis import *
+                To read the      oi=openioe_apis()
+                sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+3  ReadJSON     single nodes.    oi.DeviceID=xx
+                Type of data is  oi.DevicePin=xxx
+                "JSON".          SensorData,ResposeCode=oi.ReadJSON()
+                                 print(SensorData)
+                                 print(ResposeCode)
+                                 from openioe.openioe_apis import *
+                                 oi=openioe_apis()
+                To modify the    oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+                control signal   oi.DeviceID=xx
+4  WriteJSON    at single nodes. oi.DevicePin=xxx
+                Type of data is  oi.DataJSON={'Value': '10'}
+                "JSON".          SensorData,ResposeCode=oi.WriteJSON()
+                                 print(SensorData)
+                                 print(ResposeCode)
+                                 from openioe.openioe_apis import *
+                To read the      oi=openioe_apis()
+                sensor data from oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+5  ReadXML      single nodes.    oi.DeviceID=xx
+                Type of data is  oi.DevicePin=xxx
+                "XML".           SensorData,ResposeCode=oi.ReadXML()
+                                 print(SensorData)
+                                 print(ResposeCode)
+                                 from openioe.openioe_apis import *
+                                 oi=openioe_apis()
+                To modify the    oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+                control signal   oi.DeviceID=xx
+6  WriteXML     at single nodes. oi.DevicePin=xxx
+                Type of data is  oi.DataXML='OpenIoE'
+                "XML".           SensorData,ResposeCode=oi.WriteXML()
+                                 print(SensorData)
+                                 print(ResposeCode)
+                To read the      from openioe.openioe_apis import *
+                sensor data from oi=openioe_apis()
+                multiple nodes.  oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+7  Read         Type of data is  oi.UserIDPinAPIKeys=[[xx, xxx], [x, xxx]]
+                "Numeric/        SensorData,ResposeCode=oi.Read()
+                String".         print(SensorData)
+                                 print(ResposeCode)
+                To modify the    from openioe.openioe_apis import *
+                control signal   oi=openioe_apis()
+                at multiple      oi.APIKey='xxxxxxxxxxxxxxxxxxxx';
+8  Write        nodes. Type of   oi.UserIDPinAPIKeys=[[xx, xxx], [xx, xxx]]
+                data is          oi.Data=[xx,xx]
+                "Numeric/        Confirmation,ResposeCode=oi.ReadAPI()
+                String".         print(Confirmation)
+                                 print(ResposeCode)
+                                 from openioe.openioe_apis import *
+                                 oi.UserEmail='xxxxxxxxxx'
+                To generate new  oi.UserPassword='xxxxxxxxxxx'
+   Generate API API key for a    ResponseJson,ResponseCode=oi.GenerateAPIKey
+9  Key          given email and  ()
+                password.        print(ResponseJson['User ID'])
+                                 print(ResponseJson['API Key'])
+                                 print(ResponseJson['Message'])
+                                 print(ResponseCode)
+                                 from openioe.openioe_apis import *
+                To add new IoT   oi.APIKey='pnHEmHgjFl0PT247Eae9'
+                device for a     oi.DeviceName='Test000'
+10 Create New   given API key,   oi.CryptoName='None'
+   Device       name, cryptotype oi.DataFormat='Value' # 'XML' or 'JSON'
+                and data format. ResponseTest,ResponseCode=oi.CreateDevice()
+                                 print(ResponseTest)
+                                 print(ResponseCode)
+                To display the   from openioe.openioe_apis import *
+11 Developer    developer        oi=openioe_apis()
+                information      oi.Developer()
 --- ### 2\. Web Services Users are expected to take these steps, 1. Register
 and login to OpenIoE- [Register/Login](https://openioe.gnanodaya.org/) 2.
 Create API Key/ Get API Key from OpenIoE. 3. Embed the API Key, Device ID and
 Pin into the client code. #### Visit the OpenIoE 3.0 web portal at [https://
 openioe.gnanodaya.org](https://openioe.gnanodaya.org) #### Visit the OpenIoE
 3.0 Help Portal at [https://openioedoc.gnanodaya.org](https://
 openioedoc.gnanodaya.org) #### API List:
@@ -101,21 +117,28 @@
                      parameter                         <apikey>/2/433 <Data>
                      To get hardware XML               <endpoint>/
 5  showdevicexml     file from web service.  http get  showdevicexml/<apikey>/
                                                        2/433
                      Update the hardware XML           <endpoint>/
 6  updatedevicexml   passed as parameter     http post updatedevicexml/
                                                        <apikey>/2/433 <Data>
+                     Generate new API Key by           <endpoint>/
+7  generateapikey    providing user creds    http get  generateapikey/
+                                                       <emailid>/<password>
+                                                       <endpoint>/
+                     Add new IoT device to             createuserdevice/
+8  createuserdevice  your account            http get  <APIKey>/<DeviceName>/
+                                                       <CryptoName>/
+                                                       <DataFormat>
 --- ### Developers
 [Dr. Venkataswamy R]
-Thanks and Regards,
+Thanks and Regards
 Venkataswamy R
-Assistant Professor,
+Assistant Professor
 Department of Electrical and Electronics Engineering,
-School of Engineering and Technology,
-Christ (Deemed to be University),
+School of Engineering and Technology
+Christ (Deemed to be University)
 Bengaluru-560074, India
 
-[Image result for phone icon] 080-4012-9961 (O)  [Image result for mobile
-icon]+91-7829222446 [Related image]venkatswamy.in
+[Related image] venkatswamy.in
```

### Comparing `openioe-1.0.0/openioe/openioe_apis.py` & `openioe-1.1.0/openioe/openioe_apis.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,54 @@
         self.response_text=[]
         self.response_status_code=[]  
         self.DeviceID=0
         self.DevicePin=0
         self.Data=[]
         self.DataJSON=''
         self.DataXML=''
+        self.UserEmail=''
+        self.UserPassword=''
+        self.DeviceName='D'+DateNumberGeneration()
+        self.CryptoName='None'
+        self.DataFormat='Value'
+
         if len(args) == 0:
             self.a=0           
         elif len(args) == 1:
             self.a=args[0]
             
     def Developer(self, *args):
         print('Hi, Welcome to OpenIoE')
         print('Developed by Dr. Venkataswamy R')
         print('https://venkataswamy.in')
         print('venkataswamy.r@gmail.com')
+
+    def GenerateAPIKey(self, *args):
+        import requests
+        import json
+        if len(args) == 0:
+            u=self.endpoint+'generateapikey/'+str(self.UserEmail)+'/'+str(self.UserPassword)+'/'
+            resp = requests.get(u)
+            self.response_text=resp.json()
+            self.response_status_code=resp.status_code
+        else:
+            print('Do not Pass parameters')
+        return self.response_text, self.response_status_code
+
+    def CreateDevice(self, *args):
+        import requests
+        if len(args) == 0:
+            u=self.endpoint+'createuserdevice/'+str(self.APIKey)+'/'+str(self.DeviceName)+'/'+str(self.CryptoName)+'/'+str(self.DataFormat)+'/'
+            print(u)
+            resp = requests.get(u)
+            self.response_text=resp.text
+            self.response_status_code=resp.status_code
+        else:
+            print('Do not Pass parameters')
+        return self.response_text, self.response_status_code
         
     def Read(self, *args):
         import requests
         if len(args) == 0:
             for i in range(len(self.Devices)):
                 u=self.endpoint+'showdevicevalue/'+str(self.APIKey)+'/'+str(self.Devices[i][0])+'/'+str(self.Devices[i][1])+'/'
                 resp = requests.get(u)
@@ -112,10 +142,16 @@
                 u=self.endpoint+'updatedevicevalue/'+str(self.APIKey)+'/'+str(self.Devices[i][0])+'/'+str(self.Devices[i][1])+'/'+str(self.Data[i])
                 resp = requests.get(u)
                 self.response_text.append(resp.text)
                 self.response_status_code.append(resp.status_code)
         else:
             print('Do not Pass parameters')
         return self.response_text, self.response_status_code
+    
+def DateNumberGeneration():
+    from datetime import datetime
+    a = datetime.now()
+    a = int(a.strftime('%Y%m%d%H%M%S'))
+    return str(a)
```

### Comparing `openioe-1.0.0/setup.py` & `openioe-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="openioe", # Replace with your own username
-    version="1.0.0",
+    version="1.1.0",
     author="Venkataswamy R",
 	scripts=['openioe\openioe_apis.py'] ,
     author_email="opensourceioe@gmail.com",
     description="Open IoE",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://openioe.gnanodaya.org/",
```

