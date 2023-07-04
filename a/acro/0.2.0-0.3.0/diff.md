# Comparing `tmp/acro-0.2.0.tar.gz` & `tmp/acro-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acro-0.2.0.tar", last modified: Wed Jun 28 15:01:33 2023, max compression
+gzip compressed data, was "acro-0.3.0.tar", last modified: Tue Jul  4 13:23:06 2023, max compression
```

## Comparing `acro-0.2.0.tar` & `acro-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-28 15:01:33.486188 acro-0.2.0/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-09-08 13:00:24.000000 acro-0.2.0/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3129 2023-06-28 15:01:33.486188 acro-0.2.0/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2227 2023-06-28 14:56:03.000000 acro-0.2.0/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-28 15:01:33.486188 acro-0.2.0/acro/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       32 2023-03-13 11:57:55.000000 acro-0.2.0/acro/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    28771 2023-06-28 14:56:29.000000 acro-0.2.0/acro/acro.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1072 2023-04-18 18:15:41.000000 acro-0.2.0/acro/default.yaml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    14979 2023-06-28 14:56:03.000000 acro-0.2.0/acro/record.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9107 2023-06-28 14:56:03.000000 acro-0.2.0/acro/utils.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-28 15:01:33.486188 acro-0.2.0/acro.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3129 2023-06-28 15:01:33.000000 acro-0.2.0/acro.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      294 2023-06-28 15:01:33.000000 acro-0.2.0/acro.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-06-28 15:01:33.000000 acro-0.2.0/acro.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       46 2023-06-28 15:01:33.000000 acro-0.2.0/acro.egg-info/requires.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-06-28 15:01:33.000000 acro-0.2.0/acro.egg-info/top_level.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-06-28 15:01:33.486188 acro-0.2.0/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-06-28 14:56:03.000000 acro-0.2.0/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-06-28 15:01:33.486188 acro-0.2.0/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2022-09-26 11:44:01.000000 acro-0.2.0/test/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2058 2023-05-08 20:18:08.000000 acro-0.2.0/test/stata.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11152 2023-06-28 14:56:03.000000 acro-0.2.0/test/test_initial.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-04 13:23:06.670482 acro-0.3.0/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-09-08 13:00:24.000000 acro-0.3.0/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3129 2023-07-04 13:23:06.670482 acro-0.3.0/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2227 2023-06-28 14:56:03.000000 acro-0.3.0/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-04 13:23:06.670482 acro-0.3.0/acro/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       32 2023-06-30 14:21:04.000000 acro-0.3.0/acro/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    31733 2023-07-03 21:17:41.000000 acro-0.3.0/acro/acro.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1072 2023-06-29 14:07:18.000000 acro-0.3.0/acro/default.yaml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    15983 2023-07-04 13:10:14.000000 acro-0.3.0/acro/record.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10248 2023-07-04 13:10:14.000000 acro-0.3.0/acro/utils.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-04 13:23:06.670482 acro-0.3.0/acro.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3129 2023-07-04 13:23:06.000000 acro-0.3.0/acro.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      323 2023-07-04 13:23:06.000000 acro-0.3.0/acro.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-07-04 13:23:06.000000 acro-0.3.0/acro.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       46 2023-07-04 13:23:06.000000 acro-0.3.0/acro.egg-info/requires.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-07-04 13:23:06.000000 acro-0.3.0/acro.egg-info/top_level.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-07-04 13:23:06.670482 acro-0.3.0/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-07-04 13:18:25.000000 acro-0.3.0/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-07-04 13:23:06.670482 acro-0.3.0/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2022-09-26 11:44:01.000000 acro-0.3.0/test/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2056 2023-06-30 14:25:22.000000 acro-0.3.0/test/stata.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12940 2023-07-04 13:10:14.000000 acro-0.3.0/test/test_initial.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8932 2023-07-03 19:49:42.000000 acro-0.3.0/test/test_stata_interface.py
```

### Comparing `acro-0.2.0/LICENSE` & `acro-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acro-0.2.0/PKG-INFO` & `acro-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acro
-Version: 0.2.0
+Version: 0.3.0
 Summary: ACRO: Tools for the Automatic Checking of Research Outputs
 Home-page: https://github.com/AI-SDC/ACRO
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `acro-0.2.0/README.md` & `acro-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `acro-0.2.0/acro/acro.py` & `acro-0.3.0/acro/acro.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ACRO: Automatic Checking of Research Outputs."""
 
 import logging
 import pathlib
 import warnings
+from collections.abc import Callable
 from inspect import stack
 
 import pandas as pd
 import statsmodels.api as sm
 import statsmodels.formula.api as smf
 import yaml
 from pandas import DataFrame
@@ -15,14 +16,15 @@
 from statsmodels.regression.linear_model import RegressionResultsWrapper
 
 from . import utils
 from .record import Records
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("acro")
+warnings.simplefilter(action="ignore", category=FutureWarning)
 
 
 class ACRO:
     """ACRO: Automatic Checking of Research Outputs.
 
     Attributes
     ----------
