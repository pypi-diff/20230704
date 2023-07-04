# Comparing `tmp/sowing-0.0.2.tar.gz` & `tmp/sowing-0.0.3.tar.gz`

## Comparing `sowing-0.0.2.tar` & `sowing-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 sowing-0.0.2/sowing/lca.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 sowing-0.0.2/sowing/node.py
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 sowing-0.0.2/sowing/traversal.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sowing-0.0.2/sowing/zipper.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 sowing-0.0.2/sowing/comb/binary.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 sowing-0.0.2/sowing/comb/supertree.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 sowing-0.0.2/sowing/util/dataclasses.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 sowing-0.0.2/sowing/util/partition.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 sowing-0.0.2/sowing/util/rangequery.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 sowing-0.0.2/sowphy/clade.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sowing-0.0.2/sowphy/newick/__init__.py
--rw-r--r--   0        0        0    11870 2020-02-02 00:00:00.000000 sowing-0.0.2/sowphy/newick/parse.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 sowing-0.0.2/sowphy/newick/write.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 sowing-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sowing-0.0.2/LICENSE
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 sowing-0.0.2/README.md
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 sowing-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 sowing-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/indexed.py
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/node.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/traversal.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/zipper.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/comb/binary.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/comb/supertree.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/repr/json.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/repr/newick/__init__.py
+-rw-r--r--   0        0        0    11539 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/repr/newick/parse.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/repr/newick/write.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/util/dataclasses.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/util/partition.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 sowing-0.0.3/sowing/util/rangequery.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 sowing-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sowing-0.0.3/LICENSE
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 sowing-0.0.3/README.md
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 sowing-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 sowing-0.0.3/PKG-INFO
```

### Comparing `sowing-0.0.2/sowing/zipper.py` & `sowing-0.0.3/sowing/zipper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,134 +1,144 @@
-from typing import Hashable, Self, Optional
+from typing import Generic, Hashable, Self, TypeVar, TYPE_CHECKING
 from dataclasses import dataclass, replace
 from .util.dataclasses import repr_default
 
 
+if TYPE_CHECKING:
+    from .node import Node
+
+
+NodeData = TypeVar("NodeData", bound=Hashable)
+EdgeData = TypeVar("EdgeData", bound=Hashable)
+OutNodeData = TypeVar("OutNodeData", bound=Hashable)
+OutEdgeData = TypeVar("OutEdgeData", bound=Hashable)
+
+
 @repr_default
 @dataclass(frozen=True, slots=True)
-class Zipper:
+class Zipper(Generic[NodeData, EdgeData]):
     # Currently pointed node
-    node: Optional["Node"] = None  # noqa
+    node: "Node[NodeData, EdgeData] | None" = None
 
     # Data attached to the incoming edge
-    data: Hashable | None = None
+    data: EdgeData | None = None
 
     # Child index into the parent node
     index: int = -1
 
     # Current depth level
     depth: int = 0
 
     # Parent pointer, or None if at root
-    parent: Self | None = None
+    parent: "Zipper[NodeData, EdgeData] | None" = None
 
     def replace(self, **kwargs) -> Self:
         return replace(self, **kwargs)
 
     def is_empty(self) -> bool:
         """Test whether there is a pointed node."""
         return self.node is None
 
     def is_leaf(self) -> bool:
         """Test whether the pointed node is a leaf node."""
-        return not self.is_empty() and self.node.edges == ()
+        return self.node is None or self.node.edges == ()
 
-    def down(self, index: int = 0) -> Self:
+    def down(self, index: int = 0) -> "Zipper[NodeData, EdgeData]":
         """
         Move to a child of the pointed node.
 
         :param index: index of the child to move to;
             negative indices are supported (default: first child)
         :returns: updated zipper
         """
-        if self.is_empty() or index >= len(self.node.edges):
+        if self.node is None or index >= len(self.node.edges):
             raise IndexError("child index out of range")
 
         edges = self.node.edges
         index %= len(edges)
