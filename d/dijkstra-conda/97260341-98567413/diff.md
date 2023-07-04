# Comparing `tmp/dijkstra_conda-97260341.tar.gz` & `tmp/dijkstra_conda-98567413.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dijkstra_conda-97260341.tar", last modified: Fri Oct 21 13:23:09 2022, max compression
+gzip compressed data, was "dijkstra_conda-98567413.tar", last modified: Thu Sep 22 12:50:40 2022, max compression
```

## Comparing `dijkstra_conda-97260341.tar` & `dijkstra_conda-98567413.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 13:23:09.309554 dijkstra_conda-97260341/
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-10-21 13:22:52.000000 dijkstra_conda-97260341/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-10-21 13:22:52.000000 dijkstra_conda-97260341/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-10-21 13:23:09.309554 dijkstra_conda-97260341/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-10-21 13:22:52.000000 dijkstra_conda-97260341/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 13:23:09.305554 dijkstra_conda-97260341/dijkstra_conda/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 13:22:52.000000 dijkstra_conda-97260341/dijkstra_conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2409 2022-10-21 13:22:52.000000 dijkstra_conda-97260341/dijkstra_conda/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    27483 2022-10-21 13:22:52.000000 dijkstra_conda-97260341/dijkstra_conda/dfs_path_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 13:23:09.309554 dijkstra_conda-97260341/dijkstra_conda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-10-21 13:23:09.000000 dijkstra_conda-97260341/dijkstra_conda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-10-21 13:23:09.000000 dijkstra_conda-97260341/dijkstra_conda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 13:23:09.000000 dijkstra_conda-97260341/dijkstra_conda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-21 13:23:09.000000 dijkstra_conda-97260341/dijkstra_conda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 13:23:09.000000 dijkstra_conda-97260341/dijkstra_conda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-10-21 13:23:09.000000 dijkstra_conda-97260341/dijkstra_conda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-21 13:23:09.000000 dijkstra_conda-97260341/dijkstra_conda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-21 13:23:09.309554 dijkstra_conda-97260341/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-10-21 13:22:52.000000 dijkstra_conda-97260341/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:50:40.908970 dijkstra_conda-98567413/
+-rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-09-22 12:50:21.000000 dijkstra_conda-98567413/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-09-22 12:50:21.000000 dijkstra_conda-98567413/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2022-09-22 12:50:40.908970 dijkstra_conda-98567413/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-09-22 12:50:21.000000 dijkstra_conda-98567413/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:50:40.908970 dijkstra_conda-98567413/dijkstra_conda/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 12:50:21.000000 dijkstra_conda-98567413/dijkstra_conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-09-22 12:50:21.000000 dijkstra_conda-98567413/dijkstra_conda/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27197 2022-09-22 12:50:21.000000 dijkstra_conda-98567413/dijkstra_conda/dfs_path_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:50:40.908970 dijkstra_conda-98567413/dijkstra_conda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2022-09-22 12:50:40.000000 dijkstra_conda-98567413/dijkstra_conda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-22 12:50:40.000000 dijkstra_conda-98567413/dijkstra_conda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 12:50:40.000000 dijkstra_conda-98567413/dijkstra_conda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-22 12:50:40.000000 dijkstra_conda-98567413/dijkstra_conda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 12:50:40.000000 dijkstra_conda-98567413/dijkstra_conda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-22 12:50:40.000000 dijkstra_conda-98567413/dijkstra_conda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-22 12:50:40.000000 dijkstra_conda-98567413/dijkstra_conda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-22 12:50:40.908970 dijkstra_conda-98567413/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-09-22 12:50:21.000000 dijkstra_conda-98567413/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 12:50:40.908970 dijkstra_conda-98567413/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-09-22 12:50:21.000000 dijkstra_conda-98567413/test/test_dijkstra-conda.py
```

### Comparing `dijkstra_conda-97260341/LICENSE` & `dijkstra_conda-98567413/LICENSE`

 * *Files identical despite different names*

### Comparing `dijkstra_conda-97260341/PKG-INFO` & `dijkstra_conda-98567413/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dijkstra_conda
-Version: 97260341
+Version: 98567413
 Summary: A test project
 Home-page: https://github.com/iHeadWater/dijkstra-conda
 Author: dijkstra_conda-test
 License: MIT
 Keywords: dijkstra_conda
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `dijkstra_conda-97260341/dijkstra_conda/cli.py` & `dijkstra_conda-98567413/dijkstra_conda/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 import os
 import click
 from shapefile import Reader
-from .dfs_path_test import show_upstream_stations_graph, show_downstream_stations, upstream_node_on_mainstream, write_path_file
+from dfs_path_test import show_upstream_stations_graph, show_downstream_stations, upstream_node_on_mainstream, write_path_file
 
 
 @click.command(context_settings=dict(help_option_names=['-h', '--help']))
-@click.option('--outdated', default=False, help='decide regenerate cache files or not')
+@click.option('--outdated', is_flag=False, help='decide regenerate cache files or not')
 @click.option('--nodes_path', help='path of nodes shape file')
 @click.option('--river_path', help='path of river vector shape file')
 @click.option('--cur_sta', help='number of current station')
 @click.option('--up_sta', help='number of station which will be judge in mainstream or tributary in upstream watershed of current station')
-@click.option('--cutoff', default=2147483647, help='amount of stations which user want to limit')
-@click.option('--upstream', default=False, help='output upstream stations graph of current station')
-@click.option('--downstream', default=False, help='output list of downstream stations of current station')
-@click.option('--output_dir', default=os.curdir, help='when outdated is true,choose directory which you want to put your cache file')
-@click.option('--cache_dir', default=os.curdir, help='when outdated if false,choose directory where put cache file')
+@click.option('--cutoff', help='amount of stations which user want to limit')
+@click.option('--upstream', is_flag=False, help='output upstream stations graph of current station')
+@click.option('--downstream', is_flag=False, help='output list of downstream stations of current station')
+@click.option('--output_dir', help='when outdated is true,choose directory which you want to put your cache file')
+@click.option('--cache_dir', help='when outdated if false,choose directory where put cache file')
 def main(outdated, nodes_path, river_path, cur_sta, up_sta, cutoff, upstream, downstream, cache_dir, output_dir):
-    if (outdated is False) & (cache_dir is not None):
-        input_network_file_shp = os.path.abspath(river_path)
-        input_node_file_shp = os.path.relpath(nodes_path)
-        nodes_reader = Reader(input_node_file_shp)
-        network_reader = Reader(input_network_file_shp)
-    else:
-        input_network_file_shp = os.path.abspath(river_path)
-        input_node_file_shp = os.path.relpath(nodes_path)
-        nodes_reader = Reader(input_node_file_shp)
-        network_reader = Reader(input_network_file_shp)
-        write_path_file(nodes_reader, network_reader, cache_dir, output_dir)
+    input_network_file_shp = os.path.abspath(river_path)
+    input_node_file_shp = os.path.relpath(nodes_path)
+    nodes_reader = Reader(input_node_file_shp)
+    network_reader = Reader(input_network_file_shp)
     if upstream is True:
-        show_upstream_stations_graph(nodes_reader, network_reader, cur_sta, outdated, cache_dir, output_dir, cutoff)
+        show_upstream_stations_graph(network_reader, nodes_reader, cur_sta, outdated, cutoff, cache_dir, output_dir)
     elif downstream is True:
-        show_downstream_stations(nodes_reader, network_reader, cur_sta, outdated, cache_dir, output_dir, cutoff)
+        show_downstream_stations(nodes_reader, network_reader, cur_sta, outdated, cutoff, cache_dir, output_dir)
     if up_sta is not None:
-        upstream_node_on_mainstream(nodes_reader, network_reader, cur_sta, up_sta, outdated, cache_dir, output_dir)
+        upstream_node_on_mainstream(nodes_reader, network_reader, cur_sta, up_sta, cache_dir)
+    if outdated is True:
+        write_path_file(nodes_reader, network_reader, output_dir)
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `dijkstra_conda-97260341/dijkstra_conda/dfs_path_test.py` & `dijkstra_conda-98567413/dijkstra_conda/dfs_path_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import sys
 
 import bidict as bd
