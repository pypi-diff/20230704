# Comparing `tmp/personal_knowledge_library-1.0.5.tar.gz` & `tmp/personal_knowledge_library-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_knowledge_library-1.0.5.tar", last modified: Mon Jul  3 14:40:01 2023, max compression
+gzip compressed data, was "personal_knowledge_library-1.0.6.tar", last modified: Tue Jul  4 15:09:00 2023, max compression
```

## Comparing `personal_knowledge_library-1.0.5.tar` & `personal_knowledge_library-1.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    43169 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.914117 personal_knowledge_library-1.0.5/knowledge/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.914117 personal_knowledge_library-1.0.5/knowledge/base/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/base/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/base/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    80585 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/base/ontology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.914117 personal_knowledge_library-1.0.5/knowledge/nel/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/nel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/nel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/nel/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.914117 personal_knowledge_library-1.0.5/knowledge/ontomapping/
--rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/ontomapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/ontomapping/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/knowledge/public/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/public/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/public/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/public/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)    44912 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/public/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/knowledge/services/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    20881 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/services/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/knowledge/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/utils/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/knowledge/utils/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-07-03 14:40:01.000000 personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-03 14:40:01.000000 personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:40:01.000000 personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-03 14:40:01.000000 personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 14:40:01.000000 personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 14:40:01.918117 personal_knowledge_library-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-03 14:39:48.000000 personal_knowledge_library-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:09:00.493784 personal_knowledge_library-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-07-04 15:09:00.493784 personal_knowledge_library-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43169 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:09:00.489784 personal_knowledge_library-1.0.6/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:09:00.489784 personal_knowledge_library-1.0.6/knowledge/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/base/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/base/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80585 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/base/ontology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:09:00.489784 personal_knowledge_library-1.0.6/knowledge/nel/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/nel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/nel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/nel/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:09:00.489784 personal_knowledge_library-1.0.6/knowledge/ontomapping/
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/ontomapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/ontomapping/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:09:00.489784 personal_knowledge_library-1.0.6/knowledge/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/public/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/public/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/public/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44912 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/public/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:09:00.489784 personal_knowledge_library-1.0.6/knowledge/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/services/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20881 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/services/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/services/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/services/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/services/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:09:00.493784 personal_knowledge_library-1.0.6/knowledge/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/utils/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/knowledge/utils/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:09:00.493784 personal_knowledge_library-1.0.6/personal_knowledge_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-07-04 15:09:00.000000 personal_knowledge_library-1.0.6/personal_knowledge_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 15:09:00.000000 personal_knowledge_library-1.0.6/personal_knowledge_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:09:00.000000 personal_knowledge_library-1.0.6/personal_knowledge_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-04 15:09:00.000000 personal_knowledge_library-1.0.6/personal_knowledge_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 15:09:00.000000 personal_knowledge_library-1.0.6/personal_knowledge_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 15:09:00.493784 personal_knowledge_library-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-04 15:08:45.000000 personal_knowledge_library-1.0.6/setup.py
```

### Comparing `personal_knowledge_library-1.0.5/LICENSE` & `personal_knowledge_library-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/PKG-INFO` & `personal_knowledge_library-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal_knowledge_library
-Version: 1.0.5
+Version: 1.0.6
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
```

### Comparing `personal_knowledge_library-1.0.5/README.md` & `personal_knowledge_library-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/__init__.py` & `personal_knowledge_library-1.0.6/knowledge/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __author__ = "Markus Weber"
 __copyright__ = "Copyright 2021-2023 Wacom. All rights reserved."
 __credits__ = ["Markus Weber"]
 __license__ = "Wacom"
 __maintainer__ = ["Markus Weber"]
 __email__ = "markus.weber@wacom.com"
 __status__ = "beta"
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 # Create the Logger
 logger: Union[logging.Logger, None] = None
 
 if logger is None:
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.DEBUG)
```

### Comparing `personal_knowledge_library-1.0.5/knowledge/base/__init__.py` & `personal_knowledge_library-1.0.6/knowledge/base/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/base/access.py` & `personal_knowledge_library-1.0.6/knowledge/base/access.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/base/entity.py` & `personal_knowledge_library-1.0.6/knowledge/base/entity.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/base/ontology.py` & `personal_knowledge_library-1.0.6/knowledge/base/ontology.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/nel/base.py` & `personal_knowledge_library-1.0.6/knowledge/nel/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/nel/engine.py` & `personal_knowledge_library-1.0.6/knowledge/nel/engine.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/ontomapping/__init__.py` & `personal_knowledge_library-1.0.6/knowledge/ontomapping/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright © 2023 Wacom. All rights reserved.
 import enum
 import json
 import logging
 import os
 from datetime import datetime
 from pathlib import Path
