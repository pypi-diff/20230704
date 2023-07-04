# Comparing `tmp/re_it-1.0.0.1.tar.gz` & `tmp/re_it-1.1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\re_it-1.0.0.1.tar", last modified: Tue Jul  4 08:50:57 2023, max compression
+gzip compressed data, was "dist\re_it-1.1.1.0.tar", last modified: Tue Jul  4 09:33:20 2023, max compression
```

## Comparing `re_it-1.0.0.1.tar` & `re_it-1.1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 08:50:57.000000 re_it-1.0.0.1/
--rw-rw-rw-   0        0        0     6370 2023-07-04 08:50:57.000000 re_it-1.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4939 2023-07-04 08:50:48.000000 re_it-1.0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 08:50:57.000000 re_it-1.0.0.1/re_it/
--rw-rw-rw-   0        0        0        0 2023-07-04 08:28:05.000000 re_it-1.0.0.1/re_it/__init__.py
--rw-rw-rw-   0        0        0      754 2023-07-04 08:29:10.000000 re_it-1.0.0.1/re_it/请求.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:50:57.000000 re_it-1.0.0.1/re_it.egg-info/
--rw-rw-rw-   0        0        0     6370 2023-07-04 08:50:57.000000 re_it-1.0.0.1/re_it.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-07-04 08:50:57.000000 re_it-1.0.0.1/re_it.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 08:50:57.000000 re_it-1.0.0.1/re_it.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 08:50:57.000000 re_it-1.0.0.1/re_it.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 08:50:57.000000 re_it-1.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      527 2023-07-04 08:50:48.000000 re_it-1.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:33:20.000000 re_it-1.1.1.0/
+-rw-rw-rw-   0        0        0     6567 2023-07-04 09:33:20.000000 re_it-1.1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5104 2023-07-04 09:32:30.000000 re_it-1.1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 09:33:20.000000 re_it-1.1.1.0/re_it/
+-rw-rw-rw-   0        0        0        0 2023-07-04 08:28:05.000000 re_it-1.1.1.0/re_it/__init__.py
+-rw-rw-rw-   0        0        0      856 2023-07-04 09:28:25.000000 re_it-1.1.1.0/re_it/请求.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:33:20.000000 re_it-1.1.1.0/re_it.egg-info/
+-rw-rw-rw-   0        0        0     6567 2023-07-04 09:33:20.000000 re_it-1.1.1.0/re_it.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-07-04 09:33:20.000000 re_it-1.1.1.0/re_it.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 09:33:20.000000 re_it-1.1.1.0/re_it.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 09:33:20.000000 re_it-1.1.1.0/re_it.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 09:33:20.000000 re_it-1.1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      527 2023-07-04 09:32:30.000000 re_it-1.1.1.0/setup.py
```

### Comparing `re_it-1.0.0.1/PKG-INFO` & `re_it-1.1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 Metadata-Version: 2.1
 Name: re_it
-Version: 1.0.0.1
+Version: 1.1.1.0
 Summary: 中文的python网络请求库！
 Home-page: https://pypi.org/user/SuiBo/
 Author: SuiBo
 Author-email: 534047068@qq.com
 License: UNKNOWN
 Description: # re_it  中文的python网络请求库！
         >如果程序错了，请报告给534047068@qq.com。
         ****
+        ![快捷输入](p/kjsr.png)<br>
+        输入首字母快速输入，不用切换输入法。<br>
+        （我用的pycharm）
+        ****
         你可以按照以下步骤使用这个包，并在代码中添加注释以更好地理解其功能和用法：
         导入 re_it 模块：`from re_it import 请求`<br>
         创建一个请求对象实例：
-        ```ruby
+        ```python
         我的请求实例 = 请求.我的请求()
         ```
-        使用 `添加头部()` 方法为请求添加头部信息：
-        ```ruby
+        使用 `添加头部()` 方法为请求添加头部信息（有默认请求头）：
+        ```python
         我的请求实例.添加头部('User-Agent', 'Mozilla/5.0')  # 添加User-Agent头部信息
         我的请求实例.添加头部('Content-Type', 'application/json')  # 添加Authorization头部信息
         ```
         发送 GET 请求并获取响应内容：
