# Comparing `tmp/bsimx-0.1.2.tar.gz` & `tmp/bsimx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsimx-0.1.2.tar", max compression
+gzip compressed data, was "bsimx-0.2.0.tar", max compression
```

## Comparing `bsimx-0.1.2.tar` & `bsimx-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1030 2023-06-19 15:15:22.117286 bsimx-0.1.2/README.md
--rw-r--r--   0        0        0      514 2023-06-19 15:18:05.685917 bsimx-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6226 2023-06-19 14:48:39.875966 bsimx-0.1.2/src/bsimx.py
--rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 bsimx-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      645 2023-07-04 05:02:37.222850 bsimx-0.2.0/README.md
+-rw-r--r--   0        0        0      529 2023-07-04 05:15:56.442853 bsimx-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6406 2023-07-04 05:02:37.242850 bsimx-0.2.0/src/bsimx.py
+-rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 bsimx-0.2.0/PKG-INFO
```

### Comparing `bsimx-0.1.2/src/bsimx.py` & `bsimx-0.2.0/src/bsimx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,214 +1,249 @@
-from typing import List, Self, Any
+from typing import Callable, Optional, Any, Union
 import networkx as nx
 import json
-import numpy as np
-from flask import Flask, redirect
-from flask_cors import CORS
+from flask import Flask, render_template
 import json
 
+from type import (
+    AgentResult,
+    AreaBounds,
+    EdgeResult,
+    NodeResult,
+    Position,
+    RouteResult,
+    SimulationResult,
+    TimeBounds,
+)
+
+AnyGraph = Union[nx.Graph, nx.MultiGraph, nx.DiGraph, nx.MultiDiGraph]
+
+
+class Environment:
+    G: AnyGraph
+    timestamp: int
+    nodes: list[Any]
+    agents: list[Any]
+
+    def __init__(self, G: AnyGraph) -> None:
+        self.G = G
+        self.timestamp = 0
+        self.nodes = []
+        self.agents = []
+
+    def edge_distance(self, source: Any, target: Any) -> Optional[float]:
+        e = self.G.get_edge_data(source, target)
+        if not e:
+            return None
+        if isinstance(self.G, (nx.MultiGraph, nx.MultiDiGraph)):
+            return min([e[k]["length"] for k in e])
+        return e["length"]
+
+    def node_position(self, id: Any) -> Position:
+        n = self.G.nodes[id]
+        return Position(x=n["x"], y=n["y"])
+
 
 class Agent:
-    @staticmethod
-    def fields():
-        return ["x", "y", "timestamp"]
-
-    __id: int
-    __history: List[List[Any]]
-    __route: List[Any]
-    __edge_progress: float
-    __timestamp: int
+    env: Environment
+    id: int
+    __icon: str
     __speed: float
+    __progress: float
+    __route: list[Any]
+    __logs: list[RouteResult]
+    __todos: list[tuple[Callable[[], bool], Callable[[], Any]]]
 
-    def __init__(self, id: int, **kwargs):
-        self.__id = id
+    def reset(self):
+        self.__icon = "https://fonts.gstatic.com/s/i/short-term/release/materialsymbolsoutlined/directions_run/default/48px.svg"  # noqa: E501
+        self.__speed = 1.0
+        self.__progress = 0.0
+        self.__route = []
+        self.__logs = []
+        self.__todos = []
+        self.env = None
+
+    def __init__(self, **kwargs):
         self.reset()
         for k in kwargs:
             setattr(self, k, kwargs[k])
 
-    def push_history(self, G: nx.Graph):
-        d = self.get_data(G)
-        self.__history.append(d)
+    # override
+
+    def search_path(self, source: Any, target: Any):
+        """maybe override"""
+        return nx.dijkstra_path(self.env.G, source, target, weight="length")
+
+    def on_started(self):
+        """for override"""
+
+    def on_passed(self):
+        """for override"""
 
-    def get_data(self, G: nx.Graph):
+    def on_arrived(self):
+        """for override"""
+
+    def on_everytime(self):
+        """for override"""
+
+    def is_free(self):
         len_r = len(self.__route)