+
 from typing import Dict, Any, List, Optional
 
 from rdflib import Graph, RDFS, URIRef
 
 from knowledge.base.ontology import OntologyClassReference, OntologyPropertyReference, DataPropertyType
 from knowledge.public.wikidata import WikidataClass
 
@@ -21,16 +22,17 @@
 WIKIDATA_TYPES: str = "wikidata_types"
 OBJECT_PROPERTIES: str = "object_properties"
 DATA_PROPERTIES: str = "data_properties"
 DOMAIN_PROPERTIES: str = "domain"
 CLASSES: str = "classes"
 CONTEXT_NAME: str = 'core'
 CWD: Path = Path(__file__).parent
-CONFIGURATION_FILE: Path = CWD / '../../pkl-cache/ontology_mapping.json'
-TAXONOMY_FILE: Path = CWD / '../../pkl-cache/taxonomy_cache.json'
+CONFIGURATION_FILE: Path = Path('./.pkl-cache/ontology_mapping.json')
+TAXONOMY_PATH: Path = Path('.pkl-cache')
+
 ontology_graph: Graph = Graph()
 
 
 def subclasses_of(iri: str) -> List[str]:
     """
     Returns the subclasses of an ontology class.
     Parameters
@@ -460,20 +462,25 @@
                 property_config.domains.extend(subclasses_of(do))
         if 'inverse' in p_conf:
             property_config.inverse = p_conf['inverse']
         conf.add_property(property_config)
     return conf
 
 
-def update_taxonomy_cache():
+def update_taxonomy_cache(path: Path = TAXONOMY_PATH):
     """
     Updates the taxonomy cache.
+
+    Parameters
+    ----------
+    path: Path
+        The path to the cache file.
     """
-    with open(TAXONOMY_FILE, 'w', encoding='uft-8') as fp_taxonomy:
-        fp_taxonomy.write(json.dumps(taxonomy_cache, indent=2, cls=WikidataClassEncoder))
+    with open(path, 'w', encoding='uft-8') as fp_taxonomy_write:
+        fp_taxonomy_write.write(json.dumps(taxonomy_cache, indent=2, cls=WikidataClassEncoder))
 
 
 def register_ontology(rdf_str: str):
     """
     Registers the ontology.
     Parameters
     ----------
@@ -495,19 +502,19 @@
     Raises
     ------
     ValueError
         If the configuration file is not found.
     """
     global mapping_configuration
     if configuration.exists():
-        configuration = json.loads(CONFIGURATION_FILE.open('r').read())
+        configuration = json.loads(configuration.open('r').read())
         mapping_configuration = build_configuration(configuration)
 
     else:
-        raise ValueError(f'Configuration file {CONFIGURATION_FILE} not found.')
+        raise ValueError(f'Configuration file {configuration} not found.')
 
 
 def get_mapping_configuration() -> MappingConfiguration:
     """
     Returns the mapping configuration.
 
     Returns
@@ -518,18 +525,19 @@
     global mapping_configuration
     if mapping_configuration is None:
         raise ValueError('Please load configuration')
     return mapping_configuration
 
 
 if taxonomy_cache is None:
-    if TAXONOMY_FILE.exists():
-        try:
-            taxonomy = json.loads(TAXONOMY_FILE.open('r').read())
-        except json.decoder.JSONDecodeError:
-            taxonomy = {}
-        taxonomy_cache = {}
+    taxonomy_cache = {}
+    if TAXONOMY_PATH.exists():
+        with TAXONOMY_PATH.open('r', encoding='utf-8') as fp_taxonomy:
+            try:
+                taxonomy = json.loads(fp_taxonomy.read())
+            except json.JSONDecodeError:
+                taxonomy = {}
         for qid, data in taxonomy.items():
             if data:
                 taxonomy_cache[qid] = WikidataClass.create_from_dict(data)
     else:
         taxonomy_cache = {}
```

### Comparing `personal_knowledge_library-1.0.5/knowledge/ontomapping/manager.py` & `personal_knowledge_library-1.0.6/knowledge/ontomapping/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2023 Wacom. All rights reserved.
 import logging
 from datetime import datetime
-from typing import Optional, Any, List, Dict, Tuple
+from typing import Optional, Any, List, Dict, Tuple, Set
 
 from knowledge.base.entity import Label, LanguageCode, Description
 from knowledge.base.ontology import ThingObject, DataProperty, SYSTEM_SOURCE_SYSTEM, SYSTEM_SOURCE_REFERENCE_ID, \
     OntologyClassReference, OntologyPropertyReference, ObjectProperty, LANGUAGE_LOCALE_MAPPING, LOCALE_LANGUAGE_MAPPING
 from knowledge.ontomapping import ClassConfiguration, TOPIC_CLASS, taxonomy_cache, \
     PropertyConfiguration, PropertyType, get_mapping_configuration
 from knowledge.public.cache import pull_wikidata_object