-        ```ruby
+        ```python
         网址 = "www.example.com"  # 设置目标网址
         响应内容 = 我的请求实例.获取(网址)  # 发送GET请求并获取响应内容
         print(响应内容)  # 打印响应内容
         ```
         发送 POST 请求并获取响应内容：
-        ```ruby
+        ```python
         网址 = "www.example.com"  # 设置目标网址
         数据 = "key1=value1&key2=value2"  # 设置POST请求的数据，可选参数
         响应内容 = 我的请求实例.提交(网址, 数据)  # 发送POST请求并获取响应内容
         print(响应内容)  # 打印响应内容
         ```
         输出：
-        ```ruby
+        ```html
         <!doctype html>
         <html>
         <head>
             <title>Example Domain</title>
         
             <meta charset="utf-8" />
             <meta http-equiv="Content-type" content="text/html; charset=utf-8" />
@@ -130,26 +134,26 @@
         </html>
         ```
         ****
         这个网络请求包中的函数有一些可选参数和必选参数。下面是每个函数的参数说明：<br>
         `添加头部(self, 键, 值)` 函数：<br>
         
         必选参数：<br>
-        `键`：要添加到请求头部的键。<br>
-        `值`：要添加到请求头部的值。<br>
+        + `键`：要添加到请求头部的键。<br>
+        + `值`：要添加到请求头部的值。<br>
         `获取(self, 网址)` 函数：<br>
         
         必选参数：<br>
-        `网址`：目标网址，用于建立连接并发送 GET 请求。<br>
+        + `网址`：目标网址，用于建立连接并发送 GET 请求。<br>
         `提交(self, 网址, 数据=None)` 函数：<br>
         
         必选参数：<br>
-        `网址`：目标网址，用于建立连接并发送 POST 请求。<br>
+        + `网址`：目标网址，用于建立连接并发送 POST 请求。<br>
         可选参数：<br>
-        `数据`：POST 请求的数据，使用 URL 编码格式（例如，"key1=value1&key2=value2"）。默认值为 None，即没有请求数据。<br><br>
+        + `数据`：POST 请求的数据，使用 URL 编码格式（例如，"key1=value1&key2=value2"）。默认值为 None，即没有请求数据。<br><br>
         所有的函数都是在一个名为 "我的请求" 的类中定义的，并且都需要通过类的实例进行调用（如 请求.函数名()）。<br>
         
         需要注意的是，根据具体的使用情况，你可能需要根据需要自定义请求头部信息和请求数据，并根据目标网址发送相应的请求。<br>
         ****
         > version : 1.0.0.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 2.1 Name: re_it Version: 1.0.0.1 Summary: 中文的python网络请求库！
+Metadata-Version: 2.1 Name: re_it Version: 1.1.1.0 Summary: 中文的python网络请求库！
 Home-page: https://pypi.org/user/SuiBo/ Author: SuiBo Author-email:
 534047068@qq.com License: UNKNOWN Description: # re_it 中文的python网络请求库！
->如果程序错了，请报告给534047068@qq.com。 **** 你可以按照以下步骤使用这个包，并在代码中添加注释以更好地理解其功能和用法： 导入
-re_it 模块：`from re_it import 请求`
-创建一个请求对象实例： ```ruby 我的请求实例 = 请求.我的请求() ``` 使用 `添加头部()` 方法为请求添加头部信息： ```ruby
-我的请求实例.添加头部('User-Agent', 'Mozilla/5.0') # 添加User-Agent头部信息 我的请求实例.添加头部
-('Content-Type', 'application/json') # 添加Authorization头部信息 ``` 发送 GET
-请求并获取响应内容： ```ruby 网址 = "www.example.com" # 设置目标网址 响应内容 = 我的请求实例.获取(网址) #
-发送GET请求并获取响应内容 print(响应内容) # 打印响应内容 ``` 发送 POST 请求并获取响应内容： ```ruby 网址 =
+>如果程序错了，请报告给534047068@qq.com。 **** ![快捷输入](p/kjsr.png)
+输入首字母快速输入，不用切换输入法。
+（我用的pycharm） **** 你可以按照以下步骤使用这个包，并在代码中添加注释以更好地理解其功能和用法： 导入 re_it 模块：`from re_it
+import 请求`
+创建一个请求对象实例： ```python 我的请求实例 = 请求.我的请求() ``` 使用 `添加头部()` 方法为请求添加头部信息（有默认请求头）：
+```python 我的请求实例.添加头部('User-Agent', 'Mozilla/5.0') # 添加User-Agent头部信息
+我的请求实例.添加头部('Content-Type', 'application/json') # 添加Authorization头部信息 ``` 发送
+GET 请求并获取响应内容： ```python 网址 = "www.example.com" # 设置目标网址 响应内容 = 我的请求实例.获取(网址) #
+发送GET请求并获取响应内容 print(响应内容) # 打印响应内容 ``` 发送 POST 请求并获取响应内容： ```python 网址 =
 "www.example.com" # 设置目标网址 数据 = "key1=value1&key2=value2" # 设置POST请求的数据，可选参数
-响应内容 = 我的请求实例.提交(网址, 数据) # 发送POST请求并获取响应内容 print(响应内容) # 打印响应内容 ``` 输出： ```ruby
+响应内容 = 我的请求实例.提交(网址, 数据) # 发送POST请求并获取响应内容 print(响应内容) # 打印响应内容 ``` 输出： ```html
 
 
 ****** Example Domain ******
 This domain is for use in illustrative examples in documents. You may use this
 domain in literature without prior coordination or asking for permission.
 More_information...
 
@@ -21,22 +23,22 @@
 ****** Example Domain ******
 This domain is for use in illustrative examples in documents. You may use this
 domain in literature without prior coordination or asking for permission.
 More_information...
 ``` **** 这个网络请求包中的函数有一些可选参数和必选参数。下面是每个函数的参数说明：
 `添加头部(self, 键, 值)` 函数：
 必选参数：
