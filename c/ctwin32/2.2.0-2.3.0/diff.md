# Comparing `tmp/ctwin32-2.2.0.tar.gz` & `tmp/ctwin32-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctwin32-2.2.0.tar", last modified: Sat May 27 04:28:45 2023, max compression
+gzip compressed data, was "ctwin32-2.3.0.tar", last modified: Tue Jul  4 09:34:50 2023, max compression
```

## Comparing `ctwin32-2.2.0.tar` & `ctwin32-2.3.0.tar`

### file list

```diff
@@ -1,63 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 04:28:45.108689 ctwin32-2.2.0/
--rw-rw-rw-   0        0        0     1057 2023-01-07 08:48:10.000000 ctwin32-2.2.0/LICENSE
--rw-rw-rw-   0        0        0       14 2023-03-27 05:21:14.000000 ctwin32-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2575 2023-05-27 04:28:45.108689 ctwin32-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1651 2023-03-30 05:59:34.000000 ctwin32-2.2.0/README.md
--rw-rw-rw-   0        0        0     1617 2023-01-11 05:59:42.000000 ctwin32-2.2.0/bld.py
-drwxrwxrwx   0        0        0        0 2023-05-27 04:28:45.082105 ctwin32-2.2.0/ctwin32/
--rw-rw-rw-   0        0        0   222711 2023-05-27 04:25:20.000000 ctwin32-2.2.0/ctwin32/__init__.py
--rw-rw-rw-   0        0        0    39112 2023-05-26 05:24:56.000000 ctwin32-2.2.0/ctwin32/advapi.py
--rw-rw-rw-   0        0        0    17770 2023-04-11 05:50:33.000000 ctwin32-2.2.0/ctwin32/bcrypt.py
--rw-rw-rw-   0        0        0     4696 2023-01-07 08:47:22.000000 ctwin32-2.2.0/ctwin32/cfgmgr.py
--rw-rw-rw-   0        0        0     9079 2023-04-11 05:50:42.000000 ctwin32-2.2.0/ctwin32/comctl.py
--rw-rw-rw-   0        0        0     4352 2023-01-07 08:47:22.000000 ctwin32-2.2.0/ctwin32/gdi.py
--rw-rw-rw-   0        0        0    13791 2023-01-07 08:47:22.000000 ctwin32-2.2.0/ctwin32/iphlpapi.py
--rw-rw-rw-   0        0        0    42469 2023-05-06 04:06:32.000000 ctwin32-2.2.0/ctwin32/kernel.py
--rw-rw-rw-   0        0        0     5950 2023-01-07 08:47:22.000000 ctwin32-2.2.0/ctwin32/misc.py
--rw-rw-rw-   0        0        0     5174 2023-04-08 15:00:11.000000 ctwin32-2.2.0/ctwin32/msi.py
--rw-rw-rw-   0        0        0    17900 2023-05-26 17:30:01.000000 ctwin32-2.2.0/ctwin32/ntdll.py
--rw-rw-rw-   0        0        0     4182 2023-03-12 06:03:22.000000 ctwin32-2.2.0/ctwin32/psapi.py
--rw-rw-rw-   0        0        0     6252 2023-05-24 06:03:37.000000 ctwin32-2.2.0/ctwin32/secur.py
--rw-rw-rw-   0        0        0    17498 2023-04-08 15:00:11.000000 ctwin32-2.2.0/ctwin32/setupapi.py
--rw-rw-rw-   0        0        0     7921 2023-05-06 04:07:18.000000 ctwin32-2.2.0/ctwin32/shell.py
--rw-rw-rw-   0        0        0    44298 2023-05-27 04:08:36.000000 ctwin32-2.2.0/ctwin32/user.py
--rw-rw-rw-   0        0        0     4923 2023-04-11 05:52:35.000000 ctwin32-2.2.0/ctwin32/version.py
--rw-rw-rw-   0        0        0     6877 2023-04-11 05:52:41.000000 ctwin32-2.2.0/ctwin32/virtdisk.py
--rw-rw-rw-   0        0        0    28509 2023-04-11 05:53:33.000000 ctwin32-2.2.0/ctwin32/wndcls.py
--rw-rw-rw-   0        0        0    14247 2023-04-11 15:35:26.000000 ctwin32-2.2.0/ctwin32/wtypes.py
-drwxrwxrwx   0        0        0        0 2023-05-27 04:28:45.086106 ctwin32-2.2.0/ctwin32.egg-info/
--rw-rw-rw-   0        0        0     2575 2023-05-27 04:28:45.000000 ctwin32-2.2.0/ctwin32.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-05-27 04:28:45.000000 ctwin32-2.2.0/ctwin32.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 04:28:45.000000 ctwin32-2.2.0/ctwin32.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-27 04:28:45.000000 ctwin32-2.2.0/ctwin32.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-01-24 05:12:00.000000 ctwin32-2.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-27 04:28:45.108111 ctwin32-2.2.0/samples/
--rw-rw-rw-   0        0        0     2571 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/arp_table.py
--rw-rw-rw-   0        0        0     2529 2023-02-05 05:49:15.000000 ctwin32-2.2.0/samples/atta_vdisk.py
--rw-rw-rw-   0        0        0     3999 2023-01-24 05:13:07.000000 ctwin32-2.2.0/samples/calendar.pyw
--rw-rw-rw-   0        0        0     7327 2023-03-26 04:11:00.000000 ctwin32-2.2.0/samples/dump_ver_res.py
--rw-rw-rw-   0        0        0     2754 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/endis_bsl_usb.py
--rw-rw-rw-   0        0        0     2300 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/exbinmsi.py
--rw-rw-rw-   0        0        0     7490 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/extract_ico.py
--rw-rw-rw-   0        0        0     4738 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/find_zombies.py
--rw-rw-rw-   0        0        0     2026 2023-03-24 04:56:31.000000 ctwin32-2.2.0/samples/fopa.py
--rw-rw-rw-   0        0        0     4124 2023-01-24 05:13:26.000000 ctwin32-2.2.0/samples/hello_wnd.pyw
--rw-rw-rw-   0        0        0     6825 2023-02-05 06:01:54.000000 ctwin32-2.2.0/samples/keyview.pyw
--rw-rw-rw-   0        0        0     1989 2023-02-05 05:42:07.000000 ctwin32-2.2.0/samples/listpipes.py
--rw-rw-rw-   0        0        0     3701 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/logonsessions.py
--rw-rw-rw-   0        0        0     2011 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/netifaces.py
--rw-rw-rw-   0        0        0     2270 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/np_dev.py
--rw-rw-rw-   0        0        0     7698 2023-05-27 03:58:52.000000 ctwin32-2.2.0/samples/power_requests.py
--rw-rw-rw-   0        0        0     5274 2023-04-08 15:36:59.000000 ctwin32-2.2.0/samples/print_reparse_points.py
--rw-rw-rw-   0        0        0     3172 2023-01-24 04:50:54.000000 ctwin32-2.2.0/samples/py_ver.py
--rw-rw-rw-   0        0        0     5164 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/remove_drive_by_letter.py
--rw-rw-rw-   0        0        0     6485 2023-02-05 05:34:26.000000 ctwin32-2.2.0/samples/rm_sign_tool.py
--rw-rw-rw-   0        0        0     5460 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/senv.py
--rw-rw-rw-   0        0        0     4568 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/simple_aes.py
--rw-rw-rw-   0        0        0     3372 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/stopnow.py
--rw-rw-rw-   0        0        0     2253 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/sua_enums.py
--rw-rw-rw-   0        0        0     2703 2023-01-12 03:55:54.000000 ctwin32-2.2.0/samples/test_sign_tool.py
--rw-rw-rw-   0        0        0     2063 2023-04-10 15:30:40.000000 ctwin32-2.2.0/samples/uptime_evt.py
--rw-rw-rw-   0        0        0     2559 2023-01-07 08:47:22.000000 ctwin32-2.2.0/samples/virt_term_seq.py
--rw-rw-rw-   0        0        0       42 2023-05-27 04:28:45.108689 ctwin32-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-04-03 04:37:37.000000 ctwin32-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:34:50.633646 ctwin32-2.3.0/
+-rw-rw-rw-   0        0        0     1057 2023-01-07 08:48:10.000000 ctwin32-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-03-27 05:21:14.000000 ctwin32-2.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2575 2023-07-04 09:34:50.633646 ctwin32-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1651 2023-03-30 05:59:34.000000 ctwin32-2.3.0/README.md
+-rw-rw-rw-   0        0        0     1617 2023-06-12 13:22:22.000000 ctwin32-2.3.0/bld.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:34:50.601637 ctwin32-2.3.0/ctwin32/
+-rw-rw-rw-   0        0        0   223227 2023-07-04 09:28:48.000000 ctwin32-2.3.0/ctwin32/__init__.py
+-rw-rw-rw-   0        0        0    43996 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/advapi.py
+-rw-rw-rw-   0        0        0    17770 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/bcrypt.py
+-rw-rw-rw-   0        0        0     6010 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/cfgmgr.py
+-rw-rw-rw-   0        0        0     9079 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/comctl.py
+-rw-rw-rw-   0        0        0     4352 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/gdi.py
+-rw-rw-rw-   0        0        0    13791 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/iphlpapi.py
+-rw-rw-rw-   0        0        0    47790 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/kernel.py
+-rw-rw-rw-   0        0        0     5951 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/misc.py
+-rw-rw-rw-   0        0        0     5174 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/msi.py
+-rw-rw-rw-   0        0        0    18125 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/ntdll.py
+-rw-rw-rw-   0        0        0     4182 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/psapi.py
+-rw-rw-rw-   0        0        0     6236 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/secur.py
+-rw-rw-rw-   0        0        0    17498 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/setupapi.py
+-rw-rw-rw-   0        0        0     7921 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/shell.py
+-rw-rw-rw-   0        0        0    13158 2023-07-04 09:21:24.000000 ctwin32-2.3.0/ctwin32/svc_util.py
+-rw-rw-rw-   0        0        0    44326 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/user.py
+-rw-rw-rw-   0        0        0     4923 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/version.py
+-rw-rw-rw-   0        0        0     6877 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/virtdisk.py
+-rw-rw-rw-   0        0        0    28509 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/wndcls.py
+-rw-rw-rw-   0        0        0    14486 2023-07-04 08:36:44.000000 ctwin32-2.3.0/ctwin32/wtypes.py
+drwxrwxrwx   0        0        0        0 2023-07-04 09:34:50.605639 ctwin32-2.3.0/ctwin32.egg-info/
+-rw-rw-rw-   0        0        0     2575 2023-07-04 09:34:50.000000 ctwin32-2.3.0/ctwin32.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1273 2023-07-04 09:34:50.000000 ctwin32-2.3.0/ctwin32.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 09:34:50.000000 ctwin32-2.3.0/ctwin32.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-04 09:34:50.000000 ctwin32-2.3.0/ctwin32.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3016 2023-06-25 05:31:57.000000 ctwin32-2.3.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-04 09:34:50.631646 ctwin32-2.3.0/samples/
+-rw-rw-rw-   0        0        0        0 2023-06-10 04:52:20.000000 ctwin32-2.3.0/samples/__init__.py
+-rw-rw-rw-   0        0        0     5739 2023-06-30 11:44:13.000000 ctwin32-2.3.0/samples/api_set.py
+-rw-rw-rw-   0        0        0     2571 2023-06-10 05:14:06.000000 ctwin32-2.3.0/samples/arp_table.py
+-rw-rw-rw-   0        0        0     2527 2023-06-04 06:46:33.000000 ctwin32-2.3.0/samples/atta_vdisk.py
+-rw-rw-rw-   0        0        0     3999 2023-01-24 05:13:07.000000 ctwin32-2.3.0/samples/calendar.pyw
+-rw-rw-rw-   0        0        0     7316 2023-06-04 06:46:51.000000 ctwin32-2.3.0/samples/dump_ver_res.py
+-rw-rw-rw-   0        0        0     2754 2023-01-07 08:47:22.000000 ctwin32-2.3.0/samples/endis_bsl_usb.py
+-rw-rw-rw-   0        0        0     2300 2023-01-07 08:47:22.000000 ctwin32-2.3.0/samples/exbinmsi.py
+-rw-rw-rw-   0        0        0     7490 2023-01-07 08:47:22.000000 ctwin32-2.3.0/samples/extract_ico.py
+-rw-rw-rw-   0        0        0     4712 2023-06-10 05:14:06.000000 ctwin32-2.3.0/samples/find_zombies.py
+-rw-rw-rw-   0        0        0     2026 2023-03-24 04:56:31.000000 ctwin32-2.3.0/samples/fopa.py
+-rw-rw-rw-   0        0        0     4124 2023-06-26 07:18:40.000000 ctwin32-2.3.0/samples/hello_wnd.pyw
+-rw-rw-rw-   0        0        0     6777 2023-06-02 17:14:47.000000 ctwin32-2.3.0/samples/keyview.pyw
+-rw-rw-rw-   0        0        0     1989 2023-02-05 05:42:07.000000 ctwin32-2.3.0/samples/listpipes.py
+-rw-rw-rw-   0        0        0     3700 2023-07-03 06:56:09.000000 ctwin32-2.3.0/samples/logonsessions.py
+-rw-rw-rw-   0        0        0     3222 2023-07-03 19:45:53.000000 ctwin32-2.3.0/samples/lsc.py
+-rw-rw-rw-   0        0        0     1976 2023-06-04 06:47:28.000000 ctwin32-2.3.0/samples/netifaces.py
+-rw-rw-rw-   0        0        0     2270 2023-06-04 06:47:43.000000 ctwin32-2.3.0/samples/np_dev.py
+-rw-rw-rw-   0        0        0     8575 2023-06-10 05:14:06.000000 ctwin32-2.3.0/samples/power_requests.py
+-rw-rw-rw-   0        0        0     5267 2023-06-04 06:48:48.000000 ctwin32-2.3.0/samples/print_reparse_points.py
+-rw-rw-rw-   0        0        0     3172 2023-06-10 05:14:06.000000 ctwin32-2.3.0/samples/py_ver.py
+-rw-rw-rw-   0        0        0     5143 2023-06-10 05:14:06.000000 ctwin32-2.3.0/samples/remove_drive_by_letter.py
+-rw-rw-rw-   0        0        0     4321 2023-06-19 09:55:58.000000 ctwin32-2.3.0/samples/restart_usb_port.py
+-rw-rw-rw-   0        0        0     6485 2023-06-10 05:14:06.000000 ctwin32-2.3.0/samples/rm_sign_tool.py
+-rw-rw-rw-   0        0        0     5460 2023-06-10 05:14:06.000000 ctwin32-2.3.0/samples/senv.py
+-rw-rw-rw-   0        0        0     4569 2023-06-04 06:49:43.000000 ctwin32-2.3.0/samples/simple_aes.py
+-rw-rw-rw-   0        0        0     3373 2023-07-02 08:33:57.000000 ctwin32-2.3.0/samples/stopnow.py
+-rw-rw-rw-   0        0        0     2253 2023-01-07 08:47:22.000000 ctwin32-2.3.0/samples/sua_enums.py
+-rw-rw-rw-   0        0        0     2698 2023-06-04 06:50:10.000000 ctwin32-2.3.0/samples/test_sign_tool.py
+-rw-rw-rw-   0        0        0     2054 2023-06-04 06:50:21.000000 ctwin32-2.3.0/samples/uptime_evt.py
+-rw-rw-rw-   0        0        0     2658 2023-06-10 05:14:06.000000 ctwin32-2.3.0/samples/virt_term_seq.py
+-rw-rw-rw-   0        0        0     4002 2023-06-24 04:11:15.000000 ctwin32-2.3.0/samples/volume_paths.py
+-rw-rw-rw-   0        0        0       42 2023-07-04 09:34:50.633646 ctwin32-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1103 2023-06-10 07:41:06.000000 ctwin32-2.3.0/setup.py
```

### Comparing `ctwin32-2.2.0/LICENSE` & `ctwin32-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/PKG-INFO` & `ctwin32-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctwin32
-Version: 2.2.0
+Version: 2.3.0
 Summary: Access selected win32 APIs through ctypes
 Author: Rocco Matano
 License: MIT License
 Project-URL: homepage, https://github.com/RoccoMatano/ctwin32
 Project-URL: changelog, https://github.com/RoccoMatano/ctwin32/blob/master/changelog.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ctwin32-2.2.0/README.md` & `ctwin32-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/bld.py` & `ctwin32-2.3.0/bld.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 ################################################################################
 
 def initiate_actions():
     # distutils - that setuptools.build_meta is based on - currently do NOT
     # support to execute more than one action per process. Therefore we
     # have to use a child process for every action.
     common = [sys.executable, str(THIS_SCRIPT), "--action"]
