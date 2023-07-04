# Comparing `tmp/cashocs-2.0.6.tar.gz` & `tmp/cashocs-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashocs-2.0.6.tar", last modified: Tue Jul  4 06:39:37 2023, max compression
+gzip compressed data, was "cashocs-2.0.7.tar", last modified: Tue Jul  4 06:59:39 2023, max compression
```

## Comparing `cashocs-2.0.6.tar` & `cashocs-2.0.7.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.321548 cashocs-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-04 06:39:26.000000 cashocs-2.0.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-07-04 06:39:37.317548 cashocs-2.0.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    11556 2023-07-04 06:39:26.000000 cashocs-2.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.289548 cashocs-2.0.6/cashocs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4546 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.289548 cashocs-2.0.6/cashocs/_cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11080 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_cli/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.293547 cashocs-2.0.6/cashocs/_constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_constraints/constrained_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_constraints/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_constraints/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.293547 cashocs-2.0.6/cashocs/_database/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_database/form_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_database/function_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_database/geometry_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_database/parameter_database.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.293547 cashocs-2.0.6/cashocs/_forms/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_forms/control_form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_forms/form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_forms/general_form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_forms/shape_form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_forms/shape_regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.297548 cashocs-2.0.6/cashocs/_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/cost_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.297548 cashocs-2.0.6/cashocs/_optimization/line_search/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/line_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/line_search/armijo_line_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/line_search/line_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/line_search/polynomial_line_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.297548 cashocs-2.0.6/cashocs/_optimization/optimal_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimal_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimal_control/box_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimal_control/control_variable_abstractions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21968 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimal_control/optimal_control_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.297548 cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/gradient_descent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13523 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/l_bfgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/ncg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/newton.py
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30174 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/optimization_variable_abstractions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.301548 cashocs-2.0.6/cashocs/_optimization/shape_optimization/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/shape_optimization/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24593 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/shape_optimization/shape_optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.301548 cashocs-2.0.6/cashocs/_optimization/topology_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/topology_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/topology_optimization/topology_optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_optimization/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.301548 cashocs-2.0.6/cashocs/_pde_problems/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_pde_problems/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5602 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_pde_problems/adjoint_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4272 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_pde_problems/control_gradient_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17636 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_pde_problems/hessian_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_pde_problems/pde_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9445 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_pde_problems/shape_gradient_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7315 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_pde_problems/state_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.301548 cashocs-2.0.6/cashocs/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_utils/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_utils/interpolations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/_utils/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.305548 cashocs-2.0.6/cashocs/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/geometry/boundary_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/geometry/deformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/geometry/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/geometry/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    27202 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/geometry/mesh_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/geometry/mesh_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/geometry/quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.305548 cashocs-2.0.6/cashocs/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31412 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/io/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/io/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/io/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/io/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/io/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.305548 cashocs-2.0.6/cashocs/nonlinear_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/nonlinear_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/nonlinear_solvers/linear_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20189 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/nonlinear_solvers/newton_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/nonlinear_solvers/picard_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.305548 cashocs-2.0.6/cashocs/space_mapping/
--rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/space_mapping/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36090 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/space_mapping/optimal_control.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37353 2023-07-04 06:39:26.000000 cashocs-2.0.6/cashocs/space_mapping/shape_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.289548 cashocs-2.0.6/cashocs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-07-04 06:39:37.000000 cashocs-2.0.6/cashocs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-07-04 06:39:37.000000 cashocs-2.0.6/cashocs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 06:39:37.000000 cashocs-2.0.6/cashocs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 06:39:37.000000 cashocs-2.0.6/cashocs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-04 06:39:37.000000 cashocs-2.0.6/cashocs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-04 06:39:37.000000 cashocs-2.0.6/cashocs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.285548 cashocs-2.0.6/demos/documented/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.281547 cashocs-2.0.6/demos/documented/cashocs_as_solver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/cashocs_as_solver/control_solver/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7337 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/cashocs_as_solver/shape_solver/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7435 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.281547 cashocs-2.0.6/demos/documented/misc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/misc/xdmf_io/
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/misc/xdmf_io/demo_xdmf_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.285548 cashocs-2.0.6/demos/documented/optimal_control/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/box_constraints/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5446 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/box_constraints/demo_box_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/constraints/demo_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/control_boundary_conditions/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4275 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/dirichlet_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8210 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/heat_equation/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9065 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/heat_equation/demo_heat_equation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/iterative_solvers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7592 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/monolithic_problems/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6418 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/multiple_variables/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8060 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/neumann_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5126 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/neumann_control/demo_neumann_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/nonlinear_pdes/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4503 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/picard_iteration/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/poisson/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11431 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/poisson/demo_poisson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/pre_post_callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/scalar_control_tracking/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4956 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.309548 cashocs-2.0.6/demos/documented/optimal_control/sparse_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3548 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/sparse_control/demo_sparse_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/optimal_control/state_constraints/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6613 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/state_constraints/demo_state_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/optimal_control/stokes/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7851 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/optimal_control/stokes/demo_stokes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.285548 cashocs-2.0.6/demos/documented/shape_optimization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/shape_optimization/custom_scalar_product/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4286 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/shape_optimization/eikonal_stiffness/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5751 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/shape_optimization/inverse_tomography/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13339 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/shape_optimization/p_laplacian/
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/shape_optimization/regularization/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5411 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/shape_optimization/regularization/demo_regularization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/shape_optimization/remeshing/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9530 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/shape_optimization/remeshing/demo_remeshing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/shape_optimization/scaling/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5615 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/shape_optimization/scaling/demo_scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/shape_optimization/shape_poisson/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/shape_optimization/shape_stokes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10178 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/shape_optimization/space_mapping_semilinear_transmission/
--rw-r--r--   0 runner    (1001) docker     (123)    16551 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)    20027 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/test_mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.285548 cashocs-2.0.6/demos/undocumented/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.285548 cashocs-2.0.6/demos/undocumented/optimal_control/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/undocumented/optimal_control/different_state_adjoint_spaces/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2535 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.285548 cashocs-2.0.6/demos/undocumented/shape_optimization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/undocumented/shape_optimization/custom_functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/undocumented/shape_optimization/custom_functional/custom_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/demos/undocumented/shape_optimization/pipe_optimization/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2048 2023-07-04 06:39:26.000000 cashocs-2.0.6/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.285548 cashocs-2.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.313548 cashocs-2.0.6/docs/source/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4747 2023-07-04 06:39:26.000000 cashocs-2.0.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-04 06:39:26.000000 cashocs-2.0.6/docs/source/jupytext_process.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3175 2023-07-04 06:39:26.000000 cashocs-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 06:39:37.321548 cashocs-2.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:39:37.317548 cashocs-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7691 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_control_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19502 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2945 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_log_level.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_nonlinear_solvers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25296 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_optimal_control.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6571 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_optimal_control_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_optimal_control_space_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_p_laplacian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_pde_problems.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9455 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_picard_iterations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7247 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_remeshing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_shape_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40730 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_shape_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_shape_optimization_space_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_topology_optimization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8955 2023-07-04 06:39:26.000000 cashocs-2.0.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.447105 cashocs-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-04 06:59:28.000000 cashocs-2.0.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-07-04 06:59:39.447105 cashocs-2.0.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11025 2023-07-04 06:59:28.000000 cashocs-2.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.431105 cashocs-2.0.7/cashocs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4546 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.431105 cashocs-2.0.7/cashocs/_cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11080 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_cli/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.431105 cashocs-2.0.7/cashocs/_constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_constraints/constrained_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_constraints/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_constraints/solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.431105 cashocs-2.0.7/cashocs/_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_database/form_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_database/function_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_database/geometry_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_database/parameter_database.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.431105 cashocs-2.0.7/cashocs/_forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_forms/control_form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_forms/form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_forms/general_form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_forms/shape_form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_forms/shape_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.435105 cashocs-2.0.7/cashocs/_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/cost_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.435105 cashocs-2.0.7/cashocs/_optimization/line_search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/line_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/line_search/armijo_line_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/line_search/line_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/line_search/polynomial_line_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.435105 cashocs-2.0.7/cashocs/_optimization/optimal_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimal_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimal_control/box_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimal_control/control_variable_abstractions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21515 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimal_control/optimal_control_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.435105 cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/gradient_descent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13523 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/l_bfgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/ncg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29701 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/optimization_variable_abstractions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.435105 cashocs-2.0.7/cashocs/_optimization/shape_optimization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/shape_optimization/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24150 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/shape_optimization/shape_optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.435105 cashocs-2.0.7/cashocs/_optimization/topology_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/topology_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/topology_optimization/topology_optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_optimization/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.439105 cashocs-2.0.7/cashocs/_pde_problems/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_pde_problems/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5602 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_pde_problems/adjoint_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4272 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_pde_problems/control_gradient_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17636 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_pde_problems/hessian_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_pde_problems/pde_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9445 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_pde_problems/shape_gradient_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7315 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_pde_problems/state_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.439105 cashocs-2.0.7/cashocs/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_utils/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_utils/interpolations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/_utils/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.439105 cashocs-2.0.7/cashocs/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/geometry/boundary_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/geometry/deformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/geometry/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/geometry/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27202 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/geometry/mesh_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/geometry/mesh_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/geometry/quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.439105 cashocs-2.0.7/cashocs/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31284 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/io/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/io/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/io/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/io/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.439105 cashocs-2.0.7/cashocs/nonlinear_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/nonlinear_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/nonlinear_solvers/linear_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20189 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/nonlinear_solvers/newton_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/nonlinear_solvers/picard_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.439105 cashocs-2.0.7/cashocs/space_mapping/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/space_mapping/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36090 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/space_mapping/optimal_control.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37353 2023-07-04 06:59:28.000000 cashocs-2.0.7/cashocs/space_mapping/shape_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.431105 cashocs-2.0.7/cashocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-07-04 06:59:39.000000 cashocs-2.0.7/cashocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-07-04 06:59:39.000000 cashocs-2.0.7/cashocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 06:59:39.000000 cashocs-2.0.7/cashocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 06:59:39.000000 cashocs-2.0.7/cashocs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-04 06:59:39.000000 cashocs-2.0.7/cashocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-04 06:59:39.000000 cashocs-2.0.7/cashocs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.439105 cashocs-2.0.7/demos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.427105 cashocs-2.0.7/demos/documented/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.427105 cashocs-2.0.7/demos/documented/cashocs_as_solver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.439105 cashocs-2.0.7/demos/documented/cashocs_as_solver/control_solver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7337 2023-07-04 06:59:28.000000 cashocs-2.0.7/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.439105 cashocs-2.0.7/demos/documented/cashocs_as_solver/shape_solver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7435 2023-07-04 06:59:28.000000 cashocs-2.0.7/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.427105 cashocs-2.0.7/demos/documented/misc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.439105 cashocs-2.0.7/demos/documented/misc/xdmf_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-04 06:59:28.000000 cashocs-2.0.7/demos/documented/misc/xdmf_io/demo_xdmf_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.427105 cashocs-2.0.7/demos/documented/optimal_control/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.439105 cashocs-2.0.7/demos/documented/optimal_control/box_constraints/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5454 2023-07-04 06:59:28.000000 cashocs-2.0.7/demos/documented/optimal_control/box_constraints/demo_box_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-04 06:59:28.000000 cashocs-2.0.7/demos/documented/optimal_control/constraints/demo_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/control_boundary_conditions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4275 2023-07-04 06:59:28.000000 cashocs-2.0.7/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/dirichlet_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8210 2023-07-04 06:59:28.000000 cashocs-2.0.7/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/heat_equation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9065 2023-07-04 06:59:28.000000 cashocs-2.0.7/demos/documented/optimal_control/heat_equation/demo_heat_equation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/iterative_solvers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7592 2023-07-04 06:59:28.000000 cashocs-2.0.7/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/monolithic_problems/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6418 2023-07-04 06:59:28.000000 cashocs-2.0.7/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/multiple_variables/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8060 2023-07-04 06:59:28.000000 cashocs-2.0.7/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/neumann_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5126 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/optimal_control/neumann_control/demo_neumann_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/nonlinear_pdes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4503 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/picard_iteration/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/poisson/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11431 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/optimal_control/poisson/demo_poisson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/pre_post_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/scalar_control_tracking/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4956 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/sparse_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3548 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/optimal_control/sparse_control/demo_sparse_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/state_constraints/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6613 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/optimal_control/state_constraints/demo_state_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/optimal_control/stokes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7851 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/optimal_control/stokes/demo_stokes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.427105 cashocs-2.0.7/demos/documented/shape_optimization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/shape_optimization/custom_scalar_product/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4286 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/shape_optimization/eikonal_stiffness/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5751 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/shape_optimization/inverse_tomography/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13339 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/shape_optimization/p_laplacian/
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/shape_optimization/regularization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5411 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/shape_optimization/regularization/demo_regularization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/shape_optimization/remeshing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9530 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/shape_optimization/remeshing/demo_remeshing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/shape_optimization/scaling/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5615 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/shape_optimization/scaling/demo_scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/shape_optimization/shape_poisson/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/shape_optimization/shape_stokes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10178 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/shape_optimization/space_mapping_semilinear_transmission/
+-rw-r--r--   0 runner    (1001) docker     (123)    16551 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)    20027 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/test_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.427105 cashocs-2.0.7/demos/undocumented/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.427105 cashocs-2.0.7/demos/undocumented/optimal_control/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/undocumented/optimal_control/different_state_adjoint_spaces/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2535 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.427105 cashocs-2.0.7/demos/undocumented/shape_optimization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/undocumented/shape_optimization/custom_functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/undocumented/shape_optimization/custom_functional/custom_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/demos/undocumented/shape_optimization/pipe_optimization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2048 2023-07-04 06:59:29.000000 cashocs-2.0.7/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.427105 cashocs-2.0.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.443105 cashocs-2.0.7/docs/source/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4747 2023-07-04 06:59:29.000000 cashocs-2.0.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-04 06:59:29.000000 cashocs-2.0.7/docs/source/jupytext_process.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3175 2023-07-04 06:59:29.000000 cashocs-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 06:59:39.447105 cashocs-2.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 06:59:39.447105 cashocs-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7691 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_control_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19518 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2945 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_log_level.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_nonlinear_solvers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25328 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_optimal_control.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6571 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_optimal_control_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_optimal_control_space_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_p_laplacian.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_pde_problems.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9455 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_picard_iterations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7247 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_remeshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_shape_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40742 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_shape_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_shape_optimization_space_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_topology_optimization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8955 2023-07-04 06:59:29.000000 cashocs-2.0.7/tests/test_utils.py
```

### Comparing `cashocs-2.0.6/COPYING` & `cashocs-2.0.7/COPYING`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/PKG-INFO` & `cashocs-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: cashocs
-Version: 2.0.6
+Version: 2.0.7
 Summary: Computational Adjoint-Based Shape Optimization and Optimal Control Software
 Author: Sebastian Blauth
 Author-email: sebastian.blauth@itwm.fraunhofer.de
 License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: Documentation, https://cashocs.readthedocs.io/en/stable
+Project-URL: Documentation, https://cashocs.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/sblauth/cashocs
-Project-URL: Tutorial, https://cashocs.readthedocs.io/en/stable/user
+Project-URL: Tutorial, https://cashocs.readthedocs.io/en/latest/user
 Project-URL: Tracker, https://github.com/sblauth/cashocs/issues
 Keywords: Shape Optimization,Optimal Control,FEniCS,Optimization,PDE,Adjoint,Finite Element Method
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -98,15 +98,15 @@
     - `Hinze, Ulbrich, Ulbrich, and Pinnau - Optimization with PDE Constraints <https://doi.org/10.1007/978-1-4020-8839-1>`_
     - `Tröltzsch - Optimal Control of Partial Differential Equations <https://doi.org/10.1090/gsm/112>`_
 - Shape Optimization
     - `Delfour and Zolesio - Shapes and Geometries <https://doi.org/10.1137/1.9780898719826>`_
     - `Sokolowski and Zolesio - Introduction to Shape Optimization <https://doi.org/10.1007/978-3-642-58106-9>`_
 - FEniCS
     - `Logg, Mardal, and Wells - Automated Solution of Differential Equations by the Finite Element Method <https://doi.org/10.1007/978-3-642-23099-8>`_