-`键`：要添加到请求头部的键。
-`值`：要添加到请求头部的值。
++ `键`：要添加到请求头部的键。
++ `值`：要添加到请求头部的值。
 `获取(self, 网址)` 函数：
 必选参数：
-`网址`：目标网址，用于建立连接并发送 GET 请求。
++ `网址`：目标网址，用于建立连接并发送 GET 请求。
 `提交(self, 网址, 数据=None)` 函数：
 必选参数：
-`网址`：目标网址，用于建立连接并发送 POST 请求。
++ `网址`：目标网址，用于建立连接并发送 POST 请求。
 可选参数：
-`数据`：POST 请求的数据，使用 URL 编码格式（例如，"key1=value1&key2=value2"）。默认值为 None，即没有请求数据。
++ `数据`：POST 请求的数据，使用 URL 编码格式（例如，"key1=value1&key2=value2"）。默认值为 None，即没有请求数据。
 
 所有的函数都是在一个名为 "我的请求" 的类中定义的，并且都需要通过类的实例进行调用（如 请求.函数名()）。
 需要注意的是，根据具体的使用情况，你可能需要根据需要自定义请求头部信息和请求数据，并根据目标网址发送相应的请求。
 **** > version : 1.0.0.0 Platform: UNKNOWN Description-Content-Type: text/
 markdown
```

### Comparing `re_it-1.0.0.1/README.md` & `re_it-1.1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # re_it  中文的python网络请求库！
 >如果程序错了，请报告给534047068@qq.com。
 ****
+![快捷输入](p/kjsr.png)<br>
+输入首字母快速输入，不用切换输入法。<br>
+（我用的pycharm）
+****
 你可以按照以下步骤使用这个包，并在代码中添加注释以更好地理解其功能和用法：
 导入 re_it 模块：`from re_it import 请求`<br>
 创建一个请求对象实例：
-```ruby
+```python
 我的请求实例 = 请求.我的请求()
 ```
-使用 `添加头部()` 方法为请求添加头部信息：
-```ruby
+使用 `添加头部()` 方法为请求添加头部信息（有默认请求头）：
+```python
 我的请求实例.添加头部('User-Agent', 'Mozilla/5.0')  # 添加User-Agent头部信息
 我的请求实例.添加头部('Content-Type', 'application/json')  # 添加Authorization头部信息
 ```
 发送 GET 请求并获取响应内容：