-import click
 import matplotlib.pyplot as plt
 import multidict as md
 import networkx as nx
 import pandas as pd
 from networkx import DiGraph
 from shapely import geometry
 from shapely.geometry import Point, LineString, GeometryCollection
@@ -91,15 +90,15 @@
     """
     source = Point(source_coord)
     p2 = Point(coord)
     c = (source.x + extrapolate_ratio * (p2.x - source.x), source.y + extrapolate_ratio * (p2.y - source.y))
     return LineString([source, c])
 
 
-def tie_outside_node(node_reader: Reader, network_reader: Reader, outdated: bool, cache_dir, output_path):
+def tie_outside_node(node_reader: Reader, network_reader: Reader, outdated: bool, cache_dir=os.curdir, output_path=os.curdir):
     """
     值得注意，由于tie_outside_node操作很费时，故工程中如有source_project_points.csv文件和nearest_line_project_points.csv文件，
     程序会优先从这两个文件中读取数据，所以如要从头生成，必须删除这两个文件
 
     参数
     ----------
     node_reader: 存储站点数据的Reader
@@ -127,37 +126,32 @@
             str_point: str = line_point_frame['nearest_point'][i].lstrip('(').rstrip(')')
             point_coord = (float(str_point.split(',')[0]), float(str_point.split(',')[1]))
             nearest_point_line_dict.add(line_string_wkt, point_coord)
     else:
         source_point_line_dict = bd.bidict()
         nearest_point_line_dict = md.MultiDict()
         for x in range(0, len(node_reader)):