-    - `The FEniCS demos <https://fenicsproject.org/olddocs/dolfin/2019.1.0/python/demos.html>`_
+    - `The FEniCS demos <https://fenicsproject.org/docs/dolfin/latest/python/demos.html>`_
 
 .. readme_end_disclaimer
 
 However, the `cashocs tutorial <https://cashocs.readthedocs.io/en/latest/user>`_ also gives many references either
 to the underlying theory of PDE constrained optimization or to relevant demos
 and documentation of FEniCS.
 
@@ -228,32 +228,23 @@
 
 .. readme_start_citing
 .. _citing:
 
 Citing
 ======
 
-If you use cashocs for your research, please cite the following paper
+If you use cashocs for your research, I would be grateful if you would cite the following paper
 
 .. code-block:: text
 
 	cashocs: A Computational, Adjoint-Based Shape Optimization and Optimal Control Software
 	Sebastian Blauth
 	SoftwareX, Volume 13, 2021
 	https://doi.org/10.1016/j.softx.2020.100646
 
-as well as the preprint
-
-.. code-block:: text
-
-	Version 2.0 - cashocs: A Computational, Adjoint-Based Shape Optimization and Optimal Control Software
-	Sebastian Blauth
-	https://doi.org/10.48550/arXiv.2306.09828
-
-
 Additionally, if you are using the nonlinear conjugate gradient methods for shape optimization implemented in cashocs, please cite the following paper
 	
 .. code-block:: text
 
 	Nonlinear Conjugate Gradient Methods for PDE Constrained Shape Optimization Based on Steklov--Poincaré-Type Metrics
 	Sebastian Blauth
 	SIAM Journal on Optimization, Volume 31, Issue 3, 2021
