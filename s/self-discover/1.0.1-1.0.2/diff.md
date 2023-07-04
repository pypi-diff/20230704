# Comparing `tmp/self-discover-1.0.1.tar.gz` & `tmp/self-discover-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "self-discover-1.0.1.tar", last modified: Sun Jul  2 23:10:37 2023, max compression
+gzip compressed data, was "self-discover-1.0.2.tar", last modified: Tue Jul  4 20:05:38 2023, max compression
```

## Comparing `self-discover-1.0.1.tar` & `self-discover-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 23:10:37.550544 self-discover-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-02 19:11:24.000000 self-discover-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1232 2023-07-02 23:10:37.554544 self-discover-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      587 2023-07-02 19:29:21.000000 self-discover-1.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-07-02 19:11:24.000000 self-discover-1.0.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 23:10:37.550544 self-discover-1.0.1/self_discover/
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-02 19:11:24.000000 self-discover-1.0.1/self_discover/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3146 2023-07-02 23:04:36.000000 self-discover-1.0.1/self_discover/main.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-07-02 19:11:24.000000 self-discover-1.0.1/self_discover/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     4455 2023-07-02 23:04:36.000000 self-discover-1.0.1/self_discover/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 23:10:37.550544 self-discover-1.0.1/self_discover.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1232 2023-07-02 23:10:37.000000 self-discover-1.0.1/self_discover.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      336 2023-07-02 23:10:37.000000 self-discover-1.0.1/self_discover.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 23:10:37.000000 self-discover-1.0.1/self_discover.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-02 23:10:37.000000 self-discover-1.0.1/self_discover.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-02 23:10:37.000000 self-discover-1.0.1/self_discover.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-02 23:10:37.554544 self-discover-1.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1216 2023-07-02 23:09:00.000000 self-discover-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 20:05:38.475455 self-discover-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-02 19:11:24.000000 self-discover-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-07-04 20:05:38.475455 self-discover-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      587 2023-07-02 19:29:21.000000 self-discover-1.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-07-02 19:11:24.000000 self-discover-1.0.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 20:05:38.471455 self-discover-1.0.2/self_discover/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-02 19:11:24.000000 self-discover-1.0.2/self_discover/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3146 2023-07-02 23:04:36.000000 self-discover-1.0.2/self_discover/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-07-02 19:11:24.000000 self-discover-1.0.2/self_discover/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     4475 2023-07-04 20:04:43.000000 self-discover-1.0.2/self_discover/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 20:05:38.475455 self-discover-1.0.2/self_discover.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-07-04 20:05:38.000000 self-discover-1.0.2/self_discover.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      336 2023-07-04 20:05:38.000000 self-discover-1.0.2/self_discover.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 20:05:38.000000 self-discover-1.0.2/self_discover.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-04 20:05:38.000000 self-discover-1.0.2/self_discover.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-04 20:05:38.000000 self-discover-1.0.2/self_discover.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-04 20:05:38.475455 self-discover-1.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1216 2023-07-04 20:02:32.000000 self-discover-1.0.2/setup.py
```

### Comparing `self-discover-1.0.1/LICENSE` & `self-discover-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `self-discover-1.0.1/PKG-INFO` & `self-discover-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: self-discover
-Version: 1.0.1
+Version: 1.0.2
 Summary: Self Discover serves autodiscover (Outlook) and autoconfig (Thunderbird) XML files for mail auto-configuration.
 Home-page: https://github.com/CyberfusionIO/Self-Discover
 Author: William Edwards
 Author-email: support@cyberfusion.nl
 License: MIT
 Keywords: cyberfusion,fastapi,mail,email,outlook,thunderbird,autodiscover,autoconfig
 Platform: linux
```

### Comparing `self-discover-1.0.1/README.md` & `self-discover-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `self-discover-1.0.1/self_discover/main.py` & `self-discover-1.0.2/self_discover/main.py`

 * *Files identical despite different names*

### Comparing `self-discover-1.0.1/self_discover/utilities.py` & `self-discover-1.0.2/self_discover/utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 ) -> str:
     """Get POX ('plain old XML') autodiscover response.
 
     See: https://learn.microsoft.com/en-us/exchange/client-developer/web-service-reference/pox-autodiscover-response-for-exchange
     """
     root = ET.Element(
         "Autodiscover",
-        xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006",
+        xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006",
     )
 
     Response = ET.SubElement(
         root,
         "Response",
-        xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a",
+        xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a",
     )
 
     Account = ET.SubElement(Response, "Account")
     ET.SubElement(Account, "AccountType").text = "email"
     ET.SubElement(Account, "Action").text = "settings"
 
     Protocol = ET.SubElement(Account, "Protocol")
@@ -74,15 +74,15 @@
     ET.SubElement(Protocol, "AuthRequired").text = "on"
     ET.SubElement(Protocol, "UsePOPAuth").text = "off"
     ET.SubElement(Protocol, "SMTPLast").text = "off"
 
     tree = ET.ElementTree(root)
     ET.indent(tree, space="    ", level=0)
 
-    return ET.tostring(root, encoding="unicode") + "\n"
+    return ET.tostring(root, encoding="unicode", xml_declaration=True) + "\n"
 
 
 def get_thunderbird_autoconfig_response(
     imap_server_hostname: str,
     pop3_server_hostname: str,
     smtp_server_hostname: str,
     login_name: str,
```

### Comparing `self-discover-1.0.1/self_discover.egg-info/PKG-INFO` & `self-discover-1.0.2/self_discover.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: self-discover
-Version: 1.0.1
+Version: 1.0.2
 Summary: Self Discover serves autodiscover (Outlook) and autoconfig (Thunderbird) XML files for mail auto-configuration.
 Home-page: https://github.com/CyberfusionIO/Self-Discover
 Author: William Edwards
 Author-email: support@cyberfusion.nl
 License: MIT
 Keywords: cyberfusion,fastapi,mail,email,outlook,thunderbird,autodiscover,autoconfig
 Platform: linux
```

### Comparing `self-discover-1.0.1/setup.py` & `self-discover-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="self-discover",
-    version="1.0.1",
+    version="1.0.2",
     description="Self Discover serves autodiscover (Outlook) and autoconfig (Thunderbird) XML files for mail auto-configuration.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     author="William Edwards",
     author_email="support@cyberfusion.nl",
     url="https://github.com/CyberfusionIO/Self-Discover",
```

