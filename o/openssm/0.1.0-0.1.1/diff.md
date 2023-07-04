# Comparing `tmp/openssm-0.1.0.tar.gz` & `tmp/openssm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openssm-0.1.0.tar", max compression
+gzip compressed data, was "openssm-0.1.1.tar", max compression
```

## Comparing `openssm-0.1.0.tar` & `openssm-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,32 @@
--rw-r--r--   0        0        0      573 2023-06-23 03:02:10.966991 openssm-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     6914 2023-06-28 22:45:05.438359 openssm-0.1.0/README.md
--rw-r--r--   0        0        0     1906 2023-06-28 22:38:58.361415 openssm-0.1.0/openssm/README.md
--rw-r--r--   0        0        0        0 2023-06-30 01:07:44.427623 openssm-0.1.0/openssm/__init__.py
--rw-r--r--   0        0        0       39 2023-06-26 22:01:23.102867 openssm-0.1.0/openssm/archive/models/README.md
--rw-r--r--   0        0        0       48 2023-06-26 22:01:23.102968 openssm-0.1.0/openssm/archive/models/pre_trained/README.md
--rw-r--r--   0        0        0        0 2023-06-26 22:01:23.102992 openssm-0.1.0/openssm/archive/models/test.py
--rw-r--r--   0        0        0       50 2023-06-26 22:01:23.103133 openssm-0.1.0/openssm/archive/models/user_trained/README.md
--rw-r--r--   0        0        0       54 2023-06-26 22:01:23.103241 openssm-0.1.0/openssm/archive/models/validation/README.md
--rw-r--r--   0        0        0       45 2023-06-26 22:01:23.103348 openssm-0.1.0/openssm/archive/models/version_control/README.md
--rw-r--r--   0        0        0        0 2023-06-26 22:01:23.103399 openssm-0.1.0/openssm/archive/training/README.md
--rw-r--r--   0        0        0        0 2023-06-26 22:01:23.103472 openssm-0.1.0/openssm/archive/training/fine_tuning/README.md
--rw-r--r--   0        0        0        0 2023-06-26 22:01:23.103541 openssm-0.1.0/openssm/archive/training/validation/README.md
--rw-r--r--   0        0        0       19 2023-06-26 22:01:23.103656 openssm-0.1.0/openssm/core/__init__.py
--rw-r--r--   0        0        0     1452 2023-06-30 00:59:08.392644 openssm-0.1.0/openssm/core/adapter/abstract_adapter.py
--rw-r--r--   0        0        0      779 2023-06-30 00:25:24.109372 openssm-0.1.0/openssm/core/adapter/base_adapter.py
--rw-r--r--   0        0        0     2511 2023-06-26 22:27:58.943445 openssm-0.1.0/openssm/core/adapter/llama_index_adapter.py
--rw-r--r--   0        0        0      199 2023-06-29 18:11:08.807277 openssm-0.1.0/openssm/core/backend/abstract_backend.py
--rw-r--r--   0        0        0      197 2023-06-30 00:59:34.626526 openssm-0.1.0/openssm/core/backend/base_backend.py
--rw-r--r--   0        0        0      108 2023-06-26 22:01:23.104217 openssm-0.1.0/openssm/core/config.py
--rw-r--r--   0        0        0     2557 2023-06-26 22:01:23.104334 openssm-0.1.0/openssm/core/db.py
--rw-r--r--   0        0        0     2015 2023-06-26 22:01:23.103785 openssm-0.1.0/openssm/core/old_abstract/ssm.py
--rw-r--r--   0        0        0      821 2023-06-30 00:23:55.379436 openssm-0.1.0/openssm/core/slm/abstract_slm.py
--rw-r--r--   0        0        0      492 2023-06-30 00:24:07.069670 openssm-0.1.0/openssm/core/slm/base_slm.py
--rw-r--r--   0        0        0     2283 2023-06-26 23:07:56.491649 openssm-0.1.0/openssm/core/slm/gpt3_slm.py
--rw-r--r--   0        0        0      417 2023-06-26 22:01:23.104723 openssm-0.1.0/openssm/core/slm/memory/conversation_db.py
--rw-r--r--   0        0        0     2557 2023-06-26 22:01:23.104816 openssm-0.1.0/openssm/core/slm/memory/db.py
--rw-r--r--   0        0        0     2159 2023-06-26 22:01:23.104938 openssm-0.1.0/openssm/core/slm/memory/sqlite_conversation_db.py
--rw-r--r--   0        0        0     2425 2023-06-29 23:12:46.371782 openssm-0.1.0/openssm/core/ssm/abstract_ssm.py
--rw-r--r--   0        0        0     2291 2023-06-30 00:57:17.005182 openssm-0.1.0/openssm/core/ssm/base_ssm.py
--rw-r--r--   0        0        0     1397 2023-06-26 23:10:02.329337 openssm-0.1.0/openssm/core/ssm/gpt3_llama_index_ssm.py
--rw-r--r--   0        0        0       58 2023-06-26 22:01:23.105328 openssm-0.1.0/openssm/industrial/interpretability/README.md
--rw-r--r--   0        0        0       60 2023-06-26 22:01:23.105422 openssm-0.1.0/openssm/industrial/monitoring/README.md
--rw-r--r--   0        0        0        0 2023-06-26 22:01:23.105470 openssm-0.1.0/openssm/industrial/security/README.md
--rw-r--r--   0        0        0        0 2023-06-26 22:01:23.105561 openssm-0.1.0/openssm/industrial/security/audit/README.md
--rw-r--r--   0        0        0        0 2023-06-26 22:01:23.105659 openssm-0.1.0/openssm/industrial/security/best_practices/README.md
--rw-r--r--   0        0        0       63 2023-06-26 22:01:23.105800 openssm-0.1.0/openssm/integration/README.md
--rw-r--r--   0        0        0     3574 2023-06-26 22:01:23.105923 openssm-0.1.0/openssm/integration/llamaindex/README.md
--rw-r--r--   0        0        0       34 2023-06-26 22:01:23.106015 openssm-0.1.0/openssm/integration/testing_tools/README.md
--rw-r--r--   0        0        0       19 2023-06-26 22:01:23.106104 openssm-0.1.0/openssm/old_ssm/__init__.py
--rw-r--r--   0        0        0     2015 2023-06-26 22:01:23.106226 openssm-0.1.0/openssm/old_ssm/abstract/ssm.py
--rw-r--r--   0        0        0      310 2023-06-30 01:39:44.768524 openssm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8465 1970-01-01 00:00:00.000000 openssm-0.1.0/setup.py
--rw-r--r--   0        0        0     7394 1970-01-01 00:00:00.000000 openssm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      573 2023-06-23 03:02:10.966991 openssm-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     7182 2023-07-03 00:52:17.391051 openssm-0.1.1/README.md
+-rw-r--r--   0        0        0     2155 2023-07-01 21:58:27.291702 openssm-0.1.1/openssm/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 08:00:20.796606 openssm-0.1.1/openssm/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-30 08:00:20.798353 openssm-0.1.1/openssm/core/__init__.py
+-rw-r--r--   0        0        0     1460 2023-07-04 00:52:59.822256 openssm-0.1.1/openssm/core/adapter/abstract_adapter.py
+-rw-r--r--   0        0        0      787 2023-07-04 00:53:21.362156 openssm-0.1.1/openssm/core/adapter/base_adapter.py
+-rw-r--r--   0        0        0     2511 2023-06-30 08:00:20.799517 openssm-0.1.1/openssm/core/adapter/llama_index_adapter.py
+-rw-r--r--   0        0        0      199 2023-06-30 08:00:20.799799 openssm-0.1.1/openssm/core/backend/abstract_backend.py
+-rw-r--r--   0        0        0      197 2023-06-30 08:00:20.800029 openssm-0.1.1/openssm/core/backend/base_backend.py
+-rw-r--r--   0        0        0      131 2023-07-02 02:54:05.726183 openssm-0.1.1/openssm/core/config.py
+-rw-r--r--   0        0        0      937 2023-07-04 00:53:07.955563 openssm-0.1.1/openssm/core/slm/abstract_slm.py
+-rw-r--r--   0        0        0      541 2023-07-04 00:53:28.106772 openssm-0.1.1/openssm/core/slm/base_slm.py
+-rw-r--r--   0        0        0     2816 2023-07-04 00:53:46.345313 openssm-0.1.1/openssm/core/slm/gpt3_slm.py
+-rw-r--r--   0        0        0      417 2023-06-30 08:00:20.801854 openssm-0.1.1/openssm/core/slm/memory/conversation_db.py
+-rw-r--r--   0        0        0     2557 2023-06-30 08:00:20.801951 openssm-0.1.1/openssm/core/slm/memory/db.py
+-rw-r--r--   0        0        0     2159 2023-06-30 08:00:20.802090 openssm-0.1.1/openssm/core/slm/memory/sqlite_conversation_db.py
+-rw-r--r--   0        0        0     2502 2023-07-04 00:48:07.330715 openssm-0.1.1/openssm/core/ssm/abstract_ssm.py
+-rw-r--r--   0        0        0     2416 2023-07-04 00:53:59.598963 openssm-0.1.1/openssm/core/ssm/base_ssm.py
+-rw-r--r--   0        0        0     1416 2023-07-04 00:54:09.537284 openssm-0.1.1/openssm/core/ssm/gpt3_llama_index_ssm.py
+-rw-r--r--   0        0        0      713 2023-07-04 00:54:27.315086 openssm-0.1.1/openssm/core/ssm/gpt3_ssm.py
+-rw-r--r--   0        0        0       58 2023-06-30 08:00:20.803155 openssm-0.1.1/openssm/industrial/interpretability/README.md
+-rw-r--r--   0        0        0       60 2023-06-30 08:00:20.803373 openssm-0.1.1/openssm/industrial/monitoring/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803462 openssm-0.1.1/openssm/industrial/security/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803611 openssm-0.1.1/openssm/industrial/security/audit/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 08:00:20.803745 openssm-0.1.1/openssm/industrial/security/best_practices/README.md
+-rw-r--r--   0        0        0       63 2023-06-30 08:00:20.803985 openssm-0.1.1/openssm/integration/README.md
+-rw-r--r--   0        0        0     3574 2023-06-30 08:00:20.804216 openssm-0.1.1/openssm/integration/llamaindex/README.md
+-rw-r--r--   0        0        0       34 2023-06-30 08:00:20.804401 openssm-0.1.1/openssm/integration/testing_tools/README.md
+-rw-r--r--   0        0        0      466 2023-07-04 00:59:33.571271 openssm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8499 1970-01-01 00:00:00.000000 openssm-0.1.1/setup.py
+-rw-r--r--   0        0        0     7777 1970-01-01 00:00:00.000000 openssm-0.1.1/PKG-INFO
```

### Comparing `openssm-0.1.0/LICENSE.md` & `openssm-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openssm-0.1.0/README.md` & `openssm-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-## OpenSSM – “Small Specialist Models” for Industrial AI
+# OpenSSM – “Small Specialist Models” for Industrial AI
+
 OpenSSM (pronounced `open-ess-ess-em`) is an open-source framework for Small Specialist Models (SSMs), which are key to enhancing
 trust, reliability, and safety in Industrial-AI applications. Harnessing the power of domain expertise, SSMs operate either
 alone or in "teams". They collaborate with other SSMs, planners, and sensors/actuators to deliver real-world problem-solving
 capabilities.
 
 Unlike Large Language Models (LLMs), which are computationally intensive and generalized, SSMs are lean, efficient, and
 designed specifically for individual domains. This focus makes them an optimal choice for businesses, SMEs, researchers,
 and developers seeking specialized and robust AI solutions for industrial applications.
 
