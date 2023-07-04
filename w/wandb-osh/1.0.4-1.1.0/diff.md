# Comparing `tmp/wandb_osh-1.0.4.tar.gz` & `tmp/wandb_osh-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wandb_osh-1.0.4.tar", last modified: Thu Jan 19 01:07:55 2023, max compression
+gzip compressed data, was "wandb_osh-1.1.0.tar", last modified: Tue Jul  4 18:17:25 2023, max compression
```

## Comparing `wandb_osh-1.0.4.tar` & `wandb_osh-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 01:07:55.723717 wandb_osh-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-01-19 01:07:55.723717 wandb_osh-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-19 01:07:55.727717 wandb_osh-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 01:07:55.719717 wandb_osh-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 01:07:55.723717 wandb_osh-1.0.4/src/wandb_osh/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/ray_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/syncer.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/test_ray_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/test_syncer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 01:07:55.723717 wandb_osh-1.0.4/src/wandb_osh/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/util/hash_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/util/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-01-19 01:07:42.000000 wandb_osh-1.0.4/src/wandb_osh/util/test_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 01:07:55.723717 wandb_osh-1.0.4/src/wandb_osh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-01-19 01:07:55.000000 wandb_osh-1.0.4/src/wandb_osh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-01-19 01:07:55.000000 wandb_osh-1.0.4/src/wandb_osh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 01:07:55.000000 wandb_osh-1.0.4/src/wandb_osh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-19 01:07:55.000000 wandb_osh-1.0.4/src/wandb_osh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 01:07:55.000000 wandb_osh-1.0.4/src/wandb_osh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-19 01:07:55.000000 wandb_osh-1.0.4/src/wandb_osh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-19 01:07:55.000000 wandb_osh-1.0.4/src/wandb_osh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-04 18:17:25.518096 wandb_osh-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/src/wandb_osh/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/lightning_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/ray_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/syncer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/src/wandb_osh/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/util/hash_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/src/wandb_osh/util/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/src/wandb_osh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 18:17:25.000000 wandb_osh-1.1.0/src/wandb_osh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:17:25.514096 wandb_osh-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/tests/test_lightning_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/tests/test_ray_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-04 18:17:17.000000 wandb_osh-1.1.0/tests/test_syncer.py
```

### Comparing `wandb_osh-1.0.4/LICENSE.txt` & `wandb_osh-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.0.4/PKG-INFO` & `wandb_osh-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,32 @@
-Metadata-Version: 2.1
-Name: wandb_osh
-Version: 1.0.4
-Summary: Trigger wandb offline syncs from a compute node without internet
-Home-page: https://github.com/klieret/wandb-offline-sync-hook
-Author: Kilian Lieret
-Author-email: kilian.lieret@posteo.de
-Maintainer: Kilian Lieret
-Maintainer-email: kilian.lieret@posteo.de
-License: MIT
-Project-URL: Bug Tracker, https://github.com/klieret/wandb-offline-sync-hook/issues
-Project-URL: Documentation, https://wandb_osh.readthedocs.io/
-Project-URL: Source Code, https://github.com/klieret/wandb-offline-sync-hook
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: ray
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 <div align="center">
 <h1>Wandb Offline Sync Hook</h1>
 <em>A convenient way to trigger synchronizations to wandb if your compute nodes don't have internet!</em>
 <p></p>
 
 [![Documentation Status](https://readthedocs.org/projects/wandb-offline-sync-hook/badge/?version=latest)](https://wandb-offline-sync-hook.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/wandb-osh.svg)](https://pypi.org/project/wandb-osh)
 [![Python 3.7‒3.11](https://img.shields.io/badge/python-3.7%E2%80%923.11-blue)](https://www.python.org)
 [![PR welcome](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/klieret/wandb-offline-sync-hook/main.svg)](https://results.pre-commit.ci/latest/github/klieret/wandb-offline-sync-hook/main)
 [![.github/workflows/test.yaml](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/test.yaml/badge.svg)](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/test.yaml)
 [![link checker](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/check-links.yaml/badge.svg)](https://github.com/klieret/wandb-offline-sync-hook/actions)
-[![codecov](https://codecov.io/github/klieret/wandb-offline-sync-hook/branch/main/graph/badge.svg?token=6MQZ4LODE5)](https://codecov.io/github/klieret/wandb-offline-sync-hook)
+[![codecov](https://codecov.io/github/klieret/wandb-offline-sync-hook/branch/main/graph/badge.svg?token=6MQZ4LODE5)](https://app.codecov.io/github/klieret/wandb-offline-sync-hook)
 [![gitmoji](https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67.svg)](https://gitmoji.dev)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
 </div>
 
 ## 🤔 What is this?
 
 - ✅ You use [`wandb`/Weights & Biases](https://wandb.ai/) to record your machine learning trials?
 - ✅ Your ML experiments run on compute nodes without internet access (for example, using a batch system)?
 - ✅ Your compute nodes and your head/login node (with internet) have access to a shared file system?
 
-Then this package can be useful.
+Then this package might be useful. For alternatives, see [below](https://github.com/klieret/wandb-offline-sync-hook#what-alternatives-are-there).
 
 <div align="center">
 
 ![](https://user-images.githubusercontent.com/13602468/200086359-507b8653-e999-4cb3-ac93-ba1d175d2016.png)
 
 </div>
 
@@ -75,14 +48,19 @@
 1. You add a hook that is called every time an epoch concludes (that is, when we want to trigger a sync).
 2. You start the `wandb-osh` script in your head node with internet access. This script will now trigger `wandb sync` upon request from one of the compute nodes.
 
 ### How is this implemented?
 
 Very simple: Every time an epoch concludes, the hook gets called and creates a file in a _communication directory_ (`~/.wandb_osh_communication` by default). `wandb-osh` scans the communication directory and reads synchronization instructions from such files.
 
+### What alternatives are there?
+
+With [ray tune][ray-tune], you can use your ray head node as the place to synchronize from (rather than deploying it via the batch system as well, as the [current docs][ray-tune-slurm-docs] suggest). See the note below or my [demo repository][ray-tune-slurm-test].
+Similar strategies might be possible for `wandb` as well (let me know!).
+
 ## 📦 Installation
 
 ```
 pip3 install wandb-osh
 ```
 
 If you want to use this package with `ray`, use
@@ -122,21 +100,51 @@
     loss.backward()
     optimizer.step()
     if batch_idx % args.log_interval == 0:
         wandb.log({"loss": loss})
         trigger_sync()  # <-- New!
 ```
 
+#### With pytorch lightning
+
+```python
+from wandb_osh.lightning_hooks import TriggerWandbSyncLightningCallback  # <-- New!
+from pytorch_lightning.loggers import WandbLogger
+from pytorch_lightning import Trainer
+
+logger = WandbLogger(
+    project="project",
+    group="group",
+    offline=True,
+)
+
+model = MyLightningModule()
+trainer = Trainer(
+    logger=logger,
+    callbacks=[TriggerWandbSyncLightningCallback()]  # <-- New!
+)
+trainer.fit(model, train_dataloader, val_dataloader)
+```
+
 #### With ray tune
 
-You probably already use the `WandbLoggerCallback` callback. We simply add a second callback for `wandb-osh` (it only takes one new line!):
+> **Note**
+> With ray tune, you might not need this package! While the approach suggested in the
+> [ray tune SLURM docs][ray-tune-slurm-docs] deploys the ray head on a worker node as well (so it doesn't
+> have internet), this actually isn't needed. Instead, you can run the ray head and the
+> tuning script on the head node and only submit batch jobs for your workers.
+> In this way, `wandb` will be called from the head node and internet access is no
+> problem there.
+> For more information on this approach, take a look at my [demo repository][ray-tune-slurm-test].
+
+You probably already use the `WandbLoggerCallback` callback. We simply add a second callback for `wandb-osh` (it only takes two new lines!):
 
 ```python
 import os
-from wandb_osh.ray_hooks import TriggerWandbSyncRayHook
+from wandb_osh.ray_hooks import TriggerWandbSyncRayHook  # <-- New!
 
 
 os.environ["WANDB_MODE"] = "offline"
 
 callbacks = [
     WandbLoggerCallback(...),  # <-- ray tune documentation tells you about this
     TriggerWandbSyncRayHook(),  # <-- New!
@@ -230,7 +238,10 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 <!--  -->
 <!-- This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome! -->
 
 [github-issues]: https://github.com/klieret/wandb-offline-sync-hook/issues
 [pulls]: https://github.com/klieret/wandb-offline-sync-hook/pulls
+[ray-tune-slurm-docs]: https://docs.ray.io/en/latest/cluster/vms/user-guides/community/slurm.html
+[ray-tune-slurm-test]: https://github.com/klieret/ray-tune-slurm-test/
+[ray-tune]: https://docs.ray.io/en/latest/tune/index.html
```

### Comparing `wandb_osh-1.0.4/README.md` & `wandb_osh-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,59 @@
+Metadata-Version: 2.1
+Name: wandb_osh
+Version: 1.1.0
+Summary: Trigger wandb offline syncs from a compute node without internet
+Home-page: https://github.com/klieret/wandb-offline-sync-hook
+Author: Kilian Lieret
+Author-email: kilian.lieret@posteo.de
+Maintainer: Kilian Lieret
+Maintainer-email: kilian.lieret@posteo.de
+License: MIT
+Project-URL: Bug Tracker, https://github.com/klieret/wandb-offline-sync-hook/issues
+Project-URL: Documentation, https://wandb_osh.readthedocs.io/
+Project-URL: Source Code, https://github.com/klieret/wandb-offline-sync-hook
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: lightning
+Provides-Extra: ray
+Provides-Extra: testing
+License-File: LICENSE.txt
+
 <div align="center">
 <h1>Wandb Offline Sync Hook</h1>
 <em>A convenient way to trigger synchronizations to wandb if your compute nodes don't have internet!</em>
 <p></p>
 
 [![Documentation Status](https://readthedocs.org/projects/wandb-offline-sync-hook/badge/?version=latest)](https://wandb-offline-sync-hook.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/wandb-osh.svg)](https://pypi.org/project/wandb-osh)
 [![Python 3.7‒3.11](https://img.shields.io/badge/python-3.7%E2%80%923.11-blue)](https://www.python.org)
 [![PR welcome](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/klieret/wandb-offline-sync-hook/main.svg)](https://results.pre-commit.ci/latest/github/klieret/wandb-offline-sync-hook/main)
 [![.github/workflows/test.yaml](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/test.yaml/badge.svg)](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/test.yaml)
 [![link checker](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/check-links.yaml/badge.svg)](https://github.com/klieret/wandb-offline-sync-hook/actions)
-[![codecov](https://codecov.io/github/klieret/wandb-offline-sync-hook/branch/main/graph/badge.svg?token=6MQZ4LODE5)](https://codecov.io/github/klieret/wandb-offline-sync-hook)
+[![codecov](https://codecov.io/github/klieret/wandb-offline-sync-hook/branch/main/graph/badge.svg?token=6MQZ4LODE5)](https://app.codecov.io/github/klieret/wandb-offline-sync-hook)
 [![gitmoji](https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67.svg)](https://gitmoji.dev)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
 </div>
 
 ## 🤔 What is this?
 
 - ✅ You use [`wandb`/Weights & Biases](https://wandb.ai/) to record your machine learning trials?
 - ✅ Your ML experiments run on compute nodes without internet access (for example, using a batch system)?
 - ✅ Your compute nodes and your head/login node (with internet) have access to a shared file system?
 
-Then this package can be useful.
+Then this package might be useful. For alternatives, see [below](https://github.com/klieret/wandb-offline-sync-hook#what-alternatives-are-there).
 
 <div align="center">
 
 ![](https://user-images.githubusercontent.com/13602468/200086359-507b8653-e999-4cb3-ac93-ba1d175d2016.png)
 
 </div>
 
@@ -48,14 +75,19 @@
 1. You add a hook that is called every time an epoch concludes (that is, when we want to trigger a sync).
 2. You start the `wandb-osh` script in your head node with internet access. This script will now trigger `wandb sync` upon request from one of the compute nodes.
 
 ### How is this implemented?
 
 Very simple: Every time an epoch concludes, the hook gets called and creates a file in a _communication directory_ (`~/.wandb_osh_communication` by default). `wandb-osh` scans the communication directory and reads synchronization instructions from such files.
 
+### What alternatives are there?
+
+With [ray tune][ray-tune], you can use your ray head node as the place to synchronize from (rather than deploying it via the batch system as well, as the [current docs][ray-tune-slurm-docs] suggest). See the note below or my [demo repository][ray-tune-slurm-test].
+Similar strategies might be possible for `wandb` as well (let me know!).
+
 ## 📦 Installation
 
 ```
 pip3 install wandb-osh
 ```
 
 If you want to use this package with `ray`, use
@@ -95,21 +127,51 @@
     loss.backward()
     optimizer.step()
     if batch_idx % args.log_interval == 0:
         wandb.log({"loss": loss})
         trigger_sync()  # <-- New!
 ```
 
+#### With pytorch lightning
+
+```python
+from wandb_osh.lightning_hooks import TriggerWandbSyncLightningCallback  # <-- New!
+from pytorch_lightning.loggers import WandbLogger
+from pytorch_lightning import Trainer
+
+logger = WandbLogger(
+    project="project",
+    group="group",
+    offline=True,
+)
+
+model = MyLightningModule()
+trainer = Trainer(
+    logger=logger,
+    callbacks=[TriggerWandbSyncLightningCallback()]  # <-- New!
+)
+trainer.fit(model, train_dataloader, val_dataloader)
+```
+
 #### With ray tune
 
-You probably already use the `WandbLoggerCallback` callback. We simply add a second callback for `wandb-osh` (it only takes one new line!):
+> **Note**
+> With ray tune, you might not need this package! While the approach suggested in the
+> [ray tune SLURM docs][ray-tune-slurm-docs] deploys the ray head on a worker node as well (so it doesn't
+> have internet), this actually isn't needed. Instead, you can run the ray head and the
+> tuning script on the head node and only submit batch jobs for your workers.
+> In this way, `wandb` will be called from the head node and internet access is no
+> problem there.
+> For more information on this approach, take a look at my [demo repository][ray-tune-slurm-test].
+
+You probably already use the `WandbLoggerCallback` callback. We simply add a second callback for `wandb-osh` (it only takes two new lines!):
 
 ```python
 import os
-from wandb_osh.ray_hooks import TriggerWandbSyncRayHook
+from wandb_osh.ray_hooks import TriggerWandbSyncRayHook  # <-- New!
 
 
 os.environ["WANDB_MODE"] = "offline"
 
 callbacks = [
     WandbLoggerCallback(...),  # <-- ray tune documentation tells you about this
     TriggerWandbSyncRayHook(),  # <-- New!
@@ -203,7 +265,10 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 <!--  -->
 <!-- This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome! -->
 
 [github-issues]: https://github.com/klieret/wandb-offline-sync-hook/issues
 [pulls]: https://github.com/klieret/wandb-offline-sync-hook/pulls
+[ray-tune-slurm-docs]: https://docs.ray.io/en/latest/cluster/vms/user-guides/community/slurm.html
+[ray-tune-slurm-test]: https://github.com/klieret/ray-tune-slurm-test/
+[ray-tune]: https://docs.ray.io/en/latest/tune/index.html
```

### Comparing `wandb_osh-1.0.4/setup.cfg` & `wandb_osh-1.1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 [metadata]
 name = wandb_osh
-version = 1.0.4
+version = 1.1.0
 description = Trigger wandb offline syncs from a compute node without internet
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/klieret/wandb-offline-sync-hook
 author = Kilian Lieret
 author_email = kilian.lieret@posteo.de
 maintainer = Kilian Lieret
 maintainer_email = kilian.lieret@posteo.de
 license = MIT
-license_file = LICENSE.txt
+license_files = LICENSE.txt
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 project_urls = 
 	Bug Tracker =   https://github.com/klieret/wandb-offline-sync-hook/issues
 	Documentation = https://wandb_osh.readthedocs.io/
 	Source Code =   https://github.com/klieret/wandb-offline-sync-hook
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options]
 packages = find:
 install_requires = 
 	colorlog
 	wandb
 	importlib-metadata>=0.12;python_version<"3.8"
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	wandb-osh = wandb_osh.cli:main
 
 [options.extras_require]
+lightning = 
+	pytorch-lightning
 ray = 
 	ray[tune]
 testing = 
 	pytest
 	pytest-coverage
 
 [egg_info]
```

### Comparing `wandb_osh-1.0.4/setup.py` & `wandb_osh-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.0.4/src/wandb_osh/cli.py` & `wandb_osh-1.1.0/src/wandb_osh/cli.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.0.4/src/wandb_osh/hooks.py` & `wandb_osh-1.1.0/src/wandb_osh/hooks.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.0.4/src/wandb_osh/ray_hooks.py` & `wandb_osh-1.1.0/src/wandb_osh/ray_hooks.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.0.4/src/wandb_osh/syncer.py` & `wandb_osh-1.1.0/src/wandb_osh/syncer.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.0.4/src/wandb_osh/test_cli.py` & `wandb_osh-1.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.0.4/src/wandb_osh/test_ray_hooks.py` & `wandb_osh-1.1.0/tests/test_ray_hooks.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.0.4/src/wandb_osh/test_syncer.py` & `wandb_osh-1.1.0/tests/test_syncer.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.0.4/src/wandb_osh/util/log.py` & `wandb_osh-1.1.0/src/wandb_osh/util/log.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,15 +25,17 @@
         "DEBUG": "cyan",
         "INFO": "green",
         "WARNING": "yellow",
         "ERROR": "red",
         "CRITICAL": "red",
     }
     formatter = colorlog.ColoredFormatter(
-        "%(log_color)s%(levelname)s: %(message)s", log_colors=log_colors
+        "%(log_color)s%(asctime)s %(levelname)s: %(message)s",
+        log_colors=log_colors,
+        datefmt="%H:%M:%S",
     )
     sh.setFormatter(formatter)
     # Controlled by overall logger level
     sh.setLevel(logging.DEBUG)
 
     _log.addHandler(sh)
```

### Comparing `wandb_osh-1.0.4/src/wandb_osh.egg-info/PKG-INFO` & `wandb_osh-1.1.0/src/wandb_osh.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: wandb-osh
-Version: 1.0.4
+Version: 1.1.0
 Summary: Trigger wandb offline syncs from a compute node without internet
 Home-page: https://github.com/klieret/wandb-offline-sync-hook
 Author: Kilian Lieret
 Author-email: kilian.lieret@posteo.de
 Maintainer: Kilian Lieret
 Maintainer-email: kilian.lieret@posteo.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/klieret/wandb-offline-sync-hook/issues
 Project-URL: Documentation, https://wandb_osh.readthedocs.io/
 Project-URL: Source Code, https://github.com/klieret/wandb-offline-sync-hook
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: lightning
 Provides-Extra: ray
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 <div align="center">
 <h1>Wandb Offline Sync Hook</h1>
 <em>A convenient way to trigger synchronizations to wandb if your compute nodes don't have internet!</em>
@@ -33,27 +33,27 @@
 [![Documentation Status](https://readthedocs.org/projects/wandb-offline-sync-hook/badge/?version=latest)](https://wandb-offline-sync-hook.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/wandb-osh.svg)](https://pypi.org/project/wandb-osh)
 [![Python 3.7‒3.11](https://img.shields.io/badge/python-3.7%E2%80%923.11-blue)](https://www.python.org)
 [![PR welcome](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/klieret/wandb-offline-sync-hook/main.svg)](https://results.pre-commit.ci/latest/github/klieret/wandb-offline-sync-hook/main)
 [![.github/workflows/test.yaml](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/test.yaml/badge.svg)](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/test.yaml)
 [![link checker](https://github.com/klieret/wandb-offline-sync-hook/actions/workflows/check-links.yaml/badge.svg)](https://github.com/klieret/wandb-offline-sync-hook/actions)
-[![codecov](https://codecov.io/github/klieret/wandb-offline-sync-hook/branch/main/graph/badge.svg?token=6MQZ4LODE5)](https://codecov.io/github/klieret/wandb-offline-sync-hook)
+[![codecov](https://codecov.io/github/klieret/wandb-offline-sync-hook/branch/main/graph/badge.svg?token=6MQZ4LODE5)](https://app.codecov.io/github/klieret/wandb-offline-sync-hook)
 [![gitmoji](https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67.svg)](https://gitmoji.dev)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
 </div>
 
 ## 🤔 What is this?
 
 - ✅ You use [`wandb`/Weights & Biases](https://wandb.ai/) to record your machine learning trials?
 - ✅ Your ML experiments run on compute nodes without internet access (for example, using a batch system)?
 - ✅ Your compute nodes and your head/login node (with internet) have access to a shared file system?
 
-Then this package can be useful.
+Then this package might be useful. For alternatives, see [below](https://github.com/klieret/wandb-offline-sync-hook#what-alternatives-are-there).
 
 <div align="center">
 
 ![](https://user-images.githubusercontent.com/13602468/200086359-507b8653-e999-4cb3-ac93-ba1d175d2016.png)
 
 </div>
 
@@ -75,14 +75,19 @@
 1. You add a hook that is called every time an epoch concludes (that is, when we want to trigger a sync).
 2. You start the `wandb-osh` script in your head node with internet access. This script will now trigger `wandb sync` upon request from one of the compute nodes.
 
 ### How is this implemented?
 
 Very simple: Every time an epoch concludes, the hook gets called and creates a file in a _communication directory_ (`~/.wandb_osh_communication` by default). `wandb-osh` scans the communication directory and reads synchronization instructions from such files.
 
+### What alternatives are there?
+
+With [ray tune][ray-tune], you can use your ray head node as the place to synchronize from (rather than deploying it via the batch system as well, as the [current docs][ray-tune-slurm-docs] suggest). See the note below or my [demo repository][ray-tune-slurm-test].
+Similar strategies might be possible for `wandb` as well (let me know!).
+
 ## 📦 Installation
 
 ```
 pip3 install wandb-osh
 ```
 
 If you want to use this package with `ray`, use
@@ -122,21 +127,51 @@
     loss.backward()
     optimizer.step()
     if batch_idx % args.log_interval == 0:
         wandb.log({"loss": loss})
         trigger_sync()  # <-- New!
 ```
 
+#### With pytorch lightning
+
+```python
+from wandb_osh.lightning_hooks import TriggerWandbSyncLightningCallback  # <-- New!
+from pytorch_lightning.loggers import WandbLogger
+from pytorch_lightning import Trainer
+
+logger = WandbLogger(
+    project="project",
+    group="group",
+    offline=True,
+)
+
+model = MyLightningModule()
+trainer = Trainer(
+    logger=logger,
+    callbacks=[TriggerWandbSyncLightningCallback()]  # <-- New!
+)
+trainer.fit(model, train_dataloader, val_dataloader)
+```
+
 #### With ray tune
 
-You probably already use the `WandbLoggerCallback` callback. We simply add a second callback for `wandb-osh` (it only takes one new line!):
+> **Note**
+> With ray tune, you might not need this package! While the approach suggested in the
+> [ray tune SLURM docs][ray-tune-slurm-docs] deploys the ray head on a worker node as well (so it doesn't
+> have internet), this actually isn't needed. Instead, you can run the ray head and the
+> tuning script on the head node and only submit batch jobs for your workers.
+> In this way, `wandb` will be called from the head node and internet access is no
+> problem there.
+> For more information on this approach, take a look at my [demo repository][ray-tune-slurm-test].
+
+You probably already use the `WandbLoggerCallback` callback. We simply add a second callback for `wandb-osh` (it only takes two new lines!):
 
 ```python
 import os
-from wandb_osh.ray_hooks import TriggerWandbSyncRayHook
+from wandb_osh.ray_hooks import TriggerWandbSyncRayHook  # <-- New!
 
 
 os.environ["WANDB_MODE"] = "offline"
 
 callbacks = [
     WandbLoggerCallback(...),  # <-- ray tune documentation tells you about this
     TriggerWandbSyncRayHook(),  # <-- New!
@@ -230,7 +265,10 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 <!--  -->
 <!-- This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome! -->
 
 [github-issues]: https://github.com/klieret/wandb-offline-sync-hook/issues
 [pulls]: https://github.com/klieret/wandb-offline-sync-hook/pulls
+[ray-tune-slurm-docs]: https://docs.ray.io/en/latest/cluster/vms/user-guides/community/slurm.html
+[ray-tune-slurm-test]: https://github.com/klieret/ray-tune-slurm-test/
+[ray-tune]: https://docs.ray.io/en/latest/tune/index.html
```

