# Comparing `tmp/lealnumeros-0.0.6.3.1.tar.gz` & `tmp/lealnumeros-1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lealnumeros-0.0.6.3.1.tar", last modified: Thu May 18 19:39:43 2023, max compression
+gzip compressed data, was "lealnumeros-1.tar", last modified: Tue Jul  4 21:53:09 2023, max compression
```

## Comparing `lealnumeros-0.0.6.3.1.tar` & `lealnumeros-1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 19:39:43.107996 lealnumeros-0.0.6.3.1/
--rw-rw-rw-   0        0        0     1098 2023-05-18 19:18:17.000000 lealnumeros-0.0.6.3.1/LICENCE
--rw-rw-rw-   0        0        0     1991 2023-05-18 19:39:43.106996 lealnumeros-0.0.6.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1665 2023-05-18 19:20:23.000000 lealnumeros-0.0.6.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 19:39:43.067020 lealnumeros-0.0.6.3.1/lealNumeros/
--rw-rw-rw-   0        0        0       32 2023-05-18 19:18:17.000000 lealnumeros-0.0.6.3.1/lealNumeros/__init__.py
--rw-rw-rw-   0        0        0     4650 2023-05-18 19:29:01.000000 lealnumeros-0.0.6.3.1/lealNumeros/main.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:39:43.105997 lealnumeros-0.0.6.3.1/lealnumeros.egg-info/
--rw-rw-rw-   0        0        0     1991 2023-05-18 19:39:42.000000 lealnumeros-0.0.6.3.1/lealnumeros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-18 19:39:42.000000 lealnumeros-0.0.6.3.1/lealnumeros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 19:39:42.000000 lealnumeros-0.0.6.3.1/lealnumeros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-18 19:39:42.000000 lealnumeros-0.0.6.3.1/lealnumeros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-18 19:39:42.000000 lealnumeros-0.0.6.3.1/lealnumeros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 19:39:43.107996 lealnumeros-0.0.6.3.1/setup.cfg
--rw-rw-rw-   0        0        0      534 2023-05-18 19:39:06.000000 lealnumeros-0.0.6.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:53:09.205508 lealnumeros-1/
+-rw-rw-rw-   0        0        0     1098 2023-05-18 19:18:17.000000 lealnumeros-1/LICENCE
+-rw-rw-rw-   0        0        0     1901 2023-07-04 21:53:09.200502 lealnumeros-1/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2023-07-04 21:51:07.000000 lealnumeros-1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 21:53:09.150533 lealnumeros-1/lealNumeros/
+-rw-rw-rw-   0        0        0       32 2023-05-18 19:18:17.000000 lealnumeros-1/lealNumeros/__init__.py
+-rw-rw-rw-   0        0        0     5029 2023-07-03 19:07:38.000000 lealnumeros-1/lealNumeros/main.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:53:09.198506 lealnumeros-1/lealnumeros.egg-info/
+-rw-rw-rw-   0        0        0     1901 2023-07-04 21:53:08.000000 lealnumeros-1/lealnumeros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-04 21:53:09.000000 lealnumeros-1/lealnumeros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 21:53:08.000000 lealnumeros-1/lealnumeros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-04 21:53:08.000000 lealnumeros-1/lealnumeros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-04 21:53:08.000000 lealnumeros-1/lealnumeros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 21:53:09.206500 lealnumeros-1/setup.cfg
+-rw-rw-rw-   0        0        0      526 2023-07-04 21:53:01.000000 lealnumeros-1/setup.py
```

### Comparing `lealnumeros-0.0.6.3.1/LICENCE` & `lealnumeros-1/LICENCE`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.6.3.1/PKG-INFO` & `lealnumeros-1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: lealnumeros
-Version: 0.0.6.3.1
+Version: 1
 Summary: Trabalhe com formatação de números de uma maneira rápido e fácil.
 Author: José Rodolfo
 Author-email: silvaleal.ctt@gmail.com
 License: MIT License
 Keywords: lealnumeros
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-Trabalhe com formataÃ§Ã£o de nÃºmeros de uma maneira rÃ¡pido e fÃ¡cil.
 
 ```python
 from lealNumeros import LealNumerosAPI
 
 # Put punctuation in numbers
 print(LealNumerosAPI.numerosPontuados(10000))
 # Output: 10.000