@@ -288,26 +279,14 @@
 	  issn     = {2352-7110},
 	  pages    = {100646},
 	  volume   = {13},
 	  doi      = {https://doi.org/10.1016/j.softx.2020.100646},
 	  keywords = {PDE constrained optimization, Adjoint approach, Shape optimization, Optimal control},
 	}
 
-.. code-block:: bibtex
-
-	@Misc{Blauth2023Version,
-	  author        = {Sebastian Blauth},
-	  title         = {{Version 2.0 -- cashocs: A Computational, Adjoint-Based Shape Optimization and Optimal Control Software}},
-	  year          = {2023},
-	  archiveprefix = {arXiv},
-	  eprint        = {2306.09828},
-	  primaryclass  = {math.OC},
-	}
-
-
 
 .. code-block:: bibtex
 
 	@Article{Blauth2021Nonlinear,
 		author   = {Sebastian Blauth},
 		journal  = {SIAM J. Optim.},
 		title    = {{N}onlinear {C}onjugate {G}radient {M}ethods for {PDE} {C}onstrained {S}hape {O}ptimization {B}ased on {S}teklov-{P}oincaré-{T}ype {M}etrics},
```

### Comparing `cashocs-2.0.6/README.rst` & `cashocs-2.0.7/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     - `Hinze, Ulbrich, Ulbrich, and Pinnau - Optimization with PDE Constraints <https://doi.org/10.1007/978-1-4020-8839-1>`_
     - `Tröltzsch - Optimal Control of Partial Differential Equations <https://doi.org/10.1090/gsm/112>`_
 - Shape Optimization
     - `Delfour and Zolesio - Shapes and Geometries <https://doi.org/10.1137/1.9780898719826>`_
     - `Sokolowski and Zolesio - Introduction to Shape Optimization <https://doi.org/10.1007/978-3-642-58106-9>`_
 - FEniCS
     - `Logg, Mardal, and Wells - Automated Solution of Differential Equations by the Finite Element Method <https://doi.org/10.1007/978-3-642-23099-8>`_
-    - `The FEniCS demos <https://fenicsproject.org/olddocs/dolfin/2019.1.0/python/demos.html>`_
+    - `The FEniCS demos <https://fenicsproject.org/docs/dolfin/latest/python/demos.html>`_
 
 .. readme_end_disclaimer
 
 However, the `cashocs tutorial <https://cashocs.readthedocs.io/en/latest/user>`_ also gives many references either
 to the underlying theory of PDE constrained optimization or to relevant demos
 and documentation of FEniCS.
 
@@ -193,32 +193,23 @@
 
 .. readme_start_citing
 .. _citing:
 
 Citing
 ======
 
-If you use cashocs for your research, please cite the following paper
+If you use cashocs for your research, I would be grateful if you would cite the following paper
 
 .. code-block:: text
 
 	cashocs: A Computational, Adjoint-Based Shape Optimization and Optimal Control Software
 	Sebastian Blauth
 	SoftwareX, Volume 13, 2021
 	https://doi.org/10.1016/j.softx.2020.100646
 
-as well as the preprint
-
-.. code-block:: text
-
-	Version 2.0 - cashocs: A Computational, Adjoint-Based Shape Optimization and Optimal Control Software
-	Sebastian Blauth
-	https://doi.org/10.48550/arXiv.2306.09828
-
-
 Additionally, if you are using the nonlinear conjugate gradient methods for shape optimization implemented in cashocs, please cite the following paper
 	
 .. code-block:: text
 
 	Nonlinear Conjugate Gradient Methods for PDE Constrained Shape Optimization Based on Steklov--Poincaré-Type Metrics
 	Sebastian Blauth
 	SIAM Journal on Optimization, Volume 31, Issue 3, 2021
@@ -253,26 +244,14 @@
 	  issn     = {2352-7110},
 	  pages    = {100646},
 	  volume   = {13},
 	  doi      = {https://doi.org/10.1016/j.softx.2020.100646},
 	  keywords = {PDE constrained optimization, Adjoint approach, Shape optimization, Optimal control},
 	}
 
-.. code-block:: bibtex
-
-	@Misc{Blauth2023Version,
-	  author        = {Sebastian Blauth},
-	  title         = {{Version 2.0 -- cashocs: A Computational, Adjoint-Based Shape Optimization and Optimal Control Software}},
-	  year          = {2023},
-	  archiveprefix = {arXiv},
-	  eprint        = {2306.09828},
-	  primaryclass  = {math.OC},
-	}
-
-
 
 .. code-block:: bibtex
 
 	@Article{Blauth2021Nonlinear,
 		author   = {Sebastian Blauth},
 		journal  = {SIAM J. Optim.},
 		title    = {{N}onlinear {C}onjugate {G}radient {M}ethods for {PDE} {C}onstrained {S}hape {O}ptimization {B}ased on {S}teklov-{P}oincaré-{T}ype {M}etrics},
```

### Comparing `cashocs-2.0.6/cashocs/__init__.py` & `cashocs-2.0.7/cashocs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 from cashocs.io import convert
 from cashocs.io import import_mesh
 from cashocs.io import load_config
 from cashocs.nonlinear_solvers import linear_solve
 from cashocs.nonlinear_solvers import newton_solve
 from cashocs.nonlinear_solvers import picard_iteration
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 __citation__ = """
 @Article{Blauth2021cashocs,
     author   = {Sebastian Blauth},
     journal  = {SoftwareX},
     title    = {{cashocs: A Computational, Adjoint-Based Shape Optimization and
         Optimal Control Software}},
```

### Comparing `cashocs-2.0.6/cashocs/_cli/__init__.py` & `cashocs-2.0.7/cashocs/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_cli/_convert.py` & `cashocs-2.0.7/cashocs/_cli/_convert.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_constraints/__init__.py` & `cashocs-2.0.7/cashocs/_constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_constraints/constrained_problems.py` & `cashocs-2.0.7/cashocs/_constraints/constrained_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_constraints/constraints.py` & `cashocs-2.0.7/cashocs/_constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_constraints/solvers.py` & `cashocs-2.0.7/cashocs/_constraints/solvers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_database/__init__.py` & `cashocs-2.0.7/cashocs/_database/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_database/database.py` & `cashocs-2.0.7/cashocs/_database/database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_database/form_database.py` & `cashocs-2.0.7/cashocs/_database/form_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_database/function_database.py` & `cashocs-2.0.7/cashocs/_database/function_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_database/geometry_database.py` & `cashocs-2.0.7/cashocs/_database/geometry_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_database/parameter_database.py` & `cashocs-2.0.7/cashocs/_database/parameter_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_exceptions.py` & `cashocs-2.0.7/cashocs/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_forms/__init__.py` & `cashocs-2.0.7/cashocs/_forms/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_forms/control_form_handler.py` & `cashocs-2.0.7/cashocs/_forms/control_form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_forms/form_handler.py` & `cashocs-2.0.7/cashocs/_forms/form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_forms/general_form_handler.py` & `cashocs-2.0.7/cashocs/_forms/general_form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_forms/shape_form_handler.py` & `cashocs-2.0.7/cashocs/_forms/shape_form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_forms/shape_regularization.py` & `cashocs-2.0.7/cashocs/_forms/shape_regularization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_loggers.py` & `cashocs-2.0.7/cashocs/_loggers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/__init__.py` & `cashocs-2.0.7/cashocs/_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/cost_functional.py` & `cashocs-2.0.7/cashocs/_optimization/cost_functional.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/line_search/__init__.py` & `cashocs-2.0.7/cashocs/_optimization/line_search/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/line_search/armijo_line_search.py` & `cashocs-2.0.7/cashocs/_optimization/line_search/armijo_line_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from __future__ import annotations
 
 from typing import List, Optional, Tuple
 
 import fenics
 from typing_extensions import TYPE_CHECKING
 
-from cashocs import _exceptions
 from cashocs import _loggers
 from cashocs._optimization.line_search import line_search
 
 if TYPE_CHECKING:
     from cashocs import _typing
     from cashocs._database import database
     from cashocs._optimization import optimization_algorithms
@@ -121,17 +120,17 @@
             self.stepsize = (
                 self.optimization_variable_abstractions.update_optimization_variables(
                     search_direction, self.stepsize, self.beta_armijo
                 )
             )
 
             current_function_value = solver.objective_value
-            objective_step = self._compute_objective_at_new_iterate(
-                current_function_value
-            )
+
+            self.state_problem.has_solution = False
+            objective_step = self.cost_functional.evaluate()
 
             decrease_measure = self._compute_decrease_measure(search_direction)
 
             if self._satisfies_armijo_condition(
                 objective_step, current_function_value, decrease_measure
             ):
                 if self.optimization_variable_abstractions.requires_remeshing():
@@ -173,28 +172,7 @@
             return self.optimization_variable_abstractions.compute_decrease_measure(
                 search_direction
             )
         elif self.db.parameter_db.problem_type == "shape":
             return self.decrease_measure_w_o_step * self.stepsize
         else:
             return float("inf")
-
-    def _compute_objective_at_new_iterate(self, current_function_value: float) -> float:
-        """Computes the objective value for the new (trial) iterate.
-
-        Args:
-            current_function_value: The current function value.
-
-        Returns:
-            The value of the cost functional at the new iterate.
-
-        """
-        self.state_problem.has_solution = False
-        try:
-            objective_step = self.cost_functional.evaluate()
-        except (_exceptions.PETScKSPError, _exceptions.NotConvergedError) as error:
-            if self.config.getboolean("LineSearch", "fail_if_not_converged"):
-                raise error
-            else:
-                objective_step = 2.0 * abs(current_function_value)
-
-        return objective_step
```

### Comparing `cashocs-2.0.6/cashocs/_optimization/line_search/line_search.py` & `cashocs-2.0.7/cashocs/_optimization/line_search/line_search.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/line_search/polynomial_line_search.py` & `cashocs-2.0.7/cashocs/_optimization/line_search/polynomial_line_search.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimal_control/__init__.py` & `cashocs-2.0.7/cashocs/_optimization/optimal_control/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimal_control/box_constraints.py` & `cashocs-2.0.7/cashocs/_optimization/optimal_control/box_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimal_control/control_variable_abstractions.py` & `cashocs-2.0.7/cashocs/_optimization/optimal_control/control_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimal_control/optimal_control_problem.py` & `cashocs-2.0.7/cashocs/_optimization/optimal_control/optimal_control_problem.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with cashocs.  If not, see <https://www.gnu.org/licenses/>.
 
 """Optimal control problem."""
 
 from __future__ import annotations
 
-from typing import Callable, List, Optional, TYPE_CHECKING, Union
+from typing import List, Optional, TYPE_CHECKING, Union
 
 import fenics
 import numpy as np
 import ufl
 
 from cashocs import _exceptions
 from cashocs import _forms
@@ -83,16 +83,14 @@
             Union[
                 List[List[fenics.DirichletBC]],
                 List[fenics.DirichletBC],
                 fenics.DirichletBC,
             ]
         ] = None,
         preconditioner_forms: Optional[Union[List[ufl.Form], ufl.Form]] = None,
-        pre_callback: Optional[Callable] = None,
-        post_callback: Optional[Callable] = None,
     ) -> None:
         r"""Initializes self.
 
         Args:
             state_forms: The weak form of the state equation (user implemented). Can be
                 either a single UFL form, or a (ordered) list of UFL forms.
             bcs_list: The list of :py:class:`fenics.DirichletBC` objects describing
@@ -140,18 +138,14 @@
                 that `desired_weights` is `None`, no scaling is performed. Default is
                 `None`.
             control_bcs_list: A list of boundary conditions for the control variables.
                 This is passed analogously to ``bcs_list``. Default is ``None``.
             preconditioner_forms: The list of forms for the preconditioner. The default
                 is `None`, so that the preconditioner matrix is the same as the system
                 matrix.
-            pre_callback: A function (without arguments) that will be called before each
-                solve of the state system
-            post_callback: A function (without arguments) that will be called after the
-                computation of the gradient.
 
         Examples:
             Examples how to use this class can be found in the :ref:`tutorial
             <tutorial_index>`.
 
         """
         super().__init__(
@@ -163,16 +157,14 @@
             config=config,
             initial_guess=initial_guess,
             ksp_options=ksp_options,
             adjoint_ksp_options=adjoint_ksp_options,
             gradient_ksp_options=gradient_ksp_options,
             desired_weights=desired_weights,
             preconditioner_forms=preconditioner_forms,
-            pre_callback=pre_callback,
-            post_callback=post_callback,
         )
 
         self.db.function_db.controls = _utils.enlist(controls)
 
         self.db.parameter_db.control_dim = len(self.db.function_db.controls)
         self.db.function_db.control_spaces = [
             x.function_space() for x in self.db.function_db.controls
```

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/__init__.py` & `cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/callback.py` & `cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/callback.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/gradient_descent.py` & `cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/l_bfgs.py` & `cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/l_bfgs.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/ncg.py` & `cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/ncg.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/newton.py` & `cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/newton.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py` & `cashocs-2.0.7/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimization_problem.py` & `cashocs-2.0.7/cashocs/_optimization/optimization_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,16 +100,14 @@
         gradient_ksp_options: Optional[
             Union[_typing.KspOption, List[_typing.KspOption]]
         ] = None,
         desired_weights: Optional[List[float]] = None,
         temp_dict: Optional[Dict] = None,
         initial_function_values: Optional[List[float]] = None,
         preconditioner_forms: Optional[Union[List[ufl.Form], ufl.Form]] = None,
-        pre_callback: Optional[Callable] = None,
-        post_callback: Optional[Callable] = None,
     ) -> None:
         r"""Initializes self.
 
         Args:
             state_forms: The weak form of the state equation (user implemented). Can be
                 either a single UFL form, or a (ordered) list of UFL forms.
             bcs_list: The list of :py:class:`fenics.DirichletBC` objects describing
@@ -152,18 +150,14 @@
                 Using this parameter may result in unintended side effects.
             initial_function_values: This is a privatve parameter of the class, required
                 for remeshing. This parameter must not be set by the user and should be
                 ignored. Using this parameter may result in unintended side effects.
             preconditioner_forms: The list of forms for the preconditioner. The default
                 is `None`, so that the preconditioner matrix is the same as the system
                 matrix.
-            pre_callback: A function (without arguments) that will be called before each
-                solve of the state system
-            post_callback: A function (without arguments) that will be called after the
-                computation of the gradient.
 
         Notes:
             If one uses a single PDE constraint, the inputs can be the objects
             (UFL forms, functions, etc.) directly. In case multiple PDE constraints
             are present the inputs have to be put into (ordered) lists. The order of
             the objects depends on the order of the state variables, so that
             ``state_forms[i]`` is the weak form of the PDE for ``states[i]`` with
@@ -222,18 +216,14 @@
             self.adjoint_ksp_options,
             self.gradient_ksp_options,
             self.cost_functional_list,
             self.state_forms,
             self.bcs_list,
             self.preconditioner_forms,
         )
-
-        self.db.callback.pre_callback = pre_callback
-        self.db.callback.post_callback = post_callback
-
         if temp_dict is not None:
             self.db.parameter_db.temp_dict.update(temp_dict)
             self.db.parameter_db.is_remeshed = True
 
         self.general_form_handler = _forms.GeneralFormHandler(self.db)
         self.state_problem = _pde_problems.StateProblem(
             self.db,
```

### Comparing `cashocs-2.0.6/cashocs/_optimization/optimization_variable_abstractions.py` & `cashocs-2.0.7/cashocs/_optimization/optimization_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/shape_optimization/__init__.py` & `cashocs-2.0.7/cashocs/_optimization/shape_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/shape_optimization/shape_optimization_problem.py` & `cashocs-2.0.7/cashocs/_optimization/shape_optimization/shape_optimization_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,14 @@
         gradient_ksp_options: Optional[
             Union[_typing.KspOption, List[_typing.KspOption]]
         ] = None,
         desired_weights: Optional[List[float]] = None,
         temp_dict: Optional[Dict] = None,
         initial_function_values: Optional[List[float]] = None,
         preconditioner_forms: Optional[Union[List[ufl.Form], ufl.Form]] = None,
-        pre_callback: Optional[Callable] = None,
-        post_callback: Optional[Callable] = None,
     ) -> None:
         """Initializes self.
 
         Args:
             state_forms: The weak form of the state equation (user implemented). Can be
                 either a single UFL form, or a (ordered) list of UFL forms.
             bcs_list: The list of :py:class:`fenics.DirichletBC` objects describing
@@ -150,18 +148,14 @@
                 Using this parameter may result in unintended side effects.
             initial_function_values: This is a privatve parameter of the class, required
                 for remeshing. This parameter must not be set by the user and should be
                 ignored. Using this parameter may result in unintended side effects.
             preconditioner_forms: The list of forms for the preconditioner. The default
                 is `None`, so that the preconditioner matrix is the same as the system
                 matrix.
-            pre_callback: A function (without arguments) that will be called before each
-                solve of the state system
-            post_callback: A function (without arguments) that will be called after the
-                computation of the gradient.
 
         """
         super().__init__(
             state_forms,
             bcs_list,
             cost_functional_form,
             states,
@@ -171,16 +165,14 @@
             ksp_options=ksp_options,
             adjoint_ksp_options=adjoint_ksp_options,
             gradient_ksp_options=gradient_ksp_options,
             desired_weights=desired_weights,
             temp_dict=temp_dict,
             initial_function_values=initial_function_values,
             preconditioner_forms=preconditioner_forms,
-            pre_callback=pre_callback,
-            post_callback=post_callback,
         )
 
         if shape_scalar_product is None:
             deformation_space: fenics.FunctionSpace = fenics.VectorFunctionSpace(
                 self.db.geometry_db.mesh, "CG", 1
             )
         else:
```

### Comparing `cashocs-2.0.6/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py` & `cashocs-2.0.7/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/topology_optimization/__init__.py` & `cashocs-2.0.7/cashocs/_optimization/topology_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py` & `cashocs-2.0.7/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py` & `cashocs-2.0.7/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/topology_optimization/topology_optimization_problem.py` & `cashocs-2.0.7/cashocs/_optimization/topology_optimization/topology_optimization_problem.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,16 +77,14 @@
             Union[_typing.KspOption, List[_typing.KspOption]]
         ] = None,
         gradient_ksp_options: Optional[
             Union[_typing.KspOption, List[_typing.KspOption]]
         ] = None,
         desired_weights: list[float] | None = None,
         preconditioner_forms: Optional[Union[List[ufl.Form], ufl.Form]] = None,
