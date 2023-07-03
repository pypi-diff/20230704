# Comparing `tmp/fiddler-auditor-0.0.1rc3.tar.gz` & `tmp/fiddler-auditor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-auditor-0.0.1rc3.tar", last modified: Thu May 25 01:17:47 2023, max compression
+gzip compressed data, was "fiddler-auditor-0.0.2.tar", last modified: Mon Jul  3 22:55:42 2023, max compression
```

## Comparing `fiddler-auditor-0.0.1rc3.tar` & `fiddler-auditor-0.0.2.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.778644 fiddler-auditor-0.0.1rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-25 01:17:47.778644 fiddler-auditor-0.0.1rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.766644 fiddler-auditor-0.0.1rc3/auditor/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.766644 fiddler-auditor-0.0.1rc3/auditor/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.766644 fiddler-auditor-0.0.1rc3/auditor/assets/data/
--rw-r--r--   0 runner    (1001) docker     (123)    43309 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/assets/data/snips_dataset_dev.csv
--rw-r--r--   0 runner    (1001) docker     (123)    43115 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/assets/data/snips_dataset_test.csv
--rw-r--r--   0 runner    (1001) docker     (123)   798933 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/assets/data/snips_dataset_train.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/auditor/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/evaluation/discriminative.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/evaluation/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/evaluation/expected_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/evaluation/generative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/auditor/generations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/generations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/generations/paraphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/auditor/perturbations/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/perturbations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/perturbations/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/perturbations/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/auditor/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/reporting/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/auditor/reporting/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/reporting/templates/report_template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/auditor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/utils/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-25 01:17:47.000000 fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-25 01:17:47.000000 fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 01:17:47.000000 fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 01:17:47.000000 fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 01:17:47.000000 fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 01:17:47.778644 fiddler-auditor-0.0.1rc3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.774644 fiddler-auditor-0.0.1rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/tests/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/tests/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/tests/test_perturbations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:42.625365 fiddler-auditor-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-03 22:55:42.625365 fiddler-auditor-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:42.617365 fiddler-auditor-0.0.2/auditor/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:42.617365 fiddler-auditor-0.0.2/auditor/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:42.617365 fiddler-auditor-0.0.2/auditor/assets/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    43309 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/assets/data/snips_dataset_dev.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    43115 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/assets/data/snips_dataset_test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   798933 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/assets/data/snips_dataset_train.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:42.621365 fiddler-auditor-0.0.2/auditor/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/evaluation/discriminative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/evaluation/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/evaluation/expected_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/evaluation/generative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:42.621365 fiddler-auditor-0.0.2/auditor/generations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/generations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/generations/paraphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:42.621365 fiddler-auditor-0.0.2/auditor/perturbations/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/perturbations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/perturbations/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/perturbations/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/perturbations/paraphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/perturbations/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:42.621365 fiddler-auditor-0.0.2/auditor/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/reporting/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:42.621365 fiddler-auditor-0.0.2/auditor/reporting/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/reporting/templates/report_template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:42.621365 fiddler-auditor-0.0.2/auditor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/auditor/utils/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:42.621365 fiddler-auditor-0.0.2/fiddler_auditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-03 22:55:42.000000 fiddler-auditor-0.0.2/fiddler_auditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-03 22:55:42.000000 fiddler-auditor-0.0.2/fiddler_auditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:55:42.000000 fiddler-auditor-0.0.2/fiddler_auditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-03 22:55:42.000000 fiddler-auditor-0.0.2/fiddler_auditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 22:55:42.000000 fiddler-auditor-0.0.2/fiddler_auditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:55:42.625365 fiddler-auditor-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:55:42.625365 fiddler-auditor-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/tests/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/tests/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-03 22:51:52.000000 fiddler-auditor-0.0.2/tests/test_perturbations.py
```

### Comparing `fiddler-auditor-0.0.1rc3/LICENSE` & `fiddler-auditor-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/PKG-INFO` & `fiddler-auditor-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,72 @@
-Metadata-Version: 2.1
-Name: fiddler-auditor
-Version: 0.0.1rc3
-Summary: Auditing large language models made easy.
-Author-email: Fiddler Labs <support@fiddler.ai>
-License: Elastic License 2.0 (ELv2)
-Project-URL: repository, https://github.com/fiddler-labs/fiddler-auditor
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: <4.0,>=3.8.1
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-# <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/fiddler-auditor-logo.png" width="60%" alt="Fiddler Auditor">
+# <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/fiddler-auditor-logo.png?raw=true" width="60%" alt="Fiddler Auditor">
 
 Auditing Large Language Models made easy!
 
