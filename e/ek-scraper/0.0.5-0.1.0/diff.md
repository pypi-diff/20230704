# Comparing `tmp/ek-scraper-0.0.5.tar.gz` & `tmp/ek_scraper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ek-scraper-0.0.5.tar", last modified: Wed Jan 18 18:41:58 2023, max compression
+gzip compressed data, was "ek_scraper-0.1.0.tar", max compression
```

## Comparing `ek-scraper-0.0.5.tar` & `ek_scraper-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 18:41:58.226128 ek-scraper-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-18 18:41:49.000000 ek-scraper-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-01-18 18:41:58.226128 ek-scraper-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-01-18 18:41:49.000000 ek-scraper-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 18:41:58.222128 ek-scraper-0.0.5/ek_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-18 18:41:49.000000 ek-scraper-0.0.5/ek_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-18 18:41:49.000000 ek-scraper-0.0.5/ek_scraper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-01-18 18:41:49.000000 ek-scraper-0.0.5/ek_scraper/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 18:41:58.226128 ek-scraper-0.0.5/ek_scraper/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-18 18:41:49.000000 ek-scraper-0.0.5/ek_scraper/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-01-18 18:41:49.000000 ek-scraper-0.0.5/ek_scraper/notifications/pushover.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-01-18 18:41:49.000000 ek-scraper-0.0.5/ek_scraper/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 18:41:58.226128 ek-scraper-0.0.5/ek_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-01-18 18:41:58.000000 ek-scraper-0.0.5/ek_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-01-18 18:41:58.000000 ek-scraper-0.0.5/ek_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 18:41:58.000000 ek-scraper-0.0.5/ek_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-18 18:41:58.000000 ek-scraper-0.0.5/ek_scraper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-18 18:41:58.000000 ek-scraper-0.0.5/ek_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-18 18:41:58.000000 ek-scraper-0.0.5/ek_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-18 18:41:49.000000 ek-scraper-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 18:41:58.226128 ek-scraper-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 18:41:49.000000 ek-scraper-0.0.5/setup.py
+-rw-r--r--   0        0        0     1069 2023-07-04 19:58:35.239834 ek_scraper-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5242 2023-07-04 19:58:35.239834 ek_scraper-0.1.0/README.md
+-rw-r--r--   0        0        0      107 2023-07-04 19:58:35.239834 ek_scraper-0.1.0/ek_scraper/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-04 19:58:35.239834 ek_scraper-0.1.0/ek_scraper/__main__.py
+-rw-r--r--   0        0        0     5604 2023-07-04 19:58:35.239834 ek_scraper-0.1.0/ek_scraper/cli.py
+-rw-r--r--   0        0        0      255 2023-07-04 19:58:35.239834 ek_scraper-0.1.0/ek_scraper/notifications/__init__.py
+-rw-r--r--   0        0        0     2955 2023-07-04 19:58:35.239834 ek_scraper-0.1.0/ek_scraper/notifications/pushover.py
+-rw-r--r--   0        0        0     9797 2023-07-04 19:58:35.239834 ek_scraper-0.1.0/ek_scraper/scraper.py
+-rw-r--r--   0        0        0     1765 2023-07-04 19:58:35.239834 ek_scraper-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6226 1970-01-01 00:00:00.000000 ek_scraper-0.1.0/PKG-INFO
```

### Comparing `ek-scraper-0.0.5/LICENSE` & `ek_scraper-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ek-scraper-0.0.5/PKG-INFO` & `ek_scraper-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,32 @@
-Metadata-Version: 2.1
-Name: ek-scraper
-Version: 0.0.5
-Summary: Simple scraper for Ebay Kleinanzeigen searches with notifications for new ads.
-Author: Jonas Ehrlich
-Author-email: jonas.ehrlich@gmail.com
-License: MIT
-Project-URL: homepage, https://github.com/jonasehrlich/ek-scraper
-Project-URL: repository, https://github.com/jonasehrlich/ek-scraper
-Keywords: scraper
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # ek-scraper
 
