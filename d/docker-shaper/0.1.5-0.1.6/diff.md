# Comparing `tmp/docker_shaper-0.1.5.tar.gz` & `tmp/docker_shaper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_shaper-0.1.5.tar", max compression
+gzip compressed data, was "docker_shaper-0.1.6.tar", max compression
```

## Comparing `docker_shaper-0.1.5.tar` & `docker_shaper-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2298 2023-06-30 06:59:52.910235 docker_shaper-0.1.5/Readme.md
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/__init__.py
--rwxr-xr-x   0        0        0     1459 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/cli.py
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/common.py
--rw-r--r--   0        0        0        1 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/docker_stuff.py
--rw-r--r--   0        0        0    19167 2023-06-30 14:42:40.587435 docker_shaper-0.1.5/docker_shaper/dynamic.py
--rw-r--r--   0        0        0     7215 2023-06-30 13:27:56.721242 docker_shaper-0.1.5/docker_shaper/server.py
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/static/__init__.py
--rw-r--r--   0        0        0   155631 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/static/bootstrap.css
--rw-r--r--   0        0        0     9017 2023-06-26 07:29:52.330340 docker_shaper-0.1.5/docker_shaper/static/normalize.css
--rw-r--r--   0        0        0     6108 2023-06-26 07:36:31.223451 docker_shaper-0.1.5/docker_shaper/static/pills.css
--rw-r--r--   0        0        0     2474 2023-06-26 07:30:04.714374 docker_shaper-0.1.5/docker_shaper/static/style.css
--rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/templates/__init__.py
--rw-r--r--   0        0        0     1154 2023-06-30 13:59:39.534821 docker_shaper-0.1.5/docker_shaper/templates/base.html
--rw-r--r--   0        0        0      321 2023-06-30 07:37:58.659311 docker_shaper-0.1.5/docker_shaper/templates/containers.html
--rw-r--r--   0        0        0      378 2023-06-30 13:55:32.154530 docker_shaper-0.1.5/docker_shaper/templates/dashboard.html
--rw-r--r--   0        0        0      309 2023-06-30 07:37:58.631311 docker_shaper-0.1.5/docker_shaper/templates/images.html
--rw-r--r--   0        0        0     4641 2023-06-27 07:03:43.646288 docker_shaper-0.1.5/docker_shaper/utils.py
--rw-r--r--   0        0        0     2259 2023-06-30 14:43:03.363469 docker_shaper-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3102 1970-01-01 00:00:00.000000 docker_shaper-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2481 2023-07-03 06:21:36.838441 docker_shaper-0.1.6/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/__init__.py
+-rwxr-xr-x   0        0        0     1459 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/cli.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/common.py
+-rw-r--r--   0        0        0        1 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/docker_stuff.py
+-rw-r--r--   0        0        0    27105 2023-07-04 11:15:19.804280 docker_shaper-0.1.6/docker_shaper/dynamic.py
+-rw-r--r--   0        0        0     6580 2023-07-04 09:11:10.155947 docker_shaper-0.1.6/docker_shaper/server.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/static/__init__.py
+-rw-r--r--   0        0        0   155631 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/static/bootstrap.css
+-rw-r--r--   0        0        0     9017 2023-06-26 07:29:52.330340 docker_shaper-0.1.6/docker_shaper/static/normalize.css
+-rw-r--r--   0        0        0     6108 2023-06-26 07:36:31.223451 docker_shaper-0.1.6/docker_shaper/static/pills.css
+-rw-r--r--   0        0        0     2474 2023-06-26 07:30:04.714374 docker_shaper-0.1.6/docker_shaper/static/style.css
+-rw-r--r--   0        0        0        0 2023-06-27 07:03:43.646288 docker_shaper-0.1.6/docker_shaper/templates/__init__.py
+-rw-r--r--   0        0        0     1170 2023-07-03 13:04:26.635859 docker_shaper-0.1.6/docker_shaper/templates/base.html
+-rw-r--r--   0        0        0      321 2023-06-30 07:37:58.659311 docker_shaper-0.1.6/docker_shaper/templates/containers.html
+-rw-r--r--   0        0        0      950 2023-07-04 09:38:17.014630 docker_shaper-0.1.6/docker_shaper/templates/dashboard.html
+-rw-r--r--   0        0        0      309 2023-06-30 07:37:58.631311 docker_shaper-0.1.6/docker_shaper/templates/images.html
+-rw-r--r--   0        0        0     5472 2023-07-04 08:46:32.577312 docker_shaper-0.1.6/docker_shaper/utils.py
+-rw-r--r--   0        0        0     2259 2023-07-04 11:20:13.417072 docker_shaper-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 docker_shaper-0.1.6/PKG-INFO
```

### Comparing `docker_shaper-0.1.5/Readme.md` & `docker_shaper-0.1.6/Readme.md`

 * *Files 15% similar despite different names*

```diff
@@ -76,13 +76,14 @@
   - check installed package
   - go through review process
   - publish the new package `poetry publish --build --repository checkmk`
   - commit new version && push
 
 
 ## Knowledge