-```ruby
+```python
 网址 = "www.example.com"  # 设置目标网址
 响应内容 = 我的请求实例.获取(网址)  # 发送GET请求并获取响应内容
 print(响应内容)  # 打印响应内容
 ```
 发送 POST 请求并获取响应内容：
-```ruby
+```python
 网址 = "www.example.com"  # 设置目标网址
 数据 = "key1=value1&key2=value2"  # 设置POST请求的数据，可选参数
 响应内容 = 我的请求实例.提交(网址, 数据)  # 发送POST请求并获取响应内容
 print(响应内容)  # 打印响应内容
 ```
 输出：
-```ruby
+```html
 <!doctype html>
 <html>
 <head>
     <title>Example Domain</title>
 
     <meta charset="utf-8" />
     <meta http-equiv="Content-type" content="text/html; charset=utf-8" />
@@ -122,24 +126,24 @@
 </html>
 ```
 ****
 这个网络请求包中的函数有一些可选参数和必选参数。下面是每个函数的参数说明：<br>
 `添加头部(self, 键, 值)` 函数：<br>
 
 必选参数：<br>
-`键`：要添加到请求头部的键。<br>
-`值`：要添加到请求头部的值。<br>
++ `键`：要添加到请求头部的键。<br>
++ `值`：要添加到请求头部的值。<br>
 `获取(self, 网址)` 函数：<br>
 
 必选参数：<br>
-`网址`：目标网址，用于建立连接并发送 GET 请求。<br>
++ `网址`：目标网址，用于建立连接并发送 GET 请求。<br>
 `提交(self, 网址, 数据=None)` 函数：<br>
 
 必选参数：<br>
-`网址`：目标网址，用于建立连接并发送 POST 请求。<br>
++ `网址`：目标网址，用于建立连接并发送 POST 请求。<br>
 可选参数：<br>
-`数据`：POST 请求的数据，使用 URL 编码格式（例如，"key1=value1&key2=value2"）。默认值为 None，即没有请求数据。<br><br>
++ `数据`：POST 请求的数据，使用 URL 编码格式（例如，"key1=value1&key2=value2"）。默认值为 None，即没有请求数据。<br><br>
 所有的函数都是在一个名为 "我的请求" 的类中定义的，并且都需要通过类的实例进行调用（如 请求.函数名()）。<br>
 
 需要注意的是，根据具体的使用情况，你可能需要根据需要自定义请求头部信息和请求数据，并根据目标网址发送相应的请求。<br>
 ****
 > version : 1.0.0.0
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
-# re_it 中文的python网络请求库！ >如果程序错了，请报告给534047068@qq.com。 ****
-你可以按照以下步骤使用这个包，并在代码中添加注释以更好地理解其功能和用法： 导入 re_it 模块：`from re_it import 请求`
-创建一个请求对象实例： ```ruby 我的请求实例 = 请求.我的请求() ``` 使用 `添加头部()` 方法为请求添加头部信息： ```ruby
-我的请求实例.添加头部('User-Agent', 'Mozilla/5.0') # 添加User-Agent头部信息 我的请求实例.添加头部
-('Content-Type', 'application/json') # 添加Authorization头部信息 ``` 发送 GET
-请求并获取响应内容： ```ruby 网址 = "www.example.com" # 设置目标网址 响应内容 = 我的请求实例.获取(网址) #
-发送GET请求并获取响应内容 print(响应内容) # 打印响应内容 ``` 发送 POST 请求并获取响应内容： ```ruby 网址 =
+# re_it 中文的python网络请求库！ >如果程序错了，请报告给534047068@qq.com。 **** ![快捷输入](p/kjsr.png)
+输入首字母快速输入，不用切换输入法。
+（我用的pycharm） **** 你可以按照以下步骤使用这个包，并在代码中添加注释以更好地理解其功能和用法： 导入 re_it 模块：`from re_it
+import 请求`
+创建一个请求对象实例： ```python 我的请求实例 = 请求.我的请求() ``` 使用 `添加头部()` 方法为请求添加头部信息（有默认请求头）：
+```python 我的请求实例.添加头部('User-Agent', 'Mozilla/5.0') # 添加User-Agent头部信息
+我的请求实例.添加头部('Content-Type', 'application/json') # 添加Authorization头部信息 ``` 发送
+GET 请求并获取响应内容： ```python 网址 = "www.example.com" # 设置目标网址 响应内容 = 我的请求实例.获取(网址) #
+发送GET请求并获取响应内容 print(响应内容) # 打印响应内容 ``` 发送 POST 请求并获取响应内容： ```python 网址 =
 "www.example.com" # 设置目标网址 数据 = "key1=value1&key2=value2" # 设置POST请求的数据，可选参数
-响应内容 = 我的请求实例.提交(网址, 数据) # 发送POST请求并获取响应内容 print(响应内容) # 打印响应内容 ``` 输出： ```ruby
+响应内容 = 我的请求实例.提交(网址, 数据) # 发送POST请求并获取响应内容 print(响应内容) # 打印响应内容 ``` 输出： ```html
 
 
 ****** Example Domain ******
 This domain is for use in illustrative examples in documents. You may use this
 domain in literature without prior coordination or asking for permission.
 More_information...
 
@@ -18,21 +20,21 @@
 ****** Example Domain ******
 This domain is for use in illustrative examples in documents. You may use this
 domain in literature without prior coordination or asking for permission.
 More_information...
 ``` **** 这个网络请求包中的函数有一些可选参数和必选参数。下面是每个函数的参数说明：
 `添加头部(self, 键, 值)` 函数：
 必选参数：