@@ -37,29 +39,33 @@
     --------
     >>> acro = ACRO()
     >>> results = acro.ols(y, x)
     >>> results.summary()
     >>> acro.finalise("MYFOLDER", "json")
     """
 
-    def __init__(self, config: str = "default") -> None:
+    def __init__(self, config: str = "default", suppress: bool = False) -> None:
         """Constructs a new ACRO object and reads parameters from config.
 
         Parameters
         ----------
         config : str
             Name of a yaml configuration file with safe parameters.
+        suppress : bool, default False
+            Whether to automatically apply suppression.
         """
         self.config: dict = {}
         self.results: Records = Records()
+        self.suppress: bool = suppress
         path = pathlib.Path(__file__).with_name(config + ".yaml")
         logger.debug("path: %s", path)
         with open(path, encoding="utf-8") as handle:
             self.config = yaml.load(handle, Loader=yaml.loader.SafeLoader)
         logger.info("config: %s", self.config)
+        logger.info("automatic suppression: %s", self.suppress)
         # set globals needed for aggregation functions
         utils.THRESHOLD = self.config["safe_threshold"]
         utils.SAFE_PRATIO_P = self.config["safe_pratio_p"]
         utils.SAFE_NK_N = self.config["safe_nk_n"]
         utils.SAFE_NK_K = self.config["safe_nk_k"]
         utils.CHECK_MISSING_VALUES = self.config["check_missing_values"]
 
@@ -157,18 +163,19 @@
         -------
         DataFrame
             Cross tabulation of the data.
         """
         logger.debug("crosstab()")
         command: str = utils.get_command("crosstab()", stack())
 
-        aggfunc = utils.get_aggfunc(aggfunc)  # convert string to function
+        # convert [list of] string to [list of] function
+        aggfunc = utils.get_aggfuncs(aggfunc)
 
         # requested table