-        pre_callback: Optional[Callable] = None,
-        post_callback: Optional[Callable] = None,
     ) -> None:
         r"""Initializes the topology optimization problem.
 
         Args:
             state_forms: The weak form of the state equation (user implemented). Can be
                 either a single UFL form, or a (ordered) list of UFL forms.
             bcs_list: The list of :py:class:`fenics.DirichletBC` objects describing
@@ -134,18 +132,14 @@
                 summands. The individual terms are then scaled, so that term `i` has the
                 magnitude of `desired_weights[i]` for the initial iteration. In case
                 that `desired_weights` is `None`, no scaling is performed. Default is
                 `None`.
             preconditioner_forms: The list of forms for the preconditioner. The default
                 is `None`, so that the preconditioner matrix is the same as the system
                 matrix.
-            pre_callback: A function (without arguments) that will be called before each
-                solve of the state system
-            post_callback: A function (without arguments) that will be called after the
-                computation of the gradient.
 
         """
         super().__init__(
             state_forms,
             bcs_list,
             cost_functional_form,
             states,
@@ -153,16 +147,14 @@
             config=config,
             initial_guess=initial_guess,
             ksp_options=ksp_options,
             adjoint_ksp_options=adjoint_ksp_options,
             gradient_ksp_options=gradient_ksp_options,
             desired_weights=desired_weights,
             preconditioner_forms=preconditioner_forms,
-            pre_callback=pre_callback,
-            post_callback=post_callback,
         )
 
         self.db.parameter_db.problem_type = "topology"
         self.mesh_parametrization = None
 
         self.levelset_function = levelset_function
         self.topological_derivative_pos = topological_derivative_pos