-    subprocess.run(common + ["build_sdist"])
+    subprocess.run([*common, "build_sdist"])
     for tag in ("win_amd64", "win32", "win_arm64"):
-        cmd = common + ["build_wheel", "--build-option", f"-p {tag}"]
+        cmd = [*common, "build_wheel", "--build-option", f"-p {tag}"]
         subprocess.run(cmd)
 
 ################################################################################
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(add_help=False)
     parser.add_argument("--action")
```

### Comparing `ctwin32-2.2.0/ctwin32/__init__.py` & `ctwin32-2.3.0/ctwin32/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     UINT,
     WCHAR,
     )
 ref = ctypes.byref
 
 ################################################################################
 
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 
 ################################################################################
 
 def raise_if(condition):
     if condition:
         raise ctypes.WinError()
 
@@ -85,31 +85,44 @@
 def fun_fact(function, signature):
     function.restype = signature[0]
     function.argtypes = signature[1:]
     return function
 
 ################################################################################
 
+def multi_str_from_str(_str):
+    _str = _str.rstrip("\0")
+    return [] if not _str else _str.split("\0")
+
+################################################################################
+
 def multi_str_from_addr(addr):
     WCHAR_SIZE = ctypes.sizeof(WCHAR)
     end = addr
     while True:
         if slen := len(ctypes.cast(end, PWSTR).value):
             end += (slen + 1) * WCHAR_SIZE
         else:
             # +WCHAR_SIZE for final null
             size = (end + WCHAR_SIZE - addr) // WCHAR_SIZE
-            return ctypes.wstring_at(addr, size)
+            return multi_str_from_str(ctypes.wstring_at(addr, size))
+
+################################################################################
+
+def multi_str_from_ubuf(buf, size=-1):
+    if size >= 0:
+        return multi_str_from_str(buf[:size])
+    return multi_str_from_addr(ctypes.addressof(buf))
 
 ################################################################################
 
 def cmdline_from_args(args):
     BS = "\\"
     parts = []
-    for arg in args:
+    for arg in map(str, args):
         bs_accu = []
         if parts:
             parts.append(" ")
         if need_qmark := (" " in arg) or ("\t" in arg) or not arg:
             parts.append('"')
         for c in arg:
             if c == BS:
@@ -170,14 +183,19 @@
             )
         warnings.warn(msg, stacklevel=3)
 
 _warn_win_ver()
 
 ################################################################################
 
+def CTL_CODE(dev_type, func, method, access):
+    return (dev_type << 16) | (access << 14) | (func << 2) | method
+
+################################################################################
+
 INVALID_HANDLE_VALUE = HANDLE(-1).value
 HGDI_ERROR = INVALID_HANDLE_VALUE
 
 DBT_CONFIGCHANGECANCELED = 25
 DBT_CONFIGCHANGED = 24
 DBT_CUSTOMEVENT = 32774
 DBT_DEVICEARRIVAL = 32768
@@ -643,14 +661,34 @@
 TokenAccessInformation = 22
 TokenVirtualizationAllowed = 23
 TokenVirtualizationEnabled = 24
 TokenIntegrityLevel = 25
 TokenUIAccess = 26
 TokenMandatoryPolicy = 27
 TokenLogonSid = 28
+TokenIsAppContainer = 29
+TokenCapabilities = 30
+TokenAppContainerSid = 31
+TokenAppContainerNumber = 32
+TokenUserClaimAttributes = 33
+TokenDeviceClaimAttributes = 34
+TokenRestrictedUserClaimAttributes = 35
+TokenRestrictedDeviceClaimAttributes = 36
+TokenDeviceGroups = 37
+TokenRestrictedDeviceGroups = 38
+TokenSecurityAttributes = 39
+TokenIsRestricted = 40
+TokenProcessTrustLevel = 41
+TokenPrivateNameSpace = 42
+TokenSingletonAttributes = 43
+TokenBnoIsolation = 44
+TokenChildProcessFlags = 45
+TokenIsLessPrivilegedAppContainer = 46
+TokenIsSandboxed = 47
+TokenOriginatingProcessTrustLevel = 48
 
 WAIT_FAILED = 0xFFFFFFFF
 WAIT_OBJECT_0 = 0
 WAIT_ABANDONED = 0x00000080
 WAIT_ABANDONED_0 = WAIT_ABANDONED
 WAIT_TIMEOUT = 258
 WAIT_IO_COMPLETION = 0x000000C0
@@ -4055,28 +4093,14 @@
 FLASHW_STOP = 0
 FLASHW_CAPTION = 1
 FLASHW_TRAY = 2
 FLASHW_ALL = FLASHW_CAPTION | FLASHW_TRAY
 FLASHW_TIMER = 4
 FLASHW_TIMERNOFG = 12
 
-DS_ABSALIGN = 1
-DS_SYSMODAL = 2
-DS_LOCALEDIT = 32
-DS_SETFONT = 64
-DS_MODALFRAME = 128
-DS_NOIDLEMSG = 256
-DS_SETFOREGROUND = 512
-DS_3DLOOK = 4
-DS_FIXEDSYS = 8
-DS_NOFAILCREATE = 16
-DS_CONTROL = 1024
-DS_CENTER = 2048
-DS_CENTERMOUSE = 4096
-DS_CONTEXTHELP = 8192
 DM_GETDEFID = WM_USER + 0
 DM_SETDEFID = WM_USER + 1
 DM_REPOSITION = WM_USER + 2
 DC_HASDEFID = 21323
 DLGC_WANTARROWS = 1
 DLGC_WANTTAB = 2
 DLGC_WANTALLKEYS = 4
@@ -6923,14 +6947,18 @@
 CR_INVALID_INDEX = 0x0000003A
 CR_INVALID_STRUCTURE_SIZE = 0x0000003B
 NUM_CR_RESULTS = 0x0000003C
 
 CM_ENUMERATE_CLASSES_INSTALLER = 0x00000000
 CM_ENUMERATE_CLASSES_INTERFACE = 0x00000001
 CM_ENUMERATE_CLASSES_BITS = 0x00000001
+CM_LOCATE_DEVNODE_NORMAL =0x00000000
+CM_LOCATE_DEVNODE_PHANTOM = 0x00000001
+CM_LOCATE_DEVNODE_CANCELREMOVE = 0x00000002
+CM_LOCATE_DEVNODE_NOVALIDATION = 0x00000004
 
 SPDRP_DEVICEDESC = 0x00000000  # DeviceDesc (R/W)
 SPDRP_HARDWAREID = 0x00000001  # HardwareID (R/W)
 SPDRP_COMPATIBLEIDS = 0x00000002  # CompatibleIDs (R/W)
 SPDRP_UNUSED0 = 0x00000003  # unused
 SPDRP_SERVICE = 0x00000004  # Service (R/W)
 SPDRP_UNUSED1 = 0x00000005  # unused
@@ -7326,14 +7354,23 @@
 FILE_DEVICE_UCMTCPCI = 0x00000058
 FILE_DEVICE_PERSISTENT_MEMORY = 0x00000059
 FILE_DEVICE_NVDIMM = 0x0000005A
 FILE_DEVICE_HOLOGRAPHIC = 0x0000005B
 FILE_DEVICE_SDFXHCI = 0x0000005C
 FILE_DEVICE_UCMUCSI = 0x0000005D
 
+METHOD_BUFFERED = 0
+METHOD_IN_DIRECT = 1
+METHOD_OUT_DIRECT = 2
+METHOD_NEITHER = 3
+FILE_ANY_ACCESS = 0
+FILE_SPECIAL_ACCESS = FILE_ANY_ACCESS
+FILE_READ_ACCESS = 1
+FILE_WRITE_ACCESS = 2
+
 MONITOR_DEFAULTTONULL = 0x00000000
 MONITOR_DEFAULTTOPRIMARY = 0x00000001
 MONITOR_DEFAULTTONEAREST = 0x00000002
 
 IDC_ARROW = 32512
 IDC_IBEAM = 32513
 IDC_WAIT = 32514
@@ -7744,43 +7781,14 @@
 SS_SUNKEN = 0x00001000
 SS_EDITCONTROL = 0x00002000
 SS_ENDELLIPSIS = 0x00004000
 SS_PATHELLIPSIS = 0x00008000
 SS_WORDELLIPSIS = 0x0000C000
 SS_ELLIPSISMASK = 0x0000C000
 