+            print("Tying nodes:" + str(x))
             source_coord = tuple(node_reader.shape(x).points[0])
             nearest_line: LineString = line_min_dist(source_coord, network_reader)
             # 用以解决低质数据，下文while处若循环1000次后还连不上，就放弃
             outside_node_grid_geom_to_nearest_p \
                 = [q.wkt for q in nearest_points(Point(source_coord), nearest_line)]
             # 从两个最近点中取一个
             nearest_p = (loads(outside_node_grid_geom_to_nearest_p[1]).x, loads(outside_node_grid_geom_to_nearest_p[1]).y)
             point_src = nearest_line.coords[0]
             point_dst = nearest_line.coords[-1]
             if (nearest_p[0] == point_src[0]) & (nearest_p[1] == point_src[1]):
-                if point_dst[0] == point_src[0]:
-                    point_src_rand = (point_src[0], point_src[1] + 1e-6)
-                else:
-                    gradient = (point_dst[1] - point_src[1]) / (point_dst[0] - point_src[0])
-                    point_src_rand = (point_src[0] + 1e-6, point_src[1] + gradient * 1e-6)
+                gradient = (point_dst[1] - point_src[1]) / (point_dst[0] - point_src[0])
+                point_src_rand = (point_src[0] + 1e-6, point_src[1] + gradient * 1e-6)
                 source_point_line_dict.put(source_coord, point_src_rand)
                 nearest_point_line_dict.add(nearest_line.wkt, point_src_rand)
             elif (nearest_p[0] == point_dst[0]) & (nearest_p[1] == point_dst[1]):
-                if point_dst[0] == point_src[0]:
-                    point_dst_rand = (point_dst[0], point_dst[1] + 1e-6)
-                else:
-                    gradient = (point_dst[1] - point_src[1]) / (point_dst[0] - point_src[0])
-                    point_dst_rand = (point_dst[0] + 1e-6, point_dst[1] + gradient * 1e-6)
+                gradient = (point_dst[1] - point_src[1]) / (point_dst[0] - point_src[0])
+                point_dst_rand = (point_dst[0] + 1e-6, point_dst[1] + gradient * 1e-6)
                 source_point_line_dict.put(source_coord, point_dst_rand)
                 nearest_point_line_dict.add(nearest_line.wkt, point_dst_rand)
             else:
                 join_line = LineString([source_coord, nearest_p])
                 splits_edges_coll: GeometryCollection = geometry.GeometryCollection()
                 join_line_length = join_line.length
                 if join_line_length == 0:
