# Comparing `tmp/viggonuvemfiscal-1.1.2.tar.gz` & `tmp/viggonuvemfiscal-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggonuvemfiscal-1.1.2.tar", last modified: Tue May 30 16:45:22 2023, max compression
+gzip compressed data, was "viggonuvemfiscal-1.1.3.tar", last modified: Tue Jul  4 15:54:13 2023, max compression
```

## Comparing `viggonuvemfiscal-1.1.2.tar` & `viggonuvemfiscal-1.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.572012 viggonuvemfiscal-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-30 16:45:22.572012 viggonuvemfiscal-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:45:22.572012 viggonuvemfiscal-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.568011 viggonuvemfiscal-1.1.2/viggonuvemfiscal/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.568011 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.568011 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.568011 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.572012 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    18828 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.568011 viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-30 16:45:22.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-30 16:45:22.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:45:22.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-30 16:45:22.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 16:45:22.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:54:13.712555 viggonuvemfiscal-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-04 15:54:13.712555 viggonuvemfiscal-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 15:54:13.712555 viggonuvemfiscal-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:54:13.712555 viggonuvemfiscal-1.1.3/viggonuvemfiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:54:13.712555 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:54:13.712555 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:54:13.712555 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:54:13.712555 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18904 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-04 15:53:22.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:54:13.712555 viggonuvemfiscal-1.1.3/viggonuvemfiscal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-04 15:54:13.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-04 15:54:13.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:54:13.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-04 15:54:13.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 15:54:13.000000 viggonuvemfiscal-1.1.3/viggonuvemfiscal.egg-info/top_level.txt
```

### Comparing `viggonuvemfiscal-1.1.2/viggonuvemfiscal/__init__.py` & `viggonuvemfiscal-1.1.3/viggonuvemfiscal/__init__.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.2/viggonuvemfiscal/resources.py` & `viggonuvemfiscal-1.1.3/viggonuvemfiscal/resources.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py` & `viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,12 +31,12 @@
         self.create = Create(self)
         self.update = Update(self)
 
     def get_configuracao_nuvem_fiscal(
             self, tipo: cnf_tipo = cnf_tipo.PRODUCAO):
         configs = self.list(tipo=tipo.name)
         if len(configs) == 0:
-            raise exception.NotFound(
+            raise exception.BadRequest(
                 'Nenhuma configuração da Nuvem Fiscal cadastrada para o ' +
                 f'tipo {tipo.name}, por favor ' +
                 'cadastre uma para usar a api.')
         return configs[0]
```

### Comparing `viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py` & `viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py` & `viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py` & `viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py` & `viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,16 @@
         return self.manager.executar_requisicao('GET', url, ambiente=ambiente)
 
 
 class BaixarPdfDanfeNfce(operation.List):
 
     def do(self, session, **kwargs):
         ambiente = kwargs.pop('api_fiscal', cnf_tipo.HOMOLOGACAO)
+        if type(ambiente) == str:
+            ambiente = cnf_tipo[ambiente]
         nfce_id = self.manager.get_nfce_id(**kwargs)
         url = self.manager.get_endpoint(
             f'/nfce/{nfce_id}/pdf', ambiente)
         return self.manager.executar_requisicao('GET', url, ambiente=ambiente)
 
 
 class ConsultarCancelamentoNfce(operation.List):
```

### Comparing `viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py` & `viggonuvemfiscal-1.1.3/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/SOURCES.txt` & `viggonuvemfiscal-1.1.3/viggonuvemfiscal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