-BS_PUSHBUTTON = 0x00000000
-BS_DEFPUSHBUTTON = 0x00000001
-BS_CHECKBOX = 0x00000002
-BS_AUTOCHECKBOX = 0x00000003
-BS_RADIOBUTTON = 0x00000004
-BS_3STATE = 0x00000005
-BS_AUTO3STATE = 0x00000006
-BS_GROUPBOX = 0x00000007
-BS_USERBUTTON = 0x00000008
-BS_AUTORADIOBUTTON = 0x00000009
-BS_PUSHBOX = 0x0000000A
-BS_OWNERDRAW = 0x0000000B
-BS_TYPEMASK = 0x0000000F
-BS_LEFTTEXT = 0x00000020
-BS_TEXT = 0x00000000
-BS_ICON = 0x00000040
-BS_BITMAP = 0x00000080
-BS_LEFT = 0x00000100
-BS_RIGHT = 0x00000200
-BS_CENTER = 0x00000300
-BS_TOP = 0x00000400
-BS_BOTTOM = 0x00000800
-BS_VCENTER = 0x00000C00
-BS_PUSHLIKE = 0x00001000
-BS_MULTILINE = 0x00002000
-BS_NOTIFY = 0x00004000
-BS_FLAT = 0x00008000
-BS_RIGHTBUTTON = BS_LEFTTEXT
-
 DS_ABSALIGN = 0x01
 DS_SYSMODAL = 0x02
 DS_LOCALEDIT = 0x20
 DS_SETFONT = 0x40
 DS_MODALFRAME = 0x80
 DS_NOIDLEMSG = 0x100
 DS_SETFOREGROUND = 0x200
@@ -7793,20 +7801,14 @@
 DS_CONTEXTHELP = 0x2000
 DS_SHELLFONT = (DS_SETFONT | DS_FIXEDSYS)
 
 STD_INPUT_HANDLE = DWORD(-10).value
 STD_OUTPUT_HANDLE = DWORD(-11).value
 STD_ERROR_HANDLE = DWORD(-12).value
 
-FILE_TYPE_UNKNOWN = 0x0000
-FILE_TYPE_DISK = 0x0001
-FILE_TYPE_CHAR = 0x0002
-FILE_TYPE_PIPE = 0x0003
-FILE_TYPE_REMOTE = 0x8000
-
 ENABLE_PROCESSED_INPUT = 0x0001
 ENABLE_LINE_INPUT = 0x0002
 ENABLE_ECHO_INPUT = 0x0004
 ENABLE_WINDOW_INPUT = 0x0008
 ENABLE_MOUSE_INPUT = 0x0010
 ENABLE_INSERT_MODE = 0x0020
 ENABLE_QUICK_EDIT_MODE = 0x0040
```

### Comparing `ctwin32-2.2.0/ctwin32/advapi.py` & `ctwin32-2.3.0/ctwin32/advapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     BOOL,
     BYTE,
     DWORD,
     ENDIANNESS,
     FILETIME,
     HANDLE,
     INT,
+    LARGE_INTEGER,
     LONG,
     LUID,
     PBOOL,
     PBYTE,
     PDWORD,
     PFILETIME,
     PHANDLE,
@@ -56,14 +57,15 @@
     raise_if,
     raise_on_zero,
     raise_on_err,
     suppress_winerr,
     fun_fact,
     ns_from_struct,
     argc_argv_from_args,
+    cmdline_from_args,
     REG_DWORD,
     REG_QWORD,
     REG_SZ,
     REG_EXPAND_SZ,
     REG_MULTI_SZ,
     KEY_READ,
     KEY_ALL_ACCESS,
@@ -78,15 +80,24 @@
     ERROR_NO_MORE_ITEMS,
     ERROR_HANDLE_EOF,
     ERROR_INSUFFICIENT_BUFFER,
     CRED_TYPE_GENERIC,
     EVENTLOG_SEQUENTIAL_READ,
     EVENTLOG_BACKWARDS_READ,
     )
-from .kernel import LocalFree, GetLastError, KHANDLE
+from .kernel import (
+    LocalFree,
+    GetLastError,
+    KHANDLE,
+    PSECURITY_ATTRIBUTES,
+    PSTARTUPINFO,
+    PPROCESS_INFORMATION,
+    PROCESS_INFORMATION,
+    STARTUPINFO,
+    )
 
 _adv = ctypes.WinDLL("advapi32.dll")
 
 ################################################################################
 
 # values of predefined keys
 
@@ -382,15 +393,15 @@
             break
         elif err == ERROR_MORE_DATA:
             vlen = DWORD(vlen.value * 2)
             value = ctypes.create_string_buffer(vlen.value)
         else:
             raise ctypes.WinError(err)
 
-    return (name.value,) + registry_to_py(typ.value, value.raw[:vlen.value])
+    return (name.value, *registry_to_py(typ.value, value.raw[:vlen.value]))
 
 ################################################################################
 
 def reg_enum_values(key):
     index = 0
     with suppress_winerr(ERROR_NO_MORE_ITEMS):
         while True:
@@ -600,14 +611,145 @@
 def OpenProcessToken(proc_handle, desired_acc):
     token = KHANDLE()
     raise_on_zero(_OpenProcessToken(proc_handle, desired_acc, ref(token)))
     return token
 
 ################################################################################
 
+_DuplicateTokenEx = fun_fact(
+    _adv.DuplicateTokenEx,
+    (BOOL, HANDLE, DWORD, PSECURITY_ATTRIBUTES, INT, INT, PHANDLE)
+    )
+
+def DuplicateTokenEx(tok, acc, sattr, imp, typ):
+    dup = KHANDLE()
+    raise_on_zero(_DuplicateTokenEx(tok, acc, ref(sattr), imp, typ, ref(dup)))
+    return dup
+
+################################################################################
+
+class TOKEN_STATISTICS(ctypes.Structure):
+    _fields_ = (
+        ("TokenId", LUID),
+        ("AuthenticationId", LUID),
+        ("ExpirationTime", LARGE_INTEGER),
+        ("TokenType", INT),
+        ("ImpersonationLevel", INT),
+        ("DynamicCharged", DWORD),
+        ("DynamicAvailable", DWORD),
+        ("GroupCount", DWORD),
+        ("PrivilegeCount", DWORD),
+        ("ModifiedId", LUID),
+        )
+
+################################################################################
+_GetTokenInformation = fun_fact(
+    _adv.GetTokenInformation, (BOOL, HANDLE, INT, PVOID, DWORD, PDWORD)
+    )
+
+def GetTokenInformation(hdl, cls):
+    rlen = DWORD(256)
+    while True:
+        size = rlen.value
+        buf = ctypes.create_string_buffer(size)
+        if _GetTokenInformation(hdl, cls, buf, size, ref(rlen)):
+            return buf.raw[:rlen.value]
+        elif (err := GetLastError()) != ERROR_INSUFFICIENT_BUFFER:
+            raise ctypes.WinError(err)
+
+################################################################################
+
+_SetTokenInformation = fun_fact(
+    _adv.SetTokenInformation, (BOOL, HANDLE, INT, PVOID, DWORD)
+    )
+
+def SetTokenInformation(hdl, cls, info):
+    raise_on_zero(
+        _SetTokenInformation(hdl, cls, ref(info), ctypes.sizeof(info))
+        )
+
+################################################################################
+
+_CreateProcessAsUser = fun_fact(
+    _adv.CreateProcessAsUserW, (
+        BOOL,
+        HANDLE,
+        PWSTR,
+        PWSTR,
+        PSECURITY_ATTRIBUTES,
+        PSECURITY_ATTRIBUTES,
+        BOOL,
+        DWORD,
+        PVOID,
+        PWSTR,
+        PSTARTUPINFO,
+        PPROCESS_INFORMATION,
+        )
+    )
+
+def CreateProcessAsUser(
+        token,
+        app_name,
+        cmd_line,
+        proc_attr,
+        thread_attr,
+        inherit,
+        cflags,
+        env,
+        curdir,
+        startup_info
+        ):
+    proc_info = PROCESS_INFORMATION()
+    raise_on_zero(
+        _CreateProcessAsUser(
+            token,
+            app_name,
+            cmd_line,
+            ref(proc_attr) if proc_attr is not None else None,
+            ref(thread_attr) if thread_attr is not None else None,
+            inherit,
+            cflags,
+            env,
+            curdir,
+            ref(startup_info),
+            ref(proc_info)
+            )
+        )
+    return proc_info
+
+################################################################################
+
+def create_process_as_user(
+        token,
+        arglist,
+        cflags=0,
+        startup_info=None,
+        inherit=False,
+        env=None,
+        curdir=None,
+        proc_attr=None,
+        thread_attr=None,
+        ):
+    if startup_info is None:
+        startup_info = STARTUPINFO()
+    return CreateProcessAsUser(
+        token,
+        None,
+        cmdline_from_args(arglist),
+        proc_attr,
+        thread_attr,
+        inherit,
+        cflags,
+        env,
+        curdir,
+        startup_info
+        )
+
+################################################################################
+
 _LookupPrivilegeValue = fun_fact(
     _adv.LookupPrivilegeValueW, (BOOL, PWSTR, PWSTR, PLUID)
     )
 
 def LookupPrivilegeValue(sys_name, name):
     luid = LUID()
     raise_on_zero(_LookupPrivilegeValue(sys_name, name, ref(luid)))