@@ -186,15 +180,15 @@
         nearest_point_line_frame = pd.DataFrame({'nearest_line_wkt': nearest_point_line_dict.keys(),
                                                  'nearest_point': nearest_point_line_dict.values()})
         source_point_line_frame.to_csv(os.path.join(output_path, 'source_project_points.csv'), index=False)
         nearest_point_line_frame.to_csv(os.path.join(output_path, 'nearest_line_project_points.csv'), index=False)
     return source_point_line_dict, nearest_point_line_dict
 
 
-def build_graph(node_reader: Reader, network_reader: Reader, outdated: bool, cache_dir, output_path):
+def build_graph(node_reader: Reader, network_reader: Reader, outdated: bool, cache_dir=os.curdir, output_path=os.curdir):
     """
     参数
     ----------
     node_reader: 存储站点数据的Reader
     network_reader: 存储河网（所有LineString）数据的Reader
 
     返回
@@ -221,21 +215,21 @@
                 list_point_and_dis = sorted(list_point_and_dis, key=lambda point_dis: point_dis[1])
                 for i in range(0, len(list_point_and_dis)):
                     list_coords.append(list_point_and_dis[i][0])
                 nx.add_path(network_graph, list_coords)
             else:
                 src = line.points[0]
                 dest = line.points[-1]
-                network_graph.add_edge(tuple(src), tuple(dest))
+                network_graph.add_edge(src, dest)
         nx.write_edgelist(network_graph, os.path.join(output_path, 'network_graph.edgelist'), delimiter='|')
     return network_graph
 
 
 def get_upstream_stations(node_reader: Reader, network_reader: Reader,
-                          station_index: int, outdated: bool, cache_dir, output_path, cutoff: int = 2147483647):
+                          station_index: int, outdated: bool, cutoff: int = 2147483647, cache_dir=os.curdir, output_path=os.curdir):
     """
     参数
     ----------
     node_reader: 存储站点数据的Reader
     network_reader: 存储河网（所有LineString）数据的Reader
     station_index: 站点图层中的标号，本例中从0开始，针对不同数据，可以从图层属性表中行号辅助判断
     cutoff: 同一条河上最多可以上溯几个水文站，默认为int.max（当然也可以指定一个很大的数），即不限数量
