# Comparing `tmp/torch-pp-0.0.7.dev0.tar.gz` & `tmp/torch-pp-0.0.8.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-pp-0.0.7.dev0.tar", last modified: Thu Jun  1 18:20:26 2023, max compression
+gzip compressed data, was "torch-pp-0.0.8.dev0.tar", last modified: Thu Jun  1 18:22:31 2023, max compression
```

## Comparing `torch-pp-0.0.7.dev0.tar` & `torch-pp-0.0.8.dev0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 18:20:26.928705 torch-pp-0.0.7.dev0/
--rw-rw-r--   0 roman     (1000) roman     (1000)     1069 2023-05-19 17:45:40.000000 torch-pp-0.0.7.dev0/LICENSE
--rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-06-01 18:20:26.928705 torch-pp-0.0.7.dev0/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)       68 2023-05-20 02:43:14.000000 torch-pp-0.0.7.dev0/README.md
--rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-06-01 18:20:26.928705 torch-pp-0.0.7.dev0/setup.cfg
--rw-rw-r--   0 roman     (1000) roman     (1000)      307 2023-06-01 18:19:42.000000 torch-pp-0.0.7.dev0/setup.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 18:20:26.928705 torch-pp-0.0.7.dev0/torch_pp/
--rw-rw-r--   0 roman     (1000) roman     (1000)       43 2023-05-20 02:43:14.000000 torch-pp-0.0.7.dev0/torch_pp/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     3950 2023-06-01 18:19:25.000000 torch-pp-0.0.7.dev0/torch_pp/standardscaler.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      199 2023-05-20 19:59:15.000000 torch-pp-0.0.7.dev0/torch_pp/test_.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 18:20:26.928705 torch-pp-0.0.7.dev0/torch_pp.egg-info/
--rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-06-01 18:20:26.000000 torch-pp-0.0.7.dev0/torch_pp.egg-info/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)      220 2023-06-01 18:20:26.000000 torch-pp-0.0.7.dev0/torch_pp.egg-info/SOURCES.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-06-01 18:20:26.000000 torch-pp-0.0.7.dev0/torch_pp.egg-info/dependency_links.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        9 2023-06-01 18:20:26.000000 torch-pp-0.0.7.dev0/torch_pp.egg-info/top_level.txt
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 18:22:31.587424 torch-pp-0.0.8.dev0/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1069 2023-05-19 17:45:40.000000 torch-pp-0.0.8.dev0/LICENSE
+-rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-06-01 18:22:31.583424 torch-pp-0.0.8.dev0/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)       68 2023-05-20 02:43:14.000000 torch-pp-0.0.8.dev0/README.md
+-rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-06-01 18:22:31.587424 torch-pp-0.0.8.dev0/setup.cfg
+-rw-rw-r--   0 roman     (1000) roman     (1000)      307 2023-06-01 18:22:29.000000 torch-pp-0.0.8.dev0/setup.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 18:22:31.583424 torch-pp-0.0.8.dev0/torch_pp/
+-rw-rw-r--   0 roman     (1000) roman     (1000)       43 2023-05-20 02:43:14.000000 torch-pp-0.0.8.dev0/torch_pp/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3968 2023-06-01 18:22:23.000000 torch-pp-0.0.8.dev0/torch_pp/standardscaler.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      199 2023-05-20 19:59:15.000000 torch-pp-0.0.8.dev0/torch_pp/test_.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 18:22:31.583424 torch-pp-0.0.8.dev0/torch_pp.egg-info/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-06-01 18:22:31.000000 torch-pp-0.0.8.dev0/torch_pp.egg-info/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)      220 2023-06-01 18:22:31.000000 torch-pp-0.0.8.dev0/torch_pp.egg-info/SOURCES.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-06-01 18:22:31.000000 torch-pp-0.0.8.dev0/torch_pp.egg-info/dependency_links.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        9 2023-06-01 18:22:31.000000 torch-pp-0.0.8.dev0/torch_pp.egg-info/top_level.txt
```

### Comparing `torch-pp-0.0.7.dev0/LICENSE` & `torch-pp-0.0.8.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-pp-0.0.7.dev0/torch_pp/standardscaler.py` & `torch-pp-0.0.8.dev0/torch_pp/standardscaler.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,20 @@
         self.mean, self.var, self.n_samples_seen = incremental_mean_and_var(x, self.mean, self.var, self.n_samples_seen)
 
         self.scale = torch.where(self.var != 0, self.var, torch.ones(self.var.shape))
         # self.scale = self.var.apply_(conditional_)
         self.scale = torch.sqrt(self.scale)
 
     def transform(self, x: torch.Tensor):
-        return self.__transform(x, forward_)
+        return self.transform_proceed(x, forward_)
 
     def inverse_transform(self, x: torch.Tensor):
-        return self.__transform(x, inverse_)
+        return self.transform_proceed(x, inverse_)
 
-    def __transform(self, x: torch.Tensor, fn):
+    def transform_proceed(self, x: torch.Tensor, fn):
         x_out = x.clone()
         n_features = x.shape[1]
         for i in range(n_features):
             mean, scale = 0., 1.
             if self.with_mean:
                 mean = self.mean[i]
             if self.with_std:
```