-Simple scraper for Ebay Kleinanzeigen searches with notifications for new ads.
+Simple scraper for kleinanzeigen.de searches with notifications for new ads.
 
 ## Installation
 
 Install this package from PyPi using `pip`.
 
-``` bash
+``` sh
 pip3 install ek-scraper
 ```
 
 ## Usage
 
 > For the full usage check the `ek-scraper --help` command
 
 Create a configuration file using
 
-``` bash
+``` sh
 ek-scraper create-config <path/to/config.json>
 ```
 
 The example configuration file will look like this:
 
 ```json
-
 {
   "filter": {
     "exclude_topads": true,
     "exclude_patterns": []
   },
   "notifications": {
     "pushover": {
@@ -55,75 +34,69 @@
         "user": "<your-user-api-token>",
         "device": []
     }
   },
   "searches": [
     {
       "name": "Wohnungen in Hamburg Altona",
-      "url": "https://www.ebay-kleinanzeigen.de/s-wohnung-mieten/altona/c203l9497",
+      "url": "https://www.kleinanzeigen.de/s-wohnung-mieten/altona/c203l9497",
       "recursive": true
     }
   ]
 }
-
 ```
 
 See [Configuration](#configuration) for details on all configuration options.
 
 * Configure one or more searches in the `searches` section of the configuration, see [Searches](#searches) for
   more details
 * Configure notifications in the `notifications` section of the configuration, see [Notifications](#notifications)
   for details on notification configuration
 * (Optional) Configure filters in the `filter` section of the configuration, see [Filter](#filter) for more details
 
 Run the following command to initialize the data store without sending any notifications:
 
-``` bash
+``` sh
 ek-scraper run --no-notifications path/to/config.json
 ```
 
 Afterwards, run
 
-```bash
+```sh
 ek-scraper run path/to/config.json
 ```
 
 to receive notifications according to your `notifications` configuration.
 
 ## Development
 
 Follow the steps below to set up a development environment for this project.
 
 1. Clone this repository
 
-   ``` bash
+   ``` sh
    git clone git@github.com:jonasehrlich/ek-scraper.git
    ```
 
-2. Change into the repository
+2. Change directory into the repository
 
-   ``` bash
+   ``` sh
    cd ek-scraper
    ```
 
-3. Create a virtual environment
+3. Create a virtual environment using [poetry](https://python-poetry.org)
 
-   ``` bash
-   python3 -m venv .venv && . .venv/bin/activate
+   ``` sh
+   poetry install
    ```
 
-4. Install the package as an editable installation along with its dev dependencies
-
-   ``` bash
-   pip3 install -e .[dev]
-   ```
 
 5. (Optional) Install pre-commit environment
 
-   ``` bash
+   ``` sh
    $ pre-commit
    [INFO] Installing environment for https://github.com/pre-commit/pre-commit-hooks.
    [INFO] Once installed this environment will be reused.
    [INFO] This may take a few minutes...
    [INFO] Installing environment for https://github.com/psf/black.
    [INFO] Once installed this environment will be reused.
    [INFO] This may take a few minutes...
@@ -181,14 +154,14 @@
 
 ## Running `ek-scraper` regularly
 
 In order to run `ek-scraper` regularly on a Unix-like system, configure it as a cronjob.
 
 To configure a cronjob, run
 
-``` bash
+``` sh
 crontab -e
 ```
 
 Edit the crontab table to run the command you want to run. A handy tool to check schedule configurations for cronjobs is [crontab.guru](https://crontab.guru/).
 
 For more information on configuring cronjobs use your favorite search engine.
```

### Comparing `ek-scraper-0.0.5/README.md` & `ek_scraper-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,57 @@
+Metadata-Version: 2.1
+Name: ek-scraper
+Version: 0.1.0
+Summary: Simple scraper for kleinanzeigen.de searches with notifications for new ads.
+Home-page: https://github.com/jonasehrlich/ek-scraper
+License: MIT
+Keywords: kleinanzeigen.de,scraper
+Author: Jonas Ehrlich
+Author-email: jonas.ehrlich@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Project-URL: Repository, https://github.com/jonasehrlich/ek-scraper
+Description-Content-Type: text/markdown
+
 # ek-scraper
 
-Simple scraper for Ebay Kleinanzeigen searches with notifications for new ads.
+Simple scraper for kleinanzeigen.de searches with notifications for new ads.
 
 ## Installation
 
 Install this package from PyPi using `pip`.
 
-``` bash
+``` sh
 pip3 install ek-scraper
 ```
 
 ## Usage
 
 > For the full usage check the `ek-scraper --help` command
 
 Create a configuration file using
 
-``` bash
+``` sh
 ek-scraper create-config <path/to/config.json>
 ```
 
 The example configuration file will look like this:
 
 ```json
-
 {
   "filter": {
     "exclude_topads": true,
     "exclude_patterns": []
   },
   "notifications": {
     "pushover": {
@@ -35,75 +59,69 @@
         "user": "<your-user-api-token>",
         "device": []
     }
   },
   "searches": [
     {
       "name": "Wohnungen in Hamburg Altona",
-      "url": "https://www.ebay-kleinanzeigen.de/s-wohnung-mieten/altona/c203l9497",
+      "url": "https://www.kleinanzeigen.de/s-wohnung-mieten/altona/c203l9497",
       "recursive": true
     }
   ]
 }
-
 ```
 
 See [Configuration](#configuration) for details on all configuration options.
 
 * Configure one or more searches in the `searches` section of the configuration, see [Searches](#searches) for
   more details
 * Configure notifications in the `notifications` section of the configuration, see [Notifications](#notifications)
   for details on notification configuration
 * (Optional) Configure filters in the `filter` section of the configuration, see [Filter](#filter) for more details
 
 Run the following command to initialize the data store without sending any notifications:
 
-``` bash
+``` sh
 ek-scraper run --no-notifications path/to/config.json
 ```
 
 Afterwards, run
 
-```bash
+```sh
 ek-scraper run path/to/config.json
 ```
 
 to receive notifications according to your `notifications` configuration.
 
 ## Development
 
 Follow the steps below to set up a development environment for this project.
 
 1. Clone this repository
 
-   ``` bash
+   ``` sh
    git clone git@github.com:jonasehrlich/ek-scraper.git
    ```
 
-2. Change into the repository
+2. Change directory into the repository
 
-   ``` bash
+   ``` sh
    cd ek-scraper
    ```
 
-3. Create a virtual environment
+3. Create a virtual environment using [poetry](https://python-poetry.org)
 
-   ``` bash
-   python3 -m venv .venv && . .venv/bin/activate
+   ``` sh
+   poetry install
    ```
 
-4. Install the package as an editable installation along with its dev dependencies
-
-   ``` bash
-   pip3 install -e .[dev]
-   ```
 
 5. (Optional) Install pre-commit environment
 
-   ``` bash
+   ``` sh
    $ pre-commit
    [INFO] Installing environment for https://github.com/pre-commit/pre-commit-hooks.
    [INFO] Once installed this environment will be reused.
    [INFO] This may take a few minutes...
    [INFO] Installing environment for https://github.com/psf/black.
    [INFO] Once installed this environment will be reused.
    [INFO] This may take a few minutes...
@@ -161,14 +179,15 @@
 
 ## Running `ek-scraper` regularly
 
 In order to run `ek-scraper` regularly on a Unix-like system, configure it as a cronjob.
 
 To configure a cronjob, run
 
-``` bash
+``` sh
 crontab -e
 ```
 
 Edit the crontab table to run the command you want to run. A handy tool to check schedule configurations for cronjobs is [crontab.guru](https://crontab.guru/).
 
 For more information on configuring cronjobs use your favorite search engine.
+
```

### Comparing `ek-scraper-0.0.5/ek_scraper/cli.py` & `ek_scraper-0.1.0/ek_scraper/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 )
 
 _logger = logging.getLogger(__name__.split(".", 1)[0])
 
 
 DUMMY_SEARCH_CONFIG = SearchConfig(
     name="Wohnungen in Hamburg Altona",
-    url="https://www.ebay-kleinanzeigen.de/s-wohnung-mieten/altona/c203l9497",
+    url="https://www.kleinanzeigen.de/s-wohnung-mieten/altona/c203l9497",
 )
 
 
 def configure_logging(verbose: bool) -> None:
     """Configure stream logging"""
     level = logging.DEBUG if verbose else logging.INFO
     _logger.setLevel(level)
@@ -53,26 +53,25 @@
         metavar="CONFIG_FILE",
         type=pathlib.Path,
         help="Configuration file for the scraper",
     )
 
 
 def get_argument_parser() -> argparse.ArgumentParser:
-
     example_config_file_text = textwrap.indent(
         json.dumps(
             dataclasses.asdict(Config(searches=[DUMMY_SEARCH_CONFIG])),
             indent=2,
         ),
         prefix="    ",
     )
     parser = argparse.ArgumentParser(
         prog="ek-scraper",
         description=(
-            f"Scraper for Ebay Kleinanzeigen search results.\n\n"
+            f"Scraper for kleinanzeigen.de search results.\n\n"
             f"Example configuration file:\n\n{example_config_file_text}"
         ),
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser.add_argument("--version", action="version", version=f"%(prog)s {__version__}")
     parser.add_argument("--verbose", "-v", action="store_true", default=False, help="Enable verbose output")
 
@@ -102,15 +101,14 @@
     return parser
 
 
 NOTIFICATION_CALLBACKS: dict[str, SendNotification] = {"pushover": pushover.send_notifications}
 
 
 async def run(data_store_file: pathlib.Path, config_file: pathlib.Path, send_notifications: bool, **kwargs):
-
     config = load_config(config_file)
     with DataStore(data_store_file) as data_store:
         tasks = list()
         for search in config.searches:
             tasks.append(get_new_aditems(search, config.filter, data_store=data_store))
 
         results: list[Result] = await asyncio.gather(*tasks)
@@ -135,39 +133,42 @@
             _logger.error("No notification callback registered for key '%s'", notification_type)
             continue
         _logger.info("Call notification callback for '%s'", notification_type)
         await notification_callback(results, notification_settings)
 
 
 def create_config(config_file: pathlib.Path, **kwargs):
-    with open(config_file, "w") as f:
-
+    with config_file.open("w") as f:
         config = Config(
             notifications={"pushover": pushover.PushoverConfig.to_default_dict()}, searches=[DUMMY_SEARCH_CONFIG]
         )
         json.dump(config, f, cls=DataclassesJSONEncoder, indent=2)
     _logger.info("Created default config file at '%s'", config_file)
 
 
 async def async_main():
     """Async main function."""
     parser = get_argument_parser()
     namespace = parser.parse_args()
     configure_logging(namespace.verbose)
-    func = namespace.__func__
+
+    try:
+        func = namespace.__func__
+    except AttributeError:
+        parser.error(parser.format_usage())
 
     try:
         ret = func(**vars(namespace))
         if inspect.isawaitable(ret):
             await ret
     except Exception as exc:
         if namespace.verbose:
             _logger.exception("Error!")
 
-        parser.error(str(exc))
+        parser.exit(str(exc))
 
 
 def main():
     asyncio.run(async_main())
 
 
 if __name__ == "__main__":
```

### Comparing `ek-scraper-0.0.5/ek_scraper/notifications/pushover.py` & `ek_scraper-0.1.0/ek_scraper/notifications/pushover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
+import asyncio
 import dataclasses
+import logging
 import typing as ty
 
-import logging
 import aiohttp
-import asyncio
 
 if ty.TYPE_CHECKING:
     from ek_scraper import Result
 
 BASE_URL = "https://api.pushover.net"
 
 _logger = logging.getLogger(__name__)
@@ -74,15 +74,15 @@
     :param config_dict: Configuration for the notification
     :type config_dict: dict
     :raises ValueError: Raised if the required configuration parameters were not provided
     """
     try:
         config = PushoverConfig(**config_dict)
     except TypeError:
-        raise ValueError(f"Could not create PushoverConfig from {config_dict}")
+        raise ValueError(f"Could not create PushoverConfig from {config_dict}") from None
 
     async with aiohttp.ClientSession(BASE_URL) as session:
         tasks = list()
         for result in results:
             if not result.aditems:
                 _logger.info("")
                 continue
```

### Comparing `ek-scraper-0.0.5/ek_scraper/scraper.py` & `ek_scraper-0.1.0/ek_scraper/scraper.py`

 * *Files 16% similar despite different names*

```diff
@@ -89,21 +89,21 @@
         return self
 
     def __exit__(self, *args):
         self.close()
 
     def open(self):
         try:
-            with open(self.path) as f:
+            with self.path.open() as f:
                 self.data = {key: AdItem(**value) for key, value in json.load(f).items()}
         except FileNotFoundError:
             _logger.warning("Data store does not exist at '%s', will be created when closing", self.path)
 
     def close(self):
-        with open(self.path, "w") as f:
+        with self.path.open("w") as f:
             json.dump(self.data, f, cls=DataclassesJSONEncoder, indent=2)
 
 
 @dataclasses.dataclass
 class Result:
     """Results of search config"""
 
@@ -163,25 +163,32 @@
     _logger.debug("Find all ad items in '%s'", url)
     for soup_aditem in soup.find_all("article", class_="aditem"):
         calendar_icons = soup_aditem.select(".icon-calendar-open")
         if calendar_icons:
             added = ty.cast(str, calendar_icons[0].parent.text.strip())
         else:
             added = None
-        aditem = AdItem(
-            id=soup_aditem.get("data-adid"),
-            url=urljoin(url, soup_aditem.get("data-href")),
-            title=soup_aditem.select(".text-module-begin>a")[0].text.strip(),
-            description=soup_aditem.select(".aditem-main--middle--description")[0].text.strip(),
-            location=soup_aditem.select(".icon-pin")[0].parent.text.strip(),
-            price=soup_aditem.select('p[class*="price"]')[0].text.strip(),
-            added=added,
-            image_url=soup_aditem.select(".imagebox")[0].get("data-imgsrc"),
-            is_topad=bool(soup_aditem.select(".icon-feature-topad")),
-        )
+        try:
+            aditem = AdItem(
+                id=soup_aditem.get("data-adid"),
+                url=urljoin(url, soup_aditem.get("data-href")),
+                title=soup_aditem.select(".text-module-begin>a")[0].text.strip(),
+                description=soup_aditem.select(".aditem-main--middle--description")[0].text.strip(),
+                location=soup_aditem.select('i[class*="icon-pin"]')[0].parent.text.strip(),
+                price=soup_aditem.select('p[class*="price"]')[0].text.strip(),
+                added=added,
+                image_url=soup_aditem.select(".imagebox")[0].get("data-imgsrc"),
+                is_topad=bool(soup_aditem.select(".icon-feature-topad")),
+            )
+        except IndexError as exc:
+            raise RuntimeError(
+                "Error parsing ads, this is probably caused by changes on kleinanzeigen.de\n\n"
+                "Please run this command again with the --verbose option and open an issue with its "
+                "output at https://github.com/jonasehrlich/ek-scraper/issues"
+            ) from exc
         yield aditem
 
 
 async def get_new_aditems(search_config: SearchConfig, filter_config: FilterConfig, data_store: DataStore) -> Result:
     """
     Return a result for a search configuration
 
@@ -247,15 +254,15 @@
             result.aditems.append(aditem)
 
         return result
 
 
 def load_config(config_file: pathlib.Path) -> Config:
     """Load the configuration from the config path"""
-    with open(config_file) as f:
+    with config_file.open() as f:
         config_dict = json.load(f)
 
     filter_config = FilterConfig(**config_dict.get("filter", dict()))
     searches = [SearchConfig(**s) for s in config_dict.get("searches", list())]
 
     if not searches:
         _logger.warning("No searches configured in '%s'", config_file)
```

