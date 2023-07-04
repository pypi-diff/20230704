# Comparing `tmp/nlp_service-1.4.8.tar.gz` & `tmp/nlp_service-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp_service-1.4.8.tar", max compression
+gzip compressed data, was "nlp_service-1.4.9.tar", max compression
```

## Comparing `nlp_service-1.4.8.tar` & `nlp_service-1.4.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-07-04 08:58:58.874066 nlp_service-1.4.8/LICENSE
--rw-r--r--   0        0        0     7887 2023-07-04 08:58:58.874066 nlp_service-1.4.8/README.md
--rw-r--r--   0        0        0      226 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/__init__.py
--rw-r--r--   0        0        0       42 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/__main__.py
--rw-r--r--   0        0        0     2259 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/client.py
--rw-r--r--   0        0        0    10441 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/infersent.py
--rw-r--r--   0        0        0        0 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/py.typed
--rw-r--r--   0        0        0    17139 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/server.py
--rw-r--r--   0        0        0     9147 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/similarity.py
--rw-r--r--   0        0        0      344 2023-07-04 08:58:58.874066 nlp_service-1.4.8/nlp_service/typing.py
--rw-r--r--   0        0        0     1361 2023-07-04 09:00:12.671492 nlp_service-1.4.8/pyproject.toml
--rw-r--r--   0        0        0     9650 1970-01-01 00:00:00.000000 nlp_service-1.4.8/setup.py
--rw-r--r--   0        0        0     9517 1970-01-01 00:00:00.000000 nlp_service-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-04 13:46:10.878733 nlp_service-1.4.9/LICENSE
+-rw-r--r--   0        0        0     7887 2023-07-04 13:46:10.878733 nlp_service-1.4.9/README.md
+-rw-r--r--   0        0        0      226 2023-07-04 13:46:10.878733 nlp_service-1.4.9/nlp_service/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-04 13:46:10.878733 nlp_service-1.4.9/nlp_service/__main__.py
+-rw-r--r--   0        0        0     2259 2023-07-04 13:46:10.878733 nlp_service-1.4.9/nlp_service/client.py
+-rw-r--r--   0        0        0    10441 2023-07-04 13:46:10.878733 nlp_service-1.4.9/nlp_service/infersent.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:46:10.878733 nlp_service-1.4.9/nlp_service/py.typed
+-rw-r--r--   0        0        0    17139 2023-07-04 13:46:10.878733 nlp_service-1.4.9/nlp_service/server.py
+-rw-r--r--   0        0        0     9147 2023-07-04 13:46:10.878733 nlp_service-1.4.9/nlp_service/similarity.py
+-rw-r--r--   0        0        0      344 2023-07-04 13:46:10.878733 nlp_service-1.4.9/nlp_service/typing.py
+-rw-r--r--   0        0        0     1361 2023-07-04 13:47:11.475345 nlp_service-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0     9650 1970-01-01 00:00:00.000000 nlp_service-1.4.9/setup.py
+-rw-r--r--   0        0        0     9517 1970-01-01 00:00:00.000000 nlp_service-1.4.9/PKG-INFO
```

### Comparing `nlp_service-1.4.8/LICENSE` & `nlp_service-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.8/README.md` & `nlp_service-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.8/nlp_service/client.py` & `nlp_service-1.4.9/nlp_service/client.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.8/nlp_service/infersent.py` & `nlp_service-1.4.9/nlp_service/infersent.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.8/nlp_service/server.py` & `nlp_service-1.4.9/nlp_service/server.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.8/nlp_service/similarity.py` & `nlp_service-1.4.9/nlp_service/similarity.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.8/pyproject.toml` & `nlp_service-1.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nlp-service"
-version = "1.4.8"
+version = "1.4.9"
 description = "Microservice for NLP tasks using gRPC"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/nlp-service"
 packages = [{ include = "nlp_service" }]