-        if len_r == 0:
-            return {"x": None, "y": None, "timestamp": self.__timestamp}
+        return len_r < 2 and not self.__todos
 
-        n1 = G.nodes[self.__route[0]]
-        x_key = G.graph["x_key"]
-        y_key = G.graph["y_key"]
-        if len_r == 1:
-            return {
-                "x": n1[x_key],
-                "y": n1[y_key],
-                "timestamp": self.__timestamp,
-            }
-        n2 = G.nodes[self.__route[1]]
-        if type(G) is nx.MultiGraph or type(G) is nx.MultiDiGraph:
-            edge_datas = G.get_edge_data(self.__route[0], self.__route[1])
-            d = min([edge_datas[key][G.graph["length_key"]] for key in edge_datas])
-        else:
-            d = G.get_edge_data(self.__route[0], self.__route[1])[G.graph["length_key"]]
-        w2 = self.__edge_progress / d
-        w1 = 1 - w2
-        return {
-            "x": n1[x_key] * w1 + n2[x_key] * w2,
-            "y": n1[y_key] * w1 + n2[y_key] * w2,
-            "timestamp": self.__timestamp,
-        }
+    def set_icon(self, v: str):
+        self.__icon = v
+        self.log()
 
-    def is_arrived(self):
-        return len(self.__route) <= 1
+    def set_speed(self, v: float):
+        self.__speed = v
+        self.log()
 
-    def tick(self, G: nx.Graph):
-        self.__timestamp += 1
+    def set_start_node(self, v: Any):
         len_r = len(self.__route)
         if len_r < 2:
+            self.__route = [v]
             return
-        n1, n2 = self.__route[:2]
-        if type(G) is nx.MultiGraph or type(G) is nx.MultiDiGraph:
-            edge_datas = G.get_edge_data(self.__route[0], self.__route[1])
-            d = min([edge_datas[key][G.graph["length_key"]] for key in edge_datas])
-        else:
-            d = G.get_edge_data(self.__route[0], self.__route[1])[G.graph["length_key"]]
-        self.__edge_progress += self.__speed
-        if self.__edge_progress >= d:
-            # on_stepped
-            r = self.__edge_progress - d
-            self.__route.pop(0)
-            self.__edge_progress = 0.0
-            self.push_history(G)
-            self.on_stepped(n2, G)
-            self.__edge_progress = r
-            if len_r == 2:
-                # on_arrived
-                self.on_arrived(n2, G)
-
-    def get_id(self):
-        return self.__id
+        self.__route = self.search_path(v, self.__route[-1])
+        self.log()
 
-    def get_history(self):
-        return json.loads(json.dumps(self.__history))
+    def set_goal_node(self, v: Any):
+        len_r = len(self.__route)
+        if len_r < 1:
+            return
+        self.__route = self.search_path(self.__route[0], v)
+        self.log()
 
-    def reset(self):
-        self.__history = []
-        self.__route = []
-        self.__edge_progress = 0
-        self.__timestamp = 0
-        self.__speed = 1.0
+    def step(self):
+        self.on_everytime()
+        todos = []
+        for todo in self.__todos:
+            if todo[0]():
+                todo[1]()
+                continue
+            todos.append(todo)
+        self.__todos = todos
+        len_r = len(self.__route)
+        if len_r < 2:
+            return
+        self.__progress += self.__speed
+        e = self.env
+        n1 = self.__route[0]
+        n2 = self.__route[1]
+        n3 = self.__route[2] if len_r > 2 else None
+        d = e.edge_distance(n1, n2)
+        if d is None:
+            raise Exception("invalid route")
+        if self.__progress < d:
+            return
+        # passed
+        self.__progress -= d
+        self.__route.pop(0)
+        self.log()
+        e.nodes = [n2, n1, n3]
+        self.on_passed()
+        if n3 is not None:
+            return
+        # arrived
+        self.on_arrived()
 
