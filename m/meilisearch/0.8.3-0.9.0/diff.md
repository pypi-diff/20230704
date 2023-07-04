# Comparing `tmp/meilisearch-0.8.3.tar.gz` & `tmp/meilisearch-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meilisearch-0.8.3.tar", last modified: Thu Mar  5 10:25:22 2020, max compression
+gzip compressed data, was "dist/meilisearch-0.9.0.tar", last modified: Fri Mar 20 18:56:27 2020, max compression
```

## Comparing `meilisearch-0.8.3.tar` & `meilisearch-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-05 10:25:22.000000 meilisearch-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (115)     7557 2020-03-05 10:25:22.000000 meilisearch-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     5039 2020-03-05 10:25:02.000000 meilisearch-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-05 10:25:22.000000 meilisearch-0.8.3/meilisearch/
--rw-r--r--   0 runner    (1001) docker     (115)      116 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3066 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (115)     3095 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/client.py
--rw-r--r--   0 runner    (1001) docker     (115)      410 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/config.py
--rw-r--r--   0 runner    (1001) docker     (115)     5161 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/document.py
--rw-r--r--   0 runner    (1001) docker     (115)     1240 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/health.py
--rw-r--r--   0 runner    (1001) docker     (115)     5778 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/index.py
--rw-r--r--   0 runner    (1001) docker     (115)     2996 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/key.py
--rw-r--r--   0 runner    (1001) docker     (115)     1901 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/schema.py
--rw-r--r--   0 runner    (1001) docker     (115)     1718 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/search.py
--rw-r--r--   0 runner    (1001) docker     (115)     2863 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/setting.py
--rw-r--r--   0 runner    (1001) docker     (115)     1820 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/stat.py
--rw-r--r--   0 runner    (1001) docker     (115)     2907 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/stop_word.py
--rw-r--r--   0 runner    (1001) docker     (115)      843 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/synonym.py
--rw-r--r--   0 runner    (1001) docker     (115)      883 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (115)     1866 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/update.py
--rw-r--r--   0 runner    (1001) docker     (115)     1003 2020-03-05 10:25:02.000000 meilisearch-0.8.3/meilisearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-05 10:25:22.000000 meilisearch-0.8.3/meilisearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     7557 2020-03-05 10:25:21.000000 meilisearch-0.8.3/meilisearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      579 2020-03-05 10:25:21.000000 meilisearch-0.8.3/meilisearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-05 10:25:21.000000 meilisearch-0.8.3/meilisearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)        9 2020-03-05 10:25:21.000000 meilisearch-0.8.3/meilisearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       12 2020-03-05 10:25:21.000000 meilisearch-0.8.3/meilisearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)       38 2020-03-05 10:25:22.000000 meilisearch-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     1127 2020-03-05 10:25:02.000000 meilisearch-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-20 18:56:27.000000 meilisearch-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (115)     9230 2020-03-20 18:56:27.000000 meilisearch-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     6312 2020-03-20 18:56:04.000000 meilisearch-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-20 18:56:27.000000 meilisearch-0.9.0/meilisearch/
+-rw-r--r--   0 runner    (1001) docker     (115)       38 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2391 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2961 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (115)      409 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/config.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6137 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/document.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1236 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/health.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4757 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/index.py
+-rw-r--r--   0 runner    (1001) docker     (115)      940 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/key.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2015 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/search.py
+-rw-r--r--   0 runner    (1001) docker     (115)    13002 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/setting.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1859 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/stat.py
+-rw-r--r--   0 runner    (1001) docker     (115)      873 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1938 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/update.py
+-rw-r--r--   0 runner    (1001) docker     (115)      995 2020-03-20 18:56:04.000000 meilisearch-0.9.0/meilisearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-20 18:56:27.000000 meilisearch-0.9.0/meilisearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)     9230 2020-03-20 18:56:27.000000 meilisearch-0.9.0/meilisearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)      509 2020-03-20 18:56:27.000000 meilisearch-0.9.0/meilisearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-20 18:56:27.000000 meilisearch-0.9.0/meilisearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        9 2020-03-20 18:56:27.000000 meilisearch-0.9.0/meilisearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       12 2020-03-20 18:56:27.000000 meilisearch-0.9.0/meilisearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       38 2020-03-20 18:56:27.000000 meilisearch-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     1127 2020-03-20 18:56:04.000000 meilisearch-0.9.0/setup.py
```

### Comparing `meilisearch-0.8.3/PKG-INFO` & `meilisearch-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,87 @@
 Metadata-Version: 2.1
 Name: meilisearch
-Version: 0.8.3
+Version: 0.9.0
 Summary: The python client for MeiliSearch API.
 Home-page: https://github.com/meilisearch/meilisearch-python
 Author: Charlotte Vermandel
 Author-email: charlotte@meilisearch.com
 License: UNKNOWN
 Project-URL: Documentation, https://docs.meilisearch.com/