```

### Comparing `cashocs-2.0.6/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py` & `cashocs-2.0.7/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_optimization/verification.py` & `cashocs-2.0.7/cashocs/_optimization/verification.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_pde_problems/__init__.py` & `cashocs-2.0.7/cashocs/_pde_problems/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_pde_problems/adjoint_problem.py` & `cashocs-2.0.7/cashocs/_pde_problems/adjoint_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_pde_problems/control_gradient_problem.py` & `cashocs-2.0.7/cashocs/_pde_problems/control_gradient_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_pde_problems/hessian_problems.py` & `cashocs-2.0.7/cashocs/_pde_problems/hessian_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_pde_problems/pde_problem.py` & `cashocs-2.0.7/cashocs/_pde_problems/pde_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_pde_problems/shape_gradient_problem.py` & `cashocs-2.0.7/cashocs/_pde_problems/shape_gradient_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_pde_problems/state_problem.py` & `cashocs-2.0.7/cashocs/_pde_problems/state_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_typing.py` & `cashocs-2.0.7/cashocs/_typing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_utils/__init__.py` & `cashocs-2.0.7/cashocs/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_utils/forms.py` & `cashocs-2.0.7/cashocs/_utils/forms.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_utils/helpers.py` & `cashocs-2.0.7/cashocs/_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_utils/interpolations.py` & `cashocs-2.0.7/cashocs/_utils/interpolations.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/_utils/linalg.py` & `cashocs-2.0.7/cashocs/_utils/linalg.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/geometry/__init__.py` & `cashocs-2.0.7/cashocs/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/geometry/boundary_distance.py` & `cashocs-2.0.7/cashocs/geometry/boundary_distance.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/geometry/deformations.py` & `cashocs-2.0.7/cashocs/geometry/deformations.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/geometry/measure.py` & `cashocs-2.0.7/cashocs/geometry/measure.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/geometry/mesh.py` & `cashocs-2.0.7/cashocs/geometry/mesh.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/geometry/mesh_handler.py` & `cashocs-2.0.7/cashocs/geometry/mesh_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/geometry/mesh_testing.py` & `cashocs-2.0.7/cashocs/geometry/mesh_testing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/geometry/quality.py` & `cashocs-2.0.7/cashocs/geometry/quality.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/io/__init__.py` & `cashocs-2.0.7/cashocs/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/io/config.py` & `cashocs-2.0.7/cashocs/io/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,17 +220,14 @@
                     "attributes": ["less_than_one", "positive"],
                 },
                 "factor_high": {
                     "type": "float",
                     "attributes": ["less_than_one", "positive"],
                     "larger_than": ("LineSearch", "factor_low"),
                 },