-    def teleport(self, G: nx.Graph, node: Any):
-        goal = self.__route[-1] if len(self.__route) > 1 else None
-        self.__edge_progress = 0.0
-        self.__route = [node]
-        if goal:
-            self.set_goal(goal, G)
-        self.push_history(G)
-
-    def set_goal(self, G: nx.Graph, goal: Any):
-        r_len = len(self.__route)
-        if r_len == 0:
-            return
-        elif r_len == 1 or self.__edge_progress == 0.0:
-            source = self.__route[0]
-            path = self.search_path(G, source, goal)
-            self.__route = path
+    def log(self):
+        e = self.env
+        len_r = len(self.__route)
+        if len_r == 0:
             return
         n1 = self.__route[0]
+        p1 = e.node_position(n1)
+        if len_r == 1:
+            self.__logs.append(
+                RouteResult(x=p1.x, y=p1.y, timestamp=e.timestamp, icon=self.__icon)
+            )
+            return
         n2 = self.__route[1]
-        d = G[n1][n2][G.graph["length_key"]]
-        p1 = self.search_path(G, n1, goal)
-        p2 = self.search_path(G, n2, goal)
-        d1 = (
-            np.sum([G[i][j][G.graph["length_key"]] for i, j in zip(p1, p1[1:])])
-            if len(p1) > 1
-            else 0.0
-        ) + self.__edge_progress
-        d2 = (
-            np.sum([G[i][j][G.graph["length_key"]] for i, j in zip(p2, p2[1:])])
-            if len(p1) > 1
-            else 0.0
-        ) + (d - self.__edge_progress)
-        self.__route = p1 if d1 < d2 else p2
-        if d1 < d2:
-            self.__edge_progress = d - self.__edge_progress
-
-    def set_speed(self, G: nx.Graph, speed: float):
-        self.__speed = speed
-        self.push_history(G)
+        p2 = e.node_position(n2)
+        d = e.edge_distance(n1, n2)
+        w2 = self.__progress / d
+        w1 = 1 - w2
+        self.__logs.append(
+            RouteResult(
+                x=p1.x * w1 + p2.x * w2,
+                y=p1.y * w1 + p2.y * w2,
+                timestamp=e.timestamp,
+                icon=self.__icon,
+            )
+        )
+
+    def task(self, wait: Any, todo: Callable[[], Any]):
+        if callable(wait):
+            w = wait
+        else:
+            t = self.env.timestamp
 
-    def search_path(self, G: nx.Graph, source: Any, target: Any):
-        """maybe override"""
-        return nx.dijkstra_path(G, source, target, weight=G.graph["length_key"])
+            def w():
+                return self.env.timestamp >= t + wait
 
-    def on_started(self, G: nx.Graph, agents: List[Self]):  # type: ignore
-        """for override"""
+        self.__todos.append((w, todo))
 
-    def on_stepped(self, G: nx.Graph, node: int):
-        """for override"""
+    def get_logs(self):
+        return self.__logs
+
+
+def create_envrironment(G: AnyGraph):
+    return Environment(G)
 
-    def on_arrived(self, G: nx.Graph, node: int):
-        """for override"""
 
+def simulate(agents: list[Agent], G: AnyGraph) -> SimulationResult:
+    # starting
+    e = create_envrironment(G)
+    for i, a in enumerate(agents):
+        a.id = i
+        a.env = e
+        e.agents.append(a)
 
-def simulate(
-    agents: List[Agent], G: nx.Graph, x_key="x", y_key="y", length_key="length"
-):
-    g = G.copy()
-    g.graph["x_key"] = x_key
-    g.graph["y_key"] = y_key
-    g.graph["length_key"] = length_key
     for a in agents:
-        a.on_started(g, agents)
+        a.on_started()
 
-    while any([not a.is_arrived() for a in agents]):
+    # simulating
+    while [a for a in agents if not a.is_free()]:
+        e.timestamp += 1
         for a in agents:
-            a.tick(g)
+            a.step()
 