@@ -1003,21 +1145,21 @@
     argc, argv, _ = argc_argv_from_args(arglist)
     raise_on_zero(_StartService(handle, argc, argv))
 
 ################################################################################
 
 class SERVICE_STATUS(ctypes.Structure):
     _fields_ = (
-        ("ServiceType", DWORD),
-        ("CurrentState", DWORD),
-        ("ControlsAccepted", DWORD),
-        ("Win32ExitCode", DWORD),
-        ("ServiceSpecificExitCode", DWORD),
-        ("CheckPoint", DWORD),
-        ("WaitHint", DWORD),
+        ("dwServiceType", DWORD),
+        ("dwCurrentState", DWORD),
+        ("dwControlsAccepted", DWORD),
+        ("dwWin32ExitCode", DWORD),
+        ("dwServiceSpecificExitCode", DWORD),
+        ("dwCheckPoint", DWORD),
+        ("dwWaitHint", DWORD),
         )
 PSERVICE_STATUS = POINTER(SERVICE_STATUS)
 
 _ControlService = fun_fact(
     _adv.ControlService, (
         BOOL,
         HANDLE,
@@ -1038,23 +1180,23 @@
 def DeleteService(service):
     raise_on_zero(_DeleteService(service))
 
 ################################################################################
 
 class SERVICE_STATUS_PROCESS(ctypes.Structure):
     _fields_ = (
-        ("ServiceType", DWORD),
-        ("CurrentState", DWORD),
-        ("ControlsAccepted", DWORD),
-        ("Win32ExitCode", DWORD),
-        ("ServiceSpecificExitCode", DWORD),
-        ("CheckPoint", DWORD),
-        ("WaitHint", DWORD),
-        ("ProcessId", DWORD),
-        ("ServiceFlags", DWORD),
+        ("dwServiceType", DWORD),
+        ("dwCurrentState", DWORD),
+        ("dwControlsAccepted", DWORD),
+        ("dwWin32ExitCode", DWORD),
+        ("dwServiceSpecificExitCode", DWORD),
+        ("dwCheckPoint", DWORD),
+        ("dwWaitHint", DWORD),
+        ("dwProcessId", DWORD),
+        ("dwServiceFlags", DWORD),
         )
 
 _QueryServiceStatusEx = fun_fact(
     _adv.QueryServiceStatusEx, (
         BOOL,
         HANDLE,
         INT,
@@ -1078,16 +1220,16 @@
         )
     return status
 
 ################################################################################
 
 class ENUM_SERVICE_STATUS_PROCESS(ctypes.Structure):
     _fields_ = (
-        ("ServiceName", PWSTR),
-        ("DisplayName", PWSTR),
+        ("lpServiceName", PWSTR),
+        ("lpDisplayName", PWSTR),
         ("ServiceStatusProcess", SERVICE_STATUS_PROCESS),
         )
 
 _EnumServicesStatusEx = fun_fact(
     _adv.EnumServicesStatusExW, (
         BOOL,
         HANDLE,
@@ -1142,23 +1284,23 @@
 
     return res
 
 ################################################################################
 
 class QUERY_SERVICE_CONFIG(ctypes.Structure):
     _fields_ = (
-        ("ServiceType", DWORD),
-        ("StartType", DWORD),
-        ("ErrorControl", DWORD),
-        ("BinaryPathName", DWORD),
-        ("LoadOrderGroup", DWORD),
-        ("TagId", DWORD),
-        ("Dependencies", DWORD),
-        ("ServiceStartName", DWORD),
-        ("DisplayName", DWORD),
+        ("dwServiceType", DWORD),
+        ("dwStartType", DWORD),
+        ("dwErrorControl", DWORD),
+        ("lpBinaryPathName", PWSTR),
+        ("lpLoadOrderGroup", PWSTR),
+        ("dwTagId", DWORD),
+        ("lpDependencies", PWSTR),
+        ("lpServiceStartName", PWSTR),
+        ("lpDisplayName", PWSTR),
         )
 PQUERY_SERVICE_CONFIG = POINTER(QUERY_SERVICE_CONFIG)
 
 _QueryServiceConfig = fun_fact(
     _adv.QueryServiceConfigW, (
         BOOL,
         HANDLE,
@@ -1179,14 +1321,54 @@
     buf = ctypes.create_string_buffer(needed.value)
     pqsc = ctypes.cast(buf, PQUERY_SERVICE_CONFIG)
     raise_on_zero(_QueryServiceConfig(svc, pqsc, needed.value, ref(needed)))
     return ns_from_struct(pqsc.contents)
 
 ################################################################################
 
+SERVICE_MAIN_FUNCTION = ctypes.WINFUNCTYPE(None, DWORD, PPWSTR)
+
+class SERVICE_TABLE_ENTRY(ctypes.Structure):
+    _fields_ = (
+        ("lpServiceName", PWSTR),
+        ("lpServiceProc", SERVICE_MAIN_FUNCTION),
+        )
+PSERVICE_TABLE_ENTRY = POINTER(SERVICE_TABLE_ENTRY)
+
+_StartServiceCtrlDispatcher = fun_fact(
+    _adv.StartServiceCtrlDispatcherW, (BOOL, PSERVICE_TABLE_ENTRY)
+    )
+
+def StartServiceCtrlDispatcher(table):
+    raise_on_zero(_StartServiceCtrlDispatcher(ref(table[0])))
+
+################################################################################
+
+HANDLER_FUNCTION = ctypes.WINFUNCTYPE(None, DWORD)
+
+_RegisterServiceCtrlHandler = fun_fact(
+    _adv.RegisterServiceCtrlHandlerW, (HANDLE, PWSTR, HANDLER_FUNCTION)
+    )
+
+def RegisterServiceCtrlHandler(name, handler):
+    res = _RegisterServiceCtrlHandler(name, handler)
+    raise_on_zero(res)
+    return res
+
+################################################################################
+
+_SetServiceStatus = fun_fact(
+    _adv.SetServiceStatus, (BOOL, HANDLE, PSERVICE_STATUS)
+    )
+
+def SetServiceStatus(hdl, status):
+    raise_on_zero(_SetServiceStatus(hdl, ref(status)))
+
+################################################################################
+
 class CREDENTIAL_ATTRIBUTE(ctypes.Structure):
     _fields_ = (
         ("Keyword", PWSTR),
         ("Flags", DWORD),
         ("ValueSize", DWORD),
         ("Value", PBYTE),
         )
```

### Comparing `ctwin32-2.2.0/ctwin32/bcrypt.py` & `ctwin32-2.3.0/ctwin32/bcrypt.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/ctwin32/cfgmgr.py` & `ctwin32-2.3.0/ctwin32/cfgmgr.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,27 +26,30 @@
 from .wtypes import (
     DWORD,
     GUID,
     INT,
     PDWORD,
     PGUID,
     PINT,
+    PVOID,
     PWSTR,
     PULONG,
     ULONG,
     )
 from . import (
     ref,
     fun_fact,
     MAX_DEVICE_ID_LEN,
     MAX_PATH,
+    CM_LOCATE_DEVNODE_NORMAL,
     CR_SUCCESS,
     ERROR_FLOPPY_UNKNOWN_ERROR,
     ERROR_CURRENT_DIRECTORY,
     )
+from .advapi import registry_to_py
 _cfg = ctypes.WinDLL("cfgmgr32.dll")
 
 ################################################################################
 
 CM_MapCrToWin32Err = fun_fact(_cfg.CM_MapCrToWin32Err, (DWORD, DWORD, DWORD))
 
 def raise_on_cr(cfgret):
@@ -142,7 +145,56 @@
         vv = veto_type.value
         vn = veto_name.value
         def_err = ERROR_CURRENT_DIRECTORY
         err = CM_MapCrToWin32Err(err, def_err) or def_err
         raise OSError(err, f"device removal was vetoed ({vv}): {vn}")
 
 ################################################################################
+
+_CM_Locate_DevNode = fun_fact(
+    _cfg.CM_Locate_DevNodeW, (DWORD, PDWORD, PWSTR, ULONG)
+    )
+
+def CM_Locate_DevNode(device_id, flags=CM_LOCATE_DEVNODE_NORMAL):
+    devinst = DWORD()
+    raise_on_cr(_CM_Locate_DevNode(ref(devinst), device_id, flags))
+    return devinst.value
+
+################################################################################
+
+_CM_Get_DevNode_Registry_Property = fun_fact(
+    _cfg.CM_Get_DevNode_Registry_PropertyW, (
+        DWORD,
+        DWORD,
+        ULONG,
+        PULONG,
+        PVOID,
+        PULONG,
+        ULONG
+        )
+    )
+
+def CM_Get_DevNode_Registry_Property(devinst, prop):
+    reg_type = DWORD()
+    req_size = DWORD()
+    _CM_Get_DevNode_Registry_Property(
+        devinst,
+        prop,
+        ref(reg_type),
+        None,
+        ref(req_size),
+        0
+        )
+    buf = ctypes.create_string_buffer(req_size.value)
+    raise_on_cr(
+        _CM_Get_DevNode_Registry_Property(
+            devinst,
+            prop,
+            ref(reg_type),
+            buf,
+            ref(req_size),
+            0
+            )
+        )
+    return registry_to_py(reg_type.value, buf.raw[:req_size.value])
+
+################################################################################
```

### Comparing `ctwin32-2.2.0/ctwin32/comctl.py` & `ctwin32-2.3.0/ctwin32/comctl.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/ctwin32/gdi.py` & `ctwin32-2.3.0/ctwin32/gdi.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/ctwin32/iphlpapi.py` & `ctwin32-2.3.0/ctwin32/iphlpapi.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/ctwin32/kernel.py` & `ctwin32-2.3.0/ctwin32/kernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 #
 ################################################################################
 
 import collections as _collections
+from enum import IntEnum as _int_enum
 
 import ctypes
 from .wtypes import (
     BOOL,
     BYTE,
     CallbackContext,
     CallbackContextPtr,
@@ -34,14 +35,15 @@
     FILETIME,
     HANDLE,
     INT,
     PBOOL,
     PBYTE,
     PDWORD,
     POINTER,
+    PPWSTR,
     PSIZE_T,
     PULONG_PTR,
     PUSHORT,
     PVOID,
     PWIN32_FIND_DATA,
     PWSTR,
     ScdToBeClosed,
@@ -54,46 +56,49 @@
     ULONG_PTR,
     USHORT,
     WCHAR,
     WIN32_FIND_DATA,
     WORD,
     )
 from . import (
-    ref,
+    cmdline_from_args,
+    fun_fact,
+    multi_str_from_addr,
+    multi_str_from_ubuf,
+    ns_from_struct,
     raise_if,
+    raise_on_err,
     raise_on_zero,
-    fun_fact,
+    ref,
+    ENABLE_VIRTUAL_TERMINAL_PROCESSING,
     ERROR_ACCESS_DENIED,
     ERROR_FILE_NOT_FOUND,
     ERROR_INSUFFICIENT_BUFFER,
+    ERROR_MORE_DATA,
     ERROR_NO_MORE_FILES,
     ERROR_RESOURCE_ENUM_USER_STOP,
     ERROR_RESOURCE_NAME_NOT_FOUND,
     ERROR_SUCCESS,
+    GENERIC_READ,
+    GENERIC_WRITE,
     FILE_ATTRIBUTE_DIRECTORY,
+    FILE_ATTRIBUTE_NORMAL,
+    FILE_SHARE_READ,
+    FILE_SHARE_WRITE,
     FILE_TYPE_CHAR,
     FILE_TYPE_UNKNOWN,
     INVALID_FILE_ATTRIBUTES,
     INVALID_HANDLE_VALUE,
     IMAGE_FILE_MACHINE_UNKNOWN,
     IMAGE_FILE_MACHINE_AMD64,
     IMAGE_FILE_MACHINE_I386,
+    OPEN_EXISTING,
     RT_MESSAGETABLE,
     STD_OUTPUT_HANDLE,
     WAIT_FAILED,
-    ENABLE_VIRTUAL_TERMINAL_PROCESSING,
-    GENERIC_READ,
-    GENERIC_WRITE,
-    FILE_SHARE_READ,
-    FILE_SHARE_WRITE,
-    FILE_ATTRIBUTE_NORMAL,
-    OPEN_EXISTING,
-    multi_str_from_addr,
-    cmdline_from_args,
-    ns_from_struct,
     )
 
 _k32 = ctypes.WinDLL("kernel32.dll")
 
 ################################################################################
 
 ExitProcess = fun_fact(_k32.ExitProcess, (None, UINT))
@@ -133,15 +138,20 @@
 def GlobalLock(hmem):
     res = _GlobalLock(hmem)
     raise_on_zero(res)
     return res
 
 ################################################################################
 
-GlobalUnlock = fun_fact(_k32.GlobalUnlock, (PVOID, HANDLE))
+_GlobalUnlock = fun_fact(_k32.GlobalUnlock, (BOOL, HANDLE))
+
+def GlobalUnlock(hmem):
+    res = _GlobalUnlock(hmem)
+    if not res and (err := GetLastError()) != ERROR_SUCCESS:
+        raise ctypes.WinError(err)
 
 ################################################################################
 
 _CloseHandle = fun_fact(_k32.CloseHandle, (BOOL, HANDLE))
 
 def CloseHandle(handle):
     raise_on_zero(_CloseHandle(handle))
@@ -391,14 +401,16 @@
     )
 
 def QueryDosDevice(device_name):
     size = 512
     buf = ctypes.create_unicode_buffer(size)
     while True:
         if res := _QueryDosDevice(device_name, buf, size):
+            if device_name is None:
+                return multi_str_from_ubuf(buf, res)
             return buf.value[:res]
         raise_if(GetLastError() != ERROR_INSUFFICIENT_BUFFER)
         size *= 2
         buf = ctypes.create_unicode_buffer(size)
 
 ################################################################################
 
@@ -505,14 +517,19 @@
 _OutputDebugStringW = fun_fact(_k32.OutputDebugStringW, (None, PWSTR))
 
 def OutputDebugString(dstr):
     _OutputDebugStringW(dstr)
 
 ################################################################################
 
+def dbg_print(*args, end="\n"):
+    _OutputDebugStringW(f"{' '.join(map(str, args))}{end}")
+
+################################################################################
+
 _SetThreadExecutionState = fun_fact(
     _k32.SetThreadExecutionState, (DWORD, DWORD)
     )
 
 def SetThreadExecutionState(es_flags):
     return _SetThreadExecutionState(es_flags)
 
@@ -527,15 +544,15 @@
     size = 512
     buf = ctypes.create_unicode_buffer(size)
     res = _GetPrivateProfileSectionNames(buf, size, filename)
     while res == size - 2:
         size *= 2
         buf = ctypes.create_unicode_buffer(size)
         res = _GetPrivateProfileSectionNames(buf, size, filename)
-    return buf[:res].split("\0")[:-1]
+    return multi_str_from_ubuf(buf, res)
 
 ################################################################################
 
 _GetPrivateProfileSection = fun_fact(
     _k32.GetPrivateProfileSectionW,
     (DWORD, PWSTR, PWSTR, DWORD, PWSTR)
     )
@@ -544,15 +561,15 @@
     size = 512
     buf = ctypes.create_unicode_buffer(size)
     res = _GetPrivateProfileSection(secname, buf, size, filename)
     while res == size - 2:
         size *= 2
         buf = ctypes.create_unicode_buffer(size)
         res = _GetPrivateProfileSection(secname, buf, size, filename)
-    entries = buf[:res].split("\0")[:-1]
+    entries = multi_str_from_ubuf(buf, res)
     d = _collections.OrderedDict()
     for e in entries:
         k, v = e.split("=", 1)
         d[k] = v
     return d
 
 ################################################################################
@@ -625,15 +642,15 @@
     raise_on_zero(ptr)
     try:
         return multi_str_from_addr(ptr)
     finally:
         raise_on_zero(_FreeEnvironmentStrings(ptr))
 
 def env_str_to_dict(estr):
-    return dict(s.split("=", 1) for s in estr.strip("\0").split("\0"))
+    return dict(s.split("=", 1) for s in estr)
 
 def get_env_as_dict():
     return env_str_to_dict(GetEnvironmentStrings())
 
 ################################################################################
 
 _SetEnvironmentStrings = fun_fact(
@@ -1451,7 +1468,163 @@
 
 def find_file(name):
     hdl, info = FindFirstFile(name)
     hdl.close()
     return info
 
 ################################################################################
+
+class PowerRequest(_int_enum):
+    DisplayRequired = 0
+    SystemRequired = 1
+    AwayModeRequired = 2
+    ExecutionRequired = 3
+    Inactive = -1
+
+    @classmethod
+    def from_param(cls, obj):
+        return int(cls(obj))
+
+# values for REASON_CONTEXT.Version and REASON_CONTEXT.Flags
+POWER_REQUEST_CONTEXT_VERSION = 0
+POWER_REQUEST_CONTEXT_SIMPLE_STRING = 1
+POWER_REQUEST_CONTEXT_DETAILED_STRING = 2
+
+class REASON_CONTEXT_DETAILED(ctypes.Structure):
+    _fields_ = (
+        ("LocalizedReasonModule", HMODULE),
+        ("LocalizedReasonId", ULONG),
+        ("ReasonStringCount", ULONG),
+        ("ReasonStrings", PPWSTR),
+        )
+
+class REASON_CONTEXT_UNION(ctypes.Union):
+    _fields_ = (
+        ("Detailed", REASON_CONTEXT_DETAILED),
+        ("SimpleReasonString", PWSTR),
+        )
+
+class REASON_CONTEXT(ctypes.Structure):
+    _fields_ = (
+        ("Version", ULONG),
+        ("Flags", DWORD),
+        ("Reason", REASON_CONTEXT_UNION)
+        )
+
+    def __init__(self, reason_str=""):
+        self.Version = POWER_REQUEST_CONTEXT_VERSION
+        self.Flags = POWER_REQUEST_CONTEXT_SIMPLE_STRING
+        self.Reason = REASON_CONTEXT_UNION(SimpleReasonString=reason_str)
+
+PREASON_CONTEXT = POINTER(REASON_CONTEXT)
+
+################################################################################
+
+_PowerCreateRequest = fun_fact(
+    _k32.PowerCreateRequest, (HANDLE, PREASON_CONTEXT)
+    )
+
+def PowerCreateRequest(reason):
+    hdl = FHANDLE(_PowerCreateRequest(ref(reason)))
+    hdl.raise_on_invalid()
+    return hdl
+
+################################################################################
+
+_PowerSetRequest = fun_fact(_k32.PowerSetRequest, (BOOL, HANDLE, PowerRequest))
+
+def PowerSetRequest(hdl, pwr_request):
+    raise_on_zero(_PowerSetRequest(hdl, pwr_request))
+
+################################################################################
+
+_PowerClearRequest = fun_fact(
+    _k32.PowerClearRequest, (BOOL, HANDLE, PowerRequest)
+    )
+
+def PowerClearRequest(hdl, pwr_request):
+    raise_on_zero(_PowerClearRequest(hdl, pwr_request))
+
+################################################################################
+
+def create_power_request(reason_str, pwr_request=PowerRequest.Inactive):
+    hdl = PowerCreateRequest(REASON_CONTEXT(reason_str))
+    if pwr_request != PowerRequest.Inactive:
+        PowerSetRequest(hdl, pwr_request)
+    return hdl
+
+################################################################################
+
+GetDriveType = fun_fact(_k32.GetDriveTypeW, (UINT, PWSTR))
+
+################################################################################
+
+_GetLogicalDriveStrings = fun_fact(
+    _k32.GetLogicalDriveStringsW, (DWORD, DWORD, PWSTR)
+    )
+
+def GetLogicalDriveStrings():
+    size = 256
+    buf = ctypes.create_unicode_buffer(size)
+    raise_on_zero(res := _GetLogicalDriveStrings(size, buf))
+    return multi_str_from_ubuf(buf, res)
+
+################################################################################
+
+_FindFirstVolume = fun_fact(_k32.FindFirstVolumeW, (HANDLE, PWSTR, DWORD))
+
+def FindFirstVolume():
+    size = 256
+    buf = ctypes.create_unicode_buffer(size)
+    hdl = _FindFirstVolume(buf, size)
+    raise_if(hdl == INVALID_HANDLE_VALUE)
+    return hdl, buf.value
+
+################################################################################
+
+_FindNextVolume = fun_fact(_k32.FindNextVolumeW, (BOOL, HANDLE, PWSTR, DWORD))
+
+def FindNextVolume(hdl):
+    size = 256
+    buf = ctypes.create_unicode_buffer(size)
+    raise_on_zero(_FindNextVolume(hdl, buf, size))
+    return buf.value
+
+################################################################################
+
+_FindVolumeClose = fun_fact(_k32.FindVolumeClose, (BOOL, HANDLE))
+
+def FindVolumeClose(hdl):
+    raise_on_zero(_FindVolumeClose(hdl))
+
+################################################################################
+
+def enum_volumes():
+    hdl, vol = FindFirstVolume()
+    try:
+        while True:
+            yield vol
+            vol = FindNextVolume(hdl)
+    except OSError as e:
+        if e.winerror != ERROR_NO_MORE_FILES:
+            raise
+    finally:
+        FindVolumeClose(hdl)
+
+################################################################################
+
+_GetVolumePathNamesForVolumeName = fun_fact(
+    _k32.GetVolumePathNamesForVolumeNameW, (BOOL, PWSTR, PWSTR, DWORD, PDWORD)
+    )
+
+def GetVolumePathNamesForVolumeName(vol):
+    size = DWORD(256)
+    while True:
+        buf = ctypes.create_unicode_buffer(size.value)
+        ok = _GetVolumePathNamesForVolumeName(vol, buf, size, ref(size))
+        if ok:
+            return multi_str_from_ubuf(buf, size.value)
+        else:
+            if (err := GetLastError()) != ERROR_MORE_DATA:
+                raise_on_err(err)
+
+################################################################################
```

### Comparing `ctwin32-2.2.0/ctwin32/misc.py` & `ctwin32-2.3.0/ctwin32/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 ################################################################################
 
 _wts = ctypes.WinDLL("wtsapi32.dll")
 
 class WTS_SESSION_INFO(ctypes.Structure):
     _fields_ = (
         ("SessionId", DWORD),
-        ("WinStationName", PWSTR),
+        ("pWinStationName", PWSTR),
         ("State", LONG),
         )
 P_SESSION_INFO = POINTER(WTS_SESSION_INFO)
 PP_SESSION_INFO = POINTER(P_SESSION_INFO)
 
 ################################################################################
```

### Comparing `ctwin32-2.2.0/ctwin32/msi.py` & `ctwin32-2.3.0/ctwin32/msi.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/ctwin32/ntdll.py` & `ctwin32-2.3.0/ctwin32/ntdll.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,20 @@
     )
 
 _nt = ctypes.WinDLL("ntdll.dll")
 
 def _ntstatus(status):
     return LONG(status).value
 
+################################################################################
+
+RtlGetCurrentPeb = fun_fact(_nt.RtlGetCurrentPeb, (PVOID,))
+
+################################################################################
+
 STATUS_INFO_LENGTH_MISMATCH = _ntstatus(0xC0000004)
 STATUS_BUFFER_OVERFLOW = _ntstatus(0x80000005)
 STATUS_BUFFER_TOO_SMALL = _ntstatus(0xC0000023)
 STATUS_INVALID_SIGNATURE = _ntstatus(0xC000A000)
 
 ################################################################################
```

### Comparing `ctwin32-2.2.0/ctwin32/psapi.py` & `ctwin32-2.3.0/ctwin32/psapi.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/ctwin32/secur.py` & `ctwin32-2.3.0/ctwin32/secur.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     LUID,
     NTSTATUS,
     PLUID,
     POINTER,
     PPLUID,
     PVOID,
     PULONG,
-    SYSTEMTIME,
     UNICODE_STRING,
     ULONG,
     )
 from . import ref, fun_fact, suppress_winerr, ERROR_INVALID_PARAMETER
 from .ntdll import raise_failed_status
 from .kernel import FileTimeToLocalFileTime, FileTimeToSystemTime
 from .advapi import GetLengthSid, ConvertSidToStringSid
```

### Comparing `ctwin32-2.2.0/ctwin32/setupapi.py` & `ctwin32-2.3.0/ctwin32/setupapi.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/ctwin32/shell.py` & `ctwin32-2.3.0/ctwin32/shell.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/ctwin32/user.py` & `ctwin32-2.3.0/ctwin32/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,37 +371,37 @@
 ################################################################################
 
 class WINDOWPLACEMENT(ctypes.Structure):
     _fields_ = (
         ("length", UINT),
         ("flags", UINT),
         ("showCmd", UINT),
-        ("MinPosition", POINT),
-        ("MaxPosition", POINT),
-        ("NormalPosition", RECT),
+        ("ptMinPosition", POINT),
+        ("ptMaxPosition", POINT),
+        ("rcNormalPosition", RECT),
         )
 
     def __init__(self, f=0, s=1, mi=(0, 0), ma=(0, 0), no=(0, 0, 0, 0)):
         self.length = ctypes.sizeof(WINDOWPLACEMENT)
         self.flags = f
         self.showCmd = s
-        self.MinPosition = mi
-        self.MaxPosition = ma
-        self.NormalPosition = no
+        self.ptMinPosition = mi
+        self.ptMaxPosition = ma
+        self.rcNormalPosition = no
 
     def __repr__(self):
         cl = self.__class__.__name__
         ln = self.length
         fl = self.flags
         sc = self.showCmd
-        mi = f"({self.MinPosition.x}, {self.MinPosition.y})"
-        ma = f"({self.MaxPosition.x}, {self.MaxPosition.y})"
+        mi = f"({self.ptMinPosition.x}, {self.ptMinPosition.y})"
+        ma = f"({self.ptMaxPosition.x}, {self.ptMaxPosition.y})"
         no = (
-            f"({self.NormalPosition.left}, {self.NormalPosition.top}, ",
-            f"{self.NormalPosition.right}, {self.NormalPosition.bottom})"
+            f"({self.rcNormalPosition.left}, {self.rcNormalPosition.top}, ",
+            f"{self.rcNormalPosition.right}, {self.rcNormalPosition.bottom})"
             )
         return f"{cl}({ln}, {fl}, {sc}, {mi}, {ma}, {no})"
 
 PWINDOWPLACEMENT = POINTER(WINDOWPLACEMENT)
 
 ################################################################################
```

### Comparing `ctwin32-2.2.0/ctwin32/version.py` & `ctwin32-2.3.0/ctwin32/version.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/ctwin32/virtdisk.py` & `ctwin32-2.3.0/ctwin32/virtdisk.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/ctwin32/wndcls.py` & `ctwin32-2.3.0/ctwin32/wndcls.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/ctwin32/wtypes.py` & `ctwin32-2.3.0/ctwin32/wtypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,91 +111,91 @@
 ################################################################################
 
 class FILETIME(ctypes.Structure):
     "Time in 100 nanosecond steps since January 1, 1601 (UTC)"
     # cannot represent FILETIME as ctypes.c_ulonglong since that would change
     # the alignment
     _fields_ = (
-        ("LowDateTime", DWORD),
-        ("HighDateTime", DWORD),
+        ("dwLowDateTime", DWORD),
+        ("dwHighDateTime", DWORD),
         )
 
     def __init__(self, i64=0):
-        self.LowDateTime = i64 & 0xffffffff
-        self.HighDateTime = i64 >> 32
+        self.dwLowDateTime = i64 & 0xffffffff
+        self.dwHighDateTime = i64 >> 32
 
     def __int__(self):
-        return self.LowDateTime | (self.HighDateTime << 32)
+        return self.dwLowDateTime | (self.dwHighDateTime << 32)
 
     def __iadd__(self, other):
         i64 = int(self) + other
-        self.LowDateTime = i64 & 0xffffffff
-        self.HighDateTime = i64 >> 32
+        self.dwLowDateTime = i64 & 0xffffffff
+        self.dwHighDateTime = i64 >> 32
         return self
 
     def __repr__(self):
         return f"{self.__class__.__name__}({int(self)})"
 
 ################################################################################
 
 class SYSTEMTIME(ctypes.Structure):
     _fields_ = (
-        ("Year",         WORD),
-        ("Month",        WORD),
-        ("DayOfWeek",    WORD),
-        ("Day",          WORD),
-        ("Hour",         WORD),
-        ("Minute",       WORD),
-        ("Second",       WORD),
-        ("Milliseconds", WORD)
+        ("wYear",         WORD),
+        ("wMonth",        WORD),
+        ("wDayOfWeek",    WORD),
+        ("wDay",          WORD),
+        ("wHour",         WORD),
+        ("wMinute",       WORD),
+        ("wSecond",       WORD),
+        ("wMilliseconds", WORD)
         )
 
     ############################################################################
 
     def to_datetime(self):
         return datetime(
-            self.Year,
-            self.Month,
-            self.Day,
-            self.Hour,
-            self.Minute,
-            self.Second,
-            self.Milliseconds * 1000
+            self.wYear,
+            self.wMonth,
+            self.wDay,
+            self.wHour,
+            self.wMinute,
+            self.wSecond,
+            self.wMilliseconds * 1000
             )
 
     ############################################################################
 
     def from_datetime(self, dt):
-        self.Year = dt.year
-        self.Month = dt.month
-        self.Day = dt.day
-        self.Hour = dt.hour
-        self.Minute = dt.minute
-        self.Second = dt.second
-        self.Milliseconds = dt.microsecond // 1000
+        self.wYear = dt.year
+        self.wMonth = dt.month
+        self.wDay = dt.day
+        self.wHour = dt.hour
+        self.wMinute = dt.minute
+        self.wSecond = dt.second
+        self.wMilliseconds = dt.microsecond // 1000
         dow = dt.isoweekday()
-        self.DayOfWeek = 0 if dow == 7 else dow
+        self.wDayOfWeek = 0 if dow == 7 else dow
         return self
 
     ############################################################################
 
     def to_struct_time(self):
         return self.to_datetime().timetuple()
 
     ############################################################################
 
     def from_struct_time(self, st):
-        self.Year = st.tm_year
-        self.Month = st.tm_mon
-        self.Day = st.tm_mday
-        self.Hour = st.tm_hour
-        self.Minute = st.tm_min
-        self.Second = st.tm_sec
-        self.Milliseconds = 0
-        self.DayOfWeek = 0 if st.tm_wday == 6 else st.tm_wday + 1
+        self.wYear = st.tm_year
+        self.wMonth = st.tm_mon
+        self.wDay = st.tm_mday
+        self.wHour = st.tm_hour
+        self.wMinute = st.tm_min
+        self.wSecond = st.tm_sec
+        self.wMilliseconds = 0
+        self.wDayOfWeek = 0 if st.tm_wday == 6 else st.tm_wday + 1
         return self
 
     ############################################################################
 
     def __repr__(self):
         flds = ", ".join([f"{n}={getattr(self, n)}" for n, _ in self._fields_])
         return f"{self.__class__.__name__}({flds})"
@@ -269,17 +269,24 @@
 
 class LUID(ctypes.Structure):
     _fields_ = (
         ("LowPart", DWORD),
         ("HighPart", LONG)
         )
 
+    def __init__(self, value):
+        self.LowPart = value & 0xffffffff
+        self.HighPart = value >> 32
+
     def __int__(self):
         return self.LowPart | (self.HighPart << 32)
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}({int(self)})"
+
 ################################################################################
 
 class CallbackContext(ctypes.Structure):
     _fields_ = (
         ("callback", ctypes.py_object),
         ("context", ctypes.py_object)
         )
```

### Comparing `ctwin32-2.2.0/ctwin32.egg-info/PKG-INFO` & `ctwin32-2.3.0/ctwin32.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctwin32
-Version: 2.2.0
+Version: 2.3.0
 Summary: Access selected win32 APIs through ctypes
 Author: Rocco Matano
 License: MIT License
 Project-URL: homepage, https://github.com/RoccoMatano/ctwin32
 Project-URL: changelog, https://github.com/RoccoMatano/ctwin32/blob/master/changelog.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ctwin32-2.2.0/ctwin32.egg-info/SOURCES.txt` & `ctwin32-2.3.0/ctwin32.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -15,43 +15,49 @@
 ctwin32/misc.py
 ctwin32/msi.py
 ctwin32/ntdll.py
 ctwin32/psapi.py
 ctwin32/secur.py
 ctwin32/setupapi.py
 ctwin32/shell.py
+ctwin32/svc_util.py
 ctwin32/user.py
 ctwin32/version.py
 ctwin32/virtdisk.py
 ctwin32/wndcls.py
 ctwin32/wtypes.py
 ctwin32.egg-info/PKG-INFO
 ctwin32.egg-info/SOURCES.txt
 ctwin32.egg-info/dependency_links.txt
 ctwin32.egg-info/top_level.txt
+samples/__init__.py
+samples/api_set.py
 samples/arp_table.py
 samples/atta_vdisk.py
 samples/calendar.pyw
 samples/dump_ver_res.py
 samples/endis_bsl_usb.py
 samples/exbinmsi.py
 samples/extract_ico.py
 samples/find_zombies.py
 samples/fopa.py
 samples/hello_wnd.pyw
 samples/keyview.pyw
 samples/listpipes.py
 samples/logonsessions.py
+samples/lsc.py
 samples/netifaces.py
 samples/np_dev.py
 samples/power_requests.py
 samples/print_reparse_points.py
 samples/py_ver.py
 samples/remove_drive_by_letter.py
+samples/restart_usb_port.py
 samples/rm_sign_tool.py
 samples/senv.py
 samples/simple_aes.py
 samples/stopnow.py
 samples/sua_enums.py
 samples/test_sign_tool.py
 samples/uptime_evt.py
-samples/virt_term_seq.py
+samples/virt_term_seq.py
+samples/volume_paths.py
```

### Comparing `ctwin32-2.2.0/samples/arp_table.py` & `ctwin32-2.3.0/samples/arp_table.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/samples/atta_vdisk.py` & `ctwin32-2.3.0/samples/atta_vdisk.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 oflags = vdsk.OPEN_VIRTUAL_DISK_FLAG_NONE
 
 # Specify UNKNOWN for both device and vendor so the system will use
 # the file extension to determine the correct VHD format. The default values
 # do exactly that.
 storage_type = vdsk.VIRTUAL_STORAGE_TYPE()
 
-
 if (ext := path.rsplit(".", 1)[1].lower()) == "iso":
     oparams.Version = vdsk.OPEN_VIRTUAL_DISK_VERSION_1
     acc_mask = vdsk.VIRTUAL_DISK_ACCESS_READ
     aflags = (
         vdsk.ATTACH_VIRTUAL_DISK_FLAG_PERMANENT_LIFETIME
         | vdsk.ATTACH_VIRTUAL_DISK_FLAG_READ_ONLY
         )
@@ -51,13 +50,12 @@
     oparams.Version = vdsk.OPEN_VIRTUAL_DISK_VERSION_2
     oparams.Version2.GetInfoOnly = False
     aflags = vdsk.ATTACH_VIRTUAL_DISK_FLAG_PERMANENT_LIFETIME
 
     # not tested -> CHANGE THIS
     acc_mask = vdsk.VIRTUAL_DISK_ACCESS_NONE
 
-
 with vdsk.OpenVirtualDisk(storage_type, path, acc_mask, oflags, oparams) as vd:
     if do_detach:
         vdsk.DetachVirtualDisk(vd)
     else:
         vdsk.AttachVirtualDisk(vd, aflags)
```

### Comparing `ctwin32-2.2.0/samples/calendar.pyw` & `ctwin32-2.3.0/samples/calendar.pyw`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/samples/dump_ver_res.py` & `ctwin32-2.3.0/samples/dump_ver_res.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     ERROR_RESOURCE_TYPE_NOT_FOUND,
     ERROR_SHARING_VIOLATION,
     LOAD_LIBRARY_AS_DATAFILE,
     LOAD_LIBRARY_AS_IMAGE_RESOURCE,
     RT_VERSION,
     )
 from ctwin32.wtypes import (
-    DWORD,
     PSTR,
     PVOID,
     WORD,
     )
 from ctwin32.version import VS_FIXEDFILEINFO
 
 ################################################################################
@@ -162,17 +161,17 @@
     except OSError as e:
         if e.winerror not in EXPECTED_ERR:
             raise
 
 ################################################################################
 
 if __name__ == "__main__":
-    start_path = os.path.expandvars(sys.argv[1]) if len(sys.argv) > 1 else '.'
+    start_path = os.path.expandvars(sys.argv[1]) if len(sys.argv) > 1 else "."
     p = pathlib.Path(start_path).resolve()
-    for file in (e for e in p.rglob('*') if e.is_file()):
+    for file in (e for e in p.rglob("*") if e.is_file()):
         try:
             for ver_res_bytes in find_ver_res_in_file(file):
                 ver_res = parse_version_resource(ver_res_bytes)
                 print(f"\n{75 * '-'}\n\n{file}\n\nfixed:")
                 for name, value in ver_res.fixed_info.items():
                     print(f"    {name:18} = 0x{value:x}")
                 print("\nstrings:")
```

### Comparing `ctwin32-2.2.0/samples/endis_bsl_usb.py` & `ctwin32-2.3.0/samples/endis_bsl_usb.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/samples/exbinmsi.py` & `ctwin32-2.3.0/samples/exbinmsi.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/samples/extract_ico.py` & `ctwin32-2.3.0/samples/extract_ico.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/samples/find_zombies.py` & `ctwin32-2.3.0/samples/find_zombies.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,17 +68,15 @@
     return zombies
 
 ################################################################################
 
 def get_zombie_object_addresses(verbose):
     z = get_zombies(verbose)
     handles = ntdll.get_handles(kernel.GetCurrentProcessId())
-    res = dict(
-        [(h.Object, z[h.HandleValue]) for h in handles if h.HandleValue in z]
-        )
+    res = {h.Object: z[h.HandleValue] for h in handles if h.HandleValue in z}
     # Close the handles to the zombies so that we do not report that we ourself
     # hold on to them.
     for h in z:
         ntdll.NtClose(h)
     return res
 
 ################################################################################
```

### Comparing `ctwin32-2.2.0/samples/fopa.py` & `ctwin32-2.3.0/samples/fopa.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/samples/hello_wnd.pyw` & `ctwin32-2.3.0/samples/hello_wnd.pyw`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/samples/keyview.pyw` & `ctwin32-2.3.0/samples/keyview.pyw`

 * *Files 6% similar despite different names*

```diff
@@ -59,26 +59,24 @@
     wp: int = 0
     lp: int = 0
 
 ################################################################################
 
 class KeyViewWnd(wndcls.SimpleWnd):
 
+    CHAR_MSG = (WM_CHAR, WM_SYSCHAR, WM_DEADCHAR, WM_SYSDEADCHAR)
+
     def __init__(self, wc_params):
         self.heading = (
             " message        key     char              rep.  "
             "scan   ext. alt   prev  now"
             )
         self.underline = "".join(
                 (" " if c == " " else "_") for c in self.heading
                 )
-        self.msg_fmt = [
-            " %-13s %3d %-18s%c%6u  %4d     %3s %4s %6s %5s",
-            " %-13s          0x%04X     %1s%c %6u  %4d     %3s %4s %6s %5s"
-            ]
         self.msg_name = [
             "WM_KEYDOWN",
             "WM_KEYUP",
             "WM_CHAR",
             "WM_DEADCHAR",
             "WM_SYSKEYDOWN",
             "WM_SYSKEYUP",
@@ -126,30 +124,32 @@
         hdc, ps = self.begin_paint()
         prev_font = gdi.SelectObject(hdc, self.font)
 
         gdi.SetBkMode(hdc, TRANSPARENT)
         gdi.TextOut(hdc, 0, 0, self.heading)
         gdi.TextOut(hdc, 0, 0, self.underline)
 
-        char_msg = (WM_CHAR, WM_SYSCHAR, WM_DEADCHAR, WM_SYSDEADCHAR)
+
         for i in range(min(self.num_lines, self.y_lines)):
             then = self.history[i]
-            is_char = then.msg in char_msg
-            line = self.msg_fmt[is_char] % (
-                self.msg_name[then.msg - WM_KEYFIRST],
-                then.wp,
-                " " if is_char else user.GetKeyNameText(then.lp, True),
-                then.wp if is_char else ' ',
-                then.lp & 0xffff,
-                (then.lp >> 16) & 0xff,
-                "yes" if 0x01000000 & then.lp else "no",
-                "yes" if 0x20000000 & then.lp else "no",
-                "down" if 0x40000000 & then.lp else "up",
-                "up" if 0x80000000 & then.lp else "down",
-                )
+            rep = then.lp & 0xffff
+            scan = (then.lp >> 16) & 0xff
+            ext = "yes" if 0x01000000 & then.lp else "no"
+            alt = "yes" if 0x20000000 & then.lp else "no"
+            prev = "down" if 0x40000000 & then.lp else "up"
+            now = "up" if 0x80000000 & then.lp else "down"
+            name = self.msg_name[then.msg - WM_KEYFIRST]
+
+            if then.msg in self.CHAR_MSG:
+                middle = f"          {then.wp:#06x}      {chr(then.wp)} "
+            else:
+                kn = user.GetKeyNameText(then.lp, True)
+                middle = f" {then.wp:3} {kn:<18} "
+            end = f"{rep:6}  {scan:4}     {ext:>3} {alt:>4} {prev:>6} {now:>4}"
+            line = f" {name:<13}{middle}{end}"
             gdi.TextOut(hdc, 0, (self.y_lines - i) * self.char_height, line)
 
         gdi.SelectObject(hdc, prev_font)
         self.end_paint(ps)
         return 0
 
     ############################################################################
```

### Comparing `ctwin32-2.2.0/samples/listpipes.py` & `ctwin32-2.3.0/samples/listpipes.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/samples/logonsessions.py` & `ctwin32-2.3.0/samples/logonsessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 # inspired by
 # https://docs.microsoft.com/en-us/sysinternals/downloads/logonsessions
 
 import sys
 from ctwin32.advapi import running_as_admin
 from ctwin32.secur import LsaEnumerateLogonSessions
 
-
 if __name__ == "__main__":
     if not running_as_admin():
         m = "Need to run as administrator in order to enumerate logon sessions."
         print(m, file=sys.stderr)
         sys.exit(1)
 
     verbose = "-verbose" in sys.argv
@@ -51,15 +50,15 @@
         "RemoteInteractive",
         "CachedInteractive",
         "CachedRemoteInteractive",
         "CachedUnlock"
         ]
 
     def fmtt(dt):
-        return dt.isoformat(' ', 'seconds')
+        return dt.isoformat(" ", "seconds")
 
     for idx, ses in enumerate(LsaEnumerateLogonSessions()):
         lot = (
             lotypes[ses.LogonType] if 0 <= ses.LogonType < len(lotypes)
             else f"{ses.LogonType} (unknown)"
             )
         print(f"\n[{idx}] Logon session {ses.LogonId:016x}")
```

### Comparing `ctwin32-2.2.0/samples/netifaces.py` & `ctwin32-2.3.0/samples/netifaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,30 +24,26 @@
 
 # get_host_interfaces offers similar functionality as netifaces
 
 from ctwin32.iphlpapi import (
     get_host_interfaces,
     ConvertInterfaceGuidToLuid,
     ConvertInterfaceLuidToAlias,
-    ConvertInterfaceLuidToName,
     ConvertInterfaceIndexToLuid,
     )
 
 print("\nAdapters by index:\n")
 idx = 1
 while True:
     try:
         alias = ConvertInterfaceLuidToAlias(ConvertInterfaceIndexToLuid(idx))
         print(f"{idx:3}: {alias}")
         idx += 1
     except OSError:
         break
 
-
 print("\n\nInterfaces by adapter:")
 for guid, ifaces in get_host_interfaces(None, True).items():
     alias = ConvertInterfaceLuidToAlias(ConvertInterfaceGuidToLuid(guid))
     print(f"\nAdapter: {alias}, {guid}")
     for nif in ifaces:
         print(f"    {nif!r}")
-
-
```

### Comparing `ctwin32-2.2.0/samples/np_dev.py` & `ctwin32-2.3.0/samples/np_dev.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     for iset, ddat in enum_info_set(get_non_present_info_set()):
         desc = desc_from_info_set(iset, ddat)
         iid = SetupDiGetDeviceInstanceId(iset, ddat)
         print(f"{desc:40s} {iid}")
 
 ################################################################################
 
-do_remove = len(sys.argv) > 1 and sys.argv[1] == '-r'
+do_remove = len(sys.argv) > 1 and sys.argv[1] == "-r"
 have_to_elevate = do_remove and not advapi.running_as_admin()
 
 if have_to_elevate:
-    shell.elevate(f'"{sys.executable}"', f'"{__file__}"', '-r')
+    shell.elevate(f'"{sys.executable}"', f'"{__file__}"', "-r")
 else:
     print_non_present()
     if do_remove:
         print("\nremoving non present devices ...\n")
         remove_non_present_devices()
         print_non_present()
```

### Comparing `ctwin32-2.2.0/samples/power_requests.py` & `ctwin32-2.3.0/samples/power_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,21 +21,19 @@
 # DEALINGS IN THE SOFTWARE.
 #
 ################################################################################
 
 # This sample retrieves and prints power request. This is similar to what
 # `powercfg.exe /requests` does.
 
-import sys
 import ctypes
 from ctwin32 import (
     advapi,
     kernel,
     ntdll,
-    shell,
     user,
     suppress_winerr,
     ERROR_INSUFFICIENT_BUFFER,
     LOAD_LIBRARY_AS_DATAFILE,
     LOAD_LIBRARY_AS_IMAGE_RESOURCE,
     )
 from ctwin32.wtypes import (
@@ -45,49 +43,60 @@
     ULONG,
     ULONG_PTR,
     USHORT,
     )
 
 ################################################################################
 
+# flags for COUNTED_REASON_CONTEXT_RELATIVE.Flags
+DIAGNOSTIC_REASON_SIMPLE_STRING = 0x00000001
+DIAGNOSTIC_REASON_DETAILED_STRING = 0x00000002
+DIAGNOSTIC_REASON_NOT_SPECIFIED = 0x80000000
+DIAGNOSTIC_REASON_INVALID_FLAGS = ~ 0x80000007
+
 class _COUNTED_REASON_CTXT1(ctypes.Structure):
     _fields_ = (
         ("ResourceFileNameOffset", ULONG_PTR),
         ("ResourceReasonId", USHORT),
         ("StringCount", ULONG),
         ("SubstitutionStringsOffset", ULONG),
         )
+
 class _COUNTED_REASON_CTXT2(ctypes.Union):
     _anonymous_ = ("_anon1",)
     _fields_ = (
         ("_anon1", _COUNTED_REASON_CTXT1),
         ("SimpleStringOffset", ULONG_PTR),
         )
+
 class COUNTED_REASON_CONTEXT_RELATIVE(ctypes.Structure):
     _anonymous_ = ("_anon1",)
     _fields_ = (
         ("Flags", ULONG),
         ("_anon1", _COUNTED_REASON_CTXT2),
         )
 
+# caller types for DIAGNOSTIC_BUFFER.CallerType
 KERNEL_REQUESTER = 0
 PROCESS_REQUESTER = 1
 SERVICE_REQUESTER = 2
 
 class _DIAG_BUFF1(ctypes.Structure):
     _fields_ = (
         ("ProcessImageNameOffset", ULONG_PTR),
         ("ProcessId", ULONG),
         ("ServiceTag", ULONG),
         )
+
 class _DIAG_BUFF2(ctypes.Structure):
     _fields_ = (
         ("DeviceDescriptionOffset", ULONG_PTR),
         ("DevicePathOffset", ULONG_PTR),
         )
+
 class _DIAG_BUFF3(ctypes.Union):
     _anonymous_ = ("_anon1", "_anon2")
     _fields_ = (
         ("_anon1", _DIAG_BUFF1),
         ("_anon2", _DIAG_BUFF2),
         )
 
@@ -99,14 +108,15 @@
         ("_anon3", _DIAG_BUFF3),
         ("ReasonOffset", ULONG_PTR),
         )
 
 # !! for simplicity we ignore all the definitions older than Windows 10 RS1+ !!
 
 POWER_REQUEST_SUPPORTED_TYPES = 6
+
 class POWER_REQUEST(ctypes.Structure):
     _fields_ = (
         ("SupportedRequestMask", ULONG),
         ("PowerRequestCount", ULONG * POWER_REQUEST_SUPPORTED_TYPES),
         ("DiagnosticBuffer", DIAGNOSTIC_BUFFER),
         )
 
@@ -125,17 +135,17 @@
     2: "AWAYMODE",
     3: "EXECUTION",
     4: "PERFBOOST",
     5: "ACTIVELOCKSCREEN",
     }
 
 requester_types = {
-    KERNEL_REQUESTER  : "[DRIVER]",
-    PROCESS_REQUESTER : "[PROCESS]",
-    SERVICE_REQUESTER : "[SERVICE]",
+    KERNEL_REQUESTER:  "[DRIVER]",
+    PROCESS_REQUESTER: "[PROCESS]",
+    SERVICE_REQUESTER: "[SERVICE]",
     }
 
 ################################################################################
 
 def get_power_requests():
     GetPowerRequestList = 45
     data = b""
@@ -144,19 +154,21 @@
         size *= 2
         with suppress_winerr(ERROR_INSUFFICIENT_BUFFER):
             data = ntdll.NtPowerInformation(GetPowerRequestList, None, size)
     count = int.from_bytes(
         data[:ctypes.sizeof(ULONG_PTR)],
         byteorder=ENDIANNESS
         )
+
     class POWER_REQUEST_LIST(ctypes.Structure):
         _fields_ = (
             ("Count", ULONG),
             ("PowerRequestOffsets", ULONG_PTR * count),
             )
+
     buf = ctypes.create_string_buffer(data)
     prl = POWER_REQUEST_LIST.from_buffer(buf)
 
     requests = {k: [] for k in request_types}
     for ri in range(prl.Count):
         pr = POWER_REQUEST.from_address(
             ctypes.addressof(buf) + prl.PowerRequestOffsets[ri]
@@ -188,43 +200,61 @@
                     ]
             reason = ""
             if pr.DiagnosticBuffer.ReasonOffset:
                 ro = COUNTED_REASON_CONTEXT_RELATIVE.from_address(
                     db_addr + pr.DiagnosticBuffer.ReasonOffset
                     )
                 ro_addr = ctypes.addressof(ro)
-                if ro.Flags & 1:
+                if ro.Flags & DIAGNOSTIC_REASON_SIMPLE_STRING:
                     reason = ctypes.wstring_at(ro_addr + ro.SimpleStringOffset)
-                elif ro.Flags & 2:
+                elif ro.Flags & DIAGNOSTIC_REASON_DETAILED_STRING:
                     mod_name = ctypes.wstring_at(
                         ro_addr + ro.ResourceFileNameOffset
                         )
                     reason = load_res_str(mod_name, ro.ResourceReasonId)
 
             requests[rt].append((callt_str, callid, reason))
 
     return requests
 
+################################################################################
+
+def print_power_requests():
+    requests = get_power_requests()
+    print()
+    for req_type in sorted(request_types):
+        requesters = requests[req_type]
+        tstr = request_types[req_type]
+        print(f"{tstr}:\n{(len(tstr) + 1) * '-'}")
+        if not requesters:
+            print("None\n")
+            continue
+        for ct, cid, reason in requesters:
+            print(f"{ct} ", end="")
+            for element in cid:
+                print(element)
+            print(f"{reason}\n")
 
 ################################################################################
 
 if __name__ == "__main__":
 
     if advapi.running_as_admin():
-        requests = get_power_requests()
-        print()
-        for req_type in sorted(request_types):
-            requesters = requests[req_type]
-            tstr = request_types[req_type]
-            print(f"{tstr}:\n{(len(tstr) + 1) * '-'}")
-            if not requesters:
-                print("None\n")
-                continue
-            for ct, cid, reason in requesters:
-                print(f"{ct} ", end="")
-                for element in cid:
-                    print(element)
-                print(f"{reason}\n")
+        print("initial:")
+        print(80 * "-")
+        print_power_requests()
+
+        # create and activate a SystemRequired request
+        print("with self created 'SystemRequired' request:")
+        print(80 * "-")
+        reason = "demonstarting power requests"
+        req = kernel.PowerRequest.SystemRequired
+        with kernel.create_power_request(reason, req) as hdl:
+            print_power_requests()
+
+        print("final:")
+        print(80 * "-")
+        print_power_requests()
     else:
         print("Inquiring power request requires administrative privileges.")
 
 ################################################################################
```

### Comparing `ctwin32-2.2.0/samples/print_reparse_points.py` & `ctwin32-2.3.0/samples/print_reparse_points.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
 import os
 import ctypes
 import ctwin32
 from ctwin32 import (
     suppress_winerr,
     ERROR_MORE_DATA,
+    FILE_ATTRIBUTE_REPARSE_POINT,
     FILE_FLAG_OPEN_REPARSE_POINT,
     FILE_FLAG_BACKUP_SEMANTICS,
-    FILE_ATTRIBUTE_REPARSE_POINT,
     IO_REPARSE_TAG_SYMLINK,
     IO_REPARSE_TAG_MOUNT_POINT,
     )
 from ctwin32.wtypes import (
     BYTE,
     ULONG,
     USHORT,
@@ -74,16 +74,16 @@
         ("MountPointReparseBuffer", RP_DATA_MOUNTPOINT),
         ("GenericReparseBuffer", RP_DATA_GENERIC),
         )
 
 class REPARSE_DATA_BUFFER(ctypes.Structure):
     _fields_ = (
         ("ReparseTag", ULONG),
-        ('ReparseDataLength', USHORT),
-        ('Reserved', USHORT),
+        ("ReparseDataLength", USHORT),
+        ("Reserved", USHORT),
         ("_anon", RP_DATA_UN),
         )
     _anonymous_ = ("_anon",)
 
 PREPARSE_DATA_BUFFER = ctypes.POINTER(REPARSE_DATA_BUFFER)
 
 FSCTL_GET_REPARSE_POINT = 0x000900a8
@@ -126,20 +126,20 @@
         slen = src.PrintNameLength // 2
 
     return ctypes.wstring_at(saddr, slen)
 
 ################################################################################
 
 reparse_tags = {
-    v:k for k, v in vars(ctwin32).items() if k.startswith("IO_REPARSE_TAG_")
+    v: k for k, v in vars(ctwin32).items() if k.startswith("IO_REPARSE_TAG_")
     }
 follow = (IO_REPARSE_TAG_SYMLINK, IO_REPARSE_TAG_MOUNT_POINT)
 
-for directory, info in iter_dir(os.environ["SystemDrive"]):
-    if info.dwFileAttributes & ctwin32.FILE_ATTRIBUTE_REPARSE_POINT:
+for directory, info in iter_dir(os.environ["SYSTEMDRIVE"]):
+    if info.dwFileAttributes & FILE_ATTRIBUTE_REPARSE_POINT:
         rpp = rf"{directory}\{info.cFileName}"
         if info.dwReserved0 in reparse_tags:
             tag = reparse_tags[info.dwReserved0]
         else:
             tag = f"UNKNOWN: 0x{info.dwReserved0:08x}"
         if info.dwReserved0 in follow:
             print(f"{tag:32} {rpp}\n    -> {readlink(rpp)}")
```

### Comparing `ctwin32-2.2.0/samples/py_ver.py` & `ctwin32-2.3.0/samples/py_ver.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,21 +38,21 @@
     field3 = fver_ls >> 16
     api_ver = fver_ls & 0xffff
 
     # see https://github.com/python/cpython/blob/main/PCbuild/field3.py
     micro, remainder = divmod(field3, 1000)
     level, serial = divmod(remainder, 10)
     level = {
-        0xa: 'alpha',
-        0xb: 'beta',
-        0xc: 'candidate',
-        0xf: 'final'
+        0xa: "alpha",
+        0xb: "beta",
+        0xc: "candidate",
+        0xf: "final"
         }[level]
     ver_info = collections.namedtuple(
-        'version_info',
+        "version_info",
         ["major", "minor", "micro", "releaselevel", "serial"]
         )(major, minor, micro, level, serial)
     return ver_info, api_ver
 
 ################################################################################
 
 if __name__ == "__main__":
```

### Comparing `ctwin32-2.2.0/samples/remove_drive_by_letter.py` & `ctwin32-2.3.0/samples/remove_drive_by_letter.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,29 +79,29 @@
 ################################################################################
 
 def get_drive_devinst(drv_type, drv_num):
     # In order to find the devinst that corresponds to a certain drive, we
     # have to iterate over all device interfaces that match the drive type. The
     # drive number is only unique within the group of devices that share the
     # same interface.
-    if drv_type == FILE_DEVICE_CD_ROM or drv_type == FILE_DEVICE_DVD:
+    if drv_type in (FILE_DEVICE_CD_ROM, FILE_DEVICE_DVD):
         guid = GUID_IFACE_CDROM
     elif drv_type == FILE_DEVICE_DISK:
         # ignoring that floppies ever existed
         guid = GUID_IFACE_DISK
     else:
         raise ValueError(f"unhandled drive type: {drv_type}")
 
     for iset, did in setupapi.enum_dev_interfaces(guid):
         dev_path, deinda = setupapi.SetupDiGetDeviceInterfaceDetail(iset, did)
         dtype, dnum = get_drive_type_number(dev_path)
         if dtype == drv_type and dnum == drv_num:
             return deinda.DevInst
 
-    raise EnvironmentError(f"devinst not found for {drv_type} {drv_num}")
+    raise OSError(f"devinst not found for {drv_type} {drv_num}")
 
 ################################################################################
 
 def remove_drive_by_letter(letter):
     o = ord(letter)
     if o < ord("A") or o > ord("Z"):
         raise ValueError(f"invalid drive letter: {letter}")
```

### Comparing `ctwin32-2.2.0/samples/rm_sign_tool.py` & `ctwin32-2.3.0/samples/rm_sign_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,32 +102,32 @@
 
 ################################################################################
 
 def parse_args():
     ape = argparse.ArgumentParser()
     sub = ape.add_subparsers(
         title="available commands",
-        dest='cmd',
-        help='action',
-        metavar='command'
+        dest="cmd",
+        help="action",
+        metavar="command"
         )
 
-    create = sub.add_parser('create', help='create a new key pair')
+    create = sub.add_parser("create", help="create a new key pair")
     create.add_argument(
         dest="private",
         metavar="<private_keyfile>",
         help="name of private key file"
         )
     create.add_argument(
         dest="public",
         metavar="<public_keyfile>",
         help="name of public key file"
         )
 
-    sign = sub.add_parser('sign', help='create signature for a file')
+    sign = sub.add_parser("sign", help="create signature for a file")
     sign.add_argument(
         "-k",
         dest="keyfile",
         metavar="<private_keyfile>",
         help="name of private key file",
         required=True
         )
@@ -138,23 +138,23 @@
         help="name of output file for signature",
         required=True
         )
     sign.add_argument(
         "-x",
         dest="outhex",
         help="output signature as hex string",
-        action='store_true'
+        action="store_true"
         )
     sign.add_argument(
         dest="sourcefile",
         metavar="<source_file>",
         help="name of file to sign"
         )
 
