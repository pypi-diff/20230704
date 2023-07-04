# Comparing `tmp/docker_shaper-0.1.6.tar.gz` & `tmp/docker_shaper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_shaper-0.1.6.tar", max compression
+gzip compressed data, was "docker_shaper-0.1.7.tar", max compression
```

## Comparing `docker_shaper-0.1.6.tar` & `docker_shaper-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2481 2023-07-03 06:21:36.838441 docker_shaper-0.1.6/Readme.md
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/__init__.py
--rwxr-xr-x   0        0        0     1459 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/cli.py
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/common.py
--rw-r--r--   0        0        0        1 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/docker_stuff.py
--rw-r--r--   0        0        0    27105 2023-07-04 11:15:19.804280 docker_shaper-0.1.6/docker_shaper/dynamic.py
--rw-r--r--   0        0        0     6580 2023-07-04 09:11:10.155947 docker_shaper-0.1.6/docker_shaper/server.py
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/static/__init__.py
--rw-r--r--   0        0        0   155631 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/static/bootstrap.css
--rw-r--r--   0        0        0     9017 2023-06-26 07:29:52.330340 docker_shaper-0.1.6/docker_shaper/static/normalize.css
--rw-r--r--   0        0        0     6108 2023-06-26 07:36:31.223451 docker_shaper-0.1.6/docker_shaper/static/pills.css
--rw-r--r--   0        0        0     2474 2023-06-26 07:30:04.714374 docker_shaper-0.1.6/docker_shaper/static/style.css
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/templates/__init__.py
--rw-r--r--   0        0        0     1170 2023-07-03 13:04:26.635859 docker_shaper-0.1.6/docker_shaper/templates/base.html
--rw-r--r--   0        0        0      321 2023-06-30 07:37:58.659311 docker_shaper-0.1.6/docker_shaper/templates/containers.html
--rw-r--r--   0        0        0      950 2023-07-04 09:38:17.014630 docker_shaper-0.1.6/docker_shaper/templates/dashboard.html
--rw-r--r--   0        0        0      309 2023-06-30 07:37:58.631311 docker_shaper-0.1.6/docker_shaper/templates/images.html
--rw-r--r--   0        0        0     5472 2023-07-04 08:46:32.577312 docker_shaper-0.1.6/docker_shaper/utils.py
--rw-r--r--   0        0        0     2259 2023-07-04 11:20:13.417072 docker_shaper-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 docker_shaper-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2481 2023-07-03 06:21:36.838441 docker_shaper-0.1.7/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/__init__.py
+-rwxr-xr-x   0        0        0     1459 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/cli.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/common.py
+-rw-r--r--   0        0        0        1 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/docker_stuff.py
+-rw-r--r--   0        0        0    27912 2023-07-04 15:49:46.449395 docker_shaper-0.1.7/docker_shaper/dynamic.py
+-rw-r--r--   0        0        0     6580 2023-07-04 15:23:50.424596 docker_shaper-0.1.7/docker_shaper/server.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/static/__init__.py
+-rw-r--r--   0        0        0   155631 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/static/bootstrap.css
+-rw-r--r--   0        0        0     9017 2023-06-26 07:29:52.330340 docker_shaper-0.1.7/docker_shaper/static/normalize.css
+-rw-r--r--   0        0        0     6108 2023-06-26 07:36:31.223451 docker_shaper-0.1.7/docker_shaper/static/pills.css
+-rw-r--r--   0        0        0     2474 2023-06-26 07:30:04.714374 docker_shaper-0.1.7/docker_shaper/static/style.css
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.7/docker_shaper/templates/__init__.py
+-rw-r--r--   0        0        0     1170 2023-07-03 13:04:26.635859 docker_shaper-0.1.7/docker_shaper/templates/base.html
+-rw-r--r--   0        0        0      321 2023-06-30 07:37:58.659311 docker_shaper-0.1.7/docker_shaper/templates/containers.html
+-rw-r--r--   0        0        0      956 2023-07-04 11:41:27.395858 docker_shaper-0.1.7/docker_shaper/templates/dashboard.html
+-rw-r--r--   0        0        0      309 2023-06-30 07:37:58.631311 docker_shaper-0.1.7/docker_shaper/templates/images.html
+-rw-r--r--   0        0        0     5474 2023-07-04 15:11:26.966906 docker_shaper-0.1.7/docker_shaper/utils.py
+-rw-r--r--   0        0        0     2259 2023-07-04 15:59:07.639134 docker_shaper-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 docker_shaper-0.1.7/PKG-INFO
```

### Comparing `docker_shaper-0.1.6/Readme.md` & `docker_shaper-0.1.7/Readme.md`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.6/docker_shaper/cli.py` & `docker_shaper-0.1.7/docker_shaper/cli.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.6/docker_shaper/dynamic.py` & `docker_shaper-0.1.7/docker_shaper/dynamic.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import re
 import time
 from contextlib import suppress
 from dataclasses import dataclass
 from datetime import datetime
 from subprocess import CalledProcessError
-from typing import Union, MutableMapping, MutableSequence, Optional, Tuple
+from typing import MutableMapping, MutableSequence, Optional, Tuple, Union
 
 from aiodocker import Docker, DockerError
 from dateutil import tz
 from flask_table import Col, Table
 from quart import render_template, request, url_for
 
 from docker_shaper.utils import aimpatient, impatient, process_output, watchdog
@@ -71,24 +71,23 @@
     """
     if not docker_id:
         return docker_id
     assert is_uid(docker_id)
     return docker_id[7:17] if docker_id.startswith("sha256:") else docker_id[:10]
 
 
-def age_str(now: Union[int,datetime], age: Union[int,datetime,None]) -> str:
+def age_str(now: Union[int, datetime], age: Union[int, datetime, None]) -> str:
     """Turn a number of seconds into something human readable"""
     if age is None:
         return "--"
-    tds = int((now.timestamp() if isinstance(now, datetime) else now)-(age.timestamp() if isinstance(age, datetime) else age))
-    return (
-        f"{tds//86400:02d}d"
-        f":{tds//3600%24:02d}h"
-        f":{tds//60%60:02d}m"
+    tds = int(
+        (now.timestamp() if isinstance(now, datetime) else now)
+        - (age.timestamp() if isinstance(age, datetime) else age)
     )
+    return f"{tds//86400:02d}d" f":{tds//3600%24:02d}h" f":{tds//60%60:02d}m"
 
 
 def date_str(date: datetime) -> str:
     if not date:
         return "--"
     return (datetime.fromtimestamp(date) if isinstance(date, int) else date).strftime(
         "%Y.%m.%d-%H:%M:%S"
@@ -228,85 +227,108 @@
         )
     elif object_type in {"network", "builder"}:
         return
     elif (object_type, operator) in {
         ("image", "untag"),
         ("image", "prune"),
         ("image", "delete"),
-        ("container", "attach"),
+
+        ("container", "exec_create:"),
+        ("container", "exec_start:"),
+        ("container", "exec_die"),
+        ("container", "kill"),
         ("container", "start"),
+        ("container", "attach"),
         ("container", "die"),
         ("container", "destroy"),
         ("container", "prune"),
+        ("container", "stop"),
+        ("container", "archive-path"),
+
         ("network", "connect"),
         ("network", "disconnect"),
+
+        ("volume", "mount"),
+        ("volume", "unmount"),
+        ("volume", "destroy"),
     }:
         return
     else:
-        log().warning("unknown type/operator %s  %s", object_type, operator)
+        log().warning("unknown type/operator %s %s", object_type, operator)
         return
 
-    # log().debug("handle docker event %s", (tstamp, _uid[:12], operator, params["image"]))
-    #if not (referenced_image_id := lookup_id(global_state.image_ids, ident)):
-    #    return
-
-    # print(ident, uid)
-    # print(await docker_client.images.get(ident))
-    # print(await docker_client.containers.get(uid))
-
     global_state.event_horizon = min(global_state.event_horizon, tstamp)
-
     register_reference(ident, tstamp, global_state)
 
-def is_uid(ident:str) -> bool:
+
+def is_uid(ident: str) -> bool:
     """
     sha256:48a3535fe27fea1ac6c2f41547770d081552c54b2391c2dda99e2ad87561a4f2
     48a3535fe27fea1ac6c2f41547770d081552c54b2391c2dda99e2ad87561a4f2
     48a3535fe27f
     """
-    return ident.startswith("sha256:") or re.match("[0-9a-f]{64}", ident) or re.match("[0-9a-f]{10}", ident)
+    return (
+        ident.startswith("sha256:")
+        or re.match("[0-9a-f]{64}", ident)
+        or re.match("[0-9a-f]{10}", ident)
+    )
+
+
+def unique_ident(ident: str) -> str:
+    return short_id(ident) if is_uid(ident) else ident
 
 
 def register_reference(ident: str, timestamp: int, global_state) -> None:
-    effective_ident = short_id(ident) if (is_uid_ := is_uid(ident)) else ident
+    effective_ident = unique_ident(ident)
     if effective_ident not in global_state.last_referenced:
         global_state.last_referenced[effective_ident] = [
             0,
-            global_state.expiration_ages["tag_unknown"] if is_uid_ else expiration_age_from_rules(effective_ident, global_state)
+            expiration_age_from_ident(effective_ident, global_state),
         ]
 
     # increase last reference date if applicable
     global_state.last_referenced[effective_ident][0] = max(
         global_state.last_referenced[effective_ident][0], timestamp
     )
 
 
-def expiration_age_from_rules(ident: str, global_state: GlobalState) -> int:
+def expiration_age_from_ident(ident: str, global_state: GlobalState) -> int:
     if is_uid(ident):
-        log().error("expiration_age_from_rules %s", ident)
-    matching_rules = tuple((regex, age) for regex, age in global_state.tag_rules.items() if re.match(regex, ident))
+        return global_state.expiration_ages["tag_unknown"]
+
+    effective_ident = unique_ident(ident)
+
+    matching_rules = tuple(
+        (regex, age)
+        for regex, age in global_state.tag_rules.items()
+        if re.match(regex, effective_ident)
+    )
+
     if len(matching_rules) == 1:
         return matching_rules[0][1]
     if not matching_rules:
         log().warn("No rule found for %s", ident)
     else:
         log().error("Multiple rules found for %s:", ident)
         for rule in matching_rules:
             log().error("  %s:", rule[0])
+
     return global_state.expiration_ages["tag_unknown"]
 
 
 @impatient
 def expired(ident: str, global_state, now: int, extra_date: int = 0) -> bool:
     if ident not in global_state.last_referenced:
         log().warn("no reference: %s", ident)
-    else:
-        breakpoint
+
     # TODO
-    last_referenced, expiration_age = global_state.last_referenced.get(ident, [None, global_state.expiration_ages["tag_unknown"]])
+    last_referenced, expiration_age = global_state.last_referenced.setdefault(
+        ident, [None, expiration_age_from_ident(ident, global_state)]
+    )
+
     effective_age = now - max(
         last_referenced or 0,
         global_state.event_horizon,
         extra_date,
     )
     return effective_age > expiration_age, last_referenced, expiration_age
 
@@ -382,14 +404,15 @@
         return f"<tt><b>{content}</b></tt>"
 
 
 class ImageTable(BaseTable):
     short_id = PlainCol("short_id")
     tags = PlainCol("tags")
     created_at = PlainCol("created_at")
+    age = PlainCol("age")
 
     def sort_url(self, col_key, reverse=False):
         return url_for(
             self.endpoint,
             sort_key_images=col_key,
             sort_direction_images="desc" if reverse else "asc",
         )
@@ -399,25 +422,29 @@
         now = datetime.now(tz=tz.tzutc())
 
         def dict_from(image):
             now_timestamp = now.timestamp()
             created_timestamp = date_from(image["created_at"]).timestamp()
 
             def coloured_ident(ident):
-                is_expired, last_referenced, expiration_age = expired(ident, global_state, now_timestamp, created_timestamp)
+                is_expired, last_referenced, expiration_age = expired(
+                    ident, global_state, now_timestamp, created_timestamp
+                )
                 if is_expired:
-                    return f"<div class='text-danger'>{ident} ({age_str(now, last_referenced)})</div>"
+                    return (
+                        f"<div class='text-danger'>{ident} ({age_str(now, last_referenced)})</div>"
+                    )
                 return f"<div class='text-success'>{ident} ({age_str(now, last_referenced)})</div>"
 
             return {
                 "short_id": coloured_ident(image["short_id"]),
                 "tags": "".join(map(coloured_ident, image["tags"])),
                 "created_at": date_str(image["created_at"]),
                 "age": age_str(now, date_from(image["created_at"])),
-                #"last_referenced": last_referenced_str(image["short_id"]),
+                # "last_referenced": last_referenced_str(image["short_id"]),
                 # "class": "text-danger" if would_cleanup_image(image, now, global_state) else "text-success",
             }
 
         return ImageTable(
             endpoint,
             items=sorted(
                 map(dict_from, global_state.images.values()),
@@ -730,20 +757,27 @@
         return (
             now - date_from(show["State"]["StartedAt"]).timestamp()
             > global_state.expiration_ages["container_running"]
         )
     return False
 
 
-@impatient
-def image_expired(image, now: datetime, global_state):
+def expired_idents(image, now, global_state: GlobalState):
     created_timestamp = int(date_from(image["created_at"]).timestamp())
-    return expired(image["short_id"], global_state, now, created_timestamp) and all(
-        expired(tag, global_state, now, created_timestamp) for tag in image["tags"]
-    )
+    for tag in image["tags"]:
+        if expired(tag, global_state, now, created_timestamp)[0]:
+            yield tag
+    if expired(image["short_id"], global_state, now, created_timestamp)[0]:
+        yield image["short_id"]
+
+
+async def image_from(docker_client: Docker, ident: str) -> bool:
+    with suppress(DockerError):
+        return await docker_client.images.get(ident)
+    return None
 
 
 @aimpatient
 async def cleanup(docker_client: Docker, global_state):
     log().info("Cleanup!..")
     now = int(datetime.now().timestamp())
 
@@ -764,22 +798,30 @@
             global_state,
             "warn",
             f"force removing container {container_info['short_id']}",
             container_info["container"],
         )
         await container_info["container"].delete(force=True, v=True)
 
-    for image_info in list(
-        filter(lambda image: image_expired(image, now, global_state), global_state.images.values())
-    ):
-        if not global_state.switches.get("remove_images"):
-            log().info(f"skip removal of image {image_info['short_id']}")
-            continue
-        report(global_state, "info", f"try to remove image {image_info['short_id']}", image_info)
-        # image["cleanup"] =
+    for image_info in global_state.images.values():
+        for ident in expired_idents(image_info, now, global_state):
+            if not global_state.switches.get("remove_images"):
+                log().info(f"skip removal of image/tag {ident}")
+                continue
+            report(global_state, "info", f"remove image/tag {ident}", None)
+            try:
+                await docker_client.images.delete(ident)
+            except DockerError as exc:
+                log().error("Could not delete image %s, error was %s", ident, exc)
+
+    for ident in [
+        ident for ident in global_state.images if not await image_from(docker_client, ident)
+    ]:
+        log().warning("reference to image %s has not been cleaned up, I'll do it now..", ident)
+        del global_state.images[ident]
 
     log().info("Cleanup done!")
 
 
 @impatient
 def report(global_state, msg_type, message: str, extra):
     # TODO: cleanup
@@ -787,8 +829,8 @@
     log().info(message)
     global_state.messages.insert(0, (datetime.now().timestamp(), msg_type, message, str(extra)))
 
 
 @impatient
 def reconfigure(global_state: GlobalState) -> None:
     for ident, reference in global_state.last_referenced.items():
-        reference[1] = expiration_age_from_rules(ident, global_state)
+        reference[1] = expiration_age_from_ident(ident, global_state)
```

