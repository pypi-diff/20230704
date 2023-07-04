# Comparing `tmp/PyFakeDados-0.0.5.2.tar.gz` & `tmp/PyFakeDados-0.0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFakeDados-0.0.5.2.tar", last modified: Mon Jul  3 01:04:56 2023, max compression
+gzip compressed data, was "PyFakeDados-0.0.5.3.tar", last modified: Tue Jul  4 01:18:14 2023, max compression
```

## Comparing `PyFakeDados-0.0.5.2.tar` & `PyFakeDados-0.0.5.3.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-07-03 01:04:56.811155 PyFakeDados-0.0.5.2/
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)    35148 2023-06-29 22:25:25.000000 PyFakeDados-0.0.5.2/LICENSE.txt
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       29 2023-06-30 02:34:23.000000 PyFakeDados-0.0.5.2/MANIFEST.in
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     3406 2023-07-03 01:04:56.811155 PyFakeDados-0.0.5.2/PKG-INFO
-drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-07-03 01:04:56.811155 PyFakeDados-0.0.5.2/PyFakeDados/
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)   922861 2023-07-03 00:37:28.000000 PyFakeDados-0.0.5.2/PyFakeDados/CONSTANTS.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       23 2023-07-03 01:02:38.000000 PyFakeDados-0.0.5.2/PyFakeDados/__init__.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      857 2023-06-29 22:47:13.000000 PyFakeDados-0.0.5.2/PyFakeDados/bairro.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1661 2023-06-30 03:02:42.000000 PyFakeDados-0.0.5.2/PyFakeDados/cep.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1771 2023-06-29 23:29:37.000000 PyFakeDados-0.0.5.2/PyFakeDados/cnpj.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1487 2023-06-29 23:59:11.000000 PyFakeDados-0.0.5.2/PyFakeDados/cpf.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      177 2023-06-30 00:10:57.000000 PyFakeDados-0.0.5.2/PyFakeDados/ctps.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      823 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.2/PyFakeDados/email.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     5250 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.2/PyFakeDados/empresa.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      489 2023-07-03 00:41:15.000000 PyFakeDados-0.0.5.2/PyFakeDados/estado.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      164 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.2/PyFakeDados/inscricao_estadual.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      798 2023-06-29 22:57:01.000000 PyFakeDados-0.0.5.2/PyFakeDados/logradouro.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      446 2023-07-03 00:29:57.000000 PyFakeDados-0.0.5.2/PyFakeDados/municipio.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     3278 2023-06-30 00:32:32.000000 PyFakeDados-0.0.5.2/PyFakeDados/nome.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2872 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.2/PyFakeDados/pessoa.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      170 2023-06-30 00:12:54.000000 PyFakeDados-0.0.5.2/PyFakeDados/pis.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      630 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.2/PyFakeDados/rg.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      389 2023-06-30 00:36:02.000000 PyFakeDados-0.0.5.2/PyFakeDados/senha.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      399 2023-06-30 03:01:14.000000 PyFakeDados-0.0.5.2/PyFakeDados/site.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1820 2023-06-30 03:00:58.000000 PyFakeDados-0.0.5.2/PyFakeDados/telefone.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2119 2023-07-03 00:42:12.000000 PyFakeDados-0.0.5.2/PyFakeDados/utils.py
-drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-07-03 01:04:56.811155 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     3406 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/PKG-INFO
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      725 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/SOURCES.txt
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)        1 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/dependency_links.txt
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)        1 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/not-zip-safe
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       10 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/requires.txt
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       12 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.2/PyFakeDados.egg-info/top_level.txt
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2777 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.2/README.md
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      819 2023-07-03 01:04:56.811155 PyFakeDados-0.0.5.2/setup.cfg
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       38 2023-06-29 22:25:25.000000 PyFakeDados-0.0.5.2/setup.py
+drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-07-04 01:18:14.081434 PyFakeDados-0.0.5.3/
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)    35148 2023-06-29 22:25:25.000000 PyFakeDados-0.0.5.3/LICENSE.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       29 2023-06-30 02:34:23.000000 PyFakeDados-0.0.5.3/MANIFEST.in
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     3406 2023-07-04 01:18:14.081434 PyFakeDados-0.0.5.3/PKG-INFO
+drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-07-04 01:18:14.081434 PyFakeDados-0.0.5.3/PyFakeDados/
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)   922862 2023-07-04 01:10:17.000000 PyFakeDados-0.0.5.3/PyFakeDados/CONSTANTS.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       23 2023-07-04 01:17:17.000000 PyFakeDados-0.0.5.3/PyFakeDados/__init__.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      857 2023-06-29 22:47:13.000000 PyFakeDados-0.0.5.3/PyFakeDados/bairro.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1661 2023-06-30 03:02:42.000000 PyFakeDados-0.0.5.3/PyFakeDados/cep.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1771 2023-06-29 23:29:37.000000 PyFakeDados-0.0.5.3/PyFakeDados/cnpj.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1487 2023-06-29 23:59:11.000000 PyFakeDados-0.0.5.3/PyFakeDados/cpf.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      177 2023-06-30 00:10:57.000000 PyFakeDados-0.0.5.3/PyFakeDados/ctps.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      823 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.3/PyFakeDados/email.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     5250 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.3/PyFakeDados/empresa.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1257 2023-07-04 01:13:47.000000 PyFakeDados-0.0.5.3/PyFakeDados/endereco.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      489 2023-07-03 00:41:15.000000 PyFakeDados-0.0.5.3/PyFakeDados/estado.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      164 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.3/PyFakeDados/inscricao_estadual.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      798 2023-06-29 22:57:01.000000 PyFakeDados-0.0.5.3/PyFakeDados/logradouro.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      446 2023-07-03 00:29:57.000000 PyFakeDados-0.0.5.3/PyFakeDados/municipio.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     3278 2023-06-30 00:32:32.000000 PyFakeDados-0.0.5.3/PyFakeDados/nome.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2872 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.3/PyFakeDados/pessoa.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      170 2023-06-30 00:12:54.000000 PyFakeDados-0.0.5.3/PyFakeDados/pis.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      630 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.3/PyFakeDados/rg.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      389 2023-06-30 00:36:02.000000 PyFakeDados-0.0.5.3/PyFakeDados/senha.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      399 2023-06-30 03:01:14.000000 PyFakeDados-0.0.5.3/PyFakeDados/site.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1820 2023-06-30 03:00:58.000000 PyFakeDados-0.0.5.3/PyFakeDados/telefone.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2119 2023-07-03 00:42:12.000000 PyFakeDados-0.0.5.3/PyFakeDados/utils.py
+drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-07-04 01:18:14.081434 PyFakeDados-0.0.5.3/PyFakeDados.egg-info/
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     3406 2023-07-04 01:18:14.000000 PyFakeDados-0.0.5.3/PyFakeDados.egg-info/PKG-INFO
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      749 2023-07-04 01:18:14.000000 PyFakeDados-0.0.5.3/PyFakeDados.egg-info/SOURCES.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)        1 2023-07-04 01:18:14.000000 PyFakeDados-0.0.5.3/PyFakeDados.egg-info/dependency_links.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)        1 2023-07-03 01:04:56.000000 PyFakeDados-0.0.5.3/PyFakeDados.egg-info/not-zip-safe
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       10 2023-07-04 01:18:14.000000 PyFakeDados-0.0.5.3/PyFakeDados.egg-info/requires.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       12 2023-07-04 01:18:14.000000 PyFakeDados-0.0.5.3/PyFakeDados.egg-info/top_level.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2777 2023-07-01 18:01:17.000000 PyFakeDados-0.0.5.3/README.md
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      819 2023-07-04 01:18:14.085435 PyFakeDados-0.0.5.3/setup.cfg
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       38 2023-06-29 22:25:25.000000 PyFakeDados-0.0.5.3/setup.py
```

### Comparing `PyFakeDados-0.0.5.2/LICENSE.txt` & `PyFakeDados-0.0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PKG-INFO` & `PyFakeDados-0.0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFakeDados
-Version: 0.0.5.2
+Version: 0.0.5.3
 Summary: Generic generator fake data for application and api development.
 Home-page: https://github.com/juliansantosinfo/PyFakeDados
 Author: Julian de Almeida Santos
 Author-email: julian.santos.info@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
 Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