-`键`：要添加到请求头部的键。
-`值`：要添加到请求头部的值。
++ `键`：要添加到请求头部的键。
++ `值`：要添加到请求头部的值。
 `获取(self, 网址)` 函数：
 必选参数：
-`网址`：目标网址，用于建立连接并发送 GET 请求。
++ `网址`：目标网址，用于建立连接并发送 GET 请求。
 `提交(self, 网址, 数据=None)` 函数：
 必选参数：
-`网址`：目标网址，用于建立连接并发送 POST 请求。
++ `网址`：目标网址，用于建立连接并发送 POST 请求。
 可选参数：
-`数据`：POST 请求的数据，使用 URL 编码格式（例如，"key1=value1&key2=value2"）。默认值为 None，即没有请求数据。
++ `数据`：POST 请求的数据，使用 URL 编码格式（例如，"key1=value1&key2=value2"）。默认值为 None，即没有请求数据。
 
 所有的函数都是在一个名为 "我的请求" 的类中定义的，并且都需要通过类的实例进行调用（如 请求.函数名()）。
 需要注意的是，根据具体的使用情况，你可能需要根据需要自定义请求头部信息和请求数据，并根据目标网址发送相应的请求。
 **** > version : 1.0.0.0
```

### Comparing `re_it-1.0.0.1/re_it/请求.py` & `re_it-1.1.1.0/re_it/请求.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import http.client
 
 class 我的请求:
     def __init__(self):
-        self.headers = {}
+        self.headers = {
+            'User-Agent': 'Mozilla/5.0',
+            'Content-Type': 'application/json'
+        }
 
     def 添加头部(self, 键, 值):
         self.headers[键] = 值
 
     def 获取(self, 网址):
         conn = http.client.HTTPSConnection(网址)
         conn.request("GET", "/", headers=self.headers)
@@ -17,8 +20,8 @@
 
     def 提交(self, 网址, 数据=None):
         conn = http.client.HTTPSConnection(网址)
         conn.request("POST", "/", body=数据, headers=self.headers)
         response = conn.getresponse()
         响应内容 = response.read().decode()
         conn.close()
-        return 响应内容
+        return 响应内容
```

### Comparing `re_it-1.0.0.1/re_it.egg-info/PKG-INFO` & `re_it-1.1.1.0/re_it.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 Metadata-Version: 2.1
 Name: re-it
-Version: 1.0.0.1
+Version: 1.1.1.0
 Summary: 中文的python网络请求库！
 Home-page: https://pypi.org/user/SuiBo/
 Author: SuiBo
 Author-email: 534047068@qq.com
 License: UNKNOWN
 Description: # re_it  中文的python网络请求库！
         >如果程序错了，请报告给534047068@qq.com。
         ****
