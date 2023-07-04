# Comparing `tmp/gimie-0.4.0.tar.gz` & `tmp/gimie-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimie-0.4.0.tar", max compression
+gzip compressed data, was "gimie-0.5.0.tar", max compression
```

## Comparing `gimie-0.4.0.tar` & `gimie-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-06-09 13:34:21.959745 gimie-0.4.0/LICENSE
--rw-r--r--   0        0        0     5072 2023-06-09 13:34:21.959745 gimie-0.4.0/README.md
--rw-r--r--   0        0        0      917 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/__init__.py
--rw-r--r--   0        0        0     2575 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/cli.py
--rw-r--r--   0        0        0     1028 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/graph/namespaces.py
--rw-r--r--   0        0        0     1074 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/graph/operations.py
--rw-r--r--   0        0        0     2946 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/models.py
--rw-r--r--   0        0        0     6723 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/project.py
--rw-r--r--   0        0        0     1391 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/sources/__init__.py
--rw-r--r--   0        0        0     1849 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/sources/abstract.py
--rw-r--r--   0        0        0     1544 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/sources/common/license.py
--rw-r--r--   0        0        0      929 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/sources/common/queries.py
--rw-r--r--   0        0        0     4708 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/sources/git.py
--rw-r--r--   0        0        0    10671 2023-06-09 13:34:21.959745 gimie-0.4.0/gimie/sources/github.py
--rw-r--r--   0        0        0    10741 2023-06-09 13:34:21.963745 gimie-0.4.0/gimie/sources/gitlab.py
--rw-r--r--   0        0        0     1832 2023-06-09 13:34:21.963745 gimie-0.4.0/gimie/utils.py
--rw-r--r--   0        0        0     3131 2023-06-09 13:34:21.963745 gimie-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6263 1970-01-01 00:00:00.000000 gimie-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-04 10:12:51.383570 gimie-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5866 2023-07-04 10:12:51.383570 gimie-0.5.0/README.md
+-rw-r--r--   0        0        0      917 2023-07-04 10:12:51.383570 gimie-0.5.0/gimie/__init__.py
+-rw-r--r--   0        0        0     2760 2023-07-04 10:12:51.383570 gimie-0.5.0/gimie/cli.py
+-rw-r--r--   0        0        0     1028 2023-07-04 10:12:51.383570 gimie-0.5.0/gimie/graph/namespaces.py
+-rw-r--r--   0        0        0     1074 2023-07-04 10:12:51.383570 gimie-0.5.0/gimie/graph/operations.py
+-rw-r--r--   0        0        0     2946 2023-07-04 10:12:51.383570 gimie-0.5.0/gimie/models.py
+-rw-r--r--   0        0        0     7262 2023-07-04 10:12:51.383570 gimie-0.5.0/gimie/project.py
+-rw-r--r--   0        0        0     1391 2023-07-04 10:12:51.387570 gimie-0.5.0/gimie/sources/__init__.py
+-rw-r--r--   0        0        0     2572 2023-07-04 10:12:51.387570 gimie-0.5.0/gimie/sources/abstract.py
+-rw-r--r--   0        0        0     1544 2023-07-04 10:12:51.387570 gimie-0.5.0/gimie/sources/common/license.py
+-rw-r--r--   0        0        0      929 2023-07-04 10:12:51.387570 gimie-0.5.0/gimie/sources/common/queries.py
+-rw-r--r--   0        0        0     4874 2023-07-04 10:12:51.387570 gimie-0.5.0/gimie/sources/git.py
+-rw-r--r--   0        0        0    10643 2023-07-04 10:12:51.387570 gimie-0.5.0/gimie/sources/github.py
+-rw-r--r--   0        0        0    10890 2023-07-04 10:12:51.387570 gimie-0.5.0/gimie/sources/gitlab.py
+-rw-r--r--   0        0        0     1832 2023-07-04 10:12:51.387570 gimie-0.5.0/gimie/utils.py
+-rw-r--r--   0        0        0     3172 2023-07-04 10:12:51.387570 gimie-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7105 1970-01-01 00:00:00.000000 gimie-0.5.0/PKG-INFO
```

### Comparing `gimie-0.4.0/LICENSE` & `gimie-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gimie-0.4.0/README.md` & `gimie-0.5.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 [![gimie](docs/logo.svg)](https://github.com/SDSC-ORD/gimie)
 
-[![PyPI version](https://badge.fury.io/py/gimie.svg)](https://badge.fury.io/py/gimie) [![Python Poetry Test](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml/badge.svg)](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml) [![docs](https://github.com/SDSC-ORD/gimie/actions/workflows/sphinx-docs.yml/badge.svg)](https://sdsc-ord.github.io/gimie)
+[![PyPI version](https://badge.fury.io/py/gimie.svg)](https://badge.fury.io/py/gimie) [![Python Poetry Test](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml/badge.svg)](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml) [![docs](https://github.com/SDSC-ORD/gimie/actions/workflows/sphinx-docs.yml/badge.svg)](https://sdsc-ord.github.io/gimie) [![Coverage Status](https://coveralls.io/repos/github/SDSC-ORD/gimie/badge.svg?branch=main)](https://coveralls.io/github/SDSC-ORD/gimie?branch=main)
 
 Gimie (GIt Meta Information Extractor) is a python library and command line tool to extract structured metadata from git repositories.
 
 
 ## Context
 Scientific code repositories contain valuable metadata which can be used to enrich existing catalogues, platforms or databases. This tool aims to easily extract structured metadata from a generic git repositories. It can extract extract metadata from the Git provider (GitHub or GitLab) or from the git index itself.
 
-## Installation
+----------------------------------------------------------------------
+
+Using Gimie: easy peasy, it's a 3 step process. 
+
+## STEP 1: Installation
 
 To install the stable version on PyPI:
 
 ```shell
 pip install gimie
 ```
 
@@ -27,79 +31,50 @@
 ```shell
 docker pull ghcr.io/sdsc-ord/gimie:latest
 
 # The access token can be provided as an environment variable
 docker run -e ACCESS_TOKEN=$ACCESS_TOKEN ghcr.io/sdsc-ord/gimie:latest gimie data <repo>
 ```
 
+## STEP 2 : Set your credentials
 
-### For development:
-
-activate a conda or virtual environment with Python 3.8 or higher
-
-```shell
-git clone https://github.com/SDSC-ORD/gimie && cd gimie
-make install
-```
-
-run tests:
-
-```shell
-make test
-```
-
-run checks:
-
-```shell
-make check
-```
+In order to access the github api, you need to provide a github token with the `read:org` scope. 
 
-build documentation:
+### A. Create access tokens
 
-```shell
-make doc
-```
+New to access tokens? Or don't know how to get your Github / Gitlab token ? 
 
-## Usage
+Have no fear, see
+[here for Github tokens](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) and [here for Gitlab tokens](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html).
+(Note: tokens are as precious as passwords! Treat them as such.)
 
-### Set your github credentials
+### B. Set your access tokens via the Terminal
 
-In order to avoid rate limits with the github api, you need to provide your github
-username and a github token with the `read:org` scope: see
-[here ](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
-on how to generate a github token.
+Gimie will use your access tokens to gather information for you. If you want info about a Github repo, Gimie needs your Github token; if you want info about a Gitlab Project then Gimie needs your Gitlab token.
 
-There are 2 options for setting up your github token in your local environment:
-
-**Option 1:**
-
-```
-cp .env.dist .env
+Add your tokens one by one in your terminal:
+your Github token:
+```bash
+export GITHUB_TOKEN=
 ```
-
-And then edit the `.env` file and put your github token in.
-
-**Option 2:**
-
-Add your github token in your terminal:
-
+and/or your Gitlab token:
 ```bash
-export ACCESS_TOKEN=
+export GITLAB_TOKEN=
 ```
 
-After the github token has been added, you can run the command without running into an github api limit.
-Otherwise you can still run the command, but might hit that limit after running the command several times.
+## STEP 3: GIMIE info ! Run Gimie
 
-### Run the command
+### As a command line tool
 
-As a command line tool:
 ```shell
 gimie data https://github.com/numpy/numpy
 ```
-As a python library:
+(want a Gitlab project instead? Just replace the URL in the command line) 
+
+### As a python library
 
 ```python
 from gimie.project import Project
 proj = Project("https://github.com/numpy/numpy)
 
 # To retrieve the rdflib.Graph object
 g = proj.to_graph()
@@ -120,28 +95,59 @@
 # To retrieve the serialized graph
 gh.serialize(format='ttl')
 ```
 [For a GitLab project, replace `gimie.sources.github` by `gimie.sources.gitlab`, `GithubExtractor` by `GitlabExtractor`, as well as the URL to the GitLab project.]
 
 ## Outputs
 
-The default output is JSON-ld, a JSON serialization of the [RDF](https://en.wikipedia.org/wiki/Resource_Description_Framework) data model. We follow the schema recommended by [codemeta](https://codemeta.github.io/).
-Supported formats are json-ld, turtle and n-triples.
+The default output is [Turtle](https://www.w3.org/TR/turtle/), a textual syntax for [RDF](https://en.wikipedia.org/wiki/Resource_Description_Framework) data model. We follow the schema recommended by [codemeta](https://codemeta.github.io/).
+Supported formats are turtle, json-ld and n-triples (by specifying the `--format` argument in your call i.e. `gimie data https://github.com/numpy/numpy --format 'ttl'`).
 
-### Limitations
+With no specifications, Gimie will print results in the terminal. Want to save Gimie output to a file? Add your file path to the end : `gimie data https://github.com/numpy/numpy > path_to_output/gimie_output.ttl`
 
-* Currently, gimie will only the first 100 contributors of a repository (in arbitrary order), and for each users, at most 100 affiliations.
-* If a Github repository is owned by an organization, all "mentionable users" are reported as contributors. This will include all members of the organization in addition to contributors.
+----------------------------------------------------------------------
 
 ## Contributing
 
 All contributions are welcome. New functions and classes should have associated tests and docstrings following the [numpy style guide](https://numpydoc.readthedocs.io/en/latest/format.html).
 
 The code formatting standard we use is [black](https://github.com/psf/black), with `--line-length=79` to follow [PEP8](https://peps.python.org/pep-0008/) recommendations. We use [pytest](https://docs.pytest.org/en/7.2.x/) as our testing framework. This project uses [pyproject.toml](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/) to define package information, requirements and tooling configuration.
 
+### For development:
+
+activate a conda or virtual environment with Python 3.8 or higher
+
+```shell
+git clone https://github.com/SDSC-ORD/gimie && cd gimie
+make install
+```
+
+run tests:
+
+```shell
+make test
+```
+
+run checks:
+
+```shell
+make check
+```
+for an easier use Github/Gitlab APIs, place your access tokens in the `.env` file: (and don't worry, the `.gitignore` will ignore them when you push to GitHub) 
+
+```
+cp .env.dist .env
+```
+
+build documentation:
+
+```shell
+make doc
+```
+
 ## Releases and Publishing on Pypi
 
 Releases are done via github release
 
 - a release will trigger a github workflow to publish the package on Pypi
 - Make sure to update to a new version in `pyproject.toml` before making the release
 - It is possible to test the publishing on Pypi.test by running a manual workflow: go to github actions and run the Workflow: 'Publish on Pypi Test'
```

### Comparing `gimie-0.4.0/gimie/__init__.py` & `gimie-0.5.0/gimie/__init__.py`

 * *Files identical despite different names*

### Comparing `gimie-0.4.0/gimie/cli.py` & `gimie-0.5.0/gimie/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,25 +52,30 @@
     url: str,
     format: SerializationFormat = typer.Option(
         "ttl",
         "--format",
         show_choices=True,
         help="Output serialization format for the RDF graph.",
     ),
+    base_url: Optional[str] = typer.Option(
+        None,
+        "--base-url",
+        help="Specify the base URL of the git provider. Inferred by default.",
+    ),
     version: Optional[bool] = typer.Option(
         None,
         "--version",
         help="Display version and exit",
         callback=version_callback,
     ),
 ):
     """Extract linked metadata from a Git repository at the target URL.
 
     The output is sent to stdout, and turtle is used as the default serialization format."""
-    proj = Project(url)
+    proj = Project(url, base_url=base_url)
     print(proj.serialize(format=format))
 
 
 @app.command()
 def advice(url: str):
     """Show a metadata completion report for a Git repository
     at the target URL.
```

### Comparing `gimie-0.4.0/gimie/graph/namespaces.py` & `gimie-0.5.0/gimie/graph/namespaces.py`

 * *Files identical despite different names*

### Comparing `gimie-0.4.0/gimie/graph/operations.py` & `gimie-0.5.0/gimie/graph/operations.py`

 * *Files identical despite different names*

### Comparing `gimie-0.4.0/gimie/models.py` & `gimie-0.5.0/gimie/models.py`

 * *Files identical despite different names*

### Comparing `gimie-0.4.0/gimie/project.py` & `gimie-0.5.0/gimie/project.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,58 +13,65 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Orchestration of multiple extractors for a given project.
 This is the main entry point for end-to-end analysis."""
 from tempfile import gettempdir, TemporaryDirectory
-from typing import Iterable, List, Optional, Union
+from typing import Iterable, List, Optional, Tuple, Union
 
 import shutil
 import git
 from rdflib import Graph
+from urllib.parse import urlparse
 
 from gimie.graph.operations import combine_graphs
 from gimie.utils import validate_url
 from gimie.sources import SOURCES
 from gimie.sources.abstract import Extractor
 from gimie.utils import validate_url
 
 
 class Project:
     """A class to represent a project's git repository.
 
 
     Parameters
     ----------
-    path :
-        The path to the repository, either a file path or a URL.
+    path:
+        The full path (URL) of the repository.
+    base_url:
+        The base URL of the git remote. Can be used to
+        specify delimitation between base URL and project name.
     sources:
         The metadata sources to use.
 
     Examples
     --------
     >>> proj = Project("https://github.com/SDSC-ORD/gimie")
     """
 
     def __init__(
-        self, path: str, sources: Optional[Union[str, Iterable[str]]] = None
+        self,
+        path: str,
+        base_url: Optional[str] = None,
+        sources: Optional[Union[Iterable[str], str]] = None,
     ):
 
         sources = normalize_sources(path, sources)
-        # Remember if we cloned to cleanup at the end
+        self.base_url = base_url
+        self.project_dir = None
         self._cloned = False
         if validate_url(path):
             self.url = path
             # We only need to clone a remote project
             # if a local extractor is enabled
             if any(map(is_local_source, sources)):
                 self.project_dir = self.clone(path)
         else:
-            self.url = None
             self.project_dir = path
 
         self.extractors = self.get_extractors(sources)
         for ex in self.extractors:
             ex.extract()
 
     def clone(self, url: str) -> str:
@@ -75,18 +82,20 @@
 
         return str(cloned.working_tree_dir)
 
     def get_extractors(self, sources: Iterable[str]) -> List[Extractor]:
 
         extractors: List[Extractor] = []
         for src in sources:
-            if is_remote_source(src):
-                extractor = get_extractor(self.url, src)  # type: ignore
-            else:
-                extractor = get_extractor(self.project_dir, src, _id=self.url)
+            extractor = get_extractor(
+                self.url,
+                src,
+                base_url=self.base_url,
+                local_path=self.project_dir,
+            )
             extractors.append(extractor)
 
         return extractors
 
     def to_graph(self) -> Graph:
         graphs = map(lambda ex: ex.to_graph(), self.extractors)
         combined_graph = combine_graphs(*graphs)
@@ -96,24 +105,31 @@
         return self.to_graph().serialize(format=format, **kwargs)
 
     def cleanup(self):
         """Recursively delete the project. Only works
         for remote (i.e. cloned) projects."""
         try:
             tempdir = gettempdir()
-            in_temp = self.project_dir.startswith(tempdir)
-            if self._cloned and in_temp:
-                shutil.rmtree(self.project_dir)
+            if self.project_dir is not None:
+                in_temp = self.project_dir.startswith(tempdir)
+                if self._cloned and in_temp:
+                    shutil.rmtree(self.project_dir)
         except AttributeError:
             pass
 
     def __del__(self):
         self.cleanup()
 
 
+def split_git_url(url) -> Tuple[str, str]:
+    base_url = urlparse(url).scheme + "://" + urlparse(url).netloc
+    project = urlparse(url).path.strip("/")
+    return base_url, project
+
+
 def normalize_sources(
     path: str, sources: Optional[Union[Iterable[str], str]] = None
 ) -> List[str]:
     """Input validation and normalization for metadata sources.
     Returns a list of all input sources.
 
     Parameters
@@ -153,29 +169,36 @@
 
     if (not validate_url(path)) and any(map(is_remote_source, norm)):
         raise ValueError("Cannot use a remote source with a local project.")
     return norm
 
 
 def get_extractor(
-    path: str, source: str, _id: Optional[str] = None
+    url: str,
+    source: str,
+    base_url: Optional[str] = None,
+    local_path: Optional[str] = None,
 ) -> Extractor:
     """Instantiate the correct extractor for a given source.
 
     Parameters
     -----------
-    path
+    URL
         Where the repository metadata is extracted from.
     source
         The source of the repository (git, gitlab, github, ...).
-    _id
-        The identifier to use for the repository. If not provided,
-        it will be determined automatically by the extractor
+    base_url
+        The base URL of the git remote.
+    local_path
+        If applicable, the path to the directory where the
+        repository is cloned.
     """
-    return SOURCES[source].extractor(path, _id=_id)
+    return SOURCES[source].extractor(
+        url, base_url=base_url, local_path=local_path
+    )
 
 
 def is_valid_source(source: str) -> bool:
     """Check if input is a valid source for gimie."""
     return source in SOURCES
 
 
@@ -198,14 +221,14 @@
     return False
 
 
 def get_git_provider(url: str) -> str:
     """Given a git repository URL, return the corresponding git provider.
     Local path or unsupported git providers will return "git"."""
     # NOTE: We just check if the provider name is in the URL.
-    # There may be a more robust way.
+    # We may want to use a more robust check.
     if validate_url(url):
         for name, prov in SOURCES.items():
             if prov.git and prov.remote and name in url:
                 return name
     # Fall back to local git if local path of unsupported provider
     return "git"
```

### Comparing `gimie-0.4.0/gimie/sources/__init__.py` & `gimie-0.5.0/gimie/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `gimie-0.4.0/gimie/sources/abstract.py` & `gimie-0.5.0/gimie/sources/abstract.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,28 +16,34 @@
 # limitations under the License.
 """Abstract classes for gimie objects."""
 from abc import ABC, abstractmethod
 from typing import Optional
 
 
 from rdflib import Graph
+from urllib.parse import urlparse
 
 
 class Extractor(ABC):
     """Extractor is an Abstract Base Class. It is only meant
     to define a standard interface for all extractors.
 
     All subclasses must implement extract() and to_graph() methods
     they are free to override the default serialize() and jsonld()
     """
 
-    def __init__(self, path: str, _id: Optional[str] = None):
-        self.path = path
-        if _id is not None:
-            self._id = _id
+    def __init__(
+        self,
+        url: str,
+        base_url: Optional[str] = None,
+        local_path: Optional[str] = None,
+    ):
+        self.url = url
+        self.base_url = base_url
+        self.local_path = local_path
 
     @abstractmethod
     def extract(self):
         """Extract metadata"""
         ...
 
     @abstractmethod
@@ -48,7 +54,27 @@
     def serialize(self, format: str = "ttl", **kwargs) -> str:
         """Serialize the RDF graph representing the instance."""
         return self.to_graph().serialize(format=format, **kwargs)  # type: ignore
 
     def jsonld(self) -> str:
         """Alias for jsonld serialization."""
         return self.serialize(format="json-ld")
+
+    @property
+    def _id(self) -> str:
+        """Unique identifier for the repository."""
+        return self.url
+
+    @property
+    def path(self) -> str:
+        """Path to the repository without the base URL."""
+        if self.base_url is None:
+            return urlparse(self.url).path.strip("/")
+        return self.url.removeprefix(self.base_url).strip("/")
+
+    @property
+    def base(self) -> str:
+        """Base URL of the remote."""
+        if self.base_url is None:
+            url = urlparse(self.url)
+            return f"{url.scheme}://{url.netloc}"
+        return self.base_url
```

### Comparing `gimie-0.4.0/gimie/sources/common/license.py` & `gimie-0.5.0/gimie/sources/common/license.py`

 * *Files identical despite different names*

### Comparing `gimie-0.4.0/gimie/sources/common/queries.py` & `gimie-0.5.0/gimie/sources/common/queries.py`

 * *Files identical despite different names*

### Comparing `gimie-0.4.0/gimie/sources/git.py` & `gimie-0.5.0/gimie/sources/git.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,37 +35,42 @@
 @dataclass
 class GitExtractor(Extractor):
     """
     This class is responsible for extracting metadata from a git repository.
 
     Parameters
     ----------
-    path: str
-        The path to the git repository.
+    url: str
+        The url of the git repository.
+    base_url: Optional[str]
+        The base url of the git remote.
+    local_path: Optional[str]
+        The local path where the cloned git repository is located.
 
     Attributes
     ----------
     uri: Optional[str]
         The URI to assign the repository in RDF.
     repository: Repository
         The repository we are extracting metadata from.
     """
 
-    path: str
-    _id: Optional[str] = None
+    url: str
+    base_url: Optional[str] = None
+    local_path: Optional[str] = None
+
     author: Optional[Person] = None
     contributors: Optional[List[Person]] = None
     date_created: Optional[datetime] = None
     date_modified: Optional[datetime] = None
 
     def extract(self):
-        self.repository = pydriller.Repository(self.path)
-        if self._id is None:
-            head_commit_hash = git.Repo(self.path).head.commit.hexsha[:7]
-            self._id = generate_uri(head_commit_hash)
+        if self.local_path is None:
+            raise ValueError("Local path must be provided for extraction.")
+        self.repository = pydriller.Repository(self.local_path)
         # Assuming author is the first person to commit
         self.author = self._get_creator()
         self.contributors = self._get_contributors()
         self.date_created = self._get_creation_date()
         self.date_modified = self._get_modification_date()
 
     def to_graph(self) -> Graph:
```

### Comparing `gimie-0.4.0/gimie/sources/github.py` & `gimie-0.5.0/gimie/sources/github.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime
+from dateutil.parser import isoparse
 import os
 import requests
 from typing import Any, Dict, List, Optional, Set, Union
 from urllib.parse import urlparse
 from dotenv import load_dotenv
 
 from calamus import fields
@@ -86,21 +87,26 @@
     # Drop empty users (e.g. dependabot)
     return [user for user in contributors["data"]["nodes"] if user]
 
 
 @dataclass
 class GithubExtractor(Extractor):
     """Extractor for GitHub repositories. Uses the GitHub GraphQL API to
-    extract metadata into linked data."""
+    extract metadata into linked data.
+    url: str
+        The url of the git repository.
+    base_url: Optional[str]
+        The base url of the git remote.
+    """
+
+    url: str
+    base_url: Optional[str] = None
+    local_path: Optional[str] = None
 
-    path: str
-    _id: Optional[str] = None
     token: Optional[str] = None
-
-    name: Optional[str] = None
     author: Optional[Union[Organization, Person]] = None
     contributors: Optional[List[Person]] = None
     prog_langs: Optional[List[str]] = None
     download_url: Optional[str] = None
     description: Optional[str] = None
     date_created: Optional[datetime] = None
     date_modified: Optional[datetime] = None
@@ -113,39 +119,36 @@
         jd = GithubExtractorSchema().dumps(self)
         g: Graph = Graph().parse(format="json-ld", data=str(jd))
         g.bind("schema", SDO)
         return g
 
     def extract(self):
         """Extract metadata from target GitHub repository."""
-        if self._id is None:
-            self._id = self.path
-        self.name = urlparse(self.path).path.strip("/")
-        data = self._fetch_repo_data(self.path)
+        data = self._fetch_repo_data()
         self.author = self._get_author(data["owner"])
-        self.contributors = self._fetch_contributors(self.path)
+        self.contributors = self._fetch_contributors()
         self.description = data["description"]
-        self.date_created = datetime.fromisoformat(data["createdAt"][:-1])
-        self.date_modified = datetime.fromisoformat(data["updatedAt"][:-1])
+        self.date_created = isoparse(data["createdAt"][:-1])
+        self.date_modified = isoparse(data["updatedAt"][:-1])
         # If license is available, convert to standard SPDX URL
         if data["licenseInfo"] is not None:
             self.license = get_spdx_url(data["licenseInfo"]["spdxId"])
         if data["primaryLanguage"] is not None:
             self.prog_langs = [data["primaryLanguage"]["name"]]
         self.keywords = self._get_keywords(*data["repositoryTopics"]["nodes"])
         last_release = data["latestRelease"]
         if last_release is not None:
             self.version = last_release["name"]
             self.download_url = (
-                f"{self.path}/archive/refs/tags/{self.version}.tar.gz"
+                f"{self.url}/archive/refs/tags/{self.version}.tar.gz"
             )
 
-    def _fetch_repo_data(self, url: str) -> Dict[str, Any]:
+    def _fetch_repo_data(self) -> Dict[str, Any]:
         """Fetch repository metadata from GraphQL endpoint."""
-        owner, name = urlparse(url).path.strip("/").split("/")
+        owner, name = self.path.split("/")
         data = {"owner": owner, "name": name}
         repo_query = """
         query repo($owner: String!, $name: String!) {
             repository(name: $name, owner: $owner) {
                 createdAt
                 description
                 latestRelease {
@@ -214,20 +217,20 @@
             GH_API, repo_query, data, self._set_auth()
         )
         if "errors" in response:
             raise ValueError(response["errors"])
 
         return response["data"]["repository"]
 
-    def _fetch_contributors(self, url: str) -> List[Person]:
+    def _fetch_contributors(self) -> List[Person]:
         """Queries the GitHub GraphQL API to extract contributors through the commit list.
         NOTE: This is a workaround for the lack of a contributors field in the GraphQL API."""
         headers = self._set_auth()
         contributors = []
-        resp = query_contributors(url, headers)
+        resp = query_contributors(self.url, headers)
         for user in resp:
             contributors.append(self._get_user(user))
         return list(contributors)
 
     def _set_auth(self) -> Any:
         """Set authentication headers for GitHub API requests."""
         try:
@@ -281,15 +284,15 @@
         )
 
 
 class GithubExtractorSchema(JsonLDSchema):
     """This defines the schema used for json-ld serialization."""
 
     _id = fields.Id()
-    name = fields.String(SDO.name)
+    path = fields.String(SDO.name)
     author = fields.Nested(SDO.author, [PersonSchema, OrganizationSchema])
     contributors = fields.Nested(SDO.contributor, PersonSchema, many=True)
     prog_langs = fields.List(SDO.programmingLanguage, fields.String)
     download_url = fields.Raw(SDO.downloadUrl)
     description = fields.String(SDO.description)
     date_created = fields.Date(SDO.dateCreated)
     date_modified = fields.Date(SDO.dateModified)
```

### Comparing `gimie-0.4.0/gimie/sources/gitlab.py` & `gimie-0.5.0/gimie/sources/gitlab.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from dataclasses import dataclass
 import os
 import requests
 from datetime import datetime
+from dateutil.parser import isoparse
 from typing import Any, Dict, List, Optional, Union
 from urllib.parse import urlparse
 
 from dotenv import load_dotenv
 from calamus import fields
 from calamus.schema import JsonLDSchema
 from rdflib import Graph
@@ -17,28 +18,33 @@
     OrganizationSchema,
     Person,
     PersonSchema,
 )
 from gimie.graph.namespaces import SDO
 from gimie.sources.common.queries import send_graphql_query, send_rest_query
 
-GL_API_REST = "https://gitlab.com/api/v4/"
-GL_API_GRAPHQL = "https://gitlab.com/api"
 load_dotenv()
 
 
 @dataclass
 class GitlabExtractor(Extractor):
     """Extractor for Gitlab repositories. Uses the Gitlab GraphQL API to
-    extract metadata into linked data."""
+    extract metadata into linked data.
+    url: str
+        The url of the git repository.
+    base_url: Optional[str]
+        The base url of the git remote.
+
+    """
+
+    url: str
+    base_url: Optional[str] = None
+    local_path: Optional[str] = None
 
-    path: str
-    _id: Optional[str] = None
     token: Optional[str] = None
-
     name: Optional[str] = None
     identifier: Optional[str] = None
     author: Optional[List[Union[Organization, Person]]] = None
     contributors: Optional[List[Person]] = None
     prog_langs: Optional[List[str]] = None
     description: Optional[str] = None
     date_created: Optional[datetime] = None
@@ -54,57 +60,52 @@
         jd = GitlabExtractorSchema().dumps(self)
         g: Graph = Graph().parse(format="json-ld", data=str(jd))
         g.bind("schema", SDO)
         return g
 
     def extract(self):
         """Extract metadata from target Gitlab repository."""
-        if self._id is None:
-            self._id = self.path
-        self.name = urlparse(self.path).path.strip("/")
 
         # fetch metadata
-        data = self._fetch_repo_data(self.name)
+        data = self._fetch_repo_data(self.path)
 
         # Each Gitlab project has a unique identifier (integer)
         self.identifier = urlparse(data["id"]).path.split("/")[2]
         # at the moment, Gimie fetches only the group directly related to the project
-        # the group name will take the form: parent/subgroup
+        # the group takes the form: parent/subgroup
         self.source_organization = self._safe_extract_group(data)
         self.description = data["description"]
         self.prog_langs = [lang["name"] for lang in data["languages"]]
-        self.date_created = datetime.fromisoformat(data["createdAt"][:-1])
-        self.date_modified = datetime.fromisoformat(
-            data["lastActivityAt"][:-1]
-        )
+        self.date_created = isoparse(data["createdAt"][:-1])
+        self.date_modified = isoparse(data["lastActivityAt"][:-1])
         self.keywords = data["topics"]
 
         # Get contributors as the project members that are not owners and those that have written merge requests
         # owners are either multiple individuals or a group, if not user is marked as owner
         self.author = self._safe_extract_author(data)
         # contributors are project members or merge request authors
         self.contributors = self._safe_extract_contributors(data)
 
         if data["releases"] and (len(data["releases"]["edges"]) > 0):
             # go into releases and take the name from the first node (most recent)
             self.version = data["releases"]["edges"][0]["node"]["name"]
-            self.download_url = f"{self.path}/-/archive/{self.version}/{self.name.split('/')[-1]}-{self.version}.tar.gz"
+            self.download_url = f"{self.url}/-/archive/{self.version}/{self.path.split('/')[-1]}-{self.version}.tar.gz"
 
         # for the license, we need to query the rest API
         # the code below does not work, returns - if you have permission- the GitLab specific licence
-        # resp = requests.get(url=f"{GL_API_rest}/license/{self.identifier}")
+        # resp = requests.get(url=f"{self.graphql_endpoint}/license/{self.identifier}")
         # if resp.status_code == 200:
         #     self.license = resp.json()
 
     def _safe_extract_group(
         self, repo: Dict[str, Any]
     ) -> Optional[Organization]:
         """Extract the group from a GraphQL repository node if it has one."""
-        if (self.name is not None) and (repo["group"] is not None):
-            repo["group"]["name"] = "/".join(self.name.split("/")[0:-1])
+        if (self.path is not None) and (repo["group"] is not None):
+            repo["group"]["name"] = "/".join(self.path.split("/")[0:-1])
             return self._get_organization(repo["group"])
         return None
 
     def _safe_extract_author(
         self, repo: Dict[str, Any]
     ) -> List[Union[Person, Organization]]:
         """Extract the author from a GraphQL repository node.
@@ -121,15 +122,15 @@
             ]
 
         if repo["group"] is not None:
             return [self._get_author(repo["group"])]
 
         # If the author is absent from the GraphQL response (permission bug),
         # fallback to the REST API
-        return [self._user_from_rest(self.name.split("/")[0])]
+        return [self._user_from_rest(self.path.split("/")[0])]
 
     def _safe_extract_contributors(
         self, repo: dict[str, Any]
     ) -> list[Person] | None:
         members = [
             user["node"]["user"]
             for user in repo["projectMembers"]["edges"]
@@ -204,30 +205,30 @@
                     }
                     }
                 }
         }
         }
         """
         response = send_graphql_query(
-            GL_API_GRAPHQL, project_query, data, self._set_auth()
+            self.graphql_endpoint, project_query, data, self._set_auth()
         )
         if "errors" in response:
             raise ValueError(response["errors"])
 
         return response["data"]["project"]
 
     def _set_auth(self) -> Any:
         """Set authentication headers for Gitlab API requests."""
         try:
             if not self.token:
                 self.token = os.environ.get("GITLAB_TOKEN")
                 assert self.token
             headers = {"Authorization": f"token {self.token}"}
 
-            login = requests.get(f"{GL_API_REST}/user", headers=headers)
+            login = requests.get(f"{self.rest_endpoint}/user", headers=headers)
             assert login.json().get("login")
         except AssertionError:
             return {}
         else:
             return headers
 
     def _get_author(self, node: Dict[str, Any]) -> Union[Organization, Person]:
@@ -256,33 +257,41 @@
             email=node.get("publicEmail"),
         )
 
     def _user_from_rest(self, username: str) -> Person:
         """Given a username, use the REST API to retrieve the Person object."""
 
         author = send_rest_query(
-            GL_API_REST,
+            self.rest_endpoint,
             f"/users?username={username}",
             self._set_auth(),
         )
         if isinstance(author, list):
             author = author[0]
 
         return Person(
             _id=author["web_url"],
             identifier=author["username"],
             name=author.get("name"),
         )
 
+    @property
+    def rest_endpoint(self) -> str:
+        return f"{self.base}/api/v4/"
+
+    @property
+    def graphql_endpoint(self) -> str:
+        return f"{self.base}/api"
+
 
 class GitlabExtractorSchema(JsonLDSchema):
     """This defines the schema used for json-ld serialization."""
 
     _id = fields.Id()
-    name = fields.String(SDO.name)
+    path = fields.String(SDO.name)
     identifier = fields.String(SDO.identifier)
     source_organization = fields.Nested(SDO.isPartOf, OrganizationSchema)
     author = fields.Nested(
         SDO.author, [PersonSchema, OrganizationSchema], many=True
     )
     contributors = fields.Nested(SDO.contributor, PersonSchema, many=True)
     prog_langs = fields.List(SDO.programmingLanguage, fields.String)
```

### Comparing `gimie-0.4.0/gimie/utils.py` & `gimie-0.5.0/gimie/utils.py`

 * *Files identical despite different names*

### Comparing `gimie-0.4.0/pyproject.toml` & `gimie-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Package description
 
 [tool.poetry]
 name = "gimie"
-version = "0.4.0"
+version = "0.5.0"
 description = "Extract structured metadata from git repositories."
 authors = ["Swiss Data Science Center <contact@datascience.ch>"]
 license = "Apache-2.0"
 homepage = "https://github.com/SDSC-ORD/gimie"
 keywords = ["metadata", "git", "extraction", "linked-data"]
 readme = "README.md"
 classifiers = [
@@ -29,18 +29,21 @@
 # scancode-toolkit = "^31.2.4"
 typer = "^0.7.0"
 calamus = "^0.4.2"
 requests = "^2.28.2"
 python-dotenv = "^0.21.1"
 pre-commit = "^3.0.0"
 importlib = "^1.0.4"
+python-dateutil = "^2.8.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 black = "^22.10.0"
+pytest-cov = "^4.1.0"
+coveralls = "^3.3.1"
 
 
 [tool.poetry.group.doc.dependencies]
 sphinx = "<7.0.0"
 sphinx-click = "^4.4.0"
 sphinxawesome-theme = "^4.1.0"
 sphinx-copybutton = "^0.5.2"
@@ -58,45 +61,44 @@
 # Tooling configuration
 
 [tool.black]
 line-length = 79
 target-version = ["py38", "py39"]
 
 [tool.pytest.ini_options]
-addopts = "--doctest-modules"
+addopts = ["--doctest-modules", "--cov"]
 testpaths = ["gimie", "tests"]
 
 [tool.pyright]
 reportMissingTypeStubs = false
 reportUntypedBaseClass = false
 
 [tool.git-cliff.changelog]
 header = "Notable changes introduced in gimie releases are documented in this file\n\n"
 body = """
-# Changelog
 
 {% if version %}\
     ## [{{ version | trim_start_matches(pat="v") }}] - {{ timestamp | date(format="%Y-%m-%d") }}
 {% else %}\
     ## [unreleased]
 {% endif %}\
 {% for group, commits in commits | group_by(attribute="group") %}
     ### {{ group | upper_first }}
     {% for commit in commits
     | filter(attribute="scope")
     | sort(attribute="scope") %}
-        - *({{commit.scope}})* {{ commit.message | upper_first }}
+        - *({{commit.scope}})* {{ commit.message }}
         {%- if commit.breaking %}
         {% raw %}  {% endraw %}- **BREAKING**: {{commit.breaking_description}}
         {%- endif -%}
     {%- endfor -%}
     {%- for commit in commits %}
         {%- if commit.scope -%}
         {% else -%}
-            - {{ commit.message | upper_first }}
+            - {{ commit.message }}
             {% if commit.breaking -%}
             {% raw %}  {% endraw %}- **BREAKING**: {{commit.breaking_description}}
             {% endif -%}
         {% endif -%}
     {% endfor -%}
     {% raw %}\n{% endraw %}\
 {% endfor %}\n
```

### Comparing `gimie-0.4.0/PKG-INFO` & `gimie-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimie
-Version: 0.4.0
+Version: 0.5.0
 Summary: Extract structured metadata from git repositories.
 Home-page: https://github.com/SDSC-ORD/gimie
 License: Apache-2.0
 Keywords: metadata,git,extraction,linked-data
 Author: Swiss Data Science Center
 Author-email: contact@datascience.ch
 Requires-Python: >=3.8,<4.0
@@ -19,30 +19,35 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyDriller (>=2.3,<3.0)
 Requires-Dist: calamus (>=0.4.2,<0.5.0)
 Requires-Dist: importlib (>=1.0.4,<2.0.0)
 Requires-Dist: pre-commit (>=3.0.0,<4.0.0)
 Requires-Dist: pyshacl (>=0.20.0,<0.21.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 [![gimie](docs/logo.svg)](https://github.com/SDSC-ORD/gimie)
 
-[![PyPI version](https://badge.fury.io/py/gimie.svg)](https://badge.fury.io/py/gimie) [![Python Poetry Test](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml/badge.svg)](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml) [![docs](https://github.com/SDSC-ORD/gimie/actions/workflows/sphinx-docs.yml/badge.svg)](https://sdsc-ord.github.io/gimie)
+[![PyPI version](https://badge.fury.io/py/gimie.svg)](https://badge.fury.io/py/gimie) [![Python Poetry Test](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml/badge.svg)](https://github.com/SDSC-ORD/gimie/actions/workflows/poetry-pytest.yml) [![docs](https://github.com/SDSC-ORD/gimie/actions/workflows/sphinx-docs.yml/badge.svg)](https://sdsc-ord.github.io/gimie) [![Coverage Status](https://coveralls.io/repos/github/SDSC-ORD/gimie/badge.svg?branch=main)](https://coveralls.io/github/SDSC-ORD/gimie?branch=main)
 
 Gimie (GIt Meta Information Extractor) is a python library and command line tool to extract structured metadata from git repositories.
 
 
 ## Context
 Scientific code repositories contain valuable metadata which can be used to enrich existing catalogues, platforms or databases. This tool aims to easily extract structured metadata from a generic git repositories. It can extract extract metadata from the Git provider (GitHub or GitLab) or from the git index itself.
 
-## Installation
+----------------------------------------------------------------------
+
+Using Gimie: easy peasy, it's a 3 step process. 
+
+## STEP 1: Installation
 
 To install the stable version on PyPI:
 
 ```shell
 pip install gimie
 ```
 
@@ -57,79 +62,50 @@
 ```shell
 docker pull ghcr.io/sdsc-ord/gimie:latest
 
 # The access token can be provided as an environment variable
 docker run -e ACCESS_TOKEN=$ACCESS_TOKEN ghcr.io/sdsc-ord/gimie:latest gimie data <repo>
 ```
 
+## STEP 2 : Set your credentials
 
-### For development:
-
-activate a conda or virtual environment with Python 3.8 or higher
-
-```shell
-git clone https://github.com/SDSC-ORD/gimie && cd gimie
-make install
-```
-
-run tests:
-
-```shell
-make test
-```
-
-run checks:
-
-```shell
-make check
-```
+In order to access the github api, you need to provide a github token with the `read:org` scope. 
 
-build documentation:
+### A. Create access tokens
 
-```shell
-make doc
-```
+New to access tokens? Or don't know how to get your Github / Gitlab token ? 
 
-## Usage
+Have no fear, see
+[here for Github tokens](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) and [here for Gitlab tokens](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html).
+(Note: tokens are as precious as passwords! Treat them as such.)
 
-### Set your github credentials
+### B. Set your access tokens via the Terminal
 
-In order to avoid rate limits with the github api, you need to provide your github
-username and a github token with the `read:org` scope: see
-[here ](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
-on how to generate a github token.
+Gimie will use your access tokens to gather information for you. If you want info about a Github repo, Gimie needs your Github token; if you want info about a Gitlab Project then Gimie needs your Gitlab token.
 
-There are 2 options for setting up your github token in your local environment:
-
-**Option 1:**
-
-```
-cp .env.dist .env
+Add your tokens one by one in your terminal:
+your Github token:
+```bash
+export GITHUB_TOKEN=
 ```
-
-And then edit the `.env` file and put your github token in.
-
-**Option 2:**
-
-Add your github token in your terminal:
-
+and/or your Gitlab token:
 ```bash
-export ACCESS_TOKEN=
+export GITLAB_TOKEN=
 ```
 
-After the github token has been added, you can run the command without running into an github api limit.
-Otherwise you can still run the command, but might hit that limit after running the command several times.
+## STEP 3: GIMIE info ! Run Gimie
 
-### Run the command
+### As a command line tool
 
-As a command line tool:
 ```shell
 gimie data https://github.com/numpy/numpy
 ```
-As a python library:
+(want a Gitlab project instead? Just replace the URL in the command line) 
+
+### As a python library
 
 ```python
 from gimie.project import Project
 proj = Project("https://github.com/numpy/numpy)
 
 # To retrieve the rdflib.Graph object
 g = proj.to_graph()
@@ -150,28 +126,59 @@
 # To retrieve the serialized graph
 gh.serialize(format='ttl')
 ```
 [For a GitLab project, replace `gimie.sources.github` by `gimie.sources.gitlab`, `GithubExtractor` by `GitlabExtractor`, as well as the URL to the GitLab project.]
 
 ## Outputs
 
-The default output is JSON-ld, a JSON serialization of the [RDF](https://en.wikipedia.org/wiki/Resource_Description_Framework) data model. We follow the schema recommended by [codemeta](https://codemeta.github.io/).
-Supported formats are json-ld, turtle and n-triples.
+The default output is [Turtle](https://www.w3.org/TR/turtle/), a textual syntax for [RDF](https://en.wikipedia.org/wiki/Resource_Description_Framework) data model. We follow the schema recommended by [codemeta](https://codemeta.github.io/).
+Supported formats are turtle, json-ld and n-triples (by specifying the `--format` argument in your call i.e. `gimie data https://github.com/numpy/numpy --format 'ttl'`).
 
-### Limitations
+With no specifications, Gimie will print results in the terminal. Want to save Gimie output to a file? Add your file path to the end : `gimie data https://github.com/numpy/numpy > path_to_output/gimie_output.ttl`
 
-* Currently, gimie will only the first 100 contributors of a repository (in arbitrary order), and for each users, at most 100 affiliations.
-* If a Github repository is owned by an organization, all "mentionable users" are reported as contributors. This will include all members of the organization in addition to contributors.
+----------------------------------------------------------------------
 
 ## Contributing
 
 All contributions are welcome. New functions and classes should have associated tests and docstrings following the [numpy style guide](https://numpydoc.readthedocs.io/en/latest/format.html).
 
 The code formatting standard we use is [black](https://github.com/psf/black), with `--line-length=79` to follow [PEP8](https://peps.python.org/pep-0008/) recommendations. We use [pytest](https://docs.pytest.org/en/7.2.x/) as our testing framework. This project uses [pyproject.toml](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/) to define package information, requirements and tooling configuration.
 
+### For development:
+
+activate a conda or virtual environment with Python 3.8 or higher
+
+```shell
+git clone https://github.com/SDSC-ORD/gimie && cd gimie
+make install
+```
+
+run tests:
+
+```shell
+make test
+```
+
+run checks:
+
+```shell
+make check
+```
+for an easier use Github/Gitlab APIs, place your access tokens in the `.env` file: (and don't worry, the `.gitignore` will ignore them when you push to GitHub) 
+
+```
+cp .env.dist .env
+```
+
+build documentation:
+
+```shell
+make doc
+```
+
 ## Releases and Publishing on Pypi
 
 Releases are done via github release
 
 - a release will trigger a github workflow to publish the package on Pypi
 - Make sure to update to a new version in `pyproject.toml` before making the release
 - It is possible to test the publishing on Pypi.test by running a manual workflow: go to github actions and run the Workflow: 'Publish on Pypi Test'
```