@@ -244,15 +238,15 @@
     ----------
     upstream_graph: 从当前站点开始，河网与上游所有站点投影点构成的上游子图
     set_up_no_dup: 含有当前站点所有上游站点信息，元素为string形式
     """
     stations_up_list = []
     stations_graph = build_graph(node_reader, network_reader, outdated, cache_dir, output_path)
     source_target_dict = tie_outside_node(node_reader, network_reader, outdated, cache_dir, output_path)[0]
-    source_node_coord = tuple(node_reader.shape(int(station_index)).points[0])
+    source_node_coord = tuple(node_reader.shape(station_index).points[0])
     target_node_coord = source_target_dict.get(source_node_coord)
     upstream_graph_path = "upstream_graph_" + str(station_index) + "_cutoff_" + str(cutoff) + ".edgelist"
     if os.path.exists(os.path.join(cache_dir, upstream_graph_path)):
         if (outdated is False) & (os.path.exists(os.path.join(cache_dir, 'up_down_paths.txt'))):
             set_up_no_dup = set()
             with open(os.path.join(cache_dir, 'up_down_paths.txt'), mode='r+') as fp:
                 for line_str in fp.readlines():
@@ -269,15 +263,15 @@
         else:
             set_up_no_dup = set()
             upstream_graph = nx.read_edgelist(os.path.join(cache_dir, upstream_graph_path), delimiter='|',
                                               nodetype=lambda t: tuple([float(v) for v in str(t).strip("()").split(",")]),
                                               create_using=nx.DiGraph)
     else:
         source_target_dict = tie_outside_node(node_reader, network_reader, outdated, cache_dir, output_path)[0]
-        source_node_coord = tuple(node_reader.shape(int(station_index)).points[0])
+        source_node_coord = tuple(node_reader.shape(station_index).points[0])
         target_node_coord = source_target_dict.get(source_node_coord)
         upstream_graph = stations_graph.subgraph(nx.ancestors(stations_graph, target_node_coord) | {target_node_coord}).copy()
         if cutoff != 2147483647:
             nx.write_edgelist(upstream_graph,
                               os.path.join(output_path, upstream_graph_path), delimiter='|')
         set_up_no_dup = set()  # 给找到的路径去重
     for coord in upstream_graph.nodes:
@@ -292,15 +286,15 @@
                 if len(stations_up_list) > 1:
                     set_up_no_dup.add(str(stations_up_list[-cutoff:]))
                 stations_up_list.clear()
     return upstream_graph, set_up_no_dup
 
 
 def get_downstream_stations(node_reader: Reader, network_reader: Reader,
-                            station_index: int, outdated: bool, cache_dir, output_path, cutoff: int = 2147483647):
+                            station_index: int, outdated: bool, cutoff: int = 2147483647, cache_dir=os.curdir, output_path=os.curdir):
     """
     参数
     ----------
     node_reader: 存储站点数据的Reader
     network_reader: 存储河网（所有LineString）数据的Reader
     station_index: 站点图层中的标号，本例中从0开始，针对不同数据，可以从图层属性表中行号辅助判断
     cutoff: 同一条河上最多可以往下寻找几个水文站，默认为int.max（当然也可以指定一个很大的数），即不限数量
@@ -319,177 +313,178 @@
                 for i in range(0, len(line_str_station)):
                     line_str_station[i] = line_str_station[i].strip('\n').strip(' ').strip("'").strip('"')
                 if (line_str_head == 'downstream') & (('sta' + str(station_index)) == line_str_station[0]):
                     list_stations = line_str_station
     else:
         stations_graph = build_graph(node_reader, network_reader, outdated, cache_dir, output_path)
         source_target_dict = tie_outside_node(node_reader, network_reader, outdated, cache_dir, output_path)[0]
-        source_node_coord = tuple(node_reader.shape(int(station_index)).points[0])
+        source_node_coord = tuple(node_reader.shape(station_index).points[0])
         target_node_coord = source_target_dict.get(source_node_coord)
         dfs_tree_path = nx.dfs_tree(stations_graph, target_node_coord)
         for coord in dfs_tree_path:
             if coord in source_target_dict.values():
                 source_coord = source_target_dict.inv[coord]
                 for x in range(0, len(node_reader)):
                     if tuple(node_reader.shape(x).points[0]) == source_coord:
                         list_stations.append('sta' + str(x))
     return list_stations[:cutoff]
 
 
 def get_upstream_stations_graph(node_reader: Reader, network_reader: Reader, number: int, outdated: bool,
-                                cache_dir, output_path, cutoff: int = 2147483647):
+                                cutoff: int = 2147483647, cache_dir=os.curdir, output_path=os.curdir):
     """
     参数
     ----------
     node_reader: 存储站点数据的Reader
     network_reader: 存储河网（所有LineString）数据的Reader
     number: 站点图层中的标号，本例中从0开始，针对不同数据，可以从图层属性表中行号辅助判断
     cutoff: 同一条河上最多可以上溯几个水文站，默认为int.max（当然也可以指定一个很大的数），即不限数量
 
     返回
     ----------
     upstream_graph: 从当前站点开始，河网与上游所有站点投影点构成的上游子图
     new_graph: 当前站点及上游所有站点构成的子图
     origin_graph: 根据河源唯远判断干支流的原始河流抽象图
     """
