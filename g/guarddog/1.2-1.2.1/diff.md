# Comparing `tmp/guarddog-1.2.tar.gz` & `tmp/guarddog-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guarddog-1.2.tar", max compression
+gzip compressed data, was "guarddog-1.2.1.tar", max compression
```

## Comparing `guarddog-1.2.tar` & `guarddog-1.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    11357 2023-07-03 07:15:42.313327 guarddog-1.2/LICENSE
--rw-r--r--   0        0        0      314 2023-07-03 07:15:42.313327 guarddog-1.2/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0      154 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/__init__.py
--rw-r--r--   0        0        0      246 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/__main__.py
--rw-r--r--   0        0        0        0 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/__init__.py
--rw-r--r--   0        0        0     9679 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/analyzer.py
--rw-r--r--   0        0        0      457 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/__init__.py
--rw-r--r--   0        0        0      609 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/detector.py
--rw-r--r--   0        0        0     1166 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/empty_information.py
--rw-r--r--   0        0        0      696 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/npm/__init__.py
--rw-r--r--   0        0        0      793 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/npm/empty_information.py
--rw-r--r--   0        0        0     1176 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      578 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/npm/release_zero.py
--rw-r--r--   0        0        0     1732 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/npm/typosquatting.py
--rw-r--r--   0        0        0     4153 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      976 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/pypi/__init__.py
--rw-r--r--   0        0        0      723 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/pypi/empty_information.py
--rw-r--r--   0        0        0     1803 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      716 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/pypi/release_zero.py
--rw-r--r--   0        0        0    11057 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
--rw-r--r--   0        0        0     1369 2023-07-03 07:15:42.313327 guarddog-1.2/guarddog/analyzer/metadata/pypi/single_python_file.py
--rw-r--r--   0        0        0     3490 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/metadata/pypi/typosquatting.py
--rw-r--r--   0        0        0      438 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/metadata/release_zero.py
--rw-r--r--   0        0        0      743 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/metadata/repository_integrity_mismatch.py
--rw-r--r--   0        0        0   373303 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/metadata/resources/top_npm_packages.json
--rw-r--r--   0        0        0   387251 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/metadata/resources/top_pypi_packages.json
--rw-r--r--   0        0        0     5620 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/metadata/typosquatting.py
--rw-r--r--   0        0        0      889 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/__init__.py
--rw-r--r--   0        0        0      682 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/cmd-overwrite.yml
--rw-r--r--   0        0        0     4599 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/code-execution.yml
--rw-r--r--   0        0        0     1806 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/download-executable.yml
--rw-r--r--   0        0        0     2269 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/exec-base64.yml
--rw-r--r--   0        0        0     1786 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
--rw-r--r--   0        0        0      576 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/npm-exec-base64.yml
--rw-r--r--   0        0        0      716 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/npm-install-script.yml
--rw-r--r--   0        0        0      835 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
--rw-r--r--   0        0        0     3513 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
--rw-r--r--   0        0        0      582 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/obfuscation.yml
--rw-r--r--   0        0        0      926 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/shady-links.yml
--rw-r--r--   0        0        0      418 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/silent-process-execution.yml
--rw-r--r--   0        0        0      606 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/analyzer/sourcecode/steganography.yml
--rw-r--r--   0        0        0    11907 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/cli.py
--rw-r--r--   0        0        0      315 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/ecosystems.py
--rw-r--r--   0        0        0        0 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/reporters/__init__.py
--rw-r--r--   0        0        0     6185 2023-07-03 07:15:42.317327 guarddog-1.2/guarddog/reporters/sarif.py
--rw-r--r--   0        0        0      752 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/scanners/__init__.py
--rw-r--r--   0        0        0     1968 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/scanners/npm_package_scanner.py
--rw-r--r--   0        0        0     2243 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/scanners/npm_project_scanner.py
--rw-r--r--   0        0        0     2699 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/scanners/pypi_package_scanner.py
--rw-r--r--   0        0        0     5487 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/scanners/pypi_project_scanner.py
--rw-r--r--   0        0        0    11176 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/scanners/scanner.py
--rw-r--r--   0        0        0        0 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/utils/__init__.py
--rw-r--r--   0        0        0     1323 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/utils/archives.py
--rw-r--r--   0        0        0       54 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/utils/exceptions.py
--rw-r--r--   0        0        0      953 2023-07-03 07:15:42.321327 guarddog-1.2/guarddog/utils/package_info.py
--rw-r--r--   0        0        0       52 2023-07-03 07:15:42.321327 guarddog-1.2/pypi.rst
--rw-r--r--   0        0        0     1302 2023-07-03 07:15:54.413624 guarddog-1.2/pyproject.toml
--rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 guarddog-1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-04 14:39:05.505046 guarddog-1.2.1/LICENSE
+-rw-r--r--   0        0        0      314 2023-07-04 14:39:05.505046 guarddog-1.2.1/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0      154 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/__init__.py
+-rw-r--r--   0        0        0      246 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/__init__.py
+-rw-r--r--   0        0        0     9679 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/analyzer.py
+-rw-r--r--   0        0        0      457 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/__init__.py
+-rw-r--r--   0        0        0      609 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/detector.py
+-rw-r--r--   0        0        0     1166 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/empty_information.py
+-rw-r--r--   0        0        0      696 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/npm/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/npm/empty_information.py
+-rw-r--r--   0        0        0     1176 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      578 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/npm/release_zero.py
+-rw-r--r--   0        0        0     1732 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/npm/typosquatting.py
+-rw-r--r--   0        0        0     4153 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      976 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/pypi/__init__.py
+-rw-r--r--   0        0        0      723 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/pypi/empty_information.py
+-rw-r--r--   0        0        0     1803 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      716 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/pypi/release_zero.py
+-rw-r--r--   0        0        0    11057 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0     1369 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/pypi/single_python_file.py
+-rw-r--r--   0        0        0     3490 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/pypi/typosquatting.py
+-rw-r--r--   0        0        0      438 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/release_zero.py
+-rw-r--r--   0        0        0      743 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0   373303 2023-07-04 14:39:05.509045 guarddog-1.2.1/guarddog/analyzer/metadata/resources/top_npm_packages.json
+-rw-r--r--   0        0        0   387251 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/metadata/resources/top_pypi_packages.json
+-rw-r--r--   0        0        0     5620 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/metadata/typosquatting.py
+-rw-r--r--   0        0        0      889 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/__init__.py
+-rw-r--r--   0        0        0      682 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/cmd-overwrite.yml
+-rw-r--r--   0        0        0     4599 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/code-execution.yml
+-rw-r--r--   0        0        0     1806 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/download-executable.yml
+-rw-r--r--   0        0        0     2269 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/exec-base64.yml
+-rw-r--r--   0        0        0     1786 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
+-rw-r--r--   0        0        0      576 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/npm-exec-base64.yml
+-rw-r--r--   0        0        0      716 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/npm-install-script.yml
+-rw-r--r--   0        0        0      835 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
+-rw-r--r--   0        0        0     3513 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
+-rw-r--r--   0        0        0      582 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/obfuscation.yml
+-rw-r--r--   0        0        0      926 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/shady-links.yml
+-rw-r--r--   0        0        0      418 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/silent-process-execution.yml
+-rw-r--r--   0        0        0      606 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/analyzer/sourcecode/steganography.yml
+-rw-r--r--   0        0        0    11907 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/cli.py
+-rw-r--r--   0        0        0      315 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/ecosystems.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/reporters/__init__.py
+-rw-r--r--   0        0        0     6185 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/reporters/sarif.py
+-rw-r--r--   0        0        0      752 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/scanners/__init__.py
+-rw-r--r--   0        0        0     1968 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/scanners/npm_package_scanner.py
+-rw-r--r--   0        0        0     2243 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/scanners/npm_project_scanner.py
+-rw-r--r--   0        0        0     2699 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/scanners/pypi_package_scanner.py
+-rw-r--r--   0        0        0     5487 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/scanners/pypi_project_scanner.py
+-rw-r--r--   0        0        0    11176 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/utils/__init__.py
+-rw-r--r--   0        0        0     1323 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/utils/archives.py
+-rw-r--r--   0        0        0       54 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/utils/exceptions.py
+-rw-r--r--   0        0        0      953 2023-07-04 14:39:05.513045 guarddog-1.2.1/guarddog/utils/package_info.py
+-rw-r--r--   0        0        0       52 2023-07-04 14:39:05.517046 guarddog-1.2.1/pypi.rst
+-rw-r--r--   0        0        0     1304 2023-07-04 14:39:19.661171 guarddog-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1233 1970-01-01 00:00:00.000000 guarddog-1.2.1/PKG-INFO
```

### Comparing `guarddog-1.2/LICENSE` & `guarddog-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/analyzer.py` & `guarddog-1.2.1/guarddog/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/detector.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/detector.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/empty_information.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/npm/__init__.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/npm/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/npm/empty_information.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/npm/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/npm/release_zero.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/npm/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/npm/typosquatting.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/npm/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/potentially_compromised_email_domain.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/pypi/__init__.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/pypi/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/pypi/empty_information.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/pypi/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/pypi/release_zero.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/pypi/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/pypi/single_python_file.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/pypi/single_python_file.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/pypi/typosquatting.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/pypi/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/repository_integrity_mismatch.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/resources/top_npm_packages.json` & `guarddog-1.2.1/guarddog/analyzer/metadata/resources/top_npm_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/resources/top_pypi_packages.json` & `guarddog-1.2.1/guarddog/analyzer/metadata/resources/top_pypi_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/metadata/typosquatting.py` & `guarddog-1.2.1/guarddog/analyzer/metadata/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/__init__.py` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/cmd-overwrite.yml` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/cmd-overwrite.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/code-execution.yml` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/code-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/download-executable.yml` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/download-executable.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/exec-base64.yml` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/npm-exec-base64.yml` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/npm-exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/npm-install-script.yml` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/npm-install-script.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/npm-serialize-environment.yml` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/npm-serialize-environment.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/obfuscation.yml` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/obfuscation.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/shady-links.yml` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/shady-links.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/analyzer/sourcecode/steganography.yml` & `guarddog-1.2.1/guarddog/analyzer/sourcecode/steganography.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/cli.py` & `guarddog-1.2.1/guarddog/cli.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/reporters/sarif.py` & `guarddog-1.2.1/guarddog/reporters/sarif.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/scanners/__init__.py` & `guarddog-1.2.1/guarddog/scanners/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/scanners/npm_package_scanner.py` & `guarddog-1.2.1/guarddog/scanners/npm_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/scanners/npm_project_scanner.py` & `guarddog-1.2.1/guarddog/scanners/npm_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/scanners/pypi_package_scanner.py` & `guarddog-1.2.1/guarddog/scanners/pypi_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/scanners/pypi_project_scanner.py` & `guarddog-1.2.1/guarddog/scanners/pypi_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/scanners/scanner.py` & `guarddog-1.2.1/guarddog/scanners/scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/utils/archives.py` & `guarddog-1.2.1/guarddog/utils/archives.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/guarddog/utils/package_info.py` & `guarddog-1.2.1/guarddog/utils/package_info.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.2/pyproject.toml` & `guarddog-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "guarddog"
 description = "GuardDog is a CLI tool to Identify malicious PyPI packages"
 authors = ["Ellen Wang", "Christophe Tafani-Dereeper"]
 license = "Apache-2.0"
 readme = "pypi.rst"
 repository = "https://github.com/DataDog/guarddog"
-version = "v1.2"
+version = "v1.2.1"
 
 [tool.poetry.scripts]
 guarddog = "guarddog.cli:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 # NOTE: Before https://github.com/returntocorp/semgrep/issues/6631 is addressed, we can't seem to upgrade past 0.112.1
```

### Comparing `guarddog-1.2/PKG-INFO` & `guarddog-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guarddog
-Version: 1.2
+Version: 1.2.1
 Summary: GuardDog is a CLI tool to Identify malicious PyPI packages
 Home-page: https://github.com/DataDog/guarddog
 License: Apache-2.0
 Author: Ellen Wang
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