### Comparing `docker_shaper-0.1.6/docker_shaper/server.py` & `docker_shaper-0.1.7/docker_shaper/server.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.6/docker_shaper/static/bootstrap.css` & `docker_shaper-0.1.7/docker_shaper/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.6/docker_shaper/static/normalize.css` & `docker_shaper-0.1.7/docker_shaper/static/normalize.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.6/docker_shaper/static/pills.css` & `docker_shaper-0.1.7/docker_shaper/static/pills.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.6/docker_shaper/static/style.css` & `docker_shaper-0.1.7/docker_shaper/static/style.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.6/docker_shaper/templates/base.html` & `docker_shaper-0.1.7/docker_shaper/templates/base.html`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.6/docker_shaper/templates/dashboard.html` & `docker_shaper-0.1.7/docker_shaper/templates/dashboard.html`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   <table class="table table-striped">
     <tr>
       <td>event_horizon (monitoring since)</td>
       <td><b>{{meta.event_horizon}}</b></td>
 
     </tr><tr>
 
-      <td>intervals:</td>
+      <td>expiration ages:</td>
       {% for age in meta.expiration_ages %}
           <td>{{age}} = <b>{{meta.expiration_ages[age]}}s</b>  </td><td></td>
       {% endfor %}
 
     </tr><tr>
 
       <td>switches:</td>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "base.html" %} {% block content %}
 event_horizon (monitoring since) {{meta.event_horizon}}
