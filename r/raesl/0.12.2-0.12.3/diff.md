# Comparing `tmp/raesl-0.12.2.tar.gz` & `tmp/raesl-0.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raesl-0.12.2.tar", max compression
+gzip compressed data, was "raesl-0.12.3.tar", max compression
```

## Comparing `raesl-0.12.2.tar` & `raesl-0.12.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0    35400 2023-06-06 12:34:20.460014 raesl-0.12.2/LICENSE.rst
--rw-r--r--   0        0        0     1827 2023-06-06 12:34:20.460014 raesl-0.12.2/README.rst
--rw-r--r--   0        0        0     3015 2023-06-06 12:34:20.463014 raesl-0.12.2/pyproject.toml
--rw-r--r--   0        0        0      155 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/__init__.py
--rw-r--r--   0        0        0       64 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/__main__.py
--rw-r--r--   0        0        0      903 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/cli.py
--rw-r--r--   0        0        0     1307 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/__init__.py
--rw-r--r--   0        0        0       45 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/__init__.py
--rw-r--r--   0        0        0    17153 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/comment_storage.py
--rw-r--r--   0        0        0    16196 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/components.py
--rw-r--r--   0        0        0     6375 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/exprs.py
--rw-r--r--   0        0        0     6202 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/nodes.py
--rw-r--r--   0        0        0     1324 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/relations.py
--rw-r--r--   0        0        0    19201 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/specification.py
--rw-r--r--   0        0        0     2829 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/types.py
--rw-r--r--   0        0        0      649 2023-06-06 12:34:20.463014 raesl-0.12.2/raesl/compile/ast/verbs.py
--rw-r--r--   0        0        0     3540 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/cli.py
--rw-r--r--   0        0        0    20854 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/diagnostics.py
--rw-r--r--   0        0        0    10311 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/esl_lines.py
--rw-r--r--   0        0        0       54 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/instantiating/__init__.py
--rw-r--r--   0        0        0    63030 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/instantiating/edge_building.py
--rw-r--r--   0        0        0     1897 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/instantiating/graph_building.py
--rw-r--r--   0        0        0     1903 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/instantiating/graph_data.py
--rw-r--r--   0        0        0    16947 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/instantiating/instantation_graph_structure.yml
--rw-r--r--   0        0        0    29622 2023-06-06 12:34:20.464015 raesl-0.12.2/raesl/compile/instantiating/node_building.py
--rw-r--r--   0        0        0     1666 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/__init__.py
--rw-r--r--   0        0        0      663 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/argument_list.py
--rw-r--r--   0        0        0     8794 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/behavior.py
--rw-r--r--   0        0        0     9514 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/builder.py
--rw-r--r--   0        0        0     1179 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/comments.py
--rw-r--r--   0        0        0     1266 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/component_definitions.py
--rw-r--r--   0        0        0     2896 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/component_instances.py
--rw-r--r--   0        0        0     2787 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/designs.py
--rw-r--r--   0        0        0     3938 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/goals.py
--rw-r--r--   0        0        0     1772 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/groups.py
--rw-r--r--   0        0        0     5360 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/machine_parts.py
--rw-r--r--   0        0        0     1416 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/needs.py
--rw-r--r--   0        0        0     1805 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/parameters.py
--rw-r--r--   0        0        0     3066 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/relation_definitions.py
--rw-r--r--   0        0        0     2558 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/relation_instances.py
--rw-r--r--   0        0        0     3682 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/sub_clause.py
--rw-r--r--   0        0        0     4531 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/transforms.py
--rw-r--r--   0        0        0    12065 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/type_defs.py
--rw-r--r--   0        0        0      566 2023-06-06 12:34:20.465015 raesl-0.12.2/raesl/compile/machine_files/typing.py
--rw-r--r--   0        0        0     1700 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/machine_files/utils.py
--rw-r--r--   0        0        0     1473 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/machine_files/variables.py
--rw-r--r--   0        0        0     1171 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/machine_files/verb_defs.py
--rw-r--r--   0        0        0    11112 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/parser.py
--rw-r--r--   0        0        0    16347 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/scanner.py
--rw-r--r--   0        0        0     7418 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/state_machine.py
--rw-r--r--   0        0        0       29 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/__init__.py
--rw-r--r--   0        0        0     6565 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/ast_builder.py
--rw-r--r--   0        0        0    12213 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/compdef_behavior_builder.py
--rw-r--r--   0        0        0    18324 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/compdef_builder.py
--rw-r--r--   0        0        0     3461 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/compdef_comment_builder.py
--rw-r--r--   0        0        0     6757 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/compdef_compinst_builder.py
--rw-r--r--   0        0        0     3009 2023-06-06 12:34:20.466014 raesl-0.12.2/raesl/compile/typechecking/compdef_design_builder.py
--rw-r--r--   0        0        0     3775 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/compdef_goal_builder.py
--rw-r--r--   0        0        0     3565 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/compdef_need_builder.py
--rw-r--r--   0        0        0    16463 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/compdef_relinst_builder.py
--rw-r--r--   0        0        0     4355 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/compdef_transform_builder.py
--rw-r--r--   0        0        0     6282 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/compdef_vargroup_builder.py
--rw-r--r--   0        0        0     3925 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/compdef_varparam_builder.py
--rw-r--r--   0        0        0     6796 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/expr_checker.py
--rw-r--r--   0        0        0     8086 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/goal_transform_base.py
--rw-r--r--   0        0        0     6020 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/orderer.py
--rw-r--r--   0        0        0     7348 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/reldef_builder.py
--rw-r--r--   0        0        0    18482 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/type_builder.py
--rw-r--r--   0        0        0     9826 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/type_checker.py
--rw-r--r--   0        0        0     9158 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/utils.py
--rw-r--r--   0        0        0     2184 2023-06-06 12:34:20.467015 raesl-0.12.2/raesl/compile/typechecking/verb_builder.py
--rw-r--r--   0        0        0     1577 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/datasets/__init__.py
--rw-r--r--   0        0        0     2455 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/__init__.py
--rw-r--r--   0        0        0     2523 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/cli.py
--rw-r--r--   0        0        0    13934 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/doc.py
--rw-r--r--   0        0        0     8301 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/lines.py
--rw-r--r--   0        0        0     1456 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/locales/__init__.py
--rw-r--r--   0        0        0     7442 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/locales/en.py
--rw-r--r--   0        0        0    17968 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/locales/nl.py
--rw-r--r--   0        0        0     3710 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/rich.py
--rw-r--r--   0        0        0    18255 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/sections.py
--rw-r--r--   0        0        0     1073 2023-06-06 12:34:20.468015 raesl-0.12.2/raesl/doc/templates/background.pdf
--rw-r--r--   0        0        0    31025 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/doc/templates/eisvogel.latex
--rw-r--r--   0        0        0     4318 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/doc/utils.py
--rw-r--r--   0        0        0     2169 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/excel/__init__.py
--rw-r--r--   0        0        0     1454 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/excel/cli.py
--rw-r--r--   0        0        0     3197 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/excel/defaults.py
--rw-r--r--   0        0        0    18454 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/excel/sheets.py
--rw-r--r--   0        0        0     6367 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/excel/text.py
--rw-r--r--   0        0        0     3380 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/excel/utils.py
--rw-r--r--   0        0        0       79 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/jupyter/__init__.py
--rw-r--r--   0        0        0     2700 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/jupyter/cli.py
--rw-r--r--   0        0        0     3108 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/jupyter/kernel.py
--rw-r--r--   0        0        0      463 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/plot/__init__.py
--rw-r--r--   0        0        0    12489 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/plot/diagrams.py
--rw-r--r--   0        0        0     3834 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/plot/generic.py
--rw-r--r--   0        0        0     2438 2023-06-06 12:34:20.469015 raesl-0.12.2/raesl/plot/matrix.py
--rw-r--r--   0        0        0    16381 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/plot/utils.py
--rw-r--r--   0        0        0    12565 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/plot/view_funcs.py
--rw-r--r--   0        0        0     2474 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/pygments.py
--rw-r--r--   0        0        0      154 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/server/__init__.py
--rw-r--r--   0        0        0      821 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/server/cli.py
--rw-r--r--   0        0        0     2594 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/server/config.py
--rw-r--r--   0        0        0     6109 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/server/server.py
--rw-r--r--   0        0        0     7628 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/types.py
--rw-r--r--   0        0        0     5030 2023-06-06 12:34:20.470015 raesl-0.12.2/raesl/utils.py
--rw-r--r--   0        0        0     3677 1970-01-01 00:00:00.000000 raesl-0.12.2/PKG-INFO
+-rw-r--r--   0        0        0    35400 2023-07-04 11:47:56.761791 raesl-0.12.3/LICENSE.rst
+-rw-r--r--   0        0        0     1827 2023-07-04 11:47:56.761791 raesl-0.12.3/README.rst
+-rw-r--r--   0        0        0     3015 2023-07-04 11:47:56.763791 raesl-0.12.3/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-07-04 11:47:56.763791 raesl-0.12.3/raesl/__init__.py
+-rw-r--r--   0        0        0       64 2023-07-04 11:47:56.763791 raesl-0.12.3/raesl/__main__.py
+-rw-r--r--   0        0        0      903 2023-07-04 11:47:56.763791 raesl-0.12.3/raesl/cli.py
+-rw-r--r--   0        0        0     1307 2023-07-04 11:47:56.763791 raesl-0.12.3/raesl/compile/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-04 11:47:56.764791 raesl-0.12.3/raesl/compile/ast/__init__.py
+-rw-r--r--   0        0        0    17153 2023-07-04 11:47:56.764791 raesl-0.12.3/raesl/compile/ast/comment_storage.py
+-rw-r--r--   0        0        0    16196 2023-07-04 11:47:56.764791 raesl-0.12.3/raesl/compile/ast/components.py
+-rw-r--r--   0        0        0     6375 2023-07-04 11:47:56.764791 raesl-0.12.3/raesl/compile/ast/exprs.py
+-rw-r--r--   0        0        0     6202 2023-07-04 11:47:56.764791 raesl-0.12.3/raesl/compile/ast/nodes.py
+-rw-r--r--   0        0        0     1324 2023-07-04 11:47:56.764791 raesl-0.12.3/raesl/compile/ast/relations.py
+-rw-r--r--   0        0        0    19201 2023-07-04 11:47:56.764791 raesl-0.12.3/raesl/compile/ast/specification.py
+-rw-r--r--   0        0        0     2829 2023-07-04 11:47:56.764791 raesl-0.12.3/raesl/compile/ast/types.py
+-rw-r--r--   0        0        0      649 2023-07-04 11:47:56.764791 raesl-0.12.3/raesl/compile/ast/verbs.py
+-rw-r--r--   0        0        0     3540 2023-07-04 11:47:56.764791 raesl-0.12.3/raesl/compile/cli.py
+-rw-r--r--   0        0        0    20834 2023-07-04 11:47:56.764791 raesl-0.12.3/raesl/compile/diagnostics.py
+-rw-r--r--   0        0        0    10311 2023-07-04 11:47:56.765791 raesl-0.12.3/raesl/compile/esl_lines.py
+-rw-r--r--   0        0        0       54 2023-07-04 11:47:56.765791 raesl-0.12.3/raesl/compile/instantiating/__init__.py
+-rw-r--r--   0        0        0    63030 2023-07-04 11:47:56.765791 raesl-0.12.3/raesl/compile/instantiating/edge_building.py
+-rw-r--r--   0        0        0     1897 2023-07-04 11:47:56.765791 raesl-0.12.3/raesl/compile/instantiating/graph_building.py
+-rw-r--r--   0        0        0     1903 2023-07-04 11:47:56.765791 raesl-0.12.3/raesl/compile/instantiating/graph_data.py
+-rw-r--r--   0        0        0    16947 2023-07-04 11:47:56.765791 raesl-0.12.3/raesl/compile/instantiating/instantation_graph_structure.yml
+-rw-r--r--   0        0        0    29622 2023-07-04 11:47:56.765791 raesl-0.12.3/raesl/compile/instantiating/node_building.py
+-rw-r--r--   0        0        0     1666 2023-07-04 11:47:56.765791 raesl-0.12.3/raesl/compile/machine_files/__init__.py
+-rw-r--r--   0        0        0      663 2023-07-04 11:47:56.765791 raesl-0.12.3/raesl/compile/machine_files/argument_list.py
+-rw-r--r--   0        0        0     8794 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/behavior.py
+-rw-r--r--   0        0        0     9514 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/builder.py
+-rw-r--r--   0        0        0     1179 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/comments.py
+-rw-r--r--   0        0        0     1266 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/component_definitions.py
+-rw-r--r--   0        0        0     2896 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/component_instances.py
+-rw-r--r--   0        0        0     2787 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/designs.py
+-rw-r--r--   0        0        0     3938 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/goals.py
+-rw-r--r--   0        0        0     1772 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/groups.py
+-rw-r--r--   0        0        0     5360 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/machine_parts.py
+-rw-r--r--   0        0        0     1416 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/needs.py
+-rw-r--r--   0        0        0     1805 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/parameters.py
+-rw-r--r--   0        0        0     3066 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/relation_definitions.py
+-rw-r--r--   0        0        0     2558 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/relation_instances.py
+-rw-r--r--   0        0        0     3682 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/sub_clause.py
+-rw-r--r--   0        0        0     4531 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/transforms.py
+-rw-r--r--   0        0        0    12065 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/type_defs.py
+-rw-r--r--   0        0        0      566 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/typing.py
+-rw-r--r--   0        0        0     1700 2023-07-04 11:47:56.766791 raesl-0.12.3/raesl/compile/machine_files/utils.py
+-rw-r--r--   0        0        0     1473 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/machine_files/variables.py
+-rw-r--r--   0        0        0     1171 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/machine_files/verb_defs.py
+-rw-r--r--   0        0        0    11112 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/parser.py
+-rw-r--r--   0        0        0    16347 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/scanner.py
+-rw-r--r--   0        0        0     7418 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/state_machine.py
+-rw-r--r--   0        0        0       29 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/typechecking/__init__.py
+-rw-r--r--   0        0        0     6565 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/typechecking/ast_builder.py
+-rw-r--r--   0        0        0    12213 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/typechecking/compdef_behavior_builder.py
+-rw-r--r--   0        0        0    18324 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/typechecking/compdef_builder.py
+-rw-r--r--   0        0        0     3461 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/typechecking/compdef_comment_builder.py
+-rw-r--r--   0        0        0     6757 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/typechecking/compdef_compinst_builder.py
+-rw-r--r--   0        0        0     3009 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/typechecking/compdef_design_builder.py
+-rw-r--r--   0        0        0     3775 2023-07-04 11:47:56.767791 raesl-0.12.3/raesl/compile/typechecking/compdef_goal_builder.py
+-rw-r--r--   0        0        0     3565 2023-07-04 11:47:56.768791 raesl-0.12.3/raesl/compile/typechecking/compdef_need_builder.py
+-rw-r--r--   0        0        0    16463 2023-07-04 11:47:56.768791 raesl-0.12.3/raesl/compile/typechecking/compdef_relinst_builder.py
+-rw-r--r--   0        0        0     4355 2023-07-04 11:47:56.768791 raesl-0.12.3/raesl/compile/typechecking/compdef_transform_builder.py
+-rw-r--r--   0        0        0     6282 2023-07-04 11:47:56.768791 raesl-0.12.3/raesl/compile/typechecking/compdef_vargroup_builder.py
+-rw-r--r--   0        0        0     3925 2023-07-04 11:47:56.768791 raesl-0.12.3/raesl/compile/typechecking/compdef_varparam_builder.py
+-rw-r--r--   0        0        0     6796 2023-07-04 11:47:56.768791 raesl-0.12.3/raesl/compile/typechecking/expr_checker.py
+-rw-r--r--   0        0        0     8086 2023-07-04 11:47:56.768791 raesl-0.12.3/raesl/compile/typechecking/goal_transform_base.py
+-rw-r--r--   0        0        0     6020 2023-07-04 11:47:56.768791 raesl-0.12.3/raesl/compile/typechecking/orderer.py
+-rw-r--r--   0        0        0     7348 2023-07-04 11:47:56.768791 raesl-0.12.3/raesl/compile/typechecking/reldef_builder.py
+-rw-r--r--   0        0        0    18482 2023-07-04 11:47:56.768791 raesl-0.12.3/raesl/compile/typechecking/type_builder.py
+-rw-r--r--   0        0        0     9826 2023-07-04 11:47:56.768791 raesl-0.12.3/raesl/compile/typechecking/type_checker.py
+-rw-r--r--   0        0        0     9158 2023-07-04 11:47:56.768791 raesl-0.12.3/raesl/compile/typechecking/utils.py
+-rw-r--r--   0        0        0     2184 2023-07-04 11:47:56.769791 raesl-0.12.3/raesl/compile/typechecking/verb_builder.py
+-rw-r--r--   0        0        0     1577 2023-07-04 11:47:56.769791 raesl-0.12.3/raesl/datasets/__init__.py
+-rw-r--r--   0        0        0     2455 2023-07-04 11:47:56.769791 raesl-0.12.3/raesl/doc/__init__.py
+-rw-r--r--   0        0        0     2523 2023-07-04 11:47:56.769791 raesl-0.12.3/raesl/doc/cli.py
+-rw-r--r--   0        0        0    13934 2023-07-04 11:47:56.769791 raesl-0.12.3/raesl/doc/doc.py
+-rw-r--r--   0        0        0     8301 2023-07-04 11:47:56.769791 raesl-0.12.3/raesl/doc/lines.py
+-rw-r--r--   0        0        0     1456 2023-07-04 11:47:56.769791 raesl-0.12.3/raesl/doc/locales/__init__.py
+-rw-r--r--   0        0        0     7442 2023-07-04 11:47:56.769791 raesl-0.12.3/raesl/doc/locales/en.py
+-rw-r--r--   0        0        0    17968 2023-07-04 11:47:56.769791 raesl-0.12.3/raesl/doc/locales/nl.py
+-rw-r--r--   0        0        0     3710 2023-07-04 11:47:56.769791 raesl-0.12.3/raesl/doc/rich.py
+-rw-r--r--   0        0        0    18255 2023-07-04 11:47:56.769791 raesl-0.12.3/raesl/doc/sections.py
+-rw-r--r--   0        0        0     1073 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/doc/templates/background.pdf
+-rw-r--r--   0        0        0    31025 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/doc/templates/eisvogel.latex
+-rw-r--r--   0        0        0     4318 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/doc/utils.py
+-rw-r--r--   0        0        0     2169 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/excel/__init__.py
+-rw-r--r--   0        0        0     1454 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/excel/cli.py
+-rw-r--r--   0        0        0     3197 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/excel/defaults.py
+-rw-r--r--   0        0        0    18454 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/excel/sheets.py
+-rw-r--r--   0        0        0     6367 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/excel/text.py
+-rw-r--r--   0        0        0     3380 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/excel/utils.py
+-rw-r--r--   0        0        0       79 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/jupyter/__init__.py
+-rw-r--r--   0        0        0     2700 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/jupyter/cli.py
+-rw-r--r--   0        0        0     3108 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/jupyter/kernel.py
+-rw-r--r--   0        0        0      463 2023-07-04 11:47:56.770791 raesl-0.12.3/raesl/plot/__init__.py
+-rw-r--r--   0        0        0    12489 2023-07-04 11:47:56.771791 raesl-0.12.3/raesl/plot/diagrams.py
+-rw-r--r--   0        0        0     3834 2023-07-04 11:47:56.771791 raesl-0.12.3/raesl/plot/generic.py
+-rw-r--r--   0        0        0     2438 2023-07-04 11:47:56.771791 raesl-0.12.3/raesl/plot/matrix.py
+-rw-r--r--   0        0        0    16381 2023-07-04 11:47:56.771791 raesl-0.12.3/raesl/plot/utils.py
+-rw-r--r--   0        0        0    12565 2023-07-04 11:47:56.771791 raesl-0.12.3/raesl/plot/view_funcs.py
+-rw-r--r--   0        0        0     2474 2023-07-04 11:47:56.771791 raesl-0.12.3/raesl/pygments.py
+-rw-r--r--   0        0        0      154 2023-07-04 11:47:56.771791 raesl-0.12.3/raesl/server/__init__.py
+-rw-r--r--   0        0        0      821 2023-07-04 11:47:56.771791 raesl-0.12.3/raesl/server/cli.py
+-rw-r--r--   0        0        0     2594 2023-07-04 11:47:56.771791 raesl-0.12.3/raesl/server/config.py
+-rw-r--r--   0        0        0     6109 2023-07-04 11:47:56.771791 raesl-0.12.3/raesl/server/server.py
+-rw-r--r--   0        0        0     7628 2023-07-04 11:47:56.771791 raesl-0.12.3/raesl/types.py
+-rw-r--r--   0        0        0     5030 2023-07-04 11:47:56.771791 raesl-0.12.3/raesl/utils.py
+-rw-r--r--   0        0        0     3677 1970-01-01 00:00:00.000000 raesl-0.12.3/PKG-INFO
```

### Comparing `raesl-0.12.2/LICENSE.rst` & `raesl-0.12.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/README.rst` & `raesl-0.12.3/README.rst`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/pyproject.toml` & `raesl-0.12.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "raesl"
-version = "0.12.2"
+version = "0.12.3"
 description = "Ratio ESL support in Python."
 authors = ["Ratio Innovations B.V. <info@ratio-case.nl>"]
 license = "GPL-3.0-or-later"
 documentation = "https://raesl.ratio-case.nl"
 readme = "README.rst"
 repository = "https://gitlab.com/ratio-case-os/python/raesl"
 homepage = "https://raesl.ratio-case.nl"
```

