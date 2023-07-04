# Comparing `tmp/compose_chart_export-0.0.21-py3-none-any.whl.zip` & `tmp/compose_chart_export-0.0.22rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13383 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 08:46 compose_chart_export/__init__.py
--rw-r--r--  2.0 unx     2517 b- defN 23-Jul-03 08:46 compose_chart_export/chart_export.py
--rw-r--r--  2.0 unx    14564 b- defN 23-Jul-03 08:46 compose_chart_export/chart_file_templates.py
--rw-r--r--  2.0 unx     4974 b- defN 23-Jul-03 08:46 compose_chart_export/chart_mods.py
--rw-r--r--  2.0 unx     2285 b- defN 23-Jul-03 08:46 compose_chart_export/chart_read.py
--rw-r--r--  2.0 unx     9602 b- defN 23-Jul-03 08:46 compose_chart_export/compose_export.py
--rw-r--r--  2.0 unx     2365 b- defN 23-Jul-03 08:46 compose_chart_export/ports.py
--rw-r--r--  2.0 unx      191 b- defN 23-Jul-03 08:46 compose_chart_export/settings.py
--rw-r--r--  2.0 unx      626 b- defN 23-Jul-03 08:46 compose_chart_export-0.0.21.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 08:46 compose_chart_export-0.0.21.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-03 08:46 compose_chart_export-0.0.21.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Jul-03 08:46 compose_chart_export-0.0.21.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1199 b- defN 23-Jul-03 08:46 compose_chart_export-0.0.21.dist-info/RECORD
-13 files, 38437 bytes uncompressed, 11327 bytes compressed:  70.5%
+Zip file size: 13490 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 15:26 compose_chart_export/__init__.py
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jul-04 15:26 compose_chart_export/chart_export.py
+-rw-r--r--  2.0 unx    14564 b- defN 23-Jul-04 15:26 compose_chart_export/chart_file_templates.py
+-rw-r--r--  2.0 unx     4974 b- defN 23-Jul-04 15:26 compose_chart_export/chart_mods.py
+-rw-r--r--  2.0 unx     2285 b- defN 23-Jul-04 15:26 compose_chart_export/chart_read.py
+-rw-r--r--  2.0 unx     9945 b- defN 23-Jul-04 15:26 compose_chart_export/compose_export.py
+-rw-r--r--  2.0 unx     2365 b- defN 23-Jul-04 15:26 compose_chart_export/ports.py
+-rw-r--r--  2.0 unx      191 b- defN 23-Jul-04 15:26 compose_chart_export/settings.py
+-rw-r--r--  2.0 unx      629 b- defN 23-Jul-04 15:26 compose_chart_export-0.0.22rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 15:26 compose_chart_export-0.0.22rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-04 15:26 compose_chart_export-0.0.22rc1.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-04 15:26 compose_chart_export-0.0.22rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1214 b- defN 23-Jul-04 15:26 compose_chart_export-0.0.22rc1.dist-info/RECORD
+13 files, 38798 bytes uncompressed, 11404 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: compose_chart_export/ports.py
 Comment: 
 
 Filename: compose_chart_export/settings.py
 Comment: 
 
-Filename: compose_chart_export-0.0.21.dist-info/METADATA
+Filename: compose_chart_export-0.0.22rc1.dist-info/METADATA
 Comment: 
 
-Filename: compose_chart_export-0.0.21.dist-info/WHEEL
+Filename: compose_chart_export-0.0.22rc1.dist-info/WHEEL
 Comment: 
 
-Filename: compose_chart_export-0.0.21.dist-info/namespace_packages.txt
+Filename: compose_chart_export-0.0.22rc1.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.21.dist-info/top_level.txt
+Filename: compose_chart_export-0.0.22rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.21.dist-info/RECORD
+Filename: compose_chart_export-0.0.22rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## compose_chart_export/compose_export.py