-![SSM in Industrial AI](./diagrams/ssm-industrial-use-case.drawio.png)
+![SSM in Industrial AI](./docs/diagrams/ssm-industrial-use-case.drawio.png)
 
 A prime deployment scenario for SSMs is within the aiCALM (Collaborative Augmented Large Models) architecture. aiCALM
 represents a cohesive assembly of AI components tailored for sophisticated problem-solving capabilities. Within this
 framework, SSMs work with General Management Models (GMMs) and other components to solve complex, domain-specific, and
 industrial problems.
 
 ## Why SSM?
+
 The trend towards specialization in AI models is a clear trajectory seen by many in the field.
 
 > Specialization is crucial for quality .. not general purpose Al models – Eric Schmidt, Schmidt Foundation
-
 > .. small models .. for a specific task that are good –  Matei Zaharia, Databricks
-
 > .. small agents working together .. specific and best in their tasks – Harrison Chase, Langchain
-
 > .. small but highly capable expert models – Andrej Karpathy, OpenAI
-
 > .. small models are .. a massive paradigm shift .. about deploying AI models at scale – Rob Toews, Radical Ventures
 
 As predicted by Eric Schmidt and others, we will see “a rich ecosystem to emerge [of] high-value, specialized AI systems.”
 SSMs are the central part in the architecture of these systems.
 
 ## What OpenSSM Offers
