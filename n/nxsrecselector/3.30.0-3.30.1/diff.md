# Comparing `tmp/nxsrecselector-3.30.0.tar.gz` & `tmp/nxsrecselector-3.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxsrecselector-3.30.0.tar", last modified: Thu Jun 29 12:49:32 2023, max compression
+gzip compressed data, was "nxsrecselector-3.30.1.tar", last modified: Tue Jul  4 05:22:52 2023, max compression
```

## Comparing `nxsrecselector-3.30.0.tar` & `nxsrecselector-3.30.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-29 12:49:32.052490 nxsrecselector-3.30.0/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.30.0/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.30.0/MANIFEST.in
--rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2023-06-27 15:45:03.000000 nxsrecselector-3.30.0/NXSRecSelector
--rw-r--r--   0 jkotan   (15949) irc         (39)     7068 2023-06-29 12:49:32.052490 nxsrecselector-3.30.0/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     4313 2023-06-23 12:04:33.000000 nxsrecselector-3.30.0/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-29 12:49:32.048490 nxsrecselector-3.30.0/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)      938 2017-03-18 22:59:30.000000 nxsrecselector-3.30.0/man/NXSRecSelector.1
--rw-r--r--   0 jkotan   (15949) irc         (39)   109341 2023-03-10 08:35:11.000000 nxsrecselector-3.30.0/man/nxsrecconfig.1
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-29 12:49:32.052490 nxsrecselector-3.30.0/nxsrecconfig/
--rw-r--r--   0 jkotan   (15949) irc         (39)     6669 2023-06-07 08:45:59.000000 nxsrecselector-3.30.0/nxsrecconfig/CheckerThread.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2020-01-31 13:48:24.000000 nxsrecselector-3.30.0/nxsrecconfig/Converter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    23789 2023-02-01 13:37:17.000000 nxsrecselector-3.30.0/nxsrecconfig/Describer.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    22847 2023-02-01 13:37:17.000000 nxsrecselector-3.30.0/nxsrecconfig/DynamicComponent.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    19957 2023-06-07 08:45:59.000000 nxsrecselector-3.30.0/nxsrecconfig/MacroServerPools.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    75699 2023-06-29 12:48:10.000000 nxsrecselector-3.30.0/nxsrecconfig/NXSConfig.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    59493 2023-06-29 12:48:10.000000 nxsrecselector-3.30.0/nxsrecconfig/ProfileManager.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      930 2023-06-29 12:48:10.000000 nxsrecselector-3.30.0/nxsrecconfig/Release.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2020-01-31 13:48:24.000000 nxsrecselector-3.30.0/nxsrecconfig/Selection.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    16157 2023-02-01 13:37:17.000000 nxsrecselector-3.30.0/nxsrecconfig/Selector.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    45630 2023-06-29 12:48:10.000000 nxsrecselector-3.30.0/nxsrecconfig/Settings.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 16:17:52.000000 nxsrecselector-3.30.0/nxsrecconfig/StreamSet.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    29259 2023-05-26 09:16:32.000000 nxsrecselector-3.30.0/nxsrecconfig/Utils.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-02-01 13:37:17.000000 nxsrecselector-3.30.0/nxsrecconfig/__init__.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-29 12:49:32.052490 nxsrecselector-3.30.0/nxsrecselector.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)     7068 2023-06-29 12:49:31.000000 nxsrecselector-3.30.0/nxsrecselector.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)      710 2023-06-29 12:49:32.000000 nxsrecselector-3.30.0/nxsrecselector.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-06-29 12:49:31.000000 nxsrecselector-3.30.0/nxsrecselector.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.30.0/nxsrecselector.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       17 2023-06-29 12:49:31.000000 nxsrecselector-3.30.0/nxsrecselector.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       13 2023-06-29 12:49:31.000000 nxsrecselector-3.30.0/nxsrecselector.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      213 2023-06-29 12:49:32.052490 nxsrecselector-3.30.0/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     3985 2022-05-18 15:32:00.000000 nxsrecselector-3.30.0/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-07-04 05:22:52.185659 nxsrecselector-3.30.1/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.30.1/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.30.1/MANIFEST.in
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2023-06-27 15:45:03.000000 nxsrecselector-3.30.1/NXSRecSelector
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7119 2023-07-04 05:22:52.185659 nxsrecselector-3.30.1/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4313 2023-06-23 12:04:33.000000 nxsrecselector-3.30.1/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-07-04 05:22:52.181659 nxsrecselector-3.30.1/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      938 2017-03-18 22:59:30.000000 nxsrecselector-3.30.1/man/NXSRecSelector.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)   109341 2023-03-10 08:35:11.000000 nxsrecselector-3.30.1/man/nxsrecconfig.1
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-07-04 05:22:52.181659 nxsrecselector-3.30.1/nxsrecconfig/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6669 2023-06-07 08:45:59.000000 nxsrecselector-3.30.1/nxsrecconfig/CheckerThread.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2020-01-31 13:48:24.000000 nxsrecselector-3.30.1/nxsrecconfig/Converter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    23789 2023-02-01 13:37:17.000000 nxsrecselector-3.30.1/nxsrecconfig/Describer.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    22847 2023-02-01 13:37:17.000000 nxsrecselector-3.30.1/nxsrecconfig/DynamicComponent.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    19957 2023-06-07 08:45:59.000000 nxsrecselector-3.30.1/nxsrecconfig/MacroServerPools.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    75699 2023-06-29 12:48:10.000000 nxsrecselector-3.30.1/nxsrecconfig/NXSConfig.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    59851 2023-07-04 05:22:18.000000 nxsrecselector-3.30.1/nxsrecconfig/ProfileManager.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      930 2023-07-04 05:22:18.000000 nxsrecselector-3.30.1/nxsrecconfig/Release.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2020-01-31 13:48:24.000000 nxsrecselector-3.30.1/nxsrecconfig/Selection.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    16157 2023-02-01 13:37:17.000000 nxsrecselector-3.30.1/nxsrecconfig/Selector.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    45630 2023-06-29 12:48:10.000000 nxsrecselector-3.30.1/nxsrecconfig/Settings.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 16:17:52.000000 nxsrecselector-3.30.1/nxsrecconfig/StreamSet.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    29259 2023-05-26 09:16:32.000000 nxsrecselector-3.30.1/nxsrecconfig/Utils.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-02-01 13:37:17.000000 nxsrecselector-3.30.1/nxsrecconfig/__init__.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-07-04 05:22:52.185659 nxsrecselector-3.30.1/nxsrecselector.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7119 2023-07-04 05:22:52.000000 nxsrecselector-3.30.1/nxsrecselector.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)      710 2023-07-04 05:22:52.000000 nxsrecselector-3.30.1/nxsrecselector.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-07-04 05:22:52.000000 nxsrecselector-3.30.1/nxsrecselector.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.30.1/nxsrecselector.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       17 2023-07-04 05:22:52.000000 nxsrecselector-3.30.1/nxsrecselector.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)       13 2023-07-04 05:22:52.000000 nxsrecselector-3.30.1/nxsrecselector.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      213 2023-07-04 05:22:52.185659 nxsrecselector-3.30.1/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4035 2023-06-29 15:14:01.000000 nxsrecselector-3.30.1/setup.py
```

### Comparing `nxsrecselector-3.30.0/COPYRIGHT` & `nxsrecselector-3.30.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/NXSRecSelector` & `nxsrecselector-3.30.1/NXSRecSelector`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/PKG-INFO` & `nxsrecselector-3.30.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsrecselector
-Version: 3.30.0
+Version: 3.30.1
 Summary: Selector Server for NeXus Sardana recorder
 Home-page: https://github.com/jkotan/nexdatas/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ========================================
         Welcome to nxsrecconfig's documentation!
@@ -224,7 +224,8 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `nxsrecselector-3.30.0/README.rst` & `nxsrecselector-3.30.1/README.rst`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/man/NXSRecSelector.1` & `nxsrecselector-3.30.1/man/NXSRecSelector.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/man/nxsrecconfig.1` & `nxsrecselector-3.30.1/man/nxsrecconfig.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/CheckerThread.py` & `nxsrecselector-3.30.1/nxsrecconfig/CheckerThread.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/Converter.py` & `nxsrecselector-3.30.1/nxsrecconfig/Converter.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/Describer.py` & `nxsrecselector-3.30.1/nxsrecconfig/Describer.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/DynamicComponent.py` & `nxsrecselector-3.30.1/nxsrecconfig/DynamicComponent.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/MacroServerPools.py` & `nxsrecselector-3.30.1/nxsrecconfig/MacroServerPools.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/NXSConfig.py` & `nxsrecselector-3.30.1/nxsrecconfig/NXSConfig.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/ProfileManager.py` & `nxsrecselector-3.30.1/nxsrecconfig/ProfileManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,14 +344,25 @@
         if sync:
             self.__setFromMntGrpConf(conf, componentdatasources)
         self.__selector.storeSelection()
 
         if self.mutedPreScanAttrFilters:
             mginfo['snapshot'] = PoolUtils.filterOutTango(
                 mginfo['snapshot'], self.mutedPreScanAttrFilters)
+
+        unique_snapshot = []
+        unique_names = []
+        for sn in mginfo['snapshot']:
+            if sn[0] not in unique_names and \
+               sn[1] not in unique_names:
+                unique_names.append(sn[0])
+                unique_names.append(sn[1])
+                unique_snapshot.append(sn)
+        mginfo['snapshot'] = unique_snapshot
+
         MSUtils.setEnvs(
             {'PreScanSnapshot': mginfo['snapshot'],
              'ActiveMntGrp': mginfo['alias']},
             self.__macroServerName
         )
         return conf
```

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/Release.py` & `nxsrecselector-3.30.1/nxsrecconfig/Release.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """  NeXus Sardana Recorder Settings - Release """
 
 #: (:obj:`str`) package version