-intervals:                       {{age}} = {{meta.expiration_ages[age]}}s
+expiration ages:                 {{age}} = {{meta.expiration_ages[age]}}s
 switches:                        {{switch}} = {{meta.switches[switch]}}
 ***** containers ({{meta.container_count}}) *****
 {{ containers_html|safe }}
 ***** images ({{meta.image_count}}) *****
 {{ images_html|safe }}
 ***** messages ({{messages|length}}) *****
 {{msg[0]}} {{msg[1]}} {{msg[2]}}
```

### Comparing `docker_shaper-0.1.6/docker_shaper/utils.py` & `docker_shaper-0.1.7/docker_shaper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     """Logger for this module"""
     return logging.getLogger("docker-shaper.utils")
 
 
 def setup_logging(level: str = "INFO") -> None:
     """Make logging fun"""
     for lev in LOG_LEVELS:
-        logging.addLevelName(getattr(logging, lev), f"({lev[0] * 2})")
+        logging.addLevelName(getattr(logging, lev), f"{lev[0] * 2}")
 
     logging.basicConfig(
         format=(
-            "%(levelname)s: %(message)s"
+            "(%(levelname)s): %(message)s"
             if os.environ.get("USER") == "root"
-            else "%(levelname)s %(asctime)s %(name)s: %(message)s"
+            else "(%(levelname)s) %(asctime)s %(name)s: %(message)s"
         ),
         datefmt="%Y-%m-%d %H:%M:%S",
         level=logging.DEBUG if level == "ALL_DEBUG" else logging.WARNING,
     )
     logging.getLogger().setLevel(getattr(logging, level.split("_")[-1]))
     logging.getLogger("urllib3.connectionpool").setLevel(logging.INFO)
 
@@ -67,15 +67,15 @@
 def impatient(func):
     @wraps(func)
     def run(*args: object, **kwargs: object) -> object:
         try:
             t1 = time.time()
             return func(*args, **kwargs)
         finally:
-            if (duration := time.time() - t1) > 0.1:
+            if (duration := time.time() - t1) > 0.2:
                 log().warn("%s took %.2fs!", func.__name__, duration)
             # log().info("%s took %.2fs!", func.__name__, duration)
 
     return run
 
 
 def aimpatient(func):
```

### Comparing `docker_shaper-0.1.6/pyproject.toml` & `docker_shaper-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-shaper"
-version = "0.1.6"
+version = "0.1.7"
 description = "Keeps Docker resources in shape based on rules and usage"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/Checkmk/checkmk-dev-tools"
 readme = "Readme.md"
 packages = [
   {include = "docker_shaper/**/*.py"},
   {include = "docker_shaper/static"},
```

### Comparing `docker_shaper-0.1.6/PKG-INFO` & `docker_shaper-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-shaper
-Version: 0.1.6
+Version: 0.1.7
 Summary: Keeps Docker resources in shape based on rules and usage
 Home-page: https://github.com/Checkmk/checkmk-dev-tools
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