@@ -143,18 +143,31 @@
         Thing object
     import_warnings: List[Dict[str, Any]]
         Errors
 
     """
     import_warnings: List[Dict[str, Any]] = []
     qid: str = wikidata_thing.qid
-    labels: List[Label] = [la for la in wikidata_thing.label.values() if str(la.language_code) in supported_locales]
+    labels: List[Label] = []
+    aliases: List[Label] = []
+    # Make sure that the main label are added to labels and aliases to aliases.
+    main_languages: Set[str] = set()
+    for la in wikidata_thing.label.values():
+        if str(la.language_code) in supported_locales:
+            if str(la.language_code) not in main_languages:
+                main_languages.add(str(la.language_code))
+                labels.append(Label(content=la.content, language_code=la.language_code, main=True))
+
     for lang, aliases in wikidata_thing.aliases.items():
         if str(lang) in supported_locales:
-            labels.extend([a for a in aliases])
+            if str(lang) not in main_languages:
+                main_languages.add(str(lang))
+                labels.append(Label(content=aliases[0].content, language_code=LanguageCode(lang), main=True))
+            else:
+                aliases.append(Label(content=aliases[0].content, language_code=LanguageCode(lang), main=False))
     descriptions: List[Description] = []
     if 'wiki' in wikidata_thing.sitelinks and pull_wikipedia:
         for lang, title in wikidata_thing.sitelinks['wiki'].titles.items():
             locale: str = LANGUAGE_LOCALE_MAPPING.get(lang, "NOT_SUPPORTED")
             if locale in supported_locales:
                 try:
                     descriptions.append(Description(description=get_wikipedia_summary(title, lang),
@@ -163,14 +176,15 @@
                     logging.error(f'Failed to get Wikipedia summary for {title} ({lang}): {e}')
     if len(descriptions) == 0:
         descriptions = [de for de in wikidata_thing.description.values()]
     # Create the thing
     thing: ThingObject = ThingObject(label=labels,
                                      description=descriptions,
                                      icon=wikidata_thing.image(dpi=500))
+    thing.alias = aliases
     thing.add_source_system(DataProperty(content='wikidata', property_ref=SYSTEM_SOURCE_SYSTEM,
                                          language_code=LanguageCode('en_US')))
     thing.add_source_reference_id(DataProperty(content=qid, property_ref=SYSTEM_SOURCE_REFERENCE_ID,
                                                language_code=LanguageCode('en_US')))
     thing.add_data_property(DataProperty(content=datetime.utcnow().isoformat(),
                                          property_ref=OntologyPropertyReference.parse('wacom:core#lastUpdate')))
     class_types: List[str] = wikidata_thing.ontology_types
```

### Comparing `personal_knowledge_library-1.0.5/knowledge/public/__init__.py` & `personal_knowledge_library-1.0.6/knowledge/public/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/public/cache.py` & `personal_knowledge_library-1.0.6/knowledge/public/cache.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/public/helper.py` & `personal_knowledge_library-1.0.6/knowledge/public/helper.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/public/relations.py` & `personal_knowledge_library-1.0.6/knowledge/public/relations.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/public/wikidata.py` & `personal_knowledge_library-1.0.6/knowledge/public/wikidata.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/services/__init__.py` & `personal_knowledge_library-1.0.6/knowledge/services/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/services/base.py` & `personal_knowledge_library-1.0.6/knowledge/services/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/services/graph.py` & `personal_knowledge_library-1.0.6/knowledge/services/graph.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/services/group.py` & `personal_knowledge_library-1.0.6/knowledge/services/group.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/services/ontology.py` & `personal_knowledge_library-1.0.6/knowledge/services/ontology.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/services/tenant.py` & `personal_knowledge_library-1.0.6/knowledge/services/tenant.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/services/users.py` & `personal_knowledge_library-1.0.6/knowledge/services/users.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/utils/rdf.py` & `personal_knowledge_library-1.0.6/knowledge/utils/rdf.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/knowledge/utils/wikipedia.py` & `personal_knowledge_library-1.0.6/knowledge/utils/wikipedia.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/PKG-INFO` & `personal_knowledge_library-1.0.6/personal_knowledge_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal-knowledge-library
-Version: 1.0.5
+Version: 1.0.6
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
```

### Comparing `personal_knowledge_library-1.0.5/personal_knowledge_library.egg-info/SOURCES.txt` & `personal_knowledge_library-1.0.6/personal_knowledge_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.5/setup.py` & `personal_knowledge_library-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 an older version of knowledge-service-lib :
     $ python -m pip install personal-knowledge-library
 """)
     sys.exit(1)
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # the setup
 setup(
     name='personal_knowledge_library',
```