-https://github.com/torfsen/python-systemd-tutorial
-https://www.digitalocean.com/community/tutorials/how-to-use-templates-in-a-flask-application
-* https://blog.miguelgrinberg.com/post/beautiful-interactive-tables-for-your-flask-templates
+* [Showing Text Box On Hover (In Table)](https://stackoverflow.com/questions/52562345/showing-text-box-on-hover-in-table)
+* [Beautiful Interactive Tables for your Flask Templates](https://blog.miguelgrinberg.com/post/beautiful-interactive-tables-for-your-flask-templates)
+* https://github.com/torfsen/python-systemd-tutorial
+* https://www.digitalocean.com/community/tutorials/how-to-use-templates-in-a-flask-application
 * https://stackoverflow.com/questions/49957034/live-updating-dynamic-variable-on-html-with-flask
 * https://pgjones.gitlab.io/quart/how_to_guides/templating.html
```

### Comparing `docker_shaper-0.1.5/docker_shaper/cli.py` & `docker_shaper-0.1.6/docker_shaper/cli.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.5/docker_shaper/dynamic.py` & `docker_shaper-0.1.6/docker_shaper/dynamic.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,71 +4,136 @@
 """
 import asyncio
 import logging
 import os
 import re
 import time
 from contextlib import suppress
-from datetime import datetime, timedelta
+from dataclasses import dataclass
+from datetime import datetime
 from subprocess import CalledProcessError
-from typing import MutableMapping, Optional
+from typing import Union, MutableMapping, MutableSequence, Optional, Tuple
 
-from aiodocker import DockerError
+from aiodocker import Docker, DockerError
+from dateutil import tz
 from flask_table import Col, Table
 from quart import render_template, request, url_for
 
-from docker_shaper.utils import process_output, watchdog
+from docker_shaper.utils import aimpatient, impatient, process_output, watchdog
 
 
 def log() -> logging.Logger:
     """Logger for this module"""
     return logging.getLogger("docker-shaper.dynamic")
 
 
+@dataclass
+class GlobalState:
+    intervals: MutableMapping[str, float]
+    image_ids: MutableMapping[str, object]
+    images: MutableMapping[str, object]
+    containers: MutableMapping[str, object]
+    event_horizon: int
+    last_referenced: MutableMapping[str, MutableSequence[int]]
+    tag_rules: MutableMapping[str, int]
+    extra_links: MutableMapping[str, int]
+    messages: MutableSequence[Tuple[int, str, str]]
+    switches: MutableMapping[str, bool]
+    hostname: str
+    expiration_ages: MutableMapping[str, int]
+
+    def __init__(self):
+        self.intervals = {
+            "state": 2,
+            "image_stats": 2,
+            "image_update": 2,
+            "container_update": 2,
+            "container_stats": 2,
+            "cleanup": 3600,
+        }
+        self.image_ids = {}
+        self.images = {}
+        self.containers = {}
+        self.event_horizon = int(time.time())
+        self.last_referenced = {}
+        self.tag_rules = {}
+        self.counter = 0
+        self.extra_links = {}
+        self.switches = {}
+        self.messages = []
+        self.hostname = open("/etc/hostname").read().strip()
+        self.expiration_ages = {}
+
+
 def short_id(docker_id: str) -> str:
     """Return the 10-digit variant of a long docker ID
     >>> short_id("sha256:abcdefghijklmnop")
     'abcdefghij'
     """
     if not docker_id:
         return docker_id
-    assert docker_id.startswith("sha256:")
-    return docker_id[7:17]
+    assert is_uid(docker_id)
+    return docker_id[7:17] if docker_id.startswith("sha256:") else docker_id[:10]
 
 
-def age_str(age: Optional[int]) -> str:
+def age_str(now: Union[int,datetime], age: Union[int,datetime,None]) -> str:
     """Turn a number of seconds into something human readable"""
     if age is None:
-        return "Unknown"
-    return str(timedelta(seconds=int(age.total_seconds() if isinstance(age, timedelta) else age)))
+        return "--"
+    tds = int((now.timestamp() if isinstance(now, datetime) else now)-(age.timestamp() if isinstance(age, datetime) else age))
+    return (
+        f"{tds//86400:02d}d"
+        f":{tds//3600%24:02d}h"
+        f":{tds//60%60:02d}m"
+    )
 
 
 def date_str(date: datetime) -> str:
     if not date:
         return "--"
     return (datetime.fromtimestamp(date) if isinstance(date, int) else date).strftime(
         "%Y.%m.%d-%H:%M:%S"
     )
 
 
-from dateutil import tz
+def date_from(timestamp: str) -> datetime:
+    try:
+        if isinstance(timestamp, int):
+            return datetime.fromtimestamp(timestamp)
 
+        if timestamp[-1] == "Z":
+            return (
+                datetime.strptime(timestamp[:19], "%Y-%m-%dT%H:%M:%S")
+                .replace(tzinfo=tz.tzutc())
+                .astimezone(tz.tzlocal())
+            )
+    except OverflowError:
+        return None
+    except Exception as exc:
+        raise ValueError(f"Could not parse datetime from <{timestamp!r}> ({exc})")
 
-def date_from(timestamp: str) -> datetime:
-    if isinstance(timestamp, int):
-        datetime.fromtimestamp(timestamp)
 
-    if timestamp[-1] == "Z":
-        return (
-            datetime.strptime(timestamp[:19], "%Y-%m-%dT%H:%M:%S")
-            .replace(tzinfo=tz.tzutc())
-            .astimezone(tz.tzlocal())
+@impatient
+def id_from(name: str) -> Optional[str]:
+    """Looks up name using `docker inspect` and returns a 10 digit Docker ID"""
+    with suppress(CalledProcessError):
+        log().debug("resolve %s", name)
+        return short_id(
+            name
+            if name.startswith("sha256:")
+            else process_output(f"docker inspect --format='{{{{.Id}}}}' {name}")
         )
+    return None
 
-    return f"BAD: {timestamp}"
+
+def lookup_id(ids: MutableMapping[str, Optional[str]], name: str) -> Optional[str]:
+    """Looks up a given @name in @ids and resolves it first if not yet given"""
+    if name not in ids:
+        ids[name] = id_from(name)
+    return ids[name]
 
 
 def event_from(line: str):
     """Reads a line from event log and turns it into a tuple containing the data"""
     match = re.match(r"^(.*) \((.*)\)$", line)
     assert match, f"line did not match the expected format: {line!r}"
     cmd, params = match.groups()
@@ -138,50 +203,116 @@
         operator,
         cmd,
         uid,
         dict(p.split("=") for p in params.split(", ")),
     )
 
 
-def id_from(name: str) -> Optional[str]:
-    """Looks up name using `docker inspect` and returns a 12 digit Docker ID"""
-    with suppress(CalledProcessError):
-        log().debug("resolve %s", name)
-        return short_id(
-            name
-            if name.startswith("sha256:")
-            else process_output(f"docker inspect --format='{{{{.Id}}}}' {name}")
+async def handle_docker_event_line(docker_client, global_state, line):
+    """Read a `docker events` line and maintain the last-used information"""
+
+    tstamp, object_type, operator, _cmd, uid, params = event_from(line)
+
+    if (object_type, operator) in {
+        ("image", "tag"),
+        ("image", "pull"),
+        ("container", "create"),
+    }:
+        ident = params.get("image") or params["name"]
+        log().info(
+            "docker event %s %s %s ident=%s _uid=%s",
+            datetime.fromtimestamp(tstamp),
+            object_type,
+            operator,
+            ident,
+            uid,
         )
-    return None
+    elif object_type in {"network", "builder"}:
+        return
+    elif (object_type, operator) in {
+        ("image", "untag"),
+        ("image", "prune"),
+        ("image", "delete"),
+        ("container", "attach"),
+        ("container", "start"),
+        ("container", "die"),
+        ("container", "destroy"),
+        ("container", "prune"),
+        ("network", "connect"),
+        ("network", "disconnect"),
+    }:
+        return
+    else:
+        log().warning("unknown type/operator %s  %s", object_type, operator)
+        return
 
+    # log().debug("handle docker event %s", (tstamp, _uid[:12], operator, params["image"]))
+    #if not (referenced_image_id := lookup_id(global_state.image_ids, ident)):
+    #    return
+
+    # print(ident, uid)
+    # print(await docker_client.images.get(ident))
+    # print(await docker_client.containers.get(uid))
 
-def lookup_id(ids: MutableMapping[str, Optional[str]], name: str) -> Optional[str]:
-    """Looks up a given @name in @ids and resolves it first if not yet given"""
-    if name not in ids:
-        ids[name] = id_from(name)
-    return ids[name]
+    global_state.event_horizon = min(global_state.event_horizon, tstamp)
 
+    register_reference(ident, tstamp, global_state)
 
-async def handle_docker_event_line(global_state, line):
-    """Read a `docker events` line and maintain the last-used information"""
+def is_uid(ident:str) -> bool:
+    """
+    sha256:48a3535fe27fea1ac6c2f41547770d081552c54b2391c2dda99e2ad87561a4f2
+    48a3535fe27fea1ac6c2f41547770d081552c54b2391c2dda99e2ad87561a4f2
+    48a3535fe27f
+    """
+    return ident.startswith("sha256:") or re.match("[0-9a-f]{64}", ident) or re.match("[0-9a-f]{10}", ident)
 
-    tstamp, object_type, operator, _cmd, _uid, params = event_from(line)
-    if not object_type == "container" or operator == "prune":
-        return
-    # log().debug("docker event: %s", line)
-    log().debug("handle docker event %s", (tstamp, _uid[:12], operator, params["image"]))
-    if not (referenced_image_id := lookup_id(global_state.image_ids, params["image"])):
-        return
 
-    #    print(tstamp, object_type, operator, _cmd, _uid, params)
+def register_reference(ident: str, timestamp: int, global_state) -> None:
+    effective_ident = short_id(ident) if (is_uid_ := is_uid(ident)) else ident
+    if effective_ident not in global_state.last_referenced:
+        global_state.last_referenced[effective_ident] = [
+            0,
+            global_state.expiration_ages["tag_unknown"] if is_uid_ else expiration_age_from_rules(effective_ident, global_state)
+        ]
+
+    # increase last reference date if applicable
+    global_state.last_referenced[effective_ident][0] = max(
+        global_state.last_referenced[effective_ident][0], timestamp
+    )
 
-    global_state.event_horizon = min(global_state.event_horizon, tstamp)
-    global_state.last_referenced[referenced_image_id] = max(
-        global_state.last_referenced.setdefault(referenced_image_id, tstamp), tstamp
+
+def expiration_age_from_rules(ident: str, global_state: GlobalState) -> int:
+    if is_uid(ident):
+        log().error("expiration_age_from_rules %s", ident)
+    matching_rules = tuple((regex, age) for regex, age in global_state.tag_rules.items() if re.match(regex, ident))
+    if len(matching_rules) == 1:
+        return matching_rules[0][1]
+    if not matching_rules:
+        log().warn("No rule found for %s", ident)
+    else:
+        log().error("Multiple rules found for %s:", ident)
+        for rule in matching_rules:
+            log().error("  %s:", rule[0])
+    return global_state.expiration_ages["tag_unknown"]
+
+
+@impatient
+def expired(ident: str, global_state, now: int, extra_date: int = 0) -> bool:
+    if ident not in global_state.last_referenced:
+        log().warn("no reference: %s", ident)
+    else:
+        breakpoint
+    # TODO
+    last_referenced, expiration_age = global_state.last_referenced.get(ident, [None, global_state.expiration_ages["tag_unknown"]])
+    effective_age = now - max(
+        last_referenced or 0,
+        global_state.event_horizon,
+        extra_date,
     )
+    return effective_age > expiration_age, last_referenced, expiration_age
 
 
 def jobname_from(binds):
     candidates = [
         d.replace("/home/jenkins/workspace/", "").replace("/checkout", "")
         for b in binds or []
         for d in (b.split(":")[0],)
@@ -220,14 +351,15 @@
             "org.tribe29.cmk_version",
         )
         for w in l.split()
         if not (w.startswith("sha256") or len(w) == 64)
     )
 
 
+@aimpatient
 async def dump_global_state(global_state):
     global_state.counter += 1
     print(global_state.intervals)
     print(f"counter: {global_state.counter}")
     print(f"images: {len(global_state.images)}")
     print(f"containers: {len(global_state.containers)}")
     print(f"tag_rules: {len(global_state.tag_rules)}")
@@ -241,74 +373,80 @@
         super().__init__(items)
         self.endpoint = endpoint
 
     def get_tr_attrs(self, item):
         return {"class": item.get("class")}
 
 
+class PlainCol(Col):
+    def td_format(self, content):
+        return f"<tt><b>{content}</b></tt>"
+
+
 class ImageTable(BaseTable):
-    short_id = Col("short_id")
-    tags = Col("tags")
-    created_at = Col("created_at")
-    last_referenced = Col("last_referenced")
+    short_id = PlainCol("short_id")
+    tags = PlainCol("tags")
+    created_at = PlainCol("created_at")
 
     def sort_url(self, col_key, reverse=False):
         return url_for(
             self.endpoint,
             sort_key_images=col_key,
             sort_direction_images="desc" if reverse else "asc",
         )
 
     @staticmethod
     def html_from(endpoint, global_state, sort, reverse):
-        # - max(
-        # referenced.get(image_id, 0),
-        # GLOBALS["EVENT_HORIZON"],
-        # datetime.strptime(
-        # docker_images.get(image_id).attrs["Created"][:19], "%Y-%m-%dT%H:%M:%S"
-        # ).timestamp(),
-        # ),
-        def last_referenced_str(image_id):
-            if ref := global_state.last_referenced.get(image_id):
-                return age_str(time.time() - ref)
-            return "??"
+        now = datetime.now(tz=tz.tzutc())
+
+        def dict_from(image):
+            now_timestamp = now.timestamp()
+            created_timestamp = date_from(image["created_at"]).timestamp()
+
+            def coloured_ident(ident):
+                is_expired, last_referenced, expiration_age = expired(ident, global_state, now_timestamp, created_timestamp)
+                if is_expired:
+                    return f"<div class='text-danger'>{ident} ({age_str(now, last_referenced)})</div>"
+                return f"<div class='text-success'>{ident} ({age_str(now, last_referenced)})</div>"
+
+            return {
+                "short_id": coloured_ident(image["short_id"]),
+                "tags": "".join(map(coloured_ident, image["tags"])),
+                "created_at": date_str(image["created_at"]),
+                "age": age_str(now, date_from(image["created_at"])),
+                #"last_referenced": last_referenced_str(image["short_id"]),
+                # "class": "text-danger" if would_cleanup_image(image, now, global_state) else "text-success",
+            }
 
         return ImageTable(
             endpoint,
             items=sorted(
-                (
-                    {
-                        "short_id": image["short_id"],
-                        "tags": image["tags"],
-                        "created_at": date_str(image["created_at"]),
-                        "age": age_str(datetime.now() - date_from(image["created_at"])),
-                        "last_referenced": last_referenced_str(image["short_id"]),
-                        "class": "text-danger" if image.get("cleanup") else "text-success",
-                    }
-                    for image in global_state.images.values()
-                ),
+                map(dict_from, global_state.images.values()),
                 key=lambda e: e[sort],
                 reverse=reverse,
             ),
         ).__html__()
 
 
 class ContainerTable(BaseTable):
-    short_id = Col("short_id")
-    name = Col("name")
-    mem_usage = Col("mem_usage")
-    cpu = Col("cpu")
-    cmd = Col("cmd")
-    job = Col("job")
-    # created_at = Col("created_at")
-    started_at = Col("started_at")
-    uptime = Col("uptime")
-    status = Col("status")
-    hints = Col("hints")
-    pid = Col("pid")
+    short_id = PlainCol("short_id")
+    name = PlainCol("name")
+    image = PlainCol("image")
+
+    status = PlainCol("status")
+    created_at = PlainCol("created_at")
+    started_at = PlainCol("started_at")
+    uptime = PlainCol("uptime")
+    pid = PlainCol("pid")
+    mem_usage = PlainCol("mem_usage")
+    cpu = PlainCol("cpu")
+    cmd = PlainCol("cmd")
+
+    job = PlainCol("job")
+    hints = PlainCol("hints")
     # link = LinkCol('Link', 'route_containers', url_kwargs=dict(id='id'), allow_sort=False)
 
     def sort_url(self, col_key, reverse=False):
         return url_for(
             self.endpoint,
             sort_key_containers=col_key,
             sort_direction_containers="desc" if reverse else "asc",
@@ -320,32 +458,34 @@
         return ContainerTable(
             endpoint,
             items=sorted(
                 (
                     {
                         "short_id": cnt["short_id"],
                         "name": cnt["name"],
+                        "image": short_id(cnt["image"]) if is_uid(cnt["image"]) else cnt["image"],
                         "mem_usage": mem_stats.get("usage", 0),
                         "cpu": cpu_perc(cpu_stats, last_cpu_stats),
-                        "cmd": " ".join(cnt["show"]["Config"]["Cmd"]),
+                        "cmd": " ".join(cnt["show"]["Config"]["Cmd"])[:100],
                         "job": jobname_from(
                             cnt["show"]["HostConfig"]["Binds"]
                             or list(cnt["show"]["Config"]["Volumes"] or [])
                         ),
-                        # "created_at": date_str(date_from(cnt["show"]["Created"])),
-                        # "created_at": cnt["show"]["Created"],
+                        "created_at": date_str(date_from(cnt["show"]["Created"])),
                         "started_at": date_str(
                             started_at := date_from(cnt["show"]["State"]["StartedAt"])
                         ),
-                        "uptime": age_str(now - started_at) if started_at else "--",
+                        "uptime": age_str(now, started_at),
                         "status": cnt["show"]["State"]["Status"],
                         "hints": label_filter(cnt["show"]["Config"]["Labels"]),
                         "pid": int(cnt["show"]["State"]["Pid"]),
                         # https://getbootstrap.com/docs/4.0/utilities/colors/
-                        "class": "text-danger" if cnt.get("cleanup") else "text-success",
+                        "class": "text-danger"
+                        if would_cleanup_container(cnt, now.timestamp(), global_state)
+                        else "text-success",
                     }
                     for cnt, mem_stats, cpu_stats, last_cpu_stats in (
                         (
                             c,
                             c["stats"].get("memory_stats", {}),
                             c["stats"]["cpu_stats"],
                             c["last_stats"].get("cpu_stats"),
@@ -359,69 +499,77 @@
             ),
         ).__html__()
 
 
 def meta_info(global_state):
     return {
         "refresh_interval": global_state.intervals.get("site_refresh", 10),
-        "event_horizon": age_str(int(time.time() - global_state.event_horizon)),
+        "event_horizon": age_str(time.time(), global_state.event_horizon),
         "container_count": len(global_state.containers),
         "image_count": len(global_state.images),
         "extra_links": global_state.extra_links,
         "intervals": global_state.intervals,
+        "hostname": global_state.hostname,
+        "switches": global_state.switches,
+        "expiration_ages": global_state.expiration_ages,
     }
 
 
+@aimpatient
 async def container_table_html(global_state):
     # https://github.com/plumdog/flask_table/blob/master/examples/sortable.py
     return await render_template(
         "containers.html",
         meta=meta_info(global_state),
         containers_html=ContainerTable.html_from(
             "route_containers",
             global_state,
             sort=request.args.get("sort_key_containers", "cpu"),
             reverse=request.args.get("sort_direction_containers", "asc") == "desc",
         ),
     )
 
 
+@aimpatient
 async def image_table_html(global_state):
     # https://github.com/plumdog/flask_table/blob/master/examples/sortable.py
     return await render_template(
         "containers.html",
         meta=meta_info(global_state),
         images_html=ImageTable.html_from(
             "route_images",
             global_state,
-            sort=request.args.get("sort_key_images", "last_referenced"),
+            sort=request.args.get("sort_key_images", "created_at"),
             reverse=request.args.get("sort_direction_images", "asc") == "desc",
         ),
     )
 
 
+@aimpatient
 async def dashboard(global_state):
     return await render_template(
         "dashboard.html",
         meta=meta_info(global_state),
         containers_html=ContainerTable.html_from(
             "route_dashboard",
             global_state,
             sort=request.args.get("sort_key_containers", "cpu"),
             reverse=request.args.get("sort_direction_containers", "asc") == "desc",
         ),
         images_html=ImageTable.html_from(
             "route_dashboard",
             global_state,
-            sort=request.args.get("sort_key_images", "last_referenced"),
+            sort=request.args.get("sort_key_images", "created_at"),
             reverse=request.args.get("sort_direction_images", "asc") == "desc",
         ),
+        messages=global_state.messages,
     )
 
 
+@aimpatient
 async def print_container_stats(global_state):
     hostname = open("/etc/hostname").read().strip()
     stats = [
         {
             "short_id": cnt["short_id"],
             "name": cnt["name"],
             "usage": mem_stats.get("usage", 0),
@@ -499,75 +647,148 @@
         f" {'':>9}"
         f" {'':<60}"
         f" {''}"
     )
 
 
 @watchdog
-async def watch_container(container, containers):
+async def watch_container(container, global_state: GlobalState):
     name = "unknown"
+    containers = global_state.containers
     try:
-        containers[container.id]["container"] = container
-        containers[container.id]["short_id"] = (short_id := container.id[:12])
-        containers[container.id]["show"] = await container.show()
-        containers[container.id]["name"] = (name := containers[container.id]["show"]["Name"][1:])
-        log().info(">> new container: %s %s", short_id, name)
+        container_info = containers[container.id]
+        container_info["container"] = container
+        container_info["short_id"] = (short_id_ := short_id(container.id))
+        container_info["show"] = (show := await container.show())
+        container_info["name"] = (name := show["Name"][1:])
+        container_info["image"] = (image := show["Config"]["Image"])
+
+        # wrong - other things could have happened since..
+        # register_reference(image, date_from(show["Created"]).timestamp(), global_state)
+
+        log().info(">> new container: %s %s", short_id_, name)
+
         async for stats in container.stats():
-            containers[container.id]["last_stats"] = containers[container.id].get("stats", {})
-            containers[container.id]["stats"] = stats
-            containers[container.id]["show"] = await container.show()
+            container_info["last_stats"] = container_info.get("stats", {})
+            container_info["stats"] = stats
+            container_info["show"] = await container.show()
+
     except DockerError as exc:
         log().error("DockerError: %s", exc)
     finally:
-        log().info("<< container terminated: %s %s", short_id, name)
+        log().info("<< container terminated: %s %s", short_id_, name)
         del containers[container.id]
 
 
+# @aimpatient
 async def watch_images(docker_client, global_state):
     # TODO: also use events to register
     log().info("crawl images..")
     for image in await docker_client.images.list(all=True):
-        log().debug(image)
+        # log().debug("  found image %s", image["Id"])
         if True or image["Id"] not in global_state.images:
-            global_state.images.get(image["Id"], {}).update(
+            global_state.images.setdefault(image["Id"], {}).update(
                 {
+                    # TODO: name (also for registration)
                     "short_id": short_id(image["Id"]),
+                    "name": image["Id"],
                     "created_at": image["Created"],
                     "tags": image["RepoTags"],
                     "size": image["Size"],
                     "parent": short_id(image["ParentId"]),
                 }
             )
 
 
+@aimpatient
 async def watch_containers(docker_client, global_state):
     # TODO: also use events to register
     log().info("crawl containers..")
     for container in await docker_client.containers.list(all=True):
+        log().debug("  found container %s", container.id)
         if container.id not in global_state.containers:
             global_state.containers[container.id] = {}
-            asyncio.ensure_future(watch_container(container, global_state.containers))
 
+            asyncio.ensure_future(watch_container(container, global_state))
 
-def would_cleanup_container(container, global_state):
-    status = container["show"]["State"]["Status"]
-    if status in {"exited"}:
-        return True
 
+@impatient
+def would_cleanup_container(container, now: int, global_state):
+    if "show" not in container:
+        return False
+    status = (show := container["show"])["State"]["Status"]
+    if status == "exited":
+        return (
+            now - date_from(show["State"]["FinishedAt"]).timestamp()
+            > global_state.expiration_ages["container_exited"]
+        )
+    if status == "created":
+        return (
+            now - date_from(show["Created"]).timestamp()
+            > global_state.expiration_ages["container_created"]
+        )
+    if status == "running":
+        return (
+            now - date_from(show["State"]["StartedAt"]).timestamp()
+            > global_state.expiration_ages["container_running"]
+        )
     return False
 
 
-def would_cleanup_image(image, global_state):
-    print(image)
-    return False
+@impatient
+def image_expired(image, now: datetime, global_state):
+    created_timestamp = int(date_from(image["created_at"]).timestamp())
+    return expired(image["short_id"], global_state, now, created_timestamp) and all(
+        expired(tag, global_state, now, created_timestamp) for tag in image["tags"]
+    )
 
 
-async def cleanup(global_state):
+@aimpatient
+async def cleanup(docker_client: Docker, global_state):
     log().info("Cleanup!..")
+    now = int(datetime.now().timestamp())
 
-    for container in global_state.containers.values():
-        container["cleanup"] = would_cleanup_container(container, global_state)
+    # we could go through docker_client.containers, too, but to be more consistent, we work
+    # on one structure only
+    # also, we have to create a list we can operate on, in order to not modify the structure, we're
+    # iterating
+    for container_info in list(
+        filter(
+            lambda cnt: would_cleanup_container(cnt, now, global_state),
+            global_state.containers.values(),
+        )
+    ):
+        if not global_state.switches.get("remove_container"):
+            log().info(f"skip removal of container {container_info['short_id']}")
+            continue
+        report(
+            global_state,
+            "warn",
+            f"force removing container {container_info['short_id']}",
+            container_info["container"],
+        )
+        await container_info["container"].delete(force=True, v=True)
 
-    for image in global_state.images.values():
-        image["cleanup"] = would_cleanup_image(image, global_state)
+    for image_info in list(
+        filter(lambda image: image_expired(image, now, global_state), global_state.images.values())
+    ):
+        if not global_state.switches.get("remove_images"):
+            log().info(f"skip removal of image {image_info['short_id']}")
+            continue
+        report(global_state, "info", f"try to remove image {image_info['short_id']}", image_info)
+        # image["cleanup"] =
 
     log().info("Cleanup done!")
+
+
+@impatient
+def report(global_state, msg_type, message: str, extra):
+    # TODO: cleanup
+    # TODO: persist
+    log().info(message)
+    global_state.messages.insert(0, (datetime.now().timestamp(), msg_type, message, str(extra)))
+
+
+@impatient
+def reconfigure(global_state: GlobalState) -> None:
+    for ident, reference in global_state.last_referenced.items():
+        reference[1] = expiration_age_from_rules(ident, global_state)
```

### Comparing `docker_shaper-0.1.5/docker_shaper/server.py` & `docker_shaper-0.1.6/docker_shaper/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 #!/usr/bin/env python3
 
 import asyncio
 import importlib
 import logging
 import time
 from contextlib import suppress
-from dataclasses import dataclass
 from importlib.machinery import SourceFileLoader
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
-from typing import MutableMapping
 
 from aiodocker import Docker
 from quart import Quart
 
 from docker_shaper import dynamic
 from docker_shaper.utils import fs_changes, read_process_output, watchdog
 
@@ -21,49 +19,14 @@
 
 
 def log() -> logging.Logger:
     """Logger for this module"""
     return logging.getLogger("docker-shaper.server")
 
 
-@dataclass
-class GlobalState:
-    intervals: MutableMapping[str, float]
-
-    image_ids: MutableMapping[str, object]
-
-    images: MutableMapping[str, object]
-    containers: MutableMapping[str, object]
-
-    event_horizon: int
-    last_referenced: MutableMapping[str, int]
-
-    tag_rules: MutableMapping[str, int]
-
-    extra_links: MutableMapping[str, int]
-
-    def __init__(self):
-        self.intervals = {
-            "state": 2,
-            "image_stats": 2,
-            "image_update": 2,
-            "container_update": 2,
-            "container_stats": 2,
-            "cleanup": 3600,
-        }
-        self.image_ids = {}
-        self.images = {}
-        self.containers = {}
-        self.event_horizon = int(time.time())
-        self.last_referenced = {}
-        self.tag_rules = {}
-        self.counter = 0
-        self.extra_links = {}
-
-
 @watchdog
 async def print_container_stats(global_state):
     while True:
         try:
             await dynamic.print_container_stats(global_state)
             await asyncio.sleep(global_state.intervals.get("container_stats"), 1)
         except Exception:
@@ -122,14 +85,15 @@
     print(module)
     # assert module
     # assert isinstance(spec.loader, SourceFileLoader)
     loader: SourceFileLoader = spec.loader
     loader.exec_module(module)
     try:
         module.modify(global_state)
+        dynamic.reconfigure(global_state)
     except AttributeError:
         log().warning("File %s does not provide a `modify(global_state)` function")
 
 
 @watchdog
 async def watch_fs_changes(global_state):
     CONFIG_FILE.parent.mkdir(parents=True, exist_ok=True)
@@ -147,35 +111,43 @@
             log().exception("Reloading dynamic part failed!")
             await asyncio.sleep(5)
     assert False
 
 
 @watchdog
 async def handle_docker_events(global_state):
-    async for line in read_process_output("docker events"):
-        try:
-            await dynamic.handle_docker_event_line(global_state, line)
-        except Exception:
-            log().exception("Unhandled exception caught!")
-            await asyncio.sleep(5)
+    try:
+        docker = Docker()
+        async for line in read_process_output("docker events"):
+            try:
+                await dynamic.handle_docker_event_line(docker, global_state, line)
+            except Exception:
+                log().exception("Unhandled exception caught!")
+                await asyncio.sleep(5)
+    finally:
+        await docker.close()
 
 
 @watchdog
 async def cleanup(global_state):
-    while True:
-        try:
-            await dynamic.cleanup(global_state)
-            await asyncio.sleep(global_state.intervals.get("cleanup", 3600))
-        except Exception:
-            log().exception("Unhandled exception caught in cleanup()!")
-            await asyncio.sleep(5)
+    try:
+        docker = Docker()
+        while True:
+            try:
+                await dynamic.cleanup(docker, global_state)
+                await asyncio.sleep(global_state.intervals.get("cleanup", 3600))
+            except Exception:
+                log().exception("Unhandled exception caught in cleanup()!")
+                await asyncio.sleep(5)
+    finally:
+        await docker.close()
 
 
 def no_serve():
-    global_state = GlobalState()
+    global_state = dynamic.GlobalState()
     load_config(CONFIG_FILE, global_state)
     with suppress(KeyboardInterrupt, BrokenPipeError):
         asyncio.ensure_future(watch_fs_changes(global_state))
         asyncio.ensure_future(print_container_stats(global_state))
         asyncio.ensure_future(print_state(global_state))
         asyncio.ensure_future(watch_containers(global_state))
         asyncio.ensure_future(watch_images(global_state))
@@ -185,15 +157,15 @@
 
 
 def serve():
     """"""
     app = Quart(__name__)
     app.config["TEMPLATES_AUTO_RELOAD"] = True
 
-    global_state = GlobalState()
+    global_state = dynamic.GlobalState()
     load_config(CONFIG_FILE, global_state)
 
     @watchdog
     async def self_destroy():
         await app.terminator.wait()
         print("BOOM")
         app.shutdown()
```

### Comparing `docker_shaper-0.1.5/docker_shaper/static/bootstrap.css` & `docker_shaper-0.1.6/docker_shaper/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.5/docker_shaper/static/normalize.css` & `docker_shaper-0.1.6/docker_shaper/static/normalize.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.5/docker_shaper/static/pills.css` & `docker_shaper-0.1.6/docker_shaper/static/pills.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.5/docker_shaper/static/style.css` & `docker_shaper-0.1.6/docker_shaper/static/style.css`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.5/docker_shaper/templates/base.html` & `docker_shaper-0.1.6/docker_shaper/templates/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,26 @@
     -->
     <link rel="stylesheet" href="{{ url_for('static', filename='bootstrap.css') }}">
     <meta http-equiv="refresh" content="{{ meta.refresh_interval }}" />
   </head>
 
   <body>
      <table class="table table-striped"><tr>
-      <td>Host: --</td>
+      <td>Host: <b>{{meta.hostname}}</b></td>
       <td></td>
       {% for link in meta.extra_links %}
           <td><a href="{{ meta.extra_links[link] }}">{{link}}</a></td>
           <td></td>
       {% endfor %}
 
     </tr><tr>
+      <td>intervals:</td>
 
       {% for interval in meta.intervals %}
-          <td>{{interval}} = {{meta.intervals[interval]}}s  </td><td></td>
+          <td>{{interval}} = <b>{{meta.intervals[interval]}}s</b>  </td><td></td>
       {% endfor %}
 
     </tr><tr>
 
       <td><a href="/">Dashboard</a></td>
       <td></td>
       <td><a href="/containers">Containers</a></td>
@@ -35,11 +36,9 @@
 
     </tr></table>
 
     <div class="dashboard">
       {% block content %}{% endblock %}
     </div>
 
-    {% block scripts %}{% endblock %}
-
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 
 
-Host: --                                      {{link}}
-{{interval}} = {{meta.intervals[interval]}}s
-Dashboard                                     Containers  Images
+Host: {{meta.hostname}}                                 {{link}}
+intervals:              {{interval}} = {{meta.intervals
+                        [interval]}}s
+Dashboard                                               Containers  Images
 {% block content %}{% endblock %}
-{% block scripts %}{% endblock %}
```

### Comparing `docker_shaper-0.1.5/docker_shaper/utils.py` & `docker_shaper-0.1.6/docker_shaper/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """Common stuff shared among modules"""
 
 import asyncio
 import logging
 import os
 import shlex
+import time
 from functools import wraps
 from pathlib import Path
 from subprocess import DEVNULL, CalledProcessError, check_output, run
 
 # we need 3.8 compatible typing (python on build nodes)
 from typing import Callable, Coroutine, Iterator, Union, cast
 
@@ -59,14 +60,42 @@
             log().exception("Exception in `%s`:", afunc.__name__)
             asyncio.get_event_loop().stop()
         return None
 
     return run
 
 
+def impatient(func):
+    @wraps(func)
+    def run(*args: object, **kwargs: object) -> object:
+        try:
+            t1 = time.time()
+            return func(*args, **kwargs)
+        finally:
+            if (duration := time.time() - t1) > 0.1:
+                log().warn("%s took %.2fs!", func.__name__, duration)
+            # log().info("%s took %.2fs!", func.__name__, duration)
+
+    return run
+
+
+def aimpatient(func):
+    @wraps(func)
+    async def run(*args: object, **kwargs: object) -> object:
+        try:
+            t1 = time.time()
+            return await func(*args, **kwargs)
+        finally:
+            if (duration := time.time() - t1) > 0.1:
+                log().warn("%s took %.2fs!", func.__name__, duration)
+            # log().info("%s took %.2fs!", func.__name__, duration)
+
+    return run
+
+
 async def fs_changes(
     *paths: Path,
     queue: asyncio.Queue = asyncio.Queue(),
     mask: Mask = Mask.CLOSE_WRITE | Mask.MOVED_TO | Mask.CREATE,
     postpone: bool = False,
     timeout: float = 2,
 ) -> Iterator[Path]:
```

### Comparing `docker_shaper-0.1.5/pyproject.toml` & `docker_shaper-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-shaper"
-version = "0.1.5"
+version = "0.1.6"
 description = "Keeps Docker resources in shape based on rules and usage"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/Checkmk/checkmk-dev-tools"
 readme = "Readme.md"
 packages = [
   {include = "docker_shaper/**/*.py"},
   {include = "docker_shaper/static"},
```

### Comparing `docker_shaper-0.1.5/PKG-INFO` & `docker_shaper-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-shaper
-Version: 0.1.5
+Version: 0.1.6
 Summary: Keeps Docker resources in shape based on rules and usage
 Home-page: https://github.com/Checkmk/checkmk-dev-tools
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -96,14 +96,15 @@
   - check installed package
   - go through review process
   - publish the new package `poetry publish --build --repository checkmk`
   - commit new version && push
 
 
 ## Knowledge
-https://github.com/torfsen/python-systemd-tutorial
-https://www.digitalocean.com/community/tutorials/how-to-use-templates-in-a-flask-application
-* https://blog.miguelgrinberg.com/post/beautiful-interactive-tables-for-your-flask-templates
+* [Showing Text Box On Hover (In Table)](https://stackoverflow.com/questions/52562345/showing-text-box-on-hover-in-table)
+* [Beautiful Interactive Tables for your Flask Templates](https://blog.miguelgrinberg.com/post/beautiful-interactive-tables-for-your-flask-templates)
+* https://github.com/torfsen/python-systemd-tutorial
+* https://www.digitalocean.com/community/tutorials/how-to-use-templates-in-a-flask-application
 * https://stackoverflow.com/questions/49957034/live-updating-dynamic-variable-on-html-with-flask
 * https://pgjones.gitlab.io/quart/how_to_guides/templating.html
```