+
 OpenSSM fills this gap directly, with the following benefits to the community, developers, and businesses:
 
 - **Industrial Focus:** SSMs are developed with a specific emphasis on industrial applications, addressing the unique
 requirements of trustworthiness, safety, reliability, and scalability inherent to this sector.
 
 - **Fast, Cost-Effective & Easy to Use:** SSMs are 100-1000x faster and more efficient than LLMs, making them accessible
 and cost-effective particularly for industrial usage where time and resources are critical factors.
@@ -52,64 +51,80 @@
 
 - **Vendor Independence:** OpenSSM allows everyone to build, train, and deploy their own domain-expert AI models, offering
 freedom from vendor lock-in and security concerns.
 
 - **Composable Expertise**: SSMs are fully composable, making it easy to combine domain expertise.
 
 ## Target Audience
+
 Our primary audience includes:
 
 - **Businesses and SMEs** wishing to leverage AI in their specific industrial context without relying on extensive
 computational resources or large vendor solutions.
 
 - **AI researchers and developers** keen on creating more efficient, robust, and domain-specific AI models for industrial applications.
 
 - **Open-source contributors** believing in democratizing industrial AI and eager to contribute to a community-driven
 project focused on building and sharing specialized AI models.
 
 - **Industries** with specific domain problems that can be tackled more effectively by a specialist AI model, enhancing
 the reliability and trustworthiness of AI solutions in an industrial setting.
 
 ## SSM Architecture
+
 At a high level, SSMs comprise a front-end Small Language Model (SLM), an adapter layer in the middle, and a wide range of
 back-end domain-knowledge sources. The SLM itself is a small, efficient, language model, which may be domain-specific or not,
 and may have been distilled from a larger model. Thus, domain knowledge may come from either, or both, the SLM and the backends.
 
-
-![High-Level SSM Architecture](./diagrams/ssm-key-components.drawio.png)
+![High-Level SSM Architecture](./docs/diagrams/ssm-key-components.drawio.png)
 
 The above diagram illustrates the high-level architecture of an SSM, which comprises three main components:
 
 1. Small Language Model (SLM): This forms the communication frontend of an SSM.
 
 2. Adapters (e.g., LlamaIndex): These provide the interface between the SLM and the domain-knowledge backends.
 
 3. Domain-Knowledge Backends: These include text files, documents, PDFs, databases, code, knowledge graphs, models, other SSMs, etc.
 
 SSMs communicate in both unstructured (natural language) and structured APIs, catering to a variety of real-world industrial systems.
 
-![SSM Composability](./diagrams/ssm-composability.drawio.png)
+![SSM Composability](./docs/diagrams/ssm-composability.drawio.png)
 
 The composable nature of SSMs allows for easy combination of domain-knowledge sources from multiple models.
 
 ## Getting Started
+
+See some example user programs in the [examples](./examples) directory. For example, to run the `chatssm` example, do:
+
+```bash
+% cd examples/chatssm
+% make clean
+% make
+```
+
+then open your browser to `http://localhost:8080` and chat with the SSM.
+
 You can begin contributing to the OpenSSM project or use our pre-trained SSMs for your industrial projects. See our [Getting
 Started Guide](link-to-guide) for more information.
 
 ## Roadmap
+
 - Play with SSMs in a hosted SSM sandbox, uploading your own domain knowledge
 - Create SSMs in your own development environment, and integrate SSMs into your own AI apps
 - Capture domain knowledge in various forms into your SSMs
 - Train SLMs via distillation of LLMs, teacher/student approaches, etc.
 - Apply SSMs in collaborative problem-solving AI systems
 
 ## Community
+
 Join our vibrant community of AI enthusiasts, researchers, developers, and businesses who are democratizing industrial AI
 through SSMs. Participate in the discussions, share your ideas, or ask for help on our [Community Forum](link-to-forum).
 
 ## Contribute
+
 OpenSSM is a community-driven initiative, and we warmly welcome contributions. Whether it's enhancing existing models,
 creating new SSMs for different industrial domains, or improving our documentation, every contribution counts. See our
 [Contribution Guide](docs/CONTRIBUTING.md) for more details.
 
 ## License
+
 OpenSSM is released under the [Apache 2.0 License](./LICENSE.md).
```

### Comparing `openssm-0.1.0/openssm/README.md` & `openssm-0.1.1/openssm/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-## OpenSSM Framework Library
-![OpenSSM Key Components](../diagrams/ssm-key-components.drawio.png)
+# OpenSSM Framework Library
+
+![OpenSSM Key Components](../docs/diagrams/ssm-key-components.drawio.png)
 
 ## High-Level Class Diagram
-![OpenSSM High-Level Class Diagram](../diagrams/ssm-class-diagram.drawio.png)
+
+![OpenSSM High-Level Class Diagram](../docs/diagrams/ssm-class-diagram.drawio.png)
 
 ## Package Structure
-- `openssm`: Root package for OpenSSM. 
-  - `openssm.core`: Core functionalities of the SSMs. 
-    - `openssm.core.slm`: Small Language Model (SLM) functionality.
-    - `openssm.core.adapter`: Interface between the SLM and the domain-knowledge backends.
-    - `openssm.core.backend`: Interfaces to a variety of domain-knowledge backends.
+
+- `openssm`: Root package for OpenSSM.
+  - `openssm.core`: Core functionalities of the SSMs.
+    - `openssm.core.ssm`: Small Specialist Model (SSM) functionality.
+    - `openssm.core.slm`: Component: Small Language Model (SLM) functionality.
+    - `openssm.core.adapter`: Component: Interface between the SLM and the domain-knowledge backends.
+    - `openssm.core.backend`: Component: Interfaces to a variety of domain-knowledge backends.
   - `openssm.capture`: Tools and APIs for capturing and encoding domain knowledge into various backends.
   - `openssm.composer`: Tools for composing multiple SSMs together.