-    data = [
-        {"id": a.get_id(), "class": a.__class__.__name__, "history": a.get_history()}
-        for a in agents
+    # ending
+    agent_results = [
+        AgentResult(classname=a.__class__.__name__, routes=a.get_logs()) for a in agents
     ]
+    node_results = [NodeResult(id=id, **attr) for id, attr in G.nodes(data=True)]
+    edge_results = [EdgeResult(left=left, right=right) for left, right in G.edges()]
+    all_routes: list[RouteResult] = sum(
+        [[r for r in a.routes] for a in agent_results], []
+    )
+    time_bounds = TimeBounds(
+        min=0,
+        max=max([r.timestamp for r in all_routes]),
+    )
+    xs = [r.x for r in all_routes] + [n.x for n in node_results]
+    ys = [r.y for r in all_routes] + [n.y for n in node_results]
+    area_bounds = AreaBounds(n=max(ys), s=min(ys), e=max(xs), w=min(xs))
+    simulation_result = SimulationResult(
+        nodes=node_results,
+        edges=edge_results,
+        agents=agent_results,
+        time_bounds=time_bounds,
+        area_bounds=area_bounds,
+    )
 
     for a in agents:
         a.reset()
 
-    return data
+    return simulation_result
 
 
-def serializable(item: Any):
-    try:
-        json.dumps(item)
-    except TypeError:
-        return False
-    return True
-
-
-def preview(G: nx.Graph, simulation_result: list[dict[str, Any]] = []):
+def preview(simulation_result: SimulationResult):
     app = Flask(__name__)
-    CORS(app)
-
-    nodes = [
-        (n[0], {k: n[1][k] for k in n[1] if serializable(n[1][k])})
-        for n in G.nodes(data=True)
-    ]
-    edges = [
-        (e[0], e[1], {k: e[2][k] for k in e[2] if serializable(e[2][k])})
-        for e in G.edges(data=True)
-    ]
 
     @app.route("/")
     def home():
-        return redirect("/api/bsim")
+        return render_template(
+            "index.html", simulation_result=json.dumps(simulation_result.dict())
+        )
 
-    @app.route("/api/bsim")
-    def bsim_result():
-        return {"trips": simulation_result, "nodes": nodes, "edges": edges}
-
-    print(
-        """
-###################################################
-Bsim Preview 🗺️ : https://bsimx.netlify.app/preview
-###################################################"""
-    )
     app.run()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bsimx-0.1.2/PKG-INFO` & `bsimx-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,49 @@
 Metadata-Version: 2.1
 Name: bsimx
-Version: 0.1.2
+Version: 0.2.0
 Summary: The agent-based modeling tool with deck.gl, networkx and osmnx.
 Author: s-uei
 Author-email: uei.shunsuke@kagawa-u.ac.jp
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flask (>=2.2.3,<3.0.0)
-Requires-Dist: flask-cors (>=3.0.10,<4.0.0)
 Requires-Dist: networkx (>=2.8.8,<3.0.0)
 Requires-Dist: osmnx (>=1.3.0,<2.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Description-Content-Type: text/markdown
 
 # bsimx
 
 The agent-based modeling tool with [deck.gl](https://deck.gl/), [networkx](https://networkx.org/) and [osmnx](https://osmnx.readthedocs.io/en/stable/)..
 
+## Installation
+
+```sh
+pip install networkx osmnx bsimx
+```
+
 ## Getting Started
 
 ```py
-import networkx as nx
 import osmnx as ox
 from bsimx import preview, Agent, simulate
 
-# networkx graph from open street map.
+
 G = ox.graph_from_place("Takamatsu Hayashi", network_type="drive")
 
-# simple walker model
-class SimpleWalker(Agent):
-    start: int # start node id
-    goal: int # goal node id
-
-    # the action of this model on simulation started
-    def on_started(self, G: nx.Graph, *_):
-        # move to `start` immediately
-        self.teleport(G, self.start)
-        # set goal node
-        # continue to move to `goal` with Dijkstra algorithm
-        self.set_goal(G, self.goal)
-        # moving speed: 1.0 ms
-        self.set_speed(G, 1.0)
 
-# give parameters to model
-instances = [SimpleWalker(id=1, start=1042117440, goal=1042116599)]
+class Escaper(Agent):
+    start: int
+
+    def on_started(self):
+        self.set_start_node(self.start)
+        self.set_goal_node(1042117440)
+        self.set_speed(1.0)
 
-# simulation
-trips = simulate(instances, G)
 
-# preview on web map
-preview(G, trips)
+sr = simulate([Escaper(start=1042116599), Escaper(start=4111619945)], G)
+preview(sr)
 ```
```

