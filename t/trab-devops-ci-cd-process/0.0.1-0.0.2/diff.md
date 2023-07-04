# Comparing `tmp/trab-devops-ci-cd-process-0.0.1.tar.gz` & `tmp/trab_devops_ci_cd_process-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trab-devops-ci-cd-process-0.0.1.tar", last modified: Mon Jul  3 12:06:42 2023, max compression
+gzip compressed data, was "trab_devops_ci_cd_process-0.0.2.tar", last modified: Tue Jul  4 17:06:37 2023, max compression
```

## Comparing `trab-devops-ci-cd-process-0.0.1.tar` & `trab_devops_ci_cd_process-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 12:06:42.234531 trab-devops-ci-cd-process-0.0.1/
--rw-rw-rw-   0        0        0     1099 2023-07-02 18:40:23.000000 trab-devops-ci-cd-process-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      841 2023-07-03 12:06:42.227528 trab-devops-ci-cd-process-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-07-03 11:58:32.000000 trab-devops-ci-cd-process-0.0.1/README.md
--rw-rw-rw-   0        0        0      923 2023-07-03 12:05:04.000000 trab-devops-ci-cd-process-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      160 2023-07-03 11:44:16.000000 trab-devops-ci-cd-process-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 12:06:42.234531 trab-devops-ci-cd-process-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 12:06:42.095102 trab-devops-ci-cd-process-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 12:06:42.155117 trab-devops-ci-cd-process-0.0.1/src/bhaskara/
--rw-rw-rw-   0        0        0        0 2023-07-02 18:56:50.000000 trab-devops-ci-cd-process-0.0.1/src/bhaskara/__init__.py
--rw-rw-rw-   0        0        0      872 2023-07-02 18:58:12.000000 trab-devops-ci-cd-process-0.0.1/src/bhaskara/eq_bhaskara.py
--rw-rw-rw-   0        0        0     1428 2023-07-02 20:14:22.000000 trab-devops-ci-cd-process-0.0.1/src/bhaskara/eq_segundo_grau.py
-drwxrwxrwx   0        0        0        0 2023-07-03 12:06:42.208532 trab-devops-ci-cd-process-0.0.1/src/trab_devops_ci_cd_process.egg-info/
--rw-rw-rw-   0        0        0      841 2023-07-03 12:06:42.000000 trab-devops-ci-cd-process-0.0.1/src/trab_devops_ci_cd_process.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-07-03 12:06:42.000000 trab-devops-ci-cd-process-0.0.1/src/trab_devops_ci_cd_process.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 12:06:42.000000 trab-devops-ci-cd-process-0.0.1/src/trab_devops_ci_cd_process.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 12:06:42.000000 trab-devops-ci-cd-process-0.0.1/src/trab_devops_ci_cd_process.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-03 12:06:42.000000 trab-devops-ci-cd-process-0.0.1/src/trab_devops_ci_cd_process.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 12:06:42.218531 trab-devops-ci-cd-process-0.0.1/test/
--rw-rw-rw-   0        0        0      855 2023-07-02 19:52:34.000000 trab-devops-ci-cd-process-0.0.1/test/test_solucao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:06:37.480006 trab_devops_ci_cd_process-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-04 17:06:27.000000 trab_devops_ci_cd_process-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-04 17:06:37.480006 trab_devops_ci_cd_process-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-04 17:06:27.000000 trab_devops_ci_cd_process-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-04 17:06:27.000000 trab_devops_ci_cd_process-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-04 17:06:27.000000 trab_devops_ci_cd_process-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:06:37.480006 trab_devops_ci_cd_process-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:06:37.480006 trab_devops_ci_cd_process-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:06:37.480006 trab_devops_ci_cd_process-0.0.2/src/bhaskara/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:06:27.000000 trab_devops_ci_cd_process-0.0.2/src/bhaskara/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-04 17:06:27.000000 trab_devops_ci_cd_process-0.0.2/src/bhaskara/eq_bhaskara.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-04 17:06:27.000000 trab_devops_ci_cd_process-0.0.2/src/bhaskara/eq_segundo_grau.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:06:37.480006 trab_devops_ci_cd_process-0.0.2/src/trab_devops_ci_cd_process.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-04 17:06:37.000000 trab_devops_ci_cd_process-0.0.2/src/trab_devops_ci_cd_process.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-04 17:06:37.000000 trab_devops_ci_cd_process-0.0.2/src/trab_devops_ci_cd_process.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:06:37.000000 trab_devops_ci_cd_process-0.0.2/src/trab_devops_ci_cd_process.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-04 17:06:37.000000 trab_devops_ci_cd_process-0.0.2/src/trab_devops_ci_cd_process.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 17:06:37.000000 trab_devops_ci_cd_process-0.0.2/src/trab_devops_ci_cd_process.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:06:37.480006 trab_devops_ci_cd_process-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-04 17:06:27.000000 trab_devops_ci_cd_process-0.0.2/test/test_solucao.py
```

### Comparing `trab-devops-ci-cd-process-0.0.1/PKG-INFO` & `trab_devops_ci_cd_process-0.0.2/src/trab_devops_ci_cd_process.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: trab-devops-ci-cd-process
-Version: 0.0.1
-Summary: quadratic equation roots calculating package for devops course
-Author-email: Ricardo Báfica Pontes <ricardo.bafica@gmail.com>
-Project-URL: Homepage, https://github.com/ricobafica/trab-devops-ci-cd
-Project-URL: Bug Tracker, https://github.com/ricobafica/trab-devops-ci-cd/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# trab-devops-ci-cd
-Respositorio do trabalho final da disciplina de Praticas Devops, curso de engenharia de dados da Pucminas 2023.
-
-Final task repository of the Devops Practices discipline, data engineering course at Pucminas 2023
-
+Metadata-Version: 2.1
+Name: trab-devops-ci-cd-process
+Version: 0.0.2
+Summary: quadratic equation roots calculating package for devops course
+Author-email: Ricardo Báfica Pontes <ricardo.bafica@gmail.com>
+Project-URL: Homepage, https://github.com/ricobafica/trab-devops-ci-cd
+Project-URL: Bug Tracker, https://github.com/ricobafica/trab-devops-ci-cd/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# trab-devops-ci-cd
+Respositorio do trabalho final da disciplina de Praticas Devops, curso de engenharia de dados da Pucminas 2023.
+
+Final task repository of the Devops Practices discipline, data engineering course at Pucminas 2023
+
```

### Comparing `trab-devops-ci-cd-process-0.0.1/pyproject.toml` & `trab_devops_ci_cd_process-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# requerimentos do sistema de build
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-# informações do projeto para envio ao pypi.org
-[project]
-name = "trab-devops-ci-cd-process"
-version = "0.0.1"
-authors = [
-  { name="Ricardo Báfica Pontes", email="ricardo.bafica@gmail.com" },
-]
-description = "quadratic equation roots calculating package for devops course"
-readme = "README.md"
-requires-python = ">=3.9"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dynamic = ["dependencies"]
-
-[tool.setuptools.dynamic]
-# especificacoes das dependencias do pacote
-dependencies = {file = ["requirements.txt"]}
-
-[project.urls]
-"Homepage" = "https://github.com/ricobafica/trab-devops-ci-cd"
-"Bug Tracker" = "https://github.com/ricobafica/trab-devops-ci-cd/issues"
-
+# requerimentos do sistema de build
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+# informações do projeto para envio ao pypi.org
+[project]
+name = "trab_devops_ci_cd_process"
+version = "0.0.2"
+authors = [
+  { name="Ricardo Báfica Pontes", email="ricardo.bafica@gmail.com" },
+]
+description = "quadratic equation roots calculating package for devops course"
+readme = "README.md"
+requires-python = ">=3.9"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dynamic = ["dependencies"]
+
+[tool.setuptools.dynamic]
+# especificacoes das dependencias do pacote
+dependencies = {file = ["requirements.txt"]}
+
+[project.urls]
+"Homepage" = "https://github.com/ricobafica/trab-devops-ci-cd"
+"Bug Tracker" = "https://github.com/ricobafica/trab-devops-ci-cd/issues"
+
```

### Comparing `trab-devops-ci-cd-process-0.0.1/src/bhaskara/eq_bhaskara.py` & `trab_devops_ci_cd_process-0.0.2/src/bhaskara/eq_bhaskara.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Este codigo encontra as raízes de uma equação de 2° grau: ax^2 + bx + c = 0
-
-import math
-# import os
-
-
-def raizes(a, b, c):
-
-    # os.system('cls' if os.name == 'nt' else 'clear')
-    print("agora estou no arquivo que calcula as raizes da eq 2° grau")
-    print("\nA eq. 2ºgrau {}x2 + {}x + ({}) =0".format(a, b, c))
-    delta = b**2 - 4*a*c
-
-    if delta < 0:
-        print("não possui raízes reais.")
-        x1 = x2 = None
-    elif delta == 0:
-        x1 = (-b + math.sqrt(delta)) / (2*a)
-        x2 = x1
-        print("possui apenas uma raiz real: ", x1)
-    else:
-        x1 = (-b + math.sqrt(delta)) / (2*a)
-        x2 = (-b - math.sqrt(delta)) / (2*a)
-        print("possui duas raízes reais: ", x1, " e ", x2)
-
-    return (x1, x2)
-
-
-# x1, x2 = raizes(a, b, c)
-
-# fim = input("\nTecle enter para saír ou digite 'sair'\n")
+# Este codigo encontra as raízes de uma equação de 2° grau: ax^2 + bx + c = 0
+
+import math
+# import os
+
+
+def raizes(a, b, c):
+
+    # os.system('cls' if os.name == 'nt' else 'clear')
+    print("agora estou no arquivo que calcula as raizes da eq 2° grau")
+    print("\nA eq. 2ºgrau {}x2 + {}x + ({}) =0".format(a, b, c))
+    delta = b**2 - 4*a*c
+
+    if delta < 0:
+        print("não possui raízes reais.")
+        x1 = x2 = None
+    elif delta == 0:
+        x1 = (-b + math.sqrt(delta)) / (2*a)
+        x2 = x1
+        print("possui apenas uma raiz real: ", x1)
+    else:
+        x1 = (-b + math.sqrt(delta)) / (2*a)
+        x2 = (-b - math.sqrt(delta)) / (2*a)
+        print("possui duas raízes reais: ", x1, " e ", x2)
+
+    return (x1, x2)
+
+
+# x1, x2 = raizes(a, b, c)
+
+# fim = input("\nTecle enter para saír ou digite 'sair'\n")
```

### Comparing `trab-devops-ci-cd-process-0.0.1/src/trab_devops_ci_cd_process.egg-info/PKG-INFO` & `trab_devops_ci_cd_process-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: trab-devops-ci-cd-process
-Version: 0.0.1
-Summary: quadratic equation roots calculating package for devops course
-Author-email: Ricardo Báfica Pontes <ricardo.bafica@gmail.com>
-Project-URL: Homepage, https://github.com/ricobafica/trab-devops-ci-cd
-Project-URL: Bug Tracker, https://github.com/ricobafica/trab-devops-ci-cd/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# trab-devops-ci-cd
-Respositorio do trabalho final da disciplina de Praticas Devops, curso de engenharia de dados da Pucminas 2023.
-
-Final task repository of the Devops Practices discipline, data engineering course at Pucminas 2023
-
+Metadata-Version: 2.1
+Name: trab_devops_ci_cd_process
+Version: 0.0.2
+Summary: quadratic equation roots calculating package for devops course
+Author-email: Ricardo Báfica Pontes <ricardo.bafica@gmail.com>
+Project-URL: Homepage, https://github.com/ricobafica/trab-devops-ci-cd
+Project-URL: Bug Tracker, https://github.com/ricobafica/trab-devops-ci-cd/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# trab-devops-ci-cd
+Respositorio do trabalho final da disciplina de Praticas Devops, curso de engenharia de dados da Pucminas 2023.
+
+Final task repository of the Devops Practices discipline, data engineering course at Pucminas 2023
+
```

### Comparing `trab-devops-ci-cd-process-0.0.1/test/test_solucao.py` & `trab_devops_ci_cd_process-0.0.2/test/test_solucao.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import src.bhaskara.eq_bhaskara as eq_bhaskara
-import src.bhaskara.eq_segundo_grau as eq_segundo_grau
-
-
-def test_rais1():
-    print("estou no arquivo que testa bhaskara")
-    r1, r2 = eq_bhaskara.raizes(1, 5, -6)
-    assert (1*r1**2 + 5*r1 + -6) == 0
-
-
-def test_raiz2():
-    print("estou no arquivo que testa bhaskara")
-    r1, r2 = eq_bhaskara.raizes(1, 5, -6)
-    assert (1*r2**2 + 5*r2 + -6) == 0
-
-
-def test_solucoes():
-    print("estou no arquivo que testa 2o grau")
-    r1, r2 = eq_segundo_grau.incognitas(1, 5, -6)
-    assert (1*r2**2 + 5*r2 + -6) == 0
-
-# Why PyTest is not collecting tests (collected 0 items)?
-# https://stackoverflow.com/questions/37353960/why-pytest-is-not-collecting-tests-collected-0-items
-
-# Good Integration Practices
-# https://docs.pytest.org/en/latest/explanation/goodpractices.html#goodpractices
+import src.bhaskara.eq_bhaskara as eq_bhaskara
+import src.bhaskara.eq_segundo_grau as eq_segundo_grau
+
+
+def test_rais1():
+    print("estou no arquivo que testa bhaskara")
+    r1, r2 = eq_bhaskara.raizes(1, 5, -6)
+    assert (1*r1**2 + 5*r1 + -6) == 0
+
+
+def test_raiz2():
+    print("estou no arquivo que testa bhaskara")
+    r1, r2 = eq_bhaskara.raizes(1, 5, -6)
+    assert (1*r2**2 + 5*r2 + -6) == 0
+
+
+def test_solucoes():
+    print("estou no arquivo que testa 2o grau")
+    r1, r2 = eq_segundo_grau.incognitas(1, 5, -6)
+    assert (1*r2**2 + 5*r2 + -6) == 0
+
+# Why PyTest is not collecting tests (collected 0 items)?
+# https://stackoverflow.com/questions/37353960/why-pytest-is-not-collecting-tests-collected-0-items
+
+# Good Integration Practices
+# https://docs.pytest.org/en/latest/explanation/goodpractices.html#goodpractices
```