-[![lint](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/codelint.yml/badge.svg)](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/codelint.yml)
-[![test](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/test.yml)
+<!-- [![lint](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/codelint.yml/badge.svg)](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/codelint.yml)
+[![test](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/test.yml) -->
 
 
 ## What is Fiddler Auditor?
 
 <div align="left">
     <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/monitoring-generative-ai-models_fiddler-auditor.png?raw=true"
          alt="Fiddler Auditor Capabilities"/>
 </div>
 
 Language models enable companies to build and launch innovative applications to improve productivity and increase customer satisfaction. 
 However, it’s been known that LLMs can hallucinate, generate adversarial responses that can harm users, and even expose private information that they were trained on when prompted or unprompted. It's more critical than ever for ML and software application teams to minimize these risks and weaknesses before launching LLMs and NLP models. As a result, it’s important for you to include a process to audit language models thoroughly before production.
 The Fiddler Auditor enables you to test LLMs and NLP models, identify weaknesses in the models, and mitigate potential adversarial outcomes before deploying them to production.
 
 ## Features and Capabilities
+
+<p>
+<div align="left">
+    <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/images/fiddler-auditor-flow.png?raw=true"
+         alt="Fiddler Auditor Flow"/>
+</div>
+</p>
+
 Fiddler Auditor supports
 
 - Red-teaming LLMs for your use-case with prompt perturbation
 - Integration with LangChain
 - Custom evaluation metrics
 - Generative and Discriminative NLP models
-- Comparison of LLMs (Upcoming)
+- Comparison of LLMs
 
+<p>
 <div align="left">
     <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/fiddler-auditor-prompt-evaluation.png?raw=true"
          alt="Example Report"/>
+    <em> An example report generated by the Fiddler Auditor for text-davinci-003. </em>
 </div>
+</p>
 
-## Installation
-Auditor is available on pypi.
 
-`pip install fiddler-auditor`
+## Installation
 
-or you can install from source after cloning the repo using the following command
+### From PyPI
+Auditor is available on PyPI and we test on Python 3.8 and above. We recommend creating a virtual python environment and installing using the following command
 
-`pip install .`
+```bash
+pip install fiddler-auditor
+```
+
+### From source
+You can install from source after cloning this repo using the following command
+
+```bash
+pip install .
+```
 
 ## Quick-start guides
-- [Evaluate LLM Correctness and Robustness](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/LLM_Evaluation.ipynb)
-- [Evaluate LLMs with custom metrics](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Evaluation.ipynb)
+- [Evaluate LLM Correctness and Robustness](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/LLM_Evaluation.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fiddler-labs/fiddler-auditor/blob/main/examples/LLM_Evaluation.ipynb)
+- [Evaluate LLMs with custom metrics](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Evaluation.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Evaluation.ipynb)
+- [Prompt injection attack with custom transformation](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Transformation.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Transformation.ipynb)
 
 
 ## Contribution
 We are continuously updating this library to support language models as they evolve. 
 
 - Contributions in the form of suggestions and PRs to Fiddler Auditor are welcome!
 - If you encounter a bug, please feel free to raise issues in this repository.
```

### Comparing `fiddler-auditor-0.0.1rc3/README.md` & `fiddler-auditor-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,86 @@
-# <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/fiddler-auditor-logo.png" width="60%" alt="Fiddler Auditor">
+Metadata-Version: 2.1
+Name: fiddler-auditor
+Version: 0.0.2
+Summary: Auditing large language models made easy.
+Author-email: Fiddler Labs <support@fiddler.ai>
+License: Elastic License 2.0 (ELv2)
+Project-URL: repository, https://github.com/fiddler-labs/fiddler-auditor
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: <4.0,>=3.8.1
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+# <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/fiddler-auditor-logo.png?raw=true" width="60%" alt="Fiddler Auditor">
 
 Auditing Large Language Models made easy!
 
-[![lint](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/codelint.yml/badge.svg)](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/codelint.yml)
-[![test](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/test.yml)
+<!-- [![lint](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/codelint.yml/badge.svg)](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/codelint.yml)
+[![test](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/test.yml) -->
 
 
 ## What is Fiddler Auditor?
 
 <div align="left">
     <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/monitoring-generative-ai-models_fiddler-auditor.png?raw=true"
          alt="Fiddler Auditor Capabilities"/>
 </div>
 
 Language models enable companies to build and launch innovative applications to improve productivity and increase customer satisfaction. 
 However, it’s been known that LLMs can hallucinate, generate adversarial responses that can harm users, and even expose private information that they were trained on when prompted or unprompted. It's more critical than ever for ML and software application teams to minimize these risks and weaknesses before launching LLMs and NLP models. As a result, it’s important for you to include a process to audit language models thoroughly before production.
 The Fiddler Auditor enables you to test LLMs and NLP models, identify weaknesses in the models, and mitigate potential adversarial outcomes before deploying them to production.
 
 ## Features and Capabilities
+
+<p>
+<div align="left">
+    <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/images/fiddler-auditor-flow.png?raw=true"
+         alt="Fiddler Auditor Flow"/>
+</div>
+</p>
+
 Fiddler Auditor supports
 
 - Red-teaming LLMs for your use-case with prompt perturbation
 - Integration with LangChain
 - Custom evaluation metrics
 - Generative and Discriminative NLP models
-- Comparison of LLMs (Upcoming)
+- Comparison of LLMs
 
+<p>
 <div align="left">
     <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/fiddler-auditor-prompt-evaluation.png?raw=true"
          alt="Example Report"/>
+    <em> An example report generated by the Fiddler Auditor for text-davinci-003. </em>
 </div>
+</p>
 
-## Installation
-Auditor is available on pypi.
 
-`pip install fiddler-auditor`
+## Installation
 
-or you can install from source after cloning the repo using the following command
+### From PyPI
+Auditor is available on PyPI and we test on Python 3.8 and above. We recommend creating a virtual python environment and installing using the following command
 
-`pip install .`
+```bash
+pip install fiddler-auditor
+```
+
+### From source
+You can install from source after cloning this repo using the following command
+
+```bash
+pip install .
+```
 
 ## Quick-start guides
-- [Evaluate LLM Correctness and Robustness](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/LLM_Evaluation.ipynb)
-- [Evaluate LLMs with custom metrics](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Evaluation.ipynb)
+- [Evaluate LLM Correctness and Robustness](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/LLM_Evaluation.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fiddler-labs/fiddler-auditor/blob/main/examples/LLM_Evaluation.ipynb)
+- [Evaluate LLMs with custom metrics](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Evaluation.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Evaluation.ipynb)
+- [Prompt injection attack with custom transformation](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Transformation.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Transformation.ipynb)
 
 
 ## Contribution
 We are continuously updating this library to support language models as they evolve. 
 
 - Contributions in the form of suggestions and PRs to Fiddler Auditor are welcome!
 - If you encounter a bug, please feel free to raise issues in this repository.
```

### Comparing `fiddler-auditor-0.0.1rc3/auditor/assets/data/snips_dataset_dev.csv` & `fiddler-auditor-0.0.2/auditor/assets/data/snips_dataset_dev.csv`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/auditor/assets/data/snips_dataset_test.csv` & `fiddler-auditor-0.0.2/auditor/assets/data/snips_dataset_test.csv`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/auditor/assets/data/snips_dataset_train.csv` & `fiddler-auditor-0.0.2/auditor/assets/data/snips_dataset_train.csv`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/auditor/evaluation/discriminative.py` & `fiddler-auditor-0.0.2/auditor/evaluation/discriminative.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/auditor/evaluation/expected_behavior.py` & `fiddler-auditor-0.0.2/auditor/evaluation/expected_behavior.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/auditor/evaluation/generative.py` & `fiddler-auditor-0.0.2/auditor/evaluation/generative.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,55 +6,63 @@
     LLMEvalResult,
     LLMEvalType,
 )
 from auditor.evaluation.expected_behavior import (
     SimilarGeneration,
 )
 from auditor.utils.logging import get_logger
-from auditor.perturbations.text import PerturbText
+from auditor.perturbations import Paraphrase
+from auditor.perturbations import TransformBase
 
 LOG = get_logger(__name__)
 
 
 class LLMEval:
     def __init__(
         self,
         llm:  BaseLLM,
         expected_behavior: SimilarGeneration,
+        transformation: Optional[TransformBase] = None,
     ) -> None:
         """Class for evaluating Large Language Models (LLMs)
 
         Args:
             llm (BaseLLM): Langchain LLM Object
             expected_behavior (SimilarGeneration):
                 Expected model behavior to evaluate against
+            transformation (Optional[TransformBase], optional):
+                Transformation to evaluate against.
+                When not provided defaults to using auditor.perturbations.Paraphrase.  # noqa: E501
         """
         self.llm = llm
         self.expected_behavior = expected_behavior
+        if transformation is None:
+            self.transformation = Paraphrase()
+        else:
+            self.transformation = transformation
         return
 
     def _evaluate_generations(
         self,
         prompt: str,
         evaluation_type: Literal[LLMEvalType.robustness, LLMEvalType.correctness],  # noqa: E501
-        perturbations_per_sample: int = 5,
         pre_context: Optional[str] = None,
         post_context: Optional[str] = None,
         reference_generation: Optional[str] = None,
         prompt_perturbations: Optional[List[str]] = None,
+        *args,
+        **kwargs,
     ) -> LLMEvalResult:
         """
         Evaluates generations to paraphrased prompt perturbations
 
         Args:
             prompt (str): Prompt to be perturbed
             evaluation_type (LLMEvalType): Evaluation type. Supported types -
             Robustness or Correctness.
-            perturbations_per_sample (int, optional):
-                No of perturbations to generate for the prompt. Defaults to 5.
             pre_context (Optional[str], optional):
                 Context prior to prompt, will not be perturbed.
                 Defaults to None.
             post_context (Optional[str], optional):
                 Context post prompt, will not be perturbed.
                 Defaults to None.
             reference_generation (Optional[str], optional):
@@ -77,15 +85,16 @@
                 pre_context,
                 post_context,
             )
         # create alternative prompt perturbations
         if prompt_perturbations is None:
             prompt_perturbations = self.generate_alternative_prompts(
                 prompt=prompt,
-                perturbations_per_sample=perturbations_per_sample,
+                *args,
+                **kwargs,
             )
         # include the original prompt when evaluating correctness
         if evaluation_type.value == LLMEvalType.correctness.value:
             evaluate_prompts = [prompt] + prompt_perturbations
         else:
             evaluate_prompts = prompt_perturbations
 
@@ -151,42 +160,29 @@
         if post_context is not None:
             full_prompt += delimiter + post_context
         return full_prompt
 
     def generate_alternative_prompts(
         self,
         prompt: str,
-        perturbations_per_sample: int,
-        temperature: Optional[float] = 0.0,
-        return_original: Optional[bool] = False,
+        *args,
+        **kwargs,
     ) -> List[str]:
-        """Generates paraphrased prompts.
+        """Generates perturbed prompts
 
         Args:
             prompt (str): Prompt to be perturbed
-            perturbations_per_sample (int): No of paraphrases to generate
-            temperature (Optional[float], optional): Temperaure for
-                generations. Defaults to 0.0
-            return_original (Optional[bool], optional): If True original prompt
-                is returned as the first entry in the list. Defaults to False.
-        Returns:
-            List[str]: List of paraphrased prompts.
+            Returns:
+            List[str]: List of perturbed prompts.
         """
-        perturber = PerturbText(
-            [prompt],
-            ner_pipeline=None,
-            batch_size=1,
-            perturbations_per_sample=perturbations_per_sample,
+        return self.transformation.transform(
+            prompt,
+            *args,
+            **kwargs,
         )
-        # TODO: Add perturbation types
-        perturbed_dataset = perturber.paraphrase(temperature=temperature)
-        if return_original:
-            return perturbed_dataset.data[0]
-        else:
-            return perturbed_dataset.data[0][1:]
 
     def _get_generation_details(self) -> Dict[str, str]:
         """Returns generation related details"""
         details = {}
         if hasattr(self.llm, '_llm_type'):
             details['Provider'] = self.llm._llm_type
         if hasattr(self.llm, 'temperature'):
@@ -194,26 +190,29 @@
         if hasattr(self.llm, 'model_name'):
             details['Model Name'] = self.llm.model_name
         return details
 
     def evaluate_prompt_robustness(
         self,
         prompt: str,
-        perturbations_per_sample: int = 5,
+        perturbations_per_sample: Optional[int] = None,
         pre_context: Optional[str] = None,
         post_context: Optional[str] = None,
         prompt_perturbations: Optional[List[str]] = None,
+        *args,
+        **kwargs,
     ) -> LLMEvalResult:
         """
         Evaluates robustness of generation to paraphrased prompt perturbations
 
         Args:
             prompt (str): Prompt to be perturbed
             perturbations_per_sample (int, optional):
-                No of perturbations to generate for the prompt. Defaults to 5.
+                Deprecated. No of perturbation is now controlled by the
+                Transform object.
             pre_context (Optional[str], optional):
                 Context prior to prompt, will not be perturbed.
                 Defaults to None.
             post_context (Optional[str], optional):
                 Context post prompt, will not be perturbed.
                 Defaults to None.
             prompt_perturbations (Optional[List[str]], optional):
@@ -222,39 +221,43 @@
 
         Returns:
             LLMEvalResult: Object wth evaluation results
         """
         return self._evaluate_generations(
             prompt=prompt,
             evaluation_type=LLMEvalType.robustness,
-            perturbations_per_sample=perturbations_per_sample,
             pre_context=pre_context,
             post_context=post_context,
             reference_generation=None,
             prompt_perturbations=prompt_perturbations,
+            *args,
+            **kwargs,
         )
 
     def evaluate_prompt_correctness(
         self,
         prompt: str,
         reference_generation: str,
-        perturbations_per_sample: int = 5,
+        perturbations_per_sample: Optional[int] = None,
         pre_context: Optional[str] = None,
         post_context: Optional[str] = None,
         alternative_prompts: Optional[List[str]] = None,
+        *args,
+        **kwargs,
     ) -> LLMEvalResult:
         """
         Evaluates robustness of generation to paraphrased prompt perturbations
 
         Args:
             prompt (str): Prompt to be perturbed
             reference_generation (str):
                 Reference generation to compare against.
             perturbations_per_sample (int, optional):
-                No of perturbations to generate for the prompt. Defaults to 5.
+                Deprecated. No of perturbation is now controlled by the
+                Transform object.
             pre_context (Optional[str], optional):
                 Context prior to prompt, will not be perturbed.
                 Defaults to None.
             post_context (Optional[str], optional):
                 Context post prompt, will not be perturbed.
                 Defaults to None.
             alternative_prompts (Optional[List[str]], optional):
@@ -263,13 +266,14 @@
 
         Returns:
             LLMEvalResult: Object wth evaluation results
         """
         return self._evaluate_generations(
             prompt=prompt,
             evaluation_type=LLMEvalType.correctness,
-            perturbations_per_sample=perturbations_per_sample,
             pre_context=pre_context,
             post_context=post_context,
             reference_generation=reference_generation,
             prompt_perturbations=alternative_prompts,
+            *args,
+            **kwargs,
         )
```

### Comparing `fiddler-auditor-0.0.1rc3/auditor/generations/paraphrase.py` & `fiddler-auditor-0.0.2/auditor/generations/paraphrase.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Optional
 import os
 import openai
 
 from auditor.perturbations.constants import OPENAI_CHAT_COMPLETION
 
 SIMILAR_SENTENCES_PROMPT = (
     'Generate a numbered list of {n} sentences '
@@ -12,32 +12,41 @@
 
 def generate_similar_sentences(
     sentence: str,
     api_key: str,
     model: str = OPENAI_CHAT_COMPLETION,
     num_sentences: int = 5,
     temperature: float = 0.0,
+    api_version: Optional[str] = None,
 ) -> List[str]:
     prompt = SIMILAR_SENTENCES_PROMPT.format(
         n=num_sentences,
         sentence=sentence
     )
     payload = [
         {
             "role": "user",
             "content": prompt
         }
     ]
     if api_key is None:
         api_key = os.getenv("OPENAI_API_KEY")
     openai.api_key = api_key
+
+    engine = None
+    if openai.api_type == "azure":
+        engine = model
+        api_version = api_version
+
     response = openai.ChatCompletion.create(
       model=model,
       messages=payload,
       temperature=temperature,
+      engine=engine,
+      api_version=api_version
     )
     return _process_similar_sentence_reponse(response)
 
 
 def _process_similar_sentence_reponse(response):
     sim_sent = []
     lines = response['choices'][0]['message']['content'].split('\n')
```

### Comparing `fiddler-auditor-0.0.1rc3/auditor/perturbations/text.py` & `fiddler-auditor-0.0.2/auditor/perturbations/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,26 +15,29 @@
 from auditor.generations.paraphrase import generate_similar_sentences
 from auditor.perturbations.constants import OPENAI_CHAT_COMPLETION
 from auditor.utils.similarity import (
     DEFAULT_SENTENCE_XFMR,
     load_similarity_model,
     compute_similarity
 )
+from auditor.utils.misc import simulate_typos
+
 COUNTRIES = [x.lower() for x in Perturb.data['country']]
 CITIES = [x.lower() for x in Perturb.data['city']]
 
 LOG = get_logger(__name__)
 
 
 @enum.unique
 class PerturbationType(enum.Enum):
     """String representation for perturbations"""
     perturb_names = 'Names'
     perturb_location = 'Locations'
     perturb_number = 'Numbers'
+    pertrub_typos = 'Typos'
     paraphrase = 'Paraphrase'
 
     def __str__(self) -> str:
         return str(self.value)
 
 
 def custom_perturb_location(
@@ -249,31 +252,71 @@
         return create_perturbed_dataclass(
             checklist_data,
             perturbations_per_sample=self.perturbations_per_sample,
             original_dataset_size=len(self.data),
             perturbation_type=PerturbationType.perturb_number,
         )
 
+    def perturb_typos(
+            self,
+            typo_probability: float = 0.02
+    ) -> PerturbedTextDataset:
+        """Perturb the dataset by introducing simulated user typos
+
+        Args:
+            temprature: rate of errors
+
+        Returns:
+            PerturbedTextDataset: Perturbed dataset object
+        """
+
+        LOG.info("Perturbing user typos in the dataset.")
+
+        perturbed_dataset = []
+        total_perturbations = 0
+        for sentence in self.data:
+            similar_sentences = []
+            for i in range(0, self.perturbations_per_sample):
+                similar_sentences.append(
+                    simulate_typos(
+                        sentence,
+                        typo_probability
+                    )
+                )
+            perturbed_dataset.append([sentence] + similar_sentences)
+            total_perturbations += len(similar_sentences)
+
+        return PerturbedTextDataset(
+            data=perturbed_dataset,
+            metadata=None,
+            total_perturbations=total_perturbations,
+            original_dataset_size=len(self.data),
+            perturbations_per_sample=self.perturbations_per_sample,
+            perturbation_type=PerturbationType.pertrub_typos,
+        )
+
     def paraphrase(
         self,
         model: Optional[str] = OPENAI_CHAT_COMPLETION,
         temperature: float = 0.0,
         api_key: Optional[str] = None,
         similarity_model: Optional[str] = None,
+        api_version: Optional[str] = None,
     ) -> PerturbedTextDataset:
         """Perturb the sentence by paraphrasing.
 
         Args:
             model (str, optional): Model to use for paraphrasing.
                 Defaults to ''gpt-3.5-turbo'.
             temperature (float, optional): Tempertaure for generations.
                 Defaults to 0.0.
             api_key (str) : openai API key
             similarity_model : Model to use for scoring the similarity of
                 perturbations.
+            api_version (str, optional): openai API version
 
         Returns:
             PerturbedTextDataset: Perturbed dataset object
         """
         perturbed_dataset = []
         total_perturbations = 0
         if similarity_model is None:
@@ -284,14 +327,15 @@
         similarity_model = load_similarity_model(similarity_model)
         dataset_metadata = []
         for sentence in self.data:
             similar_sentences = generate_similar_sentences(
                 sentence=sentence,
                 api_key=api_key,
                 model=model,
+                api_version=api_version,
                 num_sentences=self.perturbations_per_sample,
                 temperature=temperature,
             )
             perturbed_dataset.append([sentence] + similar_sentences)
             total_perturbations += len(similar_sentences)
             metadata = [None]
             for new_sent in similar_sentences:
```

### Comparing `fiddler-auditor-0.0.1rc3/auditor/reporting/generate.py` & `fiddler-auditor-0.0.2/auditor/reporting/generate.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/auditor/reporting/templates/report_template.html` & `fiddler-auditor-0.0.2/auditor/reporting/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/auditor/utils/data.py` & `fiddler-auditor-0.0.2/auditor/utils/data.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/auditor/utils/dataset.py` & `fiddler-auditor-0.0.2/auditor/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/auditor/utils/logging.py` & `fiddler-auditor-0.0.2/auditor/utils/logging.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/auditor/utils/similarity.py` & `fiddler-auditor-0.0.2/auditor/utils/similarity.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
         convert_to_tensor=True
     )
     perturbed_emb = sentence_model.encode(
         sentences=[perturbed_sentence],
         convert_to_tensor=True
     )
     score = sent_util.cos_sim(ref_emb, perturbed_emb)
-    return score.numpy()[0][0]
+    return score.cpu().numpy()[0][0]
```

### Comparing `fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/PKG-INFO` & `fiddler-auditor-0.0.2/fiddler_auditor.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,86 @@
 Metadata-Version: 2.1
 Name: fiddler-auditor
-Version: 0.0.1rc3
+Version: 0.0.2
 Summary: Auditing large language models made easy.
 Author-email: Fiddler Labs <support@fiddler.ai>
 License: Elastic License 2.0 (ELv2)
 Project-URL: repository, https://github.com/fiddler-labs/fiddler-auditor
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: <4.0,>=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/fiddler-auditor-logo.png" width="60%" alt="Fiddler Auditor">
+# <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/fiddler-auditor-logo.png?raw=true" width="60%" alt="Fiddler Auditor">
 
 Auditing Large Language Models made easy!
 
-[![lint](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/codelint.yml/badge.svg)](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/codelint.yml)
-[![test](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/test.yml)
+<!-- [![lint](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/codelint.yml/badge.svg)](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/codelint.yml)
+[![test](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/test.yml/badge.svg)](https://github.com/fiddler-labs/fiddler-auditor/actions/workflows/test.yml) -->
 
 
 ## What is Fiddler Auditor?
 
 <div align="left">
     <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/monitoring-generative-ai-models_fiddler-auditor.png?raw=true"
          alt="Fiddler Auditor Capabilities"/>
 </div>
 
 Language models enable companies to build and launch innovative applications to improve productivity and increase customer satisfaction. 
 However, it’s been known that LLMs can hallucinate, generate adversarial responses that can harm users, and even expose private information that they were trained on when prompted or unprompted. It's more critical than ever for ML and software application teams to minimize these risks and weaknesses before launching LLMs and NLP models. As a result, it’s important for you to include a process to audit language models thoroughly before production.
 The Fiddler Auditor enables you to test LLMs and NLP models, identify weaknesses in the models, and mitigate potential adversarial outcomes before deploying them to production.
 
 ## Features and Capabilities
+
+<p>
+<div align="left">
+    <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/images/fiddler-auditor-flow.png?raw=true"
+         alt="Fiddler Auditor Flow"/>
+</div>
+</p>
+
 Fiddler Auditor supports
 
 - Red-teaming LLMs for your use-case with prompt perturbation
 - Integration with LangChain
 - Custom evaluation metrics
 - Generative and Discriminative NLP models
-- Comparison of LLMs (Upcoming)
+- Comparison of LLMs
 
+<p>
 <div align="left">
     <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/fiddler-auditor-prompt-evaluation.png?raw=true"
          alt="Example Report"/>
+    <em> An example report generated by the Fiddler Auditor for text-davinci-003. </em>
 </div>
+</p>
 
-## Installation
-Auditor is available on pypi.
 
-`pip install fiddler-auditor`
+## Installation
 
-or you can install from source after cloning the repo using the following command
+### From PyPI
+Auditor is available on PyPI and we test on Python 3.8 and above. We recommend creating a virtual python environment and installing using the following command
 
-`pip install .`
+```bash
+pip install fiddler-auditor
+```
+
+### From source
+You can install from source after cloning this repo using the following command
+
+```bash
+pip install .
+```
 
 ## Quick-start guides
-- [Evaluate LLM Correctness and Robustness](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/LLM_Evaluation.ipynb)
-- [Evaluate LLMs with custom metrics](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Evaluation.ipynb)
+- [Evaluate LLM Correctness and Robustness](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/LLM_Evaluation.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fiddler-labs/fiddler-auditor/blob/main/examples/LLM_Evaluation.ipynb)
+- [Evaluate LLMs with custom metrics](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Evaluation.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Evaluation.ipynb)
+- [Prompt injection attack with custom transformation](https://github.com/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Transformation.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fiddler-labs/fiddler-auditor/blob/main/examples/Custom_Transformation.ipynb)
 
 
 ## Contribution
 We are continuously updating this library to support language models as they evolve. 
 
 - Contributions in the form of suggestions and PRs to Fiddler Auditor are welcome!
 - If you encounter a bug, please feel free to raise issues in this repository.
```

### Comparing `fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/SOURCES.txt` & `fiddler-auditor-0.0.2/fiddler_auditor.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 auditor/evaluation/discriminative.py
 auditor/evaluation/evaluate.py
 auditor/evaluation/expected_behavior.py
 auditor/evaluation/generative.py
 auditor/generations/__init__.py
 auditor/generations/paraphrase.py
 auditor/perturbations/__init__.py
+auditor/perturbations/base.py
 auditor/perturbations/constants.py
+auditor/perturbations/paraphrase.py
 auditor/perturbations/text.py
 auditor/reporting/__init__.py
 auditor/reporting/generate.py
 auditor/reporting/templates/report_template.html
 auditor/utils/__init__.py
 auditor/utils/data.py
 auditor/utils/dataset.py
```

### Comparing `fiddler-auditor-0.0.1rc3/pyproject.toml` & `fiddler-auditor-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fiddler-auditor"
-version = "0.0.1.rc3"
+version = "0.0.2"
 authors = [
   { name="Fiddler Labs", email="support@fiddler.ai" },
 ]
 description = "Auditing large language models made easy."
 readme = "README.md"
 requires-python = ">=3.8.1,<4.0"
```

### Comparing `fiddler-auditor-0.0.1rc3/tests/test_dataset.py` & `fiddler-auditor-0.0.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/tests/test_evaluation.py` & `fiddler-auditor-0.0.2/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc3/tests/test_llm.py` & `fiddler-auditor-0.0.2/tests/test_llm.py`

 * *Files identical despite different names*