-        table: DataFrame = pd.crosstab(
+        table: DataFrame = pd.crosstab(  # type: ignore
             index,
             columns,
             values,
             rownames,
             colnames,
             aggfunc,
             margins,
@@ -176,57 +183,97 @@
             dropna,
             normalize,
         )
 
         # suppression masks to apply based on the following checks
         masks: dict[str, DataFrame] = {}
 
-        # threshold check
-        t_values = pd.crosstab(
-            index,
-            columns,
-            None,
-            rownames,
-            colnames,
-            None,
-            margins,
-            margins_name,
-            dropna,
-            normalize,
-        )
-        t_values = t_values < utils.THRESHOLD
-        masks["threshold"] = t_values
-
         if aggfunc is not None:
+            # create lists with single entry for when there is only one aggfunc
+            freq_funcs: list[Callable] = [utils.AGGFUNC["freq"]]
+            neg_funcs: list[Callable] = [utils.agg_negative]
+            pperc_funcs: list[Callable] = [utils.agg_p_percent]
+            nk_funcs: list[Callable] = [utils.agg_nk]
+            missing_funcs: list[Callable] = [utils.agg_missing]
+            # then expand them to deal with extra columns as needed
+            if isinstance(aggfunc, list):
+                num = len(aggfunc)
+                freq_funcs.extend([utils.AGGFUNC["freq"] for i in range(1, num)])
+                neg_funcs.extend([utils.agg_negative for i in range(1, num)])
+                pperc_funcs.extend([utils.agg_p_percent for i in range(1, num)])
+                nk_funcs.extend([utils.agg_nk for i in range(1, num)])
+                missing_funcs.extend([utils.agg_missing for i in range(1, num)])
+            # threshold check- doesn't matter what we pass for value
+            t_values = pd.crosstab(  # type: ignore
+                index,
+                columns,
+                values=index,
+                rownames=rownames,
+                colnames=colnames,
+                aggfunc=freq_funcs,
+                margins=margins,
+                margins_name=margins_name,
+                dropna=dropna,
+                normalize=normalize,
+            )
+            t_values = t_values < utils.THRESHOLD
+            masks["threshold"] = t_values
             # check for negative values -- currently unsupported
-            negative = pd.crosstab(index, columns, values, aggfunc=utils.agg_negative)
+            negative = pd.crosstab(  # type: ignore
+                index, columns, values, aggfunc=neg_funcs, margins=margins
+            )
             if negative.to_numpy().sum() > 0:
                 masks["negative"] = negative
             # p-percent check
-            masks["p-ratio"] = pd.crosstab(
-                index, columns, values, aggfunc=utils.agg_p_percent
+            masks["p-ratio"] = pd.crosstab(  # type: ignore
+                index, columns, values, aggfunc=pperc_funcs, margins=margins
             )
             # nk values check
-            masks["nk-rule"] = pd.crosstab(index, columns, values, aggfunc=utils.agg_nk)
+            masks["nk-rule"] = pd.crosstab(  # type: ignore
+                index, columns, values, aggfunc=nk_funcs, margins=margins
+            )
             # check for missing values -- currently unsupported
             if utils.CHECK_MISSING_VALUES:
-                masks["missing"] = pd.crosstab(
-                    index, columns, values, aggfunc=utils.agg_missing
+                masks["missing"] = pd.crosstab(  # type: ignore
+                    index, columns, values, aggfunc=missing_funcs, margins=margins
                 )
+        else:
+            # threshold check- doesn't matter what we pass for value
+            t_values = pd.crosstab(  # type: ignore
+                index,
+                columns,
+                values=None,
+                rownames=rownames,
+                colnames=colnames,
+                aggfunc=None,
+                margins=margins,
+                margins_name=margins_name,
+                dropna=dropna,
+                normalize=normalize,
+            )
+            t_values = t_values < utils.THRESHOLD
+            masks["threshold"] = t_values
+
         # pd.crosstab returns nan for an empty cell
         for name, mask in masks.items():
             mask.fillna(value=1, inplace=True)
             mask = mask.astype(int)
             mask.replace({0: False, 1: True}, inplace=True)
             masks[name] = mask
 
-        table, outcome = utils.apply_suppression(table, masks)
-        properties: dict = {"method": "crosstab"}
-        status, summary = utils.get_summary(masks, properties)
-
+        # build the properties dictionary
+        properties: dict = {"method": "crosstab", "suppressed": self.suppress}
+        utils.update_table_properties(masks, properties)
+        # get the status and summary
+        status, summary = utils.get_summary(properties)
+        # apply the suppression
+        safe_table, outcome = utils.apply_suppression(table, masks)
+        if self.suppress:
+            table = safe_table
+        # record output
         self.results.add(
             status=status,
             output_type="table",
             properties=properties,
             command=command,
             summary=summary,
             outcome=outcome,
@@ -318,52 +365,66 @@
         )
 
         # suppression masks to apply based on the following checks
         masks: dict[str, DataFrame] = {}
 
         # threshold check
         agg = [utils.agg_threshold] * n_agg if n_agg > 1 else utils.agg_threshold
-        t_values = pd.pivot_table(data, values, index, columns, aggfunc=agg)
+        t_values = pd.pivot_table(  # type: ignore
+            data, values, index, columns, aggfunc=agg
+        )
         masks["threshold"] = t_values
 
         if aggfunc is not None:
             # check for negative values -- currently unsupported
             agg = [utils.agg_negative] * n_agg if n_agg > 1 else utils.agg_negative
-            negative = pd.pivot_table(data, values, index, columns, aggfunc=agg)
+            negative = pd.pivot_table(  # type: ignore
+                data, values, index, columns, aggfunc=agg
+            )
             if negative.to_numpy().sum() > 0:
                 masks["negative"] = negative
             # p-percent check
             agg = [utils.agg_p_percent] * n_agg if n_agg > 1 else utils.agg_p_percent
-            masks["p-ratio"] = pd.pivot_table(data, values, index, columns, aggfunc=agg)
+            masks["p-ratio"] = pd.pivot_table(  # type: ignore
+                data, values, index, columns, aggfunc=agg
+            )
             # nk values check
             agg = [utils.agg_nk] * n_agg if n_agg > 1 else utils.agg_nk
-            masks["nk-rule"] = pd.pivot_table(data, values, index, columns, aggfunc=agg)
+            masks["nk-rule"] = pd.pivot_table(  # type: ignore
+                data, values, index, columns, aggfunc=agg
+            )
             # check for missing values -- currently unsupported
             if utils.CHECK_MISSING_VALUES:
                 agg = [utils.agg_missing] * n_agg if n_agg > 1 else utils.agg_missing
-                masks["missing"] = pd.pivot_table(
+                masks["missing"] = pd.pivot_table(  # type: ignore
                     data, values, index, columns, aggfunc=agg
                 )
 
-        table, outcome = utils.apply_suppression(table, masks)
-        properties: dict = {"method": "pivot_table"}
-        status, summary = utils.get_summary(masks, properties)
-
+        # build the properties dictionary
+        properties: dict = {"method": "pivot_table", "suppressed": self.suppress}
+        utils.update_table_properties(masks, properties)
+        # get the status and summary
+        status, summary = utils.get_summary(properties)
+        # apply the suppression
+        safe_table, outcome = utils.apply_suppression(table, masks)
+        if self.suppress:
+            table = safe_table
+        # record output
         self.results.add(
             status=status,
             output_type="table",
             properties=properties,
             command=command,
             summary=summary,
             outcome=outcome,
             output=[table],
         )
         return table
 
-    def __check_model_dof(self, name: str, model) -> [str, str, float]:
+    def __check_model_dof(self, name: str, model) -> tuple[str, str, float]:
         """Check model DOF.
 
         Parameters
         ----------
         name : str
             The name of the model.
         model
@@ -754,15 +815,15 @@
     Parameters
     ----------
     data : array_like
         A column-ordered design matrix.
     prepend : bool
         If true, the constant is in the first column. Else the constant is
         appended (last column).
-    has_constant: str {'raise', 'add', 'skip'}
+    has_constant : str {'raise', 'add', 'skip'}
         Behavior if data already has a constant. The default will return
         data without adding another constant. If 'raise', will raise an
         error if any column has a constant value. Using 'add' will add a
         column of 1s if a constant column is present.
 
     Returns
     -------
```

### Comparing `acro-0.2.0/acro/default.yaml` & `acro-0.3.0/acro/default.yaml`

 * *Files identical despite different names*

### Comparing `acro-0.2.0/acro/record.py` & `acro-0.3.0/acro/record.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,68 +3,98 @@
 import datetime
 import json
 import logging
 import os
 import shutil
 import warnings
 from pathlib import Path
+from typing import Any
 
 import pandas as pd
 from pandas import DataFrame
 
-logger = logging.getLogger("acro::records")
+logger = logging.getLogger("acro:records")
 
 
 def load_outcome(outcome: dict) -> DataFrame:
     """Returns a DataFrame from an outcome dictionary.
 
     Parameters
     ----------
     outcome : dict
         The outcome to load as a DataFrame.
     """
     return pd.DataFrame.from_dict(outcome)
 
 
-def load_output(path: str, output: list[str]) -> str | list[DataFrame]:
+def load_output(path: str, output: list[str]) -> list[str] | list[DataFrame]:
     """Returns a loaded output.
 
     Parameters
     ----------
     path : str
         The path to the output folder (with results.json).
-    output : str
+    output : list[str]
         The output to load.
+
+    Returns
+    -------
+    list[str] | list[DataFrame]
+        The loaded output field.
     """
     if len(output) < 1:
         raise ValueError("error loading output")
-    loaded: str | list[DataFrame] = []
+    loaded: list[DataFrame] = []
     for filename in output:
         _, ext = os.path.splitext(filename)
         if ext == ".csv":
             filename = os.path.normpath(f"{path}/{filename}")
             loaded.append(pd.read_csv(filename))
-    if len(loaded) < 1:  # output was a path to custom file
-        loaded = output[0]
+    if len(loaded) < 1:  # output is path(s) to custom file(s)
+        return output
     return loaded
 
 
 class Record:  # pylint: disable=too-many-instance-attributes,too-few-public-methods
-    """Stores data related to a single output record."""
+    """Stores data related to a single output record.
+
+    Attributes
+    ----------
+    uid : str
+        Unique identifier.
+    status : str
+        SDC status: {"pass", "fail", "review"}
+    output_type : str
+        Type of output, e.g., "regression"
+    properties : dict
+        Dictionary containing structured output data.
+    command : str
+        String representation of the operation performed.
+    summary : str
+        String summarising the ACRO checks.
+    outcome : DataFrame
+        DataFrame describing the details of ACRO checks.
+    output : Any
+        List of output DataFrames.
+    comments : list[str] | None
+        List of strings entered by the user to add comments to the output.
+    timestamp : str
+        Time the record was created in ISO format.
+    """
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         uid: str,
         status: str,
         output_type: str,
         properties: dict,
         command: str,
         summary: str,
         outcome: DataFrame,
-        output: str | list[DataFrame],
+        output: list[str] | list[DataFrame],
         comments: list[str] | None = None,
     ) -> None:
         """Constructs a new output record.
 
         Parameters
         ----------
         uid : str
@@ -77,75 +107,76 @@
             Dictionary containing structured output data.
         command : str
             String representation of the operation performed.
         summary : str
             String summarising the ACRO checks.
         outcome : DataFrame
             DataFrame describing the details of ACRO checks.
-        output : str | list[DataFrame]
+        output : list[str] | list[DataFrame]
             List of output DataFrames.
         comments : list[str] | None, default None
             List of strings entered by the user to add comments to the output.
         """
         self.uid: str = uid
         self.status: str = status
         self.output_type: str = output_type
         self.properties: dict = properties
         self.command: str = command
         self.summary: str = summary
         self.outcome: DataFrame = outcome
-        self.output: str | list[DataFrame] = output
+        self.output: Any = output
         self.comments: list[str] = [] if comments is None else comments
         now = datetime.datetime.now()
         self.timestamp: str = now.isoformat()
 
     def serialize_output(self, path: str = "outputs") -> list[str]:
         """Serializes outputs.
 
         Parameters
         ----------
-        path : str
+        path : str, default 'outputs'
             Name of the folder that outputs are to be written.
 
         Returns
         -------
         list[str]
             List of filepaths of the written outputs.
         """
+        output: list[str] = []
         # check if the outputs directory was already created
         try:  # pragma: no cover
             os.makedirs(path)
             logger.debug("Directory %s created successfully", path)
         except FileExistsError:
             logger.debug("Directory %s already exists", path)
         # save each output DataFrame to a different csv
-        output = [self.output]
-        if not isinstance(self.output, str):
-            output = []
-            for i, _ in enumerate(self.output):
+        if all(isinstance(obj, DataFrame) for obj in self.output):
+            for i, data in enumerate(self.output):
                 filename = f"{self.uid}_{i}.csv"
                 output.append(filename)
                 filename = os.path.normpath(f"{path}/{filename}")
                 with open(filename, mode="w", newline="", encoding="utf-8") as file:
-                    file.write(self.output[i].to_csv())
+                    file.write(data.to_csv())
         # move custom files to the output folder
-        if self.output_type == "custom" and os.path.exists(self.output):
-            shutil.copy(self.output, path)
-            output = [Path(self.output).name]
+        if self.output_type == "custom":
+            for filename in self.output:
+                if os.path.exists(filename):
+                    shutil.copy(filename, path)
+                    output.append(Path(filename).name)
         return output
 
     def to_dict(self, path: str = "outputs", serialize: bool = True) -> dict:
         """Returns a dictionary representation of an output and serializes
         any DataFrame outputs as csv.
 
         Parameters
         ----------
         path : str
             Name of the folder that outputs are to be written.
-        serialize : bool
+        serialize : bool, default True
             Whether to serialize individual output DataFrames.
         """
         output = self.output
         if serialize:
             output = self.serialize_output(path)
         # convert to dictionary
         output_dict = {
@@ -175,15 +206,15 @@
         self,
         status: str,
         output_type: str,
         properties: dict,
         command: str,
         summary: str,
         outcome: DataFrame,
-        output: str | list[DataFrame],
+        output: list[str] | list[DataFrame],
         comments: list[str] | None = None,
     ) -> None:
         """Adds an output to the results.
 
         Parameters
         ----------
         status : str
@@ -194,33 +225,33 @@
             Dictionary containing structured output data.
         command : str
             String representation of the operation performed.
         summary : str
             String summarising the ACRO checks.
         outcome : DataFrame
             DataFrame describing the details of ACRO checks.
-        output : str | list[DataFrame]
+        output : list[str | list[DataFrame]
             List of output DataFrames.
-        comments : list[str], default None
+        comments : list[str] | None, default None
             List of strings entered by the user to add comments to the output.
         """
-        output = Record(
+        new = Record(
             uid=f"output_{self.output_id}",
             status=status,
             output_type=output_type,
             properties=properties,
             command=command,
             summary=summary,
             outcome=outcome,
             output=output,
             comments=comments,
         )
-        self.results[output.uid] = output
+        self.results[new.uid] = new
         self.output_id += 1
-        logger.info("add(): %s", output.uid)
+        logger.info("add(): %s", new.uid)
 
     def remove(self, key: str) -> None:
         """Removes an output from the results.
 
         Parameters
         ----------
         key : str
@@ -228,21 +259,26 @@
         """
         if key in self.results:
             del self.results[key]
             logger.info("remove(): %s removed", key)
         else:
             warnings.warn(f"unable to remove {key}, key not found", stacklevel=8)
 
-    def get(self, key: str) -> None:
+    def get(self, key: str) -> Record:
         """Returns a specified output from the results.
 
         Parameters
         ----------
         key : str
             Key specifying which output to return, e.g., 'output_0'.
+
+        Returns
+        -------
+        Record
+            The requested output.
         """
         logger.debug("get(): %s ", key)
         return self.results[key]
 
     def get_keys(self) -> list[str]:
         """Returns the list of available output keys.
 
@@ -263,40 +299,38 @@
             Position of the output to return.
 
         Returns
         -------
         Record
             The requested output.
         """
-        logger.debug("get_keys()")
+        logger.debug("get_index(): %s", index)
         key = list(self.results.keys())[index]
         return self.results[key]
 
     def add_custom(self, filename: str, comment: str | None = None) -> None:
         """Adds an unsupported output to the results dictionary.
 
         Parameters
         ----------
         filename : str
             The name of the file that will be added to the list of the outputs.
         comment : str | None, default None
             An optional comment.
         """
-        if comment is not None:
-            comment = [comment]
         output = Record(
             uid=f"output_{self.output_id}",
             status="review",
             output_type="custom",
             properties={},
             command="custom",
             summary="review",
             outcome=DataFrame(),
-            output=os.path.normpath(filename),
-            comments=comment,
+            output=[os.path.normpath(filename)],
+            comments=None if comment is None else [comment],
         )
         self.results[output.uid] = output
 
     def rename(self, old: str, new: str) -> None:
         """Rename an output.
 
         Parameters
```

### Comparing `acro-0.2.0/acro/utils.py` & `acro-0.3.0/acro/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """ACRO: Utility Functions."""
 
 import logging
 from collections.abc import Callable
-from inspect import getframeinfo
+from inspect import FrameInfo, getframeinfo
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame, Series
 from statsmodels.iolib.table import SimpleTable
 
 logger = logging.getLogger("acro")
 
 
 AGGFUNC: dict[str, Callable] = {
     "mean": np.mean,
     "median": np.median,
     "sum": np.sum,
     "std": np.std,
+    "freq": np.size,
 }
 
 # aggregation function parameters
 THRESHOLD: int = 10
 SAFE_PRATIO_P: float = 0.1
 SAFE_NK_N: int = 2
 SAFE_NK_K: float = 0.9
+CHECK_MISSING_VALUES: bool = False
 
 
-def get_command(default: str, stack_list: list[tuple]) -> str:
+def get_command(default: str, stack_list: list[FrameInfo]) -> str:
     """Returns the calling source line as a string.
 
     Parameters
     ----------
     default : str
         Default string to return if unable to extract the stack.
     stack_list : list[tuple]
@@ -212,56 +214,84 @@
             except TypeError:
                 logger.warning("problem mask %s is not binary", name)
         outcome_df = outcome_df.replace({"": "ok"})
     logger.info("outcome_df:\n%s", outcome_df)
     return safe_df, outcome_df
 
 
-def get_summary(masks: dict[str, DataFrame], properties: dict) -> [str, str]:
-    """Returns a string summarising the suppression masks.
+def update_table_properties(masks: dict[str, DataFrame], properties: dict) -> None:
+    """Updates the properties dictionary using the suppression masks.
 
     Parameters
     ----------
     masks : dict[str, DataFrame]
         Dictionary of tables specifying suppression masks for application.
     properties : dict
         Properties of the SDC checks.
+    """
+    # summary of cells to be suppressed
+    properties["negative"] = 0
+    properties["missing"] = 0
+    properties["threshold"] = 0
+    properties["p-ratio"] = 0
+    properties["nk-rule"] = 0
+    for name, mask in masks.items():
+        properties[name] = int(mask.to_numpy().sum())
+    # positions of cells to be suppressed
+    properties["sdc"] = {}
+    properties["sdc"]["negative"] = []
+    properties["sdc"]["missing"] = []
+    properties["sdc"]["threshold"] = []
+    properties["sdc"]["p-ratio"] = []
+    properties["sdc"]["nk-rule"] = []
+    for name, mask in masks.items():
+        true_positions = np.column_stack(np.where(mask.values))
+        for pos in true_positions:
+            row_index, col_index = pos
+            properties["sdc"][name].append([int(row_index), int(col_index)])
+
+
+def get_summary(properties: dict) -> tuple[str, str]:
+    """Returns the status and summary of the suppression masks.
+
+    Parameters
+    ----------
+    properties : dict
+        Properties of the SDC checks.
 
     Returns
     -------
     str
         Status: {"review", "fail", "pass"}.
     str
         Summary of the suppression masks.
     """
-    status = "review"
+    status: str = "pass"
     summary: str = ""
-    properties["negative"] = False
-    properties["missing"] = False
-    properties["threshold"] = 0
-    properties["p-ratio"] = 0
-    properties["nk-rule"] = 0
-    if "negative" in masks:
-        summary = "review; negative values found"
-        properties["negative"] = True
-    elif "missing" in masks:
-        summary = "review; missing values found"
-        properties["missing"] = True
+    sup: str = "suppressed" if properties["suppressed"] else "may need suppressing"
+    if properties["negative"]:
+        summary += "negative values found"
+        status = "review"
+    elif properties["missing"]:
+        summary += "missing values found"
+        status = "review"
     else:
-        for name, mask in masks.items():
-            n_cells = mask.to_numpy().sum()
-            if n_cells > 0:
-                summary += f"{name}: {n_cells} cells suppressed; "
-            properties[name] = int(n_cells)
-        if summary == "":
-            status = "pass"
-            summary = "pass"
-        else:
+        if properties["threshold"] > 0:
+            summary += f"threshold: {properties['threshold']} cells {sup}; "
+            status = "fail"
+        if properties["p-ratio"] > 0:
+            summary += f"p-ratio: {properties['p-ratio']} cells {sup}; "
             status = "fail"
-            summary = "fail; " + summary
+        if properties["nk-rule"] > 0:
+            summary += f"nk-rule: {properties['nk-rule']} cells {sup}; "
+            status = "fail"
+    if summary != "":
+        summary = f"{status}; {summary}"
+    else:
+        summary = status
     logger.info("get_summary(): %s", summary)
     return status, summary
 
 
 def get_aggfunc(aggfunc: str | None) -> Callable | None:
     """Checks whether an aggregation function is allowed and returns the
     appropriate function.
@@ -276,15 +306,15 @@
     Callable | None
         The aggregation function to apply.
     """
     logger.debug("get_aggfunc()")
     func = None
     if aggfunc is not None:
         if not isinstance(aggfunc, str) or aggfunc not in AGGFUNC:
-            raise ValueError(f"aggfunc must be: {', '.join(AGGFUNC.keys())}")
+            raise ValueError(f"aggfunc {aggfunc} must be: {', '.join(AGGFUNC.keys())}")
         func = AGGFUNC[aggfunc]
     logger.debug("aggfunc: %s", func)
     return func
 
 
 def get_aggfuncs(
     aggfuncs: str | list[str] | None,
```

### Comparing `acro-0.2.0/acro.egg-info/PKG-INFO` & `acro-0.3.0/acro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acro
-Version: 0.2.0
+Version: 0.3.0
 Summary: ACRO: Tools for the Automatic Checking of Research Outputs
 Home-page: https://github.com/AI-SDC/ACRO
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `acro-0.2.0/setup.py` & `acro-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="acro",
-    version="0.2.0",
+    version="0.3.0",
     license="MIT",
     maintainer="Jim Smith",
     maintainer_email="james.smith@uwe.ac.uk",
     description="ACRO: Tools for the Automatic Checking of Research Outputs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-SDC/ACRO",
```

### Comparing `acro-0.2.0/test/stata.py` & `acro-0.3.0/test/stata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 #!/usr/bin/env python
-"""
-ACRO Stata Tests.
-"""
+"""ACRO Stata Tests."""
 
 # ACRO Tests
 
 import os
 
 import pandas as pd
```

### Comparing `acro-0.2.0/test/test_initial.py` & `acro-0.3.0/test/test_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,36 +4,77 @@
 import os
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from acro import ACRO, add_constant, record, utils
-from acro.record import Record, Records
+from acro.record import Records
 
 # pylint: disable=redefined-outer-name
 
+PATH: str = "RES_PYTEST"
+
 
 @pytest.fixture
 def data() -> pd.DataFrame:
     """Load test data."""
     path = os.path.join("data", "test_data.dta")
     data = pd.read_stata(path)
     return data
 
 
 @pytest.fixture
 def acro() -> ACRO:
     """Initialise ACRO."""
-    return ACRO()
+    return ACRO(suppress=True)
+
+
+def test_crosstab_without_suppression(data):
+    """Crosstab threshold without automatic suppression."""
+    acro = ACRO(suppress=False)
+    _ = acro.crosstab(data.year, data.grant_type)
+    output = acro.results.get_index(0)
+    correct_summary: str = "fail; threshold: 6 cells may need suppressing; "
+    assert output.summary == correct_summary
+    assert 48 == output.output[0]["R/G"].sum()
+
+
+def test_crosstab_multiple_aggregate_function(data, acro):
+    """Crosstab with multiple agg funcs."""
+    acro = ACRO(suppress=False)
+
+    _ = acro.crosstab(
+        data.year, data.grant_type, values=data.inc_grants, aggfunc=["mean", "std"]
+    )
+    output = acro.results.get_index(0)
+    correct_summary: str = (
+        "fail; threshold: 12 cells may need suppressing;"
+        " p-ratio: 2 cells may need suppressing; "
+        "nk-rule: 2 cells may need suppressing; "
+    )
+    assert (
+        output.summary == correct_summary
+    ), f"\n{output.summary}\n should be \n{correct_summary}\n"
+    print(f"{output.output[0]['mean'][ 'R/G'].sum()}")
+    correctval = 97383496.0
+    errmsg = f"{output.output[0]['mean']['R/G'].sum()} should be {correctval}"
+    assert correctval == output.output[0]["mean"]["R/G"].sum(), errmsg
 
 
 def test_crosstab_threshold(data, acro):
     """Crosstab threshold test."""
     _ = acro.crosstab(data.year, data.grant_type)
+    output = acro.results.get_index(0)
+    total_nan: int = output.output[0]["R/G"].isnull().sum()
+    assert total_nan == 6
+    positions = output.properties["sdc"]["threshold"]
+    for pos in positions:
+        row, col = pos
+        assert np.isnan(output.output[0].iloc[row, col])
     results: Records = acro.finalise()
     correct_summary: str = "fail; threshold: 6 cells suppressed; "
     output = results.get_index(0)
     assert output.summary == correct_summary
 
 
 def test_crosstab_multiple(data, acro):
@@ -63,14 +104,25 @@
     correct_summary: str = "review; negative values found"
     output_0 = results.get_index(0)
     output_1 = results.get_index(1)
     assert output_0.summary == correct_summary
     assert output_1.summary == correct_summary
 
 
+def test_pivot_table_without_suppression(data):
+    """Pivot table without automatic suppression."""
+    acro = ACRO(suppress=False)
+    _ = acro.pivot_table(
+        data, index=["grant_type"], values=["inc_grants"], aggfunc=["mean", "std"]
+    )
+    output_0 = acro.results.get_index(0)
+    assert 36293992.0 == output_0.output[0]["mean"]["inc_grants"].sum()
+    assert "pass" == output_0.summary
+
+
 def test_pivot_table_pass(data, acro):
     """Pivot table pass test."""
     _ = acro.pivot_table(
         data, index=["grant_type"], values=["inc_grants"], aggfunc=["mean", "std"]
     )
     results: Records = acro.finalise()
     correct_summary: str = "pass"
@@ -110,15 +162,15 @@
     # OLSR
     results = acro.olsr(
         formula="inc_activity ~ inc_grants + inc_donations + total_costs", data=new_df
     )
     assert results.df_resid == 807
     assert results.rsquared == pytest.approx(0.894, 0.001)
     # Finalise
-    results: dict = acro.finalise()
+    results = acro.finalise()
     correct_summary: str = "pass; dof=807.0 >= 10"
     output_0 = results.get_index(0)
     output_1 = results.get_index(1)
     assert output_0.summary == correct_summary
     assert output_1.summary == correct_summary
 
 
@@ -152,33 +204,32 @@
     results = acro.logitr(
         formula="survivor ~ inc_activity + inc_grants + inc_donations + total_costs",
         data=new_df,
     )
     assert results.df_resid == 806
     assert results.prsquared == pytest.approx(0.214, 0.01)
     # Finalise
-    results: dict = acro.finalise()
+    results = acro.finalise()
     correct_summary: str = "pass; dof=806.0 >= 10"
     output_0 = results.get_index(0)
     output_1 = results.get_index(1)
     output_2 = results.get_index(2)
     output_3 = results.get_index(3)
     assert output_0.summary == correct_summary
     assert output_1.summary == correct_summary
     assert output_2.summary == correct_summary
     assert output_3.summary == correct_summary
 
 
 def test_finalise_excel(data, acro):
     """Finalise excel test."""
     _ = acro.crosstab(data.year, data.grant_type)
-    path: str = "RES_PYTEST"
-    results: Records = acro.finalise(path, "xlsx")
+    results: Records = acro.finalise(PATH, "xlsx")
     output_0 = results.get_index(0)
-    filename = os.path.normpath(f"{path}/results.xlsx")
+    filename = os.path.normpath(f"{PATH}/results.xlsx")
     load_data = pd.read_excel(filename, sheet_name=output_0.uid)
     correct_cell: str = "_ = acro.crosstab(data.year, data.grant_type)"
     assert load_data.iloc[0, 0] == "Command"
     assert load_data.iloc[0, 1] == correct_cell
 
 
 def test_output_removal(data, acro):
@@ -201,50 +252,47 @@
     # remove something that is not there
     with pytest.warns(UserWarning):
         acro.remove_output("123")
 
 
 def test_load_output():
     """Empty array when loading output."""
-    path: str = "RES_PYTEST"
     with pytest.raises(ValueError):
-        record.load_output(path, [])
+        record.load_output(PATH, [])
 
 
 def test_finalise_invalid(data, acro):
     """Invalid output format when finalising."""
     _ = acro.crosstab(data.year, data.grant_type)
-    path: str = "RES_PYTEST"
     with pytest.raises(ValueError):
-        _ = acro.finalise(path, "123")
+        _ = acro.finalise(PATH, "123")
 
 
 def test_finalise_json(data, acro):
     """Finalise json test."""
     _ = acro.crosstab(data.year, data.grant_type)
     # write JSON
-    path: str = "RES_PYTEST"
-    result: Records = acro.finalise(path, "json")
+    result: Records = acro.finalise(PATH, "json")
     # load JSON
     loaded: Records = Records()
-    loaded.load_json(path)
+    loaded.load_json(PATH)
     orig = result.get_index(0)
     read = loaded.get_index(0)
     # check equal
     assert orig.uid == read.uid
     assert orig.status == read.status
     assert orig.output_type == read.output_type
     assert orig.properties == read.properties
     assert orig.command == read.command
     assert orig.summary == read.summary
     assert orig.comments == read.comments
     assert orig.timestamp == read.timestamp
     assert (orig.output[0].reset_index()).equals(read.output[0])
     # test reading JSON
-    with open(os.path.normpath(f"{path}/results.json"), encoding="utf-8") as file:
+    with open(os.path.normpath(f"{PATH}/results.json"), encoding="utf-8") as file:
         json_data = json.load(file)
     assert json_data[orig.uid]["output"][0] == f"{orig.uid}_0.csv"
     # regression check: the outcome fields are dicts not strings
     assert json_data[orig.uid]["outcome"]["R/G"] == {
         "2010": "threshold; ",
         "2011": "threshold; ",
         "2012": "threshold; ",
@@ -253,55 +301,54 @@
         "2015": "threshold; ",
     }
 
 
 def test_rename_output(data, acro):
     """Output renaming test."""
     _ = acro.crosstab(data.year, data.grant_type)
-    results: Record = acro.finalise()
+    results: Records = acro.finalise()
     output_0 = results.get_index(0)
     orig_name = output_0.uid
     new_name = "cross_table"
     acro.rename_output(orig_name, new_name)
     results = acro.finalise()
     assert output_0.uid == new_name
     assert orig_name not in results.get_keys()
     assert os.path.exists(f"outputs/{new_name}_0.csv")
     # rename an output that doesn't exist
     with pytest.warns(UserWarning):
         acro.rename_output("123", "name")
 
 
 def test_add_comments(data, acro):
-    """Adding comments to output test"""
+    """Adding comments to output test."""
     _ = acro.crosstab(data.year, data.grant_type)
-    results: Record = acro.finalise()
+    results: Records = acro.finalise()
     output_0 = results.get_index(0)
     assert output_0.comments == []
     comment = "This is a cross table between year and grant_type"
     acro.add_comments(output_0.uid, comment)
     assert output_0.comments == [comment]
     comment_1 = "6 cells were suppressed"
     acro.add_comments(output_0.uid, comment_1)
     assert output_0.comments == [comment, comment_1]
     # add a comment to something that is not there
     with pytest.warns(UserWarning):
         acro.add_comments("123", "comment")
 
 
 def test_custom_output(acro):
-    """Adding an unsupported output to the results dictionary test"""
-    save_path = "RES_PYTEST"
+    """Adding an unsupported output to the results dictionary test."""
     filename = "notebooks/XandY.jfif"
     file_path = os.path.normpath(filename)
     acro.custom_output(filename)
-    results: Records = acro.finalise(path=save_path)
+    results: Records = acro.finalise(path=PATH)
     output_0 = results.get_index(0)
-    assert output_0.output == file_path
-    assert os.path.exists(os.path.normpath(f"{save_path}/XandY.jfif"))
+    assert output_0.output == [file_path]
+    assert os.path.exists(os.path.normpath(f"{PATH}/XandY.jfif"))
 
 
 def test_missing(data, acro):
     """Pivot table and Crosstab with negative values."""
     utils.CHECK_MISSING_VALUES = True
     data.loc[0:10, "inc_grants"] = np.NaN
     _ = acro.crosstab(
```

