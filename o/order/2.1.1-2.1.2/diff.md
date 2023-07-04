# Comparing `tmp/order-2.1.1.tar.gz` & `tmp/order-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "order-2.1.1.tar", last modified: Mon Feb 27 20:18:31 2023, max compression
+gzip compressed data, was "order-2.1.2.tar", last modified: Tue Jul  4 11:14:11 2023, max compression
```

## Comparing `order-2.1.1.tar` & `order-2.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:18:31.351694 order-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-27 20:18:22.000000 order-2.1.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-02-27 20:18:22.000000 order-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-27 20:18:22.000000 order-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-02-27 20:18:31.351694 order-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-02-27 20:18:22.000000 order-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:18:31.351694 order-2.1.1/order/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-02-27 20:18:22.000000 order-2.1.1/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-27 20:18:22.000000 order-2.1.1/order/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-02-27 20:18:22.000000 order-2.1.1/order/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-02-27 20:18:22.000000 order-2.1.1/order/category.py
--rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-02-27 20:18:22.000000 order-2.1.1/order/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-02-27 20:18:22.000000 order-2.1.1/order/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    43274 2023-02-27 20:18:22.000000 order-2.1.1/order/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-02-27 20:18:22.000000 order-2.1.1/order/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-02-27 20:18:22.000000 order-2.1.1/order/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    48112 2023-02-27 20:18:22.000000 order-2.1.1/order/unique.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-02-27 20:18:22.000000 order-2.1.1/order/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-02-27 20:18:22.000000 order-2.1.1/order/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:18:31.351694 order-2.1.1/order.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-02-27 20:18:31.000000 order-2.1.1/order.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-27 20:18:31.000000 order-2.1.1/order.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:18:31.000000 order-2.1.1/order.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:18:31.000000 order-2.1.1/order.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-27 20:18:31.000000 order-2.1.1/order.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-27 20:18:31.000000 order-2.1.1/order.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-27 20:18:22.000000 order-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:18:31.351694 order-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-02-27 20:18:22.000000 order-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:14:11.534315 order-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-04 11:14:01.000000 order-2.1.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-04 11:14:01.000000 order-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 11:14:01.000000 order-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-04 11:14:11.534315 order-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-04 11:14:01.000000 order-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:14:11.530315 order-2.1.2/order/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-04 11:14:01.000000 order-2.1.2/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-04 11:14:01.000000 order-2.1.2/order/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-04 11:14:01.000000 order-2.1.2/order/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-07-04 11:14:01.000000 order-2.1.2/order/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-04 11:14:01.000000 order-2.1.2/order/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11422 2023-07-04 11:14:01.000000 order-2.1.2/order/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43464 2023-07-04 11:14:01.000000 order-2.1.2/order/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-04 11:14:01.000000 order-2.1.2/order/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-07-04 11:14:01.000000 order-2.1.2/order/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50236 2023-07-04 11:14:01.000000 order-2.1.2/order/unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-07-04 11:14:01.000000 order-2.1.2/order/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-07-04 11:14:01.000000 order-2.1.2/order/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:14:11.534315 order-2.1.2/order.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-04 11:14:11.000000 order-2.1.2/order.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-04 11:14:11.000000 order-2.1.2/order.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:14:11.000000 order-2.1.2/order.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:14:11.000000 order-2.1.2/order.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 11:14:11.000000 order-2.1.2/order.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 11:14:11.000000 order-2.1.2/order.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 11:14:01.000000 order-2.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 11:14:11.534315 order-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-04 11:14:01.000000 order-2.1.2/setup.py
```

### Comparing `order-2.1.1/LICENSE` & `order-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `order-2.1.1/PKG-INFO` & `order-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: order
-Version: 2.1.1
+Version: 2.1.2
 Summary: Pythonic class collection that helps you structure external data from LHC / HEP experiments.
 Home-page: https://github.com/riga/order
 Author: Marcel Rieger
-Author-email: python-order@googlegroups.com
+Author-email: github.riga@icloud.com
 License: BSD-3-Clause
 Keywords: physics,analysis,experiment,order,structure,database,lhc,hep,alice,atlas,cms,lhcb
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: order Version: 2.1.1 Summary: Pythonic class
+Metadata-Version: 2.1 Name: order Version: 2.1.2 Summary: Pythonic class
 collection that helps you structure external data from LHC / HEP experiments.
 Home-page: https://github.com/riga/order Author: Marcel Rieger Author-email:
-python-order@googlegroups.com License: BSD-3-Clause Keywords:
+github.riga@icloud.com License: BSD-3-Clause Keywords:
 physics,analysis,experiment,order,structure,database,lhc,hep,alice,atlas,cms,lhcb
 Platform: UNKNOWN Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 2 Classifier: Programming Language :: Python
 :: 2.7 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `order-2.1.1/README.md` & `order-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `order-2.1.1/order/__init__.py` & `order-2.1.2/order/__init__.py`

 * *Files identical despite different names*

### Comparing `order-2.1.1/order/analysis.py` & `order-2.1.2/order/analysis.py`

 * *Files identical despite different names*

### Comparing `order-2.1.1/order/category.py` & `order-2.1.2/order/category.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,43 +108,44 @@
 
         cat2.selection
         # -> "(nJets == 4) && (nBTags == 2)"
 
     **Members**
 
     .. py:attribute:: channel
-       type: Channel, None
 
-       The channel instance of this category, or *None* when not set.
+        type: :py:class:`Channel`, None
+
+        The channel instance of this category, or *None* when not set.
 
     .. py:attribute:: full_label
-       type: string
-       read-only
 
-       The label of this category, prefix with the channel label if a channel is set.
+        type: string (read-only)
+
+        The label of this category, prefix with the channel label if a channel is set.
 
     .. py:attribute:: full_label_short
-       type: string
-       read-only
 
-       The short label of this category, prefix with the short channel label if a channel is set.
+        type: string (read-only)
+
+        The short label of this category, prefix with the short channel label if a channel is set.
 
     .. py:attribute:: full_label_root
-       type: string
-       read-only
 
-       The label of this category, prefix with the channel label if a channel is set, converted to
-       ROOT-style latex.
+        type: string (read-only)
+
+        The label of this category, prefix with the channel label if a channel is set, converted to
+        ROOT-style latex.
 
     .. py:attribute:: full_label_short_root
-       type: string
-       read-only
 