-    upstream_graph = get_upstream_stations(node_reader, network_reader, number, outdated, cache_dir, output_path, cutoff)[0]
+    upstream_graph = get_upstream_stations(node_reader, network_reader, number, outdated, cutoff, cache_dir, output_path)[0]
     if (outdated is False) & os.path.exists(os.path.join(cache_dir, 'origin_graph.edgelist')):
         origin_graph = nx.read_edgelist(os.path.join(cache_dir, 'origin_graph.edgelist'), delimiter='|',
                                         nodetype=lambda t: tuple([float(v) for v in str(t).strip("()").split(",")]),
                                         create_using=nx.DiGraph, data=(("weight", float),))
     else:
         origin_graph = nx.DiGraph()
         for line in network_reader.shapes():
             src = tuple(line.points[0])
             dest = tuple(line.points[-1])
             shapely_line: LineString = loads(shape_type_to_wkt(line))
             origin_graph.add_edge(src, dest, weight=shapely_line.length)
     new_graph = nx.DiGraph()
     source_target_dict = tie_outside_node(node_reader, network_reader, outdated, cache_dir, output_path)[0]
-    source_node_coord = tuple(node_reader.shape(int(number)).points[0])
+    source_node_coord = tuple(node_reader.shape(number).points[0])
     target_node_coord = source_target_dict.get(source_node_coord)
     for coord in upstream_graph.nodes:
         if upstream_graph.in_degree(coord) == 0:
             for up_path in nx.all_simple_paths(upstream_graph, coord, target_node_coord):
                 list_up_path = list(up_path)
                 for path_coord in up_path:
                     if path_coord in origin_graph.nodes:
                         list_up_path.remove(path_coord)
                 nx.add_path(new_graph, list_up_path[-cutoff:])
     nx.write_edgelist(origin_graph, os.path.join(output_path, 'origin_graph.edgelist'), delimiter='|', data=["weight"])
     return upstream_graph, new_graph, origin_graph
 
 
-def write_path_file(node_reader: Reader, network_reader: Reader, cache_dir, output_path):
+def write_path_file(node_reader: Reader, network_reader: Reader, output_path=os.curdir):
     """
     将上下游信息分行保存在txt文件中以便下次读取，upstream: 代表上游，downstream: 代表下游
 
     参数
     ----------
     node_reader: 存储站点数据的Reader
     network_reader: 存储河网（所有LineString）数据的Reader
     """
     with open(os.path.join(output_path, "up_down_paths.txt"), mode='w+') as fp:
         for i in range(0, len(node_reader)):
-            click.echo('Writing stream: ' + str(i))
-            set_up_no_dup = get_upstream_stations(node_reader, network_reader, i, True, cache_dir, output_path)[1]
+            print('Writing stream: ' + str(i))
+            set_up_no_dup = get_upstream_stations(node_reader, network_reader, i, True, 2147483647, output_path)[1]
             list_up_no_dup = list(set_up_no_dup)
             for str_path in list_up_no_dup:
                 fp.writelines("upstream: " + str_path.lstrip('[').rstrip(']') + "\n")
-            list_down = get_downstream_stations(node_reader, network_reader, i, True, cache_dir, output_path)
+            list_down = get_downstream_stations(node_reader, network_reader, i, True)
             fp.writelines("downstream: " + str(list_down).lstrip('[').rstrip(']') + "\n")
 
 
 def show_upstream_stations_graph(node_reader: Reader, network_reader: Reader, number: int, outdated: bool,
-                                 cache_dir, output_path, cutoff: int = 2147483647):
+                                 cache_dir=os.curdir, output_path=os.curdir, cutoff: int = 2147483647):
     """
     显示当前站点的上游站点图
 
     参数
     ----------
     node_reader: 存储站点数据的Reader
     network_reader: 存储河网（所有LineString）数据的Reader
     number: 站点图层中的标号，本例中从0开始，针对不同数据，可以从图层属性表中行号辅助判断
     cutoff: 同一条河上最多可以上溯几个水文站，默认为int.max（当然也可以指定一个很大的数），即不限数量
     """