```diff
@@ -83,33 +83,38 @@
 class ExtraContainer(BaseModel):
     name: kubernetes_label_regex
     env: dict[str, str]
     command: list[str]
 
 
 def parse_service_name_extra_containers(
-    compose_path: Path,
+    compose_path: Path, chart_name: str
 ) -> tuple[str, list[ExtraContainer]]:
     extra_containers = []
     service_names = []
-    service_names_with_chart_name = []
+    chart_name_service_name = {}
     for each_service_name, info in iter_compose_info(compose_path):
         if info.labels.get("extra_container") == "true":
             container_name = each_service_name.replace("_", "-")
             extra_containers.append(
                 ExtraContainer(
                     name=container_name, env=info.default_env, command=info.command
                 )
             )
-        elif parse_chart_name(info.labels):
-            service_names_with_chart_name.append(each_service_name)
+        elif service_chart_name := parse_chart_name(info.labels):
+            chart_name_service_name[service_chart_name] = each_service_name
         else:
             service_names.append(each_service_name)
-    if service_names_with_chart_name:
-        service_names = service_names_with_chart_name
+    if chart_name and chart_name_service_name:
+        found_service = chart_name_service_name.get(chart_name)
+        if not found_service:
+            raise ValueError(f"chart name: {chart_name} not found in {compose_path}")
+        return found_service, extra_containers
+    if chart_name_service_name:
+        service_names = list(chart_name_service_name.values())
     if not service_names:
         raise ValueError(f"No main service name found in {compose_path}")
     if len(service_names) > 1:
         raise ValueError(
             f"Possibly more than 1 service as the main service: {service_names}, {compose_path}"
         )
     return service_names[0], extra_containers
@@ -143,15 +148,17 @@
     chart_name: str = "",
     image_url: str = "unset",
     on_exported: Callable[[Path], None] | None = None,
     use_chart_name_as_container_name: bool = True,
 ):
     chart_version = ensure_chart_version_valid(chart_version)
     compose_path = Path(compose_path)
-    service_name, extra_containers = parse_service_name_extra_containers(compose_path)
+    service_name, extra_containers = parse_service_name_extra_containers(
+        compose_path, chart_name
+    )
     info = read_compose_info(compose_path, service_name)
     env = info.default_env
     compose_labels = info.labels
     chart_name = chart_name or parse_chart_name(compose_labels)
     prefix_ports = parse_container_ports(compose_labels, info.host_container_ports)
     container_name = (
         chart_name.replace("_", "-")
```

## Comparing `compose_chart_export-0.0.21.dist-info/METADATA` & `compose_chart_export-0.0.22rc1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose-chart-export
-Version: 0.0.21
+Version: 0.0.22rc1
 Summary: compose_agent_export for docker-compose -> helm chart
 Author: Espen
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Requires-Dist: docker-compose-parser (==0.0.21)
 Requires-Dist: model-lib (==0.0.21)
```

## Comparing `compose_chart_export-0.0.21.dist-info/RECORD` & `compose_chart_export-0.0.22rc1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 compose_chart_export/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 compose_chart_export/chart_export.py,sha256=lRtxzU3Ac2SfOAxZmSv9ml0KsDM4tHx5ois0BOFF9dc,2517
 compose_chart_export/chart_file_templates.py,sha256=sQMgnbhaCgppTOO5XZD72YbshNJS90INvCENukeNY3w,14564
 compose_chart_export/chart_mods.py,sha256=6eaO7tuccQWcZDc_yoi3p7aIOO2YQ4vAb2aqKZ5qBzc,4974
 compose_chart_export/chart_read.py,sha256=5A7mcFdq1lnD7fitj5-evHE9A0zJ6aAlY0KEYPmeRZo,2285
-compose_chart_export/compose_export.py,sha256=9CLgDO88kYyR55TcHxhGsgaA4xbyj2f-mSXINYRP55w,9602
+compose_chart_export/compose_export.py,sha256=E8_y5HfKed20hKcb4GrUFP9QkoAHa6l4my3nFwr3AzI,9945
 compose_chart_export/ports.py,sha256=ubPaqe31gwDqPj8s4Bd6pZf8qB02hylpoQpYpbFkYwc,2365
 compose_chart_export/settings.py,sha256=-vo5OY1ttQUeGQwihuX2YTD-qHRgvBdMuRwP_BelWQY,191
-compose_chart_export-0.0.21.dist-info/METADATA,sha256=pt0BWsJQthTslawgiE7Vn6xjWQD2vveJcPrtoLg0jeE,626
-compose_chart_export-0.0.21.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-compose_chart_export-0.0.21.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-compose_chart_export-0.0.21.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
-compose_chart_export-0.0.21.dist-info/RECORD,,
+compose_chart_export-0.0.22rc1.dist-info/METADATA,sha256=lJbYccTcp-TS7boXR79CYfKk-JTV6u0TcKUASeuVGrc,629
+compose_chart_export-0.0.22rc1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+compose_chart_export-0.0.22rc1.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+compose_chart_export-0.0.22rc1.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
+compose_chart_export-0.0.22rc1.dist-info/RECORD,,
```