```

### Comparing `nlp_service-1.4.8/setup.py` & `nlp_service-1.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'wmd': ['gensim>=4.3.1,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['nlp-service = nlp_service.server:app']}
 
 setup_kwargs = {
     'name': 'nlp-service',
-    'version': '1.4.8',
+    'version': '1.4.9',
     'description': 'Microservice for NLP tasks using gRPC',
     'long_description': '# NLP Microservice\n\nThe goal of this project is to provide a [gRPC](https://grpc.io) server for resource-heavy NLP tasks&mdash;for instance, computing vectors/embeddings for words or sentences.\nBy using [protobuf](https://developers.google.com/protocol-buffers) internally, our NLP server provides native and strongly typed interfaces for many programming languages.\nThere are multiple advantages that arise from outsourcing such computations to such a server:\n\n- If multiple apps rely on NLP, the underlying models (which are usually quite large) only need to be loaded once into the main memory.\n- All programming languages supported by gRPC get easy access to state-of-the-art NLP architectures (e.g., transformers).\n- The logic is consolidated at a central place, drastically decreasing the maintenance effort required.\n\nIn addition to the server, we also provide a client containing convenience functions.\nThis makes it easier for python applications to interact with the gRPC server.\nWe will discuss the client at the end of this README.\n\n## Installation and Setup\n\nWe are using `nix` and `poetry` to manage the dependencies and provide a ready-to-use Docker image.\n\n### Docker (recommended)\n\nThe container caches the downloaded models, so you should not pass `--rm` to `docker run`.\n\n```sh\ndocker run ghcr.io/recap-utr/nlp-service:latest "0.0.0.0:50100"\n```\n\n### Nix (advanced)\n\n```sh\nnix run github:recap-utr/nlp-service -- "127.0.0.1:50100"\n# or after cloning this repository\nnix develop -c poetry run python -m nlp_service "127.0.0.1:50100"\n```\n\n### Poetry (advanced)\n\n```sh\n# The server dependencies are optional, thus they have to be installed explicitly.\npoetry install --extras all\n# To run the server, you need to specify the address it should listen on.\n# In this example, it should liston on port 5678 on localhost.\npoetry run python -m nlp_service "127.0.0.1:50100"\n```\n\n## General Usage\n\nOnce the server is running, you are free to call any of the functions defined in the underlying [protobuf file](https://github.com/recap-utr/arg-services/blob/main/arg_services/nlp/v1/nlp.proto).\nThe corresponding documentation is located at the [Buf Schema Registry](https://buf.build/recap/arg-services/docs/main:arg_services.nlp.v1).\n_Please note:_ The examples here use the Python programming language, but are also directly applicable to any other language supported by gRPC.\n\n```python\nimport grpc\nfrom arg_services.nlp.v1 import nlp_pb2, nlp_pb2_grpc\n\n# First of all, we are creating a channel (i.e., establish a connection to our server)\nchannel = grpc.insecure_channel("127.0.0.1:5678")\n\n# The channel can now be used to create the actual client (allowing us to call all available functions)\nclient = nlp_pb2_grpc.NlpServiceStub(channel)\n\n# Now the time has come to prepare our actual function call.\n# We will start by creating a very simple NlpConfig with the default spacy model.\n# FOr details about the parameters, please have a look at the next section.\nconfig = nlp_pb2.NlpConfig(\n  language="en",\n  spacy_model="en_core_web_lg",\n)\n\n# Next, we will build a request to query vectors from our server.\nrequest = nlp_pb2.VectorsRequest(\n  # The first parameter is a list of strings that shall be embedded by our server.\n  texts=["What a great tutorial!", "I will definitely recommend this to my friends."],\n  # Now we need to specify which embeddings have to be computed. In this example, we create one vector for each text\n  embedding_levels=[nlp_pb2.EmbeddingLevel.EMBEDDING_LEVEL_DOCUMENT],\n  # The only thing missing now is the spacy configuration we created in the previous step.\n  config=config\n)\n\n# Having created the request, we can now send it to the server and retrieve the corresponding response.\nresponse = client.Vectors(request)\n\n# Due to technical constraints, we cannot directly transfer numpy arrays, thus we convert our response.\nvectors = [np.array(entry.document.vector) for entry in response.vectors]\n```\n\n<!-- TODO: Prefer Vectors instead of Similarities for Python to increase performacne. -->\n\n## Advanced Usage\n\nA central piece for all available function is the `NlpConfig` message, allowing you to create even complex embedding models easily.\nIn addition to [its documentation](https://buf.build/recap/arg-services/docs/main:arg_services.nlp.v1), we will in the following present some examples to demonstrate the possibilities you have.\n\n```python\nfrom arg_services.nlp.v1 import nlp_pb2\n\n# In the example above, we already introduced a quite basic config:\nconfig = nlp_pb2.NlpConfig(\n  # You have to provide a language for every config: https://spacy.io/usage/models#languages\n  language="en",\n  # Also, you need to specify the model that spacy should load: https://spacy.io/models/en\n  spacy_model="en_core_web_lg",\n)\n\n# A central feature of our library is the possibility to combine multiple embedding models, potentially capturing more contextual information.\nconfig = nlp_pb2.NlpConfig(\n  language="en",\n  # This parameter expects a list of models. If you pass more than one, the respective vectors are **concatenated** to each other\n  # (e.g., two 300-dimensional embeddings will result in a 600-dimensional one).\n  # This approach is based on https://arxiv.org/abs/1803.01400\n  embedding_models=[\n    nlp_pb2.EmbeddingModel(\n      # First select the type of model you would like to use (e.g., SBERT/Sentence Transformers).\n      model_type=nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SENTENCE_TRANSFORMERS,\n      # Then select the actual model.\n      # Any of those specified on the website (https://www.sbert.net/docs/pretrained_models.html) are allowed.\n      model_name="all-mpnet-base-v2"\n    ),\n    nlp_pb2.EmbeddingModel(\n      # It is also possible to use a standard spacy model\n      model_type=nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SPACY,\n      model_name="en_core_web_lg",\n      # Since we have selected a word embedding (i.e., it cannot directly encode sentences), the token vectors need to be aggregated somehow.\n      # The default strategy is to use the arithmetic mean, but you are free to use other strategies (e.g., the geometric mean).\n      pooling_type=nlp_pb2.Pooling.POOLING_GMEAN\n    ),\n    nlp_pb2.EmbeddingModel(\n      model_type=nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SPACY,\n      model_name="en_core_web_lg",\n      # Alternatively, it is also possible to use the generalized mean / power mean.\n      # In this example, the selected pmean corresponds to the geometic mean (thus this embedding is identical to the previous one).\n      # This approach is based on https://arxiv.org/abs/1803.01400\n      pmean=0\n    )\n  ]\n  # This setting is now optional and only needed if you need spacy features (e.g., POS tagging) besides embeddings.\n  # spacy_model="en_core_web_lg",\n)\n\n# If computing the similarity between strings, you get one additional parameter.\nconfig = nlp_pb2.NlpConfig(\n  language="en",\n  # To keep the example simple, we will now only use a single spacy model instead of the more powerful embedding models.\n  # However, it is of course possible to use them here as well.\n  spacy_model="en_core_web_lg",\n  # If not specified, we will always use the cosine similarity when comparing two strings.\n  # As indicated in a recent paper (https://arxiv.org/abs/1904.13264), you may achieve better results with alternative approaches like DynaMax Jaccard.\n  # Please note that this particular method ignores your selected pooling method due to the fact that even plain word embeddings are not pooled at all.\n  similarity_method=nlp_pb2.SimilarityMethod.SIMILARITY_METHOD_DYNAMAX_JACCARD\n)\n\n# It is also possible to determine a similarity score without the use of embeddings.\nconfig = nlp_pb2.NlpConfig(\n  language="en",\n  spacy_model="en_core_web_sm",\n  # Traditional metric (Jaccard similarity and Levenshtein edit distance) are also available\n  similarity_method=nlp_pb2.SimilarityMethod.SIMILARITY_METHOD_EDIT\n)\n```\n',
     'author': 'Mirko Lenz',
     'author_email': 'info@mirko-lenz.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://recap.uni-trier.de',
```

### Comparing `nlp_service-1.4.8/PKG-INFO` & `nlp_service-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-service
-Version: 1.4.8
+Version: 1.4.9
 Summary: Microservice for NLP tasks using gRPC
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