-        return Zipper(
+        return self.replace(
             node=edges[index].node,
             data=edges[index].data,
             parent=self.replace(node=self.node.pop(index)),
             index=index,
             depth=self.depth + 1,
         )
 
     def is_root(self) -> bool:
         """Test whether the pointed node is a root node."""
         return self.parent is None
 
-    def up(self) -> Self:
+    def up(self) -> "Zipper[NodeData, EdgeData]":
         """Move to the parent of the pointed node."""
-        if self.is_root():
+        if self.parent is None:
             raise IndexError("cannot go up")
 
-        if self.is_empty():
+        if self.node is None:
             return self.parent
 
+        if self.parent.node is None:
+            raise ValueError("cannot attach to empty parent zipper")
+
         return self.parent.replace(
-            node=self.parent.node.add(self.node, self.data, self.index),
+            node=self.parent.node.add(self.node, data=self.data, index=self.index),
         )
 
     def is_last_sibling(self, direction: int = 1) -> bool:
         """
         Test whether the pointed node is the last sibling in a direction.
 
         :param direction: positive number to test in left to right order,
             negative number to test in right to left order
         """
-        if self.is_root():
+        if self.parent is None or self.parent.node is None:
             return True
 
         if direction == 0:
             return False
 
         if direction < 0:
             return self.index == 0
 
         return self.index == len(self.parent.node.edges)
 
-    def sibling(self, offset: int = 1) -> Self:
+    def sibling(self, offset: int = 1) -> "Zipper[NodeData, EdgeData]":
         """
         Move to a sibling of the pointed node.
 
         :param offset: sibling offset relative to the current node;
             zero for self, positive for right, negative for left, wrapping
             around the child list if needed (default: sibling to the right)
         :returns: updated zipper
         """
-        if self.is_root():
+        if self.parent is None or self.parent.node is None or offset == 0:
             return self
 
         if self.is_empty():
-            if offset == 0:
-                raise IndexError("cannot go to self for empty node")
-            elif offset > 0:
-                offset -= 1
+            offset -= 1
 
         index = self.index + offset
         index %= len(self.parent.node.edges) + 1
         return self.up().down(index)
 
-    def _preorder(self, flip: bool) -> Self:
+    def _preorder(self, flip: bool) -> "Zipper[NodeData, EdgeData]":
         child = -1 if flip else 0
         sibling = -1 if flip else 1
 
         if not self.is_leaf():
             return self.down(child)
 
         while self.is_last_sibling(sibling):
             if self.is_root():
                 return self
 
             self = self.up()
 
         return self.sibling(sibling)
 
-    def _postorder(self, flip: bool) -> Self:
+    def _postorder(self, flip: bool) -> "Zipper[NodeData, EdgeData]":
         child = -1 if flip else 0
         sibling = -1 if flip else 1
 
         if self.is_root():
             while not self.is_leaf():
                 self = self.down(child)
 
@@ -140,39 +150,39 @@
         self = self.sibling(sibling)
 
         while not self.is_leaf():
             self = self.down(child)
 
         return self
 
-    def next(self, preorder: bool = False) -> Self:
+    def next(self, preorder: bool = False) -> "Zipper[NodeData, EdgeData]":
         """
         Move to the next node in preorder or postorder.
 
         :param preorder: pass True to move in preorder (default is postorder)
         :returns: updated zipper
         """
         if preorder:
             return self._preorder(flip=False)
         else:
             return self._postorder(flip=False)
 
-    def prev(self, preorder: bool = False) -> Self:
+    def prev(self, preorder: bool = False) -> "Zipper[NodeData, EdgeData]":
         """
         Move to the previous node in preorder or postorder.
 
         :param preorder: pass True to move in preorder (default is postorder)
         :returns: updated zipper
         """
         if preorder:
             return self._postorder(flip=True)
         else:
             return self._preorder(flip=True)
 
-    def zip(self) -> "Node":  # noqa
+    def zip(self) -> "Node[NodeData, EdgeData] | None":
         """Zip up to the root and return it."""
         bubble = self
 
         while not bubble.is_root():
             bubble = bubble.up()
 
         return bubble.node
```

### Comparing `sowing-0.0.2/sowing/comb/binary.py` & `sowing-0.0.3/sowing/comb/binary.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from ..node import Node, Edge
-from ..traversal import traverse
+from .. import traversal
 from itertools import product, combinations_with_replacement
 from collections import Counter
 from typing import Iterable
 
 
 def is_binary(root: Node) -> bool:
-    return all(len(cursor.node.edges) in (0, 2) for cursor in traverse(root))
+    return all(len(cursor.node.edges) in (0, 2) for cursor in traversal.depth(root))
 
 
 def binarize_at(root: Node) -> Iterable[Node]:
     """
     Generate all possible binarizations of a node.
 
     This only binarizes the first level below :param:`root`.
```

### Comparing `sowing-0.0.2/sowing/comb/supertree.py` & `sowing-0.0.3/sowing/comb/supertree.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,20 +58,20 @@
 
         while base.sibling() == base and not base.is_root():
             base = base.up()
 
         if base.is_root():
             return cursor
 
-        outgroup = next(traversal.leaves(base.sibling().node))
+        outgroup = next(traversal.leaves(base.sibling().node)).node
         triples.append(Triple(children, outgroup))
         return base.replace(node=children[0])
 
-    traversal.maptree(extract_parts, traversal.traverse(root))
-    leaves = list(traversal.leaves(root))
+    traversal.fold(extract_parts, traversal.depth(root))
+    leaves = [cursor.node for cursor in traversal.leaves(root)]
     return leaves, triples, fans
 
 
 def build(
     leaves: list[Node],
     triples: list[Triple] = [],
     fans: list[Fan] = [],
```

### Comparing `sowing-0.0.2/sowing/util/partition.py` & `sowing-0.0.3/sowing/util/partition.py`

 * *Files identical despite different names*

### Comparing `sowing-0.0.2/sowing/util/rangequery.py` & `sowing-0.0.3/sowing/util/rangequery.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,25 @@
         """
         length = len(data)
         levels = _ilog2(length) + 1
 
         # sparse_table[depth][i] stores the value of the function
         # on the (i, i + 2**depth) range
         self.sparse_table = [[None] * length for _ in range(levels)]
-        self.sparse_table[0] = list(data)
 
-        for depth in range(1, levels):
-            for i in range(length - 2**depth + 1):
-                left = self.sparse_table[depth - 1][i]
-                assert left is not None
-                right = self.sparse_table[depth - 1][i + 2 ** (depth - 1)]
-                assert right is not None
-                self.sparse_table[depth][i] = function(left, right)
+        if levels > 0:
+            self.sparse_table[0] = list(data)
+
+            for depth in range(1, levels):
+                for i in range(length - 2**depth + 1):
+                    left = self.sparse_table[depth - 1][i]
+                    assert left is not None
+                    right = self.sparse_table[depth - 1][i + 2 ** (depth - 1)]
+                    assert right is not None
+                    self.sparse_table[depth][i] = function(left, right)
 
         self.function = function
 
     def __call__(self, start: int, stop: int):
         """
         Compute the value of the function on a range.
```

### Comparing `sowing-0.0.2/sowphy/newick/parse.py` & `sowing-0.0.3/sowing/repr/newick/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Iterator
 from collections import deque
 from enum import Enum, auto
 from dataclasses import dataclass
+from immutables import Map
 from sowing.node import Node
-from ..clade import Clade, Branch, Map
 
 
 class ParseError(Exception):
     """Parsing error with location information."""
 
     def __init__(self, message, start, end):
         if abs(start - end) <= 1:
@@ -335,66 +335,59 @@
     tokens = TokenIterator(tokenize(data))
     state = ParseState.NodeStart
 
     while state != ParseState.Finish:
         match state:
             case ParseState.NodeStart:
                 # Start parsing a new node
-                nodes.append(Node(Clade()))
+                nodes.append(Node())
 
                 if (token := next(tokens)).kind == TokenKind.OpenParen:
                     state = ParseState.NodeStart
                 else:
                     tokens.push(token)
                     state = ParseState.NodeData
 
             case ParseState.NodeData:
                 # Parse metadata attached to a node
-                clade = Clade()
-                branch = Branch()
+                clade = Map()
+                branch = Map()
 
                 # Parse node label
                 if (token := next(tokens)).kind == TokenKind.String:
-                    clade = clade.replace(name=token.value)
+                    clade = clade.set("name", token.value)
                 else:
                     tokens.push(token)
 
                 # Parse node props
-                clade = clade.replace(props=_parse_props(tokens))
+                clade = clade.update(_parse_props(tokens))
 
                 if (token := next(tokens)).kind == TokenKind.Colon:
                     # Parse branch length
                     if (token := next(tokens)).kind == TokenKind.String:
-                        try:
-                            branch = branch.replace(length=float(token.value))
-                        except ValueError:
-                            raise ParseError(
-                                f"invalid branch length value '{token.value}'",
-                                token.start,
-                                token.end,
-                            )
+                        branch = branch.set("length", token.value)
                     else:
                         tokens.push(token)
 
                     # Parse branch props
-                    branch = branch.replace(props=_parse_props(tokens))
+                    branch = branch.update(_parse_props(tokens))
                 else:
                     tokens.push(token)
 
                 active = nodes.pop()
-                active = active.replace(data=clade)
+                active = active.replace(data=clade or None)
 
                 if not nodes:
                     # Finished parsing the root node
                     state = ParseState.Finish
                     nodes.append(active)
                 else:
                     # Attach parsed node to its parent
                     parent = nodes.pop()
-                    nodes.append(parent.add(active, data=branch))
+                    nodes.append(parent.add(active, data=branch or None))
 
                     match (token := next(tokens)).kind:
                         case TokenKind.Comma:
                             state = ParseState.NodeStart
 
                         case TokenKind.CloseParen:
                             state = ParseState.NodeData
@@ -414,25 +407,25 @@
             token.start,
             token.end,
         )
 
     return nodes.pop(), token.end
 
 
-def parse(data: str) -> Node:
+def parse(data: str) -> Node[Map, Map]:
     """Parse a single tree encoded as a Newick string."""
     node, pos = parse_chain(data)
 
     if data[pos:].strip(WHITESPACE):
         raise ParseError("unexpected garbage after end of tree", pos, len(data))
 
     return node
 
 
-def parse_all(data: str) -> list[Node]:
+def parse_all(data: str) -> list[Node[Map, Map]]:
     """Parse a sequence of trees encoded as Newick strings."""
     result = []
 
     while data.strip(WHITESPACE):
         node, pos = parse_chain(data)
         result.append(node)
         data = data[pos:]
```

### Comparing `sowing-0.0.2/sowphy/newick/write.py` & `sowing-0.0.3/sowing/repr/newick/write.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,60 @@
+from immutables import Map
 from sowing.node import Node
-from sowing.traversal import Order, traverse, mapnodes
-from ..clade import Clade, Branch, Map
+from sowing.zipper import Zipper
+from sowing import traversal
 
 
 def quote_string(data: str) -> str:
     if any(char in "(),:;='\t\n" for char in data):
         return "'" + data.replace("'", "''") + "'"
 
     return data.replace(" ", "_")
 
 
 def write_props(props: Map) -> str:
+    if not props:
+        return ""
+
     return (
         "[&"
         + ",".join(
             f"{quote_string(str(key))}={quote_string(str(value))}"
             for key, value in sorted(props.items())
         )
         + "]"
     )
 
 
-def write_node(node: Node, branch: Branch | None) -> tuple[Node, None]:
+def write_node(cursor: Zipper[Map | None, Map | None]) -> Zipper[str, None]:
+    node = cursor.node
+    branch = cursor.data
+
     if node.edges:
         data = "(" + ",".join(edge.node.data for edge in node.edges) + ")"
     else:
         data = ""
 
     clade = node.data
 
-    if isinstance(clade, Clade):
-        data += quote_string(clade.name)
+    if isinstance(clade, Map):
+        if "name" in clade:
+            data += quote_string(clade["name"])
+            clade = clade.delete("name")
 
-        if clade.props:
-            data += write_props(clade.props)
+        data += write_props(clade)
 
-    if isinstance(branch, Branch):
-        if branch.length is not None or branch.props:
-            data += ":"
+    if isinstance(branch, Map) and branch:
+        data += ":"
 
-        if branch.length is not None:
-            data += f"{str(branch.length)}"
+        if "length" in branch:
+            data += f"{branch['length']}"
+            branch = branch.delete("length")
 
-        if branch.props:
-            data += write_props(branch.props)
+        data += write_props(branch)
 
-    return Node(data), None
+    return cursor.replace(node=Node(data), data=None)
 
 
-def write(root: Node) -> str:
+def write(root: Node[Map | None, Map | None]) -> str:
     """Encode a tree into a Newick string."""
-    return mapnodes(write_node, traverse(root, Order.Post)).data + ";"
+    return traversal.fold(write_node, traversal.depth(root)).data + ";"
```

### Comparing `sowing-0.0.2/LICENSE` & `sowing-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sowing-0.0.2/pyproject.toml` & `sowing-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sowing"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Mattéo Delabre", email="git.matteo@delab.re" },
 ]
 description = "sowing"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "immutables",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/UdeM-LBIT/sowing"
 "Bug Tracker" = "https://github.com/UdeM-LBIT/sowing/issues"
 
-
-# [tool.hatch.build.targets.wheel]
-# packages = [
-#     "src/sowing",
-#     "src/sowphy",
-# ]
 [tool.hatch.build]
 sources = ["src"]
 only-include = ["src"]
 
 [tool.hatch.envs.dev]
 dependencies = [
     "pytest",
```

### Comparing `sowing-0.0.2/PKG-INFO` & `sowing-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sowing
-Version: 0.0.2
+Version: 0.0.3
 Summary: sowing
 Project-URL: Homepage, https://github.com/UdeM-LBIT/sowing
 Project-URL: Bug Tracker, https://github.com/UdeM-LBIT/sowing/issues
 Author-email: Mattéo Delabre <git.matteo@delab.re>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Requires-Dist: immutables
 Description-Content-Type: text/markdown
 
 # sowing
```