-       The short label of this category, prefix with the short channel label if a channel is set,
-       converted to ROOT-style latex.
+        type: string (read-only)
+
+        The short label of this category, prefix with the short channel label if a channel is set,
+        converted to ROOT-style latex.
     """
 
     cls_name_singular = "category"
     cls_name_plural = "categories"
 
     # attributes for copying
     copy_specs = (
```

### Comparing `order-2.1.1/order/config.py` & `order-2.1.2/order/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,22 +64,24 @@
 
         d.campaign == c
         # -> True
 
     **Members**
 
     .. py:attribute:: ecm
-       type: float
 
-       The center-of-mass energy in arbitrary units.
+        type: float
+
+        The center-of-mass energy in arbitrary units.
 
     .. py:attribute:: bx
-       type: float
 
-       The bunch crossing in arbitrary units.
+        type: float
+
+        The bunch crossing in arbitrary units.
     """
 
     cls_name_singular = "campaign"
     cls_name_plural = "campaigns"
 
     copy_specs = (
         [
@@ -228,25 +230,25 @@
         # with other values for that campaign, e.g. for sub-measurements
         cfg2 = analysis.add_config(campaign, name="sf_meausurement", id=2)
         ...
 
     **Members**
 
     .. py:attribute:: campaign
-       type: Campaign
-       read-only
 
-       The :py:class:`Campaign` instance this config belongs to.
+        type: :py:class:`Campaign` (read-only)
+
+        The :py:class:`Campaign` instance this config belongs to.
 
     .. py:attribute:: analysis
-       type: Analysis
-       read-only
 
-       The :py:class:`~order.analysis.Analysis` instance this config belongs to. When set, *this*
-       config is added to the index of configs of the analysis object.
+        type: :py:class:`Analysis` (read-only)
+
+        The :py:class:`~order.analysis.Analysis` instance this config belongs to. When set, *this*
+        config is added to the index of configs of the analysis object.
     """
 
     cls_name_singular = "config"
     cls_name_plural = "configs"
 
     copy_specs = (
         [
```

### Comparing `order-2.1.1/order/dataset.py` & `order-2.1.2/order/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,41 +114,43 @@
 
         d["scale_up"].n_files
         # -> 100
 
     **Members**
 
     .. py:attribute:: campaign
-       type: Campaign, None
 
-       The :py:class:`~order.config.Campaign` object this dataset belongs to. When set, *this*
-       dataset is also added to the dataset index of the campaign object.
+        type: :py:class:`Campaign`, None
+
+        The :py:class:`~order.config.Campaign` object this dataset belongs to. When set, *this*
+        dataset is also added to the dataset index of the campaign object.
 
     .. py:attribute:: info
-       type: dictionary
 
-       Mapping of shift names to :py:class:`DatasetInfo` instances.
+        type: dictionary
+
+        Mapping of shift names to :py:class:`DatasetInfo` instances.
 
     .. py:attribute:: keys
-       type: list
-       read-only
 
-       The dataset keys of the nominal :py:class:`DatasetInfo` object.
+        type: list (read-only)
+
+        The dataset keys of the nominal :py:class:`DatasetInfo` object.
 
     .. py:attribute:: n_files
-       type: integer
-       read-only
 
-       The number of files of the nominal :py:class:`DatasetInfo` object.
+        type: integer (read-only)
+
+        The number of files of the nominal :py:class:`DatasetInfo` object.
 
     .. py:attribute:: n_events
-       type: integer
-       read-only
 
-       The number of events of the nominal :py:class:`DatasetInfo` object.
+        type: integer (read-only)
+
+        The number of events of the nominal :py:class:`DatasetInfo` object.
     """
 
     cls_name_singular = "dataset"
     cls_name_plural = "datasets"
 
     # attributes for copying
     copy_specs = (
@@ -312,27 +314,30 @@
     **Copy behavior**
 
     All attributes are copied.
 
     **Members**
 
     .. py:attribute:: keys
-       type: list
 
-       The dataset keys, e.g. ``["/ttHTobb_M125.../.../..."]``.
+        type: list
+
+        The dataset keys, e.g. ``["/ttHTobb_M125.../.../..."]``.
 
     .. py:attribute:: n_files
-       type: integer
 
-       The number of files.
+        type: integer
+
+        The number of files.
 
     .. py:attribute:: n_events
-       type: integer
 
-       The number of events.
+        type: integer
+
+        The number of events.
     """
 
     copy_specs = (
         AuxDataMixin.copy_specs +
         TagMixin.copy_specs
     )
```

### Comparing `order-2.1.1/order/mixins.py` & `order-2.1.2/order/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,48 +40,55 @@
     When *skip* (*skip_shallow*) is *True*, the attribute is not copied when the source objects is
     copied through :py:meth:`CopyMixin.copy` (:py:meth:`CopyMixin.copy_shallow`). When skipped,
     the attribute of the copied object will be *skip_value*.
 
     **Members**
 
     .. py:attribute:: dst
-       type: string
 
-       The destination attribute.
+        type: string
+
+        The destination attribute.
 
     .. py:attribute:: src
-       type: string
 
-       The source attribute.
+        type: string
+
+        The source attribute.
 
     .. py:attribute:: ref
-       type: bool
 
-       Whether or not the attribute should be passed as a reference instead of being copied.
+        type: bool
+
+        Whether or not the attribute should be passed as a reference instead of being copied.
 
     .. py:attribute:: ref_placeholder
-       type: any
 
-       Placeholder value for attributes carried over as a reference that is used during the copying
-       process.
+        type: any
+
+        Placeholder value for attributes carried over as a reference that is used during the copying
+        process.
 
     .. py:attribute:: skip
-       type: bool
 
-       Whether or not the attribute is skipped when copied with :py:meth:`CopyMixin.copy`.
+        type: bool
+
+        Whether or not the attribute is skipped when copied with :py:meth:`CopyMixin.copy`.
 
     .. py:attribute:: skip_shallow
-       type: bool
 
-       Whether or not the attribute is skipped when copyied with :py:meth:`CopyMixin.copy_shallow`.
+        type: bool
+
+        Whether or not the attribute is skipped when copyied with :py:meth:`CopyMixin.copy_shallow`.
 
     .. py:attribute:: skip_value
-       type: any
 
-       Value to be used for attributes that are skipped in the copy process.
+        type: any
+
+        Value to be used for attributes that are skipped in the copy process.
     """
 
     @classmethod
     def new(cls, obj):
         if isinstance(obj, cls):
             return copy.copy(obj)
 
@@ -214,17 +221,18 @@
 
         c.complex_obj is None  # note the None here
         # -> True
 
     **Members**
 
     .. py:classattribute:: copy_specs
-       type: list
 
-       List of copy specifications per attribute.
+        type: list
+
+        List of copy specifications per attribute.
     """
 
     class Deferred(object):
 
         def __init__(self, func):
             self.func = func
 
@@ -369,23 +377,24 @@
 
         c.x.notthere
         # -> AttributeError
 
     **Members**
 
     .. py:attribute:: aux
-       type: OrderedDict
 
-       The dictionary of auxiliary data.
+        type: OrderedDict
+
+        The dictionary of auxiliary data.
 
     .. py:attribute:: x
-       type: DotAccessProxy
-       read-only
 
-       An object that provides simple attribute access to auxiliary data.
+        type: :py:class:`DotAccessProxy` (read-only)
+
+        An object that provides simple attribute access to auxiliary data.
     """
 
     _no_default = object()
     _no_value = object()
 
     copy_specs = []
 
@@ -492,18 +501,19 @@
 
         c.has_tag(("foo", "ba(r|z)"), mode=all, func="re")
         # -> True
 
     **Members**
 
     .. py:attribute:: tags
+
        type: set
 
-       The set of tags of this object. See :py:meth:`has_tag` for information about how to evaluate
-       them with patterns or regular expressions.
+        The set of tags of this object. See :py:meth:`has_tag` for information about how to evaluate
+        them with patterns or regular expressions.
     """
 
     copy_specs = []
 
     def __init__(self, tags=None):
         super(TagMixin, self).__init__()
 
@@ -582,43 +592,49 @@
         c.is_data = True
         c.data_source
         # -> "data"
 
     **Members**
 
     .. py:classattribute:: DATA_SOURCE_DATA
-       type: string
 
-       The data source string for data (``"data"``).
+        type: string
+
+        The data source string for data (``"data"``).
 
     .. py:classattribute:: DATA_SOURCE_MC
-       type: string
 
-       The data source string for mc (``"mc"``).
+        type: string
+
+        The data source string for mc (``"mc"``).
 
     .. py:classattribute:: allow_undefined_data_source
-       type: boolean
 
-       A configuration flag for this class that decides whether empty (*None*) data sources are
-       allowed. *False* by default.
+        type: boolean
+
+        A configuration flag for this class that decides whether empty (*None*) data sources are
+        allowed. *False* by default.
 
     .. py:attribute:: is_data
-       type: boolean
 
-       *True* if this object contains information on real data.
+        type: boolean
+
+        *True* if this object contains information on real data.
 
     .. py:attribute:: is_mc
-       type: boolean
 
-       *True* if this object contains information on MC data.
+        type: boolean
+
+        *True* if this object contains information on MC data.
 
     .. py:attribute:: data_source
-       type: string
 
-       Either *DATA_SOURCE_DATA* or *DATA_SOURCE_MC*, depending on the source of contained data.
+        type: string
+
+        Either *DATA_SOURCE_DATA* or *DATA_SOURCE_MC*, depending on the source of contained data.
     """
 
     DATA_SOURCE_DATA = "data"
     DATA_SOURCE_MC = "mc"
 
     # whether the data source is allowed to be undefined / None
     allow_undefined_data_source = False
@@ -718,41 +734,46 @@
         # -> None
         c.add_selection("myBranchB < 100")
         # -> TypeError
 
     **Members**
 
     .. py:classattribute:: MODE_ROOT
-       type: string
 
-       Flag denoting the ROOT-style selection mode (``"root"``).
+        type: string
+
+        Flag denoting the ROOT-style selection mode (``"root"``).
 
     .. py:classattribute:: MODE_NUMEXP
-       type: string
 
-       Flag denoting the numexpr-style selection mode (``"numexpr"``).
+        type: string
+
+        Flag denoting the numexpr-style selection mode (``"numexpr"``).
 
     .. py:classattribute:: default_str_selection_mode
-       type: string
 
-       The default *str_selection_mode* when none is given in the instance constructor. It is
-       initially set to *MODE_NUMEXPR* if :py:attr:`order.util.ROOT_DEFAULT` is *false*, or to
-       *MODE_ROOT* otherwise.
+        type: string
+
+        The default *str_selection_mode* when none is given in the instance constructor. It is
+        initially set to *MODE_NUMEXPR* if :py:attr:`order.util.ROOT_DEFAULT` is *false*, or to
+        *MODE_ROOT* otherwise.
 
     .. py:attribute:: selection
-       type: string, callable, list
 
-       The selection string, callable or a sequence of them. When a string,
-       :py:attr:`str_selection_mode` decides how the string is treated.
+        type: string, callable, list
+
+        The selection string, callable or a sequence of them. When a string,
+        :py:attr:`str_selection_mode` decides how the string is treated.
 
     .. py:attribute:: str_selection_mode
-       type: string, None
 
-       The selection mode. Should either be *MODE_ROOT* or *MODE_NUMEXPR*. Only considered when
-       :py:attr:`selection` is a string.
+        type: string, None
+
+        The selection mode. Should either be *MODE_ROOT* or *MODE_NUMEXPR*. Only considered when
+        :py:attr:`selection` is a string.
     """
 
     MODE_ROOT = "root"
     MODE_NUMEXPR = "numexpr"
 
     default_str_selection_mode = MODE_ROOT if ROOT_DEFAULT else MODE_NUMEXPR
 
@@ -872,35 +893,37 @@
         # conversion to ROOT-style latex
         l.label_short_root
         # -> "#mu"
 
     **Members**
 
     .. py:attribute:: label
-       type: string
 
-       The label. When this object has a *name* (configurable via *_label_fallback_attr*) attribute,
-       the label defaults to that value when not set.
+        type: string
+
+        The label. When this object has a *name* (configurable via *_label_fallback_attr*)
+        attribute, the label defaults to that value when not set.
 
     .. py:attribute:: label_root
-       type: string
-       read-only
 
-       The label, converted to ROOT-style latex.
+        type: string (read-only)
+
+        The label, converted to ROOT-style latex.
 
     .. py:attribute:: label_short
-       type: string
 
-       A short label, which defaults to the normal label when not set.
+        type: string
+
+        A short label, which defaults to the normal label when not set.
 
     .. py:attribute:: label_short_root
-       type: string
-       read-only
 
-       Short version of the label, converted to ROOT-style latex.
+        type: string (read-only)
+
+        Short version of the label, converted to ROOT-style latex.
     """
 
     copy_specs = []
 
     def __init__(self, label=None, label_short=None):
         super(LabelMixin, self).__init__()
 
@@ -994,192 +1017,228 @@
 
         c.color2_int
         # -> (0, 0, 255)
 
     **Members**
 
     .. py:attribute:: color1_r
-       type: float
 
-       Red component of the primary color.
+        type: float
+
+        Red component of the primary color.
 
     .. py:attribute:: color1_g
-       type: float
 
-       Green component of the primary color.
+        type: float
+
+        Green component of the primary color.
 
     .. py:attribute:: color1_b
-       type: float
 
-       Blue component of the primary color.
+        type: float
+
+        Blue component of the primary color.
 
     .. py:attribute:: color1_r_int
-       type: int
 
-       Red component of the primary color, converted to an integer in the [0, 255] range.
+        type: int
+
+        Red component of the primary color, converted to an integer in the [0, 255] range.
 
     .. py:attribute:: color1_g_int
-       type: int
 
-       Green component of the primary color, converted to an integer in the [0, 255] range.
+        type: int
+
+        Green component of the primary color, converted to an integer in the [0, 255] range.
 
     .. py:attribute:: color1_b_int
-       type: int
 
-       Blue component of the primary color, converted to an integer in the [0, 255] range.
+        type: int
+
+        Blue component of the primary color, converted to an integer in the [0, 255] range.
 
     .. py:attribute:: color1_alpha
-       type: float
 
-       The alpha value of the primary color, defaults to 1.0.
+        type: float
+
+        The alpha value of the primary color, defaults to 1.0.
 
     .. py:attribute:: color1
-       type: tuple (float)
 
-       The RGB values of the primary color in a 3-tuple.
+        type: tuple (float)
+
+        The RGB values of the primary color in a 3-tuple.
 
     .. py:attribute:: color1_int
-       type: tuple (int)
 
-       The RGB int values of the primary color in a 3-tuple.
+        type: tuple (int)
+
+        The RGB int values of the primary color in a 3-tuple.
 
     .. py:attribute:: color2_r
-       type: float
 
-       Red component of the secondary color.
+        type: float
+
+        Red component of the secondary color.
 
     .. py:attribute:: color2_g
-       type: float
 
-       Green component of the secondary color.
+        type: float
+
+        Green component of the secondary color.
 
     .. py:attribute:: color2_b
-       type: float
 
-       Blue component of the secondary color.
+        type: float
+
+        Blue component of the secondary color.
 
     .. py:attribute:: color2_r_int
-       type: int
 
-       Red component of the secondary color, converted to an integer in the [0, 255] range.
+        type: int
+
+        Red component of the secondary color, converted to an integer in the [0, 255] range.
 
     .. py:attribute:: color2_g_int
-       type: int
 
-       Green component of the secondary color, converted to an integer in the [0, 255] range.
+        type: int
+
+        Green component of the secondary color, converted to an integer in the [0, 255] range.
 
     .. py:attribute:: color2_b_int
-       type: int
 
-       Blue component of the secondary color, converted to an integer in the [0, 255] range.
+        type: int
+
+        Blue component of the secondary color, converted to an integer in the [0, 255] range.
 
     .. py:attribute:: color2_alpha
-       type: float
 
-       The alpha value of the secondary color, defaults to 1.0.
+        type: float
+
+        The alpha value of the secondary color, defaults to 1.0.
 
     .. py:attribute:: color2
-       type: tuple (float)
 
-       The RGB values of the secondary color in a 3-tuple.
+        type: tuple (float)
+
+        The RGB values of the secondary color in a 3-tuple.
 
     .. py:attribute:: color2_int
-       type: tuple (int)
 
-       The RGB int values of the secondary color in a 3-tuple.
+        type: tuple (int)
+
+        The RGB int values of the secondary color in a 3-tuple.
 
     .. py:attribute:: color3_r
-       type: float
 
-       Red component of the tertiary color.
+        type: float
+
+        Red component of the tertiary color.
 
     .. py:attribute:: color3_g
-       type: float
 
-       Green component of the tertiary color.
+        type: float
+
+        Green component of the tertiary color.
 
     .. py:attribute:: color3_b
-       type: float
 
-       Blue component of the tertiary color.
+        type: float
+
+        Blue component of the tertiary color.
 
     .. py:attribute:: color3_r_int
-       type: int
 
-       Red component of the tertiary color, converted to an integer in the [0, 255] range.
+        type: int
+
+        Red component of the tertiary color, converted to an integer in the [0, 255] range.
 
     .. py:attribute:: color3_g_int
-       type: int
 
-       Green component of the tertiary color, converted to an integer in the [0, 255] range.
+        type: int
+
+        Green component of the tertiary color, converted to an integer in the [0, 255] range.
 
     .. py:attribute:: color3_b_int
-       type: int
 
-       Blue component of the tertiary color, converted to an integer in the [0, 255] range.
+        type: int
+
+        Blue component of the tertiary color, converted to an integer in the [0, 255] range.
 
     .. py:attribute:: color3_alpha
-       type: float
 
-       The alpha value of the tertiary color, defaults to 1.0.
+        type: float
+
+        The alpha value of the tertiary color, defaults to 1.0.
 
     .. py:attribute:: color3
-       type: tuple (float)
 
-       The RGB values of the tertiary color in a 3-tuple.
+        type: tuple (float)
+
+        The RGB values of the tertiary color in a 3-tuple.
 
     .. py:attribute:: color3_int
-       type: tuple (int)
 
-       The RGB int values of the tertiary color in a 3-tuple.
+        type: tuple (int)
+
+        The RGB int values of the tertiary color in a 3-tuple.
 
     .. py:attribute:: color_r
-       type: float
 
-       Shorthand for :py:attr:`color1_r`.
+        type: float
+
+        Shorthand for :py:attr:`color1_r`.
 
     .. py:attribute:: color_g
-       type: float
 
-       Shorthand for :py:attr:`color1_g`.
+        type: float
+
+        Shorthand for :py:attr:`color1_g`.
 
     .. py:attribute:: color_b
-       type: float
 
-       Shorthand for :py:attr:`color1_b`.
+        type: float
+
+        Shorthand for :py:attr:`color1_b`.
 
     .. py:attribute:: color_r_int
-       type: int
 
-       Shorthand for :py:attr:`color1_r_int`.
+        type: int
+
+        Shorthand for :py:attr:`color1_r_int`.
 
     .. py:attribute:: color_g_int
-       type: int
 
-       Shorthand for :py:attr:`color1_g_int`.
+        type: int
+
+        Shorthand for :py:attr:`color1_g_int`.
 
     .. py:attribute:: color_b_int
-       type: int
 
-       Shorthand for :py:attr:`color1_b_int`.
+        type: int
+
+        Shorthand for :py:attr:`color1_b_int`.
 
     .. py:attribute:: color_alpha
-       type: float
 
-       Shorthand for :py:attr:`color1_alpha`.
+        type: float
+
+        Shorthand for :py:attr:`color1_alpha`.
 
     .. py:attribute:: color
-       type: tuple (float)
 
-       Shorthand for :py:attr:`color1`.
+        type: tuple (float)
+
+        Shorthand for :py:attr:`color1`.
 
     .. py:attribute:: color_int
-       type: tuple (int)
 
-       Shorthand for :py:attr:`color1_int`.
+        type: tuple (int)
+
+        Shorthand for :py:attr:`color1_int`.
     """
 
     default_color = (0.0, 0.0, 0.0, 1.0)
 
     copy_specs = []
 
     def __init__(self, color=None, color1=None, color2=None, color3=None):
```

### Comparing `order-2.1.1/order/process.py` & `order-2.1.2/order/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,17 +101,18 @@
 
         p2.has_parent_process("ttH")
         # -> True
 
     **Members**
 
     .. py:attribute:: xsecs
-       type: dictionary (float -> scinum.Number)
 
-       Cross sections mapped to a center-of-mass energies with arbitrary units.
+        type: dictionary (float -> :py:class:`scinum.Number`)
+
+        Cross sections mapped to a center-of-mass energies with arbitrary units.
     """
 
     cls_name_singular = "process"
     cls_name_plural = "processes"
 
     # attributes for copying
     copy_specs = (
```

### Comparing `order-2.1.1/order/shift.py` & `order-2.1.2/order/shift.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,98 +65,105 @@
 
         s.is_up
         # -> True
 
     **Members**
 
     .. py:classattribute:: NOMINAL
-       type: string
 
-       Flag denoting a nominal shift (``"nominal"``). Same as
-       `scinum.Number.NOMINAL <https://scinum.readthedocs.io/en/latest/#scinum.Number.NOMINAL>`__.
+        type: string
+
+        Flag denoting a nominal shift (``"nominal"``). Same as
+        `scinum.Number.NOMINAL <https://scinum.readthedocs.io/en/latest/#scinum.Number.NOMINAL>`__.
 
     .. py:classattribute:: UP
-       type: string
 
-       Flag denoting an up variation (``"up"``). Same as
-       `scinum.Number.UP <https://scinum.readthedocs.io/en/latest/#scinum.Number.UP>`__.
+        type: string
+
+        Flag denoting an up variation (``"up"``). Same as
+        `scinum.Number.UP <https://scinum.readthedocs.io/en/latest/#scinum.Number.UP>`__.
 
     .. py:classattribute:: DOWN
-       type: string
 
-       Flag denoting a down variation (``"down"``). Same as
-       `scinum.Number.DOWN <https://scinum.readthedocs.io/en/latest/#scinum.Number.DOWN>`__.
+        type: string
+
+        Flag denoting a down variation (``"down"``). Same as
+        `scinum.Number.DOWN <https://scinum.readthedocs.io/en/latest/#scinum.Number.DOWN>`__.
 
     .. py:classattribute:: RATE
-       type: string
 
-       Flag denoting a rate-changing effect (``"rate"``).
+        type: string
+
+        Flag denoting a rate-changing effect (``"rate"``).
 
     .. py:classattribute:: SHAPE
-       type: string
 
-       Flag denoting a shape-changing effect (``"shape"``).
+        type: string
+
+        Flag denoting a shape-changing effect (``"shape"``).
 
     .. py:classattribute:: RATE_SHAPE
-       type: string
 
-       Flag denoting a both rate- and shape-changing effect (``"rate_shape"``).
+        type: string
+
+        Flag denoting a both rate- and shape-changing effect (``"rate_shape"``).
 
     .. py:attribute:: source
-       type: string
-       read-only
 
-       The source of this shift, e.g. *NOMINAL*, ``"pdf"``, etc.
+        type: string (read-only)
+
+        The source of this shift, e.g. *NOMINAL*, ``"pdf"``, etc.
 
     .. py:attribute:: direction
-       type: string
-       read-only
 
-       The direction of this shift, either *NOMINAL*, *UP* or *DOWN*.
+        type: string (read-only)
+
+        The direction of this shift, either *NOMINAL*, *UP* or *DOWN*.
 
     .. py:attribute:: type
-       type: string
 
-       The type of this shift, either *RATE*, *SHAPE* or *RATE_SHAPE*.
+        type: string
+
+        The type of this shift, either *RATE*, *SHAPE* or *RATE_SHAPE*.
 
     .. py:attribute:: is_nominal
-       type: bool
-       read-only
 
-       Flag denoting if the shift is nominal.
+        type: bool (read-only)
+
+        Flag denoting if the shift is nominal.
 
     .. py:attribute:: is_up
-       type: bool
-       read-only
 
-       Flag denoting if the shift direction is *UP*.
+        type: bool (read-only)
+
+        Flag denoting if the shift direction is *UP*.
 
     .. py:attribute:: is_down
-       type: bool
-       read-only
 
-       Flag denoting if the shift direction is *DOWN*.
+        type: bool (read-only)
+
+        Flag denoting if the shift direction is *DOWN*.
 
     .. py:attribute:: is_rate
-       type: bool
-       read-only
 
-       Flag denoting if the shift type is rate-changing only.
+        type: bool (read-only)
+
+        Flag denoting if the shift type is rate-changing only.
 
     .. py:attribute:: is_shape
-       type: bool
-       read-only
 
-       Flag denoting if the shift type is shape-changing only.
+        type: bool (read-only)
+
+        Flag denoting if the shift type is shape-changing only.
 
     .. py:attribute:: is_rate_shape
-       type: bool
-       read-only
 
-       Flag denoting if the shift type is rate- and shape-changing.
+        type: bool (read-only)
+
+        Flag denoting if the shift type is rate- and shape-changing.
     """
 
     cls_name_singular = "shift"
     cls_name_plural = "shifts"
 
     # nominal flag
     NOMINAL = sn.Number.NOMINAL
@@ -186,17 +193,14 @@
 
         .. code-block:: python
 
             split_name("nominal")  # -> ("nominal", "nominal")
             split_name("pdf_up")   # -> ("pdf", "up")
             split_name("pdfup")    # -> ValueError: invalid shift name format: pdfup
         """
-        if name is None:
-            return (None, None)
-
         if name == cls.NOMINAL:
             return (cls.NOMINAL, cls.NOMINAL)
 
         if "_" in name:
             source, direction = tuple(name.rsplit("_", 1))
             if source == cls.NOMINAL:
                 raise ValueError("pointless nominal shift name: {}".format(name))
```

### Comparing `order-2.1.1/order/unique.py` & `order-2.1.2/order/unique.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "UniqueObject", "UniqueObjectIndex",
     "DuplicateObjectException", "DuplicateNameException", "DuplicateIdException",
     "unique_tree",
 ]
 
 
 import collections
+import warnings
 
 import six
 
 from order.mixins import CopyMixin
 from order.util import typed, make_list, class_id, DotAccessProxy
 
 
@@ -82,24 +83,24 @@
 
         idx.ids()
         # -> [1, 2]
 
     **Members**
 
     .. py:attribute:: cls
-       type: class
-       read-only
 
-       Class of objects hold by this index.
+        type: :py:class:`UniqueObjectMeta` (read-only)
+
+        Class of objects hold by this index.
 
     .. py:attribute:: n
-       type: DotAccessProxy
-       read-only
 
-       An object that provides simple attribute access to contained objects via name.
+        type: :py:class:`DotAccessProxy` (read-only)
+
+        An object that provides simple attribute access to contained objects via name.
     """
 
     copy_specs = [
         {"attr": "_cls", "ref": True},
     ]
 
     def __init__(self, cls, objects=None):
@@ -398,34 +399,36 @@
 
         obj.id
         # -> 2  # 1 is the previous maximum id
 
     **Members**
 
     .. py:classattribute:: cls_name_singular
-       type: str
 
-       The name of the unique object class in singular form, e.g. for producing automatic messages.
+        type: str
+
+        The name of the unique object class in singular form, e.g. for producing automatic messages.
 
     .. py:classattribute:: cls_name_plural
-       type: str
 
-       The name of the unique object class in plural form, e.g. for producing automatic messages.
+        type: str
+
+        The name of the unique object class in plural form, e.g. for producing automatic messages.
 
     .. py:attribute:: name
-       type: str
-       read-only
 
-       The unique name.
+        type: str (read-only)
+
+        The unique name.
 
     .. py:attribute:: id
-       type: int
-       read-only
 
-       The unique id.
+        type: int (read-only)
+
+        The unique id.
     """
 
     cls_name_singular = "unique_object"
     cls_name_plural = "unique_objects"
 
     AUTO_ID = "+"
 
@@ -706,27 +709,27 @@
         if deep_parents:
             decorated_cls._deep_child_classes.append(cls)
 
         # add attribute docs
         if decorated_cls.__doc__:
             decorated_cls.__doc__ += """
     .. py:attribute:: {plural}
-       type: UniqueObjectIndex
-       read-only
 
-       The :py:class:`~order.unique.UniqueObjectIndex` of child {plural}.
+        type: :py:class:`UniqueObjectIndex` (read-only)
+
+        The :py:class:`~order.unique.UniqueObjectIndex` of child {plural}.
     """.format(plural=plural)
 
             if parents:
                 decorated_cls.__doc__ += """
     .. py:attribute:: parent_{plural}
-       type: UniqueObjectIndex
-       read-only
 
-       The :py:class:`~order.unique.UniqueObjectIndex` of parent {plural}.
+        type: :py:class:`UniqueObjectIndex` (read-only)
+
+        The :py:class:`~order.unique.UniqueObjectIndex` of parent {plural}.
     """.format(plural=plural)
 
         #
         # helpers for child and parent methods
         #
 
         # extend helper
@@ -744,14 +747,63 @@
             return results
 
         # clear helper
         def _clear(self, remove_fn, index):
             for name in index.names():
                 remove_fn(name)
 
+        # walk helper
+        def _walk(self, next_fn, algo="bfs", depth_first=False, include_self=False):
+            # handle cases where the deprecated depth_first argument is used
+            if depth_first:
+                if algo != "bfs":
+                    raise Exception(
+                        "using both 'algo' and 'depth_first' arguments is ambiguous; " +
+                        "'depth_first' is deprecated; use 'algo=\"{}\" instead'".format(algo),
+                    )
+                warnings.warn(
+                    "the 'depth_first' attribute is deprecated; use 'algo=\"dfs\"' instead'",
+                    DeprecationWarning,
+                )
+                algo = "dfs"
+
+            # check the algo
+            if algo == "dfs":
+                algo = "dfs_preorder"
+            known_algos = ["bfs", "dfs_preorder", "dfs_postorder"]
+            if algo not in known_algos:
+                _known_algos = ", ".join(map("'{}'".format, known_algos))
+                raise ValueError(
+                    "unknown traversel order '{}', should be one of {}".format(algo, _known_algos),
+                )
+
+            lookup = collections.deque([(self, 0)])
+            visited = set()
+            while lookup:
+                obj, depth = lookup[0]
+                if obj in visited:
+                    lookup.popleft()
+                    continue
+
+                objs = list(next_fn(obj))
+                if algo == "dfs_postorder" and any(_obj not in visited for _obj in objs):
+                    lookup.extendleft((obj, depth + 1) for obj in reversed(objs))
+                    continue
+
+                if depth > 0 or include_self:
+                    yield (obj, depth, objs)
+                    visited.add(obj)
+
+                lookup.popleft()
+
+                if algo == "dfs_preorder":
+                    lookup.extendleft((obj, depth + 1) for obj in reversed(objs))
+                elif algo == "bfs":
+                    lookup.extend((obj, depth + 1) for obj in objs)
+
         #
         # child methods, independent of parents
         #
 
         # direct child index access
         @patch()
         @typed(setter=False, name=plural)
@@ -832,48 +884,49 @@
                 if default != _no_default:
                     return default
 
                 raise ValueError("unknown {}: {}".format(singular, obj))
 
             # walk children method
             @patch("walk_" + plural)
-            def walk(self, depth_first=False, include_self=False):
+            def walk(self, algo="bfs", depth_first=False, include_self=False):
                 """
                 Walks through the :py:attr:`{plural}` index and per iteration, yields a child
                 {singular}, its depth relative to *this* {singular}, and its child {plural} in a
-                list that can be modified to alter the walking. When *depth_first* is *True*,
-                iterate depth-first instead of the default breadth-first. When *include_self* is
-                *True*, also yield this {singular} instance with a depth of 0.
-                """
-                lookup = collections.deque([(self, 0)])
-                while lookup:
-                    obj, depth = lookup.popleft()
-                    objs = list(getattr(obj, plural).values())
-
-                    if include_self:
-                        yield (obj, depth, objs)
-                    else:
-                        include_self = True
-
-                    if depth_first:
-                        lookup.extendleft((obj, depth + 1) for obj in reversed(objs))
-                    else:
-                        lookup.extend((obj, depth + 1) for obj in objs)
+                list that can be modified to alter the walking.
+
+                The traversal order is defined by *algo* which allows different values (more
+                `info <https://en.wikipedia.org/wiki/Tree_traversal>`__):
+
+                    - ``"bfs"``: Breadth-first search.
+                    - ``"dfs"``: Alias for ``"dfs_preorder"``.
+                    - ``"dfs_preorder"``: Pre-order depth-first search.
+                    - ``"dfs_postorder"``: Post-order depth-first search.
+
+                When *include_self* is *True*, this {singular} instance is yielded as well with a
+                depth of 0.
+                """
+                return _walk(
+                    self,
+                    (lambda obj: getattr(obj, plural).values()),
+                    algo=algo,
+                    depth_first=depth_first,
+                    include_self=include_self,
+                )
 
             # get leaves method
             @patch("get_leaf_" + plural)
             def get_leaves(self):
                 """
                 Returns all child {plural} from the :py:attr:`{plural}` index that have no child
                 {plural} themselves in a recursive fashion. Possible duplicates due to nested
                 structures are removed.
                 """
-                walker = getattr(self, "walk_" + plural)()
                 leaves = []
-                for obj, _, objs in walker:
+                for obj, _, objs in getattr(self, "walk_" + plural)():
                     if not objs and obj not in leaves:
                         leaves.append(obj)
                 return leaves
 
         #
         # child methods, disabled parents
         #
@@ -1108,48 +1161,49 @@
                     if default != _no_default:
                         return default
 
                     raise ValueError("unknown {}: {}".format(singular, obj))
 
                 # walk parents method
                 @patch("walk_parent_" + plural)  # noqa: F811
-                def walk(self, depth_first=False, include_self=False):  # noqa: F811
+                def walk(self, algo="bfs", depth_first=False, include_self=False):  # noqa: F811
                     """
                     Walks through the :py:attr:`parent_{plural}` index and per iteration, yields a
                     parent {singular}, its depth relative to *this* {singular}, and its parent
-                    {plural} in a list that can be modified to alter the walking. When *depth_first*
-                    is *True*, iterate depth-first instead of the default breadth-first. When
-                    *include_self* is *True*, also yield this {singular} instance with a depth of 0.
+                    {plural} in a list that can be modified to alter the walking.
+
+                    The traversal order is defined by *algo* which allows different values (more
+                    `info <https://en.wikipedia.org/wiki/Tree_traversal>`__):
+
+                        - ``"bfs"``: Breadth-first search.
+                        - ``"dfs"``: Alias for ``"dfs_preorder"``.
+                        - ``"dfs_preorder"``: Pre-order depth-first search.
+                        - ``"dfs_postorder"``: Post-order depth-first search.
+
+                    When *include_self* is *True*, this {singular} instance is yielded as well with
+                    a depth of 0.
                     """
-                    lookup = collections.deque([(self, 0)])
-                    while lookup:
-                        obj, depth = lookup.popleft()
-                        objs = list(getattr(obj, "parent_" + plural).values())
-
-                        if include_self:
-                            yield (obj, depth, objs)
-                        else:
-                            include_self = True
-
-                        if depth_first:
-                            lookup.extendleft((obj, depth + 1) for obj in reversed(objs))
-                        else:
-                            lookup.extend((obj, depth + 1) for obj in objs)
+                    return _walk(
+                        self,
+                        (lambda obj: getattr(obj, "parent_" + plural).values()),
+                        algo=algo,
+                        depth_first=depth_first,
+                        include_self=include_self,
+                    )
 
                 # get roots method
                 @patch("get_root_" + plural)
                 def get_roots(self):
                     """
                     Returns all parent {plural} from the :py:attr:`parent_{plural}` index that have
                     no parent {plural} themselves in a recursive fashion. Possible duplicates due to
                     nested structures are removed.
                     """
-                    walker = getattr(self, "walk_parent_" + plural)()
                     roots = []
-                    for obj, _, objs in walker:
+                    for obj, _, objs in getattr(self, "walk_parent_" + plural)():
                         if not objs and obj not in roots:
                             roots.append(obj)
                     return roots
 
         #
         # parent methods, exactly 1 parent
         #
```

### Comparing `order-2.1.1/order/util.py` & `order-2.1.2/order/util.py`

 * *Files identical despite different names*

### Comparing `order-2.1.1/order/variable.py` & `order-2.1.2/order/variable.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,154 +82,168 @@
 
         v2.even_binning
         # -> False
 
     **Members**
 
     .. py:attribute:: expression
-       type: string, callable, None
 
-       The expression of this variable. Defaults to name if *None*.
+        type: string, callable, None
+
+        The expression of this variable. Defaults to name if *None*.
 
     .. py:attribute:: binning
-       type: tuple, list
 
-       Descibes the bin edges when given a list, or the number of bins, minimum value and maximum
-       value when passed a 3-tuple.
+        type: tuple, list
+
+        Descibes the bin edges when given a list, or the number of bins, minimum value and maximum
+        value when passed a 3-tuple.
 
     .. py:attribute:: even_binning
-       type: bool
-       read-only
 
-       Whether or not the binning is even.
+        type: bool (read-only)
+
+        Whether or not the binning is even.
 
     .. py:attribute:: x_title
-       type: string
 
-       The title of the x-axis in standard LaTeX format.
+        type: string
+
+        The title of the x-axis in standard LaTeX format.
 
     .. py:attribute:: x_title_root
-       type: string
-       read-only
 
-       The title of the x-axis, converted to ROOT-style latex.
+        type: string (read-only)
+
+        The title of the x-axis, converted to ROOT-style latex.
 
     .. py:attribute:: x_title_short
-       type: string
 
-       Short version for the title of the x-axis in standard LaTeX format. Defaults to *x_title*
-       when not explicitely set.
+        type: string
+
+        Short version for the title of the x-axis in standard LaTeX format. Defaults to *x_title*
+        when not explicitely set.
 
     .. py:attribute:: x_title_short_root
-       type: string
-       read-only
 
-       The short version of the title of the x-axis, converted to ROOT-style latex.
+        type: string (read-only)
+
+        The short version of the title of the x-axis, converted to ROOT-style latex.
 
     .. py:attribute:: y_title
-       type: string
 
-       The title of the y-axis in standard LaTeX format.
+        type: string
+
+        The title of the y-axis in standard LaTeX format.
 
     .. py:attribute:: y_title_root
-       type: string
-       read-only
 
-       The title of the y-axis, converted to ROOT-style latex.
+        type: string (read-only)
+
+        The title of the y-axis, converted to ROOT-style latex.
 
     .. py:attribute:: y_title_short
-       type: string
 
-       Short version for the title of the y-axis in standard LaTeX format. Defaults to *y_title*
-       when not explicitely set.
+        type: string
+
+        Short version for the title of the y-axis in standard LaTeX format. Defaults to *y_title*
+        when not explicitely set.
 
     .. py:attribute:: y_title_short_root
-       type: string
-       read-only
 
-       The short version of the title of the y-axis, converted to ROOT-style latex.
+        type: string (read-only)
+
+        The short version of the title of the y-axis, converted to ROOT-style latex.
 
     .. py:attribute:: x_labels
-       type: list, None
 
-       A list of custom bin labels or *None*.
+        type: list, None
+
+        A list of custom bin labels or *None*.
 
     .. py:attribute:: x_labels_root
-       type: list, None
-       read-only
 
-       A list of custom bin labels, converted to ROOT-style latex, or *None*.
+        type: list, None (read-only)
+
+        A list of custom bin labels, converted to ROOT-style latex, or *None*.
 
     .. py:attribute:: unit
-       type: string, None
 
-       The unit to be shown on both, x- and y-axis. When *None*, no unit is shown.
+        type: string, None
+
+        The unit to be shown on both, x- and y-axis. When *None*, no unit is shown.
 
     .. py:attribute:: unit_format
-       type: string
 
-       The format string for concatenating axis titles and units, e.g. ``"{title} / {unit}"``. The
-       format string must contain the fields *title* and *unit*.
+        type: string
+
+        The format string for concatenating axis titles and units, e.g. ``"{title} / {unit}"``. The
+        format string must contain the fields *title* and *unit*.
 
     .. py:attribute:: null_value
-       type: int, float, None
 
-       A configurable NULL value for this variable, possibly denoting missing values. *None* is
-       considered as "non-configured".
+        type: int, float, None
+
+        A configurable NULL value for this variable, possibly denoting missing values. *None* is
+        considered as "non-configured".
 
     .. py:attribute:: x_log
-       type: boolean
 
-       Whether or not the x-axis should be drawn logarithmically.
+        type: boolean
+
+        Whether or not the x-axis should be drawn logarithmically.
 
     .. py:attribute:: y_log
-       type: boolean
 
-       Whether or not the y-axis should be drawn logarithmically.
+        type: boolean
+
+        Whether or not the y-axis should be drawn logarithmically.
 
     .. py:attribute:: x_discrete
-       type: boolean
 
-       Whether or not the x-axis is partitioned by discrete values (i.e, an integer axis). There is
-       not constraint on the :py:attr:`binning` setting, but it should be set accordingly.
+        type: boolean
+
+        Whether or not the x-axis is partitioned by discrete values (i.e, an integer axis). There is
+        not constraint on the :py:attr:`binning` setting, but it should be set accordingly.
 
     .. py:attribute:: y_discrete
-       type: boolean
 
-       Whether or not the y-axis is partitioned by discrete values (i.e, an integer axis).
+        type: boolean
+
+        Whether or not the y-axis is partitioned by discrete values (i.e, an integer axis).
 
     .. py:attribute:: n_bins
-       type: int
-       read-only
 
-       The number of bins.
+        type: int (read-only)
+
+        The number of bins.
 
     .. py:attribute:: x_min
-       type: float
-       read-only
 
-       The minimum value of the x-axis.
+        type: float (read-only)
+
+        The minimum value of the x-axis.
 
     .. py:attribute:: x_max
-       type: float
-       read-only
 
-       The maximum value of the x-axis.
+        type: float (read-only)
+
+        The maximum value of the x-axis.
 
     .. py:attribute:: bin_width
-       type: float
-       read-only
 
-       The width of a bin.
+        type: float (read-only)
+
+        The width of a bin.
 
     .. py:attribute:: bin_edges
-       type: list
-       read-only
 
-       A list of the *n_bins* + 1 bin edges.
+        type: list (read-only)
+
+        A list of the *n_bins* + 1 bin edges.
     """
 
     cls_name_singular = "variable"
     cls_name_plural = "variables"
 
     # attributes for copying
     copy_specs = (
```

### Comparing `order-2.1.1/order.egg-info/PKG-INFO` & `order-2.1.2/order.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: order
-Version: 2.1.1
+Version: 2.1.2
 Summary: Pythonic class collection that helps you structure external data from LHC / HEP experiments.
 Home-page: https://github.com/riga/order
 Author: Marcel Rieger
-Author-email: python-order@googlegroups.com
+Author-email: github.riga@icloud.com
 License: BSD-3-Clause
 Keywords: physics,analysis,experiment,order,structure,database,lhc,hep,alice,atlas,cms,lhcb
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: order Version: 2.1.1 Summary: Pythonic class
+Metadata-Version: 2.1 Name: order Version: 2.1.2 Summary: Pythonic class
 collection that helps you structure external data from LHC / HEP experiments.
 Home-page: https://github.com/riga/order Author: Marcel Rieger Author-email:
-python-order@googlegroups.com License: BSD-3-Clause Keywords:
+github.riga@icloud.com License: BSD-3-Clause Keywords:
 physics,analysis,experiment,order,structure,database,lhc,hep,alice,atlas,cms,lhcb
 Platform: UNKNOWN Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 2 Classifier: Programming Language :: Python
 :: 2.7 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `order-2.1.1/setup.py` & `order-2.1.2/setup.py`

 * *Files identical despite different names*

