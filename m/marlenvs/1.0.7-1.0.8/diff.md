# Comparing `tmp/marlenvs-1.0.7.tar.gz` & `tmp/marlenvs-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marlenvs-1.0.7.tar", last modified: Thu Mar  3 08:58:26 2022, max compression
+gzip compressed data, was "marlenvs-1.0.8.tar", last modified: Thu Mar  3 09:04:18 2022, max compression
```

## Comparing `marlenvs-1.0.7.tar` & `marlenvs-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2022-03-03 08:58:26.449971 marlenvs-1.0.7/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1069 2022-01-10 11:58:33.000000 marlenvs-1.0.7/LICENSE
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      211 2022-03-03 08:58:26.449971 marlenvs-1.0.7/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1807 2022-02-06 16:05:06.000000 marlenvs-1.0.7/README.md
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2022-03-03 08:58:26.445971 marlenvs-1.0.7/marlenvs/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      270 2022-02-02 12:21:55.000000 marlenvs-1.0.7/marlenvs/__init__.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2022-03-03 08:58:26.445971 marlenvs-1.0.7/marlenvs/navigation_env/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       65 2022-02-02 10:04:20.000000 marlenvs-1.0.7/marlenvs/navigation_env/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     9003 2022-03-03 08:54:42.000000 marlenvs-1.0.7/marlenvs/navigation_env/navigation_env.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2022-03-03 08:58:26.449971 marlenvs-1.0.7/marlenvs/switch_env/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       53 2022-02-02 10:03:25.000000 marlenvs-1.0.7/marlenvs/switch_env/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     9678 2022-02-24 10:17:53.000000 marlenvs-1.0.7/marlenvs/switch_env/switch_env.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2022-03-03 08:58:26.449971 marlenvs-1.0.7/marlenvs/two_step_env/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       58 2022-02-02 10:03:42.000000 marlenvs-1.0.7/marlenvs/two_step_env/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2954 2022-02-04 16:32:45.000000 marlenvs-1.0.7/marlenvs/two_step_env/two_step_env.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1681 2022-02-23 10:33:12.000000 marlenvs-1.0.7/marlenvs/wrappers.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2022-03-03 08:58:26.445971 marlenvs-1.0.7/marlenvs.egg-info/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      211 2022-03-03 08:58:26.000000 marlenvs-1.0.7/marlenvs.egg-info/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      443 2022-03-03 08:58:26.000000 marlenvs-1.0.7/marlenvs.egg-info/SOURCES.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2022-03-03 08:58:26.000000 marlenvs-1.0.7/marlenvs.egg-info/dependency_links.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       30 2022-03-03 08:58:26.000000 marlenvs-1.0.7/marlenvs.egg-info/requires.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        9 2022-03-03 08:58:26.000000 marlenvs-1.0.7/marlenvs.egg-info/top_level.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       38 2022-03-03 08:58:26.449971 marlenvs-1.0.7/setup.cfg
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      329 2022-03-03 08:58:19.000000 marlenvs-1.0.7/setup.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2022-03-03 09:04:18.480239 marlenvs-1.0.8/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1069 2022-01-10 11:58:33.000000 marlenvs-1.0.8/LICENSE
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      211 2022-03-03 09:04:18.480239 marlenvs-1.0.8/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1807 2022-02-06 16:05:06.000000 marlenvs-1.0.8/README.md
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2022-03-03 09:04:18.476239 marlenvs-1.0.8/marlenvs/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      270 2022-02-02 12:21:55.000000 marlenvs-1.0.8/marlenvs/__init__.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2022-03-03 09:04:18.480239 marlenvs-1.0.8/marlenvs/navigation_env/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       65 2022-02-02 10:04:20.000000 marlenvs-1.0.8/marlenvs/navigation_env/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     9020 2022-03-03 09:03:35.000000 marlenvs-1.0.8/marlenvs/navigation_env/navigation_env.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2022-03-03 09:04:18.480239 marlenvs-1.0.8/marlenvs/switch_env/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       53 2022-02-02 10:03:25.000000 marlenvs-1.0.8/marlenvs/switch_env/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     9678 2022-02-24 10:17:53.000000 marlenvs-1.0.8/marlenvs/switch_env/switch_env.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2022-03-03 09:04:18.480239 marlenvs-1.0.8/marlenvs/two_step_env/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       58 2022-02-02 10:03:42.000000 marlenvs-1.0.8/marlenvs/two_step_env/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2954 2022-02-04 16:32:45.000000 marlenvs-1.0.8/marlenvs/two_step_env/two_step_env.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1681 2022-02-23 10:33:12.000000 marlenvs-1.0.8/marlenvs/wrappers.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2022-03-03 09:04:18.476239 marlenvs-1.0.8/marlenvs.egg-info/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      211 2022-03-03 09:04:18.000000 marlenvs-1.0.8/marlenvs.egg-info/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      443 2022-03-03 09:04:18.000000 marlenvs-1.0.8/marlenvs.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2022-03-03 09:04:18.000000 marlenvs-1.0.8/marlenvs.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       30 2022-03-03 09:04:18.000000 marlenvs-1.0.8/marlenvs.egg-info/requires.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        9 2022-03-03 09:04:18.000000 marlenvs-1.0.8/marlenvs.egg-info/top_level.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       38 2022-03-03 09:04:18.480239 marlenvs-1.0.8/setup.cfg
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      329 2022-03-03 09:04:05.000000 marlenvs-1.0.8/setup.py
```

### Comparing `marlenvs-1.0.7/LICENSE` & `marlenvs-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `marlenvs-1.0.7/README.md` & `marlenvs-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `marlenvs-1.0.7/marlenvs/navigation_env/navigation_env.py` & `marlenvs-1.0.8/marlenvs/navigation_env/navigation_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,17 +233,18 @@
 			return int((100*coordinates)//4)
 		elif isinstance(coordinates, list):
 			return [int((c*100)//4) for c in coordinates]
 		elif isinstance(coordinates, tuple):
 			return (int((c*100)//4) for c in coordinates)
 
 	def close(self):
-		if self.viewer:
-			self.viewer.close()
-			self.viewer = None
+		if self.screen:
+			self.surface = None
+			self.screen = None
+			pygame.quit()
 
 	def get_obs_dim(self):
 		return self.n_agents*4 - 2
 
 	def get_act_dim(self):
 		return 2
```

### Comparing `marlenvs-1.0.7/marlenvs/switch_env/switch_env.py` & `marlenvs-1.0.8/marlenvs/switch_env/switch_env.py`

 * *Files identical despite different names*

### Comparing `marlenvs-1.0.7/marlenvs/two_step_env/two_step_env.py` & `marlenvs-1.0.8/marlenvs/two_step_env/two_step_env.py`

 * *Files identical despite different names*

### Comparing `marlenvs-1.0.7/marlenvs/wrappers.py` & `marlenvs-1.0.8/marlenvs/wrappers.py`

 * *Files identical despite different names*