+        ![快捷输入](p/kjsr.png)<br>
+        输入首字母快速输入，不用切换输入法。<br>
+        （我用的pycharm）
+        ****
         你可以按照以下步骤使用这个包，并在代码中添加注释以更好地理解其功能和用法：
         导入 re_it 模块：`from re_it import 请求`<br>
         创建一个请求对象实例：
-        ```ruby
+        ```python
         我的请求实例 = 请求.我的请求()
         ```
-        使用 `添加头部()` 方法为请求添加头部信息：
-        ```ruby
+        使用 `添加头部()` 方法为请求添加头部信息（有默认请求头）：
+        ```python
         我的请求实例.添加头部('User-Agent', 'Mozilla/5.0')  # 添加User-Agent头部信息
         我的请求实例.添加头部('Content-Type', 'application/json')  # 添加Authorization头部信息
         ```
         发送 GET 请求并获取响应内容：
-        ```ruby
+        ```python
         网址 = "www.example.com"  # 设置目标网址
         响应内容 = 我的请求实例.获取(网址)  # 发送GET请求并获取响应内容
         print(响应内容)  # 打印响应内容
         ```
         发送 POST 请求并获取响应内容：
-        ```ruby
+        ```python
         网址 = "www.example.com"  # 设置目标网址
         数据 = "key1=value1&key2=value2"  # 设置POST请求的数据，可选参数
         响应内容 = 我的请求实例.提交(网址, 数据)  # 发送POST请求并获取响应内容
         print(响应内容)  # 打印响应内容
         ```
         输出：
-        ```ruby
+        ```html
         <!doctype html>
         <html>
         <head>
             <title>Example Domain</title>
         
             <meta charset="utf-8" />
             <meta http-equiv="Content-type" content="text/html; charset=utf-8" />
@@ -130,26 +134,26 @@
         </html>
         ```
         ****
         这个网络请求包中的函数有一些可选参数和必选参数。下面是每个函数的参数说明：<br>
         `添加头部(self, 键, 值)` 函数：<br>
         
         必选参数：<br>
-        `键`：要添加到请求头部的键。<br>
-        `值`：要添加到请求头部的值。<br>
+        + `键`：要添加到请求头部的键。<br>
+        + `值`：要添加到请求头部的值。<br>
         `获取(self, 网址)` 函数：<br>
         
         必选参数：<br>
-        `网址`：目标网址，用于建立连接并发送 GET 请求。<br>
+        + `网址`：目标网址，用于建立连接并发送 GET 请求。<br>
         `提交(self, 网址, 数据=None)` 函数：<br>
         
         必选参数：<br>
-        `网址`：目标网址，用于建立连接并发送 POST 请求。<br>
+        + `网址`：目标网址，用于建立连接并发送 POST 请求。<br>
         可选参数：<br>
-        `数据`：POST 请求的数据，使用 URL 编码格式（例如，"key1=value1&key2=value2"）。默认值为 None，即没有请求数据。<br><br>
+        + `数据`：POST 请求的数据，使用 URL 编码格式（例如，"key1=value1&key2=value2"）。默认值为 None，即没有请求数据。<br><br>
         所有的函数都是在一个名为 "我的请求" 的类中定义的，并且都需要通过类的实例进行调用（如 请求.函数名()）。<br>
         
         需要注意的是，根据具体的使用情况，你可能需要根据需要自定义请求头部信息和请求数据，并根据目标网址发送相应的请求。<br>
         ****
         > version : 1.0.0.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 2.1 Name: re-it Version: 1.0.0.1 Summary: 中文的python网络请求库！
+Metadata-Version: 2.1 Name: re-it Version: 1.1.1.0 Summary: 中文的python网络请求库！
 Home-page: https://pypi.org/user/SuiBo/ Author: SuiBo Author-email:
 534047068@qq.com License: UNKNOWN Description: # re_it 中文的python网络请求库！
->如果程序错了，请报告给534047068@qq.com。 **** 你可以按照以下步骤使用这个包，并在代码中添加注释以更好地理解其功能和用法： 导入
-re_it 模块：`from re_it import 请求`
-创建一个请求对象实例： ```ruby 我的请求实例 = 请求.我的请求() ``` 使用 `添加头部()` 方法为请求添加头部信息： ```ruby
-我的请求实例.添加头部('User-Agent', 'Mozilla/5.0') # 添加User-Agent头部信息 我的请求实例.添加头部
-('Content-Type', 'application/json') # 添加Authorization头部信息 ``` 发送 GET
-请求并获取响应内容： ```ruby 网址 = "www.example.com" # 设置目标网址 响应内容 = 我的请求实例.获取(网址) #
-发送GET请求并获取响应内容 print(响应内容) # 打印响应内容 ``` 发送 POST 请求并获取响应内容： ```ruby 网址 =
+>如果程序错了，请报告给534047068@qq.com。 **** ![快捷输入](p/kjsr.png)
+输入首字母快速输入，不用切换输入法。
+（我用的pycharm） **** 你可以按照以下步骤使用这个包，并在代码中添加注释以更好地理解其功能和用法： 导入 re_it 模块：`from re_it
+import 请求`
+创建一个请求对象实例： ```python 我的请求实例 = 请求.我的请求() ``` 使用 `添加头部()` 方法为请求添加头部信息（有默认请求头）：
+```python 我的请求实例.添加头部('User-Agent', 'Mozilla/5.0') # 添加User-Agent头部信息
+我的请求实例.添加头部('Content-Type', 'application/json') # 添加Authorization头部信息 ``` 发送
+GET 请求并获取响应内容： ```python 网址 = "www.example.com" # 设置目标网址 响应内容 = 我的请求实例.获取(网址) #
+发送GET请求并获取响应内容 print(响应内容) # 打印响应内容 ``` 发送 POST 请求并获取响应内容： ```python 网址 =
 "www.example.com" # 设置目标网址 数据 = "key1=value1&key2=value2" # 设置POST请求的数据，可选参数
-响应内容 = 我的请求实例.提交(网址, 数据) # 发送POST请求并获取响应内容 print(响应内容) # 打印响应内容 ``` 输出： ```ruby
+响应内容 = 我的请求实例.提交(网址, 数据) # 发送POST请求并获取响应内容 print(响应内容) # 打印响应内容 ``` 输出： ```html
 
 
 ****** Example Domain ******
 This domain is for use in illustrative examples in documents. You may use this
 domain in literature without prior coordination or asking for permission.
 More_information...
 
@@ -21,22 +23,22 @@
 ****** Example Domain ******
 This domain is for use in illustrative examples in documents. You may use this
 domain in literature without prior coordination or asking for permission.
 More_information...
 ``` **** 这个网络请求包中的函数有一些可选参数和必选参数。下面是每个函数的参数说明：
 `添加头部(self, 键, 值)` 函数：
 必选参数：