-                "fail_if_not_converged": {
-                    "type": "bool",
-                },
             },
             "AlgoLBFGS": {
                 "bfgs_memory_size": {
                     "type": "int",
                     "attributes": ["non_negative"],
                 },
                 "use_bfgs_scaling": {
@@ -559,15 +556,14 @@
 epsilon_armijo = 1e-4
 beta_armijo = 2.0
 initial_stepsize = 1.0
 safeguard_stepsize = True
 polynomial_model = cubic
 factor_high = 0.5
 factor_low = 0.1
-fail_if_not_converged = False
 
 [ShapeGradient]
 lambda_lame = 0.0
 damping_factor = 0.0
 inhomogeneous = False
 mu_def = 1.0
 mu_fix = 1.0
```

### Comparing `cashocs-2.0.6/cashocs/io/function.py` & `cashocs-2.0.7/cashocs/io/function.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/io/managers.py` & `cashocs-2.0.7/cashocs/io/managers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/io/mesh.py` & `cashocs-2.0.7/cashocs/io/mesh.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/io/output.py` & `cashocs-2.0.7/cashocs/io/output.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/nonlinear_solvers/__init__.py` & `cashocs-2.0.7/cashocs/nonlinear_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/nonlinear_solvers/linear_solver.py` & `cashocs-2.0.7/cashocs/nonlinear_solvers/linear_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/nonlinear_solvers/newton_solver.py` & `cashocs-2.0.7/cashocs/nonlinear_solvers/newton_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/nonlinear_solvers/picard_solver.py` & `cashocs-2.0.7/cashocs/nonlinear_solvers/picard_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/space_mapping/__init__.py` & `cashocs-2.0.7/cashocs/space_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/space_mapping/optimal_control.py` & `cashocs-2.0.7/cashocs/space_mapping/optimal_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs/space_mapping/shape_optimization.py` & `cashocs-2.0.7/cashocs/space_mapping/shape_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/cashocs.egg-info/PKG-INFO` & `cashocs-2.0.7/cashocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: cashocs
-Version: 2.0.6
+Version: 2.0.7
 Summary: Computational Adjoint-Based Shape Optimization and Optimal Control Software
 Author: Sebastian Blauth
 Author-email: sebastian.blauth@itwm.fraunhofer.de
 License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: Documentation, https://cashocs.readthedocs.io/en/stable
+Project-URL: Documentation, https://cashocs.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/sblauth/cashocs
-Project-URL: Tutorial, https://cashocs.readthedocs.io/en/stable/user
+Project-URL: Tutorial, https://cashocs.readthedocs.io/en/latest/user
 Project-URL: Tracker, https://github.com/sblauth/cashocs/issues
 Keywords: Shape Optimization,Optimal Control,FEniCS,Optimization,PDE,Adjoint,Finite Element Method
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -98,15 +98,15 @@
     - `Hinze, Ulbrich, Ulbrich, and Pinnau - Optimization with PDE Constraints <https://doi.org/10.1007/978-1-4020-8839-1>`_
     - `Tröltzsch - Optimal Control of Partial Differential Equations <https://doi.org/10.1090/gsm/112>`_
 - Shape Optimization
     - `Delfour and Zolesio - Shapes and Geometries <https://doi.org/10.1137/1.9780898719826>`_
     - `Sokolowski and Zolesio - Introduction to Shape Optimization <https://doi.org/10.1007/978-3-642-58106-9>`_
 - FEniCS
     - `Logg, Mardal, and Wells - Automated Solution of Differential Equations by the Finite Element Method <https://doi.org/10.1007/978-3-642-23099-8>`_
-    - `The FEniCS demos <https://fenicsproject.org/olddocs/dolfin/2019.1.0/python/demos.html>`_
+    - `The FEniCS demos <https://fenicsproject.org/docs/dolfin/latest/python/demos.html>`_
 
 .. readme_end_disclaimer
 
 However, the `cashocs tutorial <https://cashocs.readthedocs.io/en/latest/user>`_ also gives many references either
 to the underlying theory of PDE constrained optimization or to relevant demos
 and documentation of FEniCS.
 
@@ -228,32 +228,23 @@
 
 .. readme_start_citing
 .. _citing:
 
 Citing
 ======
 
-If you use cashocs for your research, please cite the following paper
+If you use cashocs for your research, I would be grateful if you would cite the following paper
 
 .. code-block:: text
 
 	cashocs: A Computational, Adjoint-Based Shape Optimization and Optimal Control Software
 	Sebastian Blauth
 	SoftwareX, Volume 13, 2021
 	https://doi.org/10.1016/j.softx.2020.100646
 
-as well as the preprint
-
-.. code-block:: text
-
-	Version 2.0 - cashocs: A Computational, Adjoint-Based Shape Optimization and Optimal Control Software
-	Sebastian Blauth
-	https://doi.org/10.48550/arXiv.2306.09828
-
-
 Additionally, if you are using the nonlinear conjugate gradient methods for shape optimization implemented in cashocs, please cite the following paper
 	
 .. code-block:: text
 
 	Nonlinear Conjugate Gradient Methods for PDE Constrained Shape Optimization Based on Steklov--Poincaré-Type Metrics
 	Sebastian Blauth
 	SIAM Journal on Optimization, Volume 31, Issue 3, 2021
@@ -288,26 +279,14 @@
 	  issn     = {2352-7110},
 	  pages    = {100646},
 	  volume   = {13},
 	  doi      = {https://doi.org/10.1016/j.softx.2020.100646},
 	  keywords = {PDE constrained optimization, Adjoint approach, Shape optimization, Optimal control},
 	}
 
-.. code-block:: bibtex
-
-	@Misc{Blauth2023Version,
-	  author        = {Sebastian Blauth},
-	  title         = {{Version 2.0 -- cashocs: A Computational, Adjoint-Based Shape Optimization and Optimal Control Software}},
-	  year          = {2023},
-	  archiveprefix = {arXiv},
-	  eprint        = {2306.09828},
-	  primaryclass  = {math.OC},
-	}
-
-
 
 .. code-block:: bibtex
 
 	@Article{Blauth2021Nonlinear,
 		author   = {Sebastian Blauth},
 		journal  = {SIAM J. Optim.},
 		title    = {{N}onlinear {C}onjugate {G}radient {M}ethods for {PDE} {C}onstrained {S}hape {O}ptimization {B}ased on {S}teklov-{P}oincaré-{T}ype {M}etrics},
```

### Comparing `cashocs-2.0.6/cashocs.egg-info/SOURCES.txt` & `cashocs-2.0.7/cashocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py` & `cashocs-2.0.7/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py` & `cashocs-2.0.7/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/misc/xdmf_io/demo_xdmf_io.py` & `cashocs-2.0.7/demos/documented/misc/xdmf_io/demo_xdmf_io.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/box_constraints/demo_box_constraints.py` & `cashocs-2.0.7/demos/documented/optimal_control/box_constraints/demo_box_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
 # To check that the box constraints are actually satisfied by our solution, we perform
 # an assertion
 
 # +
 import numpy as np
 
-assert np.all(u_a.vector()[:] <= u.vector()[:]) and np.all(
+assert np.alltrue(u_a.vector()[:] <= u.vector()[:]) and np.alltrue(
     u.vector()[:] <= u_b.vector()[:]
 )
 # -
 
 # which shows that they are indeed satisfied. The visualization is carried out
 # analogously to before, via
```

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/constraints/demo_constraints.py` & `cashocs-2.0.7/demos/documented/optimal_control/constraints/demo_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py` & `cashocs-2.0.7/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py` & `cashocs-2.0.7/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/heat_equation/demo_heat_equation.py` & `cashocs-2.0.7/demos/documented/optimal_control/heat_equation/demo_heat_equation.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py` & `cashocs-2.0.7/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py` & `cashocs-2.0.7/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py` & `cashocs-2.0.7/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/neumann_control/demo_neumann_control.py` & `cashocs-2.0.7/demos/documented/optimal_control/neumann_control/demo_neumann_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py` & `cashocs-2.0.7/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py` & `cashocs-2.0.7/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/poisson/demo_poisson.py` & `cashocs-2.0.7/demos/documented/optimal_control/poisson/demo_poisson.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py` & `cashocs-2.0.7/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,60 +138,49 @@
         - q * div(u) * dx
         - inner(c, v) * dx
     )
     cashocs.newton_solve(e, up, bcs, verbose=False)
 
 
 # where we solve the Navier-Stokes equations with a lower Reynolds number of
-# {python}`Re / 10.0`. Later on, we use this function as keyword argument for defining
-# the optimization problem.
+# {python}`Re / 10.0`. Later on, we inject this {python}`pre_callback` into cashocs by
+# using the
+# {py:meth}`inject_pre_callback <cashocs.OptimalControlProblem.inject_pre_callback>`
+# method.
 #
 # Additionally, cashocs implements the functionality of also performing a pre-defined
 # action after each gradient computation, given by a so-called {python}`post_callback`.
 # In our case, we just want to print a statement so that we can visualize what is
 # happening. Therefore, we define our {python}`post_callback` as
 
 
 def post_callback():
     print("Performing an action after computing the gradient.")
 
 
-# Next, we define the optimization and use the keyword arguments to define the callbacks
-# via
+# Next, before we can inject these two callbacks, we first have to define the optimal
+# control problem
 
-ocp = cashocs.OptimalControlProblem(
-    e,
-    bcs,
-    J,
-    up,
-    c,
-    vq,
-    config=config,
-    pre_callback=pre_callback,
-    post_callback=post_callback,
-)
+ocp = cashocs.OptimalControlProblem(e, bcs, J, up, c, vq, config=config)
+
+# Finally, we can inject both hooks via
+
+ocp.inject_pre_callback(pre_callback)
+ocp.inject_post_callback(post_callback)
 
 # ::::{note}
-# Alternatively, the pre- and post-callbacks can be injected to an already defined
-# optimization problem with the code
-#
-# :::{code-block} python
-# ocp.inject_pre_callback(pre_callback)
-# ocp.inject_post_callback(post_callback)
-# :::
-#
-# or, equivalently,
-#
+# We can also save one line and use the code
 # :::{code-block} python
 # ocp.inject_pre_post_hook(pre_hook, post_hook)
 # :::
 #
+# which is equivalent to the above two lines.
 # ::::
-
-# In the end, we solve the problem with
+#
+# And in the end, we solve the problem with
 
 ocp.solve()
 
 # We visualize the results with the lines
 
 # +
 u, p = up.split(True)
```

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py` & `cashocs-2.0.7/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/sparse_control/demo_sparse_control.py` & `cashocs-2.0.7/demos/documented/optimal_control/sparse_control/demo_sparse_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/state_constraints/demo_state_constraints.py` & `cashocs-2.0.7/demos/documented/optimal_control/state_constraints/demo_state_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/optimal_control/stokes/demo_stokes.py` & `cashocs-2.0.7/demos/documented/optimal_control/stokes/demo_stokes.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py` & `cashocs-2.0.7/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py` & `cashocs-2.0.7/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py` & `cashocs-2.0.7/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py` & `cashocs-2.0.7/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/shape_optimization/regularization/demo_regularization.py` & `cashocs-2.0.7/demos/documented/shape_optimization/regularization/demo_regularization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/shape_optimization/remeshing/demo_remeshing.py` & `cashocs-2.0.7/demos/documented/shape_optimization/remeshing/demo_remeshing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/shape_optimization/scaling/demo_scaling.py` & `cashocs-2.0.7/demos/documented/shape_optimization/scaling/demo_scaling.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py` & `cashocs-2.0.7/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py` & `cashocs-2.0.7/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py` & `cashocs-2.0.7/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py` & `cashocs-2.0.7/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/test.py` & `cashocs-2.0.7/demos/test.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/test_mpi.py` & `cashocs-2.0.7/demos/test_mpi.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py` & `cashocs-2.0.7/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py` & `cashocs-2.0.7/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/undocumented/shape_optimization/custom_functional/custom_functional.py` & `cashocs-2.0.7/demos/undocumented/shape_optimization/custom_functional/custom_functional.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py` & `cashocs-2.0.7/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/docs/source/conf.py` & `cashocs-2.0.7/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "cashocs"
 copyright = "2020-2023, Sebastian Blauth"
 author = "Sebastian Blauth"
 
 # The full version, including alpha/beta/rc tags
-release = "2.0.6"
+release = "2.0.7"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `cashocs-2.0.6/docs/source/jupytext_process.py` & `cashocs-2.0.7/docs/source/jupytext_process.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/pyproject.toml` & `cashocs-2.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cashocs"
-version = "2.0.6"
+version = "2.0.7"
 description = "Computational Adjoint-Based Shape Optimization and Optimal Control Software"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "GNU General Public License v3 or later (GPLv3+)"}
 authors = [
 	{name = "Sebastian Blauth"},
 	{email = "sebastian.blauth@itwm.fraunhofer.de"}
@@ -45,17 +45,17 @@
 dependencies = [
 	"meshio >= 4.1.0",
 	"numpy",
 	"typing_extensions"
 ]
 
 [project.urls]
-Documentation = "https://cashocs.readthedocs.io/en/stable"
+Documentation = "https://cashocs.readthedocs.io/en/latest"
 Source = "https://github.com/sblauth/cashocs"
-Tutorial = "https://cashocs.readthedocs.io/en/stable/user"
+Tutorial = "https://cashocs.readthedocs.io/en/latest/user"
 Tracker = "https://github.com/sblauth/cashocs/issues"
 
 [project.scripts]
 cashocs-convert = "cashocs._cli:convert"
 
 [project.optional-dependencies]
 tests = [
```

### Comparing `cashocs-2.0.6/tests/conftest.py` & `cashocs-2.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_cli.py` & `cashocs-2.0.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_config.py` & `cashocs-2.0.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_control_constraints.py` & `cashocs-2.0.7/tests/test_control_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_exceptions.py` & `cashocs-2.0.7/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_geometry.py` & `cashocs-2.0.7/tests/test_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,19 +119,19 @@
     c_coords = gather_coordinates(regular_mesh)
     r_coords = gather_coordinates(r_mesh)
     s_coords = gather_coordinates(s_mesh)
 
     if fenics.MPI.rank(fenics.MPI.comm_world) == 0:
         assert np.allclose(c_coords, u_coords)
 
-        assert np.all((np.max(r_coords, axis=0) - lens) < 1e-14)
-        assert np.all((np.min(r_coords, axis=0) - np.array([0, 0])) < 1e-14)
+        assert np.alltrue((np.max(r_coords, axis=0) - lens) < 1e-14)
+        assert np.alltrue((np.min(r_coords, axis=0) - np.array([0, 0])) < 1e-14)
 
-        assert np.all(abs(np.max(s_coords, axis=0) - max_vals) < 1e-14)
-        assert np.all(abs(np.min(s_coords, axis=0) - min_vals) < 1e-14)
+        assert np.alltrue(abs(np.max(s_coords, axis=0) - max_vals) < 1e-14)
+        assert np.alltrue(abs(np.min(s_coords, axis=0) - min_vals) < 1e-14)
     fenics.MPI.barrier(fenics.MPI.comm_world)
 
     t_mesh, _, _, _, _, _ = cashocs.regular_box_mesh(
         2, start_x=0.0, end_x=lens[0], start_y=0.0, end_y=lens[1]
     )
     t_coords = gather_coordinates(t_mesh)
```

### Comparing `cashocs-2.0.6/tests/test_log_level.py` & `cashocs-2.0.7/tests/test_log_level.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_nonlinear_solvers.py` & `cashocs-2.0.7/tests/test_nonlinear_solvers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_optimal_control.py` & `cashocs-2.0.7/tests/test_optimal_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,46 +198,46 @@
     ocp.solve(algorithm="newton", rtol=1e-2, atol=0.0, max_iter=2)
     assert ocp.solver.relative_norm <= 1e-6
 
 
 def test_control_gd_cc(ocp_cc, cc):
     ocp_cc.solve(algorithm="gd", rtol=1e-2, atol=0.0, max_iter=22)
     assert ocp_cc.solver.relative_norm <= ocp_cc.solver.rtol
-    assert np.all(ocp_cc.db.function_db.controls[0].vector()[:] >= cc[0])
-    assert np.all(ocp_cc.db.function_db.controls[0].vector()[:] <= cc[1])
+    assert np.alltrue(ocp_cc.db.function_db.controls[0].vector()[:] >= cc[0])
+    assert np.alltrue(ocp_cc.db.function_db.controls[0].vector()[:] <= cc[1])
 
 
 @pytest.fixture
 def set_cg_tolerances_constrained(config_ocp):
     cg_method = config_ocp.get("AlgoCG", "cg_method")
     iterations = {"FR": "47", "PR": "24", "HS": "30", "DY": "9", "HZ": "37"}
     config_ocp.set("OptimizationRoutine", "max_iter", iterations[cg_method])
 
 
 def test_conjugate_gradient_solver_constrained(
     setup_cg_method, set_cg_tolerances_constrained, ocp_cc, cc
 ):
     ocp_cc.solve(algorithm="ncg", rtol=1e-2, atol=0.0)
     assert ocp_cc.solver.relative_norm <= ocp_cc.solver.rtol
-    assert np.all(ocp_cc.db.function_db.controls[0].vector()[:] >= cc[0])
-    assert np.all(ocp_cc.db.function_db.controls[0].vector()[:] <= cc[1])
+    assert np.alltrue(ocp_cc.db.function_db.controls[0].vector()[:] >= cc[0])
+    assert np.alltrue(ocp_cc.db.function_db.controls[0].vector()[:] <= cc[1])
 
 
 def test_control_lbfgs_cc(ocp_cc, cc):
     ocp_cc.solve(algorithm="bfgs", rtol=1e-2, atol=0.0, max_iter=11)
     assert ocp_cc.solver.relative_norm <= ocp_cc.solver.rtol
-    assert np.all(ocp_cc.db.function_db.controls[0].vector()[:] >= cc[0])
-    assert np.all(ocp_cc.db.function_db.controls[0].vector()[:] <= cc[1])
+    assert np.alltrue(ocp_cc.db.function_db.controls[0].vector()[:] >= cc[0])
+    assert np.alltrue(ocp_cc.db.function_db.controls[0].vector()[:] <= cc[1])
 
 
 def test_newton_solver_constrained(setup_newton_method, ocp_cc, cc):
     ocp_cc.solve(algorithm="newton", rtol=1e-2, atol=0.0, max_iter=9)
     assert ocp_cc.solver.relative_norm <= ocp_cc.solver.rtol
-    assert np.all(ocp_cc.db.function_db.controls[0].vector()[:] >= cc[0])
-    assert np.all(ocp_cc.db.function_db.controls[0].vector()[:] <= cc[1])
+    assert np.alltrue(ocp_cc.db.function_db.controls[0].vector()[:] >= cc[0])
+    assert np.alltrue(ocp_cc.db.function_db.controls[0].vector()[:] <= cc[1])
 
 
 def test_custom_supply_control(CG1, geometry, y, u, p, y_d, rng, bcs, ocp):
     adjoint_form = (
         inner(grad(p), grad(TestFunction(CG1))) * geometry.dx
         - (y - y_d) * TestFunction(CG1) * geometry.dx
     )
```

### Comparing `cashocs-2.0.6/tests/test_optimal_control_multiple.py` & `cashocs-2.0.7/tests/test_optimal_control_multiple.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_optimal_control_space_mapping.py` & `cashocs-2.0.7/tests/test_optimal_control_space_mapping.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_output.py` & `cashocs-2.0.7/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_p_laplacian.py` & `cashocs-2.0.7/tests/test_p_laplacian.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_pde_problems.py` & `cashocs-2.0.7/tests/test_pde_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_picard_iterations.py` & `cashocs-2.0.7/tests/test_picard_iterations.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_remeshing.py` & `cashocs-2.0.7/tests/test_remeshing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_shape_constraints.py` & `cashocs-2.0.7/tests/test_shape_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_shape_optimization.py` & `cashocs-2.0.7/tests/test_shape_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,23 +166,23 @@
     offset = rng.rand(2)
     trafo = interpolate(Constant(offset), V)
     sop.mesh_handler.move_mesh(trafo)
 
     deformed_coordinates = np.zeros(initial_coordinates.shape)
     deformed_coordinates[:, 0] = initial_coordinates[:, 0] + offset[0]
     deformed_coordinates[:, 1] = initial_coordinates[:, 1] + offset[1]
-    assert np.all(abs(mesh.coordinates()[:, :] - deformed_coordinates) < 1e-15)
+    assert np.alltrue(abs(mesh.coordinates()[:, :] - deformed_coordinates) < 1e-15)
 
     sop.mesh_handler.revert_transformation()
-    assert np.all(abs(mesh.coordinates()[:, :] - initial_coordinates) < 1e-15)
+    assert np.alltrue(abs(mesh.coordinates()[:, :] - initial_coordinates) < 1e-15)
 
     trafo.vector().set_local(rng.uniform(-1e3, 1e3, size=trafo.vector().local_size()))
     trafo.vector().apply("")
     sop.mesh_handler.move_mesh(trafo)
-    assert np.all(abs(mesh.coordinates()[:, :] - initial_coordinates) < 1e-15)
+    assert np.alltrue(abs(mesh.coordinates()[:, :] - initial_coordinates) < 1e-15)
 
 
 def test_shape_derivative_unconstrained(
     config_sop, geometry, state_function, adjoint_function, state_form, bcs_list
 ):
     mesh = geometry.mesh
     dx = geometry.dx
```

### Comparing `cashocs-2.0.6/tests/test_shape_optimization_space_mapping.py` & `cashocs-2.0.7/tests/test_shape_optimization_space_mapping.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_topology_optimization.py` & `cashocs-2.0.7/tests/test_topology_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.6/tests/test_utils.py` & `cashocs-2.0.7/tests/test_utils.py`

 * *Files identical despite different names*