-    verify = sub.add_parser('verify', help='verify signature for a file')
+    verify = sub.add_parser("verify", help="verify signature for a file")
     verify.add_argument(
         "-k",
         dest="keyfile",
         metavar="<public_keyfile>",
         help="name of public key file",
         required=True
         )
```

### Comparing `ctwin32-2.2.0/samples/senv.py` & `ctwin32-2.3.0/samples/senv.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/samples/simple_aes.py` & `ctwin32-2.3.0/samples/simple_aes.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,26 +80,26 @@
     lines = []
     hex_chars = bytes_per_line * 3 - 1
     length = len(data)
     offset = 0
     while offset < length:
         chunk_len = min(length - offset, bytes_per_line)
         chunk = data[offset:offset + chunk_len]
-        ascii = chunk.translate(_ascii_trans).decode('ascii')
+        ascii = chunk.translate(_ascii_trans).decode("ascii")
         hexa = " ".join([f"{c:02x}" for c in chunk]).ljust(hex_chars)
         lines.append(f"{offset:08x} | {hexa} | {ascii}")
         offset += chunk_len
     return "\n".join(lines)
 
 ################################################################################
 
 if __name__ == "__main__":
 
     try:
-        assert False
+        assert 1 == 2
     except AssertionError:
         pass
     else:
         raise RuntimeError("Assertions are not active")
 
     plain = bytes(range(256))
     key = b"\xf8\xa9V\x9e'#1\xd7\x1a\x85\r)\x02\x8c,\xa9"