-`键`：要添加到请求头部的键。
-`值`：要添加到请求头部的值。
++ `键`：要添加到请求头部的键。
++ `值`：要添加到请求头部的值。
 `获取(self, 网址)` 函数：
 必选参数：
-`网址`：目标网址，用于建立连接并发送 GET 请求。
++ `网址`：目标网址，用于建立连接并发送 GET 请求。
 `提交(self, 网址, 数据=None)` 函数：
 必选参数：
-`网址`：目标网址，用于建立连接并发送 POST 请求。
++ `网址`：目标网址，用于建立连接并发送 POST 请求。
 可选参数：
-`数据`：POST 请求的数据，使用 URL 编码格式（例如，"key1=value1&key2=value2"）。默认值为 None，即没有请求数据。
++ `数据`：POST 请求的数据，使用 URL 编码格式（例如，"key1=value1&key2=value2"）。默认值为 None，即没有请求数据。
 
 所有的函数都是在一个名为 "我的请求" 的类中定义的，并且都需要通过类的实例进行调用（如 请求.函数名()）。
 需要注意的是，根据具体的使用情况，你可能需要根据需要自定义请求头部信息和请求数据，并根据目标网址发送相应的请求。
 **** > version : 1.0.0.0 Platform: UNKNOWN Description-Content-Type: text/
 markdown
```

### Comparing `re_it-1.0.0.1/setup.py` & `re_it-1.1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='re_it',
-    version='1.0.0.1',
+    version='1.1.1.0',
     author='SuiBo',
     author_email='534047068@qq.com',
     description='中文的python网络请求库！',
     install_requires=[
 
     ],
     py_modules=["re_it"],
```