-  - `openssm.utils`: Utility functions and classes.
+  - `openssm.industrial`: Industrial-AI specific tools and APIs (trust, reliability, safety, etc.)
+  - `openssm.integration`: Tools for integrating SSMs into industrial applications.
 
 - `tests`: Unit tests for the framework's components (located at the top level of the project).
 
 - `apps`: Example applications using SSMs (located at the top level of the project).
 
 - `docs`: OpenSSM project documentation (located at the top level of the project).
 
 ## Getting Started
+
 You can begin contributing to the OpenSSM project or use our pre-trained SSMs for your industrial projects. See our [Getting
 Started Guide](link-to-guide) for more information.
 
 ## Community
+
 Join our vibrant community of AI enthusiasts, researchers, developers, and businesses who are democratizing industrial AI
 through SSMs. Participate in the discussions, share your ideas, or ask for help on our [Community Forum](link-to-forum).
 
 ## Contribute
+
 OpenSSM is a community-driven initiative, and we warmly welcome contributions. Whether it's enhancing existing models,
 creating new SSMs for different industrial domains, or improving our documentation, every contribution counts. See our
 [Contribution Guide](../docs/CONTRIBUTING.md) for more details.
 
 ## License
-OpenSSM is released under the [Apache 2.0 License](../LICENSE.md).
+
+OpenSSM is released under the [Apache 2.0 License](../LICENSE.md).
```

### Comparing `openssm-0.1.0/openssm/core/adapter/abstract_adapter.py` & `openssm-0.1.1/openssm/core/adapter/abstract_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from core.backend.abstract_backend import AbstractBackend
+from openssm.core.backend.abstract_backend import AbstractBackend
 
 
 class AbstractAdapter(ABC):
     """
     The AbstractAdapter serves as the base for all concrete Adapter classes.
     It provides an interface for interaction between the Small Language Model
     (SLM) and the Backend.
```

### Comparing `openssm-0.1.0/openssm/core/adapter/base_adapter.py` & `openssm-0.1.1/openssm/core/adapter/base_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .abstract_adapter import AbstractAdapter
-from core.backend.abstract_backend import AbstractBackend
+from openssm.core.backend.abstract_backend import AbstractBackend
 
 
 class BaseAdapter(AbstractAdapter):
     def __init__(self, backends: list = None):
         self.backends = backends or []
 
     def get_backends(self) -> list[AbstractBackend]:
```

### Comparing `openssm-0.1.0/openssm/core/adapter/llama_index_adapter.py` & `openssm-0.1.1/openssm/core/adapter/llama_index_adapter.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.0/openssm/core/db.py` & `openssm-0.1.1/openssm/core/slm/memory/db.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.0/openssm/core/slm/abstract_slm.py` & `openssm-0.1.1/openssm/core/slm/abstract_slm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from core.adapter.abstract_adapter import AbstractAdapter
+from openssm.core.adapter.abstract_adapter import AbstractAdapter
 
 
 class AbstractSLM(ABC):
     """
     The AbstractSLM serves as the base for all concrete Small Language Models
     (SLMs). It provides an interface for natural language communication and
     structured API interactions.
@@ -16,15 +16,20 @@
 
     @abstractmethod
     def set_adapter(self, adapter: AbstractAdapter):
         """Sets our adapter"""
         pass
 
     @abstractmethod
-    def discuss(self, conversation_id: str, user_input: str):
-        """Processes a natural language conversation input."""
+    def discuss(self,
+                conversation_id: str,
+                user_input: list[dict]) -> list[dict]:
+        """
+        Processes a natural language conversation input
+        and returns a list of replies
+        """
         pass
 
     @abstractmethod
     def reset_memory(self):
         """Resets our conversation memory"""
         pass
```

### Comparing `openssm-0.1.0/openssm/core/slm/memory/sqlite_conversation_db.py` & `openssm-0.1.1/openssm/core/slm/memory/sqlite_conversation_db.py`

 * *Files identical despite different names*

### Comparing `openssm-0.1.0/openssm/core/ssm/abstract_ssm.py` & `openssm-0.1.1/openssm/core/ssm/abstract_ssm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
-from core.slm.abstract_slm import AbstractSLM
-from core.adapter.abstract_adapter import AbstractAdapter
-from core.backend.abstract_backend import AbstractBackend
+from openssm.core.slm.abstract_slm import AbstractSLM
+from openssm.core.adapter.abstract_adapter import AbstractAdapter
+from openssm.core.backend.abstract_backend import AbstractBackend
 
 
 class AbstractSSM(ABC):
     """
     The AbstractSSM serves as the base for all concrete Small Specialist
     Models (SSMs).
     """
@@ -22,15 +22,17 @@
 
     @abstractmethod
     def get_backends(self) -> list[AbstractBackend]:
         """Returns our backends"""
         pass
 
     @abstractmethod
-    def discuss(self, conversation_id: str, user_input: str):
+    def discuss(self,
+                conversation_id: str,
+                user_input: list[dict]) -> list[dict]:
         """Processes a natural language conversation input."""
         pass
 
     @abstractmethod
     def api_call(self, function_name, *args, **kwargs):
         """Processes a structured API call."""
         pass
```

### Comparing `openssm-0.1.0/openssm/core/ssm/base_ssm.py` & `openssm-0.1.1/openssm/core/ssm/base_ssm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .abstract_ssm import AbstractSSM
-from core.slm.abstract_slm import AbstractSLM
-from core.adapter.abstract_adapter import AbstractAdapter
-from core.backend.abstract_backend import AbstractBackend
+from openssm.core.slm.abstract_slm import AbstractSLM
+from openssm.core.adapter.abstract_adapter import AbstractAdapter
+from openssm.core.backend.abstract_backend import AbstractBackend
 
 
 class BaseSSM(AbstractSSM):
     def __init__(self,
                  slm: AbstractSLM = None,
                  adapter: AbstractAdapter = None,
                  backends: list[AbstractBackend] = None):
@@ -15,23 +15,28 @@
         if (adapter is not None):
             adapter.set_backends(backends)
 
     def get_slm(self) -> AbstractSLM:
         return self.slm
 
     def get_adapter(self) -> AbstractAdapter:
-        return None if self.get_slm() is None else self.get_slm().get_adapter()
+        if self.get_slm() is None:
+            return None
+        else:
+            return self.get_slm().get_adapter()
 
     def get_backends(self) -> list[AbstractBackend]:
         if self.get_adapter() is None:
             return None
         else:
-            self.get_adapter().get_backends()
+            return self.get_adapter().get_backends()
 
-    def discuss(self, conversation_id: str, user_input: str):
+    def discuss(self,
+                conversation_id: str,
+                user_input: list[dict]) -> list[dict]:
         return self.get_slm().discuss(conversation_id, user_input)
 
     def api_call(self, function_name, *args, **kwargs):
         return self.get_adapter().api_call(function_name, *args, **kwargs)
 
     def reset_memory(self):
         if self.get_slm() is not None:
```

### Comparing `openssm-0.1.0/openssm/core/ssm/gpt3_llama_index_ssm.py` & `openssm-0.1.1/openssm/core/ssm/gpt3_llama_index_ssm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from .base_ssm import BaseSSM
-from core.slm.gpt3_slm import GPT3SLM
-from core.adapter.llama_index_adapter import LlamaIndexAdapter
-from core.backend.abstract_backend import AbstractBackend
+from openssm.core.slm.gpt3_slm import GPT3ChatCompletionSLM
+from openssm.core.backend.abstract_backend import AbstractBackend
+
 
 class GPT3LlamaIndexSSM(BaseSSM):
     def __init__(self, backends: list[AbstractBackend]):
-        slm = GPT3SLM()
-        #adapter = LlamaIndexAdapter()
-        adapter = None # FIXME
-        backends = None # FIXME
+        slm = GPT3ChatCompletionSLM()
+        # adapter = LlamaIndexAdapter()
+        adapter = None  # FIXME
+        backends = None  # FIXME
         super().__init__(slm, adapter, backends)
 
     def process(self, conversation_id: str, user_input: str):
-        # The SLM parses the user input and translates it into one or more calls to the Adapter
+        # The SLM parses the user input and translates it
+        # into one or more calls to the Adapter
         adapter_calls = self.slm.process(user_input)
         
         responses = []
         for call in adapter_calls:
             method = call['method']
             params = call['params']
 
-            # The Adapter executes the method and interacts with the appropriate Backend(s)
+            # The Adapter executes the method and
+            # interacts with the appropriate Backend(s)
             if hasattr(self.adapter, method):
                 result = getattr(self.adapter, method)(*params)
                 responses.append(result)
 
-        # The SLM then translates the Adapter responses back into natural language
+        # The SLM then translates the Adapter responses
+        # back into natural language
         output = self.slm.generate_output(responses)
         return output
 
     def add_backend(self, backend: AbstractBackend):
         self.backends.append(backend)
 
     def remove_backend(self, backend: AbstractBackend):