```

### Comparing `ctwin32-2.2.0/samples/stopnow.py` & `ctwin32-2.3.0/samples/stopnow.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,29 +36,29 @@
     )
 
 ################################################################################
 
 def parse_args():
     ape = argparse.ArgumentParser()
     grp = ape.add_mutually_exclusive_group(required=True)
-    grp.add_argument("-s", "--shutdown", action='store_true')
-    grp.add_argument("-r", "--restart", action='store_true')
-    grp.add_argument("-l", "--logout", action='store_true')
-    grp.add_argument("-e", "--hibernate", action='store_true')
-    grp.add_argument("-y", "--standby", action='store_true')
-    grp.add_argument("-k", "--lock", action='store_true')
-    grp.add_argument("-d", "--disconnect", action='store_true')
+    grp.add_argument("-s", "--shutdown", action="store_true")
+    grp.add_argument("-r", "--restart", action="store_true")
+    grp.add_argument("-l", "--logout", action="store_true")
+    grp.add_argument("-e", "--hibernate", action="store_true")
+    grp.add_argument("-y", "--standby", action="store_true")
+    grp.add_argument("-k", "--lock", action="store_true")
+    grp.add_argument("-d", "--disconnect", action="store_true")
     return ape.parse_args()
 
 ################################################################################
 
 def disconnect_rdp():
     for info in misc.WTSEnumerateSessions():
         if info.State == WTSActive:
-            if info.WinStationName.startswith("RDP-Tcp"):
+            if info.pWinStationName.startswith("RDP-Tcp"):
                 misc.WTSDisconnectSession(info.SessionId)
 
 ################################################################################
 
 def main():
     args = parse_args()
```

### Comparing `ctwin32-2.2.0/samples/sua_enums.py` & `ctwin32-2.3.0/samples/sua_enums.py`

 * *Files identical despite different names*

### Comparing `ctwin32-2.2.0/samples/test_sign_tool.py` & `ctwin32-2.3.0/samples/test_sign_tool.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,34 +21,29 @@
 # DEALINGS IN THE SOFTWARE.
 #
 ################################################################################
 
 import sys
 import shutil
 import pathlib
+import contextlib
 import subprocess
 
 DEFAULT_PREFIX = "$default_prefix$"
-
-if len(sys.argv) >= 2:
-    prefix = sys.argv[1]
-else:
-    prefix = DEFAULT_PREFIX
+prefix = sys.argv[1] if len(sys.argv) >= 2 else DEFAULT_PREFIX
 tool = pathlib.Path(__file__).resolve().parent / "rm_sign_tool.py"
 
 def run(*args):
     cmd = [sys.executable, tool]
     cmd.extend(map(str, args))
     subprocess.run(cmd, check=True)
 
 def unlink(pth):