-    upstream_graph = get_upstream_stations_graph(node_reader, network_reader, number, outdated, cache_dir, output_path, cutoff)[1]
-    set_up_no_dup = get_upstream_stations(node_reader, network_reader, number, outdated, cache_dir, output_path, cutoff)[1]
+    upstream_graph = get_upstream_stations_graph(node_reader, network_reader, number, outdated, cutoff, cache_dir, output_path)[1]
+    set_up_no_dup = get_upstream_stations(node_reader, network_reader, number, outdated, cutoff, cache_dir, output_path)[1]
     for list_str in set_up_no_dup:
-        click.echo(list_str.lstrip('[').rstrip(']'))  # 输出的都是字串
-    nx.draw_networkx(upstream_graph, node_size=10, with_labels=False)
+        print(list_str.lstrip('[').rstrip(']'))  # 输出的都是字串
+    nx.draw_networkx(upstream_graph, node_size=10)
+    plt.show()
     plt.savefig(os.path.join(output_path, 'upstream_graph_' + str(number) + '_cutoff_' + str(cutoff) + '.png'))
 
 
 def show_downstream_stations(node_reader: Reader, network_reader: Reader, number: int, outdated: bool,
-                             cache_dir, output_path, cutoff: int = 2147483647):
+                             cache_dir=os.curdir, output_path=os.curdir, cutoff: int = 2147483647):
     """
     显示当前站点的下游站点列表
 
     参数
     ----------
     node_reader: 存储站点数据的Reader
     network_reader: 存储河网（所有LineString）数据的Reader
     number: 站点图层中的标号，本例中从0开始，针对不同数据，可以从图层属性表中行号辅助判断
     cutoff: 同一条河上最多可以往下寻找几个水文站，默认为int.max（当然也可以指定一个很大的数），即不限数量
     """
-    list_stations = get_downstream_stations(node_reader, network_reader, number, outdated, cache_dir, output_path, cutoff)
-    click.echo(list_stations)
+    list_stations = get_downstream_stations(node_reader, network_reader, number, outdated, cutoff, cache_dir, output_path)
+    print(list_stations)
 
 
 def upstream_node_on_mainstream(node_reader: Reader, network_reader: Reader, number_src, number_target, outdated: bool,
-                                cache_dir, output_dir):
+                                cache_dir=os.curdir):
     """
     以number_src为当前站点，判断number_target所代表的站点是否存在于当前站点上游流域的干支流中，存在三种结果：
     在支流中（In tributary），在干流中（In Mainstream），不在上游流域中
 
     参数
     ----------
     node_reader: 存储站点数据的Reader
     network_reader: 存储河网（所有LineString）数据的Reader
     number_src: 用以确定上游流域的站点号，可以从图层属性表中辅助判断
     number_target: 待判断的站点号
     """
     # number_src是要生成子图的原点号，number_target是要判断干支流的点号
-    source_point = tuple(node_reader.shape(int(number_src)).points[0])
-    target_point = tuple(node_reader.shape(int(number_target)).points[0])
+    source_point = tuple(node_reader.shape(number_src).points[0])
+    target_point = tuple(node_reader.shape(number_target).points[0])
     if (outdated is False) & (os.path.exists(os.path.join(cache_dir, 'nearest_line_project_points.csv')) & os.path.exists(
             os.path.join(cache_dir, 'source_project_points.csv'))):
         nearest_line_project_df = pd.read_csv(os.path.join(cache_dir, 'nearest_line_project_points.csv'))
-        source_project_point_dict = tie_outside_node(node_reader, network_reader, outdated, cache_dir, output_dir)[0]
+        source_project_point_dict = tie_outside_node(node_reader, network_reader, outdated, cache_dir)[0]
         source_nearest_point = source_project_point_dict.get(source_point)
         target_nearest_point = source_project_point_dict.get(target_point)
         nearest_source_line_wkt = nearest_line_project_df['nearest_line_wkt'][nearest_line_project_df['nearest_point'] ==
                                                                               str(source_nearest_point)].values[0]
         nearest_target_line_wkt = nearest_line_project_df['nearest_line_wkt'][nearest_line_project_df['nearest_point'] ==
                                                                               str(target_nearest_point)].values[0]
         nearest_source_line: LineString = loads(nearest_source_line_wkt)
         nearest_target_line: LineString = loads(nearest_target_line_wkt)
     else:
         nearest_target_line: LineString = line_min_dist(target_point, network_reader)
         nearest_source_line: LineString = line_min_dist(source_point, network_reader)