### Comparing `raesl-0.12.2/raesl/cli.py` & `raesl-0.12.3/raesl/cli.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/__init__.py` & `raesl-0.12.3/raesl/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/ast/comment_storage.py` & `raesl-0.12.3/raesl/compile/ast/comment_storage.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/ast/components.py` & `raesl-0.12.3/raesl/compile/ast/components.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/ast/exprs.py` & `raesl-0.12.3/raesl/compile/ast/exprs.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/ast/nodes.py` & `raesl-0.12.3/raesl/compile/ast/nodes.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/ast/relations.py` & `raesl-0.12.3/raesl/compile/ast/relations.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/ast/specification.py` & `raesl-0.12.3/raesl/compile/ast/specification.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/ast/types.py` & `raesl-0.12.3/raesl/compile/ast/types.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/ast/verbs.py` & `raesl-0.12.3/raesl/compile/ast/verbs.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/cli.py` & `raesl-0.12.3/raesl/compile/cli.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/diagnostics.py` & `raesl-0.12.3/raesl/compile/diagnostics.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
         #100: Scanning/Parsing
         #200: Typechecking
         #300: AST Builder
         #400: Instance/output builder
 """
 
 import sys
-from typing import Iterable, List, Optional
-from typing.io import IO
+from typing import IO, Iterable, List, Optional
 
 import click
+
 from raesl import logger, utils
 from raesl.types import (
     Diagnostic,
     DiagnosticRelatedInformation,
     DiagnosticSeverity,
     Location,
 )
```

### Comparing `raesl-0.12.2/raesl/compile/esl_lines.py` & `raesl-0.12.3/raesl/compile/esl_lines.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/instantiating/edge_building.py` & `raesl-0.12.3/raesl/compile/instantiating/edge_building.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/instantiating/graph_building.py` & `raesl-0.12.3/raesl/compile/instantiating/graph_building.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/instantiating/graph_data.py` & `raesl-0.12.3/raesl/compile/instantiating/graph_data.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/instantiating/instantation_graph_structure.yml` & `raesl-0.12.3/raesl/compile/instantiating/instantation_graph_structure.yml`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/instantiating/node_building.py` & `raesl-0.12.3/raesl/compile/instantiating/node_building.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/__init__.py` & `raesl-0.12.3/raesl/compile/machine_files/__init__.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/argument_list.py` & `raesl-0.12.3/raesl/compile/machine_files/argument_list.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/behavior.py` & `raesl-0.12.3/raesl/compile/machine_files/behavior.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/builder.py` & `raesl-0.12.3/raesl/compile/machine_files/builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/comments.py` & `raesl-0.12.3/raesl/compile/machine_files/comments.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/component_definitions.py` & `raesl-0.12.3/raesl/compile/machine_files/component_definitions.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/component_instances.py` & `raesl-0.12.3/raesl/compile/machine_files/component_instances.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/designs.py` & `raesl-0.12.3/raesl/compile/machine_files/designs.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/goals.py` & `raesl-0.12.3/raesl/compile/machine_files/goals.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/groups.py` & `raesl-0.12.3/raesl/compile/machine_files/groups.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/machine_parts.py` & `raesl-0.12.3/raesl/compile/machine_files/machine_parts.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/needs.py` & `raesl-0.12.3/raesl/compile/machine_files/needs.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/parameters.py` & `raesl-0.12.3/raesl/compile/machine_files/parameters.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/relation_definitions.py` & `raesl-0.12.3/raesl/compile/machine_files/relation_definitions.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/relation_instances.py` & `raesl-0.12.3/raesl/compile/machine_files/relation_instances.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/sub_clause.py` & `raesl-0.12.3/raesl/compile/machine_files/sub_clause.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/transforms.py` & `raesl-0.12.3/raesl/compile/machine_files/transforms.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/type_defs.py` & `raesl-0.12.3/raesl/compile/machine_files/type_defs.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/typing.py` & `raesl-0.12.3/raesl/compile/machine_files/typing.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/utils.py` & `raesl-0.12.3/raesl/compile/machine_files/utils.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/variables.py` & `raesl-0.12.3/raesl/compile/machine_files/variables.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/machine_files/verb_defs.py` & `raesl-0.12.3/raesl/compile/machine_files/verb_defs.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/parser.py` & `raesl-0.12.3/raesl/compile/parser.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/scanner.py` & `raesl-0.12.3/raesl/compile/scanner.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/state_machine.py` & `raesl-0.12.3/raesl/compile/state_machine.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/ast_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/ast_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/compdef_behavior_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/compdef_behavior_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/compdef_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/compdef_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/compdef_comment_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/compdef_comment_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/compdef_compinst_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/compdef_compinst_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/compdef_design_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/compdef_design_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/compdef_goal_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/compdef_goal_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/compdef_need_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/compdef_need_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/compdef_relinst_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/compdef_relinst_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/compdef_transform_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/compdef_transform_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/compdef_vargroup_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/compdef_vargroup_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/compdef_varparam_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/compdef_varparam_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/expr_checker.py` & `raesl-0.12.3/raesl/compile/typechecking/expr_checker.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/goal_transform_base.py` & `raesl-0.12.3/raesl/compile/typechecking/goal_transform_base.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/orderer.py` & `raesl-0.12.3/raesl/compile/typechecking/orderer.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/reldef_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/reldef_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/type_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/type_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/type_checker.py` & `raesl-0.12.3/raesl/compile/typechecking/type_checker.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/utils.py` & `raesl-0.12.3/raesl/compile/typechecking/utils.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/compile/typechecking/verb_builder.py` & `raesl-0.12.3/raesl/compile/typechecking/verb_builder.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/datasets/__init__.py` & `raesl-0.12.3/raesl/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/doc/__init__.py` & `raesl-0.12.3/raesl/doc/__init__.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/doc/cli.py` & `raesl-0.12.3/raesl/doc/cli.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/doc/doc.py` & `raesl-0.12.3/raesl/doc/doc.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/doc/lines.py` & `raesl-0.12.3/raesl/doc/lines.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/doc/locales/__init__.py` & `raesl-0.12.3/raesl/doc/locales/__init__.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/doc/locales/en.py` & `raesl-0.12.3/raesl/doc/locales/en.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/doc/locales/nl.py` & `raesl-0.12.3/raesl/doc/locales/nl.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/doc/rich.py` & `raesl-0.12.3/raesl/doc/rich.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/doc/sections.py` & `raesl-0.12.3/raesl/doc/sections.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/doc/templates/background.pdf` & `raesl-0.12.3/raesl/doc/templates/background.pdf`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/doc/templates/eisvogel.latex` & `raesl-0.12.3/raesl/doc/templates/eisvogel.latex`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/doc/utils.py` & `raesl-0.12.3/raesl/doc/utils.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/excel/__init__.py` & `raesl-0.12.3/raesl/excel/__init__.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/excel/cli.py` & `raesl-0.12.3/raesl/excel/cli.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/excel/defaults.py` & `raesl-0.12.3/raesl/excel/defaults.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/excel/sheets.py` & `raesl-0.12.3/raesl/excel/sheets.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/excel/text.py` & `raesl-0.12.3/raesl/excel/text.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/excel/utils.py` & `raesl-0.12.3/raesl/excel/utils.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/jupyter/cli.py` & `raesl-0.12.3/raesl/jupyter/cli.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/jupyter/kernel.py` & `raesl-0.12.3/raesl/jupyter/kernel.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/plot/diagrams.py` & `raesl-0.12.3/raesl/plot/diagrams.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/plot/generic.py` & `raesl-0.12.3/raesl/plot/generic.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/plot/matrix.py` & `raesl-0.12.3/raesl/plot/matrix.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/plot/utils.py` & `raesl-0.12.3/raesl/plot/utils.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/plot/view_funcs.py` & `raesl-0.12.3/raesl/plot/view_funcs.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/pygments.py` & `raesl-0.12.3/raesl/pygments.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/server/cli.py` & `raesl-0.12.3/raesl/server/cli.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/server/config.py` & `raesl-0.12.3/raesl/server/config.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/server/server.py` & `raesl-0.12.3/raesl/server/server.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/types.py` & `raesl-0.12.3/raesl/types.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/raesl/utils.py` & `raesl-0.12.3/raesl/utils.py`

 * *Files identical despite different names*

### Comparing `raesl-0.12.2/PKG-INFO` & `raesl-0.12.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raesl
-Version: 0.12.2
+Version: 0.12.3
 Summary: Ratio ESL support in Python.
 Home-page: https://raesl.ratio-case.nl
 License: GPL-3.0-or-later
 Author: Ratio Innovations B.V.
 Author-email: info@ratio-case.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

