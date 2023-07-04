# Comparing `tmp/pydantic_br-0.3.0.tar.gz` & `tmp/pydantic_br-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_br-0.3.0.tar", max compression
+gzip compressed data, was "pydantic_br-0.4.0.tar", max compression
```

## Comparing `pydantic_br-0.3.0.tar` & `pydantic_br-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1090 2023-03-27 13:26:17.201060 pydantic_br-0.3.0/LICENSE
--rw-r--r--   0        0        0      452 2023-04-22 02:05:24.594119 pydantic_br-0.3.0/pydantic_br/__init__.py
--rw-r--r--   0        0        0      718 2023-04-01 15:44:31.545140 pydantic_br-0.3.0/pydantic_br/field_erros.py
--rw-r--r--   0        0        0     1970 2023-04-22 02:48:54.995154 pydantic_br-0.3.0/pydantic_br/fields/base_field.py
--rw-r--r--   0        0        0      307 2023-04-22 02:55:17.245254 pydantic_br-0.3.0/pydantic_br/fields/cnh_field.py
--rw-r--r--   0        0        0      786 2023-04-22 02:55:17.245254 pydantic_br-0.3.0/pydantic_br/fields/cnpj_field.py
--rw-r--r--   0        0        0      778 2023-04-22 02:55:17.245254 pydantic_br-0.3.0/pydantic_br/fields/cpf_field.py
--rw-r--r--   0        0        0      733 2023-04-22 02:28:55.870250 pydantic_br-0.3.0/pydantic_br/fields/pis_field.py
--rw-r--r--   0        0        0      308 2023-04-22 02:55:17.246262 pydantic_br-0.3.0/pydantic_br/fields/te_field.py
--rw-r--r--   0        0        0      226 2023-04-22 02:40:51.452781 pydantic_br-0.3.0/pydantic_br/validators/base_validator.py
--rw-r--r--   0        0        0     1266 2023-04-22 02:55:17.246262 pydantic_br-0.3.0/pydantic_br/validators/cnh_validator.py
--rw-r--r--   0        0        0     1715 2023-04-22 02:55:17.246262 pydantic_br-0.3.0/pydantic_br/validators/cnpj_validator.py
--rw-r--r--   0        0        0     1318 2023-04-22 02:55:17.247269 pydantic_br-0.3.0/pydantic_br/validators/cpf_validator.py
--rw-r--r--   0        0        0     1151 2023-04-22 02:49:26.506208 pydantic_br-0.3.0/pydantic_br/validators/pis_validator.py
--rw-r--r--   0        0        0     1945 2023-04-22 02:55:17.247269 pydantic_br-0.3.0/pydantic_br/validators/te_validator.py
--rw-r--r--   0        0        0     1740 2023-04-22 02:01:05.454342 pydantic_br-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3957 2023-04-22 01:45:04.888335 pydantic_br-0.3.0/README.md
--rw-r--r--   0        0        0     5061 1970-01-01 00:00:00.000000 pydantic_br-0.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1090 2023-03-27 13:26:17.201060 pydantic_br-0.4.0/LICENSE
+-rwxr-xr-x   0        0        0     3951 2023-07-04 01:13:14.992490 pydantic_br-0.4.0/README.md
+-rwxr-xr-x   0        0        0      560 2023-07-04 01:28:30.333645 pydantic_br-0.4.0/pydantic_br/__init__.py
+-rwxr-xr-x   0        0        0      718 2023-04-01 15:44:31.545140 pydantic_br-0.4.0/pydantic_br/field_erros.py
+-rwxr-xr-x   0        0        0     1970 2023-04-22 02:48:54.995154 pydantic_br-0.4.0/pydantic_br/fields/base_field.py
+-rwxr-xr-x   0        0        0      821 2023-07-04 00:24:53.925695 pydantic_br-0.4.0/pydantic_br/fields/certidao_field.py
+-rwxr-xr-x   0        0        0      307 2023-04-22 02:55:17.245254 pydantic_br-0.4.0/pydantic_br/fields/cnh_field.py
+-rwxr-xr-x   0        0        0      786 2023-04-22 02:55:17.245254 pydantic_br-0.4.0/pydantic_br/fields/cnpj_field.py
+-rwxr-xr-x   0        0        0      778 2023-05-08 23:01:18.303826 pydantic_br-0.4.0/pydantic_br/fields/cpf_field.py
+-rwxr-xr-x   0        0        0      733 2023-04-22 02:28:55.870250 pydantic_br-0.4.0/pydantic_br/fields/pis_field.py
+-rwxr-xr-x   0        0        0      308 2023-04-22 02:55:17.246262 pydantic_br-0.4.0/pydantic_br/fields/te_field.py
+-rwxr-xr-x   0        0        0      226 2023-04-22 02:40:51.452781 pydantic_br-0.4.0/pydantic_br/validators/base_validator.py
+-rwxr-xr-x   0        0        0     1688 2023-07-04 00:41:54.342703 pydantic_br-0.4.0/pydantic_br/validators/certidao_validator.py
+-rwxr-xr-x   0        0        0     1266 2023-04-22 02:55:17.246262 pydantic_br-0.4.0/pydantic_br/validators/cnh_validator.py
+-rwxr-xr-x   0        0        0     1715 2023-04-22 02:55:17.246262 pydantic_br-0.4.0/pydantic_br/validators/cnpj_validator.py
+-rwxr-xr-x   0        0        0     1318 2023-04-22 02:55:17.247269 pydantic_br-0.4.0/pydantic_br/validators/cpf_validator.py
+-rwxr-xr-x   0        0        0     1151 2023-04-22 02:49:26.506208 pydantic_br-0.4.0/pydantic_br/validators/pis_validator.py
+-rwxr-xr-x   0        0        0     1945 2023-04-22 02:55:17.247269 pydantic_br-0.4.0/pydantic_br/validators/te_validator.py
+-rwxr-xr-x   0        0        0     1740 2023-07-04 01:14:13.946749 pydantic_br-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 pydantic_br-0.4.0/PKG-INFO
```

### Comparing `pydantic_br-0.3.0/LICENSE` & `pydantic_br-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.3.0/pydantic_br/field_erros.py` & `pydantic_br-0.4.0/pydantic_br/field_erros.py`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.3.0/pydantic_br/fields/base_field.py` & `pydantic_br-0.4.0/pydantic_br/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.3.0/pydantic_br/fields/cnpj_field.py` & `pydantic_br-0.4.0/pydantic_br/fields/cnpj_field.py`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.3.0/pydantic_br/fields/cpf_field.py` & `pydantic_br-0.4.0/pydantic_br/fields/cpf_field.py`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.3.0/pydantic_br/fields/pis_field.py` & `pydantic_br-0.4.0/pydantic_br/fields/pis_field.py`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.3.0/pydantic_br/validators/cnh_validator.py` & `pydantic_br-0.4.0/pydantic_br/validators/cnh_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.3.0/pydantic_br/validators/cnpj_validator.py` & `pydantic_br-0.4.0/pydantic_br/validators/cnpj_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.3.0/pydantic_br/validators/cpf_validator.py` & `pydantic_br-0.4.0/pydantic_br/validators/cpf_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.3.0/pydantic_br/validators/pis_validator.py` & `pydantic_br-0.4.0/pydantic_br/validators/pis_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.3.0/pydantic_br/validators/te_validator.py` & `pydantic_br-0.4.0/pydantic_br/validators/te_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic_br-0.3.0/pyproject.toml` & `pydantic_br-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-br"
-version = "0.3.0"
+version = "0.4.0"
 description = "Pydantic library extension with Brazilian fields"
 license = "MIT"
 authors = ["Jorge Silva <jorgesilva.ti@hotmail.com>"]
 maintainers = ["Jorge Silva <jorgesilva.ti@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/scjorge/pydantic_br"
 documentation = "https://pydantic-br.readthedocs.io"
```

### Comparing `pydantic_br-0.3.0/README.md` & `pydantic_br-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 | Campo | Grupo de Documentos | Nome do Documento | Método de validação | Situação
 |---|---|---|---|---|
 | CNPJ | Pessoa Jurídica | Carteira Nacional de Pessoas Jurídicas | Digito Verificador | Concluído
 | CPF | Pessoa física | Cadastro de Pessoa Física | Digito Verificador | Concluído
 | CNH | Pessoa física | Carteira Nacional de Habilitação | Digito Verificador | Concluído
 | TE | Pessoa física  | Título de Eleitor | Digito Verificador | Concluído
 | PIS | Pessoa física  | Programa de Integração Social | Digito Verificador | Concluído
-| CERT | Pessoa física  | Certidão (Nascimento/Casamento/Óbito) | Digito Verificador | Em desenvolvimento
+| CERT | Pessoa física  | Certidão (Nascimento/Casamento/Óbito) | Digito Verificador | Concluído
 | CNS | Pessoa física  | Cartão Nacional de Saúde | Digito Verificador | Em desenvolvimento
-| RNVAM | Veículos | Registro Nacional de Veículos Automotores | RegExr | Em desenvolvimento
+| RENAVAM | Veículos | Registro Nacional de Veículos Automotores | RegExr | Em desenvolvimento
 | PLACA | Veículos | Placa do Veículo | RegExr | Em desenvolvimento
 | ISBN | Livros | Padrão Internacional de Numeração de Livro | Digito Verificador | Em desenvolvimento
 
 
 
 
 ## Instalação
```

### Comparing `pydantic_br-0.3.0/PKG-INFO` & `pydantic_br-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-br
-Version: 0.3.0
+Version: 0.4.0
 Summary: Pydantic library extension with Brazilian fields
 Home-page: https://github.com/scjorge/pydantic_br
 License: MIT
 Keywords: pydantic,json,json-schema,hints,parsin,brasil,documentos,br,fastapi,doc,documento
 Author: Jorge Silva
 Author-email: jorgesilva.ti@hotmail.com
 Maintainer: Jorge Silva
@@ -57,17 +57,17 @@
 | Campo | Grupo de Documentos | Nome do Documento | Método de validação | Situação
 |---|---|---|---|---|
 | CNPJ | Pessoa Jurídica | Carteira Nacional de Pessoas Jurídicas | Digito Verificador | Concluído
 | CPF | Pessoa física | Cadastro de Pessoa Física | Digito Verificador | Concluído
 | CNH | Pessoa física | Carteira Nacional de Habilitação | Digito Verificador | Concluído
 | TE | Pessoa física  | Título de Eleitor | Digito Verificador | Concluído
 | PIS | Pessoa física  | Programa de Integração Social | Digito Verificador | Concluído
-| CERT | Pessoa física  | Certidão (Nascimento/Casamento/Óbito) | Digito Verificador | Em desenvolvimento
+| CERT | Pessoa física  | Certidão (Nascimento/Casamento/Óbito) | Digito Verificador | Concluído
 | CNS | Pessoa física  | Cartão Nacional de Saúde | Digito Verificador | Em desenvolvimento
-| RNVAM | Veículos | Registro Nacional de Veículos Automotores | RegExr | Em desenvolvimento
+| RENAVAM | Veículos | Registro Nacional de Veículos Automotores | RegExr | Em desenvolvimento
 | PLACA | Veículos | Placa do Veículo | RegExr | Em desenvolvimento
 | ISBN | Livros | Padrão Internacional de Numeração de Livro | Digito Verificador | Em desenvolvimento
 
 
 
 
 ## Instalação
```