-    origin_graph = get_upstream_stations_graph(node_reader, network_reader, number_src, outdated, cache_dir, output_dir)[2]
+    origin_graph = get_upstream_stations_graph(node_reader, network_reader, number_src, outdated)[2]
     origin_target_point = nearest_target_line.coords[0]
     origin_source_point = nearest_source_line.coords[-1]
     origin_graph_src_sub: DiGraph = nx.subgraph(origin_graph, nx.ancestors(origin_graph, origin_source_point) | {
         origin_source_point}).copy()
-    set_up_no_dup = get_upstream_stations(node_reader, network_reader, number_src, outdated, cache_dir, output_dir)[1]
+    set_up_no_dup = get_upstream_stations(node_reader, network_reader, number_src, outdated, cutoff=10000)[1]
     in_basin = False
     for upstream_str in set_up_no_dup:
         in_basin = in_basin | ('sta' + str(number_target) in upstream_str)
         if in_basin is False:
             continue
         else:
             # 寻找所有到nearest_line.coords[-1]的边，然后判断其是否小于DAG最长长度
             line_stations = upstream_str.strip('[]').replace("'", "").replace(' ', '').split(',')
             for i in range(0, len(line_stations)):
                 line_stations[i] = line_stations[i].replace('"', '')
             if (nx.shortest_path_length(origin_graph_src_sub, origin_target_point, origin_source_point, weight='weight') <
-                nx.dag_longest_path_length(origin_graph_src_sub, weight='weight')) & (
-                    origin_target_point not in nx.dag_longest_path(origin_graph_src_sub, weight='weight')):
-                click.echo('In tributary: ' + str(line_stations))
+                nx.dag_longest_path_length(origin_graph_src_sub, weight='weight')) & (origin_target_point not in nx.dag_longest_path(
+                origin_graph_src_sub, weight='weight')):
+                print('In tributary: ' + str(line_stations))
                 break
             else:
                 cutoff = line_stations.index('sta' + str(number_target))
-                click.echo('In Mainstream: ' + str(line_stations[cutoff:]))
+                print('In Mainstream: ' + str(line_stations[cutoff:]))
                 break
     if in_basin is False:
-        click.echo(str(number_target) + ' is not in upstream basin of ' + str(number_src))
+        print(str(number_target) + ' is not in upstream basin of ' + str(number_src))
```

### Comparing `dijkstra_conda-97260341/dijkstra_conda.egg-info/PKG-INFO` & `dijkstra_conda-98567413/dijkstra_conda.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dijkstra-conda
-Version: 97260341
+Version: 98567413
 Summary: A test project
 Home-page: https://github.com/iHeadWater/dijkstra-conda
 Author: dijkstra_conda-test
 License: MIT
 Keywords: dijkstra_conda
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `dijkstra_conda-97260341/setup.py` & `dijkstra_conda-98567413/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,15 @@
     author='dijkstra_conda-test',
     url='https://github.com/iHeadWater/dijkstra-conda',
     packages=[
         'dijkstra_conda',
     ],
     package_dir={'dijkstra_conda': 'dijkstra_conda'},
     include_package_data=True,
-    install_requires=['pytest>=7.1.3', 'setuptools>=63.4.1', 'click>=8.1.3', 'bidict>=0.21.2', 'multidict>=6.0.2',
-                      'networkx>=2.8.6', 'pandas>=1.4.3', 'shapely>=1.8.4', 'pyshp>=2.3.1', 'matplotlib<=3.5.3'],
+    install_requires=['pytest>=7.1.3','setuptools>=63.4.1','click>=8.1.3','geopandas>=0.11.1','bidict>=0.21.2','multidict>=6.0.2','networkx>=2.8.6','pandas>=1.4.3','shapely>=1.8.4'],
     license='MIT',
     zip_safe=False,
     keywords='dijkstra_conda',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