```

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/CONSTANTS.py` & `PyFakeDados-0.0.5.3/PyFakeDados/CONSTANTS.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17535,8 +17535,8 @@
         "Varjão",
         "Vianópolis",
         "Vicentinópolis",
         "Vila Boa",
         "Vila Propício",
     ],
     "DF": ["Brasília"],
-}
+}
```

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/bairro.py` & `PyFakeDados-0.0.5.3/PyFakeDados/bairro.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/cep.py` & `PyFakeDados-0.0.5.3/PyFakeDados/cep.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/cnpj.py` & `PyFakeDados-0.0.5.3/PyFakeDados/cnpj.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/cpf.py` & `PyFakeDados-0.0.5.3/PyFakeDados/cpf.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/email.py` & `PyFakeDados-0.0.5.3/PyFakeDados/email.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/empresa.py` & `PyFakeDados-0.0.5.3/PyFakeDados/empresa.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/logradouro.py` & `PyFakeDados-0.0.5.3/PyFakeDados/logradouro.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/nome.py` & `PyFakeDados-0.0.5.3/PyFakeDados/nome.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/pessoa.py` & `PyFakeDados-0.0.5.3/PyFakeDados/pessoa.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/rg.py` & `PyFakeDados-0.0.5.3/PyFakeDados/rg.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/telefone.py` & `PyFakeDados-0.0.5.3/PyFakeDados/telefone.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados/utils.py` & `PyFakeDados-0.0.5.3/PyFakeDados/utils.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados.egg-info/PKG-INFO` & `PyFakeDados-0.0.5.3/PyFakeDados.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFakeDados
-Version: 0.0.5.2
+Version: 0.0.5.3
 Summary: Generic generator fake data for application and api development.
 Home-page: https://github.com/juliansantosinfo/PyFakeDados
 Author: Julian de Almeida Santos
 Author-email: julian.santos.info@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
 Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
```

### Comparing `PyFakeDados-0.0.5.2/PyFakeDados.egg-info/SOURCES.txt` & `PyFakeDados-0.0.5.3/PyFakeDados.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 PyFakeDados/bairro.py
 PyFakeDados/cep.py
 PyFakeDados/cnpj.py
 PyFakeDados/cpf.py
 PyFakeDados/ctps.py
 PyFakeDados/email.py
 PyFakeDados/empresa.py
+PyFakeDados/endereco.py
 PyFakeDados/estado.py
 PyFakeDados/inscricao_estadual.py
 PyFakeDados/logradouro.py
 PyFakeDados/municipio.py
 PyFakeDados/nome.py
 PyFakeDados/pessoa.py
 PyFakeDados/pis.py
```

### Comparing `PyFakeDados-0.0.5.2/README.md` & `PyFakeDados-0.0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5.2/setup.cfg` & `PyFakeDados-0.0.5.3/setup.cfg`

 * *Files identical despite different names*