```

### Comparing `lealnumeros-0.0.6.3.1/README.md` & `lealnumeros-1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-Trabalhe com formatação de números de uma maneira rápido e fácil.
 
 ```python
 from lealNumeros import LealNumerosAPI
 
 # Put punctuation in numbers
 print(LealNumerosAPI.numerosPontuados(10000))
 # Output: 10.000
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lealnumeros-0.0.6.3.1/lealNumeros/main.py` & `lealnumeros-1/lealNumeros/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,37 +78,52 @@
             numero_formatado = f'{numero_str[:-21]}Sx'
 
         else:
             numero_formatado = f'{numero_str[:-24]}Sp'
             
         return numero_formatado
 
-    def numerosNome(numero, lang = 'pt-BR'):
-        numero_nome = num2words(numero, lang=lang)
-        numero_nome = numero_nome.capitalize()
+    def numerosNome(numero, lang = 'en'):
+        try:
+            numero = int(numero)
 
-        return numero_nome
+            numero_nome = num2words(numero, lang=lang)
+            numero_nome = numero_nome.capitalize()
+
+
+            return numero_nome
+
+        except Exception as error:
+            return error
+
+
+
+        # if type(numero) == int:
+        #     numero_nome = num2words(numero, lang=lang)
+        #     numero_nome = numero_nome.capitalize()
+
+        #     return numero_nome
+        # else:
+        #     return 'Invalid number'
 
     def numerosDiferenca(numero_um, numero_dois):
+
         if numero_um > numero_dois: # Se o 'numero_um' for maior que o 'numero_dois'
             resposta = numero_um - numero_dois
 
-        elif numero_um < numero_dois: # Se o 'numero_dois' for maior que o 'numero_um'
+        else: # Se o 'numero_dois' for maior que o 'numero_um'
             resposta = numero_dois - numero_um
 
-        else:
-            resposta = 0 # Caso os números forem iguais.
-
-        return 
+        return resposta
 
     def numerosCalculadora(conta):
 
         # Simplificar para quem utilizar
         conta = conta.split()
-
+        
         numero_um = int(conta[0])
         operador = str(conta[1])
         numero_dois = int(conta[2])
 
         # Código...
         operadores = ['+','-','*','/']
 
@@ -126,13 +141,15 @@
             
         else:
             return 'Operator not found.'
 
     # Verificar a diferença de dias.
     def dataDiferenca(dia, mes, ano):
         formato = '%d/%m/&Y'
+        
         data_registrada = datetime.strptime(f'{int(dia)}/{int(mes)}/{int(ano)}', '%d/%m/%Y') # Pegar a data da ação (registro, punição e ect...)
         data_atual = datetime.now() # Pegar data atual (quando o código acontecer)
 
-        dia = str(data_atual - data_registrada)
+        dias_diferença = str(data_atual - data_registrada).split()
+        # dias_diferença = int(dias_diferença)
 
-        return dia[:3]
+        return dias_diferença[0]
```

### Comparing `lealnumeros-0.0.6.3.1/lealnumeros.egg-info/PKG-INFO` & `lealnumeros-1/lealnumeros.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: lealnumeros
-Version: 0.0.6.3.1
+Version: 1
 Summary: Trabalhe com formatação de números de uma maneira rápido e fácil.
 Author: José Rodolfo
 Author-email: silvaleal.ctt@gmail.com
 License: MIT License
 Keywords: lealnumeros
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-Trabalhe com formataÃ§Ã£o de nÃºmeros de uma maneira rÃ¡pido e fÃ¡cil.
 
 ```python
 from lealNumeros import LealNumerosAPI
 
 # Put punctuation in numbers
 print(LealNumerosAPI.numerosPontuados(10000))
 # Output: 10.000
```