-    try:
+    with contextlib.suppress(OSError):
         pth.unlink()
-    except OSError:
-        pass
 
 private = pathlib.Path(f"{prefix}.private.key")
 public = pathlib.Path(f"{prefix}.public.key")
 signature = pathlib.Path(f"{prefix}.{tool.name}.sig")
 fake = pathlib.Path(f"{prefix}.{tool.name}.fake")
 
 try:
```

### Comparing `ctwin32-2.2.0/samples/uptime_evt.py` & `ctwin32-2.3.0/samples/uptime_evt.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     with advapi.OpenEventLog("System") as log:
         some_events = advapi.ReadEventLog(log)
         while some_events:
             for e in some_events:
                 if (e.EventID & 0xffff) == BOOT_EVENT_ID:
                     return e.TimeGenerated
             some_events = advapi.ReadEventLog(log)
-    raise EnvironmentError("no boot event found")
+    raise OSError("no boot event found")
 
 def up_time(time_boot=None):
     if time_boot is None:
         time_boot = boot_time()
     utime = datetime.datetime.now() - time_boot
     return datetime.timedelta(seconds=int(utime.total_seconds()))
```

### Comparing `ctwin32-2.2.0/samples/virt_term_seq.py` & `ctwin32-2.3.0/samples/virt_term_seq.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,31 @@
 
 from ctwin32 import kernel
 
 # enable 'virtual terminal sequences'
 kernel.enable_virt_term()
 
 print("\x1b[31mThis text has a red foreground using SGR.31.\r\n")
-print("\x1b[1mThis text has a bright (bold) red foreground using SGR.1 to affect the previous color setting.\r\n")
-print("\x1b[mThis text has returned to default colors using SGR.0 implicitly.\r\n")
-print("\x1b[34;46mThis text shows the foreground and background change at the same time.\r\n")
-print("\x1b[0mThis text has returned to default colors using SGR.0 explicitly.\r\n")
-print("\x1b[31;32;33;34;35;36;101;102;103;104;105;106;107mThis text attempts to apply many colors in the same command. Note the colors are applied from left to right so only the right-most option of foreground cyan (SGR.36) and background bright white (SGR.107) is effective.\r\n")
+print(
+    "\x1b[1mThis text has a bright (bold) red foreground using SGR.1 to "
+    "affect the previous color setting.\r\n"
+    )
+print(
+    "\x1b[mThis text has returned to default colors using SGR.0 "
+    "implicitly.\r\n"
+    )
+print(
+    "\x1b[34;46mThis text shows the foreground and background change at "
+    "the same time.\r\n"
+    )
+print(
+    "\x1b[0mThis text has returned to default colors using SGR.0 "
+    "explicitly.\r\n"
+    )
+print(
+    "\x1b[31;32;33;34;35;36;101;102;103;104;105;106;107mThis text attempts "
+    "to apply many colors in the same command. Note the colors are applied "
+    "from left to right so only the right-most option of foreground cyan "
+    "(SGR.36) and background bright white (SGR.107) is effective.\r\n"
+    )
 print("\x1b[39mThis text has restored the foreground color only.\r\n")
 print("\x1b[49mThis text has restored the background color only.\r\n")
```

### Comparing `ctwin32-2.2.0/setup.py` & `ctwin32-2.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 import sys
 import argparse
 from setuptools import setup
+from wheel.bdist_wheel import bdist_wheel
 
 ################################################################################
 
 # trying to build on non Windows OS is useless
 if sys.platform != "win32":
     raise OSError("building ctwin32 on non Windows OS is futile")
 
 ################################################################################
 
+# hack to ensure platform tag can be set from the outside
+
 parser = argparse.ArgumentParser(add_help=False)
 parser.add_argument("-p", "--platform-name", default="")
 args, remain = parser.parse_known_args()
 remain.insert(0, sys.argv[0])
 sys.argv = remain
 PLATFORM_NAME = args.platform_name
 
-################################################################################
-
-# hack to ensure platform tag can be set from the outside
-from wheel.bdist_wheel import bdist_wheel
-
 class hacked_bdist_wheel(bdist_wheel):
     def get_tag(self):
         impl, abi_tag, platform = super().get_tag()
         return (impl, abi_tag, PLATFORM_NAME if PLATFORM_NAME else platform)
 
 ################################################################################
 
-setup(cmdclass={'bdist_wheel': hacked_bdist_wheel})
+setup(cmdclass={"bdist_wheel": hacked_bdist_wheel})
 
 ################################################################################
```