```

### Comparing `openssm-0.1.0/openssm/integration/llamaindex/README.md` & `openssm-0.1.1/openssm/integration/llamaindex/README.md`

 * *Files identical despite different names*

### Comparing `openssm-0.1.0/setup.py` & `openssm-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,44 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['openssm',
- 'openssm.archive.models',
  'openssm.core',
  'openssm.core.adapter',
  'openssm.core.backend',
- 'openssm.core.old_abstract',
  'openssm.core.slm',
  'openssm.core.slm.memory',
- 'openssm.core.ssm',
- 'openssm.old_ssm',
- 'openssm.old_ssm.abstract']
+ 'openssm.core.ssm']
 
 package_data = \
 {'': ['*'],
- 'openssm': ['archive/training/*',
-             'archive/training/fine_tuning/*',
-             'archive/training/validation/*',
-             'industrial/interpretability/*',
+ 'openssm': ['industrial/interpretability/*',
              'industrial/monitoring/*',
              'industrial/security/*',
              'industrial/security/audit/*',
              'industrial/security/best_practices/*',
              'integration/*',
              'integration/llamaindex/*',
-             'integration/testing_tools/*'],
- 'openssm.archive.models': ['pre_trained/*',
-                            'user_trained/*',
-                            'validation/*',
-                            'version_control/*']}
+             'integration/testing_tools/*']}
+
+install_requires = \
+['llama-hub>=0.0.4', 'llama-index>=0.6.33', 'pypdf>=3.11.0', 'pytest>=7.0.0']
 
 setup_kwargs = {
     'name': 'openssm',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': "OpenSSM – 'Small Specialist Models' for Industrial AI",
-    'long_description': '## OpenSSM – “Small Specialist Models” for Industrial AI\nOpenSSM (pronounced `open-ess-ess-em`) is an open-source framework for Small Specialist Models (SSMs), which are key to enhancing\ntrust, reliability, and safety in Industrial-AI applications. Harnessing the power of domain expertise, SSMs operate either\nalone or in "teams". They collaborate with other SSMs, planners, and sensors/actuators to deliver real-world problem-solving\ncapabilities.\n\nUnlike Large Language Models (LLMs), which are computationally intensive and generalized, SSMs are lean, efficient, and\ndesigned specifically for individual domains. This focus makes them an optimal choice for businesses, SMEs, researchers,\nand developers seeking specialized and robust AI solutions for industrial applications.\n\n![SSM in Industrial AI](./diagrams/ssm-industrial-use-case.drawio.png)\n\nA prime deployment scenario for SSMs is within the aiCALM (Collaborative Augmented Large Models) architecture. aiCALM\nrepresents a cohesive assembly of AI components tailored for sophisticated problem-solving capabilities. Within this\nframework, SSMs work with General Management Models (GMMs) and other components to solve complex, domain-specific, and\nindustrial problems.\n\n## Why SSM?\nThe trend towards specialization in AI models is a clear trajectory seen by many in the field.\n\n> Specialization is crucial for quality .. not general purpose Al models – Eric Schmidt, Schmidt Foundation\n\n> .. small models .. for a specific task that are good –  Matei Zaharia, Databricks\n\n> .. small agents working together .. specific and best in their tasks – Harrison Chase, Langchain\n\n> .. small but highly capable expert models – Andrej Karpathy, OpenAI\n\n> .. small models are .. a massive paradigm shift .. about deploying AI models at scale – Rob Toews, Radical Ventures\n\nAs predicted by Eric Schmidt and others, we will see “a rich ecosystem to emerge [of] high-value, specialized AI systems.”\nSSMs are the central part in the architecture of these systems.\n\n## What OpenSSM Offers\nOpenSSM fills this gap directly, with the following benefits to the community, developers, and businesses:\n\n- **Industrial Focus:** SSMs are developed with a specific emphasis on industrial applications, addressing the unique\nrequirements of trustworthiness, safety, reliability, and scalability inherent to this sector.\n\n- **Fast, Cost-Effective & Easy to Use:** SSMs are 100-1000x faster and more efficient than LLMs, making them accessible\nand cost-effective particularly for industrial usage where time and resources are critical factors.\n\n- **Easy Knowledge Capture:** OpenSSM has easy-to-use tools for capturing domain knowledge in diverse forms: books, operaring manuals, databases, knowledge graphs, text files, and code.\n\n- **Powerful Operations on Captured Knowledge:** OpenSSM enables both knowledge query and inferencing/predictive capabilities based on the domain-specific knowledge.\n\n- **Collaborative Problem-Solving**: SSMs are designed to work in problem-solving "teams". Multi-SSM collaboration is a first-class design feature, not an afterthought.\n\n- **Reliable Domain Expertise:** Each SSM has expertise in a particular field or equipment, offering precise and specialized\nknowledge, thereby enhancing trustworthiness, reliability, and safety for Industrial-AI applications. With self-reasoning,\ncausal reasoning, and retrieval-based knowledge, SSMs provide a trustable source of domain expertise.\n\n- **Vendor Independence:** OpenSSM allows everyone to build, train, and deploy their own domain-expert AI models, offering\nfreedom from vendor lock-in and security concerns.\n\n- **Composable Expertise**: SSMs are fully composable, making it easy to combine domain expertise.\n\n## Target Audience\nOur primary audience includes:\n\n- **Businesses and SMEs** wishing to leverage AI in their specific industrial context without relying on extensive\ncomputational resources or large vendor solutions.\n\n- **AI researchers and developers** keen on creating more efficient, robust, and domain-specific AI models for industrial applications.\n\n- **Open-source contributors** believing in democratizing industrial AI and eager to contribute to a community-driven\nproject focused on building and sharing specialized AI models.\n\n- **Industries** with specific domain problems that can be tackled more effectively by a specialist AI model, enhancing\nthe reliability and trustworthiness of AI solutions in an industrial setting.\n\n## SSM Architecture\nAt a high level, SSMs comprise a front-end Small Language Model (SLM), an adapter layer in the middle, and a wide range of\nback-end domain-knowledge sources. The SLM itself is a small, efficient, language model, which may be domain-specific or not,\nand may have been distilled from a larger model. Thus, domain knowledge may come from either, or both, the SLM and the backends.\n\n\n![High-Level SSM Architecture](./diagrams/ssm-key-components.drawio.png)\n\nThe above diagram illustrates the high-level architecture of an SSM, which comprises three main components:\n\n1. Small Language Model (SLM): This forms the communication frontend of an SSM.\n\n2. Adapters (e.g., LlamaIndex): These provide the interface between the SLM and the domain-knowledge backends.\n\n3. Domain-Knowledge Backends: These include text files, documents, PDFs, databases, code, knowledge graphs, models, other SSMs, etc.\n\nSSMs communicate in both unstructured (natural language) and structured APIs, catering to a variety of real-world industrial systems.\n\n![SSM Composability](./diagrams/ssm-composability.drawio.png)\n\nThe composable nature of SSMs allows for easy combination of domain-knowledge sources from multiple models.\n\n## Getting Started\nYou can begin contributing to the OpenSSM project or use our pre-trained SSMs for your industrial projects. See our [Getting\nStarted Guide](link-to-guide) for more information.\n\n## Roadmap\n- Play with SSMs in a hosted SSM sandbox, uploading your own domain knowledge\n- Create SSMs in your own development environment, and integrate SSMs into your own AI apps\n- Capture domain knowledge in various forms into your SSMs\n- Train SLMs via distillation of LLMs, teacher/student approaches, etc.\n- Apply SSMs in collaborative problem-solving AI systems\n\n## Community\nJoin our vibrant community of AI enthusiasts, researchers, developers, and businesses who are democratizing industrial AI\nthrough SSMs. Participate in the discussions, share your ideas, or ask for help on our [Community Forum](link-to-forum).\n\n## Contribute\nOpenSSM is a community-driven initiative, and we warmly welcome contributions. Whether it\'s enhancing existing models,\ncreating new SSMs for different industrial domains, or improving our documentation, every contribution counts. See our\n[Contribution Guide](docs/CONTRIBUTING.md) for more details.\n\n## License\nOpenSSM is released under the [Apache 2.0 License](./LICENSE.md).\n',
-    'author': 'ctn',
-    'author_email': 'ctn@aitomatic.com',
+    'long_description': '# OpenSSM – “Small Specialist Models” for Industrial AI\n\nOpenSSM (pronounced `open-ess-ess-em`) is an open-source framework for Small Specialist Models (SSMs), which are key to enhancing\ntrust, reliability, and safety in Industrial-AI applications. Harnessing the power of domain expertise, SSMs operate either\nalone or in "teams". They collaborate with other SSMs, planners, and sensors/actuators to deliver real-world problem-solving\ncapabilities.\n\nUnlike Large Language Models (LLMs), which are computationally intensive and generalized, SSMs are lean, efficient, and\ndesigned specifically for individual domains. This focus makes them an optimal choice for businesses, SMEs, researchers,\nand developers seeking specialized and robust AI solutions for industrial applications.\n\n![SSM in Industrial AI](./docs/diagrams/ssm-industrial-use-case.drawio.png)\n\nA prime deployment scenario for SSMs is within the aiCALM (Collaborative Augmented Large Models) architecture. aiCALM\nrepresents a cohesive assembly of AI components tailored for sophisticated problem-solving capabilities. Within this\nframework, SSMs work with General Management Models (GMMs) and other components to solve complex, domain-specific, and\nindustrial problems.\n\n## Why SSM?\n\nThe trend towards specialization in AI models is a clear trajectory seen by many in the field.\n\n> Specialization is crucial for quality .. not general purpose Al models – Eric Schmidt, Schmidt Foundation\n> .. small models .. for a specific task that are good –  Matei Zaharia, Databricks\n> .. small agents working together .. specific and best in their tasks – Harrison Chase, Langchain\n> .. small but highly capable expert models – Andrej Karpathy, OpenAI\n> .. small models are .. a massive paradigm shift .. about deploying AI models at scale – Rob Toews, Radical Ventures\n\nAs predicted by Eric Schmidt and others, we will see “a rich ecosystem to emerge [of] high-value, specialized AI systems.”\nSSMs are the central part in the architecture of these systems.\n\n## What OpenSSM Offers\n\nOpenSSM fills this gap directly, with the following benefits to the community, developers, and businesses:\n\n- **Industrial Focus:** SSMs are developed with a specific emphasis on industrial applications, addressing the unique\nrequirements of trustworthiness, safety, reliability, and scalability inherent to this sector.\n\n- **Fast, Cost-Effective & Easy to Use:** SSMs are 100-1000x faster and more efficient than LLMs, making them accessible\nand cost-effective particularly for industrial usage where time and resources are critical factors.\n\n- **Easy Knowledge Capture:** OpenSSM has easy-to-use tools for capturing domain knowledge in diverse forms: books, operaring manuals, databases, knowledge graphs, text files, and code.\n\n- **Powerful Operations on Captured Knowledge:** OpenSSM enables both knowledge query and inferencing/predictive capabilities based on the domain-specific knowledge.\n\n- **Collaborative Problem-Solving**: SSMs are designed to work in problem-solving "teams". Multi-SSM collaboration is a first-class design feature, not an afterthought.\n\n- **Reliable Domain Expertise:** Each SSM has expertise in a particular field or equipment, offering precise and specialized\nknowledge, thereby enhancing trustworthiness, reliability, and safety for Industrial-AI applications. With self-reasoning,\ncausal reasoning, and retrieval-based knowledge, SSMs provide a trustable source of domain expertise.\n\n- **Vendor Independence:** OpenSSM allows everyone to build, train, and deploy their own domain-expert AI models, offering\nfreedom from vendor lock-in and security concerns.\n\n- **Composable Expertise**: SSMs are fully composable, making it easy to combine domain expertise.\n\n## Target Audience\n\nOur primary audience includes:\n\n- **Businesses and SMEs** wishing to leverage AI in their specific industrial context without relying on extensive\ncomputational resources or large vendor solutions.\n\n- **AI researchers and developers** keen on creating more efficient, robust, and domain-specific AI models for industrial applications.\n\n- **Open-source contributors** believing in democratizing industrial AI and eager to contribute to a community-driven\nproject focused on building and sharing specialized AI models.\n\n- **Industries** with specific domain problems that can be tackled more effectively by a specialist AI model, enhancing\nthe reliability and trustworthiness of AI solutions in an industrial setting.\n\n## SSM Architecture\n\nAt a high level, SSMs comprise a front-end Small Language Model (SLM), an adapter layer in the middle, and a wide range of\nback-end domain-knowledge sources. The SLM itself is a small, efficient, language model, which may be domain-specific or not,\nand may have been distilled from a larger model. Thus, domain knowledge may come from either, or both, the SLM and the backends.\n\n![High-Level SSM Architecture](./docs/diagrams/ssm-key-components.drawio.png)\n\nThe above diagram illustrates the high-level architecture of an SSM, which comprises three main components:\n\n1. Small Language Model (SLM): This forms the communication frontend of an SSM.\n\n2. Adapters (e.g., LlamaIndex): These provide the interface between the SLM and the domain-knowledge backends.\n\n3. Domain-Knowledge Backends: These include text files, documents, PDFs, databases, code, knowledge graphs, models, other SSMs, etc.\n\nSSMs communicate in both unstructured (natural language) and structured APIs, catering to a variety of real-world industrial systems.\n\n![SSM Composability](./docs/diagrams/ssm-composability.drawio.png)\n\nThe composable nature of SSMs allows for easy combination of domain-knowledge sources from multiple models.\n\n## Getting Started\n\nSee some example user programs in the [examples](./examples) directory. For example, to run the `chatssm` example, do:\n\n```bash\n% cd examples/chatssm\n% make clean\n% make\n```\n\nthen open your browser to `http://localhost:8080` and chat with the SSM.\n\nYou can begin contributing to the OpenSSM project or use our pre-trained SSMs for your industrial projects. See our [Getting\nStarted Guide](link-to-guide) for more information.\n\n## Roadmap\n\n- Play with SSMs in a hosted SSM sandbox, uploading your own domain knowledge\n- Create SSMs in your own development environment, and integrate SSMs into your own AI apps\n- Capture domain knowledge in various forms into your SSMs\n- Train SLMs via distillation of LLMs, teacher/student approaches, etc.\n- Apply SSMs in collaborative problem-solving AI systems\n\n## Community\n\nJoin our vibrant community of AI enthusiasts, researchers, developers, and businesses who are democratizing industrial AI\nthrough SSMs. Participate in the discussions, share your ideas, or ask for help on our [Community Forum](link-to-forum).\n\n## Contribute\n\nOpenSSM is a community-driven initiative, and we warmly welcome contributions. Whether it\'s enhancing existing models,\ncreating new SSMs for different industrial domains, or improving our documentation, every contribution counts. See our\n[Contribution Guide](docs/CONTRIBUTING.md) for more details.\n\n## License\n\nOpenSSM is released under the [Apache 2.0 License](./LICENSE.md).\n',
+    'author': 'Aitomatic Engineering',
+    'author_email': 'engineering@aitomatic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
+    'install_requires': install_requires,
+    'python_requires': '>=3.8.1,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `openssm-0.1.0/PKG-INFO` & `openssm-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 Metadata-Version: 2.1
 Name: openssm
-Version: 0.1.0
+Version: 0.1.1
 Summary: OpenSSM – 'Small Specialist Models' for Industrial AI
-Author: ctn
-Author-email: ctn@aitomatic.com
-Requires-Python: >=3.8,<4.0
+Author: Aitomatic Engineering
+Author-email: engineering@aitomatic.com
+Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: llama-hub (>=0.0.4)
+Requires-Dist: llama-index (>=0.6.33)
+Requires-Dist: pypdf (>=3.11.0)
+Requires-Dist: pytest (>=7.0.0)
 Description-Content-Type: text/markdown
 
-## OpenSSM – “Small Specialist Models” for Industrial AI
+# OpenSSM – “Small Specialist Models” for Industrial AI
+
 OpenSSM (pronounced `open-ess-ess-em`) is an open-source framework for Small Specialist Models (SSMs), which are key to enhancing
 trust, reliability, and safety in Industrial-AI applications. Harnessing the power of domain expertise, SSMs operate either
 alone or in "teams". They collaborate with other SSMs, planners, and sensors/actuators to deliver real-world problem-solving
 capabilities.
 
 Unlike Large Language Models (LLMs), which are computationally intensive and generalized, SSMs are lean, efficient, and
 designed specifically for individual domains. This focus makes them an optimal choice for businesses, SMEs, researchers,
 and developers seeking specialized and robust AI solutions for industrial applications.
 
-![SSM in Industrial AI](./diagrams/ssm-industrial-use-case.drawio.png)
+![SSM in Industrial AI](./docs/diagrams/ssm-industrial-use-case.drawio.png)
 
 A prime deployment scenario for SSMs is within the aiCALM (Collaborative Augmented Large Models) architecture. aiCALM
 represents a cohesive assembly of AI components tailored for sophisticated problem-solving capabilities. Within this
 framework, SSMs work with General Management Models (GMMs) and other components to solve complex, domain-specific, and
 industrial problems.
 
 ## Why SSM?
+
 The trend towards specialization in AI models is a clear trajectory seen by many in the field.
 
 > Specialization is crucial for quality .. not general purpose Al models – Eric Schmidt, Schmidt Foundation
-
 > .. small models .. for a specific task that are good –  Matei Zaharia, Databricks
-
 > .. small agents working together .. specific and best in their tasks – Harrison Chase, Langchain
-
 > .. small but highly capable expert models – Andrej Karpathy, OpenAI
-
 > .. small models are .. a massive paradigm shift .. about deploying AI models at scale – Rob Toews, Radical Ventures
 
 As predicted by Eric Schmidt and others, we will see “a rich ecosystem to emerge [of] high-value, specialized AI systems.”
 SSMs are the central part in the architecture of these systems.
 
 ## What OpenSSM Offers
+
 OpenSSM fills this gap directly, with the following benefits to the community, developers, and businesses:
 
 - **Industrial Focus:** SSMs are developed with a specific emphasis on industrial applications, addressing the unique
 requirements of trustworthiness, safety, reliability, and scalability inherent to this sector.
 
 - **Fast, Cost-Effective & Easy to Use:** SSMs are 100-1000x faster and more efficient than LLMs, making them accessible
 and cost-effective particularly for industrial usage where time and resources are critical factors.
@@ -66,65 +68,81 @@
 
 - **Vendor Independence:** OpenSSM allows everyone to build, train, and deploy their own domain-expert AI models, offering
 freedom from vendor lock-in and security concerns.
 
 - **Composable Expertise**: SSMs are fully composable, making it easy to combine domain expertise.
 
 ## Target Audience
+
 Our primary audience includes:
 
 - **Businesses and SMEs** wishing to leverage AI in their specific industrial context without relying on extensive
 computational resources or large vendor solutions.
 
 - **AI researchers and developers** keen on creating more efficient, robust, and domain-specific AI models for industrial applications.
 
 - **Open-source contributors** believing in democratizing industrial AI and eager to contribute to a community-driven
 project focused on building and sharing specialized AI models.
 
 - **Industries** with specific domain problems that can be tackled more effectively by a specialist AI model, enhancing
 the reliability and trustworthiness of AI solutions in an industrial setting.
 
 ## SSM Architecture
+
 At a high level, SSMs comprise a front-end Small Language Model (SLM), an adapter layer in the middle, and a wide range of
 back-end domain-knowledge sources. The SLM itself is a small, efficient, language model, which may be domain-specific or not,
 and may have been distilled from a larger model. Thus, domain knowledge may come from either, or both, the SLM and the backends.
 
-
-![High-Level SSM Architecture](./diagrams/ssm-key-components.drawio.png)
+![High-Level SSM Architecture](./docs/diagrams/ssm-key-components.drawio.png)
 
 The above diagram illustrates the high-level architecture of an SSM, which comprises three main components:
 
 1. Small Language Model (SLM): This forms the communication frontend of an SSM.
 
 2. Adapters (e.g., LlamaIndex): These provide the interface between the SLM and the domain-knowledge backends.
 
 3. Domain-Knowledge Backends: These include text files, documents, PDFs, databases, code, knowledge graphs, models, other SSMs, etc.
 
 SSMs communicate in both unstructured (natural language) and structured APIs, catering to a variety of real-world industrial systems.
 
-![SSM Composability](./diagrams/ssm-composability.drawio.png)
+![SSM Composability](./docs/diagrams/ssm-composability.drawio.png)
 
 The composable nature of SSMs allows for easy combination of domain-knowledge sources from multiple models.
 
 ## Getting Started
+
+See some example user programs in the [examples](./examples) directory. For example, to run the `chatssm` example, do:
+
+```bash
+% cd examples/chatssm
+% make clean
+% make
+```
+
+then open your browser to `http://localhost:8080` and chat with the SSM.
+
 You can begin contributing to the OpenSSM project or use our pre-trained SSMs for your industrial projects. See our [Getting
 Started Guide](link-to-guide) for more information.
 
 ## Roadmap
+
 - Play with SSMs in a hosted SSM sandbox, uploading your own domain knowledge
 - Create SSMs in your own development environment, and integrate SSMs into your own AI apps
 - Capture domain knowledge in various forms into your SSMs
 - Train SLMs via distillation of LLMs, teacher/student approaches, etc.
 - Apply SSMs in collaborative problem-solving AI systems
 
 ## Community
+
 Join our vibrant community of AI enthusiasts, researchers, developers, and businesses who are democratizing industrial AI
 through SSMs. Participate in the discussions, share your ideas, or ask for help on our [Community Forum](link-to-forum).
 
 ## Contribute
+
 OpenSSM is a community-driven initiative, and we warmly welcome contributions. Whether it's enhancing existing models,
 creating new SSMs for different industrial domains, or improving our documentation, every contribution counts. See our
 [Contribution Guide](docs/CONTRIBUTING.md) for more details.
 
 ## License
+
 OpenSSM is released under the [Apache 2.0 License](./LICENSE.md).
```