-__version__ = "3.30.0"
+__version__ = "3.30.1"
```

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/Selection.py` & `nxsrecselector-3.30.1/nxsrecconfig/Selection.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/Selector.py` & `nxsrecselector-3.30.1/nxsrecconfig/Selector.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/Settings.py` & `nxsrecselector-3.30.1/nxsrecconfig/Settings.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/StreamSet.py` & `nxsrecselector-3.30.1/nxsrecconfig/StreamSet.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/Utils.py` & `nxsrecselector-3.30.1/nxsrecconfig/Utils.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecconfig/__init__.py` & `nxsrecselector-3.30.1/nxsrecconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/nxsrecselector.egg-info/PKG-INFO` & `nxsrecselector-3.30.1/nxsrecselector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsrecselector
-Version: 3.30.0
+Version: 3.30.1
 Summary: Selector Server for NeXus Sardana recorder
 Home-page: https://github.com/jkotan/nexdatas/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ========================================
         Welcome to nxsrecconfig's documentation!
@@ -224,7 +224,8 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `nxsrecselector-3.30.0/nxsrecselector.egg-info/SOURCES.txt` & `nxsrecselector-3.30.1/nxsrecselector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.30.0/setup.py` & `nxsrecselector-3.30.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,14 +111,15 @@
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     install_requires=install_requires,
     scripts=['NXSRecSelector'],
     cmdclass={
         # 'test': TestCommand,
         'build_sphinx': BuildDoc
     },
```