-Description: # MeiliSearch Python Client
+Description: # MeiliSearch Python Client <!-- omit in toc -->
         
         [![PyPI version](https://badge.fury.io/py/meilisearch.svg)](https://badge.fury.io/py/meilisearch)
         [![Licence](https://img.shields.io/badge/licence-MIT-blue.svg)](https://img.shields.io/badge/licence-MIT-blue.svg)
         [![test Status](https://github.com/meilisearch/meilisearch-python/workflows/Pytest/badge.svg)](https://github.com/{owner}/{repo}/actions)
         
-        
         The python client for MeiliSearch API.
         
-        MeiliSearch provides an ultra relevant and instant full-text search. Our solution is open-source and you can check out [our repository here](https://github.com/meilisearch/MeiliDB).
+        MeiliSearch provides an ultra relevant and instant full-text search. Our solution is open-source and you can check out [our repository here](https://github.com/meilisearch/MeiliSearch).
         
         Here is the [MeiliSearch documentation](https://docs.meilisearch.com/) 📖
         
         ## Table of Contents <!-- omit in toc -->
         
         - [🔧 Installation](#-installation)
         - [🚀 Getting started](#-getting-started)
         - [🎬 Examples](#-examples)
           - [Indexes](#indexes)
           - [Documents](#documents)
           - [Update status](#update-status)
           - [Search](#search)
+        - [⚙️ Development Workflow](#️-development-workflow)
+          - [Install dependencies](#install-dependencies)
+          - [Tests and Linter](#tests-and-linter)
+          - [Release](#release)
         - [🤖 Compatibility with MeiliSearch](#-compatibility-with-meilisearch)
         
         ## 🔧 Installation
         
         With `pip3` in command line:
         
         ```bash
         pip3 install meilisearch
         ```
         
-        ### 🏃‍♀️ Run MeiliSearch
+        ### Run MeiliSearch <!-- omit in toc -->
         
-        There are many easy ways to [download and run a MeiliSearch instance](https://docs.meilisearch.com/guides/advanced_guides/binary.html#download-and-launch).
+        There are many easy ways to [download and run a MeiliSearch instance](https://docs.meilisearch.com/guides/advanced_guides/installation.html#download-and-launch).
         
         For example, if you use Docker:
         ```bash
-        $ docker run -it --rm -p 7700:7700 getmeili/meilisearch:latest --api-key=apiKey
+        $ docker run -it --rm -p 7700:7700 getmeili/meilisearch:latest --master-key=masterKey
         ```
         
         NB: you can also download MeiliSearch from **Homebrew** or **APT**.
         
         ## 🚀 Getting started
         
         #### Add documents <!-- omit in toc -->
         
         ```python
         import meilisearch
+        
         client = meilisearch.Client("http://127.0.0.1:7700", "apiKey")
-        index = client.create_index(name='books', uid='books_uid') # If your index does not exist
-        index = client.get_index('books_uid') # If you already created your index
+        index = client.create_index(uid='books_uid') # If your index does not exist
+        index = client.get_index('books_uid')        # If you already created your index
         
         documents = [
           { "id": 123,  "title": 'Pride and Prejudice' },
           { "id": 456,  "title": 'Le Petit Prince' },
           { "id": 1,    "title": 'Alice In Wonderland' },
           { "id": 1344, "title": 'The Hobbit' },
           { "id": 4,    "title": 'Harry Potter and the Half-Blood Prince' },
           { "id": 42,   "title": 'The Hitchhiker\'s Guide to the Galaxy' }
         ]
         
-        index.add_documents(documents) # asynchronous
+        index.add_documents(documents) # => { "updateId": 0 }
         ```
         
+        With the `updateId`, you can check the status (`processed` or `failed`) of your documents addition thanks to this [method](#update-status).
+        
         #### Search in index <!-- omit in toc -->
         ``` python
         # MeiliSearch is typo-tolerant:
         index.search({
           "q": 'hary pottre'
         })
         ```
@@ -99,74 +105,74 @@
         You can check out [the API documentation](https://docs.meilisearch.com/references/).
         
         ### Indexes
         
         #### Create an index <!-- omit in toc -->
         ```python
         # Create an index
-        client.create_index(name='Books')
-        # Create an index with a specific uid (uid must be unique)
-        client.create_index(name= 'Books', uid= 'books')
-        # Create an index with a schema
-        schema = {
-          "id":    ["displayed", "indexed", "identifier"],
-          "title": ["displayed", "indexed"]
-        }
-        client.create_index(name= 'Books', schema= schema)
+        client.create_index(uid='books')
+        # Create an index and give the primary-key
+        client.create_index(uid='books', primary_key='objectID')
         ```
         
         #### List all indexes <!-- omit in toc -->
         ```python
         client.get_indexes()
         ```
         
         #### Get an index object <!-- omit in toc -->
+        
         ```python
-        index = client.get_index(uid="books")
+        index = client.get_index('books')
         ```
         
         ### Documents
         
         #### Fetch documents <!-- omit in toc -->
+        
         ```python
         # Get one document
         index.get_document(123)
         # Get documents by batch
-        index.get_documents({ "offset": 10 , "limit": 20 })
+        index.get_documents({ 'offset': 10 , 'limit': 20 })
         ```
+        
         #### Add documents <!-- omit in toc -->
+        
         ```python
-        index.add_documents([{ "id": 2, "title": 'Madame Bovary' }])
+        index.add_documents([{ 'id': 2, 'title': 'Madame Bovary' }])
         ```
         
         Response:
         ```json
         {
             "updateId": 1
         }
         ```
         This `updateId` allows you to [track the current update](#update-status).
         
         #### Delete documents <!-- omit in toc -->
+        
         ```python
         # Delete one document
         index.delete_document(2)
         # Delete several documents
         index.delete_documents([1, 42])
-        # Delete all documents 
+        # Delete all documents
         index.delete_all_documents()
         ```
         
         ### Update status
+        
         ```python
-        # Get one update
+        # Get one update status
         # Parameter: the updateId got after an asynchronous request (e.g. documents addition)
-        index.get_update(1)
-        # Get all updates
-        index.get_updates()
+        index.get_update_status(1)
+        # Get all updates status
+        index.get_all_update_status()
         ```
         
         ### Search
         
         #### Basic search <!-- omit in toc -->
         
         ```python
@@ -216,18 +222,62 @@
             "offset": 0,
             "limit": 1,
             "processingTimeMs": 10,
             "query": "prince"
         }
         ```
         
+        ## ⚙️ Development Workflow
+        
+        If you want to contribute, this section describes the steps to follow.
+        
+        Thank you for your interest in a MeiliSearch tool! ♥️
+        
+        ### Install dependencies
+        
+        ```bash
+        $ pipenv install --dev
+        ```
+        
+        ### Tests and Linter
+        
+        Each PR should pass the tests and the linter to be accepted.
+        
+        ```bash
+        # Tests
+        $ docker run -d -p 7700:7700 getmeili/meilisearch:latest ./meilisearch --master-key=masterKey --no-analytics
+        $ pipenv run pytest meilisearch
+        # Linter
+        $ pipenv run pylint meilisearch
+        ```
+        
+        ### Release
+        
+        MeiliSearch tools follow the [Semantic Versioning Convention](https://semver.org/).
+        
+        You must do a PR modifying the file `setup.py` with the right version.<br>
+        
+        ```python
+        version="X.X.X"
+        ```
+        
+        Once the changes are merged on `master`, in your terminal, you must be on the `master` branch and push a new tag with the right version:
+        
+        ```bash
+        $ git checkout master
+        $ git pull origin master
+        $ git tag vX.X.X
+        $ git push --tag origin master
+        ```
+        
+        A GitHub Action will be triggered and push the new gem on [RubyGems](https://rubygems.org/gems/meilisearch).
         
         ## 🤖 Compatibility with MeiliSearch
         
-        This package works for MeiliSearch `v0.8.x`.
+        This package works for MeiliSearch `v0.9.x`.
         
 Keywords: search python meilisearch
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `meilisearch-0.8.3/README.md` & `meilisearch-0.9.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,78 @@
-# MeiliSearch Python Client
+# MeiliSearch Python Client <!-- omit in toc -->
 
 [![PyPI version](https://badge.fury.io/py/meilisearch.svg)](https://badge.fury.io/py/meilisearch)
 [![Licence](https://img.shields.io/badge/licence-MIT-blue.svg)](https://img.shields.io/badge/licence-MIT-blue.svg)
 [![test Status](https://github.com/meilisearch/meilisearch-python/workflows/Pytest/badge.svg)](https://github.com/{owner}/{repo}/actions)
 
-
 The python client for MeiliSearch API.
 
-MeiliSearch provides an ultra relevant and instant full-text search. Our solution is open-source and you can check out [our repository here](https://github.com/meilisearch/MeiliDB).
+MeiliSearch provides an ultra relevant and instant full-text search. Our solution is open-source and you can check out [our repository here](https://github.com/meilisearch/MeiliSearch).
 
 Here is the [MeiliSearch documentation](https://docs.meilisearch.com/) 📖
 
 ## Table of Contents <!-- omit in toc -->
 
 - [🔧 Installation](#-installation)
 - [🚀 Getting started](#-getting-started)
 - [🎬 Examples](#-examples)
   - [Indexes](#indexes)
   - [Documents](#documents)
   - [Update status](#update-status)
   - [Search](#search)
+- [⚙️ Development Workflow](#️-development-workflow)
+  - [Install dependencies](#install-dependencies)
+  - [Tests and Linter](#tests-and-linter)
+  - [Release](#release)
 - [🤖 Compatibility with MeiliSearch](#-compatibility-with-meilisearch)
 
 ## 🔧 Installation
 
 With `pip3` in command line:
 
 ```bash
 pip3 install meilisearch
 ```
 
-### 🏃‍♀️ Run MeiliSearch
+### Run MeiliSearch <!-- omit in toc -->
 
-There are many easy ways to [download and run a MeiliSearch instance](https://docs.meilisearch.com/guides/advanced_guides/binary.html#download-and-launch).
+There are many easy ways to [download and run a MeiliSearch instance](https://docs.meilisearch.com/guides/advanced_guides/installation.html#download-and-launch).
 
 For example, if you use Docker:
 ```bash
-$ docker run -it --rm -p 7700:7700 getmeili/meilisearch:latest --api-key=apiKey
+$ docker run -it --rm -p 7700:7700 getmeili/meilisearch:latest --master-key=masterKey
 ```
 
 NB: you can also download MeiliSearch from **Homebrew** or **APT**.
 
 ## 🚀 Getting started
 
 #### Add documents <!-- omit in toc -->
 
 ```python
 import meilisearch
+
 client = meilisearch.Client("http://127.0.0.1:7700", "apiKey")
-index = client.create_index(name='books', uid='books_uid') # If your index does not exist
-index = client.get_index('books_uid') # If you already created your index
+index = client.create_index(uid='books_uid') # If your index does not exist
+index = client.get_index('books_uid')        # If you already created your index
 
 documents = [
   { "id": 123,  "title": 'Pride and Prejudice' },
   { "id": 456,  "title": 'Le Petit Prince' },
   { "id": 1,    "title": 'Alice In Wonderland' },
   { "id": 1344, "title": 'The Hobbit' },
   { "id": 4,    "title": 'Harry Potter and the Half-Blood Prince' },
   { "id": 42,   "title": 'The Hitchhiker\'s Guide to the Galaxy' }
 ]
 
-index.add_documents(documents) # asynchronous
+index.add_documents(documents) # => { "updateId": 0 }
 ```
 
+With the `updateId`, you can check the status (`processed` or `failed`) of your documents addition thanks to this [method](#update-status).
+
 #### Search in index <!-- omit in toc -->
 ``` python
 # MeiliSearch is typo-tolerant:
 index.search({
   "q": 'hary pottre'
 })
 ```
@@ -90,74 +96,74 @@
 You can check out [the API documentation](https://docs.meilisearch.com/references/).
 
 ### Indexes
 
 #### Create an index <!-- omit in toc -->
 ```python
 # Create an index
-client.create_index(name='Books')
-# Create an index with a specific uid (uid must be unique)
-client.create_index(name= 'Books', uid= 'books')
-# Create an index with a schema
-schema = {
-  "id":    ["displayed", "indexed", "identifier"],
-  "title": ["displayed", "indexed"]
-}
-client.create_index(name= 'Books', schema= schema)
+client.create_index(uid='books')
+# Create an index and give the primary-key
+client.create_index(uid='books', primary_key='objectID')
 ```
 
 #### List all indexes <!-- omit in toc -->
 ```python
 client.get_indexes()
 ```
 
 #### Get an index object <!-- omit in toc -->
+
 ```python
-index = client.get_index(uid="books")
+index = client.get_index('books')
 ```
 
 ### Documents
 
 #### Fetch documents <!-- omit in toc -->
+
 ```python
 # Get one document
 index.get_document(123)
 # Get documents by batch
-index.get_documents({ "offset": 10 , "limit": 20 })
+index.get_documents({ 'offset': 10 , 'limit': 20 })
 ```
+
 #### Add documents <!-- omit in toc -->
+
 ```python
-index.add_documents([{ "id": 2, "title": 'Madame Bovary' }])
+index.add_documents([{ 'id': 2, 'title': 'Madame Bovary' }])
 ```
 
 Response:
 ```json
 {
     "updateId": 1
 }
 ```
 This `updateId` allows you to [track the current update](#update-status).
 
 #### Delete documents <!-- omit in toc -->
+
 ```python
 # Delete one document
 index.delete_document(2)
 # Delete several documents
 index.delete_documents([1, 42])
-# Delete all documents 
+# Delete all documents
 index.delete_all_documents()
 ```
 
 ### Update status
+
 ```python
-# Get one update
+# Get one update status
 # Parameter: the updateId got after an asynchronous request (e.g. documents addition)
-index.get_update(1)
-# Get all updates
-index.get_updates()
+index.get_update_status(1)
+# Get all updates status
+index.get_all_update_status()
 ```
 
 ### Search
 
 #### Basic search <!-- omit in toc -->
 
 ```python
@@ -207,11 +213,55 @@
     "offset": 0,
     "limit": 1,
     "processingTimeMs": 10,
     "query": "prince"
 }
 ```
 
+## ⚙️ Development Workflow
+
+If you want to contribute, this section describes the steps to follow.
+
+Thank you for your interest in a MeiliSearch tool! ♥️
+
+### Install dependencies
+
+```bash
+$ pipenv install --dev
+```
+
+### Tests and Linter
+
+Each PR should pass the tests and the linter to be accepted.
+
+```bash
+# Tests
+$ docker run -d -p 7700:7700 getmeili/meilisearch:latest ./meilisearch --master-key=masterKey --no-analytics
+$ pipenv run pytest meilisearch
+# Linter
+$ pipenv run pylint meilisearch
+```
+
+### Release
+
+MeiliSearch tools follow the [Semantic Versioning Convention](https://semver.org/).
+
+You must do a PR modifying the file `setup.py` with the right version.<br>
+
+```python
+version="X.X.X"
+```
+
+Once the changes are merged on `master`, in your terminal, you must be on the `master` branch and push a new tag with the right version:
+
+```bash
+$ git checkout master
+$ git pull origin master
+$ git tag vX.X.X
+$ git push --tag origin master
+```
+
+A GitHub Action will be triggered and push the new gem on [RubyGems](https://rubygems.org/gems/meilisearch).
 
 ## 🤖 Compatibility with MeiliSearch
 
-This package works for MeiliSearch `v0.8.x`.
+This package works for MeiliSearch `v0.9.x`.
```

### Comparing `meilisearch-0.8.3/meilisearch/_httprequests.py` & `meilisearch-0.9.0/meilisearch/_httprequests.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,86 @@
 import requests
 
-
 class HttpRequests:
+
     @staticmethod
     def get(config, path):
-        try:
-            r = requests.get(
-                config.url + '/' + path,
-                headers={
-                    'x-meili-api-key': config.apikey,
-                    'content-type': 'application/json'
-                }
-            )
-            r.raise_for_status()
-            return r
-        except requests.exceptions.HTTPError as err:
-            raise Exception(err)
-        except requests.exceptions.ConnectionError as err:
-            raise Exception(err)
+        request = requests.get(
+            config.url + '/' + path,
+            headers={
+                'X-Meili-Api-Key': config.apikey,
+                'Content-Type': 'application/json'
+            }
+        )
+        return HttpRequests.__validate(request)
 
     @staticmethod
     def post(config, path, body=None):
-        try:
-            if body is None:
-                body = {}
-            r = requests.post(
-                config.url + '/' + path,
-                headers={
-                    'x-meili-api-key': config.apikey,
-                    'content-type': 'application/json'
-                },
-                json=body
-            )
-            r.raise_for_status()
-            return r
-        except requests.exceptions.HTTPError as err:
-            raise Exception(err)
-        except requests.exceptions.ConnectionError as err:
-            raise Exception(err)
+        if body is None:
+            body = {}
+        request = requests.post(
+            config.url + '/' + path,
+            headers={
+                'x-meili-api-key': config.apikey,
+                'content-type': 'application/json'
+            },
+            json=body
+        )
+        return HttpRequests.__validate(request)
 
     @staticmethod
     def put(config, path, body=None):
-        try:
-            if body is None:
-                body = {}
-            r = requests.put(
-                config.url + '/' + path,
-                headers={
-                    'x-meili-api-key': config.apikey,
-                    'content-type': 'application/json'
-                },
-                json=body
-            )
-            r.raise_for_status()
-            return r
-        except requests.exceptions.HTTPError as err:
-            raise Exception(err)
-        except requests.exceptions.ConnectionError as err:
-            raise Exception(err)
+        if body is None:
+            body = {}
+        request = requests.put(
+            config.url + '/' + path,
+            headers={
+                'x-meili-api-key': config.apikey,
+                'content-type': 'application/json'
+            },
+            json=body
+        )
+        return HttpRequests.__validate(request)
 
     @staticmethod
     def patch(config, path, body=None):
-        try:
-            if body is None:
-                body = {}
-            r = requests.patch(
-                config.url + '/' + path,
-                headers={
-                    'x-meili-api-key': config.apikey,
-                    'content-type': 'application/json'
-                },
-                json=body
-            )
-            r.raise_for_status()
-            return r
-        except requests.exceptions.HTTPError as err:
-            raise Exception(err)
-        except requests.exceptions.ConnectionError as err:
-            raise Exception(err)
+        if body is None:
+            body = {}
+        request = requests.patch(
+            config.url + '/' + path,
+            headers={
+                'x-meili-api-key': config.apikey,
+                'content-type': 'application/json'
+            },
+            json=body
+        )
+        return HttpRequests.__validate(request)
 
     @staticmethod
     def delete(config, path, body=None):
+        if body is None:
+            body = {}
+        request = requests.delete(
+            config.url + '/' + path,
+            headers={
+                'x-meili-api-key': config.apikey,
+                'content-type': 'application/json'
+            },
+            json=body
+        )
+        return HttpRequests.__validate(request)
+
+    @staticmethod
+    def __to_json(request):
+        if request.content == b'':
+            return request
+        return request.json()
+
+    @staticmethod
+    def __validate(request):
         try:
-            if body is None:
-                body = {}
-            r = requests.delete(
-                config.url + '/' + path,
-                headers={
-                    'x-meili-api-key': config.apikey,
-                    'content-type': 'application/json'
-                },
-                json=body
-            )
-            r.raise_for_status()
-            return r
+            request.raise_for_status()
+            return HttpRequests.__to_json(request)
         except requests.exceptions.HTTPError as err:
             raise Exception(err)
         except requests.exceptions.ConnectionError as err:
             raise Exception(err)
```

### Comparing `meilisearch-0.8.3/meilisearch/client.py` & `meilisearch-0.9.0/meilisearch/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,94 +2,92 @@
 from meilisearch.health import Health
 from meilisearch.key import Key
 from meilisearch.config import Config
 from meilisearch.sys_info import SysInfo
 from meilisearch.stat import Stat
 from meilisearch.version import Version
 
-
 class Client(Health, Key, SysInfo, Version):
     """
-    A client for the meilisearch API
+    A client for the MeiliSearch API
 
-    A client instance is needed for every meilisearch API method to know the location of
-    meilisearch and his permissions.
+    A client instance is needed for every MeiliSearch API method to know the location of
+    MeiliSearch and its permissions.
     """
 
-    def __init__(self, url, apikey=None):
+    def __init__(self, url, apiKey=None):
         """
         Parameters
         ----------
         url : str
-            The url to the meilisearch API (ex: http://localhost:8080)
-        apikey : str
-            The optionnal apikey to access the meilisearch api
+            The url to the MeiliSearch API (ex: http://localhost:7700)
+        apiKey : str
+            The optional API key for MeiliSearch
         """
-        config = Config(url, apikey)
+        config = Config(url, apiKey)
         Health.__init__(self, config)
         Key.__init__(self, config)
         SysInfo.__init__(self, config)
         Version.__init__(self, config)
         self.config = config
 
-    def create_index(self, name, uid=None, schema=None):
+    def create_index(self, uid, primary_key=None, name=None):
         """Create an index.
 
         If the argument `uid` isn't passed in, it will be generated
-        by meilisearch.
+        by MeiliSearch.
 
         Parameters
         ----------
-        name: str
+        uid: str
+            UID of the index
+        primary_key: str, optional
+            Attribute used as unique document identifier
+        name: str, optional
             Name of the index
-        uid: str, optional
-            uid of the index
-        schema: dict, optional
-            dict containing the schema of the index.
-            https://docs.meilisearch.com/main_concepts/indexes.html#schema-definition
         Returns
         -------
         index : Index
             an instance of Index containing the information of the newly created index
         Raises
         ------
         HTTPError
             In case of any other error found here https://docs.meilisearch.com/references/#errors-status-code
         """
-        index = Index.create(self.config, name=name, uid=uid, schema=schema)
-        return Index(self.config, name=index["name"], uid=index["uid"], schema=schema)
+        index = Index.create(self.config, uid=uid, primary_key=primary_key, name=name)
+        return Index(self.config, uid=index['uid'])
 
     def get_indexes(self):
         """Get all indexes.
 
         Raises
         ------
         HTTPError
             In case of any error found here https://docs.meilisearch.com/references/#errors-status-code
         Returns
         -------
         list
-            List of indexes in dictionnary format. (e.g [{ 'name': 'movies' 'uid': '12345678' }])
+            List of indexes in dictionnary format. (e.g [{ 'uid': 'movies' 'primaryKey': 'objectID' }])
         """
         return Index.get_indexes(self.config)
 
 
-    def get_index(self, uid=None, name=None):
+    def get_index(self, uid):
         """Get an index.
 
         Raises
         ------
         HTTPError
             In case of any error found here https://docs.meilisearch.com/references/#errors-status-code
         Returns
         -------
         index : Index
             an instance of Index containing the information of the index found
         """
-        return Index.get_index(self.config, uid=uid, name=name)
+        return Index.get_index(self.config, uid=uid)
 
     def get_all_stats(self):
         """Get statistics about indexes, database size and update date.
 
         Returns
         -------
         stats : dict
```

### Comparing `meilisearch-0.8.3/meilisearch/document.py` & `meilisearch-0.9.0/meilisearch/document.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,174 +1,202 @@
 import urllib
 from meilisearch._httprequests import HttpRequests
 
 class Document:
     """
     Documents routes wrapper
 
-    Index's parent that gives access to all the documents methods of meilisearch.
+    Index's parent that gives access to all the documents methods of MeiliSearch.
     https://docs.meilisearch.com/references/documents.html
 
     Attributes
     ----------
     document_path:
         Document url path
     """
     document_path = 'documents'
 
     def __init__(self, parent_path, config, uid=None, name=None):
         """
         Parameters
         ----------
         config : Config
-            Config object containing permission and location of meilisearch
+            Config object containing permission and location of MeiliSearch
         name: str
             Name of the index on which to perform the document actions.
         uid: str
             Uid of the index on which to perform the document actions.
         index_path: str
             Index url path
         """
         self.config = config
         self.name = name
         self.uid = uid
         self.index_path = parent_path
 
-
     def get_document(self, document_id):
         """Get one document with given document identifier
 
         Parameters
         ----------
         document_id: str
             Unique identifier of the document.
         Returns
         ----------
         document: `dict`
             Dictionnary containing the documents information
         """
-        return HttpRequests.get(self.config, '{}/{}/{}/{}'.format(
-            self.index_path,
-            self.uid,
-            self.document_path,
-            document_id
-            )).json()
+        return HttpRequests.get(
+            self.config,
+            '{}/{}/{}/{}'.format(
+                self.index_path,
+                self.uid,
+                self.document_path,
+                document_id
+            )
+        )
 
-    def get_documents(self, parameters):
+    def get_documents(self, parameters=None):
         """Get a set of documents from the index
 
         Parameters
         ----------
-        parameters: dict
+        parameters (optional): dict
             parameters accepted by the get documents route: https://docs.meilisearch.com/references/documents.html#get-all-documents
         Returns
         ----------
         document: `dict`
             Dictionnary containing the documents information
         """
         return HttpRequests.get(
             self.config,
             '{}/{}/{}?{}'.format(
                 self.index_path,
-                self.uid, self.document_path,
+                self.uid,
+                self.document_path,
                 urllib.parse.urlencode(parameters))
-            ).json()
-
+            )
 
-    def add_documents(self, documents):
+    def add_documents(self, documents, primary_key=None):
         """Add documents to the index
 
         Parameters
         ----------
         documents: list
             List of dics containing each a document, or json string
+        primary_key: string
+            The primary-key used in MeiliSearch index. Ignored if already set up.
         Returns
         ----------
         update: `dict`
             Dictionnary containing an update id to track the action:
             https://docs.meilisearch.com/references/updates.html#get-an-update-status
         """
-        return HttpRequests.post(self.config, '{}/{}/{}'.format(
-            self.index_path,
-            self.uid,
-            self.document_path,
-            ),
-            documents
-            ).json()
+        if primary_key is None:
+            url = '{}/{}/{}'.format(
+                self.index_path,
+                self.uid,
+                self.document_path
+            )
+        else:
+            url = '{}/{}/{}?{}'.format(
+                self.index_path,
+                self.uid,
+                self.document_path,
+                urllib.parse.urlencode({'primaryKey': primary_key})
+            )
+        return HttpRequests.post(self.config, url, documents)
 
-    def update_documents(self, documents):
+    def update_documents(self, documents, primary_key=None):
         """Update documents in the index
 
         Parameters
         ----------
         documents: list
             List of dics containing each a document, or json string
+        primary_key: string
+            The primary-key used in MeiliSearch index. Ignored if already set up.
         Returns
         ----------
         update: `dict`
             Dictionnary containing an update id to track the action:
             https://docs.meilisearch.com/references/updates.html#get-an-update-status
         """
-        return HttpRequests.put(self.config, '{}/{}/{}'.format(
-            self.index_path,
-            self.uid,
-            self.document_path,
-            ),
-            documents
-            ).json()
+        if primary_key is None:
+            url = '{}/{}/{}'.format(
+                self.index_path,
+                self.uid,
+                self.document_path
+            )
+        else:
+            url = '{}/{}/{}?{}'.format(
+                self.index_path,
+                self.uid,
+                self.document_path,
+                urllib.parse.urlencode({'primaryKey': primary_key})
+            )
+        return HttpRequests.put(self.config, url, documents)
+
 
     def delete_document(self, document_id):
         """Add documents to the index
 
         Parameters
         ----------
         document_id: str
             Unique identifier of the document.
         Returns
         ----------
         update: `dict`
             Dictionnary containing an update id to track the action:
             https://docs.meilisearch.com/references/updates.html#get-an-update-status
         """
-        return HttpRequests.delete(self.config, '{}/{}/{}/{}'.format(
-            self.index_path,
-            self.uid,
-            self.document_path,
-            document_id
-        )).json()
+        return HttpRequests.delete(
+            self.config,
+            '{}/{}/{}/{}'.format(
+                self.index_path,
+                self.uid,
+                self.document_path,
+                document_id
+            )
+        )
 
     def delete_documents(self, ids):
         """Delete multiple documents of the index
 
         Parameters
         ----------
         list: list
             List of unique identifiers of documents.
         Returns
         ----------
         update: `dict`
             Dictionnary containing an update id to track the action:
             https://docs.meilisearch.com/references/updates.html#get-an-update-status
         """
-        return HttpRequests.post(self.config, '{}/{}/{}/delete'.format(
-            self.index_path,
-            self.uid,
-            self.document_path
-        ),
-        ids
-        ).json()
+        return HttpRequests.post(
+            self.config,
+            '{}/{}/{}/delete-batch'.format(
+                self.index_path,
+                self.uid,
+                self.document_path
+            ),
+            ids
+        )
 
     def delete_all_documents(self):
         """Delete all documents of the index
 
         Returns
         ----------
         update: `dict`
             Dictionnary containing an update id to track the action:
             https://docs.meilisearch.com/references/updates.html#get-an-update-status
         """
-        return HttpRequests.delete(self.config, '{}/{}/{}'.format(
-            self.index_path,
-            self.uid,
-            self.document_path
+        return HttpRequests.delete(
+            self.config,
+            '{}/{}/{}'.format(
+                self.index_path,
+                self.uid,
+                self.document_path
+            )
         )
-        ).json()
```

### Comparing `meilisearch-0.8.3/meilisearch/health.py` & `meilisearch-0.9.0/meilisearch/health.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from meilisearch._httprequests import HttpRequests
 
-
 class Health:
     """
     Health routes wrapper
 
     Client's parent that gives access to all the health methods of meilisearch.
     https://docs.meilisearch.com/references/health.html
 
@@ -41,10 +40,9 @@
 
         Update health of meilisearch to true or false.
 
         Parameters
         ----------
         health: bool
             Boolean reprensenting the healthyness of meilisearch. True for healthy.
-
         """
-        return HttpRequests.put(self.config, self.health_path, { 'health': health })
+        return HttpRequests.put(self.config, self.health_path, {'health': health})
```

### Comparing `meilisearch-0.8.3/meilisearch/index.py` & `meilisearch-0.9.0/meilisearch/index.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,179 +1,155 @@
 from meilisearch._httprequests import HttpRequests
-from meilisearch.schema import Schema
 from meilisearch.update import Update
 from meilisearch.document import Document
-from meilisearch.synonym import Synonym
 from meilisearch.search import Search
 from meilisearch.stat import Stat
 from meilisearch.setting import Setting
-from meilisearch.stop_word import StopWord
 
 # pylint: disable=too-many-ancestors
-class Index(Schema, Update, Document, Search, Synonym, Stat, Setting, StopWord):
+class Index(Update, Document, Search, Stat, Setting):
     """
     Indexes routes wrapper
 
     Index class gives access to all indexes routes and child routes (herited).
     https://docs.meilisearch.com/references/indexes.html
 
     Attributes
     ----------
     index_path:
         Index url path
-
     """
-
     index_path = 'indexes'
 
-    def __init__(self, config, uid=None, name=None, schema=None):
+    def __init__(self, config, uid):
         """
         Parameters
         ----------
         config : Config
             Config object containing permission and location of meilisearch
-        name: str
-            Name of the index on which to perform the index actions.
         uid: str
             Uid of the index on which to perform the index actions.
-        schema: dict
-            Schema definition of index.
         index_path: str
             Index url path
         """
-
-        Schema.__init__(self, Index.index_path, config, name, uid)
-        Update.__init__(self, Index.index_path, config, name, uid)
-        Search.__init__(self, Index.index_path, config, name, uid)
-        Document.__init__(self, Index.index_path, config, name, uid)
-        Synonym.__init__(self, Index.index_path, config, name, uid)
-        Stat.__init__(self, Index.index_path, config, name, uid)
-        Setting.__init__(self, Index.index_path, config, name, uid)
-        StopWord.__init__(self, Index.index_path, config, name, uid)
+        Update.__init__(self, Index.index_path, config, uid)
+        Search.__init__(self, Index.index_path, config, uid)
+        Document.__init__(self, Index.index_path, config, uid)
+        Stat.__init__(self, Index.index_path, config, uid)
+        Setting.__init__(self, Index.index_path, config, uid)
         self.config = config
-        self.name = name
         self.uid = uid
-        self.schema = schema
 
     def delete(self):
         """Delete an index from meilisearch
 
         Returns
         ----------
         update: `dict`
             Dictionnary containing an update id to track the action:
             https://docs.meilisearch.com/references/updates.html#get-an-update-status
         """
-
         return HttpRequests.delete(self.config, '{}/{}'.format(self.index_path, self.uid))
 
     def update(self, **body):
         """Update an index from meilisearch
 
         Parameters
         ----------
         body: **kwargs
-            Accepts name as an updatable parameter.
+            Accepts primaryKey as an updatable parameter.
 
         Returns
         ----------
         update: `dict`
             Dictionnary containing an update id to track the action:
             https://docs.meilisearch.com/references/updates.html#get-an-update-status
         """
-
         payload = {}
-        name = body.get("name", None)
-        if name is not None:
-            payload["name"] = name
-        return HttpRequests.put(self.config, '{}/{}'.format(self.index_path, self.uid), payload).json()
+        primary_key = body.get('primaryKey', None)
+        if primary_key is not None:
+            payload['primaryKey'] = primary_key
+        return HttpRequests.put(self.config, '{}/{}'.format(self.index_path, self.uid), payload)
 
     def info(self):
         """Get info of index
 
         Returns
         ----------
         index: `dict`
             Dictionnary containing index information.
         """
+        return HttpRequests.get(self.config, '{}/{}'.format(self.index_path, self.uid))
 
-        return HttpRequests.get(self.config, '{}/{}'.format(self.index_path, self.uid)).json()
+    def get_primary_key(self):
+        """Get the primary key
+
+        Returns
+        ----------
+        primary_key: str
+            String containing primary key.
+        """
+        return self.info()['primaryKey']
 
     @staticmethod
-    def create(config, name, uid=None, schema=None):
+    def create(config, **body):
         """Create an index.
 
-        If the argument `uid` isn't passed in, it will be generated
-        by meilisearch.
-        If the argument `name` isn't passed in, it will raise an error.
-
         Parameters
         ----------
-        name: str
-            Name of the index
-        uid: str, optional
-            uid of the index
-        schema: dict, optional
-            dict containing the schema of the index.
-            https://docs.meilisearch.com/main_concepts/indexes.html#schema-definition
+            body: **kwargs
+            Accepts uid, name and primaryKey as parameter.
+
         Returns
         -------
         index : Index
             an instance of Index containing the information of the newly created index
         Raises
         ------
         HTTPError
             In case of any error found here https://docs.meilisearch.com/references/#errors-status-code
         """
-
         payload = {}
-        if name is not None:
-            payload["name"] = name
+        uid = body.get('uid', None)
         if uid is not None:
-            payload["uid"] = uid
-        if schema is not None:
-            payload["schema"] = schema
-        response = HttpRequests.post(config, Index.index_path, payload)
-        return response.json()
+            payload['uid'] = uid
+        name = body.get('name', None)
+        if name is not None:
+            payload['name'] = name
+        primary_key = body.get('primary_key', None)
+        if primary_key is not None:
+            payload['primaryKey'] = primary_key
+        return HttpRequests.post(config, Index.index_path, payload)
 
     @staticmethod
     def get_indexes(config):
         """Get all indexes from meilisearch.
 
         Returns
         -------
         indexes : list
             List of indexes (dict)
         Raises
         ------
         HTTPError
             In case of any error found here https://docs.meilisearch.com/references/#errors-status-code
         """
-
-        return HttpRequests.get(config, Index.index_path).json()
+        return HttpRequests.get(config, Index.index_path)
 
     @staticmethod
-    def get_index(config, name=None, uid=None):
+    def get_index(config, uid):
         """Get Index instance from given index
 
-        If the arguments `name` and `uid` aren't passed in, it
-        will raise an exception.
+        If the argument `uid` aren't passed in, it will raise an exception.
 
         Returns
         -------
         index : Index
             Instance of Index with the given index.
         Raises
         ------
         HTTPError
             In case of any error found here https://docs.meilisearch.com/references/#errors-status-code
         """
         if uid is not None:
-            return Index(config, uid=uid, name=name)
-        if name is None:
-            raise Exception('Name or Uid is needed to find index')
-        indexes = Index.get_indexes(config)
-        index = list(filter(lambda index: index["name"] == name, indexes))
-        if len(index) == 0:
-            raise Exception('Index not found')
-        index = index[0]
-        return Index(config, name=index["name"], uid=index["uid"])
+            return Index(config, uid=uid)
+        raise Exception('Uid is needed to find index')
```

### Comparing `meilisearch-0.8.3/meilisearch/key.py` & `meilisearch-0.9.0/meilisearch/search.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,63 @@
+import urllib
 from meilisearch._httprequests import HttpRequests
 
-
-class Key:
+class Search:
     """
-    Key routes wrapper
+    Search routes wrapper
 
-    Index's parent that gives access to all the keys methods of meilisearch.
-    https://docs.meilisearch.com/references/keys.html
+    Index's parent that gives access to all the search methods of meilisearch.
+    https://docs.meilisearch.com/references/search.html#search-in-an-index
 
     Attributes
     ----------
-    index_path:
-        Index url path
+    search_path:
+        Search url path
     """
+    search_path = 'search'
 
-    key_path = 'keys'
-
-    def __init__(self, config):
+    def __init__(self, parent_path, config, uid=None, name=None):
         """
-        Attributes
+        Parameters
         ----------
         config : Config
             Config object containing permission and location of meilisearch
+        name: str
+            Name of the index on which to perform the index actions.
+        uid: str
+            Uid of the index on which to perform the index actions.
+        index_path: str
+            Index url path
         """
         self.config = config
-
-    def get_keys(self):
-        """Get all keys created
-
-        Get list of all the keys that were created and all their related information.
-
-        Returns
-        ----------
-        keys: list
-            List of keys and their information.
-            https://docs.meilisearch.com/references/keys.html#get-keys
-        """
-
-        return HttpRequests.get(self.config, self.key_path).json()
-
-    def get_key(self, key):
-        """Get information about a given key
+        self.name = name
+        self.uid = uid
+        self.index_path = parent_path
+
+    # pylint: disable=dangerous-default-value
+    # Not dangerous because opt_params is not modified in the method
+    # See: https://stackoverflow.com/questions/26320899/why-is-the-empty-dictionary-a-dangerous-default-value-in-python
+    def search(self, query, opt_params={}):
+        """Search in meilisearch
 
         Parameters
         ----------
-        key: str
-            Key value
+        query: str
+            String containing the searched word(s)
+        opt_params: dict
+            Dictionnary containing optional query parameters
+            https://docs.meilisearch.com/references/search.html#search-in-an-index
         Returns
         ----------
-        key: dict
-            Information about a given key
-            https://docs.meilisearch.com/references/keys.html#get-one-key
+        results: `dict`
+            Dictionnary with hits, offset, limit, processingTime and initial query
         """
-
-        return HttpRequests.get(self.config, '{}/{}'.format(self.key_path, key)).json()
-
-    def create_key(self, body):
-        """Create a key.
-
-        Create a key with custom permissions, scope, description and expire date.
-        More info here https://docs.meilisearch.com/advanced_guides/keys.html.
-
-        Parameters
-        ----------
-        body: dict
-            Dictionnary with all information linked to the key that will be created.
-            https://docs.meilisearch.com/references/keys.html#create-key
-        Returns
-        ----------
-        key: dict
-            Information about the created key
-        """
-
-        return HttpRequests.post(self.config, self.key_path, body).json()
-
-    def update_key(self, key, body):
-        """Update a key.
-
-        Update a key with custom permissions, scope, description and expire date.
-        More info here https://docs.meilisearch.com/advanced_guides/keys.html.
-
-        Parameters
-        ----------
-        key: str
-            Key value
-        body: dict
-            Dictionnary with all information to update.
-            https://docs.meilisearch.com/references/keys.html#update-key
-        Returns
-        ----------
-        key: dict
-            Information about the updated key
-        """
-
-        return HttpRequests.put(self.config, '{}/{}'.format(self.key_path, key), body).json()
-
-    def delete_key(self, key):
-        """Delete a key.
-
-        Delete a given key.
-        More info here https://docs.meilisearch.com/references/keys.html#delete-key
-
-        Parameters
-        ----------
-        key: str
-            Key value
-        """
-
-        return HttpRequests.delete(self.config, '{}/{}'.format(self.key_path, key))
+        search_param = {'q': query}
+        params = {**search_param, **opt_params}
+        return HttpRequests.get(
+            self.config,
+            '{}/{}/{}?{}'.format(
+                self.index_path,
+                self.uid,
+                self.search_path,
+                urllib.parse.urlencode(params))
+        )
```

### Comparing `meilisearch-0.8.3/meilisearch/schema.py` & `meilisearch-0.9.0/meilisearch/update.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 from meilisearch._httprequests import HttpRequests
 
-
-class Schema:
+class Update:
     """
-    Schema routes wrapper
+    Update routes wrapper
 
-    Index's parent that gives access to all the schemas methods of meilisearch.
-    https://docs.meilisearch.com/references/indexes.html#get-one-index-schema
+    Index's parent that gives access to all the update methods of MeiliSearch.
+    https://docs.meilisearch.com/references/updates.html#get-an-update-status
 
     Attributes
     ----------
-    schema_path:
-        Schema url path
+    update_path:
+        Update url path
     """
-
-    schema_path = 'schema'
+    update_path = 'updates'
 
     def __init__(self, parent_path, config, uid=None, name=None):
         """
         Parameters
         ----------
         config : Config
-            Config object containing permission and location of meilisearch
+            Config object containing permission and location of MeiliSearch
         name: str
             Name of the index on which to perform the index actions.
         uid: str
             Uid of the index on which to perform the index actions.
-        schema: dict
-            Schema definition of index.
         index_path: str
             Index url path
         """
-
         self.config = config
         self.name = name
         self.uid = uid
         self.index_path = parent_path
 
-    def get_schema(self):
-        """Get schema of index
+    def get_all_update_status(self):
+        """Get all update status from MeiliSearch
 
         Returns
         ----------
-        update: `dict`
-            Schema definition
+        update: `list`
+            List of all enqueued and processed actions of the index.
         """
+        return HttpRequests.get(
+            self.config,
+            '{}/{}/{}'.format(
+                self.index_path,
+                self.uid,
+                self.update_path
+            )
+        )
 
-        return HttpRequests.get(self.config, '{}/{}/{}'.format(
-            self.index_path,
-            self.uid,
-            self.schema_path)).json()
+    def get_update_status(self, update_id):
+        """Get one update from MeiliSearch
 
-    def update_schema(self, schema):
-        """Update schema of index
         Parameters
         ----------
-        schema: dict, optional
-            dict containing the schema of the index.
-            https://docs.meilisearch.com/main_concepts/indexes.html#schema-definition
+        update_id: int
+            identifier of the update to retieve
         Returns
         ----------
-        update: `dict`
-            Schema definition
+        update: `list`
+            List of all enqueued and processed actions of the index.
         """
-
-        return HttpRequests.put(
+        return HttpRequests.get(
             self.config,
-            '{}/{}/{}'.format(
+            '{}/{}/{}/{}'.format(
                 self.index_path,
                 self.uid,
-                self.schema_path),
-            schema).json()
+                self.update_path,
+                update_id
+            )
+        )
```

### Comparing `meilisearch-0.8.3/meilisearch/search.py` & `meilisearch-0.9.0/meilisearch/stat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,65 @@
-import urllib
 from meilisearch._httprequests import HttpRequests
 
-
-class Search:
+class Stat:
     """
-    Search routes wrapper
+    Stats routes wrapper
 
-    Index's parent that gives access to all the search methods of meilisearch.
-    https://docs.meilisearch.com/references/search.html#search-in-an-index
+    Index's parent that gives access to all the stats methods of MeiliSearch.
+    https://docs.meilisearch.com/references/stats.html#get-stat-of-an-index
 
     Attributes
     ----------
-    search_path:
-        Search url path
+    stat_path:
+        Version url path
     """
-
-    search_path = 'search'
+    stat_path = 'stats'
 
     def __init__(self, parent_path, config, uid=None, name=None):
         """
         Parameters
         ----------
         config : Config
-            Config object containing permission and location of meilisearch
+            Config object containing permission and location of MeiliSearch
         name: str
             Name of the index on which to perform the index actions.
         uid: str
             Uid of the index on which to perform the index actions.
-        schema: dict
-            Schema definition of index.
         index_path: str
             Index url path
         """
-
         self.config = config
         self.name = name
         self.uid = uid
         self.index_path = parent_path
 
-    def search(self, parameters):
-        """Search in meilisearch
+    def get_stats(self):
+        """Get stats of an index
 
-        Parameters
-        ----------
-        parameters: dict
-            Dictionnary containing all available query parameter from the search route
-            https://docs.meilisearch.com/references/search.html#search-in-an-index
+        Get information about number of documents, fieldsfrequencies, ...
+        https://docs.meilisearch.com/references/stats.html
         Returns
         ----------
-        results: `dict`
-            Dictionnary with hits, offset, limit, processingTime and initial query
+        stats: `dict`
+            Dictionnary containing stats about the given index.
         """
-
         return HttpRequests.get(
             self.config,
-            '{}/{}/{}?{}'.format(
+            '{}/{}/{}'.format(
                 self.index_path,
                 self.uid,
-                self.search_path,
-                urllib.parse.urlencode(parameters))
-        ).json()
+                self.stat_path,
+            )
+        )
+
+    @staticmethod
+    def get_all_stats(config):
+        """Get all stats of MeiliSearch
+
+        Get information about databasesize and all indexes
+        https://docs.meilisearch.com/references/stats.html
+        Returns
+        ----------
+        stats: `dict`
+            Dictionnary containing stats about your MeiliSearch instance
+        """
+        return HttpRequests.get(config, Stat.stat_path)
```

### Comparing `meilisearch-0.8.3/meilisearch/sys_info.py` & `meilisearch-0.9.0/meilisearch/sys_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from meilisearch._httprequests import HttpRequests
 
-
 class SysInfo:
     """
     Sys-info routes wrapper
 
     Index's parent that gives access to all the sys-info methods of meilisearch.
     https://docs.meilisearch.com/references/sys-info.html#get-pretty-system-information
-
     """
-
     sys_info_path = 'sys-info'
 
     def __init__(self, config):
         """
         Attributes
         ----------
         config : Config
@@ -27,8 +24,8 @@
         Get information about memory usage and processor usage.
 
         Returns
         ----------
         sys_info: dict
             Information about memory and processor usage.
         """
-        return HttpRequests.get(self.config, self.sys_info_path).json()
+        return HttpRequests.get(self.config, self.sys_info_path)
```

### Comparing `meilisearch-0.8.3/meilisearch/version.py` & `meilisearch-0.9.0/meilisearch/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from meilisearch._httprequests import HttpRequests
 
-
 class Version:
     """
     Version routes wrapper
 
     Index's parent that gives access to all the version methods of meilisearch.
     https://docs.meilisearch.com/references/version.html#get-version-of-meilisearch
 
@@ -24,15 +23,15 @@
         """Get version meilisearch
 
         Returns
         ----------
         version: dict
             Information about version of meilisearch.
         """
-        return HttpRequests.get(self.config, self.version_path).json()
+        return HttpRequests.get(self.config, self.version_path)
 
     def version(self):
         """Alias for get_version
 
         Returns
         ----------
         version: dict
```

### Comparing `meilisearch-0.8.3/meilisearch.egg-info/PKG-INFO` & `meilisearch-0.9.0/meilisearch.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,87 @@
 Metadata-Version: 2.1
 Name: meilisearch
-Version: 0.8.3
+Version: 0.9.0
 Summary: The python client for MeiliSearch API.
 Home-page: https://github.com/meilisearch/meilisearch-python
 Author: Charlotte Vermandel
 Author-email: charlotte@meilisearch.com
 License: UNKNOWN
 Project-URL: Documentation, https://docs.meilisearch.com/
-Description: # MeiliSearch Python Client
+Description: # MeiliSearch Python Client <!-- omit in toc -->
         
         [![PyPI version](https://badge.fury.io/py/meilisearch.svg)](https://badge.fury.io/py/meilisearch)
         [![Licence](https://img.shields.io/badge/licence-MIT-blue.svg)](https://img.shields.io/badge/licence-MIT-blue.svg)
         [![test Status](https://github.com/meilisearch/meilisearch-python/workflows/Pytest/badge.svg)](https://github.com/{owner}/{repo}/actions)
         
-        
         The python client for MeiliSearch API.
         
-        MeiliSearch provides an ultra relevant and instant full-text search. Our solution is open-source and you can check out [our repository here](https://github.com/meilisearch/MeiliDB).
+        MeiliSearch provides an ultra relevant and instant full-text search. Our solution is open-source and you can check out [our repository here](https://github.com/meilisearch/MeiliSearch).
         
         Here is the [MeiliSearch documentation](https://docs.meilisearch.com/) 📖
         
         ## Table of Contents <!-- omit in toc -->
         
         - [🔧 Installation](#-installation)
         - [🚀 Getting started](#-getting-started)
         - [🎬 Examples](#-examples)
           - [Indexes](#indexes)
           - [Documents](#documents)
           - [Update status](#update-status)
           - [Search](#search)
+        - [⚙️ Development Workflow](#️-development-workflow)
+          - [Install dependencies](#install-dependencies)
+          - [Tests and Linter](#tests-and-linter)
+          - [Release](#release)
         - [🤖 Compatibility with MeiliSearch](#-compatibility-with-meilisearch)
         
         ## 🔧 Installation
         
         With `pip3` in command line:
         
         ```bash
         pip3 install meilisearch
         ```
         
-        ### 🏃‍♀️ Run MeiliSearch
+        ### Run MeiliSearch <!-- omit in toc -->
         
-        There are many easy ways to [download and run a MeiliSearch instance](https://docs.meilisearch.com/guides/advanced_guides/binary.html#download-and-launch).
+        There are many easy ways to [download and run a MeiliSearch instance](https://docs.meilisearch.com/guides/advanced_guides/installation.html#download-and-launch).
         
         For example, if you use Docker:
         ```bash
-        $ docker run -it --rm -p 7700:7700 getmeili/meilisearch:latest --api-key=apiKey
+        $ docker run -it --rm -p 7700:7700 getmeili/meilisearch:latest --master-key=masterKey
         ```
         
         NB: you can also download MeiliSearch from **Homebrew** or **APT**.
         
         ## 🚀 Getting started
         
         #### Add documents <!-- omit in toc -->
         
         ```python
         import meilisearch
+        
         client = meilisearch.Client("http://127.0.0.1:7700", "apiKey")
-        index = client.create_index(name='books', uid='books_uid') # If your index does not exist
-        index = client.get_index('books_uid') # If you already created your index
+        index = client.create_index(uid='books_uid') # If your index does not exist
+        index = client.get_index('books_uid')        # If you already created your index
         
         documents = [
           { "id": 123,  "title": 'Pride and Prejudice' },
           { "id": 456,  "title": 'Le Petit Prince' },
           { "id": 1,    "title": 'Alice In Wonderland' },
           { "id": 1344, "title": 'The Hobbit' },
           { "id": 4,    "title": 'Harry Potter and the Half-Blood Prince' },
           { "id": 42,   "title": 'The Hitchhiker\'s Guide to the Galaxy' }
         ]
         
-        index.add_documents(documents) # asynchronous
+        index.add_documents(documents) # => { "updateId": 0 }
         ```
         
+        With the `updateId`, you can check the status (`processed` or `failed`) of your documents addition thanks to this [method](#update-status).
+        
         #### Search in index <!-- omit in toc -->
         ``` python
         # MeiliSearch is typo-tolerant:
         index.search({
           "q": 'hary pottre'
         })
         ```
@@ -99,74 +105,74 @@
         You can check out [the API documentation](https://docs.meilisearch.com/references/).
         
         ### Indexes
         
         #### Create an index <!-- omit in toc -->
         ```python
         # Create an index
-        client.create_index(name='Books')
-        # Create an index with a specific uid (uid must be unique)
-        client.create_index(name= 'Books', uid= 'books')
-        # Create an index with a schema
-        schema = {
-          "id":    ["displayed", "indexed", "identifier"],
-          "title": ["displayed", "indexed"]
-        }
-        client.create_index(name= 'Books', schema= schema)
+        client.create_index(uid='books')
+        # Create an index and give the primary-key
+        client.create_index(uid='books', primary_key='objectID')
         ```
         
         #### List all indexes <!-- omit in toc -->
         ```python
         client.get_indexes()
         ```
         
         #### Get an index object <!-- omit in toc -->
+        
         ```python
-        index = client.get_index(uid="books")
+        index = client.get_index('books')
         ```
         
         ### Documents
         
         #### Fetch documents <!-- omit in toc -->
+        
         ```python
         # Get one document
         index.get_document(123)
         # Get documents by batch
-        index.get_documents({ "offset": 10 , "limit": 20 })
+        index.get_documents({ 'offset': 10 , 'limit': 20 })
         ```
+        
         #### Add documents <!-- omit in toc -->
+        
         ```python
-        index.add_documents([{ "id": 2, "title": 'Madame Bovary' }])
+        index.add_documents([{ 'id': 2, 'title': 'Madame Bovary' }])
         ```
         
         Response:
         ```json
         {
             "updateId": 1
         }
         ```
         This `updateId` allows you to [track the current update](#update-status).
         
         #### Delete documents <!-- omit in toc -->
+        
         ```python
         # Delete one document
         index.delete_document(2)
         # Delete several documents
         index.delete_documents([1, 42])
-        # Delete all documents 
+        # Delete all documents
         index.delete_all_documents()
         ```
         
         ### Update status
+        
         ```python
-        # Get one update
+        # Get one update status
         # Parameter: the updateId got after an asynchronous request (e.g. documents addition)
-        index.get_update(1)
-        # Get all updates
-        index.get_updates()
+        index.get_update_status(1)
+        # Get all updates status
+        index.get_all_update_status()
         ```
         
         ### Search
         
         #### Basic search <!-- omit in toc -->
         
         ```python
@@ -216,18 +222,62 @@
             "offset": 0,
             "limit": 1,
             "processingTimeMs": 10,
             "query": "prince"
         }
         ```
         
+        ## ⚙️ Development Workflow
+        
+        If you want to contribute, this section describes the steps to follow.
+        
+        Thank you for your interest in a MeiliSearch tool! ♥️
+        
+        ### Install dependencies
+        
+        ```bash
+        $ pipenv install --dev
+        ```
+        
+        ### Tests and Linter
+        
+        Each PR should pass the tests and the linter to be accepted.
+        
+        ```bash
+        # Tests
+        $ docker run -d -p 7700:7700 getmeili/meilisearch:latest ./meilisearch --master-key=masterKey --no-analytics
+        $ pipenv run pytest meilisearch
+        # Linter
+        $ pipenv run pylint meilisearch
+        ```
+        
+        ### Release
+        
+        MeiliSearch tools follow the [Semantic Versioning Convention](https://semver.org/).
+        
+        You must do a PR modifying the file `setup.py` with the right version.<br>
+        
+        ```python
+        version="X.X.X"
+        ```
+        
+        Once the changes are merged on `master`, in your terminal, you must be on the `master` branch and push a new tag with the right version:
+        
+        ```bash
+        $ git checkout master
+        $ git pull origin master
+        $ git tag vX.X.X
+        $ git push --tag origin master
+        ```
+        
+        A GitHub Action will be triggered and push the new gem on [RubyGems](https://rubygems.org/gems/meilisearch).
         
         ## 🤖 Compatibility with MeiliSearch
         
-        This package works for MeiliSearch `v0.8.x`.
+        This package works for MeiliSearch `v0.9.x`.
         
 Keywords: search python meilisearch
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `meilisearch-0.8.3/setup.py` & `meilisearch-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 setup(
     install_requires=[
         "requests"
     ],
     name="meilisearch",  # Replace with your own username
-    version="0.8.3",
+    version="0.9.0",
     author="Charlotte Vermandel",
     author_email="charlotte@meilisearch.com",
     description="The python client for MeiliSearch API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meilisearch/meilisearch-python",
     packages=["meilisearch"],
```

